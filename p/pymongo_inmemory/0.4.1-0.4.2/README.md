# Comparing `tmp/pymongo_inmemory-0.4.1.tar.gz` & `tmp/pymongo_inmemory-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongo_inmemory-0.4.1.tar", max compression
+gzip compressed data, was "pymongo_inmemory-0.4.2.tar", max compression
```

## Comparing `pymongo_inmemory-0.4.1.tar` & `pymongo_inmemory-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1031 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/LICENSE
--rw-r--r--   0        0        0    13890 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/README.md
--rw-r--r--   0        0        0      155 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pymongo_inmemory/__init__.py
--rw-r--r--   0        0        0      868 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pymongo_inmemory/_pim.py
--rw-r--r--   0        0        0     1177 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pymongo_inmemory/_utils.py
--rw-r--r--   0        0        0     5595 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pymongo_inmemory/context.py
--rw-r--r--   0        0        0     4016 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pymongo_inmemory/downloader/__init__.py
--rw-r--r--   0        0        0      189 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pymongo_inmemory/downloader/__main__.py
--rw-r--r--   0        0        0    31171 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pymongo_inmemory/downloader/_patterns.py
--rw-r--r--   0        0        0     2760 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pymongo_inmemory/downloader/_urls.py
--rw-r--r--   0        0        0     7896 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pymongo_inmemory/mongod.py
--rw-r--r--   0        0        0     1457 2024-03-17 20:50:46.969063 pymongo_inmemory-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    15239 1970-01-01 00:00:00.000000 pymongo_inmemory-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1031 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/LICENSE
+-rw-r--r--   0        0        0    13890 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/README.md
+-rw-r--r--   0        0        0      155 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pymongo_inmemory/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pymongo_inmemory/_pim.py
+-rw-r--r--   0        0        0     1177 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pymongo_inmemory/_utils.py
+-rw-r--r--   0        0        0     5595 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pymongo_inmemory/context.py
+-rw-r--r--   0        0        0     4016 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pymongo_inmemory/downloader/__init__.py
+-rw-r--r--   0        0        0      189 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pymongo_inmemory/downloader/__main__.py
+-rw-r--r--   0        0        0    31171 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pymongo_inmemory/downloader/_patterns.py
+-rw-r--r--   0        0        0     2760 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pymongo_inmemory/downloader/_urls.py
+-rw-r--r--   0        0        0     7896 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pymongo_inmemory/mongod.py
+-rw-r--r--   0        0        0     1462 2024-05-26 08:03:50.348228 pymongo_inmemory-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    15239 1970-01-01 00:00:00.000000 pymongo_inmemory-0.4.2/PKG-INFO
```

### Comparing `pymongo_inmemory-0.4.1/LICENSE` & `pymongo_inmemory-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.4.1/README.md` & `pymongo_inmemory-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.4.1/pymongo_inmemory/_pim.py` & `pymongo_inmemory-0.4.2/pymongo_inmemory/_pim.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.4.1/pymongo_inmemory/_utils.py` & `pymongo_inmemory-0.4.2/pymongo_inmemory/_utils.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.4.1/pymongo_inmemory/context.py` & `pymongo_inmemory-0.4.2/pymongo_inmemory/context.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.4.1/pymongo_inmemory/downloader/__init__.py` & `pymongo_inmemory-0.4.2/pymongo_inmemory/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.4.1/pymongo_inmemory/downloader/_patterns.py` & `pymongo_inmemory-0.4.2/pymongo_inmemory/downloader/_patterns.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.4.1/pymongo_inmemory/downloader/_urls.py` & `pymongo_inmemory-0.4.2/pymongo_inmemory/downloader/_urls.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.4.1/pymongo_inmemory/mongod.py` & `pymongo_inmemory-0.4.2/pymongo_inmemory/mongod.py`

 * *Files identical despite different names*

### Comparing `pymongo_inmemory-0.4.1/pyproject.toml` & `pymongo_inmemory-0.4.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymongo_inmemory"
-version = "0.4.1"
+version = "0.4.2"
 description = "A mongo mocking library with an ephemeral MongoDB running in memory."
 authors = ["Kaizen Dorks <kaizendorks@gmail.com>"]
 maintainers = [
   "Ertugrul Karademir <ekarademir@gmail.com>",
   "Daniel Jimenez Garcia",
   "Ruben Vasconcelos",
 ]
@@ -37,15 +37,15 @@
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 mypy = "*"
 flake8 = "*"
 
 [tool.poetry.group.dev.dependencies]
 ruff-lsp = "^0.0.35"
-black = "^23.3.0"
+black = ">=23.3,<25.0"
 twine = "*"
 wheel = "*"
 setuptools = "*"
 click = "*"
 
 [build-system]
 requires = ["poetry-core>=0.12"]
```

### Comparing `pymongo_inmemory-0.4.1/PKG-INFO` & `pymongo_inmemory-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymongo_inmemory
-Version: 0.4.1
+Version: 0.4.2
 Summary: A mongo mocking library with an ephemeral MongoDB running in memory.
 Home-page: https://github.com/kaizendorks/pymongo_inmemory
 License: MIT
 Keywords: mongodb,testing,pymongo
 Author: Kaizen Dorks
 Author-email: kaizendorks@gmail.com
 Maintainer: Ertugrul Karademir
```

