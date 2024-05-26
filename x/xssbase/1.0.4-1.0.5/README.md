# Comparing `tmp/xssbase-1.0.4.tar.gz` & `tmp/xssbase-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-1.0.4.tar", last modified: Sun May 26 07:19:58 2024, max compression
+gzip compressed data, was "xssbase-1.0.5.tar", last modified: Sun May 26 08:07:35 2024, max compression
```

## Comparing `xssbase-1.0.4.tar` & `xssbase-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 07:19:58.213657 xssbase-1.0.4/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-26 07:19:58.212680 xssbase-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 07:19:58.214644 xssbase-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-26 07:18:29.000000 xssbase-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 07:19:58.182428 xssbase-1.0.4/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-1.0.4/xssbase/__init__.py
--rw-rw-rw-   0        0        0     1061 2024-05-26 07:18:19.000000 xssbase-1.0.4/xssbase/cli.py
--rw-rw-rw-   0        0        0     2288 2024-05-26 06:45:27.000000 xssbase-1.0.4/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 06:46:00.000000 xssbase-1.0.4/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 07:19:58.210742 xssbase-1.0.4/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 07:19:58.000000 xssbase-1.0.4/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 07:19:57.000000 xssbase-1.0.4/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 08:07:35.514533 xssbase-1.0.5/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 08:07:35.513559 xssbase-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 08:07:35.515512 xssbase-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-26 08:04:53.000000 xssbase-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:07:35.486221 xssbase-1.0.5/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-1.0.5/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     1306 2024-05-26 08:05:45.000000 xssbase-1.0.5/xssbase/cli.py
+-rw-rw-rw-   0        0        0     1115 2024-05-26 08:05:04.000000 xssbase-1.0.5/xssbase/main.py
+-rw-rw-rw-   0        0        0     1877 2024-05-26 08:05:32.000000 xssbase-1.0.5/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:07:35.511604 xssbase-1.0.5/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 08:07:35.000000 xssbase-1.0.5/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 08:07:35.000000 xssbase-1.0.5/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 08:07:35.000000 xssbase-1.0.5/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 08:07:35.000000 xssbase-1.0.5/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 08:07:35.000000 xssbase-1.0.5/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 08:07:35.000000 xssbase-1.0.5/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-1.0.4/LICENSE` & `xssbase-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.4/PKG-INFO` & `xssbase-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.4
+Version: 1.0.5
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-1.0.4/setup.py` & `xssbase-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='1.0.4',
+    version='1.0.5',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-1.0.4/xssbase/cli.py` & `xssbase-1.0.5/xssbase/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,42 @@
+# xssbase - A professional tool for scanning XSS vulnerabilities
+# Author: Fidal
+# Date: 2024
+# License: MIT
+
 import argparse
-import os
 import sys
 import platform
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from .main import test_xss_payloads
-from .utils import download_chromedriver
+from .utils import download_chromedriver_windows, download_chromedriver_linux, download_chromedriver_mac
 
 def main():
-    # Check if the operating system is Windows
-    if platform.system() != 'Windows':
-        print("This tool only supports Windows.")
-        sys.exit(1)
-
     parser = argparse.ArgumentParser(description="XSS testing tool")
     parser.add_argument('--url', required=True, help='URL to test for XSS vulnerability')
     args = parser.parse_args()
 
-    # Download the chromedriver if it doesn't exist
-    download_chromedriver()
+    system = platform.system()
+
+    if system == 'Windows':
+        download_chromedriver_windows()
+        service = Service('chromedriver-win64/chromedriver.exe')
+    elif system == 'Linux':
+        download_chromedriver_linux()
+        service = Service('chromedriver-linux64/chromedriver')
+    elif system == 'Darwin':
+        download_chromedriver_mac()
+        service = Service('chromedriver-mac64/chromedriver')
+    else:
+        print(f"This tool does not support {system}.")
+        sys.exit(1)
 
-    # Set up Chrome WebDriver
-    service = Service('chromedriver-win64/chromedriver.exe')  # Specify the path to chromedriver executable
     driver = webdriver.Chrome(service=service)
 
     try:
-        # Test XSS payloads
         test_xss_payloads(driver, args.url)
     finally:
-        # Close the browser
         driver.quit()
 
 if __name__ == "__main__":
     main()
```

### Comparing `xssbase-1.0.4/xssbase.egg-info/PKG-INFO` & `xssbase-1.0.5/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.4
+Version: 1.0.5
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

