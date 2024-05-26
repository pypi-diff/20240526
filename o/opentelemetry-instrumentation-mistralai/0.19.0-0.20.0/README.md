# Comparing `tmp/opentelemetry_instrumentation_mistralai-0.19.0.tar.gz` & `tmp/opentelemetry_instrumentation_mistralai-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_mistralai-0.19.0.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_mistralai-0.20.0.tar", max compression
```

## Comparing `opentelemetry_instrumentation_mistralai-0.19.0.tar` & `opentelemetry_instrumentation_mistralai-0.20.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1177 2024-05-26 05:28:00.238083 opentelemetry_instrumentation_mistralai-0.19.0/README.md
--rw-r--r--   0        0        0    11717 2024-05-26 05:28:00.238376 opentelemetry_instrumentation_mistralai-0.19.0/opentelemetry/instrumentation/mistralai/__init__.py
--rw-r--r--   0        0        0       42 2024-05-26 05:28:00.238734 opentelemetry_instrumentation_mistralai-0.19.0/opentelemetry/instrumentation/mistralai/config.py
--rw-r--r--   0        0        0      702 2024-05-26 05:28:00.239080 opentelemetry_instrumentation_mistralai-0.19.0/opentelemetry/instrumentation/mistralai/utils.py
--rw-r--r--   0        0        0       23 2024-05-26 05:28:00.239343 opentelemetry_instrumentation_mistralai-0.19.0/opentelemetry/instrumentation/mistralai/version.py
--rw-r--r--   0        0        0     1430 2024-05-26 05:28:00.241256 opentelemetry_instrumentation_mistralai-0.19.0/pyproject.toml
--rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_mistralai-0.19.0/PKG-INFO
+-rw-r--r--   0        0        0     1177 2024-05-26 09:11:35.103710 opentelemetry_instrumentation_mistralai-0.20.0/README.md
+-rw-r--r--   0        0        0    11717 2024-05-26 09:11:35.103710 opentelemetry_instrumentation_mistralai-0.20.0/opentelemetry/instrumentation/mistralai/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-26 09:11:35.103710 opentelemetry_instrumentation_mistralai-0.20.0/opentelemetry/instrumentation/mistralai/config.py
+-rw-r--r--   0        0        0      702 2024-05-26 09:11:35.103710 opentelemetry_instrumentation_mistralai-0.20.0/opentelemetry/instrumentation/mistralai/utils.py
+-rw-r--r--   0        0        0       23 2024-05-26 09:11:35.103710 opentelemetry_instrumentation_mistralai-0.20.0/opentelemetry/instrumentation/mistralai/version.py
+-rw-r--r--   0        0        0     1430 2024-05-26 09:11:57.159669 opentelemetry_instrumentation_mistralai-0.20.0/pyproject.toml
+-rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_mistralai-0.20.0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_mistralai-0.19.0/README.md` & `opentelemetry_instrumentation_mistralai-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_mistralai-0.19.0/opentelemetry/instrumentation/mistralai/__init__.py` & `opentelemetry_instrumentation_mistralai-0.20.0/opentelemetry/instrumentation/mistralai/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_mistralai-0.19.0/opentelemetry/instrumentation/mistralai/utils.py` & `opentelemetry_instrumentation_mistralai-0.20.0/opentelemetry/instrumentation/mistralai/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_mistralai-0.19.0/pyproject.toml` & `opentelemetry_instrumentation_mistralai-0.20.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = ['if TYPE_CHECKING:']
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-mistralai"
-version = "0.19.0"
+version = "0.20.0"
 description = "OpenTelemetry Mistral AI instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-mistralai"
 license = "Apache-2.0"
```

### Comparing `opentelemetry_instrumentation_mistralai-0.19.0/PKG-INFO` & `opentelemetry_instrumentation_mistralai-0.20.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-mistralai
-Version: 0.19.0
+Version: 0.20.0
 Summary: OpenTelemetry Mistral AI instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-mistralai
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-mistralai Version:
-0.19.0 Summary: OpenTelemetry Mistral AI instrumentation Home-page: https://
+0.20.0 Summary: OpenTelemetry Mistral AI instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-mistralai License: Apache-2.0 Author: Gal Kleinman Author-
 email: gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

