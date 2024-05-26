# Comparing `tmp/remarkable_update_fuse-1.1.0.tar.gz` & `tmp/remarkable_update_fuse-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remarkable_update_fuse-1.1.0.tar", last modified: Sun May 26 02:41:03 2024, max compression
+gzip compressed data, was "remarkable_update_fuse-1.1.1.tar", last modified: Sun May 26 04:50:09 2024, max compression
```

## Comparing `remarkable_update_fuse-1.1.0.tar` & `remarkable_update_fuse-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:41:03.282991 remarkable_update_fuse-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-26 02:41:03.282991 remarkable_update_fuse-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:41:03.278990 remarkable_update_fuse-1.1.0/remarkable_update_fuse/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:41:03.282991 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 02:41:03.000000 remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 02:40:51.000000 remarkable_update_fuse-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 02:41:03.282991 remarkable_update_fuse-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:50:09.398180 remarkable_update_fuse-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-26 04:50:00.000000 remarkable_update_fuse-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-26 04:50:09.398180 remarkable_update_fuse-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-26 04:50:00.000000 remarkable_update_fuse-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-26 04:50:00.000000 remarkable_update_fuse-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:50:09.398180 remarkable_update_fuse-1.1.1/remarkable_update_fuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-26 04:50:00.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-26 04:50:00.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-26 04:50:00.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-26 04:50:00.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:50:09.398180 remarkable_update_fuse-1.1.1/remarkable_update_fuse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-26 04:50:09.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-26 04:50:09.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 04:50:09.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-26 04:50:09.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 04:50:09.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 04:50:09.000000 remarkable_update_fuse-1.1.1/remarkable_update_fuse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 04:50:00.000000 remarkable_update_fuse-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 04:50:09.398180 remarkable_update_fuse-1.1.1/setup.cfg
```

### Comparing `remarkable_update_fuse-1.1.0/LICENSE` & `remarkable_update_fuse-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.1.0/PKG-INFO` & `remarkable_update_fuse-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remarkable_update_fuse
-Version: 1.1.0
+Version: 1.1.1
 Summary: Userspace filesystem for remarkable update files
 Author-email: Eeems <eeems@eeems.email>
 Project-URL: Homepage, https://github.com/Eeems-Org/remarkable-update-fuse
 Project-URL: Repository, https://github.com/Eeems-Org/remarkable-update-fuse.git
 Project-URL: Issues, https://github.com/Eeems-Org/remarkable-update-fuse/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuse-python==1.0.7
-Requires-Dist: remarkable-update-image==1.0.0
+Requires-Dist: remarkable-update-image==1.0.1
 
 [![remarkable_update_fuse on PyPI](https://img.shields.io/pypi/v/remarkable_update_fuse)](https://pypi.org/project/remarkable_update_fuse)
 
 # reMarkable Update FUSE
 Mount remarkable update files using FUSE
 
 ## Usage
```

### Comparing `remarkable_update_fuse-1.1.0/README.md` & `remarkable_update_fuse-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.1.0/pyproject.toml` & `remarkable_update_fuse-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "remarkable_update_fuse"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Eeems", email="eeems@eeems.email" },
 ]
 description = "Userspace filesystem for remarkable update files"
 requires-python = ">=3.11"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `remarkable_update_fuse-1.1.0/remarkable_update_fuse/fuse.py` & `remarkable_update_fuse-1.1.1/remarkable_update_fuse/fuse.py`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.1.0/remarkable_update_fuse/threads.py` & `remarkable_update_fuse-1.1.1/remarkable_update_fuse/threads.py`

 * *Files identical despite different names*

### Comparing `remarkable_update_fuse-1.1.0/remarkable_update_fuse.egg-info/PKG-INFO` & `remarkable_update_fuse-1.1.1/remarkable_update_fuse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remarkable_update_fuse
-Version: 1.1.0
+Version: 1.1.1
 Summary: Userspace filesystem for remarkable update files
 Author-email: Eeems <eeems@eeems.email>
 Project-URL: Homepage, https://github.com/Eeems-Org/remarkable-update-fuse
 Project-URL: Repository, https://github.com/Eeems-Org/remarkable-update-fuse.git
 Project-URL: Issues, https://github.com/Eeems-Org/remarkable-update-fuse/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuse-python==1.0.7
-Requires-Dist: remarkable-update-image==1.0.0
+Requires-Dist: remarkable-update-image==1.0.1
 
 [![remarkable_update_fuse on PyPI](https://img.shields.io/pypi/v/remarkable_update_fuse)](https://pypi.org/project/remarkable_update_fuse)
 
 # reMarkable Update FUSE
 Mount remarkable update files using FUSE
 
 ## Usage
```

