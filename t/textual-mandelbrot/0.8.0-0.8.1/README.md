# Comparing `tmp/textual-mandelbrot-0.8.0.tar.gz` & `tmp/textual_mandelbrot-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textual-mandelbrot-0.8.0.tar", last modified: Sun Mar 10 12:11:46 2024, max compression
+gzip compressed data, was "textual_mandelbrot-0.8.1.tar", last modified: Sun May 26 08:21:43 2024, max compression
```

## Comparing `textual-mandelbrot-0.8.0.tar` & `textual_mandelbrot-0.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-10 12:11:46.061213 textual-mandelbrot-0.8.0/
--rw-r--r--   0 davep      (501) staff       (20)     4387 2024-03-10 12:11:46.061153 textual-mandelbrot-0.8.0/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)     2988 2024-03-10 12:05:21.000000 textual-mandelbrot-0.8.0/README.md
--rw-r--r--   0 davep      (501) staff       (20)      124 2023-03-29 20:11:20.000000 textual-mandelbrot-0.8.0/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1585 2024-03-10 12:11:46.061478 textual-mandelbrot-0.8.0/setup.cfg
--rw-r--r--   0 davep      (501) staff       (20)      344 2023-03-29 20:11:07.000000 textual-mandelbrot-0.8.0/setup.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-10 12:11:46.059990 textual-mandelbrot-0.8.0/textual_mandelbrot/
--rw-r--r--   0 davep      (501) staff       (20)      787 2024-03-10 12:10:29.000000 textual-mandelbrot-0.8.0/textual_mandelbrot/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     4830 2023-09-29 11:17:14.000000 textual-mandelbrot-0.8.0/textual_mandelbrot/__main__.py
--rw-r--r--   0 davep      (501) staff       (20)     2082 2023-09-28 21:52:47.000000 textual-mandelbrot-0.8.0/textual_mandelbrot/colouring.py
--rw-r--r--   0 davep      (501) staff       (20)     5265 2024-03-10 11:58:01.000000 textual-mandelbrot-0.8.0/textual_mandelbrot/commands.py
--rw-r--r--   0 davep      (501) staff       (20)    12362 2023-09-28 21:52:47.000000 textual-mandelbrot-0.8.0/textual_mandelbrot/mandelbrot.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-03-10 12:11:46.060920 textual-mandelbrot-0.8.0/textual_mandelbrot.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     4387 2024-03-10 12:11:46.000000 textual-mandelbrot-0.8.0/textual_mandelbrot.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      455 2024-03-10 12:11:46.000000 textual-mandelbrot-0.8.0/textual_mandelbrot.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2024-03-10 12:11:46.000000 textual-mandelbrot-0.8.0/textual_mandelbrot.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       63 2024-03-10 12:11:46.000000 textual-mandelbrot-0.8.0/textual_mandelbrot.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       31 2024-03-10 12:11:46.000000 textual-mandelbrot-0.8.0/textual_mandelbrot.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)       19 2024-03-10 12:11:46.000000 textual-mandelbrot-0.8.0/textual_mandelbrot.egg-info/top_level.txt
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-05-26 08:21:43.409424 textual_mandelbrot-0.8.1/
+-rw-r--r--   0 davep      (501) staff       (20)     4395 2024-05-26 08:21:43.409368 textual_mandelbrot-0.8.1/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)     2988 2024-05-26 08:18:10.000000 textual_mandelbrot-0.8.1/README.md
+-rw-r--r--   0 davep      (501) staff       (20)      124 2023-03-29 20:11:20.000000 textual_mandelbrot-0.8.1/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1593 2024-05-26 08:21:43.409681 textual_mandelbrot-0.8.1/setup.cfg
+-rw-r--r--   0 davep      (501) staff       (20)      344 2023-03-29 20:11:07.000000 textual_mandelbrot-0.8.1/setup.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-05-26 08:21:43.408245 textual_mandelbrot-0.8.1/textual_mandelbrot/
+-rw-r--r--   0 davep      (501) staff       (20)      787 2024-05-26 08:20:09.000000 textual_mandelbrot-0.8.1/textual_mandelbrot/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     4830 2023-09-29 11:17:14.000000 textual_mandelbrot-0.8.1/textual_mandelbrot/__main__.py
+-rw-r--r--   0 davep      (501) staff       (20)     2082 2023-09-28 21:52:47.000000 textual_mandelbrot-0.8.1/textual_mandelbrot/colouring.py
+-rw-r--r--   0 davep      (501) staff       (20)     5265 2024-05-26 08:18:10.000000 textual_mandelbrot-0.8.1/textual_mandelbrot/commands.py
+-rw-r--r--   0 davep      (501) staff       (20)    12362 2023-09-28 21:52:47.000000 textual_mandelbrot-0.8.1/textual_mandelbrot/mandelbrot.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-05-26 08:21:43.409170 textual_mandelbrot-0.8.1/textual_mandelbrot.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     4395 2024-05-26 08:21:43.000000 textual_mandelbrot-0.8.1/textual_mandelbrot.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      455 2024-05-26 08:21:43.000000 textual_mandelbrot-0.8.1/textual_mandelbrot.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2024-05-26 08:21:43.000000 textual_mandelbrot-0.8.1/textual_mandelbrot.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       63 2024-05-26 08:21:43.000000 textual_mandelbrot-0.8.1/textual_mandelbrot.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       39 2024-05-26 08:21:43.000000 textual_mandelbrot-0.8.1/textual_mandelbrot.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)       19 2024-05-26 08:21:43.000000 textual_mandelbrot-0.8.1/textual_mandelbrot.egg-info/top_level.txt
```

### Comparing `textual-mandelbrot-0.8.0/PKG-INFO` & `textual_mandelbrot-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-mandelbrot
-Version: 0.8.0
+Version: 0.8.1
 Summary: A simple Mandelbrot explorer for the terminal.
 Home-page: https://github.com/davep/textual-mandelbrot
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Terminals
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: textual>=0.52.1
+Requires-Dist: textual<0.61.0,>=0.57.0
 Requires-Dist: textual-canvas
 
 # textual-mandelbrot
 
 ![mandelexp in action](https://raw.githubusercontent.com/davep/textual-mandelbrot/main/img/mandelexp01.png)
 ![mandelexp in action](https://raw.githubusercontent.com/davep/textual-mandelbrot/main/img/mandelexp02.png)
```

### Comparing `textual-mandelbrot-0.8.0/README.md` & `textual_mandelbrot-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `textual-mandelbrot-0.8.0/setup.cfg` & `textual_mandelbrot-0.8.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 	Discussions = https://github.com/davep/textual-mandelbrot/discussions
 
 [options]
 packages = find:
 platforms = any
 include_package_data = True
 install_requires = 
-	textual>=0.52.1
+	textual>=0.57.0,<0.61.0
 	textual-canvas
 python_requires = >=3.8
 
 [options.package_data]
 textual_mandelbrot = py.typed
 
 [options.entry_points]
```

### Comparing `textual-mandelbrot-0.8.0/textual_mandelbrot/__init__.py` & `textual_mandelbrot-0.8.1/textual_mandelbrot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__ = "Dave Pearson"
 __copyright__ = "Copyright 2023-2024, Dave Pearson"
 __credits__ = ["Dave Pearson"]
 __maintainer__ = "Dave Pearson"
 __email__ = "davep@davep.org"
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 __licence__ = "MIT"
 
 ##############################################################################
 # Local imports.
 from .mandelbrot import Mandelbrot
 from .colouring import default_map, blue_brown_map, shades_of_green
```

### Comparing `textual-mandelbrot-0.8.0/textual_mandelbrot/__main__.py` & `textual_mandelbrot-0.8.1/textual_mandelbrot/__main__.py`

 * *Files identical despite different names*

### Comparing `textual-mandelbrot-0.8.0/textual_mandelbrot/colouring.py` & `textual_mandelbrot-0.8.1/textual_mandelbrot/colouring.py`

 * *Files identical despite different names*

### Comparing `textual-mandelbrot-0.8.0/textual_mandelbrot/commands.py` & `textual_mandelbrot-0.8.1/textual_mandelbrot/commands.py`

 * *Files identical despite different names*

### Comparing `textual-mandelbrot-0.8.0/textual_mandelbrot/mandelbrot.py` & `textual_mandelbrot-0.8.1/textual_mandelbrot/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `textual-mandelbrot-0.8.0/textual_mandelbrot.egg-info/PKG-INFO` & `textual_mandelbrot-0.8.1/textual_mandelbrot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-mandelbrot
-Version: 0.8.0
+Version: 0.8.1
 Summary: A simple Mandelbrot explorer for the terminal.
 Home-page: https://github.com/davep/textual-mandelbrot
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Terminals
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: textual>=0.52.1
+Requires-Dist: textual<0.61.0,>=0.57.0
 Requires-Dist: textual-canvas
 
 # textual-mandelbrot
 
 ![mandelexp in action](https://raw.githubusercontent.com/davep/textual-mandelbrot/main/img/mandelexp01.png)
 ![mandelexp in action](https://raw.githubusercontent.com/davep/textual-mandelbrot/main/img/mandelexp02.png)
```

