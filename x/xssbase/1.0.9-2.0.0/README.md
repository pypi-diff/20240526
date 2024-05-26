# Comparing `tmp/xssbase-1.0.9.tar.gz` & `tmp/xssbase-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-1.0.9.tar", last modified: Sun May 26 09:36:59 2024, max compression
+gzip compressed data, was "xssbase-2.0.0.tar", last modified: Sun May 26 09:40:54 2024, max compression
```

## Comparing `xssbase-1.0.9.tar` & `xssbase-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 09:36:59.818855 xssbase-1.0.9/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-1.0.9/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-26 09:36:59.818855 xssbase-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 09:36:59.818855 xssbase-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-26 09:36:30.000000 xssbase-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:36:59.781127 xssbase-1.0.9/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-1.0.9/xssbase/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-05-26 09:36:23.000000 xssbase-1.0.9/xssbase/cli.py
--rw-rw-rw-   0        0        0     2214 2024-05-26 09:36:12.000000 xssbase-1.0.9/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-1.0.9/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:36:59.818855 xssbase-1.0.9/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-26 09:36:59.000000 xssbase-1.0.9/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 09:36:59.000000 xssbase-1.0.9/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 09:36:59.000000 xssbase-1.0.9/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 09:36:59.000000 xssbase-1.0.9/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 09:36:59.000000 xssbase-1.0.9/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 09:36:59.000000 xssbase-1.0.9/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 09:40:54.703764 xssbase-2.0.0/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 09:40:54.703764 xssbase-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 09:40:54.703764 xssbase-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-26 09:40:29.000000 xssbase-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:40:54.672468 xssbase-2.0.0/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.0/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-05-26 09:40:21.000000 xssbase-2.0.0/xssbase/cli.py
+-rw-rw-rw-   0        0        0     2231 2024-05-26 09:40:07.000000 xssbase-2.0.0/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.0/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:40:54.703764 xssbase-2.0.0/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 09:40:54.000000 xssbase-2.0.0/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 09:40:54.000000 xssbase-2.0.0/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 09:40:54.000000 xssbase-2.0.0/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 09:40:54.000000 xssbase-2.0.0/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 09:40:54.000000 xssbase-2.0.0/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 09:40:54.000000 xssbase-2.0.0/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-1.0.9/LICENSE` & `xssbase-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.9/PKG-INFO` & `xssbase-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.9
+Version: 2.0.0
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-1.0.9/setup.py` & `xssbase-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='1.0.9',
+    version='2.0.0',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-1.0.9/xssbase/cli.py` & `xssbase-2.0.0/xssbase/cli.py`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.9/xssbase/main.py` & `xssbase-2.0.0/xssbase/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         original_url = driver.current_url
 
         for payload in xss_payloads:
             find_and_fill_inputs(driver, payload)
             
             # Check if URL changes due to payload injection
             current_url = driver.current_url
+            print(f"Payload: {payload}")
+            print(f"Current URL: {current_url}")
             if current_url != original_url:
                 print("Potential XSS vulnerability detected!")
                 print("Original URL:", original_url)
-                print("Current URL:", current_url)
-                break
 
     except Exception as e:
         print("Error occurred:", str(e))
```

#### html2text {}

```diff
@@ -13,11 +13,11 @@
 mechanism for handling stale element reference attempts = 3 for attempt in
 range(attempts): try: fill_inputs() break except
 StaleElementReferenceException: if attempt < attempts - 1: print("Stale element
 reference, retrying...") time.sleep(1) else: print("Failed after several
 attempts due to stale element reference.") def test_xss_payloads(driver, url):
 try: driver.get(url) original_url = driver.current_url for payload in
 xss_payloads: find_and_fill_inputs(driver, payload) # Check if URL changes due
-to payload injection current_url = driver.current_url if current_url !=
+to payload injection current_url = driver.current_url print(f"Payload:
+{payload}") print(f"Current URL: {current_url}") if current_url !=
 original_url: print("Potential XSS vulnerability detected!") print("Original
-URL:", original_url) print("Current URL:", current_url) break except Exception
-as e: print("Error occurred:", str(e))
+URL:", original_url) except Exception as e: print("Error occurred:", str(e))
```

### Comparing `xssbase-1.0.9/xssbase/utils.py` & `xssbase-2.0.0/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-1.0.9/xssbase.egg-info/PKG-INFO` & `xssbase-2.0.0/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 1.0.9
+Version: 2.0.0
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

