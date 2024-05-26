# Comparing `tmp/ns_search_saved_export-0.1.1.tar.gz` & `tmp/ns_search_saved_export-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_search_saved_export-0.1.1.tar", last modified: Sun May 26 15:03:42 2024, max compression
+gzip compressed data, was "ns_search_saved_export-0.1.2.tar", last modified: Sun May 26 17:17:18 2024, max compression
```

## Comparing `ns_search_saved_export-0.1.1.tar` & `ns_search_saved_export-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:03:42.893693 ns_search_saved_export-0.1.1/
--rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1540 2024-05-26 15:03:42.884775 ns_search_saved_export-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      966 2024-05-26 14:56:20.000000 ns_search_saved_export-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 15:03:42.882589 ns_search_saved_export-0.1.1/Tests/
--rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.1/Tests/__init__.py
--rw-rw-rw-   0        0        0     2086 2024-05-26 14:02:17.000000 ns_search_saved_export-0.1.1/Tests/test_ns_search_saved_export.py
--rw-rw-rw-   0        0        0      945 2024-05-26 00:21:54.000000 ns_search_saved_export-0.1.1/Tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:03:42.883684 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/
--rw-rw-rw-   0        0        0     1540 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      476 2024-05-26 13:57:25.000000 ns_search_saved_export-0.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-26 15:03:42.879884 ns_search_saved_export-0.1.1/search_saved_export/
--rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.1/search_saved_export/__init__.py
--rw-rw-rw-   0        0        0     4268 2024-05-25 23:47:55.000000 ns_search_saved_export-0.1.1/search_saved_export/ns_search_saved_export.py
--rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.1/search_saved_export/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-26 15:03:42.894244 ns_search_saved_export-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      755 2024-05-26 15:00:39.000000 ns_search_saved_export-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:17:18.072489 ns_search_saved_export-0.1.2/
+-rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1563 2024-05-26 17:17:18.071375 ns_search_saved_export-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2024-05-26 17:14:05.000000 ns_search_saved_export-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 17:17:18.068055 ns_search_saved_export-0.1.2/Tests/
+-rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.2/Tests/__init__.py
+-rw-rw-rw-   0        0        0     2086 2024-05-26 16:50:56.000000 ns_search_saved_export-0.1.2/Tests/test_ns_search_saved_export.py
+-rw-rw-rw-   0        0        0      948 2024-05-26 16:45:44.000000 ns_search_saved_export-0.1.2/Tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:17:18.032903 ns_search_saved_export-0.1.2/ns_search_saved_export/
+-rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.2/ns_search_saved_export/__init__.py
+-rw-rw-rw-   0        0        0     4268 2024-05-25 23:47:55.000000 ns_search_saved_export-0.1.2/ns_search_saved_export/ns_search_saved_export.py
+-rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.2/ns_search_saved_export/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:17:18.069721 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/
+-rw-rw-rw-   0        0        0     1563 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      518 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      476 2024-05-26 13:57:25.000000 ns_search_saved_export-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 17:17:18.072557 ns_search_saved_export-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-05-26 17:11:02.000000 ns_search_saved_export-0.1.2/setup.py
```

### Comparing `ns_search_saved_export-0.1.1/PKG-INFO` & `ns_search_saved_export-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 ```python
 pip install ns_search_saved_export
 ```
 
 ## Usage
 
 ```python
-from ns_search_saved_export import NsSearchSavedExport
+from ns_search_saved_export.ns_search_saved_export import NsSearchSavedExport
 
 # Initialize the API
 api = NsSearchSavedExport(
     url='https://your-netsuite-url',
     consumer_key='your_consumer_key',
     consumer_secret='your_consumer_secret',
     token_key='your_token_key',
```

### Comparing `ns_search_saved_export-0.1.1/README.md` & `ns_search_saved_export-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```python
 pip install ns_search_saved_export
 ```
 
 ## Usage
 
 ```python
-from ns_search_saved_export import NsSearchSavedExport
+from ns_search_saved_export.ns_search_saved_export import NsSearchSavedExport
 
 # Initialize the API
 api = NsSearchSavedExport(
     url='https://your-netsuite-url',
     consumer_key='your_consumer_key',
     consumer_secret='your_consumer_secret',
     token_key='your_token_key',
```

### Comparing `ns_search_saved_export-0.1.1/Tests/test_ns_search_saved_export.py` & `ns_search_saved_export-0.1.2/Tests/test_ns_search_saved_export.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.1/Tests/test_utils.py` & `ns_search_saved_export-0.1.2/Tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import oauth2 as oauth
-from search_saved_export.utils import SignatureMethod_HMAC_SHA256
+from ns_search_saved_export.utils import SignatureMethod_HMAC_SHA256
 
 class TestSignatureMethod_HMAC_SHA256(unittest.TestCase):
     
     def setUp(self):
         self.consumer = oauth.Consumer(key='consumer_key', secret='consumer_secret')
         self.token = oauth.Token(key='token_key', secret='token_secret')
         self.signature_method = SignatureMethod_HMAC_SHA256()
```

### Comparing `ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/PKG-INFO` & `ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,15 @@
 ```python
 pip install ns_search_saved_export
 ```
 
 ## Usage
 
 ```python
-from ns_search_saved_export import NsSearchSavedExport
+from ns_search_saved_export.ns_search_saved_export import NsSearchSavedExport
 
 # Initialize the API
 api = NsSearchSavedExport(
     url='https://your-netsuite-url',
     consumer_key='your_consumer_key',
     consumer_secret='your_consumer_secret',
     token_key='your_token_key',
```

### Comparing `ns_search_saved_export-0.1.1/search_saved_export/ns_search_saved_export.py` & `ns_search_saved_export-0.1.2/ns_search_saved_export/ns_search_saved_export.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.1/search_saved_export/utils.py` & `ns_search_saved_export-0.1.2/ns_search_saved_export/utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.1/setup.py` & `ns_search_saved_export-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ns_search_saved_export',
-    version='0.1.1',
+    version='0.1.2',
     description='A library for interacting with NetSuite API and exporting data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Gildder',
     author_email='gildder@outlook.com',
     url='https://github.com/gildder/netsuite-search-saved-export',
     packages=find_packages(),
```

