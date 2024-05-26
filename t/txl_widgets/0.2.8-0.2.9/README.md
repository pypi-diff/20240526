# Comparing `tmp/txl_widgets-0.2.8.tar.gz` & `tmp/txl_widgets-0.2.9.tar.gz`

## Comparing `txl_widgets-0.2.8.tar` & `txl_widgets-0.2.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 txl_widgets-0.2.8/txl_widgets/__init__.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 txl_widgets-0.2.8/txl_widgets/components.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 txl_widgets-0.2.8/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 txl_widgets-0.2.8/LICENSE.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 txl_widgets-0.2.8/README.md
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 txl_widgets-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 txl_widgets-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 txl_widgets-0.2.9/txl_widgets/__init__.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 txl_widgets-0.2.9/txl_widgets/components.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 txl_widgets-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 txl_widgets-0.2.9/LICENSE.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 txl_widgets-0.2.9/README.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 txl_widgets-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 txl_widgets-0.2.9/PKG-INFO
```

### Comparing `txl_widgets-0.2.8/txl_widgets/components.py` & `txl_widgets-0.2.9/txl_widgets/components.py`

 * *Files identical despite different names*

### Comparing `txl_widgets-0.2.8/LICENSE.txt` & `txl_widgets-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `txl_widgets-0.2.8/pyproject.toml` & `txl_widgets-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "txl",
   "ypywidgets >=0.6.5,<0.7.0",
-  "ypywidgets-textual >=0.2.4,<0.3.0",
+  "ypywidgets-textual >=0.3.0,<0.4.0",
   "pycrdt >=0.8.11,<0.9.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://github.com/davidbrochart/jpterm/plugins/widgets"
```

### Comparing `txl_widgets-0.2.8/PKG-INFO` & `txl_widgets-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txl_widgets
-Version: 0.2.8
+Version: 0.2.9
 Summary: TXL plugin for kernel widgets
 Project-URL: Source, https://github.com/davidbrochart/jpterm/plugins/widgets
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -12,12 +12,12 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: pycrdt<0.9.0,>=0.8.11
 Requires-Dist: txl
-Requires-Dist: ypywidgets-textual<0.3.0,>=0.2.4
+Requires-Dist: ypywidgets-textual<0.4.0,>=0.3.0
 Requires-Dist: ypywidgets<0.7.0,>=0.6.5
 Description-Content-Type: text/markdown
 
 # TXL plugin for widgets
```

