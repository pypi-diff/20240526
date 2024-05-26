# Comparing `tmp/blue_stability-4.30.1.tar.gz` & `tmp/blue_stability-4.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_stability-4.30.1.tar", last modified: Sat May 25 17:36:29 2024, max compression
+gzip compressed data, was "blue_stability-4.31.1.tar", last modified: Sat May 25 20:30:36 2024, max compression
```

## Comparing `blue_stability-4.30.1.tar` & `blue_stability-4.31.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 17:36:29.483310 blue_stability-4.30.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-12-05 02:50:06.000000 blue_stability-4.30.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:08:53.000000 blue_stability-4.30.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     2868 2024-05-25 17:36:29.482667 blue_stability-4.30.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1831 2024-03-04 07:34:46.000000 blue_stability-4.30.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 17:36:29.479607 blue_stability-4.30.1/blue_stability/
--rw-r--r--   0 kamangir   (502) staff       (20)      143 2024-05-25 17:36:24.000000 blue_stability-4.30.1/blue_stability/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      245 2024-05-24 02:08:27.000000 blue_stability-4.30.1/blue_stability/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       95 2024-03-24 00:16:18.000000 blue_stability-4.30.1/blue_stability/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-12-05 02:50:06.000000 blue_stability-4.30.1/blue_stability/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 17:36:29.481921 blue_stability-4.30.1/blue_stability.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     2868 2024-05-25 17:36:29.000000 blue_stability-4.30.1/blue_stability.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      361 2024-05-25 17:36:29.000000 blue_stability-4.30.1/blue_stability.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 17:36:29.000000 blue_stability-4.30.1/blue_stability.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      157 2024-05-25 17:36:29.000000 blue_stability-4.30.1/blue_stability.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       15 2024-05-25 17:36:29.000000 blue_stability-4.30.1/blue_stability.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:08:53.000000 blue_stability-4.30.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      157 2024-05-25 01:42:30.000000 blue_stability-4.30.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 17:36:29.483419 blue_stability-4.30.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      238 2024-05-24 02:07:25.000000 blue_stability-4.30.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 20:30:36.153882 blue_stability-4.31.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-12-05 02:50:06.000000 blue_stability-4.31.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:08:53.000000 blue_stability-4.31.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     2846 2024-05-25 20:30:36.153245 blue_stability-4.31.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1831 2024-03-04 07:34:46.000000 blue_stability-4.31.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 20:30:36.149905 blue_stability-4.31.1/blue_stability/
+-rw-r--r--   0 kamangir   (502) staff       (20)      121 2024-05-25 20:30:30.000000 blue_stability-4.31.1/blue_stability/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      245 2024-05-24 02:08:27.000000 blue_stability-4.31.1/blue_stability/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       95 2024-03-24 00:16:18.000000 blue_stability-4.31.1/blue_stability/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-12-05 02:50:06.000000 blue_stability-4.31.1/blue_stability/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 20:30:36.152416 blue_stability-4.31.1/blue_stability.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     2846 2024-05-25 20:30:36.000000 blue_stability-4.31.1/blue_stability.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      361 2024-05-25 20:30:36.000000 blue_stability-4.31.1/blue_stability.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 20:30:36.000000 blue_stability-4.31.1/blue_stability.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      157 2024-05-25 20:30:36.000000 blue_stability-4.31.1/blue_stability.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       15 2024-05-25 20:30:36.000000 blue_stability-4.31.1/blue_stability.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:08:53.000000 blue_stability-4.31.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      157 2024-05-25 01:42:30.000000 blue_stability-4.31.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 20:30:36.153981 blue_stability-4.31.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      238 2024-05-24 02:07:25.000000 blue_stability-4.31.1/setup.py
```

### Comparing `blue_stability-4.30.1/LICENSE` & `blue_stability-4.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blue_stability-4.30.1/PKG-INFO` & `blue_stability-4.31.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: blue_stability
-Version: 4.30.1
-Summary: 🟦 bash cli for stability.ai API's stable diffusion inference
+Version: 4.31.1
+Summary: 🟦 a command interface to stability.ai.
 Home-page: https://github.com/kamangir/blue-stability
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
```

### Comparing `blue_stability-4.30.1/README.md` & `blue_stability-4.31.1/README.md`

 * *Files identical despite different names*

### Comparing `blue_stability-4.30.1/blue_stability.egg-info/PKG-INFO` & `blue_stability-4.31.1/blue_stability.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: blue_stability
-Version: 4.30.1
-Summary: 🟦 bash cli for stability.ai API's stable diffusion inference
+Version: 4.31.1
+Summary: 🟦 a command interface to stability.ai.
 Home-page: https://github.com/kamangir/blue-stability
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
```

