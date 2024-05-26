# Comparing `tmp/xssbase-2.0.4.tar.gz` & `tmp/xssbase-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-2.0.4.tar", last modified: Sun May 26 10:03:31 2024, max compression
+gzip compressed data, was "xssbase-2.0.5.tar", last modified: Sun May 26 10:06:10 2024, max compression
```

## Comparing `xssbase-2.0.4.tar` & `xssbase-2.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 10:03:31.760531 xssbase-2.0.4/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.4/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-26 10:03:31.760531 xssbase-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 10:03:31.760531 xssbase-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-26 10:03:14.000000 xssbase-2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:03:31.738371 xssbase-2.0.4/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.4/xssbase/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-05-26 10:03:05.000000 xssbase-2.0.4/xssbase/cli.py
--rw-rw-rw-   0        0        0     2411 2024-05-26 10:02:40.000000 xssbase-2.0.4/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.4/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:03:31.760531 xssbase-2.0.4/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 10:06:10.473311 xssbase-2.0.5/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 10:06:10.457691 xssbase-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:06:10.473311 xssbase-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-26 10:05:58.000000 xssbase-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:06:10.442068 xssbase-2.0.5/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.5/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-05-26 10:03:05.000000 xssbase-2.0.5/xssbase/cli.py
+-rw-rw-rw-   0        0        0     2598 2024-05-26 10:05:52.000000 xssbase-2.0.5/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.5/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:06:10.457691 xssbase-2.0.5/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 10:06:10.000000 xssbase-2.0.5/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 10:06:10.000000 xssbase-2.0.5/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:06:10.000000 xssbase-2.0.5/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 10:06:10.000000 xssbase-2.0.5/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 10:06:10.000000 xssbase-2.0.5/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 10:06:10.000000 xssbase-2.0.5/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-2.0.4/LICENSE` & `xssbase-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.4/PKG-INFO` & `xssbase-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.4
+Version: 2.0.5
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-2.0.4/setup.py` & `xssbase-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='2.0.4',
+    version='2.0.5',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-2.0.4/xssbase/cli.py` & `xssbase-2.0.5/xssbase/cli.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.4/xssbase/utils.py` & `xssbase-2.0.5/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.4/xssbase.egg-info/PKG-INFO` & `xssbase-2.0.5/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.4
+Version: 2.0.5
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

