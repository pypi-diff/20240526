# Comparing `tmp/maestro_compose-0.1.2.tar.gz` & `tmp/maestro_compose-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro_compose-0.1.2.tar", max compression
+gzip compressed data, was "maestro_compose-0.1.3.tar", max compression
```

## Comparing `maestro_compose-0.1.2.tar` & `maestro_compose-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0        9 2024-05-25 23:28:35.104821 maestro_compose-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-25 23:20:44.277925 maestro_compose-0.1.2/maestro_compose/__init__.py
--rw-r--r--   0        0        0     5844 2024-05-25 23:29:56.483183 maestro_compose-0.1.2/maestro_compose/__main__.py
--rw-r--r--   0        0        0      765 2024-05-25 23:49:59.398906 maestro_compose-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 maestro_compose-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        9 2024-05-25 23:28:35.104821 maestro_compose-0.1.3/README.md
+-rw-r--r--   0        0        0       57 2024-05-26 00:57:34.299753 maestro_compose-0.1.3/maestro_compose/__init__.py
+-rw-r--r--   0        0        0     6325 2024-05-26 00:57:09.483656 maestro_compose-0.1.3/maestro_compose/__main__.py
+-rw-r--r--   0        0        0     1330 2024-05-26 00:57:34.299139 maestro_compose-0.1.3/maestro_compose/models.py
+-rw-r--r--   0        0        0      765 2024-05-26 00:57:56.189519 maestro_compose-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 maestro_compose-0.1.3/PKG-INFO
```

### Comparing `maestro_compose-0.1.2/maestro_compose/__main__.py` & `maestro_compose-0.1.3/maestro_compose/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,85 +1,55 @@
 import json
-import socket
 import subprocess
 from pathlib import Path
 
 import click
 import yaml
-from pydantic import BaseModel, Field, ValidationError, model_validator
+from pydantic import ValidationError
 
-CONFIG_NAME = "maestro-config.yaml"
-TARGET_NAME = "maestro-target.yaml"
+from .models import MaestroConfig, MaestroTarget
+
+TARGET_NAME = "maestro.yaml"
 TARGET_DIR = "."
 APPLICATIONS_DIR = "applications"
-
-
-class MaestroConfig(BaseModel):
-    enabled: bool
-    priority: int = 100
-    hosts: list[str] = Field(default_factory=list)
-    tags: list[str] = Field(default_factory=list)
-
-    @model_validator(mode="after")
-    def check_hosts(self):
-        if not self.hosts:
-            self.hosts = [socket.gethostname()]
-        return self
-
-
-class MaestroTarget(BaseModel):
-    hosts_include: list
-    hosts_exclude: list[str] = Field(default_factory=list)
-    tags_include: list[str] = Field(default_factory=list)
-    tags_exclude: list[str] = Field(default_factory=list)
-
-    @model_validator(mode="after")
-    def check_hosts(self):
-        for i, host in enumerate(self.hosts_include):
-            self.hosts_include[i] = self.replace_template(template=host)
-        for i, host in enumerate(self.hosts_exclude):
-            self.hosts_exclude[i] = self.replace_template(template=host)
-        return self
-
-    def replace_template(self, template: str) -> str:
-        if template.startswith("$"):
-            if template == "$current":
-                return socket.gethostname()
-            elif template == "$all":
-                return "$all"
-            else:
-                raise ValueError(f"Template {template} not supported.")
-        return template
+DOCKER_COMPOSE_FILES = ["docker-compose.yaml", "docker-compose.yml"]
 
 
 def load_target(root_dir: Path, target_name: str = TARGET_NAME) -> MaestroTarget:
     params_path = root_dir / target_name
     params_yaml = yaml.safe_load(params_path.read_text())
     return MaestroTarget(**params_yaml)
 
 
-def load_config(app_dir: Path, config_name: str = CONFIG_NAME) -> MaestroConfig:
-    config_path = app_dir / config_name
-    config_yaml = yaml.safe_load(config_path.read_text())
-    try:
-        return MaestroConfig(**config_yaml)
-    except ValidationError as e:
-        print(f"Validation error in {app_dir}/{config_name}: {e}")
-        return None
+def load_config(app_dir: Path) -> MaestroConfig:
+    for compose_file in DOCKER_COMPOSE_FILES:
+        try:
+            config_path = app_dir / compose_file
+            compose_yaml = yaml.safe_load(config_path.read_text())
+            maestro_labels = get_maestro_labels(compose_yaml=compose_yaml)
+            try:
+                return MaestroConfig(**maestro_labels)
+            except ValidationError as e:
+                print(f"Validation error in {app_dir}/{compose_file}: {e}")
+                return None
+        except FileNotFoundError:
+            pass
+    print(f"No docker-compose file found in {app_dir}")
+    return None
 
 
 def get_applications(base_dir: Path, target: MaestroTarget):
     apps = []
     for app_dir in base_dir.iterdir():
-        if app_dir.is_dir() and (app_dir / CONFIG_NAME).exists():
+        if app_dir.is_dir():
             config = load_config(app_dir)
             # print(config)
 
             # Maestro config exists and enabled
