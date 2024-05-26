# Comparing `tmp/kapoorlabs_lightning-5.3.8.tar.gz` & `tmp/kapoorlabs_lightning-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kapoorlabs_lightning-5.3.8.tar", last modified: Mon May 20 17:23:54 2024, max compression
+gzip compressed data, was "kapoorlabs_lightning-5.4.0.tar", last modified: Sun May 26 15:13:18 2024, max compression
```

## Comparing `kapoorlabs_lightning-5.3.8.tar` & `kapoorlabs_lightning-5.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.255281 kapoorlabs_lightning-5.3.8/.github/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.255281 kapoorlabs_lightning-5.3.8/.github/workflows/
--rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/.github/workflows/deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/.gitignore
--rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/.pre-commit-config.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/LICENSE
--rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/MANIFEST.in
--rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.259281 kapoorlabs_lightning-5.3.8/licenses/
--rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/Apache-2
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/BSD-3
--rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/GPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/LGPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/MIT
--rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/licenses/MPL-2
--rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/pyproject.toml
--rw-r--r--   0 debian    (1000) debian    (1000)     1766 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/setup.cfg
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.255281 kapoorlabs_lightning-5.3.8/src/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)      102 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-20 17:23:54.000000 kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/
--rw-r--r--   0 debian    (1000) debian    (1000)     1603 2024-05-17 14:55:57.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-20 17:23:54.267281 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_tests/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_tests/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-20 17:22:56.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_version.py
--rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/caped.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/graph_functions.py
--rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/kapoorlabs.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)    65805 2024-05-18 20:51:03.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/lightning_trainer.py
--rw-r--r--   0 debian    (1000) debian    (1000)    13532 2024-05-20 17:22:52.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/metrics.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/optimizers.py
--rw-r--r--   0 debian    (1000) debian    (1000)    10230 2024-05-13 17:03:42.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_callbacks.py
--rw-r--r--   0 debian    (1000) debian    (1000)    16120 2024-05-20 11:14:56.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_datasets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_loggers.py
--rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_losses.py
--rw-r--r--   0 debian    (1000) debian    (1000)    23059 2024-05-18 20:48:11.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_transforms.py
--rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/schedulers.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2504 2024-05-17 21:13:17.000000 kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/utils.py
--rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/tox.ini
--rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.8/update_version.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.369069 kapoorlabs_lightning-5.4.0/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.357069 kapoorlabs_lightning-5.4.0/.github/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.361069 kapoorlabs_lightning-5.4.0/.github/workflows/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/.github/workflows/deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/.gitignore
+-rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/LICENSE
+-rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-26 15:13:18.369069 kapoorlabs_lightning-5.4.0/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.361069 kapoorlabs_lightning-5.4.0/licenses/
+-rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/Apache-2
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/BSD-3
+-rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/GPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/LGPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/MIT
+-rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/licenses/MPL-2
+-rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/pyproject.toml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1766 2024-05-26 15:13:18.369069 kapoorlabs_lightning-5.4.0/setup.cfg
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.357069 kapoorlabs_lightning-5.4.0/src/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.365069 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     4108 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)      102 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-26 15:13:18.000000 kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.365069 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1603 2024-05-17 14:55:57.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-26 15:13:18.365069 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_tests/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_tests/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-25 17:21:15.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_version.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/caped.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/graph_functions.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)    67911 2024-05-25 17:20:46.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/lightning_trainer.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    13532 2024-05-20 17:22:52.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/metrics.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/optimizers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    10230 2024-05-13 17:03:42.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_callbacks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    16120 2024-05-25 17:04:44.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_datasets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_loggers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_losses.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    23059 2024-05-18 20:48:11.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_transforms.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/schedulers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2504 2024-05-17 21:13:17.000000 kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/utils.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/tox.ini
+-rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.4.0/update_version.py
```

### Comparing `kapoorlabs_lightning-5.3.8/.github/workflows/deploy.yml` & `kapoorlabs_lightning-5.4.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/.github/workflows/test_and_deploy.yml` & `kapoorlabs_lightning-5.4.0/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/.gitignore` & `kapoorlabs_lightning-5.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/.pre-commit-config.yaml` & `kapoorlabs_lightning-5.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/LICENSE` & `kapoorlabs_lightning-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/PKG-INFO` & `kapoorlabs_lightning-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.8
+Version: 5.4.0
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `kapoorlabs_lightning-5.3.8/README.md` & `kapoorlabs_lightning-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/licenses/Apache-2` & `kapoorlabs_lightning-5.4.0/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/licenses/BSD-3` & `kapoorlabs_lightning-5.4.0/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/licenses/GPL-3` & `kapoorlabs_lightning-5.4.0/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/licenses/LGPL-3` & `kapoorlabs_lightning-5.4.0/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/licenses/MIT` & `kapoorlabs_lightning-5.4.0/licenses/MIT`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/licenses/MPL-2` & `kapoorlabs_lightning-5.4.0/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/setup.cfg` & `kapoorlabs_lightning-5.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.8
+Version: 5.4.0
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `kapoorlabs_lightning-5.3.8/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `kapoorlabs_lightning-5.4.0/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/__init__.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/graph_functions.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/lightning_trainer.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -140,14 +140,65 @@
                 f"Invalid loss function choice, must be one of {self.LOSS_CHOICES}"
             )
         if self.scheduler_choice not in self.SCHEDULER_CHOICES:
             raise ValueError(
                 f"Invalid scheduler choice, must be one of {self.SCHEDULER_CHOICES}"
             )
 
