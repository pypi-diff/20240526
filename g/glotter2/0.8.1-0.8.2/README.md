# Comparing `tmp/glotter2-0.8.1.tar.gz` & `tmp/glotter2-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glotter2-0.8.1.tar", max compression
+gzip compressed data, was "glotter2-0.8.2.tar", max compression
```

## Comparing `glotter2-0.8.1.tar` & `glotter2-0.8.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1105 2024-04-12 23:36:18.088296 glotter2-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0     3273 2024-04-12 23:36:18.092296 glotter2-0.8.1/README.md
--rw-r--r--   0        0        0      191 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/__init__.py
--rw-r--r--   0        0        0     4258 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/__main__.py
--rw-r--r--   0        0        0    13060 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/auto_gen_test.py
--rw-r--r--   0        0        0     2334 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/batch.py
--rw-r--r--   0        0        0     4340 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/containerfactory.py
--rw-r--r--   0        0        0      680 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/decorators.py
--rw-r--r--   0        0        0     1340 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/download.py
--rw-r--r--   0        0        0     4753 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/project.py
--rw-r--r--   0        0        0     3087 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/report.py
--rw-r--r--   0        0        0      762 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/run.py
--rw-r--r--   0        0        0     7758 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/settings.py
--rw-r--r--   0        0        0      327 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/singleton.py
--rw-r--r--   0        0        0     6648 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/source.py
--rw-r--r--   0        0        0     1933 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/test.py
--rw-r--r--   0        0        0     5027 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/test_doc_generator.py
--rw-r--r--   0        0        0     2195 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/test_generator.py
--rw-r--r--   0        0        0     5490 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/testinfo.py
--rw-r--r--   0        0        0      853 2024-04-12 23:36:18.092296 glotter2-0.8.1/glotter/utils.py
--rw-r--r--   0        0        0     1595 2024-04-12 23:36:18.092296 glotter2-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4572 1970-01-01 00:00:00.000000 glotter2-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-05-26 18:16:37.446706 glotter2-0.8.2/LICENSE.txt
+-rw-r--r--   0        0        0     3309 2024-05-26 18:16:37.446706 glotter2-0.8.2/README.md
+-rw-r--r--   0        0        0      191 2024-05-26 18:16:37.446706 glotter2-0.8.2/glotter/__init__.py
+-rw-r--r--   0        0        0     4258 2024-05-26 18:16:37.446706 glotter2-0.8.2/glotter/__main__.py
+-rw-r--r--   0        0        0    13060 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/auto_gen_test.py
+-rw-r--r--   0        0        0     2334 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/batch.py
+-rw-r--r--   0        0        0     4340 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/containerfactory.py
+-rw-r--r--   0        0        0      680 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/decorators.py
+-rw-r--r--   0        0        0     1340 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/download.py
+-rw-r--r--   0        0        0     4753 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/project.py
+-rw-r--r--   0        0        0     3087 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/report.py
+-rw-r--r--   0        0        0      762 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/run.py
+-rw-r--r--   0        0        0     7758 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/settings.py
+-rw-r--r--   0        0        0      327 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/singleton.py
+-rw-r--r--   0        0        0     6648 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/source.py
+-rw-r--r--   0        0        0     1933 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/test.py
+-rw-r--r--   0        0        0     5027 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/test_doc_generator.py
+-rw-r--r--   0        0        0     2195 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/test_generator.py
+-rw-r--r--   0        0        0     5490 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/testinfo.py
+-rw-r--r--   0        0        0      853 2024-05-26 18:16:37.450706 glotter2-0.8.2/glotter/utils.py
+-rw-r--r--   0        0        0     1595 2024-05-26 18:16:37.450706 glotter2-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 glotter2-0.8.2/PKG-INFO
```

### Comparing `glotter2-0.8.1/LICENSE.txt` & `glotter2-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/README.md` & `glotter2-0.8.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 If you'd like to contribute to Glotter2, read our [contributing guidelines](./CONTRIBUTING.md).
 
 ## Changelog
 
 ### Glotter2 releases
 
