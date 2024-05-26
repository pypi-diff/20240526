# Comparing `tmp/ns_search_saved_export-0.1.2.tar.gz` & `tmp/ns_search_saved_export-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_search_saved_export-0.1.2.tar", last modified: Sun May 26 17:17:18 2024, max compression
+gzip compressed data, was "ns_search_saved_export-0.1.3.tar", last modified: Sun May 26 18:02:50 2024, max compression
```

## Comparing `ns_search_saved_export-0.1.2.tar` & `ns_search_saved_export-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 17:17:18.072489 ns_search_saved_export-0.1.2/
--rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1563 2024-05-26 17:17:18.071375 ns_search_saved_export-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      989 2024-05-26 17:14:05.000000 ns_search_saved_export-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 17:17:18.068055 ns_search_saved_export-0.1.2/Tests/
--rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.2/Tests/__init__.py
--rw-rw-rw-   0        0        0     2086 2024-05-26 16:50:56.000000 ns_search_saved_export-0.1.2/Tests/test_ns_search_saved_export.py
--rw-rw-rw-   0        0        0      948 2024-05-26 16:45:44.000000 ns_search_saved_export-0.1.2/Tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:17:18.032903 ns_search_saved_export-0.1.2/ns_search_saved_export/
--rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.2/ns_search_saved_export/__init__.py
--rw-rw-rw-   0        0        0     4268 2024-05-25 23:47:55.000000 ns_search_saved_export-0.1.2/ns_search_saved_export/ns_search_saved_export.py
--rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.2/ns_search_saved_export/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:17:18.069721 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/
--rw-rw-rw-   0        0        0     1563 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-26 17:17:17.000000 ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      476 2024-05-26 13:57:25.000000 ns_search_saved_export-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-26 17:17:18.072557 ns_search_saved_export-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      755 2024-05-26 17:11:02.000000 ns_search_saved_export-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:02:50.783170 ns_search_saved_export-0.1.3/
+-rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1563 2024-05-26 18:02:50.781449 ns_search_saved_export-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2024-05-26 17:14:05.000000 ns_search_saved_export-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 18:02:50.778414 ns_search_saved_export-0.1.3/Tests/
+-rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.3/Tests/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-05-26 17:33:39.000000 ns_search_saved_export-0.1.3/Tests/test_main.py
+-rw-rw-rw-   0        0        0     2660 2024-05-26 17:29:33.000000 ns_search_saved_export-0.1.3/Tests/test_ns_search_saved_export.py
+-rw-rw-rw-   0        0        0      948 2024-05-26 16:45:44.000000 ns_search_saved_export-0.1.3/Tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:02:50.734249 ns_search_saved_export-0.1.3/ns_search_saved_export/
+-rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.3/ns_search_saved_export/__init__.py
+-rw-rw-rw-   0        0        0     4268 2024-05-25 23:47:55.000000 ns_search_saved_export-0.1.3/ns_search_saved_export/ns_search_saved_export.py
+-rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.3/ns_search_saved_export/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:02:50.780125 ns_search_saved_export-0.1.3/ns_search_saved_export.egg-info/
+-rw-rw-rw-   0        0        0     1563 2024-05-26 18:02:50.000000 ns_search_saved_export-0.1.3/ns_search_saved_export.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2024-05-26 18:02:50.000000 ns_search_saved_export-0.1.3/ns_search_saved_export.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:02:50.000000 ns_search_saved_export-0.1.3/ns_search_saved_export.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-26 18:02:50.000000 ns_search_saved_export-0.1.3/ns_search_saved_export.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-26 18:02:50.000000 ns_search_saved_export-0.1.3/ns_search_saved_export.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      497 2024-05-26 18:01:07.000000 ns_search_saved_export-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 18:02:50.783170 ns_search_saved_export-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-05-26 18:01:32.000000 ns_search_saved_export-0.1.3/setup.py
```

### Comparing `ns_search_saved_export-0.1.2/PKG-INFO` & `ns_search_saved_export-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ns_search_saved_export-0.1.2/README.md` & `ns_search_saved_export-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.2/Tests/test_utils.py` & `ns_search_saved_export-0.1.3/Tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.2/ns_search_saved_export/ns_search_saved_export.py` & `ns_search_saved_export-0.1.3/ns_search_saved_export/ns_search_saved_export.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.2/ns_search_saved_export/utils.py` & `ns_search_saved_export-0.1.3/ns_search_saved_export/utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/PKG-INFO` & `ns_search_saved_export-0.1.3/ns_search_saved_export.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ns_search_saved_export-0.1.2/ns_search_saved_export.egg-info/SOURCES.txt` & `ns_search_saved_export-0.1.3/ns_search_saved_export.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 Tests/__init__.py
+Tests/test_main.py
 Tests/test_ns_search_saved_export.py
 Tests/test_utils.py
 ns_search_saved_export/__init__.py
 ns_search_saved_export/ns_search_saved_export.py
 ns_search_saved_export/utils.py
 ns_search_saved_export.egg-info/PKG-INFO
 ns_search_saved_export.egg-info/SOURCES.txt
 ns_search_saved_export.egg-info/dependency_links.txt
 ns_search_saved_export.egg-info/requires.txt
 ns_search_saved_export.egg-info/top_level.txt
+tests/test_main.py
 tests/test_ns_search_saved_export.py
 tests/test_utils.py
```

### Comparing `ns_search_saved_export-0.1.2/setup.py` & `ns_search_saved_export-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ns_search_saved_export',
-    version='0.1.2',
+    version='0.1.3',
     description='A library for interacting with NetSuite API and exporting data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Gildder',
     author_email='gildder@outlook.com',
     url='https://github.com/gildder/netsuite-search-saved-export',
     packages=find_packages(),
```

