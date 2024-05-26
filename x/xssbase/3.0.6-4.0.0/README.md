# Comparing `tmp/xssbase-3.0.6.tar.gz` & `tmp/xssbase-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-3.0.6.tar", last modified: Sun May 26 15:39:42 2024, max compression
+gzip compressed data, was "xssbase-4.0.0.tar", last modified: Sun May 26 15:42:07 2024, max compression
```

## Comparing `xssbase-3.0.6.tar` & `xssbase-4.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:39:42.693646 xssbase-3.0.6/
--rw-rw-rw-   0        0        0     1065 2024-05-26 12:22:40.000000 xssbase-3.0.6/LICENSE
--rw-rw-rw-   0        0        0     3223 2024-05-26 15:39:42.693646 xssbase-3.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2430 2024-05-26 15:37:45.000000 xssbase-3.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 15:39:42.709268 xssbase-3.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1081 2024-05-26 15:37:55.000000 xssbase-3.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:39:42.662405 xssbase-3.0.6/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 12:22:40.000000 xssbase-3.0.6/xssbase/__init__.py
--rw-rw-rw-   0        0        0     1801 2024-05-26 15:35:00.000000 xssbase-3.0.6/xssbase/cli.py
--rw-rw-rw-   0        0        0     5318 2024-05-26 15:31:08.000000 xssbase-3.0.6/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 12:22:40.000000 xssbase-3.0.6/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:39:42.693646 xssbase-3.0.6/xssbase.egg-info/
--rw-rw-rw-   0        0        0     3223 2024-05-26 15:39:42.000000 xssbase-3.0.6/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 15:39:42.000000 xssbase-3.0.6/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:39:42.000000 xssbase-3.0.6/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 15:39:42.000000 xssbase-3.0.6/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 15:39:42.000000 xssbase-3.0.6/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 15:39:42.000000 xssbase-3.0.6/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 15:42:07.406272 xssbase-4.0.0/
+-rw-rw-rw-   0        0        0     1065 2024-05-26 12:22:40.000000 xssbase-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3223 2024-05-26 15:42:07.406272 xssbase-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2430 2024-05-26 15:37:45.000000 xssbase-4.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:42:07.406272 xssbase-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2024-05-26 15:41:14.000000 xssbase-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:42:07.375029 xssbase-4.0.0/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 12:22:40.000000 xssbase-4.0.0/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     1804 2024-05-26 15:41:33.000000 xssbase-4.0.0/xssbase/cli.py
+-rw-rw-rw-   0        0        0     5318 2024-05-26 15:31:08.000000 xssbase-4.0.0/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 12:22:40.000000 xssbase-4.0.0/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:42:07.406272 xssbase-4.0.0/xssbase.egg-info/
+-rw-rw-rw-   0        0        0     3223 2024-05-26 15:42:07.000000 xssbase-4.0.0/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 15:42:07.000000 xssbase-4.0.0/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:42:07.000000 xssbase-4.0.0/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 15:42:07.000000 xssbase-4.0.0/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 15:42:07.000000 xssbase-4.0.0/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 15:42:07.000000 xssbase-4.0.0/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-3.0.6/LICENSE` & `xssbase-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-3.0.6/PKG-INFO` & `xssbase-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 3.0.6
+Version: 4.0.0
 Summary: XSSbase: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal,cyber security
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xssbase Version: 3.0.6 Summary: XSSbase: A
+Metadata-Version: 2.1 Name: xssbase Version: 4.0.0 Summary: XSSbase: A
 professional tool for scanning XSS vulnerabilities. Home-page: https://
 mrfidal.in/cyber-security/xssbase Author: Fidal Author-email: mrfidal@proton.me
 License: MIT Keywords: xssbase,xss,vulnerability,scanning,mrfidal,cyber
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `xssbase-3.0.6/README.md` & `xssbase-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `xssbase-3.0.6/setup.py` & `xssbase-4.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='3.0.6',
+    version='4.0.0',
     description='XSSbase: A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-3.0.6/xssbase/cli.py` & `xssbase-4.0.0/xssbase/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         sys.exit(1)
 
     # Define the argument parser
     parser = argparse.ArgumentParser(
         description="XSSbase - A professional tool for scanning XSS vulnerabilities.",
         epilog="Author: Fidal\nGitHub: https://github.com/mr-fidal\n\n"
                "Copyright 2024 Fidal. All rights reserved. \n"
-               "payload list : https://mrfidal.in/cyber-security/xssbase/payload-list.html"
+               "payload list : https://mrfidal.in/cyber-security/xssbase/payload-list.html \n"
                "Unauthorized copying of this tool, via any medium is strictly prohibited."
     )
     parser.add_argument('--url', required=True, help='URL to test for XSS vulnerability')
     parser.add_argument('--payload', help='File containing XSS payloads to use')
     args = parser.parse_args()
 
     # Download the chromedriver if it doesn't exist
```

### Comparing `xssbase-3.0.6/xssbase/main.py` & `xssbase-4.0.0/xssbase/main.py`

 * *Files identical despite different names*

### Comparing `xssbase-3.0.6/xssbase/utils.py` & `xssbase-4.0.0/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-3.0.6/xssbase.egg-info/PKG-INFO` & `xssbase-4.0.0/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 3.0.6
+Version: 4.0.0
 Summary: XSSbase: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal,cyber security
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xssbase Version: 3.0.6 Summary: XSSbase: A
+Metadata-Version: 2.1 Name: xssbase Version: 4.0.0 Summary: XSSbase: A
 professional tool for scanning XSS vulnerabilities. Home-page: https://
 mrfidal.in/cyber-security/xssbase Author: Fidal Author-email: mrfidal@proton.me
 License: MIT Keywords: xssbase,xss,vulnerability,scanning,mrfidal,cyber
 security Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

