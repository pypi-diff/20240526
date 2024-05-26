# Comparing `tmp/dicio_py-1.1.tar.gz` & `tmp/dicio_py-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicio_py-1.1.tar", last modified: Sun May 26 15:05:52 2024, max compression
+gzip compressed data, was "dicio_py-1.2.tar", last modified: Sun May 26 15:19:03 2024, max compression
```

## Comparing `dicio_py-1.1.tar` & `dicio_py-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 15:05:52.509818 dicio_py-1.1/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.1/LICENSE
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1619 2024-05-26 15:05:52.505818 dicio_py-1.1/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.1/README.md
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 15:05:52.501818 dicio_py-1.1/dicio_py.egg-info/
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1619 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      205 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       43 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/entry_points.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        4 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/top_level.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-26 15:05:52.509818 dicio_py-1.1/setup.cfg
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      738 2024-05-26 15:05:18.000000 dicio_py-1.1/setup.py
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 15:05:52.501818 dicio_py-1.1/src/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.1/src/__init__.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 15:19:03.535235 dicio_py-1.2/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.2/LICENSE
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1619 2024-05-26 15:19:03.531235 dicio_py-1.2/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.2/README.md
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 15:19:03.531235 dicio_py-1.2/dicio_py.egg-info/
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1619 2024-05-26 15:19:03.000000 dicio_py-1.2/dicio_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      205 2024-05-26 15:19:03.000000 dicio_py-1.2/dicio_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-26 15:19:03.000000 dicio_py-1.2/dicio_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       43 2024-05-26 15:19:03.000000 dicio_py-1.2/dicio_py.egg-info/entry_points.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        4 2024-05-26 15:19:03.000000 dicio_py-1.2/dicio_py.egg-info/top_level.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-26 15:19:03.535235 dicio_py-1.2/setup.cfg
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      738 2024-05-26 15:18:53.000000 dicio_py-1.2/setup.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 15:19:03.531235 dicio_py-1.2/src/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.2/src/__init__.py
```

### Comparing `dicio_py-1.1/LICENSE` & `dicio_py-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dicio_py-1.1/PKG-INFO` & `dicio_py-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.1
+Version: 1.2
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `dicio_py-1.1/README.md` & `dicio_py-1.2/README.md`

 * *Files identical despite different names*

### Comparing `dicio_py-1.1/dicio_py.egg-info/PKG-INFO` & `dicio_py-1.2/dicio_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.1
+Version: 1.2
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `dicio_py-1.1/setup.py` & `dicio_py-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dicio-py",  # Replace with your own username
-    version="1.1",
+    version="1.2",
     author="Jetrom17",
     author_email="Jeiel@duck.com",
     description="Dicionário via CLI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Jetrom17/dicio-py",
     packages=setuptools.find_packages(),
```

