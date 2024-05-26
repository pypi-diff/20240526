# Comparing `tmp/pylonparser-0.1.2.tar.gz` & `tmp/pylonparser-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylonparser-0.1.2.tar", max compression
+gzip compressed data, was "pylonparser-0.1.3.tar", max compression
```

## Comparing `pylonparser-0.1.2.tar` & `pylonparser-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-05-23 19:03:26.231140 pylonparser-0.1.2/LICENSE
--rw-r--r--   0        0        0     1834 2024-05-23 18:45:59.171621 pylonparser-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-23 17:01:37.948193 pylonparser-0.1.2/pylonparser/__init__.py
--rw-r--r--   0        0        0     3307 2024-05-23 19:03:26.241140 pylonparser-0.1.2/pylonparser/parser.py
--rw-r--r--   0        0        0      740 2024-05-23 19:17:14.500833 pylonparser-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2705 1970-01-01 00:00:00.000000 pylonparser-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-23 19:03:26.231140 pylonparser-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1834 2024-05-23 18:45:59.171621 pylonparser-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 17:01:37.948193 pylonparser-0.1.3/pylonparser/__init__.py
+-rw-r--r--   0        0        0     1666 2024-05-26 18:02:35.771810 pylonparser-0.1.3/pylonparser/matches.py
+-rw-r--r--   0        0        0     5736 2024-05-26 18:02:35.771810 pylonparser-0.1.3/pylonparser/scraper.py
+-rw-r--r--   0        0        0      758 2024-05-26 18:07:26.701783 pylonparser-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2705 1970-01-01 00:00:00.000000 pylonparser-0.1.3/PKG-INFO
```

### Comparing `pylonparser-0.1.2/LICENSE` & `pylonparser-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylonparser-0.1.2/README.md` & `pylonparser-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pylonparser-0.1.2/pyproject.toml` & `pylonparser-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylonparser"
-version = "0.1.2"
+version = "0.1.3"
 description = "A tool to parse football game stats."
 authors = ["Your Name <your.email@example.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/traxxo/pylonparser"
 repository = "https://github.com/traxxo/pylonparser"
 documentation = "https://github.com/traxxo/pylonparser/wiki"
@@ -17,11 +17,12 @@
 
 
 requests = "^2.32.2"
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.1"
 pre-commit = "^3.7.1"
 bump2version = "^1.0.1"
+pandas = "^2.2.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pylonparser-0.1.2/PKG-INFO` & `pylonparser-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylonparser
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to parse football game stats.
 Home-page: https://github.com/traxxo/pylonparser
 License: MIT
 Keywords: parser,football,stats,nfl,pro-football-by-reference
 Author: Your Name
 Author-email: your.email@example.com
 Requires-Python: >=3.10,<4.0
```

