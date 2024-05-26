# Comparing `tmp/c64img-3.2.tar.gz` & `tmp/c64img-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c64img-3.2.tar", last modified: Sat May 25 14:41:25 2024, max compression
+gzip compressed data, was "c64img-3.5.tar", last modified: Sun May 26 16:00:27 2024, max compression
```

## Comparing `c64img-3.2.tar` & `c64img-3.5.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/
--rw-r--r--   0 gryf      (1000) gryf      (1000)     1528 2024-05-25 14:40:46.000000 c64img-3.2/LICENSE
--rw-r--r--   0 gryf      (1000) gryf      (1000)       19 2024-05-25 14:40:46.000000 c64img-3.2/MANIFEST.in
--rw-r--r--   0 gryf      (1000) gryf      (1000)     7974 2024-05-25 14:41:25.814042 c64img-3.2/PKG-INFO
--rw-r--r--   0 gryf      (1000) gryf      (1000)     7014 2024-05-25 14:40:46.000000 c64img-3.2/README.rst
-drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/c64img/
--rw-r--r--   0 gryf      (1000) gryf      (1000)       20 2024-05-25 14:40:46.000000 c64img-3.2/c64img/__init__.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)    18012 2024-05-25 14:40:46.000000 c64img-3.2/c64img/base.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)     5044 2024-05-25 14:40:46.000000 c64img-3.2/c64img/cmd_convert.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)     5542 2024-05-25 14:40:46.000000 c64img-3.2/c64img/hires.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)     1545 2024-05-25 14:40:46.000000 c64img-3.2/c64img/logger.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)    11505 2024-05-25 14:40:46.000000 c64img-3.2/c64img/multi.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)      503 2024-05-25 14:40:46.000000 c64img-3.2/c64img/path.py
-drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/c64img.egg-info/
--rw-r--r--   0 gryf      (1000) gryf      (1000)     7974 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/PKG-INFO
--rw-r--r--   0 gryf      (1000) gryf      (1000)      447 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/SOURCES.txt
--rw-r--r--   0 gryf      (1000) gryf      (1000)        1 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/dependency_links.txt
--rw-r--r--   0 gryf      (1000) gryf      (1000)        7 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/requires.txt
--rw-r--r--   0 gryf      (1000) gryf      (1000)        7 2024-05-25 14:41:25.000000 c64img-3.2/c64img.egg-info/top_level.txt
-drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/scripts/
--rwxr-xr-x   0 gryf      (1000) gryf      (1000)      123 2024-05-25 14:40:46.000000 c64img-3.2/scripts/image2c64
--rw-r--r--   0 gryf      (1000) gryf      (1000)       38 2024-05-25 14:41:25.814042 c64img-3.2/setup.cfg
--rwxr-xr-x   0 gryf      (1000) gryf      (1000)     1449 2024-05-25 14:40:46.000000 c64img-3.2/setup.py
-drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-25 14:41:25.814042 c64img-3.2/tests/
--rw-r--r--   0 gryf      (1000) gryf      (1000)    18171 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_base.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)     7578 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_convert.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)    11119 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_hires.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)     2508 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_logger.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)    16490 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_multi.py
--rw-r--r--   0 gryf      (1000) gryf      (1000)      871 2024-05-25 14:40:46.000000 c64img-3.2/tests/test_path.py
+drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-26 16:00:27.642038 c64img-3.5/
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     1528 2024-05-26 16:00:20.000000 c64img-3.5/LICENSE
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     8053 2024-05-26 16:00:27.642038 c64img-3.5/PKG-INFO
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     7001 2024-05-26 16:00:20.000000 c64img-3.5/README.rst
+drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-26 16:00:27.638038 c64img-3.5/c64img/
+-rw-r--r--   0 gryf      (1000) gryf      (1000)       20 2024-05-26 16:00:20.000000 c64img-3.5/c64img/__init__.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    17994 2024-05-26 16:00:20.000000 c64img-3.5/c64img/base.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     4946 2024-05-26 16:00:20.000000 c64img-3.5/c64img/cmd_convert.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     5542 2024-05-26 16:00:20.000000 c64img-3.5/c64img/hires.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     1537 2024-05-26 16:00:20.000000 c64img-3.5/c64img/logger.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    11505 2024-05-26 16:00:20.000000 c64img-3.5/c64img/multi.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)      503 2024-05-26 16:00:20.000000 c64img-3.5/c64img/path.py
+drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-26 16:00:27.642038 c64img-3.5/c64img.egg-info/
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     8053 2024-05-26 16:00:27.000000 c64img-3.5/c64img.egg-info/PKG-INFO
+-rw-r--r--   0 gryf      (1000) gryf      (1000)      456 2024-05-26 16:00:27.000000 c64img-3.5/c64img.egg-info/SOURCES.txt
+-rw-r--r--   0 gryf      (1000) gryf      (1000)        1 2024-05-26 16:00:27.000000 c64img-3.5/c64img.egg-info/dependency_links.txt
+-rw-r--r--   0 gryf      (1000) gryf      (1000)       59 2024-05-26 16:00:27.000000 c64img-3.5/c64img.egg-info/entry_points.txt
+-rw-r--r--   0 gryf      (1000) gryf      (1000)       15 2024-05-26 16:00:27.000000 c64img-3.5/c64img.egg-info/requires.txt
+-rw-r--r--   0 gryf      (1000) gryf      (1000)        7 2024-05-26 16:00:27.000000 c64img-3.5/c64img.egg-info/top_level.txt
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     1355 2024-05-26 16:00:20.000000 c64img-3.5/pyproject.toml
+-rw-r--r--   0 gryf      (1000) gryf      (1000)       38 2024-05-26 16:00:27.642038 c64img-3.5/setup.cfg
+drwxr-xr-x   0 gryf      (1000) gryf      (1000)        0 2024-05-26 16:00:27.642038 c64img-3.5/tests/
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    18155 2024-05-26 16:00:20.000000 c64img-3.5/tests/test_base.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     7546 2024-05-26 16:00:20.000000 c64img-3.5/tests/test_convert.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    11103 2024-05-26 16:00:20.000000 c64img-3.5/tests/test_hires.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)     2508 2024-05-26 16:00:20.000000 c64img-3.5/tests/test_logger.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)    16474 2024-05-26 16:00:20.000000 c64img-3.5/tests/test_multi.py
+-rw-r--r--   0 gryf      (1000) gryf      (1000)      871 2024-05-26 16:00:20.000000 c64img-3.5/tests/test_path.py
```

### Comparing `c64img-3.2/LICENSE` & `c64img-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `c64img-3.2/PKG-INFO` & `c64img-3.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: c64img
-Version: 3.2
+Version: 3.5
 Summary: Image processing and converter for C64 graphic formats
-Home-page: https://bitbucket.org/gryf/image2c64
-Download-URL: https://bitbucket.org/gryf/image2c64.git
-Author: Roman Dobosz
-Author-email: gryf73@gmail.com
+Author-email: Roman Dobosz <gryf73@gmail.com>
+License: BSD
+Project-URL: Homepage, https://bitbucket.org/gryf/image2c64
 Keywords: c64,image,converter,koala,Art Studio,raw
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Pillow
+Requires-Dist: Pillow>=10.3.0
 
 ======
 C64img
 ======
 
 C64img is a python package which provides an abstraction layer for creating
 images which Commodore 64 understands. This is especially useful in converting
 images created on PC graphics tools, with C64 limitation in mind.
 
-This project was inspired by `PNG2HIRES_ v0.2 gfx format converter`_ /enthusi
+This project was inspired by `PNG2HIRES_ v0.1 gfx format converter`_ /enthusi
 (onslaught), which was initially used as simple graphics converter between
 PNG/GIF images to C64 hires (Art studio + executable). It evolved to bunch of
 modules, which have own purposes - from simply converting graphics, to
 generating data for C64 programs written in cross compilers, or even generating
 data for memory optimised animations out of sequence of images.
 
 Image2c64
@@ -48,50 +50,46 @@
 expected. Mutlicolor pictures will be scaled down to 160x200. Picture will be
 converted to 16 colors. During that process some information can be lost, if
 used more than 16 colors.
 
 Requirements:
 -------------
 
-+ `Python`_ 2.7, >3.5
-+ `Pillow`_ module
++ `Python`_ >=3.8
++ `Pillow`_ >=10.3.0
 
 
 Installation
 ------------
 
-Like other standard Python pro programs, ``c64img`` provide a convenient way to
-install using `setuptools`_, so the procedure will look like:
+To install c64img you'll need `pip`_ tool. For installation system wide use
+following command as a root (or by using i.e. sudo), assuming you're inside
+cloned c64img repository:
 
 .. code:: shell-session
 
-   $ python setup.py install
-
-or, `pip`_ might be used as well:
-
-.. code:: shell-session
-
-   $ pip install -e /path/to/c64img_repository
+   # pip install .
 
 or, you can grab latest stable version from `pypi`_:
 
 .. code:: shell-session
 
-   $ pip install c64img
+   # pip install c64img
 
-finally, if you prefer to use virtualenv:
+Virtualenv also can be used, especially if you have no root access:
 
 .. code:: shell-session
 
    $ virtualenv venvname
    $ source venvname/bin/activate
    (venvname) $ pip install c64img
 
-After that, you should be able to access ``image2c64`` script or import
-``c64img`` module in Python interpreter.
+After that, you should have ``image2c64`` executable available and be able to
+import ``c64img`` module in Python interpreter.
+
 
 Usage:
 ------
 
 First of all, check up the switches program provides:
 
 .. code:: shell-session
@@ -210,14 +208,14 @@
 Licence
 -------
 
 This software is licensed under 3-clause BSD license. See LICENSE file for
 details.
 
 
-.. _PNG2HIRES_ v0.2 gfx format converter: http://www.atlantis-prophecy.org/onslaught/legal.html
+.. _PNG2HIRES_ v0.1 gfx format converter: https://onslaught.atlantis-prophecy.org/releases/productions/c64/p/300/png-hires-v-.
 .. _pillow: https://github.com/python-imaging/Pillow
 .. _grafx2: http://grafx2.chez.com
 .. _python: https://www.python.org
 .. _setuptools: https://pypi.python.org/pypi/setuptools
 .. _pip: https://github.com/pypa/pip
 .. _pypi: https://pypi.org
```

