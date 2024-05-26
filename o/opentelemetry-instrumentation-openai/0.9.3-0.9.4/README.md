# Comparing `tmp/opentelemetry_instrumentation_openai-0.9.3.tar.gz` & `tmp/opentelemetry_instrumentation_openai-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_openai-0.9.3.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_openai-0.9.4.tar", max compression
```

## Comparing `opentelemetry_instrumentation_openai-0.9.3.tar` & `opentelemetry_instrumentation_openai-0.9.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      999 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/README.md
--rw-r--r--   0        0        0      937 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     4501 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/shared/__init__.py
--rw-r--r--   0        0        0     5957 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/shared/chat_wrappers.py
--rw-r--r--   0        0        0     4472 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/shared/completion_wrappers.py
--rw-r--r--   0        0        0     2711 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py
--rw-r--r--   0        0        0      546 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/utils.py
--rw-r--r--   0        0        0     1613 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/v0/__init__.py
--rw-r--r--   0        0        0     1983 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/v1/__init__.py
--rw-r--r--   0        0        0       22 2024-01-15 12:25:43.153360 opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0      921 2024-01-15 12:26:06.981198 opentelemetry_instrumentation_openai-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_openai-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      999 2024-01-15 22:27:20.423534 opentelemetry_instrumentation_openai-0.9.4/README.md
+-rw-r--r--   0        0        0      937 2024-01-15 22:27:20.423534 opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     4384 2024-01-15 22:27:20.423534 opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/shared/__init__.py
+-rw-r--r--   0        0        0     6133 2024-01-15 22:27:20.423534 opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/shared/chat_wrappers.py
+-rw-r--r--   0        0        0     4650 2024-01-15 22:27:20.423534 opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/shared/completion_wrappers.py
+-rw-r--r--   0        0        0     2889 2024-01-15 22:27:20.423534 opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py
+-rw-r--r--   0        0        0      546 2024-01-15 22:27:20.423534 opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/utils.py
+-rw-r--r--   0        0        0     1613 2024-01-15 22:27:20.427534 opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/v0/__init__.py
+-rw-r--r--   0        0        0     1983 2024-01-15 22:27:20.427534 opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/v1/__init__.py
+-rw-r--r--   0        0        0       22 2024-01-15 22:27:20.427534 opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0      921 2024-01-15 22:27:43.179577 opentelemetry_instrumentation_openai-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_openai-0.9.4/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_openai-0.9.3/README.md` & `opentelemetry_instrumentation_openai-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/__init__.py` & `opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/shared/__init__.py` & `opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/shared/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,24 +59,21 @@
         _set_span_attribute(span, f"{prefix}.name", function.get("name"))
         _set_span_attribute(span, f"{prefix}.description", function.get("description"))
         _set_span_attribute(
             span, f"{prefix}.parameters", json.dumps(function.get("parameters"))
         )
 
 
-def _set_request_attributes(span, llm_request_type, kwargs):
+def _set_request_attributes(span, kwargs):
     if not span.is_recording():
         return
 
     try:
         _set_api_attributes(span)
         _set_span_attribute(span, SpanAttributes.LLM_VENDOR, "OpenAI")
-        _set_span_attribute(
-            span, SpanAttributes.LLM_REQUEST_TYPE, llm_request_type.value
-        )
         _set_span_attribute(span, SpanAttributes.LLM_REQUEST_MODEL, kwargs.get("model"))
         _set_span_attribute(
             span, SpanAttributes.LLM_REQUEST_MAX_TOKENS, kwargs.get("max_tokens")
         )
         _set_span_attribute(
             span, SpanAttributes.LLM_TEMPERATURE, kwargs.get("temperature")
         )
@@ -132,15 +129,17 @@
         )
 
 
 def is_streaming_response(response):
     if is_openai_v1():
         return isinstance(response, openai.Stream)
 
-    return isinstance(response, types.GeneratorType) or isinstance(response, types.AsyncGeneratorType)
+    return isinstance(response, types.GeneratorType) or isinstance(
+        response, types.AsyncGeneratorType
+    )
 
 
 def model_as_dict(model):
     if version("pydantic") < "2.0.0":
         return model.dict()
 
     return model.model_dump()
```

### Comparing `opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/shared/chat_wrappers.py` & `opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/shared/chat_wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 import logging
 
 from opentelemetry import context as context_api
 
 from opentelemetry.semconv.ai import SpanAttributes, LLMRequestTypeValues
 
 from opentelemetry.instrumentation.utils import _SUPPRESS_INSTRUMENTATION_KEY
