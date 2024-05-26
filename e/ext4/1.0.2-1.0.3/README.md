# Comparing `tmp/ext4-1.0.2.tar.gz` & `tmp/ext4-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ext4-1.0.2.tar", last modified: Thu Apr 11 22:19:49 2024, max compression
+gzip compressed data, was "ext4-1.0.3.tar", last modified: Sun May 26 04:20:53 2024, max compression
```

## Comparing `ext4-1.0.2.tar` & `ext4-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:49.406913 ext4-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-11 22:19:45.000000 ext4-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-11 22:19:49.406913 ext4-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 22:19:45.000000 ext4-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:49.406913 ext4-1.0.2/ext4/
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/blockdescriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/extent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/htree.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/inode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/superblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-04-11 22:19:45.000000 ext4-1.0.2/ext4/xattr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:19:49.406913 ext4-1.0.2/ext4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 22:19:49.000000 ext4-1.0.2/ext4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-11 22:19:45.000000 ext4-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 22:19:45.000000 ext4-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:19:49.406913 ext4-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:53.980211 ext4-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-26 04:20:49.000000 ext4-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-26 04:20:53.980211 ext4-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-26 04:20:49.000000 ext4-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:53.976211 ext4-1.0.3/ext4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/blockdescriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/htree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/inode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/superblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/xattr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:53.980211 ext4-1.0.3/ext4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-26 04:20:49.000000 ext4-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 04:20:49.000000 ext4-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 04:20:53.980211 ext4-1.0.3/setup.cfg
```

### Comparing `ext4-1.0.2/LICENSE` & `ext4-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/PKG-INFO` & `ext4-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: ext4
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for read only interactions with an ext4 filesystem
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
```

### Comparing `ext4-1.0.2/ext4/__init__.py` & `ext4-1.0.3/ext4/__init__.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/block.py` & `ext4-1.0.3/ext4/block.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/blockdescriptor.py` & `ext4-1.0.3/ext4/blockdescriptor.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/directory.py` & `ext4-1.0.3/ext4/directory.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/enum.py` & `ext4-1.0.3/ext4/enum.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/extent.py` & `ext4-1.0.3/ext4/extent.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/htree.py` & `ext4-1.0.3/ext4/htree.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/inode.py` & `ext4-1.0.3/ext4/inode.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/struct.py` & `ext4-1.0.3/ext4/struct.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/superblock.py` & `ext4-1.0.3/ext4/superblock.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4/volume.py` & `ext4-1.0.3/ext4/volume.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
-import os
 import errno
 
 from uuid import UUID
+from pathlib import PurePosixPath
 
 from cachetools import cached
 from cachetools import LRUCache
 
 from .enum import EXT4_INO
 from .enum import MODE
 from .superblock import Superblock
@@ -175,31 +175,18 @@
         assert count > 0
         block_size = self.block_size  # Only calculate once
         self.seek(index * block_size)
         return self.read(count * block_size)
 
     @staticmethod
     def path_tuple(path):
-        if not isinstance(path, bytes):
-            path = path.encode("utf-8")
+        if isinstance(path, bytes):
+            path = path.decode("utf-8")
 
-        path = os.path.normpath(path)
-        paths = tuple()
-        if path == "/":
-            return paths
-
-        while True:
-            split = os.path.split(path)
-            path = split[0]
-            if not split[1]:
-                break
-
-            paths = (split[1],) + paths
-
-        return paths
+        return tuple(x.encode("utf-8") for x in PurePosixPath(path).parts)
 
     @cached(cache=LRUCache(maxsize=32))
     def inode_at(self, path):
         paths = list(self.path_tuple(path))
         cwd = self.root
         if not paths:
             return cwd
```

### Comparing `ext4-1.0.2/ext4/xattr.py` & `ext4-1.0.3/ext4/xattr.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.2/ext4.egg-info/PKG-INFO` & `ext4-1.0.3/ext4.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: ext4
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for read only interactions with an ext4 filesystem
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
```

### Comparing `ext4-1.0.2/pyproject.toml` & `ext4-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [project]
 name = "ext4"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Eeems", email="eeems@eeems.email" },
 ]
 description = "Library for read only interactions with an ext4 filesystem"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: POSIX :: Linux",
+    "Operating System :: POSIX",
+    "Operating System :: MacOS",
+    "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Filesystems",
     "Topic :: Utilities",
 ]
```

