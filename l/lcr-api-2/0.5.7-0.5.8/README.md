# Comparing `tmp/lcr_api_2-0.5.7.tar.gz` & `tmp/lcr_api_2-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcr_api_2-0.5.7.tar", last modified: Sun May 26 19:43:55 2024, max compression
+gzip compressed data, was "lcr_api_2-0.5.8.tar", last modified: Sun May 26 19:55:10 2024, max compression
```

## Comparing `lcr_api_2-0.5.7.tar` & `lcr_api_2-0.5.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2024-05-26 19:43:55.882904 lcr_api_2-0.5.7/
--rw-r--r--   0 sirsmith   (505) staff       (20)     1773 2024-05-26 19:43:55.882415 lcr_api_2-0.5.7/PKG-INFO
--rwxr-xr-x   0 sirsmith   (505) staff       (20)     1350 2022-08-07 14:17:59.000000 lcr_api_2-0.5.7/README.md
-drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2024-05-26 19:43:55.877870 lcr_api_2-0.5.7/lcr/
--rw-r--r--   0 sirsmith   (505) staff       (20)     8168 2024-05-26 19:40:51.000000 lcr_api_2-0.5.7/lcr/__init__.py
-drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2024-05-26 19:43:55.881876 lcr_api_2-0.5.7/lcr_api_2.egg-info/
--rw-r--r--   0 sirsmith   (505) staff       (20)     1773 2024-05-26 19:43:55.000000 lcr_api_2-0.5.7/lcr_api_2.egg-info/PKG-INFO
--rw-r--r--   0 sirsmith   (505) staff       (20)      248 2024-05-26 19:43:55.000000 lcr_api_2-0.5.7/lcr_api_2.egg-info/SOURCES.txt
--rw-r--r--   0 sirsmith   (505) staff       (20)        1 2024-05-26 19:43:55.000000 lcr_api_2-0.5.7/lcr_api_2.egg-info/dependency_links.txt
--rw-r--r--   0 sirsmith   (505) staff       (20)        1 2022-07-17 21:42:15.000000 lcr_api_2-0.5.7/lcr_api_2.egg-info/not-zip-safe
--rw-r--r--   0 sirsmith   (505) staff       (20)       15 2024-05-26 19:43:55.000000 lcr_api_2-0.5.7/lcr_api_2.egg-info/requires.txt
--rw-r--r--   0 sirsmith   (505) staff       (20)        4 2024-05-26 19:43:55.000000 lcr_api_2-0.5.7/lcr_api_2.egg-info/top_level.txt
--rw-r--r--   0 sirsmith   (505) staff       (20)       38 2024-05-26 19:43:55.883031 lcr_api_2-0.5.7/setup.cfg
--rwxr-xr-x   0 sirsmith   (505) staff       (20)     1092 2024-03-31 17:25:43.000000 lcr_api_2-0.5.7/setup.py
-drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2024-05-26 19:43:55.880945 lcr_api_2-0.5.7/tests/
--rw-r--r--   0 sirsmith   (505) staff       (20)     5780 2022-07-17 21:41:43.000000 lcr_api_2-0.5.7/tests/test_all.py
+drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2024-05-26 19:55:10.339654 lcr_api_2-0.5.8/
+-rw-r--r--   0 sirsmith   (505) staff       (20)     1773 2024-05-26 19:55:10.337970 lcr_api_2-0.5.8/PKG-INFO
+-rwxr-xr-x   0 sirsmith   (505) staff       (20)     1350 2022-08-07 14:17:59.000000 lcr_api_2-0.5.8/README.md
+drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2024-05-26 19:55:10.327898 lcr_api_2-0.5.8/lcr/
+-rw-r--r--   0 sirsmith   (505) staff       (20)     8168 2024-05-26 19:40:51.000000 lcr_api_2-0.5.8/lcr/__init__.py
+drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2024-05-26 19:55:10.335855 lcr_api_2-0.5.8/lcr_api_2.egg-info/
+-rw-r--r--   0 sirsmith   (505) staff       (20)     1773 2024-05-26 19:55:10.000000 lcr_api_2-0.5.8/lcr_api_2.egg-info/PKG-INFO
+-rw-r--r--   0 sirsmith   (505) staff       (20)      248 2024-05-26 19:55:10.000000 lcr_api_2-0.5.8/lcr_api_2.egg-info/SOURCES.txt
+-rw-r--r--   0 sirsmith   (505) staff       (20)        1 2024-05-26 19:55:10.000000 lcr_api_2-0.5.8/lcr_api_2.egg-info/dependency_links.txt
+-rw-r--r--   0 sirsmith   (505) staff       (20)        1 2022-07-17 21:42:15.000000 lcr_api_2-0.5.8/lcr_api_2.egg-info/not-zip-safe
+-rw-r--r--   0 sirsmith   (505) staff       (20)       15 2024-05-26 19:55:10.000000 lcr_api_2-0.5.8/lcr_api_2.egg-info/requires.txt
+-rw-r--r--   0 sirsmith   (505) staff       (20)        4 2024-05-26 19:55:10.000000 lcr_api_2-0.5.8/lcr_api_2.egg-info/top_level.txt
+-rw-r--r--   0 sirsmith   (505) staff       (20)       38 2024-05-26 19:55:10.339917 lcr_api_2-0.5.8/setup.cfg
+-rwxr-xr-x   0 sirsmith   (505) staff       (20)     1092 2024-05-26 19:49:59.000000 lcr_api_2-0.5.8/setup.py
+drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2024-05-26 19:55:10.334283 lcr_api_2-0.5.8/tests/
+-rw-r--r--   0 sirsmith   (505) staff       (20)     5780 2022-07-17 21:41:43.000000 lcr_api_2-0.5.8/tests/test_all.py
```

### Comparing `lcr_api_2-0.5.7/PKG-INFO` & `lcr_api_2-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lcr-api-2
-Version: 0.5.7
+Version: 0.5.8
 Summary: An API for the LDS churches Leader and Clerk Resources (LCR),
 Home-page: https://github.com/SpencerMKSmith/LCR-API-2
