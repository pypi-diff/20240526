# Comparing `tmp/socketbee-0.1.1.tar.gz` & `tmp/socketbee-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketbee-0.1.1.tar", last modified: Mon May 13 16:19:51 2024, max compression
+gzip compressed data, was "socketbee-0.1.2.tar", last modified: Sun May 26 21:23:03 2024, max compression
```

## Comparing `socketbee-0.1.1.tar` & `socketbee-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 16:19:51.562888 socketbee-0.1.1/
--rw-r--r--   0 boulamakandine   (501) staff       (20)     1053 2024-05-13 04:59:24.000000 socketbee-0.1.1/LICENSE.md
--rw-r--r--   0 boulamakandine   (501) staff       (20)      665 2024-05-13 16:19:51.562730 socketbee-0.1.1/PKG-INFO
--rw-r--r--   0 boulamakandine   (501) staff       (20)       32 2024-05-13 05:00:53.000000 socketbee-0.1.1/README.md
--rw-r--r--   0 boulamakandine   (501) staff       (20)      716 2024-05-13 16:19:49.000000 socketbee-0.1.1/pyproject.toml
--rw-r--r--   0 boulamakandine   (501) staff       (20)       38 2024-05-13 16:19:51.562925 socketbee-0.1.1/setup.cfg
--rw-r--r--   0 boulamakandine   (501) staff       (20)      121 2024-05-13 04:56:07.000000 socketbee-0.1.1/setup.py
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 16:19:51.561554 socketbee-0.1.1/socketbee/
--rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:01.000000 socketbee-0.1.1/socketbee/__init__.py
--rw-r--r--   0 boulamakandine   (501) staff       (20)     1583 2024-05-13 06:05:26.000000 socketbee-0.1.1/socketbee/client.py
--rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:14.000000 socketbee-0.1.1/socketbee/settings.py
-drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-13 16:19:51.562565 socketbee-0.1.1/socketbee.egg-info/
--rw-r--r--   0 boulamakandine   (501) staff       (20)      665 2024-05-13 16:19:51.000000 socketbee-0.1.1/socketbee.egg-info/PKG-INFO
--rw-r--r--   0 boulamakandine   (501) staff       (20)      272 2024-05-13 16:19:51.000000 socketbee-0.1.1/socketbee.egg-info/SOURCES.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)        1 2024-05-13 16:19:51.000000 socketbee-0.1.1/socketbee.egg-info/dependency_links.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)       33 2024-05-13 16:19:51.000000 socketbee-0.1.1/socketbee.egg-info/requires.txt
--rw-r--r--   0 boulamakandine   (501) staff       (20)       10 2024-05-13 16:19:51.000000 socketbee-0.1.1/socketbee.egg-info/top_level.txt
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-26 21:23:03.719967 socketbee-0.1.2/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     1053 2024-05-13 04:59:24.000000 socketbee-0.1.2/LICENSE.md
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      626 2024-05-26 21:23:03.719765 socketbee-0.1.2/PKG-INFO
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       32 2024-05-13 05:00:53.000000 socketbee-0.1.2/README.md
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      689 2024-05-26 21:23:00.000000 socketbee-0.1.2/pyproject.toml
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       38 2024-05-26 21:23:03.720007 socketbee-0.1.2/setup.cfg
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      121 2024-05-13 04:56:07.000000 socketbee-0.1.2/setup.py
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-26 21:23:03.718638 socketbee-0.1.2/socketbee/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:01.000000 socketbee-0.1.2/socketbee/__init__.py
+-rw-r--r--   0 boulamakandine   (501) staff       (20)     1460 2024-05-24 19:06:50.000000 socketbee-0.1.2/socketbee/client.py
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        0 2024-05-13 04:42:14.000000 socketbee-0.1.2/socketbee/settings.py
+drwxr-xr-x   0 boulamakandine   (501) staff       (20)        0 2024-05-26 21:23:03.719531 socketbee-0.1.2/socketbee.egg-info/
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      626 2024-05-26 21:23:03.000000 socketbee-0.1.2/socketbee.egg-info/PKG-INFO
+-rw-r--r--   0 boulamakandine   (501) staff       (20)      272 2024-05-26 21:23:03.000000 socketbee-0.1.2/socketbee.egg-info/SOURCES.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        1 2024-05-26 21:23:03.000000 socketbee-0.1.2/socketbee.egg-info/dependency_links.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)        9 2024-05-26 21:23:03.000000 socketbee-0.1.2/socketbee.egg-info/requires.txt
+-rw-r--r--   0 boulamakandine   (501) staff       (20)       10 2024-05-26 21:23:03.000000 socketbee-0.1.2/socketbee.egg-info/top_level.txt
```

### Comparing `socketbee-0.1.1/LICENSE.md` & `socketbee-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socketbee-0.1.1/PKG-INFO` & `socketbee-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: socketbee
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python wrapper for the SocketBee.
 Author-email: "Boulama K." <boulama@otimbi.com>
 Project-URL: Homepage, https://github.com/socketbee/socketbee.py
 Project-URL: Bug Tracker, https://github.com/socketbee/socketbee.py/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: python-socketio[client]
 Requires-Dist: requests
 
 ## SocketBee Python client
 
 WIP.
```

### Comparing `socketbee-0.1.1/pyproject.toml` & `socketbee-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "socketbee"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Boulama K.", email="boulama@otimbi.com" },
 ]
 description = "A Python wrapper for the SocketBee."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
-dependencies = ["python-socketio[client]", "requests"]
+dependencies = ["requests"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `socketbee-0.1.1/socketbee.egg-info/PKG-INFO` & `socketbee-0.1.2/socketbee.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: socketbee
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python wrapper for the SocketBee.
 Author-email: "Boulama K." <boulama@otimbi.com>
 Project-URL: Homepage, https://github.com/socketbee/socketbee.py
 Project-URL: Bug Tracker, https://github.com/socketbee/socketbee.py/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: python-socketio[client]
 Requires-Dist: requests
 
 ## SocketBee Python client
 
 WIP.
```

