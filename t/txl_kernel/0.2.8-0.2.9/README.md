# Comparing `tmp/txl_kernel-0.2.8.tar.gz` & `tmp/txl_kernel-0.2.9.tar.gz`

## Comparing `txl_kernel-0.2.8.tar` & `txl_kernel-0.2.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 txl_kernel-0.2.8/txl_kernel/__init__.py
--rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 txl_kernel-0.2.8/txl_kernel/driver.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 txl_kernel-0.2.8/txl_kernel/driver.py.keep
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 txl_kernel-0.2.8/txl_kernel/message.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 txl_kernel-0.2.8/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 txl_kernel-0.2.8/LICENSE.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 txl_kernel-0.2.8/README.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 txl_kernel-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 txl_kernel-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 txl_kernel-0.2.9/txl_kernel/__init__.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 txl_kernel-0.2.9/txl_kernel/driver.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 txl_kernel-0.2.9/txl_kernel/driver.py.keep
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 txl_kernel-0.2.9/txl_kernel/message.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 txl_kernel-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 txl_kernel-0.2.9/LICENSE.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 txl_kernel-0.2.9/README.md
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 txl_kernel-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 txl_kernel-0.2.9/PKG-INFO
```

### Comparing `txl_kernel-0.2.8/txl_kernel/driver.py` & `txl_kernel-0.2.9/txl_kernel/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import time
 from typing import Dict
 
+from asphalt.core import Event, Signal
 from pycrdt import Array, Map
 
 from .message import create_message
 
 
 def deadline_to_timeout(deadline: float) -> float:
     return max(0, deadline - time.monotonic())
@@ -27,15 +28,23 @@
             msg_id=self.msg_cnt,
             buffers=buffers,
         )
         self.msg_cnt += 1
         asyncio.create_task(self.send_message(msg, self.shell_channel, change_date_to_str=True))
 
 
+class BusyEvent(Event):
+    def __init__(self, source, topic, busy: bool):
+        super().__init__(source, topic)
+        self.busy = busy
+
+
 class KernelMixin:
+    busy = Signal(BusyEvent)
+
     def __init__(self):
         self.msg_cnt = 0
         self.execute_requests: Dict[str, Dict[str, asyncio.Queue]] = {}
         self.recv_queue = asyncio.Queue()
         self.started = asyncio.Event()
         asyncio.create_task(self.recv())
 
@@ -85,14 +94,20 @@
                 for comm_handler in self.comm_handlers:
                     comm_id = msg["content"]["comm_id"]
                     comm = Comm(comm_id, self.shell_channel, self.session_id, self.send_message)
                     comm_handler.comm_open(msg, comm)
             elif msg_type == "comm_msg":
                 for comm_handler in self.comm_handlers:
                     comm_handler.comm_msg(msg)
+            elif msg_type == "status":
+                execution_state = msg["content"]["execution_state"]
+                if execution_state == "idle":
+                    self.busy.dispatch(False)
+                elif execution_state == "busy":
+                    self.busy.dispatch(True)
             msg_id = msg["parent_header"].get("msg_id")
             if msg_id in self.execute_requests:
                 # msg["header"] = str_to_date(msg["header"])
                 # msg["parent_header"] = str_to_date(msg["parent_header"])
                 self.execute_requests[msg_id][channel].put_nowait(msg)
 
     async def execute(
```

### Comparing `txl_kernel-0.2.8/txl_kernel/driver.py.keep` & `txl_kernel-0.2.9/txl_kernel/driver.py.keep`

 * *Files identical despite different names*

### Comparing `txl_kernel-0.2.8/txl_kernel/message.py` & `txl_kernel-0.2.9/txl_kernel/message.py`

 * *Files identical despite different names*

### Comparing `txl_kernel-0.2.8/LICENSE.txt` & `txl_kernel-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `txl_kernel-0.2.8/pyproject.toml` & `txl_kernel-0.2.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "txl",
+  "asphalt",
   "python-dateutil >=2.8.2",
   "pycrdt >=0.8.11,<0.9.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://github.com/davidbrochart/jpterm/plugins/kernel"
```

### Comparing `txl_kernel-0.2.8/PKG-INFO` & `txl_kernel-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: txl_kernel
-Version: 0.2.8
+Version: 0.2.9
 Summary: TXL plugin for a kernel driver
 Project-URL: Source, https://github.com/davidbrochart/jpterm/plugins/kernel
 Author-email: David Brochart <david.brochart@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
+Requires-Dist: asphalt
 Requires-Dist: pycrdt<0.9.0,>=0.8.11
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: txl
 Description-Content-Type: text/markdown
 
 # TXL plugin for a kernel driver
```

