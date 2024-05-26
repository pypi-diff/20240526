# Comparing `tmp/z2m_log_parser-0.0.5.tar.gz` & `tmp/z2m_log_parser-0.0.6.tar.gz`

## Comparing `z2m_log_parser-0.0.5.tar` & `z2m_log_parser-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.5/src/z2m_log_parser/__init__.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.5/src/z2m_log_parser/z2m_log_parser.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.5/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.5/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/src/z2m_log_parser/__init__.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/src/z2m_log_parser/z2m_log_parser.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 z2m_log_parser-0.0.6/PKG-INFO
```

### Comparing `z2m_log_parser-0.0.5/.github/workflows/python-publish.yml` & `z2m_log_parser-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.0.5/src/z2m_log_parser/z2m_log_parser.py` & `z2m_log_parser-0.0.6/src/z2m_log_parser/z2m_log_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,65 +15,58 @@
 
 class LogEntry(object):
     def __init__(self):
         self.type = str
         self.date = datetime
         self.data = LogEntryData()
 
-class Z2mLogParser:
-    '''
-    Used to parse Zigbee2mqtt log entries from log.txt file
-    '''
-
-    def parse_logs(self, path):
-        parsed_lines = []
-        with open(path) as log:
-            for line in log:
-                parsed_line= LogEntry()
-                parsed_line.data.is_mqtt_publish
+def parse_logs(path):
+    parsed_lines = []
+    with open(path) as log:
+        for line in log:
+            parsed_line= LogEntry()
+            parsed_line.data.is_mqtt_publish
+            try:
+                parsed_line.type = line[0:4]
+                parsed_line.date = datetime.strptime(line[6:25], '%Y-%m-%d %H:%M:%S')
+            except:
+                try:
+                    parsed_lines[-1].data.message = parsed_lines[-1].data.message + line
+                except Exception:
+                    pass
+                continue
+            parsed_line.data.message = line[27:]
+            if parsed_line.data.message[0:12] == "MQTT publish":
+                parsed_line.data.is_mqtt_publish = True
+                parsed_line.data.mqtt_message.topic = line.split("topic")[1].rsplit(", payload")[0].strip().strip("'")
+                parsed_line.data.mqtt_message.payload = line.split("payload")[1].strip().strip("'")
                 try:
-                    parsed_line.type = line[0:4]
-                    parsed_line.date = datetime.strptime(line[6:25], '%Y-%m-%d %H:%M:%S')
+                    parsed_line.data.mqtt_message.payload = json.loads("{\"payload\":" + "\""  + line.split("payload")[1].strip().strip("'") + "\"" + "}")
                 except:
-                    try:
-                        parsed_lines[-1].data.message = parsed_lines[-1].data.message + line
-                    except Exception:
-                        pass
-                    continue
-
-                parsed_line.data.message = line[27:]
-                if parsed_line.data.message[0:12] == "MQTT publish":
-                    parsed_line.data.is_mqtt_publish = True
-                    parsed_line.data.mqtt_message.topic = line.split("topic")[1].rsplit(", payload")[0].strip().strip("'")
-                    parsed_line.data.mqtt_message.payload = line.split("payload")[1].strip().strip("'")
-                    try:
-                        parsed_line.data.mqtt_message.payload = json.loads("{\"payload\":" + "\""  + line.split("payload")[1].strip().strip("'") + "\"" + "}")
-                    except:
-                        parsed_line.data.mqtt_message.payload = json.loads("{\"payload\":" + "\"Couldn't convert to JSON\"" + "}")
-                else:
-                    parsed_line.data.is_mqtt_publish = True
-                    parsed_line.data.mqtt_message.topic = None
-                    parsed_line.data.mqtt_message.payload = None
-                parsed_lines.append(parsed_line)
-        return parsed_lines
-
-    def parse_latest_logs(self, path: str):
-            events = self.parse_logs(path)
-            pinter_path = "./eventPointer.txt"
-            last_event = datetime.strftime(events[(len(events))-1].date, '%Y-%m-%d %H:%M:%S')
-            if not os.path.exists(pinter_path):
-                f = open(pinter_path, "w")
-                f.write(last_event)
-                f.close()
+                    parsed_line.data.mqtt_message.payload = json.loads("{\"payload\":" + "\"Couldn't convert to JSON\"" + "}")
             else:
-                f = open(pinter_path, "r+")
-                date_st = f.read()
-                date_dt = datetime.strptime(date_st, '%Y-%m-%d %H:%M:%S')
-                if date_st and date_dt <= events[(len(events))-1].date:
-                    events = [x for x in events if x.date > date_dt]
-                if events:
-                    f.seek(0)
-                    f.truncate()
-                    f.write(last_event)
-            if any(events):
-                return events
-            return None
+                parsed_line.data.is_mqtt_publish = True
+                parsed_line.data.mqtt_message.topic = None
+                parsed_line.data.mqtt_message.payload = None
+            parsed_lines.append(parsed_line)
+    return parsed_lines
+def parse_latest_logs(path: str):
+        events = parse_logs(path)
+        pinter_path = "./eventPointer.txt"
+        last_event = datetime.strftime(events[(len(events))-1].date, '%Y-%m-%d %H:%M:%S')
+        if not os.path.exists(pinter_path):
+            f = open(pinter_path, "w")
+            f.write(last_event)
+            f.close()
+        else:
+            f = open(pinter_path, "r+")
+            date_st = f.read()
+            date_dt = datetime.strptime(date_st, '%Y-%m-%d %H:%M:%S')
+            if date_st and date_dt <= events[(len(events))-1].date:
+                events = [x for x in events if x.date > date_dt]
+            if events:
+                f.seek(0)
+                f.truncate()
+                f.write(last_event)
+        if any(events):
+            return events
+        return None
```

### Comparing `z2m_log_parser-0.0.5/LICENSE` & `z2m_log_parser-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `z2m_log_parser-0.0.5/pyproject.toml` & `z2m_log_parser-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "z2m_log_parser"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Stoyan Dimitrov", email="stdimitrov@gmail.com" },
 ]
 description = "Parser for Zigbee2Mqtt logs to python object for further processing"
 readme = "README.md"
 requires-python = ">=3.12.2"
 classifiers = [
```

### Comparing `z2m_log_parser-0.0.5/PKG-INFO` & `z2m_log_parser-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: z2m_log_parser
-Version: 0.0.5
+Version: 0.0.6
 Summary: Parser for Zigbee2Mqtt logs to python object for further processing
 Project-URL: Homepage, https://github.com/st0yanDimitrov/z2m_log_parser
 Project-URL: Issues, https://github.com/st0yanDimitrov/z2m_log_parser/issues
 Author-email: Stoyan Dimitrov <stdimitrov@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

