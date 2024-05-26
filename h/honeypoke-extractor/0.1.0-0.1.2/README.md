# Comparing `tmp/honeypoke_extractor-0.1.0.tar.gz` & `tmp/honeypoke_extractor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honeypoke_extractor-0.1.0.tar", last modified: Sat Jan  6 19:55:15 2024, max compression
+gzip compressed data, was "honeypoke_extractor-0.1.2.tar", last modified: Sun May 26 00:26:04 2024, max compression
```

## Comparing `honeypoke_extractor-0.1.0.tar` & `honeypoke_extractor-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-01-06 19:55:15.856142 honeypoke_extractor-0.1.0/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1069 2024-01-05 03:45:17.000000 honeypoke_extractor-0.1.0/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2496 2024-01-06 19:55:15.856142 honeypoke_extractor-0.1.0/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      163 2023-12-30 06:22:45.000000 honeypoke_extractor-0.1.0/README.md
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-01-06 19:55:15.852808 honeypoke_extractor-0.1.0/honeypoke_extractor/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5367 2024-01-06 19:52:28.000000 honeypoke_extractor-0.1.0/honeypoke_extractor/__init__.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-01-06 19:55:15.856142 honeypoke_extractor-0.1.0/honeypoke_extractor/detect/
--rw-r--r--   0 jacob     (1000) jacob     (1000)      383 2023-12-30 05:30:33.000000 honeypoke_extractor-0.1.0/honeypoke_extractor/detect/portpattern.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-01-06 19:55:15.852808 honeypoke_extractor-0.1.0/honeypoke_extractor/enrichment/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-01-06 19:55:15.856142 honeypoke_extractor-0.1.0/honeypoke_extractor/enrichment/address/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4320 2023-12-30 17:05:31.000000 honeypoke_extractor-0.1.0/honeypoke_extractor/enrichment/address/__init__.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-01-06 19:55:15.856142 honeypoke_extractor-0.1.0/honeypoke_extractor.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2496 2024-01-06 19:55:15.000000 honeypoke_extractor-0.1.0/honeypoke_extractor.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      371 2024-01-06 19:55:15.000000 honeypoke_extractor-0.1.0/honeypoke_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2024-01-06 19:55:15.000000 honeypoke_extractor-0.1.0/honeypoke_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       85 2024-01-06 19:55:15.000000 honeypoke_extractor-0.1.0/honeypoke_extractor.egg-info/requires.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       20 2024-01-06 19:55:15.000000 honeypoke_extractor-0.1.0/honeypoke_extractor.egg-info/top_level.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1340 2024-01-06 19:49:15.000000 honeypoke_extractor-0.1.0/pyproject.toml
--rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2024-01-06 19:55:15.856142 honeypoke_extractor-0.1.0/setup.cfg
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-26 00:26:04.827697 honeypoke_extractor-0.1.2/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1069 2024-01-05 03:45:17.000000 honeypoke_extractor-0.1.2/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2496 2024-05-26 00:26:04.827697 honeypoke_extractor-0.1.2/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      163 2023-12-30 06:22:45.000000 honeypoke_extractor-0.1.2/README.md
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-26 00:26:04.824363 honeypoke_extractor-0.1.2/honeypoke_extractor/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6210 2024-05-16 02:11:46.000000 honeypoke_extractor-0.1.2/honeypoke_extractor/__init__.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-26 00:26:04.824363 honeypoke_extractor-0.1.2/honeypoke_extractor/detect/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      383 2023-12-30 05:30:33.000000 honeypoke_extractor-0.1.2/honeypoke_extractor/detect/portpattern.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-26 00:26:04.824363 honeypoke_extractor-0.1.2/honeypoke_extractor/enrichment/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-26 00:26:04.824363 honeypoke_extractor-0.1.2/honeypoke_extractor/enrichment/address/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4320 2023-12-30 17:05:31.000000 honeypoke_extractor-0.1.2/honeypoke_extractor/enrichment/address/__init__.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-26 00:26:04.824363 honeypoke_extractor-0.1.2/honeypoke_extractor.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2496 2024-05-26 00:26:04.000000 honeypoke_extractor-0.1.2/honeypoke_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      371 2024-05-26 00:26:04.000000 honeypoke_extractor-0.1.2/honeypoke_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2024-05-26 00:26:04.000000 honeypoke_extractor-0.1.2/honeypoke_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       85 2024-05-26 00:26:04.000000 honeypoke_extractor-0.1.2/honeypoke_extractor.egg-info/requires.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       20 2024-05-26 00:26:04.000000 honeypoke_extractor-0.1.2/honeypoke_extractor.egg-info/top_level.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1394 2024-05-22 02:21:40.000000 honeypoke_extractor-0.1.2/pyproject.toml
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2024-05-26 00:26:04.827697 honeypoke_extractor-0.1.2/setup.cfg
```

### Comparing `honeypoke_extractor-0.1.0/LICENSE` & `honeypoke_extractor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `honeypoke_extractor-0.1.0/PKG-INFO` & `honeypoke_extractor-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeypoke_extractor
-Version: 0.1.0
+Version: 0.1.2
 Summary: Script to extract interesting information from HoneyPoke data
 Author-email: Jacob Hartman <jacob@j2h2.com>
 Maintainer-email: Jacob Hartman <jacob@j2h2.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Hartman
```

