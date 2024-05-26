# Comparing `tmp/xssbase-1.0.1.tar.gz` & `tmp/xssbase-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-1.0.1.tar", last modified: Tue May 21 19:46:58 2024, max compression
+gzip compressed data, was "xssbase-1.0.2.tar", last modified: Sun May 26 06:48:15 2024, max compression
```

## Comparing `xssbase-1.0.1.tar` & `xssbase-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 19:46:58.384102 xssbase-1.0.1/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-21 19:46:58.384102 xssbase-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 19:46:58.384102 xssbase-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1036 2024-05-21 19:45:33.000000 xssbase-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:46:58.321612 xssbase-1.0.1/xssbase/
--rw-rw-rw-   0        0        0       80 2024-05-21 19:45:32.000000 xssbase-1.0.1/xssbase/__init__.py
--rw-rw-rw-   0        0        0     1418 2024-05-21 19:45:32.000000 xssbase-1.0.1/xssbase/cli.py
--rw-rw-rw-   0        0        0     7551 2024-05-21 19:45:33.000000 xssbase-1.0.1/xssbase/xssbase.py
-drwxrwxrwx   0        0        0        0 2024-05-21 19:46:58.384102 xssbase-1.0.1/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-21 19:46:58.000000 xssbase-1.0.1/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-21 19:46:58.000000 xssbase-1.0.1/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 19:46:58.000000 xssbase-1.0.1/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-21 19:46:58.000000 xssbase-1.0.1/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2024-05-21 19:46:58.000000 xssbase-1.0.1/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-21 19:46:58.000000 xssbase-1.0.1/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 06:48:15.001833 xssbase-1.0.2/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 06:48:15.001833 xssbase-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 06:48:15.001833 xssbase-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2024-05-26 06:41:19.000000 xssbase-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 06:48:14.954971 xssbase-1.0.2/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-1.0.2/xssbase/__init__.py
+-rw-rw-rw-   0        0        0      859 2024-05-26 06:44:56.000000 xssbase-1.0.2/xssbase/cli.py
+-rw-rw-rw-   0        0        0     2288 2024-05-26 06:45:27.000000 xssbase-1.0.2/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 06:46:00.000000 xssbase-1.0.2/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 06:48:15.001833 xssbase-1.0.2/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 06:48:14.000000 xssbase-1.0.2/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 06:48:14.000000 xssbase-1.0.2/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 06:48:14.000000 xssbase-1.0.2/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 06:48:14.000000 xssbase-1.0.2/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2024-05-26 06:48:14.000000 xssbase-1.0.2/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 06:48:14.000000 xssbase-1.0.2/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-1.0.1/LICENSE` & `xssbase-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.1/PKG-INFO` & `xssbase-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.1
+Version: 1.0.2
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-1.0.1/setup.py` & `xssbase-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='1.0.1',
+    version='1.0.2',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-1.0.1/xssbase.egg-info/PKG-INFO` & `xssbase-1.0.2/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.1
+Version: 1.0.2
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