### Comparing `c64img-3.2/README.rst` & `c64img-3.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 C64img
 ======
 
 C64img is a python package which provides an abstraction layer for creating
 images which Commodore 64 understands. This is especially useful in converting
 images created on PC graphics tools, with C64 limitation in mind.
 
-This project was inspired by `PNG2HIRES_ v0.2 gfx format converter`_ /enthusi
+This project was inspired by `PNG2HIRES_ v0.1 gfx format converter`_ /enthusi
 (onslaught), which was initially used as simple graphics converter between
 PNG/GIF images to C64 hires (Art studio + executable). It evolved to bunch of
 modules, which have own purposes - from simply converting graphics, to
 generating data for C64 programs written in cross compilers, or even generating
 data for memory optimised animations out of sequence of images.
 
 Image2c64
@@ -24,50 +24,46 @@
 expected. Mutlicolor pictures will be scaled down to 160x200. Picture will be
 converted to 16 colors. During that process some information can be lost, if
 used more than 16 colors.
 
 Requirements:
 -------------
 
-+ `Python`_ 2.7, >3.5
-+ `Pillow`_ module
++ `Python`_ >=3.8
++ `Pillow`_ >=10.3.0
 
 
 Installation
 ------------
 
-Like other standard Python pro programs, ``c64img`` provide a convenient way to
-install using `setuptools`_, so the procedure will look like:
+To install c64img you'll need `pip`_ tool. For installation system wide use
+following command as a root (or by using i.e. sudo), assuming you're inside
+cloned c64img repository:
 
 .. code:: shell-session
 
