# Comparing `tmp/neginver-0.0.2.tar.gz` & `tmp/neginver-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neginver-0.0.2.tar", last modified: Sat May 25 10:47:10 2024, max compression
+gzip compressed data, was "neginver-0.0.5.tar", last modified: Sun May 26 05:41:09 2024, max compression
```

## Comparing `neginver-0.0.2.tar` & `neginver-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-25 10:47:10.766480 neginver-0.0.2/
--rw-r--r--   0 flemyng    (501) staff       (20)     1070 2024-05-25 07:37:37.000000 neginver-0.0.2/LICENSE
--rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-25 07:40:46.000000 neginver-0.0.2/MANIFEST.in
--rw-r--r--   0 flemyng    (501) staff       (20)     5168 2024-05-25 10:47:10.766227 neginver-0.0.2/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)     4535 2024-05-25 10:43:22.000000 neginver-0.0.2/README.md
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-25 10:47:10.765260 neginver-0.0.2/neginver/
--rw-r--r--   0 flemyng    (501) staff       (20)      107 2024-05-25 07:56:15.000000 neginver-0.0.2/neginver/__init__.py
--rw-r--r--   0 flemyng    (501) staff       (20)     3140 2024-05-25 07:56:10.000000 neginver-0.0.2/neginver/image_info.py
--rw-r--r--   0 flemyng    (501) staff       (20)    16085 2024-05-25 10:38:59.000000 neginver-0.0.2/neginver/negative_inversion.py
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-25 10:47:10.766009 neginver-0.0.2/neginver.egg-info/
--rw-r--r--   0 flemyng    (501) staff       (20)     5168 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)      272 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/SOURCES.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/dependency_links.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       39 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/requires.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        9 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/top_level.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-25 10:47:10.766524 neginver-0.0.2/setup.cfg
--rw-r--r--   0 flemyng    (501) staff       (20)      863 2024-05-25 10:44:25.000000 neginver-0.0.2/setup.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-26 05:41:09.282462 neginver-0.0.5/
+-rw-r--r--   0 flemyng    (501) staff       (20)     1070 2024-05-25 07:37:37.000000 neginver-0.0.5/LICENSE
+-rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-25 07:40:46.000000 neginver-0.0.5/MANIFEST.in
+-rw-r--r--   0 flemyng    (501) staff       (20)     5309 2024-05-26 05:41:09.282216 neginver-0.0.5/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)     4676 2024-05-26 04:54:43.000000 neginver-0.0.5/README.md
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-26 05:41:09.281037 neginver-0.0.5/neginver/
+-rw-r--r--   0 flemyng    (501) staff       (20)      107 2024-05-25 07:56:15.000000 neginver-0.0.5/neginver/__init__.py
+-rw-r--r--   0 flemyng    (501) staff       (20)     2973 2024-05-26 05:36:04.000000 neginver-0.0.5/neginver/image_info.py
+-rw-r--r--   0 flemyng    (501) staff       (20)    16085 2024-05-25 10:38:59.000000 neginver-0.0.5/neginver/negative_inversion.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-26 05:41:09.281954 neginver-0.0.5/neginver.egg-info/
+-rw-r--r--   0 flemyng    (501) staff       (20)     5309 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)      272 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/SOURCES.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/dependency_links.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       39 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/requires.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        9 2024-05-26 05:41:09.000000 neginver-0.0.5/neginver.egg-info/top_level.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-26 05:41:09.282522 neginver-0.0.5/setup.cfg
+-rw-r--r--   0 flemyng    (501) staff       (20)      863 2024-05-26 05:39:34.000000 neginver-0.0.5/setup.py
```

### Comparing `neginver-0.0.2/LICENSE` & `neginver-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neginver-0.0.2/neginver/image_info.py` & `neginver-0.0.5/neginver/image_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 @Author  :   Flemyng 
 @Version :   1.0
 @Desc    :   None
 '''
 
 from typing import Union
 
-import geotifflib as gt
 import numpy as np
 import matplotlib.pyplot as plt
 
 
 def print_array_info(
     img_array: np.ndarray,
 ) -> None:
@@ -106,16 +105,7 @@
     # Plot the histogram
     plot_rgb_hist(image, axes[1])
 
     if image.dtype == np.uint16:
         axes[1].set_xlim([0, 65535])
     elif image.dtype == np.uint8:
         axes[1].set_xlim([0, 255])
-
-
-if __name__ == '__main__':
-    img_test = gt.read(tif_files[1])
-
-    print_info(img_test)
-
-    # Plot the image
-    plot_image_info(img_test)
```

### Comparing `neginver-0.0.2/neginver/negative_inversion.py` & `neginver-0.0.5/neginver/negative_inversion.py`

 * *Files identical despite different names*

### Comparing `neginver-0.0.2/setup.py` & `neginver-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.5'
 
 setup(
     name='neginver',
     version=VERSION,
     author='flemyng feng',
     author_email='flemyng1999@outlook.com',
     description='A Python project for automatic Negative Film inversion',
```