-            if config and config.enabled:
+            if config and config.enable:
                 # Check host match
 
                 if (
                     not "$all" in target.hosts_include
                     and (not any(host in config.hosts for host in target.hosts_include))
                     or (any(host in config.hosts for host in target.hosts_exclude))
                 ):
@@ -95,80 +65,117 @@
                     continue
 
                 apps.append((app_dir, config))
     apps.sort(key=lambda x: x[1].priority)
     return apps
 
 
+def get_maestro_labels(compose_yaml: dict, maestro_key: str = "maestro."):
+    maestro_labels = {}
+    for data in compose_yaml["services"].values():
+        if "labels" in data.keys():
+            for label in data["labels"]:
+                if isinstance(label, dict):
+                    if any(maestro_key in k for k in label.keys()):
+                        maestro_labels.update(label)
+                elif isinstance(label, str):
+                    k, v = label.split("=")
+                    if maestro_key in k:
+                        maestro_labels[k] = v
+                else:
+                    raise ValueError(f"Label {label} in unsupported format")
+    maestro_labels = {k.replace(maestro_key, ""): v for k, v in maestro_labels.items()}
+    if "tags" in maestro_labels:
+        maestro_labels["tags"] = maestro_labels["tags"].split(",")
+    if "hosts" in maestro_labels:
+        maestro_labels["hosts"] = maestro_labels["hosts"].split(",")
+    return maestro_labels
+
+
 def execute_make(app_dir: Path, command: str):
     subprocess.run(["make", command], cwd=app_dir)
 
 
 @click.group()
 def cli():
     pass
 
 
 @cli.command()
 @click.option(
+    "--applications-dir",
+    default=APPLICATIONS_DIR,
+    help="Specify the path containing docker compose applications.",
+)
+@click.option(
     "--target-file",
     default=TARGET_NAME,
     help="Specify the target YAML file to use for configuration.",
 )
 @click.option(
     "--dry-run", is_flag=True, help="Simulate the command without making any changes."
 )
-def up(target_file, dry_run):
+def up(applications_dir, target_file, dry_run):
     apps = get_applications(
-        base_dir=Path(APPLICATIONS_DIR),
+        base_dir=Path(applications_dir),
         target=load_target(root_dir=Path(TARGET_DIR), target_name=target_file),
     )
     for app_dir, _ in apps:
         print(f"Starting {app_dir.name}".upper())
         if not dry_run:
             execute_make(app_dir, "up")
         print()
 
 
 @cli.command()
 @click.option(
+    "--applications-dir",
+    default=APPLICATIONS_DIR,
+    help="Specify the path containing docker compose applications.",
+)
+@click.option(
     "--target-file",
     default=TARGET_NAME,
     help="Specify the target YAML file to use for configuration.",
 )
 @click.option(
     "--dry-run", is_flag=True, help="Simulate the command without making any changes."
 )
-def down(target_file, dry_run):
+def down(applications_dir, target_file, dry_run):
     apps = get_applications(
-        base_dir=Path(APPLICATIONS_DIR),
+        base_dir=Path(applications_dir),
         target=load_target(root_dir=Path(TARGET_DIR), target_name=target_file),
     )
     for app_dir, _ in reversed(apps):
         print(f"Stopping {app_dir.name}".upper())
         if not dry_run:
             execute_make(app_dir, "down")
         print()
 
 
 @cli.command()
 @click.option(
+    "--applications-dir",
+    default=APPLICATIONS_DIR,
+    help="Specify the path containing docker compose applications.",
+)
+@click.option(
     "--target-file",
     default=TARGET_NAME,
     help="Specify the target YAML file to use for configuration.",
 )
 @click.option(
     "--services",
     is_flag=True,
     default=False,
     help="List the services running in each application.",
 )
-def list(target_file, services):
+def list(applications_dir, target_file, services):
     apps = get_applications(
-        base_dir=Path(APPLICATIONS_DIR),
+        base_dir=Path(applications_dir),
         target=load_target(root_dir=Path(TARGET_DIR), target_name=target_file),
     )
     for app_dir, app_config in apps:
         print(f"{app_dir.name}: - {app_config}")
 
         if services:
             docker_command = ["docker", "compose", "ps", "--format", "json"]
```

### Comparing `maestro_compose-0.1.2/pyproject.toml` & `maestro_compose-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maestro-compose"
-version = "0.1.2"
+version = "0.1.3"
 description = "A simple command line tool for managing Docker Compose stacks using tags and other metadata."
 license = "MIT"
 authors = ["Nick Schenone <nschenone16@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/nschenone/maestro-compose"
 
 [tool.poetry.dependencies]
```

### Comparing `maestro_compose-0.1.2/PKG-INFO` & `maestro_compose-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro-compose
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple command line tool for managing Docker Compose stacks using tags and other metadata.
 Home-page: https://github.com/nschenone/maestro-compose
 License: MIT
 Author: Nick Schenone
 Author-email: nschenone16@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

