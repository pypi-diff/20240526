# Comparing `tmp/z2m_log_parser-0.0.6.tar.gz` & `tmp/z2m_log_parser-0.0.7.tar.gz`

## Comparing `z2m_log_parser-0.0.6.tar` & `z2m_log_parser-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/src/z2m_log_parser/__init__.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/src/z2m_log_parser/z2m_log_parser.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.7/src/z2m_log_parser/__init__.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.7/src/z2m_log_parser/z2m_log_parser.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.7/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.7/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.7/PKG-INFO
```

### Comparing `z2m_log_parser-0.0.6/.github/workflows/python-publish.yml` & `z2m_log_parser-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.0.6/src/z2m_log_parser/z2m_log_parser.py` & `z2m_log_parser-0.0.7/src/z2m_log_parser/z2m_log_parser.py`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.0.6/LICENSE` & `z2m_log_parser-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.0.6/pyproject.toml` & `z2m_log_parser-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "z2m_log_parser"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Stoyan Dimitrov", email="stdimitrov@gmail.com" },
 ]
 description = "Parser for Zigbee2Mqtt logs to python object for further processing"
 readme = "README.md"
-requires-python = ">=3.12.2"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `z2m_log_parser-0.0.6/PKG-INFO` & `z2m_log_parser-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.3
 Name: z2m_log_parser
-Version: 0.0.6
+Version: 0.0.7
 Summary: Parser for Zigbee2Mqtt logs to python object for further processing
 Project-URL: Homepage, https://github.com/st0yanDimitrov/z2m_log_parser
 Project-URL: Issues, https://github.com/st0yanDimitrov/z2m_log_parser/issues
 Author-email: Stoyan Dimitrov <stdimitrov@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.12.2
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Zigbee2mqtt log parser
 
 A simple log parser for zigbee2mqtt logs.
```

