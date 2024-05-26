# Comparing `tmp/neginver-0.0.1.tar.gz` & `tmp/neginver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neginver-0.0.1.tar", last modified: Sat May 25 07:58:45 2024, max compression
+gzip compressed data, was "neginver-0.0.2.tar", last modified: Sat May 25 10:47:10 2024, max compression
```

## Comparing `neginver-0.0.1.tar` & `neginver-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-25 07:58:45.760761 neginver-0.0.1/
--rw-r--r--   0 flemyng    (501) staff       (20)     1070 2024-05-25 07:37:37.000000 neginver-0.0.1/LICENSE
--rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-25 07:40:46.000000 neginver-0.0.1/MANIFEST.in
--rw-r--r--   0 flemyng    (501) staff       (20)      621 2024-05-25 07:58:45.760621 neginver-0.0.1/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)      102 2024-05-25 07:37:37.000000 neginver-0.0.1/README.md
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-25 07:58:45.759684 neginver-0.0.1/neginver/
--rw-r--r--   0 flemyng    (501) staff       (20)      107 2024-05-25 07:56:15.000000 neginver-0.0.1/neginver/__init__.py
--rw-r--r--   0 flemyng    (501) staff       (20)     3140 2024-05-25 07:56:10.000000 neginver-0.0.1/neginver/image_info.py
--rw-r--r--   0 flemyng    (501) staff       (20)    14935 2024-05-25 07:52:51.000000 neginver-0.0.1/neginver/negative_inversion.py
-drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-25 07:58:45.760423 neginver-0.0.1/neginver.egg-info/
--rw-r--r--   0 flemyng    (501) staff       (20)      621 2024-05-25 07:58:45.000000 neginver-0.0.1/neginver.egg-info/PKG-INFO
--rw-r--r--   0 flemyng    (501) staff       (20)      272 2024-05-25 07:58:45.000000 neginver-0.0.1/neginver.egg-info/SOURCES.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-25 07:58:45.000000 neginver-0.0.1/neginver.egg-info/dependency_links.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       39 2024-05-25 07:58:45.000000 neginver-0.0.1/neginver.egg-info/requires.txt
--rw-r--r--   0 flemyng    (501) staff       (20)        9 2024-05-25 07:58:45.000000 neginver-0.0.1/neginver.egg-info/top_level.txt
--rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-25 07:58:45.760810 neginver-0.0.1/setup.cfg
--rw-r--r--   0 flemyng    (501) staff       (20)      863 2024-05-25 07:45:42.000000 neginver-0.0.1/setup.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-25 10:47:10.766480 neginver-0.0.2/
+-rw-r--r--   0 flemyng    (501) staff       (20)     1070 2024-05-25 07:37:37.000000 neginver-0.0.2/LICENSE
+-rw-r--r--   0 flemyng    (501) staff       (20)       34 2024-05-25 07:40:46.000000 neginver-0.0.2/MANIFEST.in
+-rw-r--r--   0 flemyng    (501) staff       (20)     5168 2024-05-25 10:47:10.766227 neginver-0.0.2/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)     4535 2024-05-25 10:43:22.000000 neginver-0.0.2/README.md
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-25 10:47:10.765260 neginver-0.0.2/neginver/
+-rw-r--r--   0 flemyng    (501) staff       (20)      107 2024-05-25 07:56:15.000000 neginver-0.0.2/neginver/__init__.py
+-rw-r--r--   0 flemyng    (501) staff       (20)     3140 2024-05-25 07:56:10.000000 neginver-0.0.2/neginver/image_info.py
+-rw-r--r--   0 flemyng    (501) staff       (20)    16085 2024-05-25 10:38:59.000000 neginver-0.0.2/neginver/negative_inversion.py
+drwxr-xr-x   0 flemyng    (501) staff       (20)        0 2024-05-25 10:47:10.766009 neginver-0.0.2/neginver.egg-info/
+-rw-r--r--   0 flemyng    (501) staff       (20)     5168 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/PKG-INFO
+-rw-r--r--   0 flemyng    (501) staff       (20)      272 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/SOURCES.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        1 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/dependency_links.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       39 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/requires.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)        9 2024-05-25 10:47:10.000000 neginver-0.0.2/neginver.egg-info/top_level.txt
+-rw-r--r--   0 flemyng    (501) staff       (20)       38 2024-05-25 10:47:10.766524 neginver-0.0.2/setup.cfg
+-rw-r--r--   0 flemyng    (501) staff       (20)      863 2024-05-25 10:44:25.000000 neginver-0.0.2/setup.py
```

### Comparing `neginver-0.0.1/LICENSE` & `neginver-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neginver-0.0.1/neginver/image_info.py` & `neginver-0.0.2/neginver/image_info.py`

 * *Files identical despite different names*

### Comparing `neginver-0.0.1/neginver/negative_inversion.py` & `neginver-0.0.2/neginver/negative_inversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 '''
 @File    :   negative_reverse.py
 @Time    :   2024/05/24 21:38:02
 @Author  :   Flemyng 
 @Version :   1.0
-@Desc    :   Negative film image inverse
+@Desc    :   Negative image inverse
 '''
 import os
 from pathlib import Path
 from typing import Union
 from datetime import datetime
 
 import numpy as np
