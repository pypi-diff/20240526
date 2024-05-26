# Comparing `tmp/rds-scheduler-1.0.8.tar.gz` & `tmp/rds-scheduler-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-scheduler-1.0.8.tar", last modified: Tue May 14 00:20:24 2024, max compression
+gzip compressed data, was "rds-scheduler-1.0.9.tar", last modified: Sun May 26 01:28:10 2024, max compression
```

## Comparing `rds-scheduler-1.0.8.tar` & `rds-scheduler-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/src/rds_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/src/rds_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/src/rds_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/src/rds_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62194 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/src/rds_scheduler/_jsii/cdk-rds-scheduler@1.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:20:13.000000 rds-scheduler-1.0.8/src/rds_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:20:24.242092 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 00:20:24.000000 rds-scheduler-1.0.8/src/rds_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:10.808225 rds-scheduler-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-26 01:27:52.000000 rds-scheduler-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 01:27:52.000000 rds-scheduler-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-26 01:28:10.808225 rds-scheduler-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-26 01:27:52.000000 rds-scheduler-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-26 01:27:52.000000 rds-scheduler-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 01:28:10.808225 rds-scheduler-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-26 01:27:52.000000 rds-scheduler-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:10.804225 rds-scheduler-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:10.804225 rds-scheduler-1.0.9/src/rds_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)    18712 2024-05-26 01:27:52.000000 rds-scheduler-1.0.9/src/rds_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:10.808225 rds-scheduler-1.0.9/src/rds_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-26 01:27:52.000000 rds-scheduler-1.0.9/src/rds_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62194 2024-05-26 01:27:52.000000 rds-scheduler-1.0.9/src/rds_scheduler/_jsii/cdk-rds-scheduler@1.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:27:52.000000 rds-scheduler-1.0.9/src/rds_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:10.808225 rds-scheduler-1.0.9/src/rds_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-26 01:28:10.000000 rds-scheduler-1.0.9/src/rds_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-26 01:28:10.000000 rds-scheduler-1.0.9/src/rds_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:28:10.000000 rds-scheduler-1.0.9/src/rds_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-26 01:28:10.000000 rds-scheduler-1.0.9/src/rds_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 01:28:10.000000 rds-scheduler-1.0.9/src/rds_scheduler.egg-info/top_level.txt
```

### Comparing `rds-scheduler-1.0.8/LICENSE` & `rds-scheduler-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rds-scheduler-1.0.8/PKG-INFO` & `rds-scheduler-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds-scheduler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Automatic Start and Stop Scheduler for AWS RDS
 Home-page: https://github.com/badmintoncryer/cdk-rds-scheduler.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `rds-scheduler-1.0.8/README.md` & `rds-scheduler-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rds-scheduler-1.0.8/setup.py` & `rds-scheduler-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "rds-scheduler",
-    "version": "1.0.8",
+    "version": "1.0.9",
     "description": "Automatic Start and Stop Scheduler for AWS RDS",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-rds-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "rds_scheduler",
         "rds_scheduler._jsii"
     ],
     "package_data": {
         "rds_scheduler._jsii": [
-            "cdk-rds-scheduler@1.0.8.jsii.tgz"
+            "cdk-rds-scheduler@1.0.9.jsii.tgz"
         ],
         "rds_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `rds-scheduler-1.0.8/src/rds_scheduler/__init__.py` & `rds-scheduler-1.0.9/src/rds_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-scheduler-1.0.8/src/rds_scheduler.egg-info/PKG-INFO` & `rds-scheduler-1.0.9/src/rds_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds-scheduler
-Version: 1.0.8
+Version: 1.0.9
 Summary: Automatic Start and Stop Scheduler for AWS RDS
 Home-page: https://github.com/badmintoncryer/cdk-rds-scheduler.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

