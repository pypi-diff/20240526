# Comparing `tmp/getblocks-2024.5.26.tar.gz` & `tmp/getblocks-2024.5.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getblocks-2024.5.26.tar", last modified: Sat May 25 22:47:54 2024, max compression
+gzip compressed data, was "getblocks-2024.5.27.tar", last modified: Sat May 25 23:16:45 2024, max compression
```

## Comparing `getblocks-2024.5.26.tar` & `getblocks-2024.5.27.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:47:54.484567 getblocks-2024.5.26/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 22:47:50.000000 getblocks-2024.5.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 22:47:54.484567 getblocks-2024.5.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-25 22:47:50.000000 getblocks-2024.5.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:47:54.480567 getblocks-2024.5.26/getblocks/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 22:47:50.000000 getblocks-2024.5.26/getblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 22:47:50.000000 getblocks-2024.5.26/getblocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-25 22:47:50.000000 getblocks-2024.5.26/getblocks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:47:54.484567 getblocks-2024.5.26/getblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 22:47:54.000000 getblocks-2024.5.26/getblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 22:47:54.484567 getblocks-2024.5.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 22:47:50.000000 getblocks-2024.5.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:16:45.398188 getblocks-2024.5.27/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 23:16:36.000000 getblocks-2024.5.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 23:16:45.398188 getblocks-2024.5.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-25 23:16:36.000000 getblocks-2024.5.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:16:45.398188 getblocks-2024.5.27/getblocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 23:16:36.000000 getblocks-2024.5.27/getblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 23:16:36.000000 getblocks-2024.5.27/getblocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-25 23:16:36.000000 getblocks-2024.5.27/getblocks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:16:45.398188 getblocks-2024.5.27/getblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 23:16:45.000000 getblocks-2024.5.27/getblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:16:45.398188 getblocks-2024.5.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-25 23:16:36.000000 getblocks-2024.5.27/setup.py
```

### Comparing `getblocks-2024.5.26/LICENSE` & `getblocks-2024.5.27/LICENSE`

 * *Files identical despite different names*

### Comparing `getblocks-2024.5.26/PKG-INFO` & `getblocks-2024.5.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.5.26
+Version: 2024.5.27
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/4n6ir/getblocks
 Author: John Lukach
 Author-email: hello@4n6ir.com
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `getblocks-2024.5.26/README.md` & `getblocks-2024.5.27/README.md`

 * *Files identical despite different names*

### Comparing `getblocks-2024.5.26/getblocks/cli.py` & `getblocks-2024.5.27/getblocks/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,15 @@
         pass
 
     print('  '+amiid)
 
     with concurrent.futures.ThreadPoolExecutor() as executor:
         executor.submit(start, amiid)
 
-    time.sleep(30)
-
     with open(amiid+'.txt', 'rb') as f_in:
         with gzip.open(amiid+'.txt.gz', 'wb') as f_out:
             shutil.copyfileobj(f_in, f_out)
+            time.sleep(60)
+        f_out.close()
+    f_in.close()
 
     print('    Done!!')
```

### Comparing `getblocks-2024.5.26/getblocks.egg-info/PKG-INFO` & `getblocks-2024.5.27/getblocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.5.26
+Version: 2024.5.27
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/4n6ir/getblocks
 Author: John Lukach
 Author-email: hello@4n6ir.com
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `getblocks-2024.5.26/setup.py` & `getblocks-2024.5.27/setup.py`

 * *Files identical despite different names*