@@ -456,43 +456,74 @@
 
 
 def negative_inverse(
     img: np.ndarray,
     film_type: str = 'color', # 'color', 'bw'
     mode: str = 'default',
     rates: tuple[float] = (1.195, 1.155),
+    percentile: float = 0.1,
+    crop_percentage: float = 0.02,
 ) -> np.ndarray:
     '''
     Convert the negative image to positive image
 
     :param img: np.ndarray, The negative image to convert.
-    :param film_type: str, The type of the film.
-    :param mode: str, The mode of the conversion.
-    :param rates: tuple[float], The control points rates.
-    '''
-    # Check the shape of the image
-    if img.shape[0] != 3:
-        raise ValueError(
-            "The image array's shape must be [3, height, width] or [1, height, width]!"
-        )
-    else:
+    :param film_type: str, The type of the film, 'color' or 'bw'.
+    :param mode: str, The mode of the conversion, 'auto', 'default' or 'manual'.
+    :param rates: tuple[float], The control points rate.
+    :param percentile: float, The percentile of the histogram to cut.
+    :param crop_percentage: float, The percentage of the black side to crop.
+    :return: np.ndarray, The positive image.
+    '''
+    # Check the img shape
+    if img.shape[0] == 3:
         pass
+    else:
+        raise ValueError('Invalid image shape, must be [3, height, width]!')
 
     # Check the film type
     if film_type == 'color':
         if mode == 'auto':
-            return color_inverse(img, auto_rates=True)
+            return color_inverse(
+                img,
+                auto_rates=True,
+                percentile=percentile,
+                crop_percentage=crop_percentage
+            )
         elif mode == 'default':
-            return color_inverse(img, rates=(1.195, 1.155))
+            return color_inverse(
+                img,
+                rates=(1.195, 1.155),
+                percentile=percentile,
+                crop_percentage=crop_percentage
+            )
         elif mode == 'manual':
-            return color_inverse(img, rates=rates)
+            if rates == (1.195, 1.155):
+                print('The default rates are (1.195, 1.155), you can change it by setting the rates parameter.')
+                return color_inverse(
+                    img,
+                    rates=rates,
+                    percentile=percentile,
+                    crop_percentage=crop_percentage
+                )
+            else:
+                return color_inverse(
+                    img,
+                    rates=rates,
+                    percentile=percentile,
+                    crop_percentage=crop_percentage
+                )
         else:
             raise ValueError('Invalid mode, must be "auto", "default" or "manual"!')
     elif film_type == 'bw':
-        return bw_inverse(img)
+        return bw_inverse(
+            img,
+            percentile=percentile,
+            crop_percentage=crop_percentage
+        )
     else:
         raise ValueError('Invalid film type, must be "color" or "bw"!')
 
 
 if __name__ == "__main__":
     # Directory path
     data_dir = Path('/Users/flemyng/Desktop/Phocus/2024_05_24')
```

### Comparing `neginver-0.0.1/setup.py` & `neginver-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 setup(
     name='neginver',
     version=VERSION,
     author='flemyng feng',
     author_email='flemyng1999@outlook.com',
     description='A Python project for automatic Negative Film inversion',
```

