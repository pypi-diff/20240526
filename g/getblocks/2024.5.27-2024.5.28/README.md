# Comparing `tmp/getblocks-2024.5.27.tar.gz` & `tmp/getblocks-2024.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getblocks-2024.5.27.tar", last modified: Sat May 25 23:16:45 2024, max compression
+gzip compressed data, was "getblocks-2024.5.28.tar", last modified: Sat May 25 23:42:54 2024, max compression
```

## Comparing `getblocks-2024.5.27.tar` & `getblocks-2024.5.28.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:16:45.398188 getblocks-2024.5.27/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 23:16:36.000000 getblocks-2024.5.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 23:16:45.398188 getblocks-2024.5.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-25 23:16:36.000000 getblocks-2024.5.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:16:45.398188 getblocks-2024.5.27/getblocks/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 23:16:36.000000 getblocks-2024.5.27/getblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 23:16:36.000000 getblocks-2024.5.27/getblocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-25 23:16:36.000000 getblocks-2024.5.27/getblocks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:16:45.398188 getblocks-2024.5.27/getblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:16:45.398188 getblocks-2024.5.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 23:16:36.000000 getblocks-2024.5.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:42:54.513433 getblocks-2024.5.28/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 23:42:50.000000 getblocks-2024.5.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 23:42:54.513433 getblocks-2024.5.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-25 23:42:50.000000 getblocks-2024.5.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:42:54.509433 getblocks-2024.5.28/getblocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 23:42:50.000000 getblocks-2024.5.28/getblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 23:42:50.000000 getblocks-2024.5.28/getblocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-05-25 23:42:50.000000 getblocks-2024.5.28/getblocks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:42:54.513433 getblocks-2024.5.28/getblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 23:42:54.000000 getblocks-2024.5.28/getblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 23:42:54.000000 getblocks-2024.5.28/getblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:42:54.000000 getblocks-2024.5.28/getblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 23:42:54.000000 getblocks-2024.5.28/getblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:42:54.000000 getblocks-2024.5.28/getblocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 23:42:54.000000 getblocks-2024.5.28/getblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 23:42:54.000000 getblocks-2024.5.28/getblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:42:54.513433 getblocks-2024.5.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 23:42:50.000000 getblocks-2024.5.28/setup.py
```

### Comparing `getblocks-2024.5.27/LICENSE` & `getblocks-2024.5.28/LICENSE`

 * *Files identical despite different names*

### Comparing `getblocks-2024.5.27/PKG-INFO` & `getblocks-2024.5.28/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.5.27
+Version: 2024.5.28
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/4n6ir/getblocks
 Author: John Lukach
 Author-email: hello@4n6ir.com
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `getblocks-2024.5.27/README.md` & `getblocks-2024.5.28/README.md`

 * *Files identical despite different names*

### Comparing `getblocks-2024.5.27/getblocks/cli.py` & `getblocks-2024.5.28/getblocks/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import concurrent.futures
 import gzip
 import hashlib
 import math
 import platform
 import requests
 import shutil
-import time
 from blake3 import blake3
 from getblocks import __version__
 from pathlib import Path, PurePath
 
 def hasher(fname):
 
     try:
@@ -255,12 +254,11 @@
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
         executor.submit(start, amiid)
 
     with open(amiid+'.txt', 'rb') as f_in:
         with gzip.open(amiid+'.txt.gz', 'wb') as f_out:
             shutil.copyfileobj(f_in, f_out)
-            time.sleep(60)
         f_out.close()
     f_in.close()
 
     print('    Done!!')
```

### Comparing `getblocks-2024.5.27/getblocks.egg-info/PKG-INFO` & `getblocks-2024.5.28/getblocks.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.5.27
+Version: 2024.5.28
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/4n6ir/getblocks
 Author: John Lukach
 Author-email: hello@4n6ir.com
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `getblocks-2024.5.27/setup.py` & `getblocks-2024.5.28/setup.py`

 * *Files identical despite different names*

