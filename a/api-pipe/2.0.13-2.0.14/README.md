# Comparing `tmp/api_pipe-2.0.13.tar.gz` & `tmp/api_pipe-2.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_pipe-2.0.13.tar", max compression
+gzip compressed data, was "api_pipe-2.0.14.tar", max compression
```

## Comparing `api_pipe-2.0.13.tar` & `api_pipe-2.0.14.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       11 2024-05-26 05:18:45.354088 api_pipe-2.0.13/README.md
--rw-r--r--   0        0        0      557 2024-05-26 05:20:27.000000 api_pipe-2.0.13/pyproject.toml
--rw-r--r--   0        0        0       78 2024-05-26 05:20:27.000000 api_pipe-2.0.13/src/api_pipe/__init__.py
--rw-r--r--   0        0        0     8504 2024-05-26 05:18:45.354088 api_pipe-2.0.13/src/api_pipe/api.py
--rw-r--r--   0        0        0      827 2024-05-26 05:18:45.354088 api_pipe-2.0.13/src/api_pipe/config.py
--rw-r--r--   0        0        0      556 2024-05-26 05:20:26.503985 api_pipe-2.0.13/src/api_pipe/directory.py
--rw-r--r--   0        0        0     1577 2024-05-26 05:18:45.354088 api_pipe-2.0.13/src/api_pipe/error.py
--rw-r--r--   0        0        0     1490 2024-05-26 05:18:45.354088 api_pipe-2.0.13/src/api_pipe/logger.py
--rw-r--r--   0        0        0     3212 2024-05-26 05:18:45.354088 api_pipe-2.0.13/src/api_pipe/manual_test_run.py
--rw-r--r--   0        0        0     3570 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/params.py
--rw-r--r--   0        0        0     1057 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/params_schema.py
--rw-r--r--   0        0        0        3 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/steps/__init__.py
--rw-r--r--   0        0        0     2117 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/steps/fetch.py
--rw-r--r--   0        0        0     1900 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/steps/fetch_async.py
--rw-r--r--   0        0        0     1002 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/steps/filter.py
--rw-r--r--   0        0        0      649 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/steps/key.py
--rw-r--r--   0        0        0     1237 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/steps/map.py
--rw-r--r--   0        0        0      913 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/steps/select.py
--rw-r--r--   0        0        0      507 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/steps/to_json.py
--rw-r--r--   0        0        0      738 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/steps/to_python.py
--rw-r--r--   0        0        0      720 2024-05-26 05:18:45.355088 api_pipe-2.0.13/src/api_pipe/url.py
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 api_pipe-2.0.13/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-05-26 05:25:53.529127 api_pipe-2.0.14/README.md
+-rw-r--r--   0        0        0      557 2024-05-26 05:26:39.000000 api_pipe-2.0.14/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-05-26 05:26:39.000000 api_pipe-2.0.14/src/api_pipe/__init__.py
+-rw-r--r--   0        0        0     8504 2024-05-26 05:25:53.529127 api_pipe-2.0.14/src/api_pipe/api.py
+-rw-r--r--   0        0        0      827 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/config.py
+-rw-r--r--   0        0        0      556 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/directory.py
+-rw-r--r--   0        0        0     1577 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/error.py
+-rw-r--r--   0        0        0     1491 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/logger.py
+-rw-r--r--   0        0        0     3212 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/manual_test_run.py
+-rw-r--r--   0        0        0     3570 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/params.py
+-rw-r--r--   0        0        0     1057 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/params_schema.py
+-rw-r--r--   0        0        0        3 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/steps/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/steps/fetch.py
+-rw-r--r--   0        0        0     1900 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/steps/fetch_async.py
+-rw-r--r--   0        0        0     1002 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/steps/filter.py
+-rw-r--r--   0        0        0      649 2024-05-26 05:25:53.530127 api_pipe-2.0.14/src/api_pipe/steps/key.py
+-rw-r--r--   0        0        0     1237 2024-05-26 05:25:53.531127 api_pipe-2.0.14/src/api_pipe/steps/map.py
+-rw-r--r--   0        0        0      913 2024-05-26 05:25:53.531127 api_pipe-2.0.14/src/api_pipe/steps/select.py
+-rw-r--r--   0        0        0      507 2024-05-26 05:25:53.531127 api_pipe-2.0.14/src/api_pipe/steps/to_json.py
+-rw-r--r--   0        0        0      738 2024-05-26 05:25:53.531127 api_pipe-2.0.14/src/api_pipe/steps/to_python.py
+-rw-r--r--   0        0        0      720 2024-05-26 05:25:53.531127 api_pipe-2.0.14/src/api_pipe/url.py
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 api_pipe-2.0.14/PKG-INFO
```

### Comparing `api_pipe-2.0.13/pyproject.toml` & `api_pipe-2.0.14/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "api-pipe"
-version = "2.0.13"
+version = "2.0.14"
 description = "API Pipe"
 authors = ["Rafael Roman Otero <rromanotero@gmail.com>"]
 readme = "README.md"
 packages = [{include = "api_pipe", from = "src"}]
 
 [tool.poetry.scripts]
 manual-test-run = "api_pipe.manual_test_run:main"
```

### Comparing `api_pipe-2.0.13/src/api_pipe/api.py` & `api_pipe-2.0.14/src/api_pipe/api.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/config.py` & `api_pipe-2.0.14/src/api_pipe/config.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/directory.py` & `api_pipe-2.0.14/src/api_pipe/directory.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/error.py` & `api_pipe-2.0.14/src/api_pipe/error.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/logger.py` & `api_pipe-2.0.14/src/api_pipe/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         log_to_file: Optional[Path] = None
     ) -> logging.Logger:
     '''
         Sets up a logger that logs to stdout
 
         Uses RichHandler to pretty print logs
 
-        When log_level is DEBUG, also logs to a file in log_to_file
+        When log_level is DEBUG, also logs to a file in log_to_file.
     '''
     #stdout handler
     stdout_handler = RichHandler(
         show_time=config.logger_show_time,
         keywords=[w.lower() for w in log_words_to_highlight] + \
                  [w.upper() for w in log_words_to_highlight] + \
                  [w.capitalize() for w in log_words_to_highlight]
```

### Comparing `api_pipe-2.0.13/src/api_pipe/manual_test_run.py` & `api_pipe-2.0.14/src/api_pipe/manual_test_run.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/params.py` & `api_pipe-2.0.14/src/api_pipe/params.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/params_schema.py` & `api_pipe-2.0.14/src/api_pipe/params_schema.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/steps/fetch.py` & `api_pipe-2.0.14/src/api_pipe/steps/fetch.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/steps/fetch_async.py` & `api_pipe-2.0.14/src/api_pipe/steps/fetch_async.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/steps/filter.py` & `api_pipe-2.0.14/src/api_pipe/steps/filter.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/steps/key.py` & `api_pipe-2.0.14/src/api_pipe/steps/key.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/steps/map.py` & `api_pipe-2.0.14/src/api_pipe/steps/map.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/steps/select.py` & `api_pipe-2.0.14/src/api_pipe/steps/select.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/steps/to_python.py` & `api_pipe-2.0.14/src/api_pipe/steps/to_python.py`

 * *Files identical despite different names*

### Comparing `api_pipe-2.0.13/src/api_pipe/url.py` & `api_pipe-2.0.14/src/api_pipe/url.py`

 * *Files identical despite different names*

