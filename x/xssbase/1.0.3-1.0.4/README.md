# Comparing `tmp/xssbase-1.0.3.tar.gz` & `tmp/xssbase-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-1.0.3.tar", last modified: Sun May 26 06:55:47 2024, max compression
+gzip compressed data, was "xssbase-1.0.4.tar", last modified: Sun May 26 07:19:58 2024, max compression
```

## Comparing `xssbase-1.0.3.tar` & `xssbase-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 06:55:47.656856 xssbase-1.0.3/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-26 06:55:47.655880 xssbase-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 06:55:47.657833 xssbase-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-26 06:54:44.000000 xssbase-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 06:55:47.627416 xssbase-1.0.3/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-1.0.3/xssbase/__init__.py
--rw-rw-rw-   0        0        0      859 2024-05-26 06:44:56.000000 xssbase-1.0.3/xssbase/cli.py
--rw-rw-rw-   0        0        0     2288 2024-05-26 06:45:27.000000 xssbase-1.0.3/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 06:46:00.000000 xssbase-1.0.3/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 06:55:47.654905 xssbase-1.0.3/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-26 06:55:47.000000 xssbase-1.0.3/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 06:55:47.000000 xssbase-1.0.3/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 06:55:47.000000 xssbase-1.0.3/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 06:55:47.000000 xssbase-1.0.3/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 06:55:47.000000 xssbase-1.0.3/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 06:55:47.000000 xssbase-1.0.3/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 07:19:58.213657 xssbase-1.0.4/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 07:19:58.212680 xssbase-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 07:19:58.214644 xssbase-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-26 07:18:29.000000 xssbase-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 07:19:58.182428 xssbase-1.0.4/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-1.0.4/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     1061 2024-05-26 07:18:19.000000 xssbase-1.0.4/xssbase/cli.py
+-rw-rw-rw-   0        0        0     2288 2024-05-26 06:45:27.000000 xssbase-1.0.4/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 06:46:00.000000 xssbase-1.0.4/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 07:19:58.210742 xssbase-1.0.4/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 07:19:58.000000 xssbase-1.0.4/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-1.0.3/LICENSE` & `xssbase-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.3/PKG-INFO` & `xssbase-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.3
+Version: 1.0.4
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-1.0.3/setup.py` & `xssbase-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='1.0.3',
+    version='1.0.4',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-1.0.3/xssbase/cli.py` & `xssbase-1.0.4/xssbase/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import argparse
-from .main import test_xss_payloads
-from .utils import download_chromedriver
+import os
+import sys
+import platform
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
+from .main import test_xss_payloads
+from .utils import download_chromedriver
 
 def main():
+    # Check if the operating system is Windows
+    if platform.system() != 'Windows':
+        print("This tool only supports Windows.")
+        sys.exit(1)
+
     parser = argparse.ArgumentParser(description="XSS testing tool")
     parser.add_argument('--url', required=True, help='URL to test for XSS vulnerability')
     args = parser.parse_args()
 
     # Download the chromedriver if it doesn't exist
     download_chromedriver()
```

### Comparing `xssbase-1.0.3/xssbase/main.py` & `xssbase-1.0.4/xssbase/main.py`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.3/xssbase/utils.py` & `xssbase-1.0.4/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.3/xssbase.egg-info/PKG-INFO` & `xssbase-1.0.4/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.3
+Version: 1.0.4
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

