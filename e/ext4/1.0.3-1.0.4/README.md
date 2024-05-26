# Comparing `tmp/ext4-1.0.3.tar.gz` & `tmp/ext4-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ext4-1.0.3.tar", last modified: Sun May 26 04:20:53 2024, max compression
+gzip compressed data, was "ext4-1.0.4.tar", last modified: Sun May 26 04:28:36 2024, max compression
```

## Comparing `ext4-1.0.3.tar` & `ext4-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:53.980211 ext4-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-26 04:20:49.000000 ext4-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-26 04:20:53.980211 ext4-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-26 04:20:49.000000 ext4-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:53.976211 ext4-1.0.3/ext4/
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/blockdescriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/extent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/htree.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/inode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/superblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-26 04:20:49.000000 ext4-1.0.3/ext4/xattr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:53.980211 ext4-1.0.3/ext4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 04:20:53.000000 ext4-1.0.3/ext4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-26 04:20:49.000000 ext4-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 04:20:49.000000 ext4-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 04:20:53.980211 ext4-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:28:36.772600 ext4-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-26 04:28:31.000000 ext4-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-26 04:28:36.772600 ext4-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-26 04:28:31.000000 ext4-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:28:36.768600 ext4-1.0.4/ext4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/blockdescriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/htree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/inode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/superblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-26 04:28:31.000000 ext4-1.0.4/ext4/xattr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:28:36.772600 ext4-1.0.4/ext4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-26 04:28:36.000000 ext4-1.0.4/ext4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-26 04:28:36.000000 ext4-1.0.4/ext4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 04:28:36.000000 ext4-1.0.4/ext4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 04:28:36.000000 ext4-1.0.4/ext4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 04:28:36.000000 ext4-1.0.4/ext4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-26 04:28:31.000000 ext4-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 04:28:31.000000 ext4-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 04:28:36.772600 ext4-1.0.4/setup.cfg
```

### Comparing `ext4-1.0.3/LICENSE` & `ext4-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/PKG-INFO` & `ext4-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ext4
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for read only interactions with an ext4 filesystem
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `ext4-1.0.3/ext4/__init__.py` & `ext4-1.0.4/ext4/__init__.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/block.py` & `ext4-1.0.4/ext4/block.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/blockdescriptor.py` & `ext4-1.0.4/ext4/blockdescriptor.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/directory.py` & `ext4-1.0.4/ext4/directory.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/enum.py` & `ext4-1.0.4/ext4/enum.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/extent.py` & `ext4-1.0.4/ext4/extent.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/htree.py` & `ext4-1.0.4/ext4/htree.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/inode.py` & `ext4-1.0.4/ext4/inode.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/struct.py` & `ext4-1.0.4/ext4/struct.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/superblock.py` & `ext4-1.0.4/ext4/superblock.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4/volume.py` & `ext4-1.0.4/ext4/volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         return self.read(count * block_size)
 
     @staticmethod
     def path_tuple(path):
         if isinstance(path, bytes):
             path = path.decode("utf-8")
 
-        return tuple(x.encode("utf-8") for x in PurePosixPath(path).parts)
+        return tuple(x.encode("utf-8") for x in PurePosixPath(path).parts[1:])
 
     @cached(cache=LRUCache(maxsize=32))
     def inode_at(self, path):
         paths = list(self.path_tuple(path))
         cwd = self.root
         if not paths:
             return cwd
```

### Comparing `ext4-1.0.3/ext4/xattr.py` & `ext4-1.0.4/ext4/xattr.py`

 * *Files identical despite different names*

### Comparing `ext4-1.0.3/ext4.egg-info/PKG-INFO` & `ext4-1.0.4/ext4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ext4
-Version: 1.0.3
+Version: 1.0.4
 Summary: Library for read only interactions with an ext4 filesystem
 Author-email: Eeems <eeems@eeems.email>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `ext4-1.0.3/pyproject.toml` & `ext4-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ext4"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Eeems", email="eeems@eeems.email" },
 ]
 description = "Library for read only interactions with an ext4 filesystem"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
```

