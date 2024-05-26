# Comparing `tmp/cadprox-4.9.tar.gz` & `tmp/cadprox-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-4.9.tar", last modified: Sun May 26 08:51:52 2024, max compression
+gzip compressed data, was "cadprox-5.tar", last modified: Sun May 26 08:59:12 2024, max compression
```

## Comparing `cadprox-4.9.tar` & `cadprox-5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:51:52.154297 cadprox-4.9/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.9/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:51:52.150297 cadprox-4.9/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-4.9/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:51:52.134297 cadprox-4.9/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.9/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     4964 2024-05-26 08:51:37.000000 cadprox-4.9/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    14990 2024-05-26 08:51:27.000000 cadprox-4.9/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:51:52.150297 cadprox-4.9/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     5351 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 08:51:52.000000 cadprox-4.9/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 08:51:52.154297 cadprox-4.9/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2563 2024-05-26 08:51:44.000000 cadprox-4.9/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:59:12.332359 cadprox-5/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-5/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     5349 2024-05-26 08:59:12.332359 cadprox-5/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4769 2024-05-25 06:52:13.000000 cadprox-5/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:59:12.316359 cadprox-5/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-5/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4964 2024-05-26 08:58:56.000000 cadprox-5/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    14990 2024-05-26 08:58:40.000000 cadprox-5/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 08:59:12.332359 cadprox-5/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     5349 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 08:59:12.000000 cadprox-5/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 08:59:12.336359 cadprox-5/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2561 2024-05-26 08:59:02.000000 cadprox-5/setup.py
```

### Comparing `cadprox-4.9/PKG-INFO` & `cadprox-5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.9
+Version: 5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.9/README.md` & `cadprox-5/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-4.9/app/main.py` & `cadprox-5/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-4.9/app/utils.py` & `cadprox-5/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-4.9/cadprox.egg-info/PKG-INFO` & `cadprox-5/cadprox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.9
+Version: 5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.9/setup.py` & `cadprox-5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 # Read the version from version.txt
 with open("version.txt") as version_file:
     version = version_file.read().strip()
 
 setup(
     name='cadprox',
-    version=4.9,
+    version=5,
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

