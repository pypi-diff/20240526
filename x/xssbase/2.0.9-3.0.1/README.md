# Comparing `tmp/xssbase-2.0.9.tar.gz` & `tmp/xssbase-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-2.0.9.tar", last modified: Sun May 26 11:01:43 2024, max compression
+gzip compressed data, was "xssbase-3.0.1.tar", last modified: Sun May 26 11:04:48 2024, max compression
```

## Comparing `xssbase-2.0.9.tar` & `xssbase-3.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 11:01:43.897343 xssbase-2.0.9/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.9/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-26 11:01:43.897343 xssbase-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 11:01:43.897343 xssbase-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-26 11:01:28.000000 xssbase-2.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:01:43.875153 xssbase-2.0.9/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.9/xssbase/__init__.py
--rw-rw-rw-   0        0        0     4310 2024-05-26 10:43:09.000000 xssbase-2.0.9/xssbase/cli.py
--rw-rw-rw-   0        0        0     1945 2024-05-26 11:01:22.000000 xssbase-2.0.9/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.9/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:01:43.897343 xssbase-2.0.9/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-26 11:01:43.000000 xssbase-2.0.9/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 11:01:43.000000 xssbase-2.0.9/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 11:01:43.000000 xssbase-2.0.9/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 11:01:43.000000 xssbase-2.0.9/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 11:01:43.000000 xssbase-2.0.9/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 11:01:43.000000 xssbase-2.0.9/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 11:04:48.276069 xssbase-3.0.1/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 11:04:48.276069 xssbase-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-3.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 11:04:48.276069 xssbase-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-26 11:04:41.000000 xssbase-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:04:48.244826 xssbase-3.0.1/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-3.0.1/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     4310 2024-05-26 10:43:09.000000 xssbase-3.0.1/xssbase/cli.py
+-rw-rw-rw-   0        0        0     1538 2024-05-26 11:04:32.000000 xssbase-3.0.1/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-3.0.1/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:04:48.276069 xssbase-3.0.1/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 11:04:48.000000 xssbase-3.0.1/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 11:04:48.000000 xssbase-3.0.1/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 11:04:48.000000 xssbase-3.0.1/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 11:04:48.000000 xssbase-3.0.1/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 11:04:48.000000 xssbase-3.0.1/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 11:04:48.000000 xssbase-3.0.1/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-2.0.9/LICENSE` & `xssbase-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.9/PKG-INFO` & `xssbase-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.9
+Version: 3.0.1
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-2.0.9/setup.py` & `xssbase-3.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='2.0.9',
+    version='3.0.1',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-2.0.9/xssbase/cli.py` & `xssbase-3.0.1/xssbase/cli.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.9/xssbase/main.py` & `xssbase-3.0.1/xssbase/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
 from selenium import webdriver
 import time
-from selenium.common.exceptions import StaleElementReferenceException
 
-def test_xss_payloads(driver, url, payload):
-    vulnerability_found = False  # Flag to track if XSS vulnerability is found
+def test_xss_payloads(driver, url, payloads):
+    vulnerability_found = False
 
     try:
         driver.get(url)
         original_url = driver.current_url
 
-        # Find all input boxes and skip those with types 'number', 'email', and 'date'
-        input_boxes = driver.find_elements(By.XPATH, "//input[@type='text' or @type='password' or @type='search' or @type='tel' or @type='url' or @type='text' or @type='text' or @type='text' or @type='text']")
-        for input_box in input_boxes:
-            input_box_type = input_box.get_attribute('type')
-            if input_box_type in ['number', 'email', 'date']:
-                continue
-
-            # Fill the input box with XSS payload
-            input_box.clear()
-            input_box.send_keys(payload)
-            input_box.submit()
-
-            # Check if URL changes due to payload injection
-            time.sleep(2)  # Allow time for potential alert boxes to appear
-            current_url = driver.current_url
-            if current_url != original_url:
-                vulnerability_found = True  # Set flag to True if XSS vulnerability is found
-                print("Potential XSS vulnerability detected!")
-                print("Payload:", payload)
-                print("Current URL:", current_url)
-                print("Original URL:", original_url)
-                break  # Exit the loop once XSS vulnerability is found
+        for payload in payloads:
+            input_boxes = driver.find_elements(By.XPATH, "//input[@type='text' or @type='password' or @type='search' or @type='tel' or @type='url' or @type='text' or @type='text' or @type='text' or @type='text']")
+            for input_box in input_boxes:
+                input_box_type = input_box.get_attribute('type')
+                if input_box_type in ['number', 'email', 'date']:
+                    continue
+
+                input_box.clear()
+                input_box.send_keys(payload)
+                input_box.submit()
+
+                time.sleep(2)
+                current_url = driver.current_url
+                if current_url != original_url:
+                    vulnerability_found = True
+                    print("Potential XSS vulnerability detected!")
+                    print("Payload:", payload)
+                    print("Current URL:", current_url)
+                    print("Original URL:", original_url)
+                    break
+
+            if vulnerability_found:
+                break
 
-        # Check the flag and print message accordingly
         if not vulnerability_found:
             print("No XSS vulnerability found. The site may be in good health. Try another site.")
 
     except Exception as e:
         print("Error occurred:", str(e))
```

### Comparing `xssbase-2.0.9/xssbase/utils.py` & `xssbase-3.0.1/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.9/xssbase.egg-info/PKG-INFO` & `xssbase-3.0.1/xssbase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.9
+Version: 3.0.1
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

