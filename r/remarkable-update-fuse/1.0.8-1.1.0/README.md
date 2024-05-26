# Comparing `tmp/remarkable_update_fuse-1.0.8.tar.gz` & `tmp/remarkable_update_fuse-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remarkable_update_fuse-1.0.8.tar", last modified: Sat May  4 09:09:37 2024, max compression
+gzip compressed data, was "remarkable_update_fuse-1.1.0.tar", last modified: Sun May 26 02:41:03 2024, max compression
```

## Comparing `remarkable_update_fuse-1.0.8.tar` & `remarkable_update_fuse-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/remarkable_update_fuse/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-04 09:09:26.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse/update_metadata_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-04 09:09:37.000000 remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 09:09:05.000000 remarkable_update_fuse-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 09:09:37.605716 remarkable_update_fuse-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:41:03.282991 remarkable_update_fuse-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-26 02:41:03.282991 remarkable_update_fuse-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:41:03.278990 remarkable_update_fuse-1.1.0/remarkable_update_fuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:41:03.282991 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 02:41:03.282991 remarkable_update_fuse-1.1.0/setup.cfg
```

### Comparing `remarkable_update_fuse-1.0.8/LICENSE` & `remarkable_update_fuse-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.8/PKG-INFO` & `remarkable_update_fuse-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: remarkable_update_fuse
-Version: 1.0.8
+Version: 1.1.0
 Summary: Userspace filesystem for remarkable update files
 Author-email: Eeems <eeems@eeems.email>
+Project-URL: Homepage, https://github.com/Eeems-Org/remarkable-update-fuse
+Project-URL: Repository, https://github.com/Eeems-Org/remarkable-update-fuse.git
+Project-URL: Issues, https://github.com/Eeems-Org/remarkable-update-fuse/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cryptography==41.0.7
 Requires-Dist: fuse-python==1.0.7
-Requires-Dist: protobuf==4.21.1
-Requires-Dist: ext4==1.0.2
+Requires-Dist: remarkable-update-image==1.0.0
 
 [![remarkable_update_fuse on PyPI](https://img.shields.io/pypi/v/remarkable_update_fuse)](https://pypi.org/project/remarkable_update_fuse)
 
 # reMarkable Update FUSE
 Mount remarkable update files using FUSE
 
 ## Usage
@@ -36,33 +37,14 @@
 ```
 
 ## Known Issues
 
 - Will report checksum errors for Directory inode, even though they are fine
 - Will report checksum errors for extent headers, even though they are fine
 
-## Programatic Usage
-
-```python
-from ext4 import Volume
-from remarkable_update_fuse import UpdateImage
-
-image = UpdateImage("path/to/update/file.signed")
-
-# Extract raw ext4 image
-with open("image.ext4", "wb") as f:
-    f.write(image.read())
-
-# Extract specific file
-volume = Volume(image)
-inode = volume.inode_at("/etc/version")
-with open("version", "wb") as f:
-    f.write(inode.open().read())
-```
-
 ## Building
 Dependencies:
 - curl
 - protoc
 - python
 - python-build
 - python-pip
@@ -71,9 +53,10 @@
 - python-wheel
 
 ```bash
 make # Build wheel and sdist packages in dist/
 make wheel # Build wheel package in dist/
 make sdist # Build sdist package in dist/
 make dev # Test mounting 2.15.1.1189 to .venv/mnt
+make test # Run automated tests
 make install # Build wheel and install it with pipx or pip install --user
 ```
```

### Comparing `remarkable_update_fuse-1.0.8/pyproject.toml` & `remarkable_update_fuse-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "remarkable_update_fuse"
-version = "1.0.8"
+version = "1.1.0"
 authors = [
   { name="Eeems", email="eeems@eeems.email" },
 ]
 description = "Userspace filesystem for remarkable update files"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -17,14 +17,19 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Filesystems",
     "Topic :: Utilities",
 ]
 dynamic = ["dependencies", "readme"]
 
+[project.urls]
+Homepage = "https://github.com/Eeems-Org/remarkable-update-fuse"
+Repository = "https://github.com/Eeems-Org/remarkable-update-fuse.git"
+Issues = "https://github.com/Eeems-Org/remarkable-update-fuse/issues"
+
 [project.scripts]
 rmufuse = "remarkable_update_fuse.__main__:main"
 
 [tool.setuptools]
 packages = [
     "remarkable_update_fuse",
 ]
```

### Comparing `remarkable_update_fuse-1.0.8/remarkable_update_fuse/fuse.py` & `remarkable_update_fuse-1.1.0/remarkable_update_fuse/fuse.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,22 @@
 import warnings
 
 from pathlib import PurePosixPath
 
 import fuse
 import ext4
 
-from .image import UpdateImage
-from .image import UpdateImageSignatureException
+from remarkable_update_image import UpdateImage
+from remarkable_update_image import UpdateImageSignatureException
 from .threads import KillableThread
 
 
 fuse.fuse_python_api = (0, 2)
 
 
-class ImageException(Exception):
-    pass
-
-
 class FuseArgs(fuse.FuseArgs):
     def __init__(self):
         fuse.FuseArgs.__init__(self)
         self.update_file = None
 
     def __str__(self):
         return (
```

### Comparing `remarkable_update_fuse-1.0.8/remarkable_update_fuse/threads.py` & `remarkable_update_fuse-1.1.0/remarkable_update_fuse/threads.py`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.0.8/remarkable_update_fuse.egg-info/PKG-INFO` & `remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: remarkable_update_fuse
-Version: 1.0.8
+Version: 1.1.0
 Summary: Userspace filesystem for remarkable update files
 Author-email: Eeems <eeems@eeems.email>
+Project-URL: Homepage, https://github.com/Eeems-Org/remarkable-update-fuse
+Project-URL: Repository, https://github.com/Eeems-Org/remarkable-update-fuse.git
+Project-URL: Issues, https://github.com/Eeems-Org/remarkable-update-fuse/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cryptography==41.0.7
 Requires-Dist: fuse-python==1.0.7
-Requires-Dist: protobuf==4.21.1
-Requires-Dist: ext4==1.0.2
+Requires-Dist: remarkable-update-image==1.0.0
 
 [![remarkable_update_fuse on PyPI](https://img.shields.io/pypi/v/remarkable_update_fuse)](https://pypi.org/project/remarkable_update_fuse)
 
 # reMarkable Update FUSE
 Mount remarkable update files using FUSE
 
 ## Usage
@@ -36,33 +37,14 @@
 ```
 
 ## Known Issues
 
 - Will report checksum errors for Directory inode, even though they are fine
 - Will report checksum errors for extent headers, even though they are fine
 
-## Programatic Usage
-
-```python
-from ext4 import Volume
-from remarkable_update_fuse import UpdateImage
-
-image = UpdateImage("path/to/update/file.signed")
-
-# Extract raw ext4 image
-with open("image.ext4", "wb") as f:
-    f.write(image.read())
-
-# Extract specific file
-volume = Volume(image)
-inode = volume.inode_at("/etc/version")
-with open("version", "wb") as f:
-    f.write(inode.open().read())
-```
-
 ## Building
 Dependencies:
 - curl
 - protoc
 - python
 - python-build
 - python-pip
@@ -71,9 +53,10 @@
 - python-wheel
 
 ```bash
 make # Build wheel and sdist packages in dist/
 make wheel # Build wheel package in dist/
 make sdist # Build sdist package in dist/
 make dev # Test mounting 2.15.1.1189 to .venv/mnt
+make test # Run automated tests
 make install # Build wheel and install it with pipx or pip install --user
 ```
```

