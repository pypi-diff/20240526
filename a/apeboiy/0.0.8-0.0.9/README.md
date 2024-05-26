# Comparing `tmp/apeboiy-0.0.8.tar.gz` & `tmp/apeboiy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apeboiy-0.0.8.tar", last modified: Wed May 22 14:07:46 2024, max compression
+gzip compressed data, was "apeboiy-0.0.9.tar", last modified: Wed May 22 14:26:49 2024, max compression
```

## Comparing `apeboiy-0.0.8.tar` & `apeboiy-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:07:46.525631 apeboiy-0.0.8/
--rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.8/LICENSE
--rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 14:07:46.525436 apeboiy-0.0.8/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      225 2024-05-22 10:51:09.000000 apeboiy-0.0.8/README.md
--rw-r--r--   0 iccy       (501) staff       (20)      621 2024-05-22 14:07:43.000000 apeboiy-0.0.8/pyproject.toml
--rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 14:07:46.525673 apeboiy-0.0.8/setup.cfg
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:07:46.522832 apeboiy-0.0.8/src/
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:07:46.523725 apeboiy-0.0.8/src/apeboiy/
--rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.8/src/apeboiy/__init__.py
--rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.8/src/apeboiy/example.py
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:07:46.524925 apeboiy-0.0.8/src/apeboiy/ply/
--rw-r--r--   0 iccy       (501) staff       (20)       28 2024-05-22 14:07:30.000000 apeboiy-0.0.8/src/apeboiy/ply/__init__.py
--rw-r--r--   0 iccy       (501) staff       (20)     3504 2024-05-22 14:04:38.000000 apeboiy-0.0.8/src/apeboiy/ply/_reader.py
-drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:07:46.525188 apeboiy-0.0.8/src/apeboiy.egg-info/
--rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 14:07:46.000000 apeboiy-0.0.8/src/apeboiy.egg-info/PKG-INFO
--rw-r--r--   0 iccy       (501) staff       (20)      308 2024-05-22 14:07:46.000000 apeboiy-0.0.8/src/apeboiy.egg-info/SOURCES.txt
--rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 14:07:46.000000 apeboiy-0.0.8/src/apeboiy.egg-info/dependency_links.txt
--rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 14:07:46.000000 apeboiy-0.0.8/src/apeboiy.egg-info/requires.txt
--rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 14:07:46.000000 apeboiy-0.0.8/src/apeboiy.egg-info/top_level.txt
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:26:49.193249 apeboiy-0.0.9/
+-rw-r--r--   0 iccy       (501) staff       (20)     1053 2024-05-22 10:25:41.000000 apeboiy-0.0.9/LICENSE
+-rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 14:26:49.193019 apeboiy-0.0.9/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      225 2024-05-22 10:51:09.000000 apeboiy-0.0.9/README.md
+-rw-r--r--   0 iccy       (501) staff       (20)      766 2024-05-22 14:26:42.000000 apeboiy-0.0.9/pyproject.toml
+-rw-r--r--   0 iccy       (501) staff       (20)       38 2024-05-22 14:26:49.193292 apeboiy-0.0.9/setup.cfg
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:26:49.188974 apeboiy-0.0.9/src/
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:26:49.189948 apeboiy-0.0.9/src/apeboiy/
+-rw-r--r--   0 iccy       (501) staff       (20)        0 2024-05-22 10:20:04.000000 apeboiy-0.0.9/src/apeboiy/__init__.py
+-rw-r--r--   0 iccy       (501) staff       (20)      115 2024-05-22 10:21:19.000000 apeboiy-0.0.9/src/apeboiy/example.py
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:26:49.191045 apeboiy-0.0.9/src/apeboiy/ply/
+-rw-r--r--   0 iccy       (501) staff       (20)       28 2024-05-22 14:07:30.000000 apeboiy-0.0.9/src/apeboiy/ply/__init__.py
+-rw-r--r--   0 iccy       (501) staff       (20)     3504 2024-05-22 14:04:38.000000 apeboiy-0.0.9/src/apeboiy/ply/_reader.py
+drwxr-xr-x   0 iccy       (501) staff       (20)        0 2024-05-22 14:26:49.191385 apeboiy-0.0.9/src/apeboiy.egg-info/
+-rw-r--r--   0 iccy       (501) staff       (20)      747 2024-05-22 14:26:49.000000 apeboiy-0.0.9/src/apeboiy.egg-info/PKG-INFO
+-rw-r--r--   0 iccy       (501) staff       (20)      308 2024-05-22 14:26:49.000000 apeboiy-0.0.9/src/apeboiy.egg-info/SOURCES.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        1 2024-05-22 14:26:49.000000 apeboiy-0.0.9/src/apeboiy.egg-info/dependency_links.txt
+-rw-r--r--   0 iccy       (501) staff       (20)       31 2024-05-22 14:26:49.000000 apeboiy-0.0.9/src/apeboiy.egg-info/requires.txt
+-rw-r--r--   0 iccy       (501) staff       (20)        8 2024-05-22 14:26:49.000000 apeboiy-0.0.9/src/apeboiy.egg-info/top_level.txt
```

### Comparing `apeboiy-0.0.8/LICENSE` & `apeboiy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apeboiy-0.0.8/PKG-INFO` & `apeboiy-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
 Keywords: appleboiy,shared,packages
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `apeboiy-0.0.8/pyproject.toml` & `apeboiy-0.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apeboiy"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { "name"="AppleBoiy", "email"="contact.chaipat@gmail.com"}
 ]
 description = "Shared AppleBoiy's packages."
 readme = "README.md"
 keywords = ["appleboiy", "shared", "packages"]
 requires-python = ">=3.8"
@@ -21,7 +21,11 @@
 [project.urls]
 Homepage = "https://github.com/AppleBoiy"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+[testenv]
+description = "Environment for running the tests"
+deps = "unittest"
+commands = "python -m unittest discover -s tests -v -p '*_test.py'"
```

### Comparing `apeboiy-0.0.8/src/apeboiy/ply/_reader.py` & `apeboiy-0.0.9/src/apeboiy/ply/_reader.py`

 * *Files identical despite different names*

### Comparing `apeboiy-0.0.8/src/apeboiy.egg-info/PKG-INFO` & `apeboiy-0.0.9/src/apeboiy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apeboiy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Shared AppleBoiy's packages.
 Author-email: AppleBoiy <contact.chaipat@gmail.com>
 Project-URL: Homepage, https://github.com/AppleBoiy
 Keywords: appleboiy,shared,packages
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

