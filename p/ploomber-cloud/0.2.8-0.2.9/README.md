# Comparing `tmp/ploomber-cloud-0.2.8.tar.gz` & `tmp/ploomber-cloud-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-cloud-0.2.8.tar", last modified: Wed May 15 22:37:25 2024, max compression
+gzip compressed data, was "ploomber-cloud-0.2.9.tar", last modified: Tue May 21 18:52:10 2024, max compression
```

## Comparing `ploomber-cloud-0.2.8.tar` & `ploomber-cloud-0.2.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.062686 ploomber-cloud-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/abc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/test-vllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/community.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/premium.json
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-15 22:37:09.000000 ploomber-cloud-0.2.8/src/ploomber_cloud/zip_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:37:25.070686 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 22:37:24.000000 ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:52:10.070762 ploomber-cloud-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-21 18:52:10.070762 ploomber-cloud-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-21 18:52:10.070762 ploomber-cloud-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:52:10.066762 ploomber-cloud-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:52:10.070762 ploomber-cloud-0.2.9/src/ploomber_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:52:10.070762 ploomber-cloud-0.2.9/src/ploomber_cloud/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:52:10.070762 ploomber-cloud-0.2.9/src/ploomber_cloud/assets/vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/assets/vllm/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/assets/vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/assets/vllm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/assets/vllm/test-vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:52:10.070762 ploomber-cloud-0.2.9/src/ploomber_cloud/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/configurations/community.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/configurations/premium.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-21 18:51:53.000000 ploomber-cloud-0.2.9/src/ploomber_cloud/zip_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:52:10.070762 ploomber-cloud-0.2.9/src/ploomber_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-21 18:52:09.000000 ploomber-cloud-0.2.9/src/ploomber_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-21 18:52:09.000000 ploomber-cloud-0.2.9/src/ploomber_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:52:09.000000 ploomber-cloud-0.2.9/src/ploomber_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 18:52:09.000000 ploomber-cloud-0.2.9/src/ploomber_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-21 18:52:09.000000 ploomber-cloud-0.2.9/src/ploomber_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 18:52:09.000000 ploomber-cloud-0.2.9/src/ploomber_cloud.egg-info/top_level.txt
```

### Comparing `ploomber-cloud-0.2.8/CHANGELOG.md` & `ploomber-cloud-0.2.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 0.2.9 (2024-05-21)
+
+- [Feature] show custom ID when using `--from-existing`.
+
 ## 0.2.8 (2024-05-15)
 
 - [Feature] Add support for Flask applications
 
 ## 0.2.7 (2024-05-08)
 
 - [Feature] Add `--clear-cache` option to `ploomber-cloud examples`.
```

### Comparing `ploomber-cloud-0.2.8/pyproject.toml` & `ploomber-cloud-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/setup.py` & `ploomber-cloud-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/abc.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/abc.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/api.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/api.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/api_key.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/api_key.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/requirements.txt` & `ploomber-cloud-0.2.9/src/ploomber_cloud/assets/vllm/requirements.txt`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/assets/vllm/test-vllm.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/assets/vllm/test-vllm.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/cli.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/cli.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/config.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/config.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/community.json` & `ploomber-cloud-0.2.9/src/ploomber_cloud/configurations/community.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/configurations/premium.json` & `ploomber-cloud-0.2.9/src/ploomber_cloud/configurations/premium.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/constants.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/constants.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/delete.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/delete.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/deploy.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/examples.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/examples.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/exceptions.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/functions.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/functions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/github.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/github.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/init.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/init.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,21 +75,45 @@
     return click.prompt(
         "Project type",
         type=click.Choice(VALID_PROJECT_TYPES),
         show_choices=False,
     )
 
 
+def _get_project_details_mappings(projects):
+    """Function for returning lookup of:
+    1. Project ID that is displayed to the user and its original ID.
+       Projects with custom name are displayed as project id (custom name).
+    2. Project custom names and the corresponding ID.
+    """
+
+    display_id_mapping = {}
+    project_name_mapping = {}
+
+    for project in projects:
+        pid = display_id = project["id"]
+        name = project["name"]
+        if name and pid != name:
+            display_id = f"{pid} ({name})"
+        display_id_mapping[display_id], project_name_mapping[name] = pid, pid
+
+    return display_id_mapping, project_name_mapping
+
+
 def _init_from_existing():
     """Generate ploomber-cloud.json from existing project"""
     click.echo("Initializing from existing project...")
     client = api.PloomberCloudClient()
 
     # Get user's available projects
-    project_choices = [project["id"] for project in client.get_projects()["projects"]]
+    all_projects = client.get_projects()["projects"]
+
+    display_id_lookup, name_id_lookup = _get_project_details_mappings(all_projects)
+
+    project_choices = list(display_id_lookup.keys())
     if len(project_choices) == 0:
         click.echo("You have no existing projects. Initialize without --from-existing.")
         return
 
     project_choices.append("exit")
     prompt = ["These are your existing projects, choose the one you're configuring:\n"]
     for i, item in enumerate(project_choices):
@@ -98,16 +122,30 @@
 
     # Prompt user for choice of existing project
     while True:
         choice = click.prompt(prompt_str, type=str)
         # Case: user enters number
         if choice.isnumeric() and 0 < int(choice) <= len(project_choices):
             choice = project_choices[int(choice) - 1]
+            # get original project ID for choice
+            if choice in display_id_lookup:
+                choice = display_id_lookup[choice]
+            break
+        # Case: user entered ID as displayed.
+        # Get original project ID if any
+        elif choice in display_id_lookup:
+            choice = display_id_lookup[choice]
+            break
+        # Case: user enters the custom name of project
+        elif choice in name_id_lookup:
+            choice = name_id_lookup[choice]
             break
-        elif choice in project_choices:  # Case: user enters id
+        # Case: choice is original project ID
+        # of project with custom name
+        elif choice in list(display_id_lookup.values()):
             break
         else:  # Case: user enters invalid
             click.echo("Please enter a valid choice.")
 
     # Allow user to exit menu without init
     if choice == "exit":
         click.echo("Exited.")
```

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/io.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/io.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/labels.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/labels.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/resources.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/resources.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/templates.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/templates.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/util.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/util.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud/zip_.py` & `ploomber-cloud-0.2.9/src/ploomber_cloud/zip_.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.8/src/ploomber_cloud.egg-info/SOURCES.txt` & `ploomber-cloud-0.2.9/src/ploomber_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

