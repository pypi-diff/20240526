# Comparing `tmp/ns_search_saved_export-0.1.0.tar.gz` & `tmp/ns_search_saved_export-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_search_saved_export-0.1.0.tar", last modified: Sun May 26 14:23:00 2024, max compression
+gzip compressed data, was "ns_search_saved_export-0.1.1.tar", last modified: Sun May 26 15:03:42 2024, max compression
```

## Comparing `ns_search_saved_export-0.1.0.tar` & `ns_search_saved_export-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:23:00.595914 ns_search_saved_export-0.1.0/
--rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      529 2024-05-26 14:23:00.594200 ns_search_saved_export-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-05-25 23:38:29.000000 ns_search_saved_export-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 14:23:00.589255 ns_search_saved_export-0.1.0/Tests/
--rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.0/Tests/__init__.py
--rw-rw-rw-   0        0        0     2086 2024-05-26 14:02:17.000000 ns_search_saved_export-0.1.0/Tests/test_ns_search_saved_export.py
--rw-rw-rw-   0        0        0      945 2024-05-26 00:21:54.000000 ns_search_saved_export-0.1.0/Tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:23:00.592203 ns_search_saved_export-0.1.0/ns_search_saved_export.egg-info/
--rw-rw-rw-   0        0        0      529 2024-05-26 14:22:59.000000 ns_search_saved_export-0.1.0/ns_search_saved_export.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      509 2024-05-26 14:22:59.000000 ns_search_saved_export-0.1.0/ns_search_saved_export.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:22:59.000000 ns_search_saved_export-0.1.0/ns_search_saved_export.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-26 14:22:59.000000 ns_search_saved_export-0.1.0/ns_search_saved_export.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-26 14:22:59.000000 ns_search_saved_export-0.1.0/ns_search_saved_export.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      476 2024-05-26 13:57:25.000000 ns_search_saved_export-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-26 14:23:00.586926 ns_search_saved_export-0.1.0/search_saved_export/
--rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.0/search_saved_export/__init__.py
--rw-rw-rw-   0        0        0     4268 2024-05-25 23:47:55.000000 ns_search_saved_export-0.1.0/search_saved_export/ns_search_saved_export.py
--rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.0/search_saved_export/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-26 14:23:00.596439 ns_search_saved_export-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      655 2024-05-26 00:30:32.000000 ns_search_saved_export-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:03:42.893693 ns_search_saved_export-0.1.1/
+-rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1540 2024-05-26 15:03:42.884775 ns_search_saved_export-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      966 2024-05-26 14:56:20.000000 ns_search_saved_export-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 15:03:42.882589 ns_search_saved_export-0.1.1/Tests/
+-rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.1/Tests/__init__.py
+-rw-rw-rw-   0        0        0     2086 2024-05-26 14:02:17.000000 ns_search_saved_export-0.1.1/Tests/test_ns_search_saved_export.py
+-rw-rw-rw-   0        0        0      945 2024-05-26 00:21:54.000000 ns_search_saved_export-0.1.1/Tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:03:42.883684 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/
+-rw-rw-rw-   0        0        0     1540 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-26 15:03:42.000000 ns_search_saved_export-0.1.1/ns_search_saved_export.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      476 2024-05-26 13:57:25.000000 ns_search_saved_export-0.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-26 15:03:42.879884 ns_search_saved_export-0.1.1/search_saved_export/
+-rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.1/search_saved_export/__init__.py
+-rw-rw-rw-   0        0        0     4268 2024-05-25 23:47:55.000000 ns_search_saved_export-0.1.1/search_saved_export/ns_search_saved_export.py
+-rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.1/search_saved_export/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:03:42.894244 ns_search_saved_export-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-05-26 15:00:39.000000 ns_search_saved_export-0.1.1/setup.py
```

### Comparing `ns_search_saved_export-0.1.0/Tests/test_ns_search_saved_export.py` & `ns_search_saved_export-0.1.1/Tests/test_ns_search_saved_export.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.0/Tests/test_utils.py` & `ns_search_saved_export-0.1.1/Tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.0/search_saved_export/ns_search_saved_export.py` & `ns_search_saved_export-0.1.1/search_saved_export/ns_search_saved_export.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.0/search_saved_export/utils.py` & `ns_search_saved_export-0.1.1/search_saved_export/utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.0/setup.py` & `ns_search_saved_export-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ns_search_saved_export',
-    version='0.1.0',
+    version='0.1.1',
     description='A library for interacting with NetSuite API and exporting data',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author='Gildder',
     author_email='gildder@outlook.com',
     url='https://github.com/gildder/netsuite-search-saved-export',
     packages=find_packages(),
     install_requires=[
         'oauth2',
         'requests',
```

