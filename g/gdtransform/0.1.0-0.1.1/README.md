# Comparing `tmp/gdtransform-0.1.0.tar.gz` & `tmp/gdtransform-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdtransform-0.1.0.tar", last modified: Sun May 26 13:30:16 2024, max compression
+gzip compressed data, was "gdtransform-0.1.1.tar", last modified: Sun May 26 14:44:50 2024, max compression
```

## Comparing `gdtransform-0.1.0.tar` & `gdtransform-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 13:30:16.322141 gdtransform-0.1.0/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.1.0/LICENSE
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-26 13:30:16.322141 gdtransform-0.1.0/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.1.0/README.md
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-26 13:30:01.000000 gdtransform-0.1.0/pyproject.toml
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-26 13:30:16.322141 gdtransform-0.1.0/setup.cfg
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 13:30:16.318141 gdtransform-0.1.0/src/
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 13:30:16.322141 gdtransform-0.1.0/src/gdtransform/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:56:25.000000 gdtransform-0.1.0/src/gdtransform/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      238 2024-05-26 13:01:29.000000 gdtransform-0.1.0/src/gdtransform/constants.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     1386 2024-05-26 13:15:23.000000 gdtransform-0.1.0/src/gdtransform/introspect.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     3057 2024-05-25 17:34:12.000000 gdtransform-0.1.0/src/gdtransform/test.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     1890 2024-05-26 13:23:10.000000 gdtransform-0.1.0/src/gdtransform/transform.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 13:30:16.322141 gdtransform-0.1.0/src/gdtransform.egg-info/
--rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-26 13:30:16.000000 gdtransform-0.1.0/src/gdtransform.egg-info/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      367 2024-05-26 13:30:16.000000 gdtransform-0.1.0/src/gdtransform.egg-info/SOURCES.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-26 13:30:16.000000 gdtransform-0.1.0/src/gdtransform.egg-info/dependency_links.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-26 13:30:16.000000 gdtransform-0.1.0/src/gdtransform.egg-info/top_level.txt
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 13:30:16.322141 gdtransform-0.1.0/tests/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      670 2024-05-26 13:29:22.000000 gdtransform-0.1.0/tests/test_suite.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     3384 2024-05-25 17:43:42.000000 gdtransform-0.1.0/tests/test_test.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:44:50.755257 gdtransform-0.1.1/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-17 10:41:53.000000 gdtransform-0.1.1/LICENSE
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-26 14:44:50.755257 gdtransform-0.1.1/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       91 2024-05-17 10:41:53.000000 gdtransform-0.1.1/README.md
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      733 2024-05-26 14:44:45.000000 gdtransform-0.1.1/pyproject.toml
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-26 14:44:50.755257 gdtransform-0.1.1/setup.cfg
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:44:50.755257 gdtransform-0.1.1/src/
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:44:50.755257 gdtransform-0.1.1/src/gdtransform/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-17 11:56:25.000000 gdtransform-0.1.1/src/gdtransform/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      310 2024-05-26 14:42:58.000000 gdtransform-0.1.1/src/gdtransform/constants.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1683 2024-05-26 14:42:58.000000 gdtransform-0.1.1/src/gdtransform/introspect.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     3057 2024-05-25 17:34:12.000000 gdtransform-0.1.1/src/gdtransform/test.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2109 2024-05-26 14:42:58.000000 gdtransform-0.1.1/src/gdtransform/transform.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:44:50.755257 gdtransform-0.1.1/src/gdtransform.egg-info/
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      715 2024-05-26 14:44:50.000000 gdtransform-0.1.1/src/gdtransform.egg-info/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      367 2024-05-26 14:44:50.000000 gdtransform-0.1.1/src/gdtransform.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-26 14:44:50.000000 gdtransform-0.1.1/src/gdtransform.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-26 14:44:50.000000 gdtransform-0.1.1/src/gdtransform.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:44:50.755257 gdtransform-0.1.1/tests/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      670 2024-05-26 13:29:22.000000 gdtransform-0.1.1/tests/test_suite.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     3384 2024-05-25 17:43:42.000000 gdtransform-0.1.1/tests/test_test.py
```

### Comparing `gdtransform-0.1.0/LICENSE` & `gdtransform-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdtransform-0.1.0/PKG-INFO` & `gdtransform-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdtransform-0.1.0/pyproject.toml` & `gdtransform-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gdtransform"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Mayank Bhargava", email = "mbhargava.gd@gmail.com" },
 ]
 description = "Transformation library to build transformations for Godel Grid data platform"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdtransform-0.1.0/src/gdtransform/introspect.py` & `gdtransform-0.1.1/src/gdtransform/introspect.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from inspect import getmembers, isfunction
 
