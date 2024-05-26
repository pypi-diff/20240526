# Comparing `tmp/gammarers.aws-secure-cloudfront-origin-bucket-1.5.4.tar.gz` & `tmp/gammarers.aws-secure-cloudfront-origin-bucket-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-secure-cloudfront-origin-bucket-1.5.4.tar", last modified: Sun May 19 18:27:38 2024, max compression
+gzip compressed data, was "gammarers.aws-secure-cloudfront-origin-bucket-1.5.5.tar", last modified: Sun May 26 18:27:04 2024, max compression
```

## Comparing `gammarers.aws-secure-cloudfront-origin-bucket-1.5.4.tar` & `gammarers.aws-secure-cloudfront-origin-bucket-1.5.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:38.540949 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 18:27:24.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 18:27:24.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-19 18:27:38.540949 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-19 18:27:24.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-19 18:27:24.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:27:38.540949 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-19 18:27:24.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:38.536949 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:38.536949 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:38.536949 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers/aws_secure_cloudfront_origin_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-05-19 18:27:24.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers/aws_secure_cloudfront_origin_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:38.536949 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-19 18:27:24.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32126 2024-05-19 18:27:24.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.5.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:27:24.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers/aws_secure_cloudfront_origin_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:38.536949 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-19 18:27:38.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-19 18:27:38.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:27:38.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-19 18:27:38.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 18:27:38.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:27:04.028149 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-26 18:26:53.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 18:26:53.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-26 18:27:04.028149 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-26 18:26:53.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-26 18:26:53.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 18:27:04.028149 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-26 18:26:53.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:27:04.028149 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:27:04.028149 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:27:04.028149 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers/aws_secure_cloudfront_origin_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    12287 2024-05-26 18:26:53.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers/aws_secure_cloudfront_origin_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:27:04.028149 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-26 18:26:53.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32126 2024-05-26 18:26:53.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.5.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:26:53.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers/aws_secure_cloudfront_origin_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:27:04.028149 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-26 18:27:03.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-26 18:27:04.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:27:03.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-26 18:27:03.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 18:27:03.000000 gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
```

### Comparing `gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/LICENSE` & `gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/PKG-INFO` & `gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-cloudfront-origin-bucket
-Version: 1.5.4
+Version: 1.5.5
 Summary: AWS CloudFront distribution origin S3 bucket.
 Home-page: https://github.com/gammarers/aws-secure-cloudfront-origin-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-cloudfront-origin-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/README.md` & `gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/setup.py` & `gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-secure-cloudfront-origin-bucket",
-    "version": "1.5.4",
+    "version": "1.5.5",
     "description": "AWS CloudFront distribution origin S3 bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-secure-cloudfront-origin-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_secure_cloudfront_origin_bucket",
         "gammarers.aws_secure_cloudfront_origin_bucket._jsii"
     ],
     "package_data": {
         "gammarers.aws_secure_cloudfront_origin_bucket._jsii": [
-            "aws-secure-cloudfront-origin-bucket@1.5.4.jsii.tgz"
+            "aws-secure-cloudfront-origin-bucket@1.5.5.jsii.tgz"
         ],
         "gammarers.aws_secure_cloudfront_origin_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers/aws_secure_cloudfront_origin_bucket/__init__.py` & `gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers/aws_secure_cloudfront_origin_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py` & `gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-secure-cloudfront-origin-bucket",
-    "1.5.4",
+    "1.5.5",
     __name__[0:-6],
-    "aws-secure-cloudfront-origin-bucket@1.5.4.jsii.tgz",
+    "aws-secure-cloudfront-origin-bucket@1.5.5.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO` & `gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-secure-cloudfront-origin-bucket
-Version: 1.5.4
+Version: 1.5.5
 Summary: AWS CloudFront distribution origin S3 bucket.
 Home-page: https://github.com/gammarers/aws-secure-cloudfront-origin-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-secure-cloudfront-origin-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-secure-cloudfront-origin-bucket-1.5.4/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt` & `gammarers.aws-secure-cloudfront-origin-bucket-1.5.5/src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/SOURCES.txt
 src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/dependency_links.txt
 src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/requires.txt
 src/gammarers.aws_secure_cloudfront_origin_bucket.egg-info/top_level.txt
 src/gammarers/aws_secure_cloudfront_origin_bucket/__init__.py
 src/gammarers/aws_secure_cloudfront_origin_bucket/py.typed
 src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/__init__.py
-src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.5.4.jsii.tgz
+src/gammarers/aws_secure_cloudfront_origin_bucket/_jsii/aws-secure-cloudfront-origin-bucket@1.5.5.jsii.tgz
```

