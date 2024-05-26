# Comparing `tmp/neginver-0.0.5.tar.gz` & `tmp/neginver-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neginver-0.0.5.tar", last modified: Sun May 26 05:41:09 2024, max compression
+gzip compressed data, was "neginver-0.0.6.tar", last modified: Sun May 26 05:46:54 2024, max compression
```

## Comparing `neginver-0.0.5.tar` & `neginver-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-26 05:41:09.282462 neginver-0.0.5/
--rw-r--r--   0 flemyng    (501) staff       (20)     1070 2024-05-25 07:37:37.000000 neginver-0.0.5/LICENSE
--rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-25 07:40:46.000000 neginver-0.0.5/MANIFEST.in
--rw-r--r--   0 flemyng    (501) staff       (20)     5309 2024-05-26 05:41:09.282216 neginver-0.0.5/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)     4676 2024-05-26 04:54:43.000000 neginver-0.0.5/README.md
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-26 05:41:09.281037 neginver-0.0.5/neginver/
--rw-r--r--   0 flemyng    (501) staff       (20)      107 2024-05-25 07:56:15.000000 neginver-0.0.5/neginver/__init__.py
--rw-r--r--   0 flemyng    (501) staff       (20)     2973 2024-05-26 05:36:04.000000 neginver-0.0.5/neginver/image_info.py
--rw-r--r--   0 flemyng    (501) staff       (20)    16085 2024-05-25 10:38:59.000000 neginver-0.0.5/neginver/negative_inversion.py
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-26 05:41:09.281954 neginver-0.0.5/neginver.egg-info/
--rw-r--r--   0 flemyng    (501) staff       (20)     5309 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)      272 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/SOURCES.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/dependency_links.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       39 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/requires.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        9 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/top_level.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-26 05:41:09.282522 neginver-0.0.5/setup.cfg
--rw-r--r--   0 flemyng    (501) staff       (20)      863 2024-05-26 05:39:34.000000 neginver-0.0.5/setup.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-26 05:46:54.142232 neginver-0.0.6/
+-rw-r--r--   0 flemyng    (501) staff       (20)     1070 2024-05-25 07:37:37.000000 neginver-0.0.6/LICENSE
+-rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-25 07:40:46.000000 neginver-0.0.6/MANIFEST.in
+-rw-r--r--   0 flemyng    (501) staff       (20)     5309 2024-05-26 05:46:54.141986 neginver-0.0.6/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)     4676 2024-05-26 04:54:43.000000 neginver-0.0.6/README.md
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-26 05:46:54.140910 neginver-0.0.6/neginver/
+-rw-r--r--   0 flemyng    (501) staff       (20)      107 2024-05-25 07:56:15.000000 neginver-0.0.6/neginver/__init__.py
+-rw-r--r--   0 flemyng    (501) staff       (20)     2941 2024-05-26 05:45:36.000000 neginver-0.0.6/neginver/image_info.py
+-rw-r--r--   0 flemyng    (501) staff       (20)    16085 2024-05-25 10:38:59.000000 neginver-0.0.6/neginver/negative_inversion.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-26 05:46:54.141734 neginver-0.0.6/neginver.egg-info/
+-rw-r--r--   0 flemyng    (501) staff       (20)     5309 2024-05-26 05:46:54.000000 neginver-0.0.6/neginver.egg-info/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)      272 2024-05-26 05:46:54.000000 neginver-0.0.6/neginver.egg-info/SOURCES.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-26 05:46:54.000000 neginver-0.0.6/neginver.egg-info/dependency_links.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       39 2024-05-26 05:46:54.000000 neginver-0.0.6/neginver.egg-info/requires.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        9 2024-05-26 05:46:54.000000 neginver-0.0.6/neginver.egg-info/top_level.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-26 05:46:54.142276 neginver-0.0.6/setup.cfg
+-rw-r--r--   0 flemyng    (501) staff       (20)      863 2024-05-26 05:46:47.000000 neginver-0.0.6/setup.py
```

### Comparing `neginver-0.0.5/LICENSE` & `neginver-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neginver-0.0.5/PKG-INFO` & `neginver-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neginver
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python project for automatic Negative Film inversion
 Home-page: https://github.com/Flemyng1999/neginver
 Author: flemyng feng
 Author-email: flemyng1999@outlook.com
 Keywords: python,negative,film,windows,mac,linux
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neginver-0.0.5/README.md` & `neginver-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `neginver-0.0.5/neginver/image_info.py` & `neginver-0.0.6/neginver/image_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 @Version :   1.0
 @Desc    :   None
 '''
 
 from typing import Union
 
 import numpy as np
-import matplotlib.pyplot as plt
 
 
 def print_array_info(
     img_array: np.ndarray,
 ) -> None:
     '''
     Print the image information.
```

### Comparing `neginver-0.0.5/neginver/negative_inversion.py` & `neginver-0.0.6/neginver/negative_inversion.py`

 * *Files identical despite different names*

### Comparing `neginver-0.0.5/neginver.egg-info/PKG-INFO` & `neginver-0.0.6/neginver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neginver
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python project for automatic Negative Film inversion
 Home-page: https://github.com/Flemyng1999/neginver
 Author: flemyng feng
 Author-email: flemyng1999@outlook.com
 Keywords: python,negative,film,windows,mac,linux
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neginver-0.0.5/setup.py` & `neginver-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 setup(
     name='neginver',
     version=VERSION,
     author='flemyng feng',
     author_email='flemyng1999@outlook.com',
     description='A Python project for automatic Negative Film inversion',
```

