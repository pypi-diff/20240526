# Comparing `tmp/clank_so_openinference_instrumentation_dspy-0.1.6.tar.gz` & `tmp/clank_so_openinference_instrumentation_dspy-0.1.9.tar.gz`

## Comparing `clank_so_openinference_instrumentation_dspy-0.1.6.tar` & `clank_so_openinference_instrumentation_dspy-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    23818 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/version.py
--rw-r--r--   0        0        0    15850 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/tests/openinference/instrumentation/dspy/test_instrumentor.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/.gitignore
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/LICENSE
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/README.md
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    24687 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/version.py
+-rw-r--r--   0        0        0    28449 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/tests/openinference/instrumentation/dspy/test_instrumentor.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/.gitignore
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/README.md
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 clank_so_openinference_instrumentation_dspy-0.1.9/PKG-INFO
```

### Comparing `clank_so_openinference_instrumentation_dspy-0.1.6/src/openinference/instrumentation/dspy/__init__.py` & `clank_so_openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     List,
     Mapping,
     Optional,
     Tuple,
 )
 
 import opentelemetry.context as context_api
+from openinference.instrumentation import get_attributes_from_context, safe_json_dumps
 from openinference.instrumentation.dspy.package import _instruments
 from openinference.instrumentation.dspy.version import __version__
 from openinference.semconv.trace import (
     DocumentAttributes,
     OpenInferenceMimeTypeValues,
     OpenInferenceSpanKindValues,
     SpanAttributes,
@@ -214,21 +215,22 @@
         with self._tracer.start_as_current_span(
             span_name,
             attributes=dict(
                 _flatten(
                     {
                         OPENINFERENCE_SPAN_KIND: LLM.value,
                         LLM_MODEL_NAME: instance.kwargs.get("model"),
-                        LLM_INVOCATION_PARAMETERS: json.dumps(invocation_parameters),
+                        LLM_INVOCATION_PARAMETERS: safe_json_dumps(invocation_parameters),
                         INPUT_VALUE: str(prompt),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.TEXT.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 response = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             # TODO: parse usage. Need to decide if this
@@ -300,25 +302,26 @@
                             **kwargs,
                         ),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 prediction = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
                 dict(
                     _flatten(
                         {
-                            OUTPUT_VALUE: json.dumps(
+                            OUTPUT_VALUE: safe_json_dumps(
                                 self._prediction_to_output_dict(prediction, signature)
                             ),
                             OUTPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                         }
                     )
                 )
             )
@@ -369,25 +372,26 @@
                             else {}
                         ),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 prediction = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
                 dict(
                     _flatten(
                         {
-                            OUTPUT_VALUE: json.dumps(prediction, cls=DSPyJSONEncoder),
+                            OUTPUT_VALUE: safe_json_dumps(prediction, cls=DSPyJSONEncoder),
                             OUTPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                         }
                     )
                 )
             )
             span.set_status(trace_api.StatusCode.OK)
         return prediction
@@ -420,14 +424,15 @@
                         OPENINFERENCE_SPAN_KIND: RETRIEVER.value,
                         INPUT_VALUE: _get_input_value(wrapped, *args, **kwargs),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 prediction = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
@@ -472,14 +477,15 @@
                         OPENINFERENCE_SPAN_KIND: RETRIEVER.value,
                         INPUT_VALUE: (_get_input_value(wrapped, *args, **kwargs)),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                     }
                 )
             ),
         ) as span:
+            span.set_attributes(dict(get_attributes_from_context()))
             try:
                 retrieved_documents = wrapped(*args, **kwargs)
             except Exception as exception:
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
@@ -525,14 +531,28 @@
                 return {
                     "fields": [self.default(field) for field in o.fields],
                     "instructions": o.instructions,
                 }
             return repr(o)
 
 
