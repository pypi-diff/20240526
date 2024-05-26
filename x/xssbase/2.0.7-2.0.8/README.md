# Comparing `tmp/xssbase-2.0.7.tar.gz` & `tmp/xssbase-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-2.0.7.tar", last modified: Sun May 26 10:55:02 2024, max compression
+gzip compressed data, was "xssbase-2.0.8.tar", last modified: Sun May 26 10:57:52 2024, max compression
```

## Comparing `xssbase-2.0.7.tar` & `xssbase-2.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 10:55:02.515337 xssbase-2.0.7/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.7/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-26 10:55:02.515337 xssbase-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 10:55:02.515337 xssbase-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-26 10:54:42.000000 xssbase-2.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:55:02.493204 xssbase-2.0.7/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.7/xssbase/__init__.py
--rw-rw-rw-   0        0        0     4310 2024-05-26 10:43:09.000000 xssbase-2.0.7/xssbase/cli.py
--rw-rw-rw-   0        0        0     1640 2024-05-26 10:54:38.000000 xssbase-2.0.7/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.7/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:55:02.515337 xssbase-2.0.7/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-26 10:55:02.000000 xssbase-2.0.7/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 10:55:02.000000 xssbase-2.0.7/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 10:55:02.000000 xssbase-2.0.7/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 10:55:02.000000 xssbase-2.0.7/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 10:55:02.000000 xssbase-2.0.7/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 10:55:02.000000 xssbase-2.0.7/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 10:57:52.565533 xssbase-2.0.8/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.8/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 10:57:52.565533 xssbase-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:57:52.565533 xssbase-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-26 10:57:34.000000 xssbase-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:57:52.534283 xssbase-2.0.8/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.8/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     4310 2024-05-26 10:43:09.000000 xssbase-2.0.8/xssbase/cli.py
+-rw-rw-rw-   0        0        0     1749 2024-05-26 10:57:30.000000 xssbase-2.0.8/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.8/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:57:52.565533 xssbase-2.0.8/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 10:57:52.000000 xssbase-2.0.8/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 10:57:52.000000 xssbase-2.0.8/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:57:52.000000 xssbase-2.0.8/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 10:57:52.000000 xssbase-2.0.8/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 10:57:52.000000 xssbase-2.0.8/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 10:57:52.000000 xssbase-2.0.8/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-2.0.7/LICENSE` & `xssbase-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.7/PKG-INFO` & `xssbase-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.7
+Version: 2.0.8
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-2.0.7/setup.py` & `xssbase-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='2.0.7',
+    version='2.0.8',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-2.0.7/xssbase/cli.py` & `xssbase-2.0.8/xssbase/cli.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.7/xssbase/main.py` & `xssbase-2.0.8/xssbase/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,13 +25,14 @@
             time.sleep(2)  # Allow time for potential alert boxes to appear
             current_url = driver.current_url
             if current_url != original_url:
                 print("Potential XSS vulnerability detected!")
                 print("Payload:", payload)
                 print("Current URL:", current_url)
                 print("Original URL:", original_url)
-                break
-        else:
-            print("No XSS vulnerability found. The site may be in good health. Try another site.")
+                return  # Exit the function once XSS vulnerability is found
+
+        # If no XSS vulnerability found after checking all input boxes
+        print("No XSS vulnerability found. The site may be in good health. Try another site.")
 
     except Exception as e:
         print("Error occurred:", str(e))
```

### Comparing `xssbase-2.0.7/xssbase/utils.py` & `xssbase-2.0.8/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.7/xssbase.egg-info/PKG-INFO` & `xssbase-2.0.8/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.7
+Version: 2.0.8
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

