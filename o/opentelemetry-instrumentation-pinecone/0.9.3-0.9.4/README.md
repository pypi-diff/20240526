# Comparing `tmp/opentelemetry_instrumentation_pinecone-0.9.3.tar.gz` & `tmp/opentelemetry_instrumentation_pinecone-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_pinecone-0.9.3.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_pinecone-0.9.4.tar", max compression
```

## Comparing `opentelemetry_instrumentation_pinecone-0.9.3.tar` & `opentelemetry_instrumentation_pinecone-0.9.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      455 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_pinecone-0.9.3/README.md
--rw-r--r--   0        0        0     4221 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_pinecone-0.9.3/opentelemetry/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0       22 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_pinecone-0.9.3/opentelemetry/instrumentation/pinecone/version.py
--rw-r--r--   0        0        0      929 2024-01-15 12:26:05.553209 opentelemetry_instrumentation_pinecone-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_pinecone-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      455 2024-01-15 22:27:20.427534 opentelemetry_instrumentation_pinecone-0.9.4/README.md
+-rw-r--r--   0        0        0     4221 2024-01-15 22:27:20.427534 opentelemetry_instrumentation_pinecone-0.9.4/opentelemetry/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0       22 2024-01-15 22:27:20.427534 opentelemetry_instrumentation_pinecone-0.9.4/opentelemetry/instrumentation/pinecone/version.py
+-rw-r--r--   0        0        0      929 2024-01-15 22:27:41.727574 opentelemetry_instrumentation_pinecone-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_pinecone-0.9.4/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_pinecone-0.9.3/opentelemetry/instrumentation/pinecone/__init__.py` & `opentelemetry_instrumentation_pinecone-0.9.4/opentelemetry/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_pinecone-0.9.3/pyproject.toml` & `opentelemetry_instrumentation_pinecone-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-pinecone"
-version = "0.9.3"
+version = "0.9.4"
 description = "OpenTelemetry Pinecone instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 license = "Apache-2.0"
```

### Comparing `opentelemetry_instrumentation_pinecone-0.9.3/PKG-INFO` & `opentelemetry_instrumentation_pinecone-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-pinecone
-Version: 0.9.3
+Version: 0.9.4
 Summary: OpenTelemetry Pinecone instrumentation
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-pinecone Version:
-0.9.3 Summary: OpenTelemetry Pinecone instrumentation License: Apache-2.0
+0.9.4 Summary: OpenTelemetry Pinecone instrumentation License: Apache-2.0
 Author: Gal Kleinman Author-email: gal@traceloop.com Requires-Python:
 >=3.8.1,<4 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation (==0.43b0) Requires-Dist:
```

