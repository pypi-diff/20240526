# Comparing `tmp/aipkgs_requests-1.0.2.tar.gz` & `tmp/aipkgs_requests-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_requests-1.0.2.tar", max compression
+gzip compressed data, was "aipkgs_requests-1.0.3.tar", max compression
```

## Comparing `aipkgs_requests-1.0.2.tar` & `aipkgs_requests-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1058 2022-01-01 19:20:43.000000 aipkgs_requests-1.0.2/LICENSE.md
--rw-r--r--   0        0        0       13 2022-03-08 09:21:31.816882 aipkgs_requests-1.0.2/README.rst
--rw-r--r--   0        0        0      109 2022-03-08 12:59:23.046426 aipkgs_requests-1.0.2/aipkgs_requests/__init__.py
--rw-r--r--   0        0        0     1492 2022-09-03 17:57:35.173266 aipkgs_requests-1.0.2/aipkgs_requests/helpers.py
--rw-r--r--   0        0        0     1992 2022-09-03 17:57:35.176462 aipkgs_requests-1.0.2/aipkgs_requests/helpers_session.py
--rw-r--r--   0        0        0     2156 2023-10-28 13:29:46.880191 aipkgs_requests-1.0.2/aipkgs_requests/status.py
--rw-r--r--   0        0        0      534 2024-05-15 22:15:21.568803 aipkgs_requests-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 aipkgs_requests-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-01-01 19:20:43.000000 aipkgs_requests-1.0.3/LICENSE.md
+-rw-r--r--   0        0        0       13 2022-03-08 09:21:31.816882 aipkgs_requests-1.0.3/README.rst
+-rw-r--r--   0        0        0     1492 2022-09-03 17:57:35.173266 aipkgs_requests-1.0.3/aipkgs_requests/helpers.py
+-rw-r--r--   0        0        0     1992 2022-09-03 17:57:35.176462 aipkgs_requests-1.0.3/aipkgs_requests/helpers_session.py
+-rw-r--r--   0        0        0     2156 2023-10-28 13:29:46.880191 aipkgs_requests-1.0.3/aipkgs_requests/status.py
+-rw-r--r--   0        0        0      534 2024-05-25 22:41:30.047927 aipkgs_requests-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 aipkgs_requests-1.0.3/PKG-INFO
```

### Comparing `aipkgs_requests-1.0.2/LICENSE.md` & `aipkgs_requests-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_requests-1.0.2/aipkgs_requests/helpers.py` & `aipkgs_requests-1.0.3/aipkgs_requests/helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_requests-1.0.2/aipkgs_requests/helpers_session.py` & `aipkgs_requests-1.0.3/aipkgs_requests/helpers_session.py`

 * *Files identical despite different names*

### Comparing `aipkgs_requests-1.0.2/aipkgs_requests/status.py` & `aipkgs_requests-1.0.3/aipkgs_requests/status.py`

 * *Files identical despite different names*

### Comparing `aipkgs_requests-1.0.2/pyproject.toml` & `aipkgs_requests-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aipkgs-requests"
-version = "1.0.2"
+version = "1.0.3"
 description = "A package for requests"
 authors = ["Alexy <alexy.ib@outlook.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/packages.git"
 repository = "https://gitlab.com/aipy/packages.git"
 keywords = ["ai"]
@@ -16,9 +16,9 @@
 python = "^3.11.4"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
-requires = ["poetry-core>=1.0.2"]
+requires = ["poetry-core>=1.0.3"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aipkgs_requests-1.0.2/PKG-INFO` & `aipkgs_requests-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipkgs-requests
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for requests
 Home-page: https://gitlab.com/aipy/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.4,<4.0.0
```

