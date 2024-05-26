# Comparing `tmp/xssbase-2.0.1.tar.gz` & `tmp/xssbase-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-2.0.1.tar", last modified: Sun May 26 09:46:01 2024, max compression
+gzip compressed data, was "xssbase-2.0.2.tar", last modified: Sun May 26 09:51:55 2024, max compression
```

## Comparing `xssbase-2.0.1.tar` & `xssbase-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:01.521510 xssbase-2.0.1/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-26 09:46:01.521510 xssbase-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 09:46:01.521510 xssbase-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-26 09:45:45.000000 xssbase-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:01.505889 xssbase-2.0.1/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.1/xssbase/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-05-26 09:45:39.000000 xssbase-2.0.1/xssbase/cli.py
--rw-rw-rw-   0        0        0     2252 2024-05-26 09:45:27.000000 xssbase-2.0.1/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.1/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:46:01.521510 xssbase-2.0.1/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-26 09:46:01.000000 xssbase-2.0.1/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 09:46:01.000000 xssbase-2.0.1/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 09:46:01.000000 xssbase-2.0.1/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 09:46:01.000000 xssbase-2.0.1/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 09:46:01.000000 xssbase-2.0.1/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 09:46:01.000000 xssbase-2.0.1/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 09:51:55.194873 xssbase-2.0.2/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 09:51:55.194873 xssbase-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 09:51:55.194873 xssbase-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-26 09:51:38.000000 xssbase-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:51:55.179248 xssbase-2.0.2/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.2/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-05-26 09:45:39.000000 xssbase-2.0.2/xssbase/cli.py
+-rw-rw-rw-   0        0        0     2428 2024-05-26 09:50:39.000000 xssbase-2.0.2/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.2/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:51:55.194873 xssbase-2.0.2/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 09:51:55.000000 xssbase-2.0.2/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 09:51:55.000000 xssbase-2.0.2/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 09:51:55.000000 xssbase-2.0.2/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 09:51:55.000000 xssbase-2.0.2/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 09:51:55.000000 xssbase-2.0.2/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 09:51:55.000000 xssbase-2.0.2/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-2.0.1/LICENSE` & `xssbase-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.1/PKG-INFO` & `xssbase-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.1
+Version: 2.0.2
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-2.0.1/setup.py` & `xssbase-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='2.0.1',
+    version='2.0.2',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-2.0.1/xssbase/cli.py` & `xssbase-2.0.2/xssbase/cli.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.1/xssbase/main.py` & `xssbase-2.0.2/xssbase/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,22 +40,25 @@
             else:
                 print("Failed after several attempts due to stale element reference.")
 
 def test_xss_payloads(driver, url):
     try:
         driver.get(url)
         original_url = driver.current_url
+        xss_found = False  # Flag to track if XSS vulnerability is found
 
         for payload in xss_payloads:
             find_and_fill_inputs(driver, payload)
             
             # Check if URL changes due to payload injection
             current_url = driver.current_url
-            print(f"Payload: {payload}")
-            print(f"Current URL: {current_url}")
             if current_url != original_url:
                 print("Potential XSS vulnerability detected!")
                 print("Original URL:", original_url)
-            print()
+                print("Current URL:", current_url)
+                xss_found = True
+
+        if not xss_found:
+            print("No XSS vulnerability found. The site may be in good health. Try another site.")
 
     except Exception as e:
         print("Error occurred:", str(e))
```

#### html2text {}

```diff
@@ -11,14 +11,15 @@
 (Keys.ENTER) time.sleep(1) # Allow time for potential alert boxes to appear
 except Exception as e: print(f"Could not fill input box: {e}") # Retry
 mechanism for handling stale element reference attempts = 3 for attempt in
 range(attempts): try: fill_inputs() break except
 StaleElementReferenceException: if attempt < attempts - 1: print("Stale element
 reference, retrying...") time.sleep(1) else: print("Failed after several
 attempts due to stale element reference.") def test_xss_payloads(driver, url):
-try: driver.get(url) original_url = driver.current_url for payload in
-xss_payloads: find_and_fill_inputs(driver, payload) # Check if URL changes due
-to payload injection current_url = driver.current_url print(f"Payload:
-{payload}") print(f"Current URL: {current_url}") if current_url !=
-original_url: print("Potential XSS vulnerability detected!") print("Original
-URL:", original_url) print() except Exception as e: print("Error occurred:",
-str(e))
+try: driver.get(url) original_url = driver.current_url xss_found = False # Flag
+to track if XSS vulnerability is found for payload in xss_payloads:
+find_and_fill_inputs(driver, payload) # Check if URL changes due to payload
+injection current_url = driver.current_url if current_url != original_url:
+print("Potential XSS vulnerability detected!") print("Original URL:",
+original_url) print("Current URL:", current_url) xss_found = True if not
+xss_found: print("No XSS vulnerability found. The site may be in good health.
+Try another site.") except Exception as e: print("Error occurred:", str(e))
```

### Comparing `xssbase-2.0.1/xssbase/utils.py` & `xssbase-2.0.2/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.1/xssbase.egg-info/PKG-INFO` & `xssbase-2.0.2/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.1
+Version: 2.0.2
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

