# Comparing `tmp/traceloop_sdk-0.9.3.tar.gz` & `tmp/traceloop_sdk-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceloop_sdk-0.9.3.tar", max compression
+gzip compressed data, was "traceloop_sdk-0.9.4.tar", max compression
```

## Comparing `traceloop_sdk-0.9.3.tar` & `traceloop_sdk-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      614 2024-01-15 12:27:15.735125 traceloop_sdk-0.9.3/README.md
--rw-r--r--   0        0        0     2139 2024-01-15 12:27:33.579167 traceloop_sdk-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     6485 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/__init__.py
--rw-r--r--   0        0        0      248 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/config/__init__.py
--rw-r--r--   0        0        0     8262 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/decorators/__init__.py
--rw-r--r--   0        0        0     4277 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/fetcher.py
--rw-r--r--   0        0        0      154 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/prompts/__init__.py
--rw-r--r--   0        0        0     5591 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/prompts/client.py
--rw-r--r--   0        0        0     1558 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/prompts/model.py
--rw-r--r--   0        0        0      410 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/prompts/registry.py
--rw-r--r--   0        0        0     2430 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/telemetry.py
--rw-r--r--   0        0        0      141 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/tracing/__init__.py
--rw-r--r--   0        0        0      846 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/tracing/content_allow_list.py
--rw-r--r--   0        0        0      299 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/tracing/context_manager.py
--rw-r--r--   0        0        0    15040 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/tracing/tracing.py
--rw-r--r--   0        0        0      604 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/utils/__init__.py
--rw-r--r--   0        0        0     2112 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/utils/in_memory_span_exporter.py
--rw-r--r--   0        0        0       22 2024-01-15 12:27:15.739125 traceloop_sdk-0.9.3/traceloop/sdk/version.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 traceloop_sdk-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      614 2024-01-15 22:28:45.812170 traceloop_sdk-0.9.4/README.md
+-rw-r--r--   0        0        0     2139 2024-01-15 22:29:05.488363 traceloop_sdk-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     6485 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/__init__.py
+-rw-r--r--   0        0        0      248 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/config/__init__.py
+-rw-r--r--   0        0        0     8262 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/decorators/__init__.py
+-rw-r--r--   0        0        0     4277 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/fetcher.py
+-rw-r--r--   0        0        0      154 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/prompts/__init__.py
+-rw-r--r--   0        0        0     5591 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/prompts/client.py
+-rw-r--r--   0        0        0     1558 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/prompts/model.py
+-rw-r--r--   0        0        0      410 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/prompts/registry.py
+-rw-r--r--   0        0        0     2430 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/telemetry.py
+-rw-r--r--   0        0        0      141 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/tracing/__init__.py
+-rw-r--r--   0        0        0      846 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/tracing/content_allow_list.py
+-rw-r--r--   0        0        0      299 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/tracing/context_manager.py
+-rw-r--r--   0        0        0    15040 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/tracing/tracing.py
+-rw-r--r--   0        0        0      604 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2112 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/utils/in_memory_span_exporter.py
+-rw-r--r--   0        0        0       22 2024-01-15 22:28:45.816170 traceloop_sdk-0.9.4/traceloop/sdk/version.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 traceloop_sdk-0.9.4/PKG-INFO
```

### Comparing `traceloop_sdk-0.9.3/README.md` & `traceloop_sdk-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/pyproject.toml` & `traceloop_sdk-0.9.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "traceloop-sdk"
-version = "0.9.3"
+version = "0.9.4"
 description = "Traceloop Software Development Kit (SDK) for Python"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 repository = "https://github.com/traceloop/openllmetry"
@@ -29,25 +29,25 @@
 opentelemetry-sdk = "^1.20.0"
 opentelemetry-exporter-otlp-proto-http = "^1.20.0"
 opentelemetry-exporter-otlp-proto-grpc = "^1.20.0"
 opentelemetry-instrumentation-requests = "0.43b0"
 opentelemetry-instrumentation-pymysql = "0.43b0"
 opentelemetry-instrumentation-urllib3 = "0.43b0"
 opentelemetry-semantic-conventions-ai = "^0.0.14"
