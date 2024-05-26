# Comparing `tmp/almax_common-0.7.0.tar.gz` & `tmp/almax_common-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-0.7.0.tar", last modified: Fri May 24 17:00:39 2024, max compression
+gzip compressed data, was "almax_common-0.8.2.tar", last modified: Sun May 26 21:28:39 2024, max compression
```

## Comparing `almax_common-0.7.0.tar` & `almax_common-0.8.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 almax      (501) staff       (20)        0 2024-05-24 17:00:39.315350 almax_common-0.7.0/
--rw-r--r--   0 almax      (501) staff       (20)      401 2024-05-24 17:00:39.314822 almax_common-0.7.0/PKG-INFO
--rw-r--r--   0 almax      (501) staff       (20)       61 2024-04-17 14:32:05.000000 almax_common-0.7.0/README.md
-drwxr-xr-x   0 almax      (501) staff       (20)        0 2024-05-24 17:00:39.314227 almax_common-0.7.0/almax_common.egg-info/
--rw-r--r--   0 almax      (501) staff       (20)      401 2024-05-24 17:00:39.000000 almax_common-0.7.0/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 almax      (501) staff       (20)      197 2024-05-24 17:00:39.000000 almax_common-0.7.0/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 almax      (501) staff       (20)        1 2024-05-24 17:00:39.000000 almax_common-0.7.0/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 almax      (501) staff       (20)       63 2024-05-24 17:00:39.000000 almax_common-0.7.0/almax_common.egg-info/requires.txt
--rw-r--r--   0 almax      (501) staff       (20)        1 2024-05-24 17:00:39.000000 almax_common-0.7.0/almax_common.egg-info/top_level.txt
--rw-r--r--   0 almax      (501) staff       (20)       38 2024-05-24 17:00:39.315568 almax_common-0.7.0/setup.cfg
--rw-r--r--   0 almax      (501) staff       (20)      528 2024-04-17 23:05:35.000000 almax_common-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:39.911149 almax_common-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-26 21:28:39.911149 almax_common-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 21:28:13.000000 almax_common-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:39.911149 almax_common-0.8.2/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-26 21:28:39.000000 almax_common-0.8.2/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-26 21:28:39.000000 almax_common-0.8.2/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:28:39.000000 almax_common-0.8.2/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-26 21:28:39.000000 almax_common-0.8.2/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:28:39.000000 almax_common-0.8.2/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:28:39.911149 almax_common-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-26 21:28:13.000000 almax_common-0.8.2/setup.py
```

### Comparing `almax_common-0.7.0/setup.py` & `almax_common-0.8.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+with open("requirements.txt") as f:
+    required = f.read().splitlines()
+
 setup(
     name='almax_common',
-    version='0.7.0',
+    version='0.8.2',
     description='A common library with some of my implementations',
     long_description='test',
     long_description_content_type='text/markdown',
     author='AlMax98',
     author_email='alihaider.maqsood@gmail.com',
     packages=find_packages(),
     install_requires=[
```

