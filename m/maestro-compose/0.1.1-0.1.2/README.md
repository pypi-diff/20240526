# Comparing `tmp/maestro_compose-0.1.1.tar.gz` & `tmp/maestro_compose-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro_compose-0.1.1.tar", max compression
+gzip compressed data, was "maestro_compose-0.1.2.tar", max compression
```

## Comparing `maestro_compose-0.1.1.tar` & `maestro_compose-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        9 2024-05-25 23:28:35.104821 maestro_compose-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-25 23:20:44.277925 maestro_compose-0.1.1/maestro_compose/__init__.py
--rw-r--r--   0        0        0     5844 2024-05-25 23:29:56.483183 maestro_compose-0.1.1/maestro_compose/__main__.py
--rw-r--r--   0        0        0      759 2024-05-25 23:48:25.665704 maestro_compose-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      845 1970-01-01 00:00:00.000000 maestro_compose-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        9 2024-05-25 23:28:35.104821 maestro_compose-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 23:20:44.277925 maestro_compose-0.1.2/maestro_compose/__init__.py
+-rw-r--r--   0        0        0     5844 2024-05-25 23:29:56.483183 maestro_compose-0.1.2/maestro_compose/__main__.py
+-rw-r--r--   0        0        0      765 2024-05-25 23:49:59.398906 maestro_compose-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 maestro_compose-0.1.2/PKG-INFO
```

### Comparing `maestro_compose-0.1.1/maestro_compose/__main__.py` & `maestro_compose-0.1.2/maestro_compose/__main__.py`

 * *Files identical despite different names*

### Comparing `maestro_compose-0.1.1/pyproject.toml` & `maestro_compose-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "maestro-compose"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple command line tool for managing Docker Compose stacks using tags and other metadata."
 license = "MIT"
 authors = ["Nick Schenone <nschenone16@gmail.com>"]
 readme = "README.md"
-repository = "https://github.com/nschenone/notionaut"
+repository = "https://github.com/nschenone/maestro-compose"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 click = "^8.1.7"
 pydantic = "^2.7.1"
 pyyaml = "^6.0.1"
```

### Comparing `maestro_compose-0.1.1/PKG-INFO` & `maestro_compose-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: maestro-compose
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple command line tool for managing Docker Compose stacks using tags and other metadata.
-Home-page: https://github.com/nschenone/notionaut
+Home-page: https://github.com/nschenone/maestro-compose
 License: MIT
 Author: Nick Schenone
 Author-email: nschenone16@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Project-URL: Repository, https://github.com/nschenone/notionaut
+Project-URL: Repository, https://github.com/nschenone/maestro-compose
 Description-Content-Type: text/markdown
 
 # Maestro
```