-   $ python setup.py install
-
-or, `pip`_ might be used as well:
-
-.. code:: shell-session
-
-   $ pip install -e /path/to/c64img_repository
+   # pip install .
 
 or, you can grab latest stable version from `pypi`_:
 
 .. code:: shell-session
 
-   $ pip install c64img
+   # pip install c64img
 
-finally, if you prefer to use virtualenv:
+Virtualenv also can be used, especially if you have no root access:
 
 .. code:: shell-session
 
    $ virtualenv venvname
    $ source venvname/bin/activate
    (venvname) $ pip install c64img
 
-After that, you should be able to access ``image2c64`` script or import
-``c64img`` module in Python interpreter.
+After that, you should have ``image2c64`` executable available and be able to
+import ``c64img`` module in Python interpreter.
+
 
 Usage:
 ------
 
 First of all, check up the switches program provides:
 
 .. code:: shell-session
@@ -186,14 +182,14 @@
 Licence
 -------
 
 This software is licensed under 3-clause BSD license. See LICENSE file for
 details.
 
 
-.. _PNG2HIRES_ v0.2 gfx format converter: http://www.atlantis-prophecy.org/onslaught/legal.html
+.. _PNG2HIRES_ v0.1 gfx format converter: https://onslaught.atlantis-prophecy.org/releases/productions/c64/p/300/png-hires-v-.
 .. _pillow: https://github.com/python-imaging/Pillow
 .. _grafx2: http://grafx2.chez.com
 .. _python: https://www.python.org
 .. _setuptools: https://pypi.python.org/pypi/setuptools
 .. _pip: https://github.com/pypa/pip
 .. _pypi: https://pypi.org
