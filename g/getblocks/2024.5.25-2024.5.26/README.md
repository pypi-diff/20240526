# Comparing `tmp/getblocks-2024.5.25.tar.gz` & `tmp/getblocks-2024.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getblocks-2024.5.25.tar", last modified: Sat May 25 18:41:13 2024, max compression
+gzip compressed data, was "getblocks-2024.5.26.tar", last modified: Sat May 25 22:47:54 2024, max compression
```

## Comparing `getblocks-2024.5.25.tar` & `getblocks-2024.5.26.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:41:13.746012 getblocks-2024.5.25/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 18:41:09.000000 getblocks-2024.5.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 18:41:13.746012 getblocks-2024.5.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-25 18:41:09.000000 getblocks-2024.5.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:41:13.742012 getblocks-2024.5.25/getblocks/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 18:41:09.000000 getblocks-2024.5.25/getblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 18:41:09.000000 getblocks-2024.5.25/getblocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-25 18:41:09.000000 getblocks-2024.5.25/getblocks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:41:13.746012 getblocks-2024.5.25/getblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 18:41:13.000000 getblocks-2024.5.25/getblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 18:41:13.746012 getblocks-2024.5.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 18:41:09.000000 getblocks-2024.5.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:47:54.484567 getblocks-2024.5.26/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 22:47:50.000000 getblocks-2024.5.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 22:47:54.484567 getblocks-2024.5.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-25 22:47:50.000000 getblocks-2024.5.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:47:54.480567 getblocks-2024.5.26/getblocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 22:47:50.000000 getblocks-2024.5.26/getblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 22:47:50.000000 getblocks-2024.5.26/getblocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-25 22:47:50.000000 getblocks-2024.5.26/getblocks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:47:54.484567 getblocks-2024.5.26/getblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 22:47:54.484567 getblocks-2024.5.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 22:47:50.000000 getblocks-2024.5.26/setup.py
```

### Comparing `getblocks-2024.5.25/LICENSE` & `getblocks-2024.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `getblocks-2024.5.25/PKG-INFO` & `getblocks-2024.5.26/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.5.25
+Version: 2024.5.26
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/4n6ir/getblocks
 Author: John Lukach
 Author-email: hello@4n6ir.com
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `getblocks-2024.5.25/README.md` & `getblocks-2024.5.26/README.md`

 * *Files identical despite different names*

### Comparing `getblocks-2024.5.25/getblocks/cli.py` & `getblocks-2024.5.26/getblocks/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import concurrent.futures
 import gzip
 import hashlib
 import math
 import platform
 import requests
 import shutil
+import time
 from blake3 import blake3
 from getblocks import __version__
 from pathlib import Path, PurePath
 
 def hasher(fname):
 
     try:
@@ -222,14 +223,15 @@
                                             block = sector(s,count)
                                             parse = block.split('|')
                                             f.write(str(out[0])+'|-|-|'+str(out[3])+'|-|-|'+str(out[6])+'|-|-|-|-|-|-|-|-|-|SECTOR|'+str(parse[0])+'|'+str(parse[1])+'|'+str(location)+'\n')
                                         except:
                                             pass
                                         count = count + 512
                                         location = location + 1
+    f.close()
 
 def main():
 
     print('GETBLOCKS v'+__version__)
 
     ### Instance Metadata Service Version 2 (IMDSv2) ###
 
@@ -250,12 +252,14 @@
         pass
 
     print('  '+amiid)
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
         executor.submit(start, amiid)
 
+    time.sleep(30)
+
     with open(amiid+'.txt', 'rb') as f_in:
         with gzip.open(amiid+'.txt.gz', 'wb') as f_out:
             shutil.copyfileobj(f_in, f_out)
 
     print('    Done!!')
```

### Comparing `getblocks-2024.5.25/getblocks.egg-info/PKG-INFO` & `getblocks-2024.5.26/getblocks.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.5.25
+Version: 2024.5.26
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/4n6ir/getblocks
 Author: John Lukach
 Author-email: hello@4n6ir.com
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `getblocks-2024.5.25/setup.py` & `getblocks-2024.5.26/setup.py`

 * *Files identical despite different names*

