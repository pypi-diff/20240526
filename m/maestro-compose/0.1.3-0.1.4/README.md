# Comparing `tmp/maestro_compose-0.1.3.tar.gz` & `tmp/maestro_compose-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro_compose-0.1.3.tar", max compression
+gzip compressed data, was "maestro_compose-0.1.4.tar", max compression
```

## Comparing `maestro_compose-0.1.3.tar` & `maestro_compose-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        9 2024-05-25 23:28:35.104821 maestro_compose-0.1.3/README.md
--rw-r--r--   0        0        0       57 2024-05-26 00:57:34.299753 maestro_compose-0.1.3/maestro_compose/__init__.py
--rw-r--r--   0        0        0     6325 2024-05-26 00:57:09.483656 maestro_compose-0.1.3/maestro_compose/__main__.py
--rw-r--r--   0        0        0     1330 2024-05-26 00:57:34.299139 maestro_compose-0.1.3/maestro_compose/models.py
--rw-r--r--   0        0        0      765 2024-05-26 00:57:56.189519 maestro_compose-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 maestro_compose-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        9 2024-05-25 23:28:35.104821 maestro_compose-0.1.4/README.md
+-rw-r--r--   0        0        0       57 2024-05-26 00:57:34.299753 maestro_compose-0.1.4/maestro_compose/__init__.py
+-rw-r--r--   0        0        0     6394 2024-05-26 01:06:58.457624 maestro_compose-0.1.4/maestro_compose/__main__.py
+-rw-r--r--   0        0        0     1330 2024-05-26 00:57:34.299139 maestro_compose-0.1.4/maestro_compose/models.py
+-rw-r--r--   0        0        0      765 2024-05-26 01:07:22.786359 maestro_compose-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 maestro_compose-0.1.4/PKG-INFO
```

### Comparing `maestro_compose-0.1.3/maestro_compose/__main__.py` & `maestro_compose-0.1.4/maestro_compose/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 
 def load_config(app_dir: Path) -> MaestroConfig:
     for compose_file in DOCKER_COMPOSE_FILES:
         try:
             config_path = app_dir / compose_file
             compose_yaml = yaml.safe_load(config_path.read_text())
             maestro_labels = get_maestro_labels(compose_yaml=compose_yaml)
-            try:
-                return MaestroConfig(**maestro_labels)
-            except ValidationError as e:
-                print(f"Validation error in {app_dir}/{compose_file}: {e}")
-                return None
+            if maestro_labels:
+                try:
+                    return MaestroConfig(**maestro_labels)
+                except ValidationError as e:
+                    print(f"Validation error in {app_dir}/{compose_file}: {e}")
+                    return None
         except FileNotFoundError:
             pass
-    print(f"No docker-compose file found in {app_dir}")
+    print(f"No docker-compose file with maestro tags found in {app_dir}")
     return None
 
 
 def get_applications(base_dir: Path, target: MaestroTarget):
     apps = []
     for app_dir in base_dir.iterdir():
         if app_dir.is_dir():
```

### Comparing `maestro_compose-0.1.3/maestro_compose/models.py` & `maestro_compose-0.1.4/maestro_compose/models.py`

 * *Files identical despite different names*

### Comparing `maestro_compose-0.1.3/pyproject.toml` & `maestro_compose-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maestro-compose"
-version = "0.1.3"
+version = "0.1.4"
 description = "A simple command line tool for managing Docker Compose stacks using tags and other metadata."
 license = "MIT"
 authors = ["Nick Schenone <nschenone16@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/nschenone/maestro-compose"
 
 [tool.poetry.dependencies]
```

### Comparing `maestro_compose-0.1.3/PKG-INFO` & `maestro_compose-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maestro-compose
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple command line tool for managing Docker Compose stacks using tags and other metadata.
 Home-page: https://github.com/nschenone/maestro-compose
 License: MIT
 Author: Nick Schenone
 Author-email: nschenone16@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

