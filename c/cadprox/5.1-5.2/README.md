# Comparing `tmp/cadprox-5.1.tar.gz` & `tmp/cadprox-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-5.1.tar", last modified: Sun May 26 09:13:47 2024, max compression
+gzip compressed data, was "cadprox-5.2.tar", last modified: Sun May 26 09:17:26 2024, max compression
```

## Comparing `cadprox-5.1.tar` & `cadprox-5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:13:47.367058 cadprox-5.1/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-5.1/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:13:47.367058 cadprox-5.1/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-5.1/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:13:47.351058 cadprox-5.1/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-5.1/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     5072 2024-05-26 09:13:27.000000 cadprox-5.1/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    15082 2024-05-26 09:13:14.000000 cadprox-5.1/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:13:47.363058 cadprox-5.1/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 09:13:47.000000 cadprox-5.1/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 09:13:47.367058 cadprox-5.1/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 09:13:42.000000 cadprox-5.1/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:17:26.358988 cadprox-5.2/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-5.2/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:17:26.358988 cadprox-5.2/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-5.2/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:17:26.342987 cadprox-5.2/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-5.2/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     5237 2024-05-26 09:17:15.000000 cadprox-5.2/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    15082 2024-05-26 09:13:14.000000 cadprox-5.2/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 09:17:26.354987 cadprox-5.2/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 09:17:26.000000 cadprox-5.2/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 09:17:26.358988 cadprox-5.2/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 09:17:21.000000 cadprox-5.2/setup.py
```

### Comparing `cadprox-5.1/PKG-INFO` & `cadprox-5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 5.1
+Version: 5.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-5.1/README.md` & `cadprox-5.2/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-5.1/app/main.py` & `cadprox-5.2/app/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import argparse
 import os
 import sys
 import boto3
+import logging
+
+# Configure logging
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+logger = logging.getLogger(__name__)
 
 from .utils import (
     get_external_ip,
     add_dns_record,
     download_caddyfile_from_s3,
     upload_caddyfile_to_s3,
     update_caddyfile,
```

### Comparing `cadprox-5.1/app/utils.py` & `cadprox-5.2/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-5.1/cadprox.egg-info/PKG-INFO` & `cadprox-5.2/cadprox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 5.1
+Version: 5.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-5.1/setup.py` & `cadprox-5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=5.1,
+    version=5.2,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

