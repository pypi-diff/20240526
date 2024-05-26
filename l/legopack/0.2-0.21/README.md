# Comparing `tmp/legopack-0.2.tar.gz` & `tmp/legopack-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legopack-0.2.tar", last modified: Sun May 26 16:04:14 2024, max compression
+gzip compressed data, was "legopack-0.21.tar", last modified: Sun May 26 16:22:58 2024, max compression
```

## Comparing `legopack-0.2.tar` & `legopack-0.21.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:04:14.150865 legopack-0.2/
--rw-r--r--   0 zeugy     (1000) users      (100)      182 2024-05-26 16:04:14.150865 legopack-0.2/PKG-INFO
--rw-r--r--   0 zeugy     (1000) users      (100)       29 2024-05-26 14:58:16.000000 legopack-0.2/README.md
-drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:04:14.146865 legopack-0.2/legopack/
--rw-r--r--   0 zeugy     (1000) users      (100)        0 2024-05-26 14:58:16.000000 legopack-0.2/legopack/__init__.py
-drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:04:14.150865 legopack-0.2/legopack/models/
--rw-r--r--   0 zeugy     (1000) users      (100)        0 2024-05-26 14:58:16.000000 legopack-0.2/legopack/models/__init__.py
--rw-r--r--   0 zeugy     (1000) users      (100)     3719 2024-05-26 14:57:11.000000 legopack-0.2/legopack/models/adaptators.py
--rw-r--r--   0 zeugy     (1000) users      (100)    13272 2024-05-26 14:58:16.000000 legopack-0.2/legopack/models/custom.py
--rw-r--r--   0 zeugy     (1000) users      (100)     3907 2024-05-26 14:58:16.000000 legopack-0.2/legopack/tools.py
-drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:04:14.146865 legopack-0.2/legopack.egg-info/
--rw-r--r--   0 zeugy     (1000) users      (100)      182 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/PKG-INFO
--rw-r--r--   0 zeugy     (1000) users      (100)      331 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/SOURCES.txt
--rw-r--r--   0 zeugy     (1000) users      (100)        1 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/dependency_links.txt
--rw-r--r--   0 zeugy     (1000) users      (100)        1 2024-05-26 14:58:16.000000 legopack-0.2/legopack.egg-info/not-zip-safe
--rw-r--r--   0 zeugy     (1000) users      (100)       28 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/requires.txt
--rw-r--r--   0 zeugy     (1000) users      (100)        9 2024-05-26 16:04:14.000000 legopack-0.2/legopack.egg-info/top_level.txt
--rw-r--r--   0 zeugy     (1000) users      (100)       38 2024-05-26 16:04:14.150865 legopack-0.2/setup.cfg
--rw-r--r--   0 zeugy     (1000) users      (100)      628 2024-05-26 16:04:08.000000 legopack-0.2/setup.py
+drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:22:58.734821 legopack-0.21/
+-rw-r--r--   0 zeugy     (1000) users      (100)      183 2024-05-26 16:22:58.730821 legopack-0.21/PKG-INFO
+-rw-r--r--   0 zeugy     (1000) users      (100)       29 2024-05-26 14:58:16.000000 legopack-0.21/README.md
+drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:22:58.730821 legopack-0.21/legopack/
+-rw-r--r--   0 zeugy     (1000) users      (100)        0 2024-05-26 14:58:16.000000 legopack-0.21/legopack/__init__.py
+drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:22:58.730821 legopack-0.21/legopack/models/
+-rw-r--r--   0 zeugy     (1000) users      (100)        0 2024-05-26 14:58:16.000000 legopack-0.21/legopack/models/__init__.py
+-rw-r--r--   0 zeugy     (1000) users      (100)     3719 2024-05-26 14:57:11.000000 legopack-0.21/legopack/models/adaptators.py
+-rw-r--r--   0 zeugy     (1000) users      (100)    13272 2024-05-26 14:58:16.000000 legopack-0.21/legopack/models/custom.py
+-rw-r--r--   0 zeugy     (1000) users      (100)     3907 2024-05-26 14:58:16.000000 legopack-0.21/legopack/tools.py
+drwxr-xr-x   0 zeugy     (1000) users      (100)        0 2024-05-26 16:22:58.730821 legopack-0.21/legopack.egg-info/
+-rw-r--r--   0 zeugy     (1000) users      (100)      183 2024-05-26 16:22:58.000000 legopack-0.21/legopack.egg-info/PKG-INFO
+-rw-r--r--   0 zeugy     (1000) users      (100)      331 2024-05-26 16:22:58.000000 legopack-0.21/legopack.egg-info/SOURCES.txt
+-rw-r--r--   0 zeugy     (1000) users      (100)        1 2024-05-26 16:22:58.000000 legopack-0.21/legopack.egg-info/dependency_links.txt
+-rw-r--r--   0 zeugy     (1000) users      (100)        1 2024-05-26 14:58:16.000000 legopack-0.21/legopack.egg-info/not-zip-safe
+-rw-r--r--   0 zeugy     (1000) users      (100)       28 2024-05-26 16:22:58.000000 legopack-0.21/legopack.egg-info/requires.txt
+-rw-r--r--   0 zeugy     (1000) users      (100)        9 2024-05-26 16:22:58.000000 legopack-0.21/legopack.egg-info/top_level.txt
+-rw-r--r--   0 zeugy     (1000) users      (100)       38 2024-05-26 16:22:58.734821 legopack-0.21/setup.cfg
+-rw-r--r--   0 zeugy     (1000) users      (100)      570 2024-05-26 16:22:56.000000 legopack-0.21/setup.py
```

### Comparing `legopack-0.2/legopack/models/adaptators.py` & `legopack-0.21/legopack/models/adaptators.py`

 * *Files identical despite different names*

### Comparing `legopack-0.2/legopack/models/custom.py` & `legopack-0.21/legopack/models/custom.py`

 * *Files identical despite different names*

### Comparing `legopack-0.2/legopack/tools.py` & `legopack-0.21/legopack/tools.py`

 * *Files identical despite different names*

### Comparing `legopack-0.2/setup.py` & `legopack-0.21/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='legopack',
-    version='0.2',
+    version='0.21',
     author='Remi Prince',
     description='personal',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scikit-learn",
         "streamad"
     ],
     python_requires='>=3.8',
     zip_safe=False
 )
 
-# python3 -m build
-# python3 -m twine upload --repository testpypi dist/*
-
+# pip install .
 # pip install setuptools wheel twine
 # python setup.py sdist bdist_wheel
 # twine check dist/*
 # twine upload dist/* --username __token__
```

