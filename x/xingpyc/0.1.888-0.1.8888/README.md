# Comparing `tmp/xingpyc-0.1.888.tar.gz` & `tmp/xingpyc-0.1.8888.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.1.888.tar", last modified: Sun May 26 06:25:14 2024, max compression
+gzip compressed data, was "xingpyc-0.1.8888.tar", last modified: Sun May 26 06:32:30 2024, max compression
```

## Comparing `xingpyc-0.1.888.tar` & `xingpyc-0.1.8888.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.656989 xingpyc-0.1.888/
--rw-r--r--   0 xiaolin    (501) staff       (20)      588 2024-05-26 06:25:14.656748 xingpyc-0.1.888/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.888/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      570 2024-05-26 06:25:07.000000 xingpyc-0.1.888/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:25:14.657040 xingpyc-0.1.888/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.654063 xingpyc-0.1.888/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.654941 xingpyc-0.1.888/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)     8325 2024-05-26 06:25:00.000000 xingpyc-0.1.888/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.888/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.656399 xingpyc-0.1.888/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      588 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/requires.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:25:14.000000 xingpyc-0.1.888/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:25:14.656217 xingpyc-0.1.888/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.888/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:32:30.003044 xingpyc-0.1.8888/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      589 2024-05-26 06:32:30.002837 xingpyc-0.1.8888/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.1.8888/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      571 2024-05-26 06:32:26.000000 xingpyc-0.1.8888/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-26 06:32:30.003088 xingpyc-0.1.8888/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:32:30.000928 xingpyc-0.1.8888/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:32:30.001443 xingpyc-0.1.8888/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)     8467 2024-05-26 06:32:14.000000 xingpyc-0.1.8888/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.1.8888/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:32:30.002624 xingpyc-0.1.8888/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      589 2024-05-26 06:32:29.000000 xingpyc-0.1.8888/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      260 2024-05-26 06:32:29.000000 xingpyc-0.1.8888/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-26 06:32:29.000000 xingpyc-0.1.8888/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-26 06:32:29.000000 xingpyc-0.1.8888/src/xingpyc.egg-info/requires.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-26 06:32:29.000000 xingpyc-0.1.8888/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-26 06:32:30.002468 xingpyc-0.1.8888/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-26 05:08:18.000000 xingpyc-0.1.8888/tests/test1.py
```

### Comparing `xingpyc-0.1.888/PKG-INFO` & `xingpyc-0.1.8888/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.888
+Version: 0.1.8888
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xingpyc-0.1.888/pyproject.toml` & `xingpyc-0.1.8888/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xingpyc"
-version = "0.1.888"
+version = "0.1.8888"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xingpyc-0.1.888/src/xingpyc/__init__.py` & `xingpyc-0.1.8888/src/xingpyc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,17 +155,20 @@
                             task_id = task_id.encode("utf-8")
                         if isinstance(header, str):
                             header = header.encode("utf-8")
                         if isinstance(content, str):
                             content = content.encode("utf-8")
                         if client_id == -1:
                             print("start sending to cloud")
+                            count = 0
                             while len(content) > blocksize:
                                 self.cloudClient.send_bytes(b"block     " + task_id + content[0:blocksize])
                                 content = content[blocksize:]
+                                print(f"sent block {count}")
+                                count += 1
 
                             self.cloudClient.send_bytes(header + task_id + content)
                             print("sent to cloud")
                         else:
                             await self.asServer_send(client_id, header, task_id, content)
 
                         break # only send one result at a time
```

### Comparing `xingpyc-0.1.888/src/xingpyc.egg-info/PKG-INFO` & `xingpyc-0.1.8888/src/xingpyc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xingpyc
-Version: 0.1.888
+Version: 0.1.8888
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/Lx017/XingPyClient
 Project-URL: Issues, https://github.com/Lx017/XingPyClient/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
