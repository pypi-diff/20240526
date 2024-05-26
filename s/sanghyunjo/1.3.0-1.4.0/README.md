# Comparing `tmp/sanghyunjo-1.3.0.tar.gz` & `tmp/sanghyunjo-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sanghyunjo-1.3.0.tar", last modified: Tue May 21 03:47:10 2024, max compression
+gzip compressed data, was "dist\sanghyunjo-1.4.0.tar", last modified: Sun May 26 14:11:15 2024, max compression
```

## Comparing `sanghyunjo-1.3.0.tar` & `sanghyunjo-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 03:47:10.618899 sanghyunjo-1.3.0/
--rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.3.0/LICENSE
--rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      365 2024-05-21 03:47:10.617901 sanghyunjo-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-05-16 07:32:26.000000 sanghyunjo-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 03:47:10.603341 sanghyunjo-1.3.0/sanghyunjo/
--rw-rw-rw-   0        0        0      194 2024-05-21 03:17:40.000000 sanghyunjo-1.3.0/sanghyunjo/__init__.py
--rw-rw-rw-   0        0        0     9233 2024-05-21 03:47:01.000000 sanghyunjo-1.3.0/sanghyunjo/cv_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 03:47:10.609535 sanghyunjo-1.3.0/sanghyunjo/fonts/
--rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.3.0/sanghyunjo/fonts/Times New Roman MT Std.otf
--rw-rw-rw-   0        0        0      358 2024-05-20 07:08:56.000000 sanghyunjo-1.3.0/sanghyunjo/json_utils.py
--rw-rw-rw-   0        0        0     3046 2024-05-21 01:07:13.000000 sanghyunjo-1.3.0/sanghyunjo/misc.py
-drwxrwxrwx   0        0        0        0 2024-05-21 03:47:10.609535 sanghyunjo-1.3.0/sanghyunjo.egg-info/
--rw-rw-rw-   0        0        0      365 2024-05-21 03:47:10.000000 sanghyunjo-1.3.0/sanghyunjo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2024-05-21 03:47:10.000000 sanghyunjo-1.3.0/sanghyunjo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 03:47:10.000000 sanghyunjo-1.3.0/sanghyunjo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.3.0/sanghyunjo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-21 03:47:10.000000 sanghyunjo-1.3.0/sanghyunjo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 03:47:10.618899 sanghyunjo-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-20 07:09:32.000000 sanghyunjo-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:15.282432 sanghyunjo-1.4.0/
+-rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      365 2024-05-26 14:11:15.280440 sanghyunjo-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-05-16 07:32:26.000000 sanghyunjo-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:15.260482 sanghyunjo-1.4.0/sanghyunjo/
+-rw-rw-rw-   0        0        0      194 2024-05-25 14:39:10.000000 sanghyunjo-1.4.0/sanghyunjo/__init__.py
+-rw-rw-rw-   0        0        0     9318 2024-05-22 06:49:06.000000 sanghyunjo-1.4.0/sanghyunjo/cv_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:15.278441 sanghyunjo-1.4.0/sanghyunjo/fonts/
+-rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.4.0/sanghyunjo/fonts/Times New Roman MT Std.otf
+-rw-rw-rw-   0        0        0      358 2024-05-20 07:08:56.000000 sanghyunjo-1.4.0/sanghyunjo/json_utils.py
+-rw-rw-rw-   0        0        0     3100 2024-05-26 14:10:42.000000 sanghyunjo-1.4.0/sanghyunjo/misc.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:15.280440 sanghyunjo-1.4.0/sanghyunjo.egg-info/
+-rw-rw-rw-   0        0        0      365 2024-05-26 14:11:14.000000 sanghyunjo-1.4.0/sanghyunjo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-05-26 14:11:15.000000 sanghyunjo-1.4.0/sanghyunjo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:11:14.000000 sanghyunjo-1.4.0/sanghyunjo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.4.0/sanghyunjo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-26 14:11:14.000000 sanghyunjo-1.4.0/sanghyunjo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:11:15.282432 sanghyunjo-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-20 07:09:32.000000 sanghyunjo-1.4.0/setup.py
```

### Comparing `sanghyunjo-1.3.0/LICENSE` & `sanghyunjo-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.3.0/README.md` & `sanghyunjo-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.3.0/sanghyunjo/cv_utils.py` & `sanghyunjo-1.4.0/sanghyunjo/cv_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import os
 import cv2
 import cmapy
 import numpy as np
 
 from PIL import ImageFont, ImageDraw, Image
 
+Image.MAX_IMAGE_PIXELS = None # to read unlimited pixels like a large tiff format
+
 ESC = 27
 SPACE = 32
 PLUS = ord('+')
 MINUS = ord('-')
 
 class MouseEventHandler:
     def __init__(self): self.clear()
```

### Comparing `sanghyunjo-1.3.0/sanghyunjo/fonts/Times New Roman MT Std.otf` & `sanghyunjo-1.4.0/sanghyunjo/fonts/Times New Roman MT Std.otf`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.3.0/sanghyunjo/misc.py` & `sanghyunjo-1.4.0/sanghyunjo/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 
 def parallel(fn, data_list, n_jobs=cpus(), show=False):
     print_dict = {}
     if show: print_dict = {'verbose': 10, 'pre_dispatch': 'all'}
 
     return Parallel(n_jobs, **print_dict)([delayed(fn)(*data) for data in data_list])
 
+def strfmt(fmt='%5s', v='True'):
+    return fmt%v
+
 class Timer:
     def __init__(self):
         self.start = time.time()
 
     def __enter__(self):
         self.start = time.time()
         return self
```

### Comparing `sanghyunjo-1.3.0/setup.py` & `sanghyunjo-1.4.0/setup.py`

 * *Files identical despite different names*

