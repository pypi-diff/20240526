# Comparing `tmp/api_pipe-2.0.16.tar.gz` & `tmp/api_pipe-2.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_pipe-2.0.16.tar", max compression
+gzip compressed data, was "api_pipe-2.0.17.tar", max compression
```

## Comparing `api_pipe-2.0.16.tar` & `api_pipe-2.0.17.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       11 2024-05-26 06:09:31.247524 api_pipe-2.0.16/README.md
--rw-r--r--   0        0        0      557 2024-05-26 06:05:14.000000 api_pipe-2.0.16/pyproject.toml
--rw-r--r--   0        0        0       78 2024-05-26 06:05:14.000000 api_pipe-2.0.16/src/api_pipe/__init__.py
--rw-r--r--   0        0        0     8504 2024-05-26 06:09:31.247524 api_pipe-2.0.16/src/api_pipe/api.py
--rw-r--r--   0        0        0      827 2024-05-26 06:09:31.247524 api_pipe-2.0.16/src/api_pipe/config.py
--rw-r--r--   0        0        0      555 2024-05-26 06:09:31.247524 api_pipe-2.0.16/src/api_pipe/directory.py
--rw-r--r--   0        0        0     1577 2024-05-26 06:09:31.247524 api_pipe-2.0.16/src/api_pipe/error.py
--rw-r--r--   0        0        0     1491 2024-05-26 06:09:31.247524 api_pipe-2.0.16/src/api_pipe/logger.py
--rw-r--r--   0        0        0     3212 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/manual_test_run.py
--rw-r--r--   0        0        0     3570 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/params.py
--rw-r--r--   0        0        0     1056 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/params_schema.py
--rw-r--r--   0        0        0        3 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/steps/__init__.py
--rw-r--r--   0        0        0     2117 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/steps/fetch.py
--rw-r--r--   0        0        0     1900 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/steps/fetch_async.py
--rw-r--r--   0        0        0     1002 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/steps/filter.py
--rw-r--r--   0        0        0      649 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/steps/key.py
--rw-r--r--   0        0        0     1237 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/steps/map.py
--rw-r--r--   0        0        0      913 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/steps/select.py
--rw-r--r--   0        0        0      507 2024-05-26 06:09:31.248524 api_pipe-2.0.16/src/api_pipe/steps/to_json.py
--rw-r--r--   0        0        0      738 2024-05-26 06:09:31.249524 api_pipe-2.0.16/src/api_pipe/steps/to_python.py
--rw-r--r--   0        0        0      720 2024-05-26 06:09:31.249524 api_pipe-2.0.16/src/api_pipe/url.py
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 api_pipe-2.0.16/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-05-26 06:20:52.224151 api_pipe-2.0.17/README.md
+-rw-r--r--   0        0        0      557 2024-05-26 06:16:29.000000 api_pipe-2.0.17/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-05-26 06:16:29.000000 api_pipe-2.0.17/src/api_pipe/__init__.py
+-rw-r--r--   0        0        0     8504 2024-05-26 06:20:52.224151 api_pipe-2.0.17/src/api_pipe/api.py
+-rw-r--r--   0        0        0      827 2024-05-26 06:20:52.224151 api_pipe-2.0.17/src/api_pipe/config.py
+-rw-r--r--   0        0        0      555 2024-05-26 06:20:52.224151 api_pipe-2.0.17/src/api_pipe/directory.py
+-rw-r--r--   0        0        0     1577 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/error.py
+-rw-r--r--   0        0        0     1491 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/logger.py
+-rw-r--r--   0        0        0     3212 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/manual_test_run.py
+-rw-r--r--   0        0        0     3569 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/params.py
+-rw-r--r--   0        0        0     1056 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/params_schema.py
+-rw-r--r--   0        0        0        3 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/steps/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/steps/fetch.py
+-rw-r--r--   0        0        0     1900 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/steps/fetch_async.py
+-rw-r--r--   0        0        0     1002 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/steps/filter.py
+-rw-r--r--   0        0        0      649 2024-05-26 06:20:52.225151 api_pipe-2.0.17/src/api_pipe/steps/key.py
+-rw-r--r--   0        0        0     1237 2024-05-26 06:20:52.226151 api_pipe-2.0.17/src/api_pipe/steps/map.py
+-rw-r--r--   0        0        0      913 2024-05-26 06:20:52.226151 api_pipe-2.0.17/src/api_pipe/steps/select.py
+-rw-r--r--   0        0        0      507 2024-05-26 06:20:52.226151 api_pipe-2.0.17/src/api_pipe/steps/to_json.py
+-rw-r--r--   0        0        0      738 2024-05-26 06:20:52.226151 api_pipe-2.0.17/src/api_pipe/steps/to_python.py
+-rw-r--r--   0        0        0      720 2024-05-26 06:20:52.226151 api_pipe-2.0.17/src/api_pipe/url.py
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 api_pipe-2.0.17/PKG-INFO
```

### Comparing `api_pipe-2.0.16/pyproject.toml` & `api_pipe-2.0.17/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "api-pipe"
-version = "2.0.16"
+version = "2.0.17"
 description = "API Pipe"
 authors = ["Rafael Roman Otero <rromanotero@gmail.com>"]
 readme = "README.md"
 packages = [{include = "api_pipe", from = "src"}]
 
 [tool.poetry.scripts]
 manual-test-run = "api_pipe.manual_test_run:main"
```

### Comparing `api_pipe-2.0.16/src/api_pipe/api.py` & `api_pipe-2.0.17/src/api_pipe/api.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/config.py` & `api_pipe-2.0.17/src/api_pipe/config.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/directory.py` & `api_pipe-2.0.17/src/api_pipe/directory.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/error.py` & `api_pipe-2.0.17/src/api_pipe/error.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/logger.py` & `api_pipe-2.0.17/src/api_pipe/logger.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/manual_test_run.py` & `api_pipe-2.0.17/src/api_pipe/manual_test_run.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/params.py` & `api_pipe-2.0.17/src/api_pipe/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         '''
             String representation
         '''
         return f"ApiParams(headers={self.headers}, timeout={self.timeout}, retries={self.retries}, logs={self.logs})"
 
     def validate(self) -> None:
         '''
-            Validates params against parameters schemas.
+            Validates params against parameters schemas
         '''
         for field in fields(self):
 
             try:
                 param_name = field.name
                 param_value = getattr(self, param_name)
             except AttributeError as e:
```

### Comparing `api_pipe-2.0.16/src/api_pipe/params_schema.py` & `api_pipe-2.0.17/src/api_pipe/params_schema.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/steps/fetch.py` & `api_pipe-2.0.17/src/api_pipe/steps/fetch.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/steps/fetch_async.py` & `api_pipe-2.0.17/src/api_pipe/steps/fetch_async.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/steps/filter.py` & `api_pipe-2.0.17/src/api_pipe/steps/filter.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/steps/key.py` & `api_pipe-2.0.17/src/api_pipe/steps/key.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/steps/map.py` & `api_pipe-2.0.17/src/api_pipe/steps/map.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/steps/select.py` & `api_pipe-2.0.17/src/api_pipe/steps/select.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/steps/to_python.py` & `api_pipe-2.0.17/src/api_pipe/steps/to_python.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.16/src/api_pipe/url.py` & `api_pipe-2.0.17/src/api_pipe/url.py`

 * *Files identical despite different names*