-Download-URL: https://github.com/SpencerMKSmith/LCR-API-2/archive/v0.5.7.zip
+Download-URL: https://github.com/SpencerMKSmith/LCR-API-2/archive/v0.5.8.zip
 Author: Spencer Smith
 Author-email: spencermksmith@gmail.com
 License: MIT License
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: requests<3,>=2
```

### Comparing `lcr_api_2-0.5.7/README.md` & `lcr_api_2-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `lcr_api_2-0.5.7/lcr/__init__.py` & `lcr_api_2-0.5.8/lcr/__init__.py`

 * *Files identical despite different names*

### Comparing `lcr_api_2-0.5.7/lcr_api_2.egg-info/PKG-INFO` & `lcr_api_2-0.5.8/lcr_api_2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lcr-api-2
-Version: 0.5.7
+Version: 0.5.8
 Summary: An API for the LDS churches Leader and Clerk Resources (LCR),
 Home-page: https://github.com/SpencerMKSmith/LCR-API-2
-Download-URL: https://github.com/SpencerMKSmith/LCR-API-2/archive/v0.5.7.zip
+Download-URL: https://github.com/SpencerMKSmith/LCR-API-2/archive/v0.5.8.zip
 Author: Spencer Smith
 Author-email: spencermksmith@gmail.com
 License: MIT License
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: requests<3,>=2
```

### Comparing `lcr_api_2-0.5.7/setup.py` & `lcr_api_2-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 import os
 from setuptools import setup, find_packages
 
-VERSION = 'v0.5.7'
+VERSION = 'v0.5.8'
 PACKAGE_NAME = 'lcr-api-2'
 HERE = os.path.abspath(os.path.dirname(__file__))
 DOWNLOAD_URL = ('https://github.com/SpencerMKSmith/LCR-API-2/archive/'
                 '{}.zip'.format(VERSION))
 
 PACKAGES = find_packages(exclude=['tests', 'tests.*'])
```

### Comparing `lcr_api_2-0.5.7/tests/test_all.py` & `lcr_api_2-0.5.8/tests/test_all.py`

 * *Files identical despite different names*

