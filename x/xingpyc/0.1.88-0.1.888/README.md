# Comparing `tmp/xingpyc-0.1.88.tar.gz` & `tmp/xingpyc-0.1.888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.1.88.tar", last modified: Sun May 26 06:21:12 2024, max compression
+gzip compressed data, was "xingpyc-0.1.888.tar", last modified: Sun May 26 06:25:14 2024, max compression
```

## Comparing `xingpyc-0.1.88.tar` & `xingpyc-0.1.888.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.484682 xingpyc-0.1.88/
--rw-r--r--   0 xiaolin    (501) staff       (20)      587 2024-05-26 06:21:12.484473 xingpyc-0.1.88/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.88/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      569 2024-05-26 06:21:09.000000 xingpyc-0.1.88/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:21:12.484723 xingpyc-0.1.88/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.482471 xingpyc-0.1.88/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.483132 xingpyc-0.1.88/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     8331 2024-05-26 06:18:43.000000 xingpyc-0.1.88/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.88/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.484240 xingpyc-0.1.88/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      587 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:21:12.000000 xingpyc-0.1.88/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:21:12.484051 xingpyc-0.1.88/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.88/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.656989 xingpyc-0.1.888/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      588 2024-05-26 06:25:14.656748 xingpyc-0.1.888/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.888/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      570 2024-05-26 06:25:07.000000 xingpyc-0.1.888/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:25:14.657040 xingpyc-0.1.888/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.654063 xingpyc-0.1.888/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.654941 xingpyc-0.1.888/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     8325 2024-05-26 06:25:00.000000 xingpyc-0.1.888/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.888/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.656399 xingpyc-0.1.888/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      588 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.656217 xingpyc-0.1.888/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.888/tests/test1.py
```

### Comparing `xingpyc-0.1.88/PKG-INFO` & `xingpyc-0.1.888/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.88
+Version: 0.1.888
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.1.88/pyproject.toml` & `xingpyc-0.1.888/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.1.88"
+version = "0.1.888"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.1.88/src/xingpyc/__init__.py` & `xingpyc-0.1.888/src/xingpyc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,24 +95,24 @@
     def global_onRecv(self, client_id, message):
         '''
         WebSocket Object should NOT go inside here, only client_id and message
         
         '''
         print(
             "\033[93mheader:"+
-            message[:10].replace(b"\x00", b"").decode()+
+            message[:10].replace(b" ", b"").decode()+
             "   id:"+
             message[10:20].decode()+
             "   length:"+
             str(len(message[20:]))+
             "\033[0m"
         )
         # connect client and save client id
 
-        header = message[:10].replace(b"\x00", b"").decode()
+        header = message[:10].replace(b" ", b"").decode()
         task_id = message[10:20]
 
         if client_id not in self.blockbuffers:
             self.blockbuffers[client_id] = []
 
         content = message[20:]
```

### Comparing `xingpyc-0.1.88/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.1.888/src/xingpyc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.88
+Version: 0.1.888
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