+class SafeJSONEncoder(json.JSONEncoder):
+    """
+    Safely encodes non-JSON-serializable objects.
+    """
+
+    def default(self, o: Any) -> Any:
+        try:
+            return super().default(o)
+        except TypeError:
+            if hasattr(o, "dict") and callable(o.dict):  # pydantic v1 models, e.g., from Cohere
+                return o.dict()
+            return repr(o)
+
+
 def _get_input_value(method: Callable[..., Any], *args: Any, **kwargs: Any) -> str:
     """
     Parses a method call's inputs into a JSON string. Ensures a consistent
     output regardless of whether the those inputs are passed as positional or
     keyword arguments.
     """
 
@@ -547,15 +567,15 @@
             [None]  # the value bound to the method's self argument is discarded below, so pass None
             if signature_contains_self_parameter
             else []  # no self parameter, so no need to pass a value
         ),
         *args,
         **kwargs,
     )
-    return json.dumps(
+    return safe_json_dumps(
         {
             **{
                 argument_name: argument_value
                 for argument_name, argument_value in bound_arguments.arguments.items()
                 if argument_name not in ["self", "kwargs"]
             },
             **bound_arguments.arguments.get("kwargs", {}),
@@ -609,20 +629,20 @@
 
 
 def _jsonify_output(response: Any) -> str:
     """
     Converts output to JSON string.
     """
     if isinstance(response, BaseModel):
-        return json.dumps(response.model_dump())
+        return safe_json_dumps(response.model_dump())
 
     if _is_google_response(response):
-        return json.dumps(_parse_google_response(response))
+        return safe_json_dumps(_parse_google_response(response))
 
-    return json.dumps(response)
+    return safe_json_dumps(response, cls=SafeJSONEncoder)
 
 
 def _is_google_response(response: Any) -> TypeGuard["GenerateContentResponseType"]:
     """
     Checks whether a candidate response is an instance of
     GenerateContentResponse returned by the Google generative AI SDK.
     """
```

### Comparing `clank_so_openinference_instrumentation_dspy-0.1.6/LICENSE` & `clank_so_openinference_instrumentation_dspy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clank_so_openinference_instrumentation_dspy-0.1.6/README.md` & `clank_so_openinference_instrumentation_dspy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `clank_so_openinference_instrumentation_dspy-0.1.6/pyproject.toml` & `clank_so_openinference_instrumentation_dspy-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "opentelemetry-api",
   "opentelemetry-instrumentation",
   "opentelemetry-semantic-conventions",
+  "openinference-instrumentation>=0.1.7",
   "openinference-semantic-conventions",
   "wrapt",
   "typing-extensions",
 ]
 
 [project.optional-dependencies]
 instruments = [
@@ -56,22 +57,36 @@
   "/tests",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/openinference"]
 
 [tool.mypy]
-plugins = []
-disallow_untyped_calls = true
-disallow_untyped_defs = true
-disallow_incomplete_defs  = true
 strict = true
+explicit_package_bases = true
 exclude = [
-  "dist/",
+  "examples",
+  "dist",
+  "sdist",
+]
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = [
+  "wrapt",
+  "dspy.*",
+  "dsp.*",
 ]
 
 [tool.ruff]
-exclude = [".git", "__pycache__", "*_pb2.py*", "*.pyi"]
-ignore-init-module-imports = true
 line-length = 100
-select = ["E", "F", "W", "I"]
 target-version = "py38"
+
+[tool.ruff.lint.per-file-ignores]
+"*.ipynb" = ["E402", "E501"]
+
+[tool.ruff.lint]
+ignore-init-module-imports = true
+select = ["E", "F", "W", "I"]
+
+[tool.ruff.lint.isort]
+force-single-line = false
```

### Comparing `clank_so_openinference_instrumentation_dspy-0.1.6/PKG-INFO` & `clank_so_openinference_instrumentation_dspy-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: clank-so-openinference-instrumentation-dspy
-Version: 0.1.6
+Version: 0.1.9
 Summary: OpenInference DSPy Instrumentation (clank.so fork)
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-dspy
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.9
+Requires-Dist: openinference-instrumentation>=0.1.7
 Requires-Dist: openinference-semantic-conventions
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: typing-extensions
 Requires-Dist: wrapt
 Provides-Extra: instruments
```

