# Comparing `tmp/ZeroXRequests-1.0.tar.gz` & `tmp/ZeroXRequests-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZeroXRequests-1.0.tar", last modified: Sun May 26 15:01:18 2024, max compression
+gzip compressed data, was "ZeroXRequests-1.1.tar", last modified: Sun May 26 15:33:47 2024, max compression
```

## Comparing `ZeroXRequests-1.0.tar` & `ZeroXRequests-1.1.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-26 15:01:18.761808 ZeroXRequests-1.0/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1360 2024-05-26 15:01:18.761808 ZeroXRequests-1.0/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      949 2022-12-17 16:10:31.000000 ZeroXRequests-1.0/README.md
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       90 2024-05-26 14:52:46.000000 ZeroXRequests-1.0/pyproject.toml
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2024-05-26 15:01:18.761808 ZeroXRequests-1.0/setup.cfg
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      681 2024-05-26 14:59:33.000000 ZeroXRequests-1.0/setup.py
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-26 15:01:18.761808 ZeroXRequests-1.0/src/
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-26 15:01:18.761808 ZeroXRequests-1.0/src/ZeroXRequests.egg-info/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     1360 2024-05-26 15:01:18.000000 ZeroXRequests-1.0/src/ZeroXRequests.egg-info/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      237 2024-05-26 15:01:18.000000 ZeroXRequests-1.0/src/ZeroXRequests.egg-info/SOURCES.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-05-26 15:01:18.000000 ZeroXRequests-1.0/src/ZeroXRequests.egg-info/dependency_links.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       12 2024-05-26 15:01:18.000000 ZeroXRequests-1.0/src/ZeroXRequests.egg-info/requires.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-05-26 15:01:18.000000 ZeroXRequests-1.0/src/ZeroXRequests.egg-info/top_level.txt
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-26 15:33:47.276222 ZeroXRequests-1.1/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1360 2024-05-26 15:33:47.276222 ZeroXRequests-1.1/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      949 2022-12-17 16:10:31.000000 ZeroXRequests-1.1/README.md
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       90 2024-05-26 14:52:46.000000 ZeroXRequests-1.1/pyproject.toml
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2024-05-26 15:33:47.276222 ZeroXRequests-1.1/setup.cfg
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      681 2024-05-26 15:33:02.000000 ZeroXRequests-1.1/setup.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-26 15:33:47.276222 ZeroXRequests-1.1/src/
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-26 15:33:47.276222 ZeroXRequests-1.1/src/ZeroXRequests/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     9498 2024-05-26 14:54:06.000000 ZeroXRequests-1.1/src/ZeroXRequests/RawRequests.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     6394 2024-05-26 14:54:01.000000 ZeroXRequests-1.1/src/ZeroXRequests/RequestUtils.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      247 2024-05-26 14:53:41.000000 ZeroXRequests-1.1/src/ZeroXRequests/__init__.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2024-05-26 15:33:47.276222 ZeroXRequests-1.1/src/ZeroXRequests.egg-info/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1360 2024-05-26 15:33:47.000000 ZeroXRequests-1.1/src/ZeroXRequests.egg-info/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      334 2024-05-26 15:33:47.000000 ZeroXRequests-1.1/src/ZeroXRequests.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2024-05-26 15:33:47.000000 ZeroXRequests-1.1/src/ZeroXRequests.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       12 2024-05-26 15:33:47.000000 ZeroXRequests-1.1/src/ZeroXRequests.egg-info/requires.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       14 2024-05-26 15:33:47.000000 ZeroXRequests-1.1/src/ZeroXRequests.egg-info/top_level.txt
```

### Comparing `ZeroXRequests-1.0/PKG-INFO` & `ZeroXRequests-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZeroXRequests
-Version: 1.0
+Version: 1.1
 Summary: Requests for hackers
 Home-page: https://github.com/rafax00/ZeroXRequests
 Author: Rafax00
 Author-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ZeroXRequests-1.0/README.md` & `ZeroXRequests-1.1/README.md`

 * *Files identical despite different names*

### Comparing `ZeroXRequests-1.0/setup.py` & `ZeroXRequests-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ZeroXRequests',
-    version='1.0',
+    version='1.1',
     description='Requests for hackers',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rafax00/ZeroXRequests',
     author='Rafax00',
     author_email='',
     license='MIT',
```

### Comparing `ZeroXRequests-1.0/src/ZeroXRequests.egg-info/PKG-INFO` & `ZeroXRequests-1.1/src/ZeroXRequests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZeroXRequests
-Version: 1.0
+Version: 1.1
 Summary: Requests for hackers
 Home-page: https://github.com/rafax00/ZeroXRequests
 Author: Rafax00
 Author-email: 
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

