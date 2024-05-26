# Comparing `tmp/puepy-0.1.0a0.tar.gz` & `tmp/puepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puepy-0.1.0a0.tar", max compression
+gzip compressed data, was "puepy-0.1.1.tar", max compression
```

## Comparing `puepy-0.1.0a0.tar` & `puepy-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     3040 2024-05-23 22:56:56.973923 puepy-0.1.0a0/README.md
--rw-r--r--   0        0        0       51 2024-01-27 14:28:42.000000 puepy-0.1.0a0/puepy/.git
--rw-r--r--   0        0        0       90 2024-05-23 22:56:56.974136 puepy-0.1.0a0/puepy/__init__.py
--rw-r--r--   0        0        0     2756 2024-05-22 16:40:08.205022 puepy-0.1.0a0/puepy/application.py
--rw-r--r--   0        0        0    21358 2024-05-22 16:40:08.340089 puepy-0.1.0a0/puepy/core.py
--rw-r--r--   0        0        0       84 2024-05-19 09:43:46.381198 puepy-0.1.0a0/puepy/errors.py
--rw-r--r--   0        0        0     2659 2024-05-22 16:40:08.205435 puepy-0.1.0a0/puepy/reactivity.py
--rw-r--r--   0        0        0     2893 2024-05-22 16:40:08.205611 puepy-0.1.0a0/puepy/router.py
--rw-r--r--   0        0        0     1390 2024-05-22 16:40:08.205797 puepy-0.1.0a0/puepy/runtime.py
--rw-r--r--   0        0        0     2211 2024-05-19 09:43:46.381673 puepy-0.1.0a0/puepy/storage.py
--rw-r--r--   0        0        0     4055 2024-05-22 16:40:08.206270 puepy-0.1.0a0/puepy/util.py
--rw-r--r--   0        0        0      336 2024-05-23 22:56:56.974429 puepy-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 puepy-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     3040 2024-05-26 17:02:46.417236 puepy-0.1.1/README.md
+-rw-r--r--   0        0        0       90 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/__init__.py
+-rw-r--r--   0        0        0     2756 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/application.py
+-rw-r--r--   0        0        0    21358 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/core.py
+-rw-r--r--   0        0        0       84 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/errors.py
+-rw-r--r--   0        0        0     2659 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/reactivity.py
+-rw-r--r--   0        0        0     2893 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/router.py
+-rw-r--r--   0        0        0     1390 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/runtime.py
+-rw-r--r--   0        0        0     2211 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/storage.py
+-rw-r--r--   0        0        0     4055 2024-05-26 17:02:46.417236 puepy-0.1.1/puepy/util.py
+-rw-r--r--   0        0        0      466 2024-05-26 17:02:46.417236 puepy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 puepy-0.1.1/PKG-INFO
```

### Comparing `puepy-0.1.0a0/README.md` & `puepy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `puepy-0.1.0a0/puepy/application.py` & `puepy-0.1.1/puepy/application.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.0a0/puepy/core.py` & `puepy-0.1.1/puepy/core.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.0a0/puepy/reactivity.py` & `puepy-0.1.1/puepy/reactivity.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.0a0/puepy/router.py` & `puepy-0.1.1/puepy/router.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.0a0/puepy/runtime.py` & `puepy-0.1.1/puepy/runtime.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.0a0/puepy/storage.py` & `puepy-0.1.1/puepy/storage.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.0a0/puepy/util.py` & `puepy-0.1.1/puepy/util.py`

 * *Files identical despite different names*

### Comparing `puepy-0.1.0a0/PKG-INFO` & `puepy-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: puepy
-Version: 0.1.0a0
+Version: 0.1.1
 Summary: Frontend Framework for PyScript
 Author: Ken Kinder
 Author-email: ken+github@kkinder.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pypugjs (>=5.9.12,<6.0.0)
 Description-Content-Type: text/markdown
 
 # PuePy -- PyScript Frontend Framework
 
 PuePy is an attempt to create a frontend framework using [PyScript](https://pyscript.net). PuePy is partially inspired by Vue. It runs entirely in your browser, though server-side rendering is likely feasible.  PuePy aims to support two runtime environments: PyScript Pyodide or PyScript Micropython. The Micropython option foregoes some features found in the CPython, but offers a far, far smaller runtime, making it a better option for websites. Line-of-business or scientific webapp developers may prefer the CPython version, which is heavier but more functional.
 
 Without further ado, here's a taste:
```

