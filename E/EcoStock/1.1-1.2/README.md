# Comparing `tmp/ecostock-1.1.tar.gz` & `tmp/ecostock-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecostock-1.1.tar", last modified: Sat May 25 20:14:27 2024, max compression
+gzip compressed data, was "ecostock-1.2.tar", last modified: Sat May 25 20:46:16 2024, max compression
```

## Comparing `ecostock-1.1.tar` & `ecostock-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 20:14:27.556620 ecostock-1.1/
-drwxrwxrwx   0        0        0        0 2024-05-25 20:14:27.545580 ecostock-1.1/EcoStock/
--rw-rw-rw-   0        0        0     1530 2024-05-25 20:13:30.000000 ecostock-1.1/EcoStock/__init__.py
--rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-1.1/EcoStock/adalo.py
--rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-1.1/EcoStock/api.py
--rw-rw-rw-   0        0        0    51141 2024-05-25 20:03:52.000000 ecostock-1.1/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:14:27.554553 ecostock-1.1/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     4404 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 20:14:27.000000 ecostock-1.1/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-1.1/LICENSE.md
--rw-rw-rw-   0        0        0     4404 2024-05-25 20:14:27.555552 ecostock-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3455 2024-05-25 19:35:45.000000 ecostock-1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 20:14:27.556620 ecostock-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1153 2024-05-25 20:13:07.000000 ecostock-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:46:16.969159 ecostock-1.2/
+drwxrwxrwx   0        0        0        0 2024-05-25 20:46:16.953216 ecostock-1.2/EcoStock/
+-rw-rw-rw-   0        0        0     1530 2024-05-25 20:44:31.000000 ecostock-1.2/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-1.2/EcoStock/adalo.py
+-rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-1.2/EcoStock/api.py
+-rw-rw-rw-   0        0        0    51141 2024-05-25 20:03:52.000000 ecostock-1.2/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:46:16.967172 ecostock-1.2/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     4404 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-1.2/LICENSE.md
+-rw-rw-rw-   0        0        0     4404 2024-05-25 20:46:16.968162 ecostock-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3455 2024-05-25 19:35:45.000000 ecostock-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 20:46:16.970130 ecostock-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2024-05-25 20:44:06.000000 ecostock-1.2/setup.py
```

### Comparing `ecostock-1.1/EcoStock/__init__.py` & `ecostock-1.2/EcoStock/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This package includes functions for generating candlestick charts, calculating Bollinger Bands, calculating the correlation between stocks and macroeconomic indicators,
 and much more. In addition, EcoStock provides a FastAPI-based API to access useful functions for use in no-code programming apps (e.g., via HTTP requests).
 The functions provided by EcoStock can be used to generate visualizations and insights that can help users make informed decisions in the financial markets.
 
 """
 
 # The current version of the EcoStock package
-__version__ = "1.1"
+__version__ = "1.2"
 
 # Import the FastAPI application from the api module
 from .api import app
 
 # Import the functions provided by the adalo module
 from .adalo import (
     candlestick,
```

### Comparing `ecostock-1.1/EcoStock/adalo.py` & `ecostock-1.2/EcoStock/adalo.py`

 * *Files identical despite different names*

### Comparing `ecostock-1.1/EcoStock/api.py` & `ecostock-1.2/EcoStock/api.py`

 * *Files identical despite different names*

### Comparing `ecostock-1.1/EcoStock/functions.py` & `ecostock-1.2/EcoStock/functions.py`

 * *Files identical despite different names*

### Comparing `ecostock-1.1/EcoStock.egg-info/PKG-INFO` & `ecostock-1.2/EcoStock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 1.1
+Version: 1.2
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
 Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecostock-1.1/LICENSE.md` & `ecostock-1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecostock-1.1/PKG-INFO` & `ecostock-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 1.1
+Version: 1.2
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
 Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecostock-1.1/README.md` & `ecostock-1.2/README.md`

 * *Files identical despite different names*

### Comparing `ecostock-1.1/setup.py` & `ecostock-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='1.1',
+    version='1.2',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo",
     author_email="antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com", 
     description='A Python package designed for finance professionals and economists',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/EcoStock",
     packages=find_packages(),
```

