# Comparing `tmp/cdk-rds-dump-2.1.3.tar.gz` & `tmp/cdk-rds-dump-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-rds-dump-2.1.3.tar", last modified: Mon May 13 04:23:38 2024, max compression
+gzip compressed data, was "cdk-rds-dump-2.1.4.tar", last modified: Sun May 26 01:28:25 2024, max compression
```

## Comparing `cdk-rds-dump-2.1.3.tar` & `cdk-rds-dump-2.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:23:38.418465 cdk-rds-dump-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-13 04:23:26.000000 cdk-rds-dump-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 04:23:26.000000 cdk-rds-dump-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-13 04:23:38.414465 cdk-rds-dump-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-13 04:23:26.000000 cdk-rds-dump-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-13 04:23:26.000000 cdk-rds-dump-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 04:23:38.418465 cdk-rds-dump-2.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-13 04:23:26.000000 cdk-rds-dump-2.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:23:38.410465 cdk-rds-dump-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:23:38.410465 cdk-rds-dump-2.1.3/src/cdk_rds_dump/
--rw-r--r--   0 runner    (1001) docker     (127)    25150 2024-05-13 04:23:26.000000 cdk-rds-dump-2.1.3/src/cdk_rds_dump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:23:38.414465 cdk-rds-dump-2.1.3/src/cdk_rds_dump/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 04:23:26.000000 cdk-rds-dump-2.1.3/src/cdk_rds_dump/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2632995 2024-05-13 04:23:26.000000 cdk-rds-dump-2.1.3/src/cdk_rds_dump/_jsii/cdk-rds-dump@2.1.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 04:23:26.000000 cdk-rds-dump-2.1.3/src/cdk_rds_dump/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:23:38.414465 cdk-rds-dump-2.1.3/src/cdk_rds_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-13 04:23:38.000000 cdk-rds-dump-2.1.3/src/cdk_rds_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 04:23:38.000000 cdk-rds-dump-2.1.3/src/cdk_rds_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 04:23:38.000000 cdk-rds-dump-2.1.3/src/cdk_rds_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 04:23:38.000000 cdk-rds-dump-2.1.3/src/cdk_rds_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 04:23:38.000000 cdk-rds-dump-2.1.3/src/cdk_rds_dump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:25.587394 cdk-rds-dump-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-26 01:28:08.000000 cdk-rds-dump-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 01:28:08.000000 cdk-rds-dump-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-26 01:28:25.587394 cdk-rds-dump-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-26 01:28:08.000000 cdk-rds-dump-2.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-26 01:28:08.000000 cdk-rds-dump-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 01:28:25.587394 cdk-rds-dump-2.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-26 01:28:08.000000 cdk-rds-dump-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:25.583394 cdk-rds-dump-2.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:25.583394 cdk-rds-dump-2.1.4/src/cdk_rds_dump/
+-rw-r--r--   0 runner    (1001) docker     (127)    25150 2024-05-26 01:28:08.000000 cdk-rds-dump-2.1.4/src/cdk_rds_dump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:25.583394 cdk-rds-dump-2.1.4/src/cdk_rds_dump/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-26 01:28:08.000000 cdk-rds-dump-2.1.4/src/cdk_rds_dump/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2560882 2024-05-26 01:28:08.000000 cdk-rds-dump-2.1.4/src/cdk_rds_dump/_jsii/cdk-rds-dump@2.1.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:28:08.000000 cdk-rds-dump-2.1.4/src/cdk_rds_dump/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:28:25.583394 cdk-rds-dump-2.1.4/src/cdk_rds_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-26 01:28:25.000000 cdk-rds-dump-2.1.4/src/cdk_rds_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-26 01:28:25.000000 cdk-rds-dump-2.1.4/src/cdk_rds_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:28:25.000000 cdk-rds-dump-2.1.4/src/cdk_rds_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-26 01:28:25.000000 cdk-rds-dump-2.1.4/src/cdk_rds_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 01:28:25.000000 cdk-rds-dump-2.1.4/src/cdk_rds_dump.egg-info/top_level.txt
```

### Comparing `cdk-rds-dump-2.1.3/LICENSE` & `cdk-rds-dump-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-2.1.3/PKG-INFO` & `cdk-rds-dump-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 2.1.3
+Version: 2.1.4
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-rds-dump-2.1.3/README.md` & `cdk-rds-dump-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-2.1.3/setup.py` & `cdk-rds-dump-2.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-rds-dump",
-    "version": "2.1.3",
+    "version": "2.1.4",
     "description": "CDK Construct Library by Typescript for RDS Dump",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-rds-dump.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_rds_dump",
         "cdk_rds_dump._jsii"
     ],
     "package_data": {
         "cdk_rds_dump._jsii": [
-            "cdk-rds-dump@2.1.3.jsii.tgz"
+            "cdk-rds-dump@2.1.4.jsii.tgz"
         ],
         "cdk_rds_dump": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-rds-dump-2.1.3/src/cdk_rds_dump/__init__.py` & `cdk-rds-dump-2.1.4/src/cdk_rds_dump/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-rds-dump-2.1.3/src/cdk_rds_dump.egg-info/PKG-INFO` & `cdk-rds-dump-2.1.4/src/cdk_rds_dump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-rds-dump
-Version: 2.1.3
+Version: 2.1.4
 Summary: CDK Construct Library by Typescript for RDS Dump
 Home-page: https://github.com/badmintoncryer/cdk-rds-dump.git
 Author: Kazuho CryerShinozuka<malaysia.cryer@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/badmintoncryer/cdk-rds-dump.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

