# Comparing `tmp/ricklib-0.0.1.tar.gz` & `tmp/ricklib-0.0.2.tar.gz`

## Comparing `ricklib-0.0.1.tar` & `ricklib-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ricklib-0.0.1/src/ricklib/__init__.py
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 ricklib-0.0.1/src/ricklib/graphics/pngenerator.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 ricklib-0.0.1/LICENSE
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ricklib-0.0.1/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ricklib-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ricklib-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ricklib-0.0.2/src/ricklib/__init__.py
+-rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 ricklib-0.0.2/src/ricklib/pngenerator.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ricklib-0.0.2/tests/graphic_test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 ricklib-0.0.2/LICENSE
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ricklib-0.0.2/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ricklib-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ricklib-0.0.2/PKG-INFO
```

### Comparing `ricklib-0.0.1/src/ricklib/graphics/pngenerator.py` & `ricklib-0.0.2/src/ricklib/pngenerator.py`

 * *Files identical despite different names*

### Comparing `ricklib-0.0.1/LICENSE` & `ricklib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ricklib-0.0.1/pyproject.toml` & `ricklib-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ricklib"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Richard (Rick) Howell", email="rick.howell.arts@gmail.com" },
 ]
 description = "A small package for personal use including useful operations."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ricklib-0.0.1/PKG-INFO` & `ricklib-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ricklib
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package for personal use including useful operations.
 Project-URL: Homepage, https://github.com/rick-howell/ricklib
 Project-URL: Issues, https://github.com/rick-howell/ricklib/issues
 Author-email: "Richard (Rick) Howell" <rick.howell.arts@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

