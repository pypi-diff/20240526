# Comparing `tmp/mnists-0.2.0rc1.tar.gz` & `tmp/mnists-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnists-0.2.0rc1.tar", last modified: Mon May  6 10:56:35 2024, max compression
+gzip compressed data, was "mnists-0.2.1.tar", last modified: Sun May 26 14:56:50 2024, max compression
```

## Comparing `mnists-0.2.0rc1.tar` & `mnists-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pczarnik (4214435) pczarnik (4214435)        0 2024-05-06 10:56:35.389177 mnists-0.2.0rc1/
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     1070 2024-05-03 18:18:09.000000 mnists-0.2.0rc1/LICENSE
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2995 2024-05-06 10:56:35.388177 mnists-0.2.0rc1/PKG-INFO
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2158 2024-05-06 10:29:42.000000 mnists-0.2.0rc1/README.md
-drwxr-xr-x   0 pczarnik (4214435) pczarnik (4214435)        0 2024-05-06 10:56:35.386177 mnists-0.2.0rc1/mnists/
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)      112 2024-05-06 10:55:35.000000 mnists-0.2.0rc1/mnists/__init__.py
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     8410 2024-05-06 10:53:51.000000 mnists-0.2.0rc1/mnists/_mnist.py
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2594 2024-05-03 18:18:09.000000 mnists-0.2.0rc1/mnists/utils.py
-drwxr-xr-x   0 pczarnik (4214435) pczarnik (4214435)        0 2024-05-06 10:56:35.387177 mnists-0.2.0rc1/mnists.egg-info/
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)     2995 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/PKG-INFO
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)      233 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/SOURCES.txt
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)        1 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/dependency_links.txt
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)       98 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/requires.txt
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)        7 2024-05-06 10:56:35.000000 mnists-0.2.0rc1/mnists.egg-info/top_level.txt
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)      999 2024-05-03 21:57:43.000000 mnists-0.2.0rc1/pyproject.toml
--rw-r--r--   0 pczarnik (4214435) pczarnik (4214435)       38 2024-05-06 10:56:35.389177 mnists-0.2.0rc1/setup.cfg
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-26 14:56:50.369155 mnists-0.2.1/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1070 2024-05-26 12:44:53.000000 mnists-0.2.1/LICENSE
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     2992 2024-05-26 14:56:50.368155 mnists-0.2.1/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     2158 2024-05-26 12:44:53.000000 mnists-0.2.1/README.md
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-26 14:56:50.367155 mnists-0.2.1/mnists/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      109 2024-05-26 14:54:28.000000 mnists-0.2.1/mnists/__init__.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     8473 2024-05-26 14:48:34.000000 mnists-0.2.1/mnists/_mnist.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     2594 2024-05-26 14:46:48.000000 mnists-0.2.1/mnists/utils.py
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-26 14:56:50.368155 mnists-0.2.1/mnists.egg-info/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     2992 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      233 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/SOURCES.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        1 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/dependency_links.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       98 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/requires.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        7 2024-05-26 14:56:50.000000 mnists-0.2.1/mnists.egg-info/top_level.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      999 2024-05-26 12:44:53.000000 mnists-0.2.1/pyproject.toml
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       38 2024-05-26 14:56:50.369155 mnists-0.2.1/setup.cfg
```

### Comparing `mnists-0.2.0rc1/LICENSE` & `mnists-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mnists-0.2.0rc1/PKG-INFO` & `mnists-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnists
-Version: 0.2.0rc1
+Version: 0.2.1
 Summary: MNISTs: All MNIST-like datasets in one package
 Author-email: Piotr Czarnik <ptr.czarnik@gmail.com>
 Project-URL: Homepage, https://github.com/pczarnik/mnists
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `mnists-0.2.0rc1/README.md` & `mnists-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mnists-0.2.0rc1/mnists/_mnist.py` & `mnists-0.2.1/mnists/_mnist.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         "6 - six",
         "7 - seven",
         "8 - eight",
         "9 - nine",
     ]
 
     mirrors = [
+        "https://storage.googleapis.com/cvdf-datasets/mnist/",
         "https://ossci-datasets.s3.amazonaws.com/mnist/",
         "http://yann.lecun.com/exdb/mnist/",
     ]
 
     resources = {
         "train_images": (
             "train-images-idx3-ubyte.gz",
```

### Comparing `mnists-0.2.0rc1/mnists/utils.py` & `mnists-0.2.1/mnists/utils.py`

 * *Files identical despite different names*

### Comparing `mnists-0.2.0rc1/mnists.egg-info/PKG-INFO` & `mnists-0.2.1/mnists.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnists
-Version: 0.2.0rc1
+Version: 0.2.1
 Summary: MNISTs: All MNIST-like datasets in one package
 Author-email: Piotr Czarnik <ptr.czarnik@gmail.com>
 Project-URL: Homepage, https://github.com/pczarnik/mnists
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `mnists-0.2.0rc1/pyproject.toml` & `mnists-0.2.1/pyproject.toml`

 * *Files identical despite different names*