```

### Comparing `c64img-3.2/c64img/base.py` & `c64img-3.5/c64img/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
               LIGHT_GRAY: [LIGHT_GREEN, YELLOW, GRAY, WHITE]}
 COLOR_NAMES = dict(enumerate(["Black", "White", "Red", "Magenta", "Purple",
                               "Green", "Dark blue", "Yellow", "Orange",
                               "Brown", "Pink", "Dark gray", "Gray",
                               "Light green", "Light blue", "Light gray"]))
 
 
-class Char(object):
+class Char:
     """
     Char implementation
     """
 
     def __init__(self, log, prev=None, fix_clash=False):
         """
         Init. prev is the Char object which represents the same character in
@@ -213,15 +213,15 @@
         """
         Make a color map to the pixels
         """
         if self._compare_colors_with_prev_char(colors):
             self._compare_colors_with_prev_char(colors, True)
 
 
-class FullScreenImage(object):
+class FullScreenImage:
     """
     Class represents full-screen image in unspecified C64 format
     """
     WIDTH = 320
     HEIGHT = 200
     LOGGER_NAME = 'PictureConverter'
 
@@ -361,15 +361,15 @@
         return [(pal[i], pal[i + 1], pal[i + 2]) for i in range(0, 16 * 3, 3)]
 
     def _fill_memory(self):
         """
         Create bitmap/screen-ram/color-ram colors if needed. Should be
         implemented in concrete implementation.
         """
-        raise NotImplementedError()
+        raise NotImplementedError
 
     def _find_best_palette_map(self):
         """
         Try to match source image palette to predefined ones, and return name
         of the best matched palette and color map for current source image.
         """
         palettes_map = {}
```

### Comparing `c64img-3.2/c64img/cmd_convert.py` & `c64img-3.5/c64img/cmd_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 image2c64 converts virtually any fullscreen image supported by Pillow to C64
 hires or multicolor formats. Best results are achived with filetypes PNG or
 GIF.
 """
 import argparse
 import os
@@ -125,12 +123,8 @@
                        default=0)
     group.add_argument("-v", "--verbose", help='be verbose. Adding more "v" '
                        'will increase verbosity', action="count", default=0)
     parser.add_argument("-V", "--version", action='version',
                         version="%(prog)s v" + ver)
 
     arguments = parser.parse_args()
