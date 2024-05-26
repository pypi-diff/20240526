# Comparing `tmp/cam_manager-0.1.2.tar.gz` & `tmp/cam_manager-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cam_manager-0.1.2.tar", last modified: Tue May 21 13:54:11 2024, max compression
+gzip compressed data, was "cam_manager-0.1.3.tar", last modified: Sun May 26 20:38:17 2024, max compression
```

## Comparing `cam_manager-0.1.2.tar` & `cam_manager-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:11.882697 cam_manager-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-21 13:54:11.882697 cam_manager-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-21 13:54:08.000000 cam_manager-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:11.878697 cam_manager-0.1.2/cam_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 13:54:08.000000 cam_manager-0.1.2/cam_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-21 13:54:08.000000 cam_manager-0.1.2/cam_manager/cam_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:11.878697 cam_manager-0.1.2/cam_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-21 13:54:11.000000 cam_manager-0.1.2/cam_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-21 13:54:11.000000 cam_manager-0.1.2/cam_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:54:11.000000 cam_manager-0.1.2/cam_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 13:54:11.000000 cam_manager-0.1.2/cam_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 13:54:11.000000 cam_manager-0.1.2/cam_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:54:11.882697 cam_manager-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 13:54:08.000000 cam_manager-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:38:17.567403 cam_manager-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 20:38:13.000000 cam_manager-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-26 20:38:17.567403 cam_manager-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-26 20:38:13.000000 cam_manager-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:38:17.567403 cam_manager-0.1.3/cam_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-26 20:38:13.000000 cam_manager-0.1.3/cam_manager/cam_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:38:17.567403 cam_manager-0.1.3/cam_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 20:38:17.000000 cam_manager-0.1.3/cam_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 20:38:17.567403 cam_manager-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-26 20:38:13.000000 cam_manager-0.1.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)  6534387 2024-05-26 20:38:14.000000 cam_manager-0.1.3/yolov8n.pt
```

### Comparing `cam_manager-0.1.2/PKG-INFO` & `cam_manager-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cam_manager-0.1.2/README.md` & `cam_manager-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cam_manager-0.1.2/cam_manager.egg-info/PKG-INFO` & `cam_manager-0.1.3/cam_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cam_manager
-Version: 0.1.2
+Version: 0.1.3
 Summary: A camera management library to easily handle cameras with OpenCV.
 Home-page: https://github.com/snatev/cam-manager
 Author: snatev
 Author-email: snatev@proton.me
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cam_manager-0.1.2/setup.py` & `cam_manager-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
-    version = "0.1.2",
+    version = "0.1.3",
     name = "cam_manager",
     description = "A camera management library to easily handle cameras with OpenCV.",
 
     long_description = open("README.md").read(),
     long_description_content_type = "text/markdown",
 
     author = "snatev",
     author_email = "snatev@proton.me",
     url = "https://github.com/snatev/cam-manager",
 
+    include_package_data = True,
+
     packages = find_packages(),
     install_requires = [
         "opencv-python"
     ],
 
     classifiers = [
         "Operating System :: OS Independent",
```

