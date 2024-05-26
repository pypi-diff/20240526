# Comparing `tmp/gammarers.aws-secure-flow-log-bucket-1.4.3.tar.gz` & `tmp/gammarers.aws-secure-flow-log-bucket-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-secure-flow-log-bucket-1.4.3.tar", last modified: Sun May 19 19:18:52 2024, max compression
+gzip compressed data, was "gammarers.aws-secure-flow-log-bucket-1.4.4.tar", last modified: Sun May 26 19:19:59 2024, max compression
```

## Comparing `gammarers.aws-secure-flow-log-bucket-1.4.3.tar` & `gammarers.aws-secure-flow-log-bucket-1.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:18:52.319885 gammarers.aws-secure-flow-log-bucket-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 19:18:42.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 19:18:42.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-19 19:18:52.319885 gammarers.aws-secure-flow-log-bucket-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-19 19:18:42.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-19 19:18:42.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:18:52.319885 gammarers.aws-secure-flow-log-bucket-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-19 19:18:42.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:18:52.315885 gammarers.aws-secure-flow-log-bucket-1.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:18:52.315885 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:18:52.315885 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers/aws_secure_flow_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-05-19 19:18:42.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers/aws_secure_flow_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:18:52.315885 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers/aws_secure_flow_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-19 19:18:42.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers/aws_secure_flow_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23971 2024-05-19 19:18:42.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.4.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:18:42.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers/aws_secure_flow_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:18:52.315885 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers.aws_secure_flow_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-19 19:18:52.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers.aws_secure_flow_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-19 19:18:52.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:18:52.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-19 19:18:52.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers.aws_secure_flow_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 19:18:52.000000 gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers.aws_secure_flow_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:19:59.117004 gammarers.aws-secure-flow-log-bucket-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-26 19:19:47.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 19:19:47.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-26 19:19:59.117004 gammarers.aws-secure-flow-log-bucket-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-26 19:19:47.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-26 19:19:47.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 19:19:59.117004 gammarers.aws-secure-flow-log-bucket-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-26 19:19:47.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:19:59.113003 gammarers.aws-secure-flow-log-bucket-1.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:19:59.113003 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:19:59.117004 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers/aws_secure_flow_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-05-26 19:19:47.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers/aws_secure_flow_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:19:59.117004 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers/aws_secure_flow_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-26 19:19:47.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers/aws_secure_flow_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23973 2024-05-26 19:19:47.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.4.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:19:47.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers/aws_secure_flow_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:19:59.117004 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers.aws_secure_flow_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-26 19:19:59.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers.aws_secure_flow_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-26 19:19:59.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:19:59.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-26 19:19:59.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers.aws_secure_flow_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 19:19:59.000000 gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers.aws_secure_flow_log_bucket.egg-info/top_level.txt
```

### Comparing `gammarers.aws-secure-flow-log-bucket-1.4.3/LICENSE` & `gammarers.aws-secure-flow-log-bucket-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-flow-log-bucket-1.4.3/PKG-INFO` & `gammarers.aws-secure-flow-log-bucket-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-flow-log-bucket
-Version: 1.4.3
+Version: 1.4.4
 Summary: Specific AWS VPC FlowLog Bucket
 Home-page: https://github.com/gammarers/aws-secure-flow-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-flow-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-flow-log-bucket-1.4.3/README.md` & `gammarers.aws-secure-flow-log-bucket-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-flow-log-bucket-1.4.3/setup.py` & `gammarers.aws-secure-flow-log-bucket-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-secure-flow-log-bucket",
-    "version": "1.4.3",
+    "version": "1.4.4",
     "description": "Specific AWS VPC FlowLog Bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-secure-flow-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_secure_flow_log_bucket",
         "gammarers.aws_secure_flow_log_bucket._jsii"
     ],
     "package_data": {
         "gammarers.aws_secure_flow_log_bucket._jsii": [
-            "aws-secure-flow-log-bucket@1.4.3.jsii.tgz"
+            "aws-secure-flow-log-bucket@1.4.4.jsii.tgz"
         ],
         "gammarers.aws_secure_flow_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers/aws_secure_flow_log_bucket/__init__.py` & `gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers/aws_secure_flow_log_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers/aws_secure_flow_log_bucket/_jsii/__init__.py` & `gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers/aws_secure_flow_log_bucket/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import aws_cdk._jsii
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 import gammarers.aws_secure_log_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-secure-flow-log-bucket",
-    "1.4.3",
+    "1.4.4",
     __name__[0:-6],
-    "aws-secure-flow-log-bucket@1.4.3.jsii.tgz",
+    "aws-secure-flow-log-bucket@1.4.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers.aws_secure_flow_log_bucket.egg-info/PKG-INFO` & `gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers.aws_secure_flow_log_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-flow-log-bucket
-Version: 1.4.3
+Version: 1.4.4
 Summary: Specific AWS VPC FlowLog Bucket
 Home-page: https://github.com/gammarers/aws-secure-flow-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-flow-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-flow-log-bucket-1.4.3/src/gammarers.aws_secure_flow_log_bucket.egg-info/SOURCES.txt` & `gammarers.aws-secure-flow-log-bucket-1.4.4/src/gammarers.aws_secure_flow_log_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_secure_flow_log_bucket.egg-info/SOURCES.txt
 src/gammarers.aws_secure_flow_log_bucket.egg-info/dependency_links.txt
 src/gammarers.aws_secure_flow_log_bucket.egg-info/requires.txt
 src/gammarers.aws_secure_flow_log_bucket.egg-info/top_level.txt
 src/gammarers/aws_secure_flow_log_bucket/__init__.py
 src/gammarers/aws_secure_flow_log_bucket/py.typed
 src/gammarers/aws_secure_flow_log_bucket/_jsii/__init__.py
-src/gammarers/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.4.3.jsii.tgz
+src/gammarers/aws_secure_flow_log_bucket/_jsii/aws-secure-flow-log-bucket@1.4.4.jsii.tgz
```

