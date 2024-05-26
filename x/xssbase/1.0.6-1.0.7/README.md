# Comparing `tmp/xssbase-1.0.6.tar.gz` & `tmp/xssbase-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-1.0.6.tar", last modified: Sun May 26 09:19:44 2024, max compression
+gzip compressed data, was "xssbase-1.0.7.tar", last modified: Sun May 26 09:26:30 2024, max compression
```

## Comparing `xssbase-1.0.6.tar` & `xssbase-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 09:19:44.431487 xssbase-1.0.6/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-26 09:19:44.431487 xssbase-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 09:19:44.437994 xssbase-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-26 09:18:58.000000 xssbase-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:19:44.384624 xssbase-1.0.6/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-1.0.6/xssbase/__init__.py
--rw-rw-rw-   0        0        0     1061 2024-05-26 09:18:10.000000 xssbase-1.0.6/xssbase/cli.py
--rw-rw-rw-   0        0        0     2288 2024-05-26 09:18:44.000000 xssbase-1.0.6/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-1.0.6/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:19:44.415866 xssbase-1.0.6/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-26 09:19:44.000000 xssbase-1.0.6/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 09:19:44.000000 xssbase-1.0.6/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 09:19:44.000000 xssbase-1.0.6/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 09:19:44.000000 xssbase-1.0.6/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 09:19:44.000000 xssbase-1.0.6/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 09:19:44.000000 xssbase-1.0.6/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 09:26:30.619816 xssbase-1.0.7/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 09:26:30.619816 xssbase-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 09:26:30.619816 xssbase-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-26 09:26:17.000000 xssbase-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:26:30.572956 xssbase-1.0.7/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-1.0.7/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     1412 2024-05-26 09:26:11.000000 xssbase-1.0.7/xssbase/cli.py
+-rw-rw-rw-   0        0        0     2288 2024-05-26 09:18:44.000000 xssbase-1.0.7/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-1.0.7/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:26:30.619816 xssbase-1.0.7/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 09:26:30.000000 xssbase-1.0.7/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 09:26:30.000000 xssbase-1.0.7/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 09:26:30.000000 xssbase-1.0.7/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 09:26:30.000000 xssbase-1.0.7/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 09:26:30.000000 xssbase-1.0.7/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 09:26:30.000000 xssbase-1.0.7/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-1.0.6/LICENSE` & `xssbase-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.6/PKG-INFO` & `xssbase-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.6
+Version: 1.0.7
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-1.0.6/setup.py` & `xssbase-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='1.0.6',
+    version='1.0.7',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-1.0.6/xssbase/cli.py` & `xssbase-1.0.7/xssbase/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 
 def main():
     # Check if the operating system is Windows
     if platform.system() != 'Windows':
         print("This tool only supports Windows.")
         sys.exit(1)
 
-    parser = argparse.ArgumentParser(description="XSS testing tool")
+    # Define the argument parser
+    parser = argparse.ArgumentParser(
+        description="XSSbase - A professional tool for scanning XSS vulnerabilities.",
+        epilog="Author: Fidal\nEmail: mrfidal@proton.me\nGitHub: https://github.com/mr-fidal\n\n"
+               "Copyright 2024 Fidal. All rights reserved. "
+               "Unauthorized copying of this tool, via any medium is strictly prohibited."
+    )
     parser.add_argument('--url', required=True, help='URL to test for XSS vulnerability')
     args = parser.parse_args()
 
     # Download the chromedriver if it doesn't exist
     download_chromedriver()
 
     # Set up Chrome WebDriver
```

### Comparing `xssbase-1.0.6/xssbase/main.py` & `xssbase-1.0.7/xssbase/main.py`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.6/xssbase/utils.py` & `xssbase-1.0.7/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.6/xssbase.egg-info/PKG-INFO` & `xssbase-1.0.7/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.6
+Version: 1.0.7
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