-    return convert(arguments, class_map[arguments.format])
-
-
-if __name__ == "__main__":
-    sys.exit(image2c64())
+    sys.exit(convert(arguments, class_map[arguments.format]))
```

### Comparing `c64img-3.2/c64img/hires.py` & `c64img-3.5/c64img/hires.py`

 * *Files identical despite different names*

### Comparing `c64img-3.2/c64img/logger.py` & `c64img-3.5/c64img/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import logging
 
 
-class Logger(object):
+class Logger:
     """
     Logger class with output on console only
     """
     def __init__(self, logger_name):
         """
         Initialize named logger
         """
```

### Comparing `c64img-3.2/c64img/multi.py` & `c64img-3.5/c64img/multi.py`

 * *Files identical despite different names*

### Comparing `c64img-3.2/c64img.egg-info/PKG-INFO` & `c64img-3.5/c64img.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: c64img
-Version: 3.2
+Version: 3.5
 Summary: Image processing and converter for C64 graphic formats
-Home-page: https://bitbucket.org/gryf/image2c64
-Download-URL: https://bitbucket.org/gryf/image2c64.git
-Author: Roman Dobosz
-Author-email: gryf73@gmail.com
+Author-email: Roman Dobosz <gryf73@gmail.com>
+License: BSD
+Project-URL: Homepage, https://bitbucket.org/gryf/image2c64
 Keywords: c64,image,converter,koala,Art Studio,raw
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Pillow
+Requires-Dist: Pillow>=10.3.0
 
 ======
 C64img
 ======
 
 C64img is a python package which provides an abstraction layer for creating
 images which Commodore 64 understands. This is especially useful in converting
 images created on PC graphics tools, with C64 limitation in mind.
 
-This project was inspired by `PNG2HIRES_ v0.2 gfx format converter`_ /enthusi
+This project was inspired by `PNG2HIRES_ v0.1 gfx format converter`_ /enthusi
 (onslaught), which was initially used as simple graphics converter between
 PNG/GIF images to C64 hires (Art studio + executable). It evolved to bunch of
 modules, which have own purposes - from simply converting graphics, to
 generating data for C64 programs written in cross compilers, or even generating
 data for memory optimised animations out of sequence of images.
 
 Image2c64
@@ -48,50 +50,46 @@
 expected. Mutlicolor pictures will be scaled down to 160x200. Picture will be
 converted to 16 colors. During that process some information can be lost, if
 used more than 16 colors.
 
 Requirements:
 -------------
 
-+ `Python`_ 2.7, >3.5
-+ `Pillow`_ module
++ `Python`_ >=3.8
++ `Pillow`_ >=10.3.0
 
 
 Installation
 ------------
 
-Like other standard Python pro programs, ``c64img`` provide a convenient way to
-install using `setuptools`_, so the procedure will look like:
+To install c64img you'll need `pip`_ tool. For installation system wide use
+following command as a root (or by using i.e. sudo), assuming you're inside
+cloned c64img repository:
 
 .. code:: shell-session
 
-   $ python setup.py install
-
-or, `pip`_ might be used as well:
-
-.. code:: shell-session
-
-   $ pip install -e /path/to/c64img_repository
+   # pip install .
 
 or, you can grab latest stable version from `pypi`_:
 
 .. code:: shell-session
 
-   $ pip install c64img
+   # pip install c64img
 
-finally, if you prefer to use virtualenv:
+Virtualenv also can be used, especially if you have no root access:
 
 .. code:: shell-session
 
    $ virtualenv venvname
    $ source venvname/bin/activate
    (venvname) $ pip install c64img
 
-After that, you should be able to access ``image2c64`` script or import
-``c64img`` module in Python interpreter.
+After that, you should have ``image2c64`` executable available and be able to
+import ``c64img`` module in Python interpreter.
+
 
 Usage:
 ------
 
 First of all, check up the switches program provides:
 
 .. code:: shell-session
@@ -210,14 +208,14 @@
 Licence
 -------
 
 This software is licensed under 3-clause BSD license. See LICENSE file for
 details.
 
 