+* 0.8.2:
+  * Update to docker 7.1.0
 * 0.8.1:
   * Update to black 24.4.0
 * 0.8.0:
   * Add ability to split lines on the expected value
 * 0.7.2:
   * Make sure temporary directory used for docker is world accessible
 * 0.7.1:
```

### Comparing `glotter2-0.8.1/glotter/__main__.py` & `glotter2-0.8.2/glotter/__main__.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/auto_gen_test.py` & `glotter2-0.8.2/glotter/auto_gen_test.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/batch.py` & `glotter2-0.8.2/glotter/batch.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/containerfactory.py` & `glotter2-0.8.2/glotter/containerfactory.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/decorators.py` & `glotter2-0.8.2/glotter/decorators.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/download.py` & `glotter2-0.8.2/glotter/download.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/project.py` & `glotter2-0.8.2/glotter/project.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/report.py` & `glotter2-0.8.2/glotter/report.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/run.py` & `glotter2-0.8.2/glotter/run.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/settings.py` & `glotter2-0.8.2/glotter/settings.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/source.py` & `glotter2-0.8.2/glotter/source.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/test.py` & `glotter2-0.8.2/glotter/test.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/test_doc_generator.py` & `glotter2-0.8.2/glotter/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/test_generator.py` & `glotter2-0.8.2/glotter/test_generator.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/testinfo.py` & `glotter2-0.8.2/glotter/testinfo.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/glotter/utils.py` & `glotter2-0.8.2/glotter/utils.py`

 * *Files identical despite different names*

### Comparing `glotter2-0.8.1/pyproject.toml` & `glotter2-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "glotter2"
 packages = [{include="glotter"}]
-version = "0.8.1"
+version = "0.8.2"
 description = "An execution library for scripts written in any language. This is a fork of https://github.com/auroq/glotter"
 authors = ["auroq", "rzuckerm"]
 readme = "README.md"
 license = "LICENSE.txt"
 homepage = "https://github.com/rzuckerm/glotter2"
 documentation = "https://rzuckerm.github.io/glotter2"
 classifiers = [
@@ -16,15 +16,15 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/rzuckerm/glotter2/issues"
 "Changelog" = "https://github.com/rzuckerm/glotter2#changelog"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-docker = "^6.1.0"
+docker = "^7.1.0"
 jinja2 = "^3.1.2"
 pytest = "^7.2.1"
 pyyaml = "^6.0"
 pytest-xdist = "^3.2.0"
 black = "^24.4.0"
 pydantic = "^1.10.6"
```

### Comparing `glotter2-0.8.1/PKG-INFO` & `glotter2-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glotter2
-Version: 0.8.1
+Version: 0.8.2
 Summary: An execution library for scripts written in any language. This is a fork of https://github.com/auroq/glotter
 Home-page: https://github.com/rzuckerm/glotter2
 License: LICENSE.txt
 Author: auroq
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=24.4.0,<25.0.0)
-Requires-Dist: docker (>=6.1.0,<7.0.0)
+Requires-Dist: docker (>=7.1.0,<8.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: pytest-xdist (>=3.2.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Bug Tracker, https://github.com/rzuckerm/glotter2/issues
 Project-URL: Changelog, https://github.com/rzuckerm/glotter2#changelog
@@ -51,14 +51,16 @@
 
 If you'd like to contribute to Glotter2, read our [contributing guidelines](./CONTRIBUTING.md).
 
 ## Changelog
 
 ### Glotter2 releases
 
+* 0.8.2:
+  * Update to docker 7.1.0
 * 0.8.1:
   * Update to black 24.4.0
 * 0.8.0:
   * Add ability to split lines on the expected value
 * 0.7.2:
   * Make sure temporary directory used for docker is world accessible
 * 0.7.1:
```

