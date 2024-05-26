# Comparing `tmp/gdtransform-0.0.8.tar.gz` & `tmp/gdtransform-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdtransform-0.0.8.tar", last modified: Sat May 25 17:57:38 2024, max compression
+gzip compressed data, was "gdtransform-0.0.9.tar", last modified: Sat May 25 19:47:39 2024, max compression
```

## Comparing `gdtransform-0.0.8.tar` & `gdtransform-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.557418 gdtransform-0.0.8/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.0.8/LICENSE
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-25 17:57:38.557418 gdtransform-0.0.8/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.0.8/README.md
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-25 17:57:04.000000 gdtransform-0.0.8/pyproject.toml
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-25 17:57:38.557418 gdtransform-0.0.8/setup.cfg
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.553418 gdtransform-0.0.8/src/
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.557418 gdtransform-0.0.8/src/gdtransform/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:56:25.000000 gdtransform-0.0.8/src/gdtransform/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      170 2024-05-25 17:34:12.000000 gdtransform-0.0.8/src/gdtransform/constants.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      929 2024-05-25 17:34:12.000000 gdtransform-0.0.8/src/gdtransform/introspect.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     3057 2024-05-25 17:34:12.000000 gdtransform-0.0.8/src/gdtransform/test.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      989 2024-05-25 17:43:42.000000 gdtransform-0.0.8/src/gdtransform/transform.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.557418 gdtransform-0.0.8/src/gdtransform.egg-info/
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-25 17:57:38.000000 gdtransform-0.0.8/src/gdtransform.egg-info/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      367 2024-05-25 17:57:38.000000 gdtransform-0.0.8/src/gdtransform.egg-info/SOURCES.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-25 17:57:38.000000 gdtransform-0.0.8/src/gdtransform.egg-info/dependency_links.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-25 17:57:38.000000 gdtransform-0.0.8/src/gdtransform.egg-info/top_level.txt
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 17:57:38.557418 gdtransform-0.0.8/tests/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      575 2024-05-25 17:54:40.000000 gdtransform-0.0.8/tests/test_suite.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     3384 2024-05-25 17:43:42.000000 gdtransform-0.0.8/tests/test_test.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 19:47:38.997145 gdtransform-0.0.9/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.0.9/LICENSE
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-25 19:47:38.997145 gdtransform-0.0.9/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.0.9/README.md
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-25 19:46:57.000000 gdtransform-0.0.9/pyproject.toml
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-25 19:47:38.997145 gdtransform-0.0.9/setup.cfg
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 19:47:38.993145 gdtransform-0.0.9/src/
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 19:47:38.997145 gdtransform-0.0.9/src/gdtransform/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:56:25.000000 gdtransform-0.0.9/src/gdtransform/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      170 2024-05-25 17:34:12.000000 gdtransform-0.0.9/src/gdtransform/constants.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1095 2024-05-25 19:46:57.000000 gdtransform-0.0.9/src/gdtransform/introspect.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     3057 2024-05-25 17:34:12.000000 gdtransform-0.0.9/src/gdtransform/test.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      989 2024-05-25 17:43:42.000000 gdtransform-0.0.9/src/gdtransform/transform.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 19:47:38.997145 gdtransform-0.0.9/src/gdtransform.egg-info/
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-25 19:47:38.000000 gdtransform-0.0.9/src/gdtransform.egg-info/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      367 2024-05-25 19:47:38.000000 gdtransform-0.0.9/src/gdtransform.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-25 19:47:38.000000 gdtransform-0.0.9/src/gdtransform.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-25 19:47:38.000000 gdtransform-0.0.9/src/gdtransform.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-25 19:47:38.997145 gdtransform-0.0.9/tests/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      575 2024-05-25 17:54:40.000000 gdtransform-0.0.9/tests/test_suite.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     3384 2024-05-25 17:43:42.000000 gdtransform-0.0.9/tests/test_test.py
```

### Comparing `gdtransform-0.0.8/LICENSE` & `gdtransform-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gdtransform-0.0.8/PKG-INFO` & `gdtransform-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.0.8
+Version: 0.0.9
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdtransform-0.0.8/pyproject.toml` & `gdtransform-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gdtransform"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "Mayank Bhargava", email = "mbhargava.gd@gmail.com" },
 ]
 description = "Transformation library to build transformations for Godel Grid data platform"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdtransform-0.0.8/src/gdtransform/introspect.py` & `gdtransform-0.0.9/src/gdtransform/introspect.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,7 +21,12 @@
     if not members:
         return None
     for (_, member_func) in members:
         if is_valid_transformation(member_func, name):
             return member_func
 
     return None
+
+
+def is_batch_transformation(function):
+    return hasattr(function, GRID_BATCH_TRANSFORMATION_FLAG) and \
+        getattr(function, GRID_BATCH_TRANSFORMATION_FLAG)
```

### Comparing `gdtransform-0.0.8/src/gdtransform/test.py` & `gdtransform-0.0.9/src/gdtransform/test.py`

 * *Files identical despite different names*

### Comparing `gdtransform-0.0.8/src/gdtransform/transform.py` & `gdtransform-0.0.9/src/gdtransform/transform.py`

 * *Files identical despite different names*

### Comparing `gdtransform-0.0.8/src/gdtransform.egg-info/PKG-INFO` & `gdtransform-0.0.9/src/gdtransform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.0.8
+Version: 0.0.9
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdtransform-0.0.8/tests/test_suite.py` & `gdtransform-0.0.9/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `gdtransform-0.0.8/tests/test_test.py` & `gdtransform-0.0.9/tests/test_test.py`

 * *Files identical despite different names*

