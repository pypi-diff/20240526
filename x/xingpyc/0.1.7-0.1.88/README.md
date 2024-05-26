# Comparing `tmp/xingpyc-0.1.7.tar.gz` & `tmp/xingpyc-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.1.7.tar", last modified: Sun May 26 06:12:55 2024, max compression
+gzip compressed data, was "xingpyc-0.1.88.tar", last modified: Sun May 26 06:21:12 2024, max compression
```

## Comparing `xingpyc-0.1.7.tar` & `xingpyc-0.1.88.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.179544 xingpyc-0.1.7/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:12:55.179333 xingpyc-0.1.7/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.7/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-26 06:12:49.000000 xingpyc-0.1.7/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:12:55.179585 xingpyc-0.1.7/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.177202 xingpyc-0.1.7/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.178120 xingpyc-0.1.7/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     8331 2024-05-26 06:12:42.000000 xingpyc-0.1.7/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.7/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.179110 xingpyc-0.1.7/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:12:55.000000 xingpyc-0.1.7/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:12:55.178950 xingpyc-0.1.7/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.7/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.484682 xingpyc-0.1.88/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      587 2024-05-26 06:21:12.484473 xingpyc-0.1.88/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.88/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      569 2024-05-26 06:21:09.000000 xingpyc-0.1.88/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:21:12.484723 xingpyc-0.1.88/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.482471 xingpyc-0.1.88/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.483132 xingpyc-0.1.88/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     8331 2024-05-26 06:18:43.000000 xingpyc-0.1.88/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.88/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.484240 xingpyc-0.1.88/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      587 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.484051 xingpyc-0.1.88/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.88/tests/test1.py
```

### Comparing `xingpyc-0.1.7/PKG-INFO` & `xingpyc-0.1.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.7
+Version: 0.1.88
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.1.7/pyproject.toml` & `xingpyc-0.1.88/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.1.7"
+version = "0.1.88"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.1.7/src/xingpyc/__init__.py` & `xingpyc-0.1.88/src/xingpyc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                         with open(f"results/{file}", "rb") as f:
                             result_data = f.read()
                         os.remove(f"results/{file}")
                         content = result_data
                         client_id, task_id, header = file.split(".")
                         client_id = int(client_id)
                 
-                        header = (header + "0" * (10 - len(header))).encode("utf-8")
+                        header = (header + " " * (10 - len(header))).encode("utf-8")
                         if isinstance(task_id, str):
                             task_id = task_id.encode("utf-8")
                         if isinstance(header, str):
                             header = header.encode("utf-8")
                         if isinstance(content, str):
                             content = content.encode("utf-8")
                         if client_id == -1:
@@ -174,15 +174,15 @@
             else:
                 await asyncio.sleep(0.1)
 
     async def asServer_send(self, client_id, header, task_id, content):
         websocket = self.clients.get(client_id)
         while len(content) > 0:
             if len(content) > 100000:
-                await websocket.send(b"block00000" + task_id + content[0:100000])
+                await websocket.send(b"block     " + task_id + content[0:100000])
                 content = content[100000:]
             else:
                 await websocket.send(header + task_id + content)
                 content = b""
             await asyncio.sleep(0.01)
         await asyncio.sleep(0.01)
```

### Comparing `xingpyc-0.1.7/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.1.88/src/xingpyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.7
+Version: 0.1.88
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

