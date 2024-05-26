# Comparing `tmp/profile-metrics-local-0.0.8.tar.gz` & `tmp/profile-metrics-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile-metrics-local-0.0.8.tar", last modified: Tue Nov 21 10:55:16 2023, max compression
+gzip compressed data, was "profile-metrics-local-0.0.9.tar", last modified: Tue Nov 21 10:58:18 2023, max compression
```

## Comparing `profile-metrics-local-0.0.8.tar` & `profile-metrics-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 10:55:16.374519 profile-metrics-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-21 10:55:16.374519 profile-metrics-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-11-21 10:54:48.000000 profile-metrics-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 10:55:16.374519 profile-metrics-local-0.0.8/profile_metrics_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 10:55:16.374519 profile-metrics-local-0.0.8/profile_metrics_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 10:54:48.000000 profile-metrics-local-0.0.8/profile_metrics_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2023-11-21 10:54:48.000000 profile-metrics-local-0.0.8/profile_metrics_local/src/profile_metrics_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 10:55:16.374519 profile-metrics-local-0.0.8/profile_metrics_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-21 10:55:16.000000 profile-metrics-local-0.0.8/profile_metrics_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-21 10:55:16.000000 profile-metrics-local-0.0.8/profile_metrics_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 10:55:16.000000 profile-metrics-local-0.0.8/profile_metrics_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-21 10:55:16.000000 profile-metrics-local-0.0.8/profile_metrics_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-21 10:55:16.000000 profile-metrics-local-0.0.8/profile_metrics_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-11-21 10:54:48.000000 profile-metrics-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 10:55:16.374519 profile-metrics-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2023-11-21 10:54:48.000000 profile-metrics-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 10:58:18.128206 profile-metrics-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-21 10:58:18.128206 profile-metrics-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-11-21 10:57:49.000000 profile-metrics-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 10:58:18.124206 profile-metrics-local-0.0.9/profile_metrics_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 10:58:18.124206 profile-metrics-local-0.0.9/profile_metrics_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 10:57:49.000000 profile-metrics-local-0.0.9/profile_metrics_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2023-11-21 10:57:49.000000 profile-metrics-local-0.0.9/profile_metrics_local/src/profile_metrics_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 10:58:18.124206 profile-metrics-local-0.0.9/profile_metrics_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2023-11-21 10:58:18.000000 profile-metrics-local-0.0.9/profile_metrics_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2023-11-21 10:58:18.000000 profile-metrics-local-0.0.9/profile_metrics_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 10:58:18.000000 profile-metrics-local-0.0.9/profile_metrics_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-21 10:58:18.000000 profile-metrics-local-0.0.9/profile_metrics_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-21 10:58:18.000000 profile-metrics-local-0.0.9/profile_metrics_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2023-11-21 10:57:49.000000 profile-metrics-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 10:58:18.128206 profile-metrics-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2023-11-21 10:57:49.000000 profile-metrics-local-0.0.9/setup.py
```

### Comparing `profile-metrics-local-0.0.8/PKG-INFO` & `profile-metrics-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-metrics-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles profile-metrics-local Python
 Home-page: https://github.com/circles/profile-metrics-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profile-metrics-local-0.0.8/README.md` & `profile-metrics-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `profile-metrics-local-0.0.8/profile_metrics_local/src/profile_metrics_local.py` & `profile-metrics-local-0.0.9/profile_metrics_local/src/profile_metrics_local.py`

 * *Files identical despite different names*

### Comparing `profile-metrics-local-0.0.8/profile_metrics_local.egg-info/PKG-INFO` & `profile-metrics-local-0.0.9/profile_metrics_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-metrics-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles profile-metrics-local Python
 Home-page: https://github.com/circles/profile-metrics-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profile-metrics-local-0.0.8/pyproject.toml` & `profile-metrics-local-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "profile-metrics-local"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.8" # https://pypi.org/project/profile-metrics-local i.e. https://pypi.org/project/storage-local/
+version = "0.0.9" # https://pypi.org/project/profile-metrics-local i.e. https://pypi.org/project/storage-local/
 description = "profile-metrics-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `profile-metrics-local-0.0.8/setup.py` & `profile-metrics-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 with open('README.md') as f:
     readme = f.read()
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/profile-metrics-local/
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/profile-metrics-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles profile-metrics-local Python",
     long_description="This Package implements CRUD operation of profile-metrics",
     long_description_content_type='text/markdown',
     url="https://github.com/circles/profile-metrics-local-python-package",  # https://pypi.org/project/profile-metrics-local/
     # packages=setuptools.find_packages(),
```

