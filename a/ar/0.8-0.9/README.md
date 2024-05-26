# Comparing `tmp/ar-0.8.tar.gz` & `tmp/ar-0.9.tar.gz`

## Comparing `ar-0.8.tar` & `ar-0.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ar-0.8/.pylintrc
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 ar-0.8/release.sh
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 ar-0.8/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ar-0.8/ar/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ar-0.8/ar/__main__.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 ar-0.8/ar/archive.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ar-0.8/ar/substream.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ar-0.8/ar/tests/test_bad_archive.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ar-0.8/ar/tests/test_bsd.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 ar-0.8/ar/tests/test_linux.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 ar-0.8/ar/tests/test_roundtrip.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 ar-0.8/ar/tests/test_windows.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 ar-0.8/ar/tests/test_wrong_mody.py
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 ar-0.8/test_data/MiniLib.lib
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ar-0.8/test_data/bad.a
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ar-0.8/test_data/bsd.a
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 ar-0.8/test_data/linux.a
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ar-0.8/.gitignore
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 ar-0.8/README.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ar-0.8/hatch.toml
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ar-0.8/pyproject.toml
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 ar-0.8/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ar-0.9/.pylintrc
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 ar-0.9/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ar-0.9/ar/__init__.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 ar-0.9/ar/__main__.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 ar-0.9/ar/archive.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ar-0.9/ar/substream.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ar-0.9/ar/tests/test_bad_archive.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 ar-0.9/ar/tests/test_bsd.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 ar-0.9/ar/tests/test_linux.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 ar-0.9/ar/tests/test_roundtrip.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 ar-0.9/ar/tests/test_windows.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 ar-0.9/ar/tests/test_wrong_mody.py
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 ar-0.9/test_data/MiniLib.lib
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ar-0.9/test_data/bad.a
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ar-0.9/test_data/bsd.a
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 ar-0.9/test_data/linux.a
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ar-0.9/.gitignore
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 ar-0.9/README.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ar-0.9/hatch.toml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 ar-0.9/pyproject.toml
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 ar-0.9/PKG-INFO
```

### Comparing `ar-0.8/.github/workflows/python-package.yml` & `ar-0.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `ar-0.8/ar/__main__.py` & `ar-0.9/ar/__main__.py`

 * *Files identical despite different names*

### Comparing `ar-0.8/ar/archive.py` & `ar-0.9/ar/archive.py`

 * *Files identical despite different names*

### Comparing `ar-0.8/ar/substream.py` & `ar-0.9/ar/substream.py`

 * *Files identical despite different names*

### Comparing `ar-0.8/ar/tests/test_bsd.py` & `ar-0.9/ar/tests/test_bsd.py`

 * *Files identical despite different names*

### Comparing `ar-0.8/ar/tests/test_linux.py` & `ar-0.9/ar/tests/test_linux.py`

 * *Files identical despite different names*

### Comparing `ar-0.8/ar/tests/test_roundtrip.py` & `ar-0.9/ar/tests/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `ar-0.8/ar/tests/test_windows.py` & `ar-0.9/ar/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `ar-0.8/test_data/MiniLib.lib` & `ar-0.9/test_data/MiniLib.lib`

 * *Files identical despite different names*

### Comparing `ar-0.8/README.md` & `ar-0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 Extract all files:
 ```python
 from ar import Archive
 with open('file.a', 'rb') as f:
   archive = Archive(f)
   for entry in archive:
-    with open(entry.name) as output:
-      content = entry.get_stream().read()
+    with open(entry.name, 'wb') as output:
+      content = archive.open(entry, 'rb').read()
       output.write(content)
 ```
 
 ## Developing
 Create a virtual environment using python version of liking
 
     python3.10 -m venv venv
```

### Comparing `ar-0.8/pyproject.toml` & `ar-0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,7 +29,10 @@
 
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 source = "vcs"
+
+[tool.hatch.build.targets.wheel]
+only-packages = true
```

### Comparing `ar-0.8/PKG-INFO` & `ar-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ar
-Version: 0.8
+Version: 0.9
 Summary: Access ar archive files (.a)!
 Project-URL: Repository, https://github.com/vidstige/ar/
 Project-URL: Bug Tracker, https://github.com/vidstige/ar/issues
 Author-email: Samuel Carlsson <samuel.carlsson@gmail.com>
 Keywords: ar,archive,extract,library
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -52,16 +52,16 @@
 
 Extract all files:
 ```python
 from ar import Archive
 with open('file.a', 'rb') as f:
   archive = Archive(f)
   for entry in archive:
-    with open(entry.name) as output:
-      content = entry.get_stream().read()
+    with open(entry.name, 'wb') as output:
+      content = archive.open(entry, 'rb').read()
       output.write(content)
 ```
 
 ## Developing
 Create a virtual environment using python version of liking
 
     python3.10 -m venv venv
```

