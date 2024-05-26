# Comparing `tmp/cdk-ecr-deployment-3.0.8.tar.gz` & `tmp/cdk-ecr-deployment-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-ecr-deployment-3.0.8.tar", last modified: Thu Jan 11 18:15:46 2024, max compression
+gzip compressed data, was "cdk-ecr-deployment-3.0.9.tar", last modified: Fri Jan 12 18:15:57 2024, max compression
```

## Comparing `cdk-ecr-deployment-3.0.8.tar` & `cdk-ecr-deployment-3.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:15:46.461860 cdk-ecr-deployment-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-01-11 18:15:46.461860 cdk-ecr-deployment-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 18:15:46.461860 cdk-ecr-deployment-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:15:46.457859 cdk-ecr-deployment-3.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:15:46.457859 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment/
--rw-r--r--   0 runner    (1001) docker     (127)    25667 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:15:46.457859 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  2033096 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment/_jsii/cdk-ecr-deployment@3.0.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 18:15:35.000000 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:15:46.457859 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-01-11 18:15:46.000000 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-11 18:15:46.000000 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 18:15:46.000000 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-11 18:15:46.000000 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-11 18:15:46.000000 cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 18:15:57.385522 cdk-ecr-deployment-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-01-12 18:15:57.385522 cdk-ecr-deployment-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 18:15:57.385522 cdk-ecr-deployment-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 18:15:57.381522 cdk-ecr-deployment-3.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 18:15:57.381522 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)    25667 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 18:15:57.381522 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2033160 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment/_jsii/cdk-ecr-deployment@3.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 18:15:45.000000 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 18:15:57.381522 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-01-12 18:15:57.000000 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-12 18:15:57.000000 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 18:15:57.000000 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-01-12 18:15:57.000000 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-12 18:15:57.000000 cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment.egg-info/top_level.txt
```

### Comparing `cdk-ecr-deployment-3.0.8/LICENSE` & `cdk-ecr-deployment-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-ecr-deployment-3.0.8/PKG-INFO` & `cdk-ecr-deployment-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-ecr-deployment
-Version: 3.0.8
+Version: 3.0.9
 Summary: CDK construct to deploy docker image to Amazon ECR
 Home-page: https://github.com/cdklabs/cdk-ecr-deployment
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecr-deployment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-ecr-deployment-3.0.8/README.md` & `cdk-ecr-deployment-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-ecr-deployment-3.0.8/setup.py` & `cdk-ecr-deployment-3.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-ecr-deployment",
-    "version": "3.0.8",
+    "version": "3.0.9",
     "description": "CDK construct to deploy docker image to Amazon ECR",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-ecr-deployment",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_ecr_deployment",
         "cdk_ecr_deployment._jsii"
     ],
     "package_data": {
         "cdk_ecr_deployment._jsii": [
-            "cdk-ecr-deployment@3.0.8.jsii.tgz"
+            "cdk-ecr-deployment@3.0.9.jsii.tgz"
         ],
         "cdk_ecr_deployment": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment/__init__.py` & `cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-ecr-deployment-3.0.8/src/cdk_ecr_deployment.egg-info/PKG-INFO` & `cdk-ecr-deployment-3.0.9/src/cdk_ecr_deployment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-ecr-deployment
-Version: 3.0.8
+Version: 3.0.9
 Summary: CDK construct to deploy docker image to Amazon ECR
 Home-page: https://github.com/cdklabs/cdk-ecr-deployment
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-ecr-deployment
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

