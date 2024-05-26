# Comparing `tmp/roofai-4.32.1.tar.gz` & `tmp/roofai-4.33.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roofai-4.32.1.tar", last modified: Sun May 26 18:52:21 2024, max compression
+gzip compressed data, was "roofai-4.33.1.tar", last modified: Sun May 26 20:40:48 2024, max compression
```

## Comparing `roofai-4.32.1.tar` & `roofai-4.33.1.tar`

### file list

```diff
@@ -1,20 +1,38 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 18:52:21.077910 roofai-4.32.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.32.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:37.000000 roofai-4.32.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-26 18:52:21.077538 roofai-4.32.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3117 2024-05-19 23:19:15.000000 roofai-4.32.1/README.md
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-23 04:22:10.000000 roofai-4.32.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      318 2024-05-20 22:40:00.000000 roofai-4.32.1/requirements.txt
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 18:52:21.074097 roofai-4.32.1/roofAI/
--rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-26 18:52:14.000000 roofai-4.32.1/roofAI/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.32.1/roofAI/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.32.1/roofAI/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.32.1/roofAI/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 18:52:21.076961 roofai-4.32.1/roofAI.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-26 18:52:21.000000 roofai-4.32.1/roofAI.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      289 2024-05-26 18:52:21.000000 roofai-4.32.1/roofAI.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 18:52:21.000000 roofai-4.32.1/roofAI.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      319 2024-05-26 18:52:21.000000 roofai-4.32.1/roofAI.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-26 18:52:21.000000 roofai-4.32.1/roofAI.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 18:52:21.077985 roofai-4.32.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      222 2024-05-23 04:23:01.000000 roofai-4.32.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:40:48.876968 roofai-4.33.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.33.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:37.000000 roofai-4.33.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-26 20:40:48.876187 roofai-4.33.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3117 2024-05-19 23:19:15.000000 roofai-4.33.1/README.md
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-23 04:22:10.000000 roofai-4.33.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      318 2024-05-20 22:40:00.000000 roofai-4.33.1/requirements.txt
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:40:48.862860 roofai-4.33.1/roofAI/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:40:48.872224 roofai-4.33.1/roofAI/.abcli/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:40:48.873208 roofai-4.33.1/roofAI/.abcli/QGIS/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1264 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/QGIS/expressions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      803 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/QGIS/server.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1338 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/QGIS.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      142 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/aka.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1307 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/cloudwatch.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     3052 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/conda.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     4275 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/dataset_ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1028 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/dataset_review.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     5921 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/inference.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     1682 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/roofAI.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     4940 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/semseg.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:40:48.874692 roofai-4.33.1/roofAI/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      964 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/tests/dataset_ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      863 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/tests/sagemaker_train.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1255 2024-05-26 18:51:36.000000 roofai-4.33.1/roofAI/.abcli/tests/semseg_train.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-26 20:40:41.000000 roofai-4.33.1/roofAI/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.33.1/roofAI/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.33.1/roofAI/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.33.1/roofAI/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:40:48.875305 roofai-4.33.1/roofAI.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-26 20:40:48.000000 roofai-4.33.1/roofAI.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      723 2024-05-26 20:40:48.000000 roofai-4.33.1/roofAI.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 20:40:48.000000 roofai-4.33.1/roofAI.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      319 2024-05-26 20:40:48.000000 roofai-4.33.1/roofAI.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-26 20:40:48.000000 roofai-4.33.1/roofAI.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 20:40:48.877100 roofai-4.33.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      336 2024-05-26 20:40:34.000000 roofai-4.33.1/setup.py
```

### Comparing `roofai-4.32.1/LICENSE` & `roofai-4.33.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roofai-4.32.1/PKG-INFO` & `roofai-4.33.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.32.1
+Version: 4.33.1
 Summary: 🏛️ everything AI about roofs.
 Home-page: https://github.com/kamangir/roofAI
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `roofai-4.32.1/README.md` & `roofai-4.33.1/README.md`

 * *Files identical despite different names*

### Comparing `roofai-4.32.1/roofAI/__main__.py` & `roofai-4.33.1/roofAI/__main__.py`

 * *Files identical despite different names*

### Comparing `roofai-4.32.1/roofAI.egg-info/PKG-INFO` & `roofai-4.33.1/roofAI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.32.1
+Version: 4.33.1
 Summary: 🏛️ everything AI about roofs.
 Home-page: https://github.com/kamangir/roofAI
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

