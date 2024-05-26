# Comparing `tmp/outpostcli-0.0.8.tar.gz` & `tmp/outpostcli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outpostcli-0.0.8.tar", last modified: Wed Feb 14 09:19:47 2024, max compression
+gzip compressed data, was "outpostcli-0.0.9.tar", last modified: Wed Feb 14 13:45:19 2024, max compression
```

## Comparing `outpostcli-0.0.8.tar` & `outpostcli-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 09:19:47.000086 outpostcli-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-14 09:19:40.000000 outpostcli-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-14 09:19:47.000086 outpostcli-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-14 09:19:40.000000 outpostcli-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 09:19:46.996086 outpostcli-0.0.8/outpostcli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 09:19:40.000000 outpostcli-0.0.8/outpostcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-02-14 09:19:40.000000 outpostcli-0.0.8/outpostcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-02-14 09:19:40.000000 outpostcli-0.0.8/outpostcli/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-14 09:19:40.000000 outpostcli-0.0.8/outpostcli/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-02-14 09:19:40.000000 outpostcli-0.0.8/outpostcli/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-14 09:19:40.000000 outpostcli-0.0.8/outpostcli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-02-14 09:19:40.000000 outpostcli-0.0.8/outpostcli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 09:19:47.000086 outpostcli-0.0.8/outpostcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-14 09:19:46.000000 outpostcli-0.0.8/outpostcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-14 09:19:46.000000 outpostcli-0.0.8/outpostcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 09:19:46.000000 outpostcli-0.0.8/outpostcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-14 09:19:46.000000 outpostcli-0.0.8/outpostcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-14 09:19:46.000000 outpostcli-0.0.8/outpostcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-14 09:19:46.000000 outpostcli-0.0.8/outpostcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-02-14 09:19:40.000000 outpostcli-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 09:19:47.000086 outpostcli-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-14 09:19:40.000000 outpostcli-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:45:19.983836 outpostcli-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-14 13:45:12.000000 outpostcli-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-14 13:45:19.983836 outpostcli-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-14 13:45:12.000000 outpostcli-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:45:19.983836 outpostcli-0.0.9/outpostcli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 13:45:12.000000 outpostcli-0.0.9/outpostcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-02-14 13:45:12.000000 outpostcli-0.0.9/outpostcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-02-14 13:45:12.000000 outpostcli-0.0.9/outpostcli/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-14 13:45:12.000000 outpostcli-0.0.9/outpostcli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11399 2024-02-14 13:45:12.000000 outpostcli-0.0.9/outpostcli/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-14 13:45:12.000000 outpostcli-0.0.9/outpostcli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-02-14 13:45:12.000000 outpostcli-0.0.9/outpostcli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:45:19.983836 outpostcli-0.0.9/outpostcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-14 13:45:19.000000 outpostcli-0.0.9/outpostcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-14 13:45:19.000000 outpostcli-0.0.9/outpostcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 13:45:19.000000 outpostcli-0.0.9/outpostcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-14 13:45:19.000000 outpostcli-0.0.9/outpostcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-14 13:45:19.000000 outpostcli-0.0.9/outpostcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-14 13:45:19.000000 outpostcli-0.0.9/outpostcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-02-14 13:45:12.000000 outpostcli-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 13:45:19.983836 outpostcli-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-14 13:45:12.000000 outpostcli-0.0.9/setup.py
```

### Comparing `outpostcli-0.0.8/LICENSE` & `outpostcli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `outpostcli-0.0.8/PKG-INFO` & `outpostcli-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outpostcli
-Version: 0.0.8
+Version: 0.0.9
 Summary: CLI for Outpost
 Author: Outpost Innovations, Inc.
 License: MIT License
         
         Copyright (c) 2023 Outpost Innovations, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `outpostcli-0.0.8/README.md` & `outpostcli-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `outpostcli-0.0.8/outpostcli/cli.py` & `outpostcli-0.0.9/outpostcli/cli.py`

 * *Files identical despite different names*

### Comparing `outpostcli-0.0.8/outpostcli/config_utils.py` & `outpostcli-0.0.9/outpostcli/config_utils.py`

 * *Files identical despite different names*

### Comparing `outpostcli-0.0.8/outpostcli/endpoints.py` & `outpostcli-0.0.9/outpostcli/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
     help="base image",
     required=False,
 )
 @click.option(
     "--visibility",
     type=click.Choice(["private", "public", "internal"]),
     # type=str,
+    default="private",
     help="visibility of the endpoint",
     required=False,
 )
 @click.option(
     "--replica-scaling-min",
     type=int,
     default=0,
@@ -165,33 +166,31 @@
     base_image: Optional[str],
     name: Optional[str],
     template_path: Optional[str],
     task_type: str,
     replica_scaling_min: int,
     replica_scaling_max: int,
     visibility: str,
-    replica_scaling_scaledowm_period: int,
+    replica_scaling_scaledown_period: int,
     replica_scaling_target_pending_req: int,
 ):
     client = Client(api_token=api_token)
     if template_path:
         [actual_path, class_name] = template_path.rsplit(":", 1)
