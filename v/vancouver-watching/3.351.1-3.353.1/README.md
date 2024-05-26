# Comparing `tmp/vancouver_watching-3.351.1.tar.gz` & `tmp/vancouver_watching-3.353.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vancouver_watching-3.351.1.tar", last modified: Sun May 26 04:18:02 2024, max compression
+gzip compressed data, was "vancouver_watching-3.353.1.tar", last modified: Sun May 26 04:44:29 2024, max compression
```

## Comparing `vancouver_watching-3.351.1.tar` & `vancouver_watching-3.353.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:18:02.607294 vancouver_watching-3.351.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-26 04:18:02.606715 vancouver_watching-3.351.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3611 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/README.md
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 04:18:02.607416 vancouver_watching-3.351.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      301 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/setup.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:18:02.603901 vancouver_watching-3.351.1/vancouver_watching/
--rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/vancouver_watching/QGIS.py
--rw-r--r--   0 kamangir   (502) staff       (20)      117 2024-05-26 04:17:57.000000 vancouver_watching-3.351.1/vancouver_watching/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1235 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/vancouver_watching/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/vancouver_watching/area.py
--rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/vancouver_watching/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/vancouver_watching/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/vancouver_watching/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/vancouver_watching/notebook.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 04:17:22.000000 vancouver_watching-3.351.1/vancouver_watching/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:18:02.606005 vancouver_watching-3.351.1/vancouver_watching.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-26 04:18:02.000000 vancouver_watching-3.351.1/vancouver_watching.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      538 2024-05-26 04:18:02.000000 vancouver_watching-3.351.1/vancouver_watching.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 04:18:02.000000 vancouver_watching-3.351.1/vancouver_watching.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:18:02.000000 vancouver_watching-3.351.1/vancouver_watching.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-05-26 04:18:02.000000 vancouver_watching-3.351.1/vancouver_watching.egg-info/top_level.txt
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:44:29.285978 vancouver_watching-3.353.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-26 04:44:29.285477 vancouver_watching-3.353.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3611 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/README.md
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 04:44:29.286059 vancouver_watching-3.353.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      301 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:44:29.281643 vancouver_watching-3.353.1/vancouver_watching/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/vancouver_watching/QGIS.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      117 2024-05-26 04:44:24.000000 vancouver_watching-3.353.1/vancouver_watching/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1235 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/vancouver_watching/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/vancouver_watching/area.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/vancouver_watching/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/vancouver_watching/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/vancouver_watching/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/vancouver_watching/notebook.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 04:17:22.000000 vancouver_watching-3.353.1/vancouver_watching/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:44:29.284641 vancouver_watching-3.353.1/vancouver_watching.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-26 04:44:29.000000 vancouver_watching-3.353.1/vancouver_watching.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      538 2024-05-26 04:44:29.000000 vancouver_watching-3.353.1/vancouver_watching.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 04:44:29.000000 vancouver_watching-3.353.1/vancouver_watching.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:44:29.000000 vancouver_watching-3.353.1/vancouver_watching.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-05-26 04:44:29.000000 vancouver_watching-3.353.1/vancouver_watching.egg-info/top_level.txt
```

### Comparing `vancouver_watching-3.351.1/LICENSE` & `vancouver_watching-3.353.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.351.1/PKG-INFO` & `vancouver_watching-3.353.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.351.1
+Version: 3.353.1
 Summary: 🌈 Vancouver Watching with AI.
 Home-page: https://github.com/kamangir/Vancouver-Watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `vancouver_watching-3.351.1/README.md` & `vancouver_watching-3.353.1/README.md`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.351.1/vancouver_watching/QGIS.py` & `vancouver_watching-3.353.1/vancouver_watching/QGIS.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.351.1/vancouver_watching/__main__.py` & `vancouver_watching-3.353.1/vancouver_watching/__main__.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.351.1/vancouver_watching/area.py` & `vancouver_watching-3.353.1/vancouver_watching/area.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.351.1/vancouver_watching.egg-info/PKG-INFO` & `vancouver_watching-3.353.1/vancouver_watching.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.351.1
+Version: 3.353.1
 Summary: 🌈 Vancouver Watching with AI.
 Home-page: https://github.com/kamangir/Vancouver-Watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `vancouver_watching-3.351.1/vancouver_watching.egg-info/SOURCES.txt` & `vancouver_watching-3.353.1/vancouver_watching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

