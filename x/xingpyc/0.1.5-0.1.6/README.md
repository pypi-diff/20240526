# Comparing `tmp/xingpyc-0.1.5.tar.gz` & `tmp/xingpyc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.1.5.tar", last modified: Sat May 25 15:03:38 2024, max compression
+gzip compressed data, was "xingpyc-0.1.6.tar", last modified: Sun May 26 06:07:18 2024, max compression
```

## Comparing `xingpyc-0.1.5.tar` & `xingpyc-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 15:03:38.525767 xingpyc-0.1.5/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 15:03:38.525478 xingpyc-0.1.5/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.5/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-25 15:03:35.000000 xingpyc-0.1.5/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 15:03:38.525821 xingpyc-0.1.5/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 15:03:38.523128 xingpyc-0.1.5/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 15:03:38.523804 xingpyc-0.1.5/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     7978 2024-05-25 15:03:31.000000 xingpyc-0.1.5/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.5/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 15:03:38.525225 xingpyc-0.1.5/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-25 15:03:38.000000 xingpyc-0.1.5/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-25 15:03:38.000000 xingpyc-0.1.5/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 15:03:38.000000 xingpyc-0.1.5/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 15:03:38.000000 xingpyc-0.1.5/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 15:03:38.000000 xingpyc-0.1.5/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 15:03:38.525021 xingpyc-0.1.5/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)      494 2024-05-25 15:03:30.000000 xingpyc-0.1.5/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.829259 xingpyc-0.1.6/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:07:18.829033 xingpyc-0.1.6/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.6/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      568 2024-05-26 06:07:07.000000 xingpyc-0.1.6/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:07:18.829298 xingpyc-0.1.6/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.827133 xingpyc-0.1.6/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.827670 xingpyc-0.1.6/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     8302 2024-05-26 05:21:58.000000 xingpyc-0.1.6/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.6/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.828828 xingpyc-0.1.6/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      586 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:07:18.000000 xingpyc-0.1.6/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:07:18.828678 xingpyc-0.1.6/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.6/tests/test1.py
```

### Comparing `xingpyc-0.1.5/PKG-INFO` & `xingpyc-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.5
+Version: 0.1.6
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.1.5/pyproject.toml` & `xingpyc-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.1.5/src/xingpyc/__init__.py` & `xingpyc-0.1.6/src/xingpyc/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,80 +7,56 @@
 from websockets.server import serve
 from websocket import WebSocket
 import time
 import sys
 import numpy as np
 from threading import Thread
 
-try:
-    progress = SharedMemory(name="progress", create=True, size=1*8)
-except FileExistsError:
-    progress = SharedMemory(name="progress", create=False, size=1*8)
-
-try:
-    curClient = SharedMemory(name="curClient", create=True, size=1*8)
-except FileExistsError:
-    curClient = SharedMemory(name="curClient", create=False, size=1*8)
-
-progressfloat = np.ndarray((1,), dtype=np.float64, buffer=progress.buf)
-curClientint = np.ndarray((1,), dtype=np.int64, buffer=curClient.buf)
-
-class ConsoleCapture:
-    def write(self, text):
-        # Capture the printed text
-        if text == '\n':
-            return
-        if text[1:5]=="XING" :
-            progressfloat[0]=float(text[15:])
-
-        sys.stdout= sys.__stdout__
-        print(text)
-        sys.stdout = self
-
-    def flush(self):
-        pass
     
 # Redirect sys.stdout to the custom stream
-capture_stream = ConsoleCapture()
-sys.stdout = capture_stream
 
 class XClient:
     def __init__(self,funcs,mode: str, ip=None, portOrInfo=None):
         '''
         init a ComClient with AI functions
         funcs: a list of AI functions
         '''
         self.cloudClient = None
 
 
         self.clients = {}
         self.blockbuffers = {}
-
+        
+        #tasks folder is for placing incoming commands
         if not os.path.exists("tasks"):
             os.mkdir("tasks")
         tasks = os.listdir("tasks")
         for task in tasks:
             os.remove(f"tasks/{task}")
 
