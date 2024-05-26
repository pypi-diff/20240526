# Comparing `tmp/xingpyc-0.1.9.tar.gz` & `tmp/xingpyc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.1.9.tar", last modified: Sun May 26 06:47:02 2024, max compression
+gzip compressed data, was "xingpyc-0.2.0.tar", last modified: Sun May 26 06:59:51 2024, max compression
```

## Comparing `xingpyc-0.1.9.tar` & `xingpyc-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:47:02.471614 xingpyc-0.1.9/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:47:02.471409 xingpyc-0.1.9/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.9/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-26 06:46:59.000000 xingpyc-0.1.9/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:47:02.471654 xingpyc-0.1.9/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:47:02.469345 xingpyc-0.1.9/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:47:02.470088 xingpyc-0.1.9/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     8625 2024-05-26 06:45:48.000000 xingpyc-0.1.9/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.9/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:47:02.471205 xingpyc-0.1.9/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:47:02.000000 xingpyc-0.1.9/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:47:02.000000 xingpyc-0.1.9/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:47:02.000000 xingpyc-0.1.9/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:47:02.000000 xingpyc-0.1.9/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:47:02.000000 xingpyc-0.1.9/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:47:02.471051 xingpyc-0.1.9/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.9/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.289636 xingpyc-0.2.0/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:59:51.289446 xingpyc-0.2.0/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.2.0/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-26 06:59:47.000000 xingpyc-0.2.0/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:59:51.289674 xingpyc-0.2.0/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.287797 xingpyc-0.2.0/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.288354 xingpyc-0.2.0/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     8765 2024-05-26 06:59:27.000000 xingpyc-0.2.0/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.2.0/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.289247 xingpyc-0.2.0/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:59:51.000000 xingpyc-0.2.0/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:59:51.289081 xingpyc-0.2.0/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.2.0/tests/test1.py
```

### Comparing `xingpyc-0.1.9/PKG-INFO` & `xingpyc-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.9
+Version: 0.2.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.1.9/pyproject.toml` & `xingpyc-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.1.9/src/xingpyc/__init__.py` & `xingpyc-0.2.0/src/xingpyc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                     f.write(content)
                 del self.blockbuffers[client_id] # clean buffer
 
         except Exception as e:
             print(f"Error in websocket communication: {e}")
             return
 
-    async def global_send(self, blocksize=10000):
+    async def global_send(self, blocksize=30000):
         print("start result->sender loop")
         while True:
             if len(os.listdir("results")) > 0:
                 for file in os.listdir("results"):
                     try:
                         with open(f"results/{file}", "rb") as f:
                             result_data = f.read()
@@ -159,15 +159,16 @@
                         if isinstance(content, str):
                             content = content.encode("utf-8")
                         if client_id == -1:
                             print("start sending to cloud")
                             count = 0
                             totalblocks = len(content) // blocksize
                             while len(content) > blocksize:
-                                self.cloudClient.send_bytes(b"block     " + task_id + content[0:blocksize])
+                                Thread(target=self.cloudClient.send_bytes, args=(b"block     " + task_id + content[0:blocksize],)).start()
+                                #self.cloudClient.send_bytes(b"block     " + task_id + content[0:blocksize])
                                 content = content[blocksize:]
                                 print(f"sent block {count}/{totalblocks}")
                                 count += 1
 
                             self.cloudClient.send_bytes(header + task_id + content)
                             print("sent to cloud")
                         else:
```

### Comparing `xingpyc-0.1.9/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.2.0/src/xingpyc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.9
+Version: 0.2.0
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