+    def setup_gbr_datasets(self):
+
+        training_data = np.load(self.npz_file)
+
+        train_goblet_arrays = training_data["goblet_train_arrays"]
+        train_goblet_labels = training_data["goblet_train_labels"]
+        train_basal_arrays = training_data["basal_train_arrays"]
+        train_basal_labels = training_data["basal_train_labels"]
+        train_radial_arrays = training_data["radial_train_arrays"]
+        train_radial_labels = training_data["radial_train_labels"]
+
+        val_goblet_arrays = training_data["goblet_val_arrays"]
+        val_goblet_labels = training_data["goblet_val_labels"]
+        val_basal_arrays = training_data["basal_val_arrays"]
+        val_basal_labels = training_data["basal_val_labels"]
+        val_radial_arrays = training_data["radial_val_arrays"]
+        val_radial_labels = training_data["radial_val_labels"]
+
+        print(
+            f"Goblet labels in training {len(train_goblet_labels)}, Radial labels in training {len(train_radial_labels)}, Basal labels in training {len(train_basal_labels)}"
+        )
+        train_arrays = np.concatenate(
+            (train_goblet_arrays, train_basal_arrays, train_radial_arrays)
+        )
+        train_labels = np.concatenate(
+            (train_goblet_labels, train_basal_labels, train_radial_labels)
+        )
+
+        self.dataset_train = MitosisDataset(train_arrays, train_labels)
+
+        self.input_channels = self.dataset_train.input_channels
+
+        val_arrays = np.concatenate(
+            (val_goblet_arrays, val_basal_arrays, val_radial_arrays)
+        )
+        val_labels = np.concatenate(
+            (val_goblet_labels, val_basal_labels, val_radial_labels)
+        )
+
+        self.dataset_val = MitosisDataset(val_arrays, val_labels)
+
+        self.mitosis_data = LightningData(
+            data_train=self.dataset_train,
+            data_val=self.dataset_val,
+            batch_size=self.batch_size,
+            num_workers=self.num_workers,
+        )
+
+        self.train_loader = self.mitosis_data.train_dataloader()
+        self.val_loader = self.mitosis_data.val_dataloader()
+
     def setup_datasets(self):
 
         training_data = np.load(self.npz_file)
         train_dividing_arrays = training_data["dividing_train_arrays"]
         train_dividing_labels = training_data["dividing_train_labels"]
         train_non_dividing_arrays = training_data["non_dividing_train_arrays"]
         train_non_dividing_labels = training_data["non_dividing_train_labels"]
@@ -210,17 +261,15 @@
         self.logger = self.npz_logger
 
     def setup_checkpoint(self):
         self.ckpt_path = load_checkpoint_model(self.log_path)
         self.modelcheckpoint = CheckpointModel(save_dir=self.log_path)
 
     def setup_adam(self):
-        self.optimizer = Adam(
-            lr=self.learning_rate
-        )
+        self.optimizer = Adam(lr=self.learning_rate)
 
     def setup_rmsprop(self):
         self.optimizer = RMSprop(
             lr=self.learning_rate,
             momentum=self.momentum,
             weight_decay=self.decay,
             eps=self.epsilon,
@@ -263,14 +312,15 @@
 
         self.progress = CustomProgressBar()
         self.lightning_model = LightningModel(
             self.model,
             self.loss,
             self.optimizer,
             scheduler=self.scheduler,
+            num_classes=self.num_classes,
         )
         model_hyperparameters = {
             "input_channels": self.input_channels,
             "num_classes": self.num_classes,
             "learning_rate": self.learning_rate,
             "model_path": self.log_path,
             "model_name": self.experiment_name,
@@ -507,15 +557,14 @@
     def loss(self, y_hat, y):
 
         return self.loss_func(y_hat, y)
 
     def training_step(self, batch, batch_idx):
         x, y = batch
         y_hat = self(x)
-
         if not self.automatic_optimization:
             opt = self.optimizers()
             loss = self.loss(y_hat, y)
             opt.zero_grad()
             self.manual_backward(loss)
             opt.step()
         else:
@@ -609,15 +658,14 @@
     def compute_accuracy(self, outputs, labels):
 
         predicted = outputs.data
         accuracy = Accuracy(task="multiclass", num_classes=self.num_classes).to(
             self.device
         )
         accuracies = accuracy(predicted, labels)
-
         return accuracies
 
     def configure_optimizers(self):
         optimizer = self.optim_func(self.parameters())
 
         if self.scheduler is not None:
             scheduler = self.scheduler(optimizer=optimizer)
```

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/metrics.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/metrics.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/optimizers.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_callbacks.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_callbacks.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_datasets.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_loggers.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_losses.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_models.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/pytorch_transforms.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/schedulers.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/src/kapoorlabs_lightning/utils.py` & `kapoorlabs_lightning-5.4.0/src/kapoorlabs_lightning/utils.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/tox.ini` & `kapoorlabs_lightning-5.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.8/update_version.py` & `kapoorlabs_lightning-5.4.0/update_version.py`

 * *Files identical despite different names*

