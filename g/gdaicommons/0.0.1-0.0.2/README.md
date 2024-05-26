# Comparing `tmp/gdaicommons-0.0.1.tar.gz` & `tmp/gdaicommons-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdaicommons-0.0.1.tar", last modified: Sun May 26 14:16:42 2024, max compression
+gzip compressed data, was "gdaicommons-0.0.2.tar", last modified: Sun May 26 14:49:17 2024, max compression
```

## Comparing `gdaicommons-0.0.1.tar` & `gdaicommons-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:16:42.422386 gdaicommons-0.0.1/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-26 09:35:40.000000 gdaicommons-0.0.1/LICENSE
--rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-26 14:16:42.422386 gdaicommons-0.0.1/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       15 2024-05-26 09:35:40.000000 gdaicommons-0.0.1/README.md
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      737 2024-05-26 14:12:21.000000 gdaicommons-0.0.1/pyproject.toml
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-26 14:16:42.422386 gdaicommons-0.0.1/setup.cfg
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:16:42.422386 gdaicommons-0.0.1/src/
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:16:42.422386 gdaicommons-0.0.1/src/gdaicommons/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-26 09:36:59.000000 gdaicommons-0.0.1/src/gdaicommons/__init__.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     2545 2024-05-26 14:10:41.000000 gdaicommons-0.0.1/src/gdaicommons/textclassification.py
--rw-rw-r--   0 mayank    (1000) mayank    (1000)     1180 2024-05-26 14:10:41.000000 gdaicommons-0.0.1/src/gdaicommons/transformations.py
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:16:42.422386 gdaicommons-0.0.1/src/gdaicommons.egg-info/
--rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-26 14:16:42.000000 gdaicommons-0.0.1/src/gdaicommons.egg-info/PKG-INFO
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      309 2024-05-26 14:16:42.000000 gdaicommons-0.0.1/src/gdaicommons.egg-info/SOURCES.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-26 14:16:42.000000 gdaicommons-0.0.1/src/gdaicommons.egg-info/dependency_links.txt
--rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-26 14:16:42.000000 gdaicommons-0.0.1/src/gdaicommons.egg-info/top_level.txt
-drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:16:42.422386 gdaicommons-0.0.1/tests/
--rw-rw-r--   0 mayank    (1000) mayank    (1000)      270 2024-05-26 14:00:18.000000 gdaicommons-0.0.1/tests/test_suite.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:49:17.020634 gdaicommons-0.0.2/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)    34523 2024-05-26 09:35:40.000000 gdaicommons-0.0.2/LICENSE
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-26 14:49:17.020634 gdaicommons-0.0.2/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       15 2024-05-26 09:35:40.000000 gdaicommons-0.0.2/README.md
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      737 2024-05-26 14:47:52.000000 gdaicommons-0.0.2/pyproject.toml
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       38 2024-05-26 14:49:17.020634 gdaicommons-0.0.2/setup.cfg
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:49:17.020634 gdaicommons-0.0.2/src/
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:49:17.020634 gdaicommons-0.0.2/src/gdaicommons/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        0 2024-05-26 09:36:59.000000 gdaicommons-0.0.2/src/gdaicommons/__init__.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     2545 2024-05-26 14:10:41.000000 gdaicommons-0.0.2/src/gdaicommons/textclassification.py
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)     1216 2024-05-26 14:46:31.000000 gdaicommons-0.0.2/src/gdaicommons/transformations.py
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:49:17.020634 gdaicommons-0.0.2/src/gdaicommons.egg-info/
+-rw-r--r--   0 mayank    (1000) mayank    (1000)      644 2024-05-26 14:49:17.000000 gdaicommons-0.0.2/src/gdaicommons.egg-info/PKG-INFO
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      309 2024-05-26 14:49:17.000000 gdaicommons-0.0.2/src/gdaicommons.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)        1 2024-05-26 14:49:17.000000 gdaicommons-0.0.2/src/gdaicommons.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)       12 2024-05-26 14:49:17.000000 gdaicommons-0.0.2/src/gdaicommons.egg-info/top_level.txt
+drwxrwxr-x   0 mayank    (1000) mayank    (1000)        0 2024-05-26 14:49:17.020634 gdaicommons-0.0.2/tests/
+-rw-rw-r--   0 mayank    (1000) mayank    (1000)      270 2024-05-26 14:00:18.000000 gdaicommons-0.0.2/tests/test_suite.py
```

### Comparing `gdaicommons-0.0.1/LICENSE` & `gdaicommons-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.1/PKG-INFO` & `gdaicommons-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdaicommons
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI transformation libraries and utilities to run on Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gd-ai-commons
 Project-URL: Issues, https://github.com/godelgrid/gd-ai-commons/issues
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gdaicommons-0.0.1/pyproject.toml` & `gdaicommons-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "gdaicommons"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "Mayank Bhargava", email = "mbhargava.gd@gmail.com" },
 ]
 description = "AI transformation libraries and utilities to run on Godel Grid data platform"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gdaicommons-0.0.1/src/gdaicommons/textclassification.py` & `gdaicommons-0.0.2/src/gdaicommons/textclassification.py`

 * *Files identical despite different names*

### Comparing `gdaicommons-0.0.1/src/gdaicommons/transformations.py` & `gdaicommons-0.0.2/src/gdaicommons/transformations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from gdtransform.transform import transformation_builder
 
 from .textclassification import TextClassificationTransformation
 
 
-@transformation_builder(is_batch=True)
+@transformation_builder(name='text-classification-builder', is_batch=True)
 def text_classification(*args, **kwargs):
     model = kwargs['model']
     input_field = kwargs['input_field']
     top_k_scores = int(kwargs['top_k_scores']) if 'top_k_scores' in kwargs and kwargs['top_k_scores'] else 1
     full_output_field = kwargs.get('full_output_field', None)
     label_output_field = kwargs.get('label_output_field', None)
     score_output_field = kwargs.get('score_output_field', None)
```

### Comparing `gdaicommons-0.0.1/src/gdaicommons.egg-info/PKG-INFO` & `gdaicommons-0.0.2/src/gdaicommons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdaicommons
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI transformation libraries and utilities to run on Godel Grid data platform
 Author-email: Mayank Bhargava <mbhargava.gd@gmail.com>
 Project-URL: Homepage, https://www.godelgrid.com
 Project-URL: Documentation, https://www.godelgrid.com/docs
 Project-URL: Repository, https://github.com/godelgrid/gd-ai-commons
 Project-URL: Issues, https://github.com/godelgrid/gd-ai-commons/issues
 Classifier: Programming Language :: Python :: 3.10
```