-opentelemetry-instrumentation-openai = "^0.9.3"
-opentelemetry-instrumentation-anthropic = "^0.9.3"
-opentelemetry-instrumentation-cohere = "^0.9.3"
-opentelemetry-instrumentation-pinecone = "^0.9.3"
-opentelemetry-instrumentation-langchain = "^0.9.3"
-opentelemetry-instrumentation-chromadb = "^0.9.3"
-opentelemetry-instrumentation-transformers = "^0.9.3"
-opentelemetry-instrumentation-llamaindex = "^0.9.3"
-opentelemetry-instrumentation-bedrock = "^0.9.3"
-opentelemetry-instrumentation-replicate = "^0.9.3"
-opentelemetry-instrumentation-vertexai = "^0.9.3"
+opentelemetry-instrumentation-openai = "^0.9.4"
+opentelemetry-instrumentation-anthropic = "^0.9.4"
+opentelemetry-instrumentation-cohere = "^0.9.4"
+opentelemetry-instrumentation-pinecone = "^0.9.4"
+opentelemetry-instrumentation-langchain = "^0.9.4"
+opentelemetry-instrumentation-chromadb = "^0.9.4"
+opentelemetry-instrumentation-transformers = "^0.9.4"
+opentelemetry-instrumentation-llamaindex = "^0.9.4"
+opentelemetry-instrumentation-bedrock = "^0.9.4"
+opentelemetry-instrumentation-replicate = "^0.9.4"
+opentelemetry-instrumentation-vertexai = "^0.9.4"
 colorama = "^0.4.6"
 tenacity = "^8.2.3"
 pydantic = ">=1"
 jinja2 = "^3.1.2"
 deprecated = "^1.2.14"
 posthog = "^3.0.2"
```

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/__init__.py` & `traceloop_sdk-0.9.4/traceloop/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/decorators/__init__.py` & `traceloop_sdk-0.9.4/traceloop/sdk/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/fetcher.py` & `traceloop_sdk-0.9.4/traceloop/sdk/fetcher.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/prompts/client.py` & `traceloop_sdk-0.9.4/traceloop/sdk/prompts/client.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/prompts/model.py` & `traceloop_sdk-0.9.4/traceloop/sdk/prompts/model.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/telemetry.py` & `traceloop_sdk-0.9.4/traceloop/sdk/telemetry.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/tracing/content_allow_list.py` & `traceloop_sdk-0.9.4/traceloop/sdk/tracing/content_allow_list.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/tracing/tracing.py` & `traceloop_sdk-0.9.4/traceloop/sdk/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/utils/__init__.py` & `traceloop_sdk-0.9.4/traceloop/sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/traceloop/sdk/utils/in_memory_span_exporter.py` & `traceloop_sdk-0.9.4/traceloop/sdk/utils/in_memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.9.3/PKG-INFO` & `traceloop_sdk-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceloop-sdk
-Version: 0.9.3
+Version: 0.9.4
 Summary: Traceloop Software Development Kit (SDK) for Python
 Home-page: https://github.com/traceloop/openllmetry
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,28 +15,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (>=1.20.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.20.0,<2.0.0)
-Requires-Dist: opentelemetry-instrumentation-anthropic (>=0.9.3,<0.10.0)
-Requires-Dist: opentelemetry-instrumentation-bedrock (>=0.9.3,<0.10.0)
-Requires-Dist: opentelemetry-instrumentation-chromadb (>=0.9.3,<0.10.0)
-Requires-Dist: opentelemetry-instrumentation-cohere (>=0.9.3,<0.10.0)
-Requires-Dist: opentelemetry-instrumentation-langchain (>=0.9.3,<0.10.0)
-Requires-Dist: opentelemetry-instrumentation-llamaindex (>=0.9.3,<0.10.0)
-Requires-Dist: opentelemetry-instrumentation-openai (>=0.9.3,<0.10.0)
-Requires-Dist: opentelemetry-instrumentation-pinecone (>=0.9.3,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-anthropic (>=0.9.4,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-bedrock (>=0.9.4,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-chromadb (>=0.9.4,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-cohere (>=0.9.4,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-langchain (>=0.9.4,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-llamaindex (>=0.9.4,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-openai (>=0.9.4,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-pinecone (>=0.9.4,<0.10.0)
 Requires-Dist: opentelemetry-instrumentation-pymysql (==0.43b0)
-Requires-Dist: opentelemetry-instrumentation-replicate (>=0.9.3,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-replicate (>=0.9.4,<0.10.0)
 Requires-Dist: opentelemetry-instrumentation-requests (==0.43b0)
-Requires-Dist: opentelemetry-instrumentation-transformers (>=0.9.3,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-transformers (>=0.9.4,<0.10.0)
 Requires-Dist: opentelemetry-instrumentation-urllib3 (==0.43b0)
-Requires-Dist: opentelemetry-instrumentation-vertexai (>=0.9.3,<0.10.0)
+Requires-Dist: opentelemetry-instrumentation-vertexai (>=0.9.4,<0.10.0)
 Requires-Dist: opentelemetry-sdk (>=1.20.0,<2.0.0)
 Requires-Dist: opentelemetry-semantic-conventions-ai (>=0.0.14,<0.0.15)
 Requires-Dist: posthog (>=3.0.2,<4.0.0)
 Requires-Dist: pydantic (>=1)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Project-URL: Documentation, https://traceloop.com/docs/python-sdk
 Project-URL: Repository, https://github.com/traceloop/openllmetry
```

