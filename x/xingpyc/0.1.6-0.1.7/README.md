# Comparing `tmp/xingpyc-0.1.6.tar.gz` & `tmp/xingpyc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.1.6.tar", last modified: Sun May 26 06:07:18 2024, max compression
+gzip compressed data, was "xingpyc-0.1.7.tar", last modified: Sun May 26 06:12:55 2024, max compression
```

## Comparing `xingpyc-0.1.6.tar` & `xingpyc-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.829259 xingpyc-0.1.6/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:07:18.829033 xingpyc-0.1.6/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.6/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-26 06:07:07.000000 xingpyc-0.1.6/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:07:18.829298 xingpyc-0.1.6/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.827133 xingpyc-0.1.6/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.827670 xingpyc-0.1.6/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     8302 2024-05-26 05:21:58.000000 xingpyc-0.1.6/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.6/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.828828 xingpyc-0.1.6/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.828678 xingpyc-0.1.6/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.6/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.179544 xingpyc-0.1.7/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:12:55.179333 xingpyc-0.1.7/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.7/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-26 06:12:49.000000 xingpyc-0.1.7/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:12:55.179585 xingpyc-0.1.7/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.177202 xingpyc-0.1.7/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.178120 xingpyc-0.1.7/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     8331 2024-05-26 06:12:42.000000 xingpyc-0.1.7/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.7/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.179110 xingpyc-0.1.7/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.178950 xingpyc-0.1.7/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.7/tests/test1.py
```

### Comparing `xingpyc-0.1.6/PKG-INFO` & `xingpyc-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.6
+Version: 0.1.7
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.1.6/pyproject.toml` & `xingpyc-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.1.6/src/xingpyc/__init__.py` & `xingpyc-0.1.7/src/xingpyc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                     f.write(content)
                 del self.blockbuffers[client_id] # clean buffer
 
         except Exception as e:
             print(f"Error in websocket communication: {e}")
             return
 
-    async def global_send(self):
+    async def global_send(self, blocksize=10000):
         print("start result->sender loop")
         while True:
             if len(os.listdir("results")) > 0:
                 for file in os.listdir("results"):
                     try:
                         with open(f"results/{file}", "rb") as f:
                             result_data = f.read()
@@ -155,17 +155,17 @@
                             task_id = task_id.encode("utf-8")
                         if isinstance(header, str):
                             header = header.encode("utf-8")
                         if isinstance(content, str):
                             content = content.encode("utf-8")
                         if client_id == -1:
                             print("start sending to cloud")
-                            while len(content) > 10000:
-                                self.cloudClient.send_bytes(b"block00000" + task_id + content[0:10000])
-                                content = content[10000:]
+                            while len(content) > blocksize:
+                                self.cloudClient.send_bytes(b"block     " + task_id + content[0:blocksize])
+                                content = content[blocksize:]
 
                             self.cloudClient.send_bytes(header + task_id + content)
                             print("sent to cloud")
                         else:
                             await self.asServer_send(client_id, header, task_id, content)
 
                         break # only send one result at a time
```

### Comparing `xingpyc-0.1.6/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.1.7/src/xingpyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.6
+Version: 0.1.7
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

