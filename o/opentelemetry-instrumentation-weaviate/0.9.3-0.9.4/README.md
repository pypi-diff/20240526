# Comparing `tmp/opentelemetry_instrumentation_weaviate-0.9.3.tar.gz` & `tmp/opentelemetry_instrumentation_weaviate-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_weaviate-0.9.3.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_weaviate-0.9.4.tar", max compression
```

## Comparing `opentelemetry_instrumentation_weaviate-0.9.3.tar` & `opentelemetry_instrumentation_weaviate-0.9.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       68 2024-01-15 12:25:43.157360 opentelemetry_instrumentation_weaviate-0.9.3/README.md
--rw-r--r--   0        0        0       45 2024-01-15 12:25:43.157360 opentelemetry_instrumentation_weaviate-0.9.3/opentelemetry/instrumentation/weaviate/__init__.py
--rw-r--r--   0        0        0       22 2024-01-15 12:25:43.157360 opentelemetry_instrumentation_weaviate-0.9.3/opentelemetry/instrumentation/weaviate/version.py
--rw-r--r--   0        0        0      928 2024-01-15 12:26:08.169189 opentelemetry_instrumentation_weaviate-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_weaviate-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0       68 2024-01-15 22:27:20.427534 opentelemetry_instrumentation_weaviate-0.9.4/README.md
+-rw-r--r--   0        0        0       45 2024-01-15 22:27:20.427534 opentelemetry_instrumentation_weaviate-0.9.4/opentelemetry/instrumentation/weaviate/__init__.py
+-rw-r--r--   0        0        0       22 2024-01-15 22:27:20.427534 opentelemetry_instrumentation_weaviate-0.9.4/opentelemetry/instrumentation/weaviate/version.py
+-rw-r--r--   0        0        0      928 2024-01-15 22:27:44.183579 opentelemetry_instrumentation_weaviate-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_weaviate-0.9.4/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_weaviate-0.9.3/pyproject.toml` & `opentelemetry_instrumentation_weaviate-0.9.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = ['if TYPE_CHECKING:']
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-weaviate"
-version = "0.9.3"
+version = "0.9.4"
 description = "OpenTelemetry Weaviate instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 license = "Apache-2.0"
```

### Comparing `opentelemetry_instrumentation_weaviate-0.9.3/PKG-INFO` & `opentelemetry_instrumentation_weaviate-0.9.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-weaviate
-Version: 0.9.3
+Version: 0.9.4
 Summary: OpenTelemetry Weaviate instrumentation
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