### Comparing `honeypoke_extractor-0.1.0/honeypoke_extractor/__init__.py` & `honeypoke_extractor-0.1.2/honeypoke_extractor/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -181,7 +181,36 @@
 
         for item in results['hits']['hits']:
             return_item = item['_source']
             return_item['_id'] = item['_id']
             return_list.append(return_item)
 
         return return_list
+
+    def get_hits(self, count=100, skip=0, time_start=None, time_end=None):
+        time_start, time_end = self._get_times(time_start, time_end)
+
+        results = self._client.search(index=self._index, query={"bool": {
+        "filter": [
+            {
+                "range": {
+                    "time": {
+                        "format": "strict_date_optional_time",
+                        "gte": time_start,
+                        "lte": time_end
+                    }
+                }
+            }
+        ],
+        "should": [],
+        "must_not": []
+        }}
+        , size=count, from_=skip)
+
+        return_list = []
+
+        for item in results['hits']['hits']:
+            return_item = item['_source']
+            return_item['_id'] = item['_id']
+            return_list.append(return_item)
+
+        return return_list
```

### Comparing `honeypoke_extractor-0.1.0/honeypoke_extractor/enrichment/address/__init__.py` & `honeypoke_extractor-0.1.2/honeypoke_extractor/enrichment/address/__init__.py`

 * *Files identical despite different names*

### Comparing `honeypoke_extractor-0.1.0/honeypoke_extractor.egg-info/PKG-INFO` & `honeypoke_extractor-0.1.2/honeypoke_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeypoke_extractor
-Version: 0.1.0
+Version: 0.1.2
 Summary: Script to extract interesting information from HoneyPoke data
 Author-email: Jacob Hartman <jacob@j2h2.com>
 Maintainer-email: Jacob Hartman <jacob@j2h2.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Hartman
```

### Comparing `honeypoke_extractor-0.1.0/pyproject.toml` & `honeypoke_extractor-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "honeypoke_extractor"
-version = "0.1.0"
+version = "0.1.2"
 description = "Script to extract interesting information from HoneyPoke data"
 dependencies = [
     "requests==2.31.0",
     "elasticsearch==8.11.1",
     'importlib-metadata; python_version<"3.8"',
 ]
 authors = [
@@ -38,8 +38,11 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.urls]
 Homepage = "https://github.com/bocajspear1/honeypoke-extractor"
 Repository = "https://github.com/bocajspear1/honeypoke-extractor"
-Issues = "https://github.com/bocajspear1/honeypoke-extractor/issues"
+Issues = "https://github.com/bocajspear1/honeypoke-extractor/issues"
+
+[tool.setuptools]
+packages = ["honeypoke_extractor"]
```

