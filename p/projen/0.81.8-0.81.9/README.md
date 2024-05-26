# Comparing `tmp/projen-0.81.8.tar.gz` & `tmp/projen-0.81.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.81.8.tar", last modified: Wed May  8 12:27:46 2024, max compression
+gzip compressed data, was "projen-0.81.9.tar", last modified: Fri May 10 08:52:21 2024, max compression
```

## Comparing `projen-0.81.8.tar` & `projen-0.81.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.633467 projen-0.81.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 12:27:34.000000 projen-0.81.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 12:27:34.000000 projen-0.81.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-08 12:27:46.629467 projen-0.81.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-05-08 12:27:34.000000 projen-0.81.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 12:27:34.000000 projen-0.81.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 12:27:46.633467 projen-0.81.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-08 12:27:34.000000 projen-0.81.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.613467 projen-0.81.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.617467 projen-0.81.8/src/projen/
--rw-r--r--   0 runner    (1001) docker     (127)   653632 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.617467 projen-0.81.8/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.621467 projen-0.81.8/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (127)  2641224 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/_jsii/projen@0.81.8.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.621467 projen-0.81.8/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.621467 projen-0.81.8/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.621467 projen-0.81.8/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.625467 projen-0.81.8/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.625467 projen-0.81.8/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.625467 projen-0.81.8/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.625467 projen-0.81.8/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (127)   409613 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.625467 projen-0.81.8/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.625467 projen-0.81.8/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)   202810 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.625467 projen-0.81.8/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.625467 projen-0.81.8/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)   844523 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.629467 projen-0.81.8/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.629467 projen-0.81.8/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.629467 projen-0.81.8/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.629467 projen-0.81.8/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.629467 projen-0.81.8/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-05-08 12:27:34.000000 projen-0.81.8/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:27:46.617467 projen-0.81.8/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-08 12:27:46.000000 projen-0.81.8/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-08 12:27:46.000000 projen-0.81.8/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:27:46.000000 projen-0.81.8/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-08 12:27:46.000000 projen-0.81.8/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 12:27:46.000000 projen-0.81.8/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.862256 projen-0.81.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-10 08:52:11.000000 projen-0.81.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 08:52:11.000000 projen-0.81.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-10 08:52:21.862256 projen-0.81.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    78674 2024-05-10 08:52:11.000000 projen-0.81.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 08:52:11.000000 projen-0.81.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:52:21.862256 projen-0.81.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-10 08:52:11.000000 projen-0.81.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.842256 projen-0.81.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.846256 projen-0.81.9/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (127)   653934 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.846256 projen-0.81.9/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.850256 projen-0.81.9/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (127)  2641567 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/_jsii/projen@0.81.9.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.850256 projen-0.81.9/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (127)  1079302 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.850256 projen-0.81.9/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    52320 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)   510147 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (127)   597384 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (127)   224466 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)    75913 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (127)   409613 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)   250737 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)   202810 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.854256 projen-0.81.9/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (127)   183709 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)   844523 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (127)   213158 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (127)   285447 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (127)   474506 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)    69040 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.858256 projen-0.81.9/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (127)   797444 2024-05-10 08:52:11.000000 projen-0.81.9/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:52:21.846256 projen-0.81.9/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    79503 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 08:52:21.000000 projen-0.81.9/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.81.8/LICENSE` & `projen-0.81.9/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/PKG-INFO` & `projen-0.81.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.8
+Version: 0.81.9
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.8/README.md` & `projen-0.81.9/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/setup.py` & `projen-0.81.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.81.8",
+    "version": "0.81.9",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.81.8.jsii.tgz"
+            "projen@0.81.9.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `projen-0.81.8/src/projen/__init__.py` & `projen-0.81.9/src/projen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1296,15 +1296,15 @@
         name_suffix: typing.Optional[builtins.str] = None,
         schema_version: typing.Optional[builtins.str] = None,
         services: typing.Optional[typing.Mapping[builtins.str, typing.Union["DockerComposeServiceDescription", typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
         :param project: -
         :param name_suffix: (experimental) A name to add to the docker-compose.yml filename. Default: - no name is added
-        :param schema_version: (experimental) Docker Compose schema version do be used. Default: 3.3
+        :param schema_version: (deprecated) Docker Compose schema version do be used. Default: - no version is provided
         :param services: (experimental) Service descriptions.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__befd8e58ddccbbc1a83afe6a4e464b7951ad377df97c7553777909a18eefec9a)
             check_type(argname="argument project", value=project, expected_type=type_hints["project"])
@@ -1986,15 +1986,15 @@
         name_suffix: typing.Optional[builtins.str] = None,
         schema_version: typing.Optional[builtins.str] = None,
         services: typing.Optional[typing.Mapping[builtins.str, typing.Union["DockerComposeServiceDescription", typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''(experimental) Props for DockerCompose.
 
         :param name_suffix: (experimental) A name to add to the docker-compose.yml filename. Default: - no name is added
-        :param schema_version: (experimental) Docker Compose schema version do be used. Default: 3.3
+        :param schema_version: (deprecated) Docker Compose schema version do be used. Default: - no version is provided
         :param services: (experimental) Service descriptions.
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__04b3a9f497a8a34deecb2bf90e8650e81e98e0a4a6480a090f371e2d60385583)
             check_type(argname="argument name_suffix", value=name_suffix, expected_type=type_hints["name_suffix"])
@@ -2021,19 +2021,24 @@
             'myname' yields 'docker-compose.myname.yml'
         '''
         result = self._values.get("name_suffix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def schema_version(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Docker Compose schema version do be used.
+        '''(deprecated) Docker Compose schema version do be used.
 
-        :default: 3.3
+        :default: - no version is provided
 
-        :stability: experimental
+        :deprecated:
+
+        - The top level ``version`` field is obsolete per the Compose Specification.
+        {@link https://github.com/compose-spec/compose-spec/blob/master/spec.md#version-and-name-top-level-elements Compose Specification}
+
+        :stability: deprecated
         '''
         result = self._values.get("schema_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def services(
         self,
```

### Comparing `projen-0.81.8/src/projen/awscdk/__init__.py` & `projen-0.81.9/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/build/__init__.py` & `projen-0.81.9/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/cdk/__init__.py` & `projen-0.81.9/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/cdk8s/__init__.py` & `projen-0.81.9/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/cdktf/__init__.py` & `projen-0.81.9/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/circleci/__init__.py` & `projen-0.81.9/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/github/__init__.py` & `projen-0.81.9/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/github/workflows/__init__.py` & `projen-0.81.9/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/gitlab/__init__.py` & `projen-0.81.9/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/java/__init__.py` & `projen-0.81.9/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/javascript/__init__.py` & `projen-0.81.9/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/python/__init__.py` & `projen-0.81.9/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/release/__init__.py` & `projen-0.81.9/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/typescript/__init__.py` & `projen-0.81.9/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/vscode/__init__.py` & `projen-0.81.9/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen/web/__init__.py` & `projen-0.81.9/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.81.8/src/projen.egg-info/PKG-INFO` & `projen-0.81.9/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.81.8
+Version: 0.81.9
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.81.8/src/projen.egg-info/SOURCES.txt` & `projen-0.81.9/src/projen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.81.8.jsii.tgz
+src/projen/_jsii/projen@0.81.9.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

