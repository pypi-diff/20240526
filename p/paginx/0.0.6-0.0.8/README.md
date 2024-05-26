# Comparing `tmp/paginx-0.0.6.tar.gz` & `tmp/paginx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paginx-0.0.6.tar", max compression
+gzip compressed data, was "paginx-0.0.8.tar", max compression
```

## Comparing `paginx-0.0.6.tar` & `paginx-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1071 2024-04-23 12:21:11.278196 paginx-0.0.6/LICENSE
--rw-r--r--   0        0        0      479 2024-05-01 15:05:05.400525 paginx-0.0.6/README.md
--rw-r--r--   0        0        0      878 2024-05-26 10:59:48.029261 paginx-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      123 2024-05-25 21:44:51.867130 paginx-0.0.6/src/paginx/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 20:40:54.836761 paginx-0.0.6/src/paginx/llm/__init__.py
--rw-r--r--   0        0        0      901 2024-05-25 21:14:36.791250 paginx-0.0.6/src/paginx/llm/llm.py
--rw-r--r--   0        0        0      398 2024-05-25 20:56:20.097163 paginx-0.0.6/src/paginx/main.py
--rw-r--r--   0        0        0        0 2024-05-25 15:30:49.865803 paginx-0.0.6/src/paginx/ner/__init__.py
--rw-r--r--   0        0        0     4398 2024-05-25 21:13:10.581073 paginx-0.0.6/src/paginx/ner/extract.py
--rw-r--r--   0        0        0      703 2024-05-25 15:28:41.198860 paginx-0.0.6/src/paginx/ner/models/entities.py
--rw-r--r--   0        0        0        0 2024-05-04 15:24:34.935828 paginx-0.0.6/src/paginx/page_crawler/__init__.py
--rw-r--r--   0        0        0     5951 2024-05-23 07:35:57.974824 paginx-0.0.6/src/paginx/page_crawler/crawler.py
--rw-r--r--   0        0        0      619 2024-05-04 18:29:15.959142 paginx-0.0.6/src/paginx/page_crawler/models/site_pages.py
--rw-r--r--   0        0        0     2045 2024-05-04 19:03:43.941499 paginx-0.0.6/src/paginx/page_crawler/web_chunker.py
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 paginx-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-26 11:17:42.704732 paginx-0.0.8/LICENSE
+-rw-r--r--   0        0        0      479 2024-05-26 11:17:42.704732 paginx-0.0.8/README.md
+-rw-r--r--   0        0        0      878 2024-05-26 11:17:42.712732 paginx-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      123 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/llm/__init__.py
+-rw-r--r--   0        0        0      901 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/llm/llm.py
+-rw-r--r--   0        0        0      398 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/main.py
+-rw-r--r--   0        0        0        0 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/ner/__init__.py
+-rw-r--r--   0        0        0     4398 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/ner/extract.py
+-rw-r--r--   0        0        0      703 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/ner/models/entities.py
+-rw-r--r--   0        0        0        0 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/page_crawler/__init__.py
+-rw-r--r--   0        0        0     5951 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/page_crawler/crawler.py
+-rw-r--r--   0        0        0      619 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/page_crawler/models/site_pages.py
+-rw-r--r--   0        0        0     2045 2024-05-26 11:17:42.712732 paginx-0.0.8/src/paginx/page_crawler/web_chunker.py
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 paginx-0.0.8/PKG-INFO
```

### Comparing `paginx-0.0.6/LICENSE` & `paginx-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `paginx-0.0.6/pyproject.toml` & `paginx-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paginx"
-version = "0.0.6"
+version = "0.0.8"
 description = "An assistant helping you to index webpages into structured datasets."
 authors = ["Ben Selleslagh <ben@dataframe.be>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "paginx", from = "src"},
 ]
```

### Comparing `paginx-0.0.6/src/paginx/llm/llm.py` & `paginx-0.0.8/src/paginx/llm/llm.py`

 * *Files identical despite different names*

### Comparing `paginx-0.0.6/src/paginx/ner/extract.py` & `paginx-0.0.8/src/paginx/ner/extract.py`

 * *Files identical despite different names*

### Comparing `paginx-0.0.6/src/paginx/ner/models/entities.py` & `paginx-0.0.8/src/paginx/ner/models/entities.py`

 * *Files identical despite different names*

### Comparing `paginx-0.0.6/src/paginx/page_crawler/crawler.py` & `paginx-0.0.8/src/paginx/page_crawler/crawler.py`

 * *Files identical despite different names*

### Comparing `paginx-0.0.6/src/paginx/page_crawler/models/site_pages.py` & `paginx-0.0.8/src/paginx/page_crawler/models/site_pages.py`

 * *Files identical despite different names*

### Comparing `paginx-0.0.6/src/paginx/page_crawler/web_chunker.py` & `paginx-0.0.8/src/paginx/page_crawler/web_chunker.py`

 * *Files identical despite different names*

### Comparing `paginx-0.0.6/PKG-INFO` & `paginx-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paginx
-Version: 0.0.6
+Version: 0.0.8
 Summary: An assistant helping you to index webpages into structured datasets.
 License: MIT
 Author: Ben Selleslagh
 Author-email: ben@dataframe.be
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