-        click.echo(f"{actual_path},{class_name}")
         if not actual_path or not class_name:
             click.echo(
                 "Please specify the template classname along with the path.", err=True
             )
             return
         if not base_image:
             click.echo("Please specify the base image you want to use.", err=True)
             return
         try:
             result = urlparse(actual_path)
             if all([result.scheme, result.netloc]):
-                click.echo("url")
                 data = {
                     "templateType": "custom",
                     "customTemplateConfig": {
                         "className": class_name,
                         "url": actual_path,
                     },
                     "hardwareInstance": hardware_instance,
@@ -199,40 +198,38 @@
                     "name": name,
                     "containerType": "prebuilt",
                     "visibility": visibility,
                     "prebuiltImageName": base_image,
                     "replicaScalingConfig": {
                         "min": replica_scaling_min,
                         "max": replica_scaling_max,
-                        "scaledownPeriod": replica_scaling_scaledowm_period,
+                        "scaledownPeriod": replica_scaling_scaledown_period,
                         "targetPendingRequests": replica_scaling_target_pending_req,
                     },
                 }
                 create_resp = Endpoints(client=client, entity=entity).create(json=data)
             else:
                 raise ValueError("Not an url.")
         except ValueError:
             if os.path.exists(actual_path) and os.path.isfile(actual_path):
-                click.echo("file")
-                # do something
                 data = {
                     "templateType": "custom",
                     "customTemplateConfig": {
                         "className": class_name,
                     },
                     "taskType": task_type,
                     "name": name,
                     "containerType": "prebuilt",
                     "visibility": visibility,
                     "hardwareInstance": hardware_instance,
                     "prebuiltImageName": base_image,
                     "replicaScalingConfig": {
                         "min": replica_scaling_min,
                         "max": replica_scaling_max,
-                        "scaledownPeriod": replica_scaling_scaledowm_period,
+                        "scaledownPeriod": replica_scaling_scaledown_period,
                         "targetPendingRequests": replica_scaling_target_pending_req,
                     },
                 }
                 create_resp = Endpoints(client=client, entity=entity).create(
                     data={"metadata": json.dumps(data)},
                     files={"template": open(actual_path, mode="rb")},
                 )
@@ -274,15 +271,15 @@
             "autogeneratedTemplateConfig": model_details,
             "hardwareInstance": hardware_instance,
             "visibility": visibility,
             "name": name,
             "replicaScalingConfig": {
                 "min": replica_scaling_min,
                 "max": replica_scaling_max,
-                "scaledownPeriod": replica_scaling_scaledowm_period,
+                "scaledownPeriod": replica_scaling_scaledown_period,
                 "targetPendingRequests": replica_scaling_target_pending_req,
             },
         }
         create_resp = Endpoints(client=client, entity=entity).create(json=create_body)
         click.echo("endpoint created...")
     click.echo(f"name: {create_resp.name}")
     click.echo(f"id: {create_resp.id}")
```

### Comparing `outpostcli-0.0.8/outpostcli/utils.py` & `outpostcli-0.0.9/outpostcli/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 import click
 from outpostkit._types.endpoint import (
-    InferenceAutogeneratedHFModelDetails,
-    InferenceAutogeneratedOutpostModelDetails,
+    EndpointAutogeneratedHFModelDetails,
+    EndpointAutogeneratedOutpostModelDetails,
 )
 from rich.console import Console
 
 from outpostcli.config_utils import (
     get_default_api_token_from_config,
     get_default_entity_from_config,
 )
@@ -56,16 +56,16 @@
     except Exception as e:
         click.echo(e)
         return -1, None
 
 
 def combine_inf_load_source_model(
     load_source,
-    outpost_model: Optional[InferenceAutogeneratedOutpostModelDetails],
-    hf_model: Optional[InferenceAutogeneratedHFModelDetails],
+    outpost_model: Optional[EndpointAutogeneratedOutpostModelDetails],
+    hf_model: Optional[EndpointAutogeneratedHFModelDetails],
 ):
     if load_source == "hugginface" and hf_model:
         return f"hf:{hf_model.id}"
     elif load_source == "outpost" and outpost_model:
         return f"{outpost_model.model.fullName}"
     else:
         return "custom"
```

### Comparing `outpostcli-0.0.8/outpostcli.egg-info/PKG-INFO` & `outpostcli-0.0.9/outpostcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outpostcli
-Version: 0.0.8
+Version: 0.0.9
 Summary: CLI for Outpost
 Author: Outpost Innovations, Inc.
 License: MIT License
         
         Copyright (c) 2023 Outpost Innovations, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `outpostcli-0.0.8/pyproject.toml` & `outpostcli-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "outpostcli"
-version = "0.0.8"
+version = "0.0.9"
 description = "CLI for Outpost"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Outpost Innovations, Inc." }]
 requires-python = ">=3.8"
 dependencies = [
     "outpostkit>=0.0.34",
```

