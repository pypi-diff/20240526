# Comparing `tmp/api_pipe-1.0.7.tar.gz` & `tmp/api_pipe-2.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_pipe-1.0.7.tar", max compression
+gzip compressed data, was "api_pipe-2.0.10.tar", max compression
```

## Comparing `api_pipe-1.0.7.tar` & `api_pipe-2.0.10.tar`

### file list

```diff
@@ -1,9 +1,22 @@
--rw-r--r--   0        0        0       11 2024-01-06 08:05:02.508433 api_pipe-1.0.7/README.md
--rw-r--r--   0        0        0      531 2024-02-02 08:03:13.996378 api_pipe-1.0.7/pyproject.toml
--rw-r--r--   0        0        0       43 2024-02-02 08:03:19.691939 api_pipe-1.0.7/src/api_pipe/__init__.py
--rw-r--r--   0        0        0     8836 2024-02-02 08:02:57.207282 api_pipe-1.0.7/src/api_pipe/api.py
--rw-r--r--   0        0        0      600 2024-01-14 07:11:54.785518 api_pipe-1.0.7/src/api_pipe/config.py
--rw-r--r--   0        0        0      797 2024-01-06 10:12:12.494414 api_pipe-1.0.7/src/api_pipe/logger.py
--rw-r--r--   0        0        0     1818 2024-02-02 06:48:33.176945 api_pipe-1.0.7/src/api_pipe/manual_test_run.py
--rw-r--r--   0        0        0      721 2024-01-06 10:44:07.416343 api_pipe-1.0.7/src/api_pipe/url.py
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 api_pipe-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-05-26 04:49:31.676215 api_pipe-2.0.10/README.md
+-rw-r--r--   0        0        0      557 2024-05-26 04:49:31.676215 api_pipe-2.0.10/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-05-26 04:49:31.676215 api_pipe-2.0.10/src/api_pipe/__init__.py
+-rw-r--r--   0        0        0     8504 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/api.py
+-rw-r--r--   0        0        0      827 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/config.py
+-rw-r--r--   0        0        0      555 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/directory.py
+-rw-r--r--   0        0        0     1577 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/error.py
+-rw-r--r--   0        0        0     1490 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/logger.py
+-rw-r--r--   0        0        0     3212 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/manual_test_run.py
+-rw-r--r--   0        0        0     3570 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/params.py
+-rw-r--r--   0        0        0     1056 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/params_schema.py
+-rw-r--r--   0        0        0        3 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/steps/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/steps/fetch.py
+-rw-r--r--   0        0        0     1900 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/steps/fetch_async.py
+-rw-r--r--   0        0        0     1002 2024-05-26 04:49:31.677215 api_pipe-2.0.10/src/api_pipe/steps/filter.py
+-rw-r--r--   0        0        0      649 2024-05-26 04:49:31.678215 api_pipe-2.0.10/src/api_pipe/steps/key.py
+-rw-r--r--   0        0        0     1237 2024-05-26 04:49:31.678215 api_pipe-2.0.10/src/api_pipe/steps/map.py
+-rw-r--r--   0        0        0      913 2024-05-26 04:49:31.678215 api_pipe-2.0.10/src/api_pipe/steps/select.py
+-rw-r--r--   0        0        0      507 2024-05-26 04:49:31.678215 api_pipe-2.0.10/src/api_pipe/steps/to_json.py
+-rw-r--r--   0        0        0      738 2024-05-26 04:49:31.678215 api_pipe-2.0.10/src/api_pipe/steps/to_python.py
+-rw-r--r--   0        0        0      720 2024-05-26 04:49:31.678215 api_pipe-2.0.10/src/api_pipe/url.py
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 api_pipe-2.0.10/PKG-INFO
```

### Comparing `api_pipe-1.0.7/pyproject.toml` & `api_pipe-2.0.10/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "api-pipe"
-version = "1.0.7"
+version = "2.0.10"
 description = "API Pipe"
 authors = ["Rafael Roman Otero <rromanotero@gmail.com>"]
 readme = "README.md"
 packages = [{include = "api_pipe", from = "src"}]
 
 [tool.poetry.scripts]
 manual-test-run = "api_pipe.manual_test_run:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-httpx = "^0.26.0"
+httpx = ">=0.26.0,<1.0.0"
 rich = "^13.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 toml = "^0.10.2"
 rich = "^13.7.0"
+mypy = "^1.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `api_pipe-1.0.7/src/api_pipe/url.py` & `api_pipe-2.0.10/src/api_pipe/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''
     URL
 '''
 class Url:
     '''
         URL
     '''
-
     def __init__(self, value: str) -> None:
         '''
             Init
         '''
         self.value = value
 
     def __truediv__(self, other) -> "Url":
```

