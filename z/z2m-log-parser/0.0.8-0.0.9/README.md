# Comparing `tmp/z2m_log_parser-0.0.8.tar.gz` & `tmp/z2m_log_parser-0.0.9.tar.gz`

## Comparing `z2m_log_parser-0.0.8.tar` & `z2m_log_parser-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.8/src/z2m_log_parser/__init__.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.8/src/z2m_log_parser/z2m_log_parser.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.8/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.8/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/src/z2m_log_parser/__init__.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/src/z2m_log_parser/z2m_log_parser.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.9/PKG-INFO
```

### Comparing `z2m_log_parser-0.0.8/.github/workflows/python-publish.yml` & `z2m_log_parser-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.0.8/src/z2m_log_parser/z2m_log_parser.py` & `z2m_log_parser-0.0.9/src/z2m_log_parser/z2m_log_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,16 +47,15 @@
                 parsed_line.data.is_mqtt_publish = True
                 parsed_line.data.mqtt_message.topic = None
                 parsed_line.data.mqtt_message.payload = None
             parsed_lines.append(parsed_line)
     return parsed_lines
 def parse_latest_logs(path: str):
         events = parse_logs(path)
-        execution_path = os.path.dirname(os.path.realpath(__file__))
-        pointer_file_name = execution_path + "/eventPointer.txt"
+        pointer_file_name =  "/eventPointer.txt"
         last_event = datetime.strftime(events[(len(events))-1].date, '%Y-%m-%d %H:%M:%S')
         if not os.path.exists(pointer_file_name):
             f = open(pointer_file_name, "w")
             f.write(last_event)
             f.close()
         else:
             f = open(pointer_file_name, "r+")
```

### Comparing `z2m_log_parser-0.0.8/LICENSE` & `z2m_log_parser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.0.8/pyproject.toml` & `z2m_log_parser-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "z2m_log_parser"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Stoyan Dimitrov", email="stdimitrov@gmail.com" },
 ]
 description = "Parser for Zigbee2Mqtt logs to python object for further processing"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `z2m_log_parser-0.0.8/PKG-INFO` & `z2m_log_parser-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: z2m_log_parser
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parser for Zigbee2Mqtt logs to python object for further processing
 Project-URL: Homepage, https://github.com/st0yanDimitrov/z2m_log_parser
 Project-URL: Issues, https://github.com/st0yanDimitrov/z2m_log_parser/issues
 Author-email: Stoyan Dimitrov <stdimitrov@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