-from .constants import GRID_BATCH_TRANSFORMATION_FLAG, GRID_TRANSFORMATION_BUILDER_FLAG, GRID_TRANSFORMATION_FLAG, \
+from .constants import GRID_BATCH_TRANSFORMATION_FLAG, GRID_TRANSFORMATION_BUILDER_FLAG, \
+    GRID_TRANSFORMATION_BUILDER_NAME, GRID_TRANSFORMATION_FLAG, \
     GRID_TRANSFORMATION_NAME
 
 
 def has_transformation_flag(function):
     return (hasattr(function, GRID_TRANSFORMATION_FLAG) and
             getattr(function, GRID_TRANSFORMATION_FLAG)) or \
         (hasattr(function, GRID_BATCH_TRANSFORMATION_FLAG) and
@@ -18,20 +19,26 @@
 
 def is_valid_transformation(function, name):
     return has_transformation_flag(function) and \
         hasattr(function, GRID_TRANSFORMATION_NAME) and \
         getattr(function, GRID_TRANSFORMATION_NAME) == name
 
 
+def is_valid_builder(function, name):
+    return has_builder_flag(function) and \
+        hasattr(function, GRID_TRANSFORMATION_BUILDER_NAME) and \
+        getattr(function, GRID_TRANSFORMATION_BUILDER_NAME) == name
+
+
 def get_module_transformation(module, name: str):
     members = getmembers(module, isfunction)
     if not members:
         return None
     for (_, member_func) in members:
-        if is_valid_transformation(member_func, name):
+        if is_valid_transformation(member_func, name) or is_valid_builder(member_func, name):
             return member_func
 
     return None
 
 
 def is_batch_transformation(function):
     return hasattr(function, GRID_BATCH_TRANSFORMATION_FLAG) and \
```

### Comparing `gdtransform-0.1.0/src/gdtransform/test.py` & `gdtransform-0.1.1/src/gdtransform/test.py`

 * *Files identical despite different names*

### Comparing `gdtransform-0.1.0/src/gdtransform/transform.py` & `gdtransform-0.1.1/src/gdtransform/transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List
 
 from .constants import GRID_BATCH_TRANSFORMATION_FLAG, \
-    GRID_TRANSFORMATION_BUILDER_FLAG, GRID_TRANSFORMATION_FLAG, \
+    GRID_TRANSFORMATION_BUILDER_FLAG, GRID_TRANSFORMATION_BUILDER_NAME, GRID_TRANSFORMATION_FLAG, \
     GRID_TRANSFORMATION_NAME
 
 
 def transformation(name: str):
     if not name:
         raise Exception('invalid transformation name')
 
@@ -35,33 +35,36 @@
         setattr(wrapper, GRID_TRANSFORMATION_NAME, name)
 
         return wrapper
 
     return __transformation
 
 
-def transformation_builder(is_batch: bool):
-    if is_batch is None:
+def transformation_builder(name: str, is_batch: bool):
+    if not name:
+        raise Exception('name is mandatory')
+    elif is_batch is None:
         raise Exception('is_batch option not specified')
 
     def __builder(operator):
-        def wrapper(name: str, *args, **kwargs):
+        def wrapper(transformation_name: str, *args, **kwargs):
             operator_callable = operator(*args, **kwargs)
 
             if not is_batch:
-                @transformation(name=name)
+                @transformation(name=transformation_name)
                 def __wrapped_transformation(data: Dict[str, Any]):
                     operator_callable(data)
 
                 return __wrapped_transformation
             else:
-                @batch_transformation(name=name)
+                @batch_transformation(name=transformation_name)
                 def __wrapped_transformation(data_list: List[Dict[str, Any]]):
                     operator_callable(data_list)
 
                 return __wrapped_transformation
 
         setattr(wrapper, GRID_TRANSFORMATION_BUILDER_FLAG, True)
+        setattr(wrapper, GRID_TRANSFORMATION_BUILDER_NAME, name)
 
         return wrapper
 
     return __builder
```

### Comparing `gdtransform-0.1.0/src/gdtransform.egg-info/PKG-INFO` & `gdtransform-0.1.1/src/gdtransform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdtransform
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transformation library to build transformations for Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gdtransform
 Project-URL: Issues, https://github.com/godelgrid/gdtransform/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdtransform-0.1.0/tests/test_suite.py` & `gdtransform-0.1.1/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `gdtransform-0.1.0/tests/test_test.py` & `gdtransform-0.1.1/tests/test_test.py`

 * *Files identical despite different names*