-.. _PNG2HIRES_ v0.2 gfx format converter: http://www.atlantis-prophecy.org/onslaught/legal.html
+.. _PNG2HIRES_ v0.1 gfx format converter: https://onslaught.atlantis-prophecy.org/releases/productions/c64/p/300/png-hires-v-.
 .. _pillow: https://github.com/python-imaging/Pillow
 .. _grafx2: http://grafx2.chez.com
 .. _python: https://www.python.org
 .. _setuptools: https://pypi.python.org/pypi/setuptools
 .. _pip: https://github.com/pypa/pip
 .. _pypi: https://pypi.org
```

### Comparing `c64img-3.2/setup.py` & `c64img-3.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,48 @@
-#!/usr/bin/env python2
-"""
-Setup for the c64img
-"""
-from setuptools import setup
-
-from c64img import __version__ as ver
-
-
-setup(name='c64img',
-      packages=['c64img'],
-      version=ver,
-      description='Image processing and converter for C64 graphic formats',
-      author='Roman Dobosz',
-      author_email='gryf73@gmail.com',
-      url='https://bitbucket.org/gryf/image2c64',
-      download_url='https://bitbucket.org/gryf/image2c64.git',
-      keywords=['c64', 'image', 'converter', 'koala', 'Art Studio', 'raw'],
-      install_requires=['Pillow'],
-      scripts=['scripts/image2c64'],
-      classifiers=['Programming Language :: Python :: 2',
-                   'Programming Language :: Python :: 2.7',
-                   'Programming Language :: Python :: 3',
-                   'Programming Language :: Python :: 3.5',
-                   'Programming Language :: Python :: 3.6',
-                   'Development Status :: 5 - Production/Stable',
-                   'Environment :: Console',
-                   'Intended Audience :: End Users/Desktop',
-                   'License :: OSI Approved :: BSD License',
-                   'Operating System :: OS Independent',
-                   'Topic :: Multimedia :: Graphics',
-                   'Topic :: Multimedia :: Graphics :: Graphics Conversion'],
-      long_description=open('README.rst').read(),
-      options={'test': {'verbose': False,
-                        'coverage': False}})
+[build-system]
+requires = ["setuptools >= 61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "c64img"
+dynamic = ["version"]
+authors = [
+    {name = "Roman Dobosz", email = "gryf73@gmail.com"}
+]
+license = {text = "BSD"}
+description = "Image processing and converter for C64 graphic formats"
+readme = "README.rst"
+requires-python = ">=3.8"
+keywords = ['c64', 'image', 'converter', 'koala', 'Art Studio', 'raw']
+classifiers = [
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.8',
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
+    'Development Status :: 5 - Production/Stable',
+    'Environment :: Console',
+    'Intended Audience :: End Users/Desktop',
+    'License :: OSI Approved :: BSD License',
+    'Operating System :: OS Independent',
+    'Topic :: Multimedia :: Graphics',
+    'Topic :: Multimedia :: Graphics :: Graphics Conversion'
+]
+dependencies = [
+    "Pillow>=10.3.0"
+]
+
+[project.urls]
+Homepage = "https://bitbucket.org/gryf/image2c64"
+
+[project.scripts]
+image2c64 = "c64img.cmd_convert:image2c64"
+
+[tool.setuptools]
+packages = ["c64img"]
+
+[tool.setuptools.dynamic]
+version = {attr = "c64img.__version__"}
+
+[tool.distutils.bdist_wheel]
+universal = true
```

### Comparing `c64img-3.2/tests/test_base.py` & `c64img-3.5/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,27 +38,27 @@
 COLORS_2 = get_image_path("hires_2c.png")
 COLORS_256_U16 = get_image_path("hires_256_16p.png")  # 256 defined, uniq 16
 HIRES = get_image_path("hires.png")
 MULTI = get_image_path("multi.160x200.png")
 MULTI_320 = get_image_path("multi.320x200.png")
 
 
-class LogMock(object):
+class LogMock:
     """Mock logger class"""
     def warning(*args, **kwargs):
         return
 
     def debug(*args, **kwargs):
         return
 
     def critical(*args, **kwargs):
         return
 
 
-class Interceptor(object):
+class Interceptor:
     """
     Interceptor class for function call detection
     """
     def __init__(self):
         """
         Init.
         """
```

### Comparing `c64img-3.2/tests/test_convert.py` & `c64img-3.5/tests/test_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from c64img import cmd_convert
 from c64img.base import FullScreenImage
 
 
 HIRES = os.path.join(os.path.dirname(__file__), "test_images", "hires.png")
 
 
-class Interceptor(object):
+class Interceptor:
     """
     Interceptor class for function call detection
     """
     def __init__(self):
         """
         Init.
         """
@@ -43,15 +43,15 @@
     """Test resolve name function"""
 
     def setUp(self):
         if not hasattr(self, "_path"):
             self._path = os.path.abspath(os.curdir)
 
         if not hasattr(self, "_args_mock_cls"):
-            class Obj(object):
+            class Obj:
                 """
                 Mock args class
                 """
                 def __init__(self):
                     """
                     Initialization
                     """
@@ -124,15 +124,15 @@
     """
 
     def test_convert(self):
         """
         Test convert function
         """
 
-        class Mock(object):
+        class Mock:
             def __init__(self):
                 self.filename = []
                 self.errors = ['show', 'save', 'none'][2]
                 self.border = None
                 self.background = None
                 self.verbose = 0
                 self.quiet = 0
@@ -212,19 +212,19 @@
 
 
 class TestCmd(TestCase):
     """Test cmd_convert functions"""
 
     def setUp(self):
         """Setup"""
-        class AnyObj(object):
+        class AnyObj:
             """General mock"""
             pass
 
-        class ArgParseMock(object):
+        class ArgParseMock:
             """ArgumentParser mock"""
 
             def __init__(self, *args, **kwargs):
                 pass
 
             def add_argument(self, *args, **kwargs):
                 pass
@@ -247,12 +247,12 @@
         argparse.ArgumentParser = self._argparse
         cmd_convert.convert = self._convert
 
     def test_image2c64(self):
         """
         Test image2c64 cmd_convert
         """
-        self.assertEqual(cmd_convert.image2c64(), 0)
+        self.assertRaises(SystemExit, cmd_convert.image2c64)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `c64img-3.2/tests/test_hires.py` & `c64img-3.5/tests/test_hires.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 COLORS_2 = get_image_path("hires_2c.png")
 COLORS_256_U16 = get_image_path("hires_256_16p.png")  # 256 defined, uniq 16
 HIRES = get_image_path("hires.png")
 MULTI = get_image_path("multi.160x200.png")
 MULTI_320 = get_image_path("multi.320x200.png")
 
 
-class LogMock(object):
+class LogMock:
     """Mock logger class"""
 
     def warning(*args, **kwargs):
         return
 
     def debug(*args, **kwargs):
         return
 
 
-class Interceptor(object):
+class Interceptor:
     """
     Interceptor class for function call detection
     """
     def __init__(self):
         """
         Init.
         """
```

### Comparing `c64img-3.2/tests/test_logger.py` & `c64img-3.5/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `c64img-3.2/tests/test_multi.py` & `c64img-3.5/tests/test_multi.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 COLORS_2 = get_image_path("hires_2c.png")
 COLORS_256_U16 = get_image_path("hires_256_16p.png")  # 256 defined, uniq 16
 HIRES = get_image_path("hires.png")
 MULTI = get_image_path("multi.160x200.png")
 MULTI_320 = get_image_path("multi.320x200.png")
 
 
-class LogMock(object):
+class LogMock:
     """Mock logger class"""
 
     def warning(*args, **kwargs):
         return
 
     def debug(*args, **kwargs):
         return
@@ -53,15 +53,15 @@
     def critical(*args, **kwargs):
         return
 
     def getEffectiveLevel(self):
         return 30  # warn
 
 
-class Interceptor(object):
+class Interceptor:
     """
     Interceptor class for function call detection
     """
     def __init__(self):
         """
         Init.
         """
```

### Comparing `c64img-3.2/tests/test_path.py` & `c64img-3.5/tests/test_path.py`

 * *Files identical despite different names*

