# Comparing `tmp/oahspe-0.0.2.tar.gz` & `tmp/oahspe-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oahspe-0.0.2.tar", last modified: Sun May 26 13:51:24 2024, max compression
+gzip compressed data, was "oahspe-0.0.3.tar", last modified: Sun May 26 14:03:09 2024, max compression
```

## Comparing `oahspe-0.0.2.tar` & `oahspe-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-26 13:51:24.055180 oahspe-0.0.2/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-26 13:20:10.000000 oahspe-0.0.2/LICENSE.txt
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-26 13:51:24.055180 oahspe-0.0.2/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-26 13:43:14.000000 oahspe-0.0.2/README.md
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-26 13:51:24.055180 oahspe-0.0.2/oahspe/
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3840 2024-05-26 13:20:10.000000 oahspe-0.0.2/oahspe/SSL.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    12967 2024-05-26 13:20:10.000000 oahspe-0.0.2/oahspe/crypt.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-26 13:20:10.000000 oahspe-0.0.2/oahspe/host.py
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     4648 2024-05-26 13:20:10.000000 oahspe-0.0.2/oahspe/tool.py
-drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-26 13:51:24.055180 oahspe-0.0.2/oahspe.egg-info/
--rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-26 13:51:24.000000 oahspe-0.0.2/oahspe.egg-info/PKG-INFO
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      220 2024-05-26 13:51:24.000000 oahspe-0.0.2/oahspe.egg-info/SOURCES.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-26 13:51:24.000000 oahspe-0.0.2/oahspe.egg-info/dependency_links.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-26 13:51:24.000000 oahspe-0.0.2/oahspe.egg-info/top_level.txt
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-26 13:51:24.055180 oahspe-0.0.2/setup.cfg
--rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-26 13:45:30.000000 oahspe-0.0.2/setup.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-26 14:03:09.791261 oahspe-0.0.3/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1066 2024-05-26 13:20:10.000000 oahspe-0.0.3/LICENSE.txt
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-26 14:03:09.791261 oahspe-0.0.3/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        9 2024-05-26 13:43:14.000000 oahspe-0.0.3/README.md
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-26 14:03:09.791261 oahspe-0.0.3/oahspe/
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     3840 2024-05-26 13:20:10.000000 oahspe-0.0.3/oahspe/SSL.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)    12967 2024-05-26 13:20:10.000000 oahspe-0.0.3/oahspe/crypt.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     1925 2024-05-26 13:20:10.000000 oahspe-0.0.3/oahspe/host.py
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)     4648 2024-05-26 13:20:10.000000 oahspe-0.0.3/oahspe/tool.py
+drwxrwxr-x   0 vt_admin  (1000) vt_admin  (1000)        0 2024-05-26 14:03:09.791261 oahspe-0.0.3/oahspe.egg-info/
+-rw-r--r--   0 vt_admin  (1000) vt_admin  (1000)      548 2024-05-26 14:03:09.000000 oahspe-0.0.3/oahspe.egg-info/PKG-INFO
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      220 2024-05-26 14:03:09.000000 oahspe-0.0.3/oahspe.egg-info/SOURCES.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        1 2024-05-26 14:03:09.000000 oahspe-0.0.3/oahspe.egg-info/dependency_links.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)        7 2024-05-26 14:03:09.000000 oahspe-0.0.3/oahspe.egg-info/top_level.txt
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)       38 2024-05-26 14:03:09.791261 oahspe-0.0.3/setup.cfg
+-rw-rw-r--   0 vt_admin  (1000) vt_admin  (1000)      640 2024-05-26 14:03:08.000000 oahspe-0.0.3/setup.py
```

### Comparing `oahspe-0.0.2/LICENSE.txt` & `oahspe-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.2/PKG-INFO` & `oahspe-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.2/oahspe/SSL.py` & `oahspe-0.0.3/oahspe/SSL.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.2/oahspe/crypt.py` & `oahspe-0.0.3/oahspe/crypt.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.2/oahspe/host.py` & `oahspe-0.0.3/oahspe/host.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.2/oahspe/tool.py` & `oahspe-0.0.3/oahspe/tool.py`

 * *Files identical despite different names*

### Comparing `oahspe-0.0.2/oahspe.egg-info/PKG-INFO` & `oahspe-0.0.3/oahspe.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oahspe
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cloud DevOps
 Home-page: https://github.com/quangproo/oahspe
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: quangproo
 Author-email: contact@quang.pro
 License: MIT
 Keywords: oahspe
```

### Comparing `oahspe-0.0.2/setup.py` & `oahspe-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 setup(
   name = 'oahspe',
   packages = ['oahspe'],
   keywords = ['oahspe'],
-  version = '0.0.2',
+  version = '0.0.3',
   author = 'quangproo',
   license='MIT',
   description = 'Cloud DevOps',
   author_email = 'contact@quang.pro',
   url = 'https://github.com/quangproo/oahspe',
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',
   install_requires = [],
```