+        #results folder is for placing results from various AI functions, no matter binded to XClient or not
         if not os.path.exists("results"):
             os.mkdir("results")
         results = os.listdir("results")
         for result in results:
             os.remove(f"results/{result}")
 
+        #for functions registered with XClient, create a process for each processor that will automatically listen according to there function name
+        #e.g. if there is a function named "i2i" in the list, a process will be created to listen for "i2i" header tasks in the tasks folder
         for func in funcs:
             Process(target=add_listener, args=(func,)).start()
         #sending
         asyncio.get_event_loop().create_task(self.global_send())
 
         #listening
         if(mode == "server"):
             print("\033[93m Server started on "+ip+":"+str(portOrInfo)+" \033[0m")
             asyncio.get_event_loop().run_until_complete(serve(self.asServer_onRecv, ip, portOrInfo))
 
+        #for client mode, connect to the cloud server, use sync websocket, async one is not working well for now
         elif(mode == "client"):
             print("\033[93m Client started \033[0m")
             self.cloudClient = WebSocket()
             self.cloudClient.connect(ip)
             self.cloudClient.send_bytes(("login     "+"0000000000"+portOrInfo).encode("utf-8"))
             login_res = self.cloudClient.recv()
             if login_res == b"login success":
@@ -149,14 +125,15 @@
             if client_id in self.blockbuffers:
                 # if there is a block buffer, concat it
                 self.blockbuffers[client_id].append(content)
                 content = b"".join(self.blockbuffers[client_id])
 
                 #finally write the file to tasks folder for processing from other processes
                 with open(f"tasks/{client_id}.{task_id.decode()}.{header}", "wb") as f:
+                    print("place task: "+f"{client_id}.{task_id.decode()}.{header}")
                     f.write(content)
                 del self.blockbuffers[client_id] # clean buffer
 
         except Exception as e:
             print(f"Error in websocket communication: {e}")
             return
 
@@ -177,15 +154,21 @@
                         if isinstance(task_id, str):
                             task_id = task_id.encode("utf-8")
                         if isinstance(header, str):
                             header = header.encode("utf-8")
                         if isinstance(content, str):
                             content = content.encode("utf-8")
                         if client_id == -1:
+                            print("start sending to cloud")
+                            while len(content) > 10000:
+                                self.cloudClient.send_bytes(b"block00000" + task_id + content[0:10000])
+                                content = content[10000:]
+
                             self.cloudClient.send_bytes(header + task_id + content)
+                            print("sent to cloud")
                         else:
                             await self.asServer_send(client_id, header, task_id, content)
 
                         break # only send one result at a time
                     except Exception as e:
                         print(f"Error in sending message to websocket: {e}")
             else:
@@ -204,26 +187,36 @@
         await asyncio.sleep(0.01)
 
 
 
 def add_listener(callback, interval=0.1):
     while True:
         taskfiles = os.listdir("tasks")
+        time.sleep(interval)
         found = False
         try:
             for file in taskfiles:
                 client_id, task_id, header = file.split(".")
                 if header == callback.__name__:
                     found = True
                     res=callback("tasks/"+file)
-                    os.remove("tasks/"+file)
                     assert type(res) == bytes, "Return type must be bytes"
                     if res is not None:
                         with open("results/"+file,"wb") as f:
                             f.write(res)
+                    os.remove("tasks/"+file)
         except Exception as e:
             print(f"Error in interpreting task of {callback.__name__}: {e}")
 
-        if found is None:
-            time.sleep(interval)
-            print(callback.__name__)
-            continue
+
+
+def i2i(file):
+    print("i2i task received, file:",file)
+    return b"i2i"
+
+def config(file):
+    print("config task received, file:",file)
+    return b"hello from com test"
+
+if __name__ == "__main__":
+    
+    XClient([i2i,config],"client", "wss://xing.art/com/","testuser.testuser")
```

### Comparing `xingpyc-0.1.5/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.1.6/src/xingpyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.5
+Version: 0.1.6
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

