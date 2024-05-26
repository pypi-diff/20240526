# Comparing `tmp/tracor-0.1.1.tar.gz` & `tmp/tracor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracor-0.1.1.tar", last modified: Sun May 26 07:56:09 2024, max compression
+gzip compressed data, was "tracor-0.1.2.tar", last modified: Sun May 26 20:24:15 2024, max compression
```

## Comparing `tracor-0.1.1.tar` & `tracor-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:56:09.684624 tracor-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 07:56:05.000000 tracor-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-26 07:56:09.684624 tracor-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-26 07:56:05.000000 tracor-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:56:09.684624 tracor-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-26 07:56:05.000000 tracor-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:56:09.684624 tracor-0.1.1/tracor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:24:15.383989 tracor-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 20:24:07.000000 tracor-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-26 20:24:15.383989 tracor-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-26 20:24:07.000000 tracor-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 20:24:15.383989 tracor-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-26 20:24:07.000000 tracor-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:24:15.379989 tracor-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:24:07.000000 tracor-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:24:15.383989 tracor-0.1.2/tracor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:24:07.000000 tracor-0.1.2/tracor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-05-26 20:24:07.000000 tracor-0.1.2/tracor/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:24:15.383989 tracor-0.1.2/tracor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-26 20:24:15.000000 tracor-0.1.2/tracor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-26 20:24:15.000000 tracor-0.1.2/tracor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:24:15.000000 tracor-0.1.2/tracor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 20:24:15.000000 tracor-0.1.2/tracor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 20:24:15.000000 tracor-0.1.2/tracor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 20:24:15.000000 tracor-0.1.2/tracor.egg-info/top_level.txt
```

### Comparing `tracor-0.1.1/LICENSE` & `tracor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tracor-0.1.1/PKG-INFO` & `tracor-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for running Python scripts line by line with error handling and reporting.
 Home-page: https://github.com/ArlinJae/Tracor
 Author: Jae Arlin
 Author-email: jairelan.2005@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tracor-0.1.1/README.md` & `tracor-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tracor-0.1.1/setup.py` & `tracor-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tracor",
-    version="0.1.1",  # Ensure this is the updated version
+    version="0.1.2",  # Ensure this is the updated version
     packages=find_packages(),
     install_requires=[
         "colorama",
     ],
     entry_points={
         'console_scripts': [
             'tracor = tracor.core:main',
```

### Comparing `tracor-0.1.1/tracor.egg-info/PKG-INFO` & `tracor-0.1.2/tracor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for running Python scripts line by line with error handling and reporting.
 Home-page: https://github.com/ArlinJae/Tracor
 Author: Jae Arlin
 Author-email: jairelan.2005@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