-from opentelemetry.instrumentation.openai.utils import (
-    _with_tracer_wrapper
-)
+from opentelemetry.instrumentation.openai.utils import _with_tracer_wrapper
 from opentelemetry.instrumentation.openai.shared import (
     _set_request_attributes,
     _set_span_attribute,
     _set_functions_attributes,
     _set_response_attributes,
     is_streaming_response,
     should_send_prompts,
@@ -31,15 +29,19 @@
 
 @_with_tracer_wrapper
 def chat_wrapper(tracer, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     # span needs to be opened and closed manually because the response is a generator
-    span = tracer.start_span(SPAN_NAME, kind=SpanKind.CLIENT)
+    span = tracer.start_span(
+        SPAN_NAME,
+        kind=SpanKind.CLIENT,
+        attributes={SpanAttributes.LLM_REQUEST_TYPE: LLM_REQUEST_TYPE.value},
+    )
 
     _handle_request(span, kwargs)
     response = wrapped(*args, **kwargs)
 
     if is_streaming_response(response):
         # span will be closed after the generator is done
         return _build_from_streaming_response(span, response)
@@ -51,30 +53,34 @@
 
 
 @_with_tracer_wrapper
 async def achat_wrapper(tracer, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
-    span = tracer.start_span(SPAN_NAME, kind=SpanKind.CLIENT)
+    span = tracer.start_span(
+        SPAN_NAME,
+        kind=SpanKind.CLIENT,
+        attributes={SpanAttributes.LLM_REQUEST_TYPE: LLM_REQUEST_TYPE.value},
+    )
     _handle_request(span, kwargs)
     response = await wrapped(*args, **kwargs)
 
     if is_streaming_response(response):
         # span will be closed after the generator is done
         return _abuild_from_streaming_response(span, response)
 
     _handle_response(response, span)
     span.end()
 
     return response
 
 
 def _handle_request(span, kwargs):
-    _set_request_attributes(span, LLM_REQUEST_TYPE, kwargs)
+    _set_request_attributes(span, kwargs)
     if should_send_prompts():
         _set_prompts(span, kwargs.get("messages"))
         _set_functions_attributes(span, kwargs.get("functions"))
 
 
 def _handle_response(response, span):
     if is_openai_v1():
```

### Comparing `opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/shared/completion_wrappers.py` & `opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/shared/completion_wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,19 @@
 
 @_with_tracer_wrapper
 def completion_wrapper(tracer, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     # span needs to be opened and closed manually because the response is a generator
-    span = tracer.start_span(SPAN_NAME, kind=SpanKind.CLIENT)
+    span = tracer.start_span(
+        SPAN_NAME,
+        kind=SpanKind.CLIENT,
+        attributes={SpanAttributes.LLM_REQUEST_TYPE: LLM_REQUEST_TYPE.value},
+    )
 
     _handle_request(span, kwargs)
     response = wrapped(*args, **kwargs)
 
     if is_streaming_response(response):
         # span will be closed after the generator is done
         return _build_from_streaming_response(span, response)
@@ -53,25 +57,28 @@
 
 @_with_tracer_wrapper
 async def acompletion_wrapper(tracer, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     async with start_as_current_span_async(
-        tracer=tracer, name=SPAN_NAME, kind=SpanKind.CLIENT
+        tracer=tracer,
+        name=SPAN_NAME,
+        kind=SpanKind.CLIENT,
+        attributes={SpanAttributes.LLM_REQUEST_TYPE: LLM_REQUEST_TYPE.value},
     ) as span:
         _handle_request(span, kwargs)
         response = await wrapped(*args, **kwargs)
         _handle_response(response, span)
 
         return response
 
 
 def _handle_request(span, kwargs):
-    _set_request_attributes(span, LLM_REQUEST_TYPE, kwargs)
+    _set_request_attributes(span, kwargs)
     if should_send_prompts():
         _set_prompts(span, kwargs.get("prompt"))
         _set_functions_attributes(span, kwargs.get("functions"))
 
 
 def _handle_response(response, span):
     if is_openai_v1():
```

### Comparing `opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py` & `opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/shared/embeddings_wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,39 +28,46 @@
 
 
 @_with_tracer_wrapper
 def embeddings_wrapper(tracer, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
-    with tracer.start_as_current_span(name=SPAN_NAME, kind=SpanKind.CLIENT) as span:
+    with tracer.start_as_current_span(
+        name=SPAN_NAME,
+        kind=SpanKind.CLIENT,
+        attributes={SpanAttributes.LLM_REQUEST_TYPE: LLM_REQUEST_TYPE.value},
+    ) as span:
         _handle_request(span, kwargs)
         response = wrapped(*args, **kwargs)
         _handle_response(response, span)
 
         return response
 
 
 @_with_tracer_wrapper
 async def aembeddings_wrapper(tracer, wrapped, instance, args, kwargs):
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
 
     async with start_as_current_span_async(
-        tracer=tracer, name=SPAN_NAME, kind=SpanKind.CLIENT
+        tracer=tracer,
+        name=SPAN_NAME,
+        kind=SpanKind.CLIENT,
+        attributes={SpanAttributes.LLM_REQUEST_TYPE: LLM_REQUEST_TYPE.value},
     ) as span:
         _handle_request(span, kwargs)
         response = await wrapped(*args, **kwargs)
         _handle_response(response, span)
 
         return response
 
 
 def _handle_request(span, kwargs):
-    _set_request_attributes(span, LLM_REQUEST_TYPE, kwargs)
+    _set_request_attributes(span, kwargs)
     if should_send_prompts():
         _set_prompts(span, kwargs.get("input"))
 
 
 def _handle_response(response, span):
     if is_openai_v1():
         response_dict = model_as_dict(response)
```

### Comparing `opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/utils.py` & `opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/v0/__init__.py` & `opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_openai-0.9.3/opentelemetry/instrumentation/openai/v1/__init__.py` & `opentelemetry_instrumentation_openai-0.9.4/opentelemetry/instrumentation/openai/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_openai-0.9.3/pyproject.toml` & `opentelemetry_instrumentation_openai-0.9.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-openai"
-version = "0.9.3"
+version = "0.9.4"
 description = "OpenTelemetry OpenAI instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 license = "Apache-2.0"
```

### Comparing `opentelemetry_instrumentation_openai-0.9.3/PKG-INFO` & `opentelemetry_instrumentation_openai-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-openai
-Version: 0.9.3
+Version: 0.9.4
 Summary: OpenTelemetry OpenAI instrumentation
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opentelemetry-instrumentation-openai Version: 0.9.3
+Metadata-Version: 2.1 Name: opentelemetry-instrumentation-openai Version: 0.9.4
 Summary: OpenTelemetry OpenAI instrumentation License: Apache-2.0 Author: Gal
 Kleinman Author-email: gal@traceloop.com Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0) Requires-
```

