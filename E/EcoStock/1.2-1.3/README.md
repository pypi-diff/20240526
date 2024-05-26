# Comparing `tmp/ecostock-1.2.tar.gz` & `tmp/ecostock-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecostock-1.2.tar", last modified: Sat May 25 20:46:16 2024, max compression
+gzip compressed data, was "ecostock-1.3.tar", last modified: Sun May 26 09:02:23 2024, max compression
```

## Comparing `ecostock-1.2.tar` & `ecostock-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 20:46:16.969159 ecostock-1.2/
-drwxrwxrwx   0        0        0        0 2024-05-25 20:46:16.953216 ecostock-1.2/EcoStock/
--rw-rw-rw-   0        0        0     1530 2024-05-25 20:44:31.000000 ecostock-1.2/EcoStock/__init__.py
--rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-1.2/EcoStock/adalo.py
--rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-1.2/EcoStock/api.py
--rw-rw-rw-   0        0        0    51141 2024-05-25 20:03:52.000000 ecostock-1.2/EcoStock/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-25 20:46:16.967172 ecostock-1.2/EcoStock.egg-info/
--rw-rw-rw-   0        0        0     4404 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 20:46:16.000000 ecostock-1.2/EcoStock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-1.2/LICENSE.md
--rw-rw-rw-   0        0        0     4404 2024-05-25 20:46:16.968162 ecostock-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3455 2024-05-25 19:35:45.000000 ecostock-1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 20:46:16.970130 ecostock-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1153 2024-05-25 20:44:06.000000 ecostock-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:02:23.599918 ecostock-1.3/
+drwxrwxrwx   0        0        0        0 2024-05-26 09:02:23.584298 ecostock-1.3/EcoStock/
+-rw-rw-rw-   0        0        0     1530 2024-05-26 09:00:18.000000 ecostock-1.3/EcoStock/__init__.py
+-rw-rw-rw-   0        0        0    24285 2024-05-24 14:43:10.000000 ecostock-1.3/EcoStock/adalo.py
+-rw-rw-rw-   0        0        0     5251 2024-05-25 16:03:40.000000 ecostock-1.3/EcoStock/api.py
+-rw-rw-rw-   0        0        0    51141 2024-05-25 20:03:52.000000 ecostock-1.3/EcoStock/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:02:23.599918 ecostock-1.3/EcoStock.egg-info/
+-rw-rw-rw-   0        0        0     4347 2024-05-26 09:02:23.000000 ecostock-1.3/EcoStock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-26 09:02:23.000000 ecostock-1.3/EcoStock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 09:02:23.000000 ecostock-1.3/EcoStock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2024-05-26 09:02:23.000000 ecostock-1.3/EcoStock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-26 09:02:23.000000 ecostock-1.3/EcoStock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-25 15:51:44.000000 ecostock-1.3/LICENSE.md
+-rw-rw-rw-   0        0        0     4347 2024-05-26 09:02:23.599918 ecostock-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3455 2024-05-25 19:35:45.000000 ecostock-1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 09:02:23.599918 ecostock-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2024-05-26 08:59:57.000000 ecostock-1.3/setup.py
```

### Comparing `ecostock-1.2/EcoStock/__init__.py` & `ecostock-1.3/EcoStock/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This package includes functions for generating candlestick charts, calculating Bollinger Bands, calculating the correlation between stocks and macroeconomic indicators,
 and much more. In addition, EcoStock provides a FastAPI-based API to access useful functions for use in no-code programming apps (e.g., via HTTP requests).
 The functions provided by EcoStock can be used to generate visualizations and insights that can help users make informed decisions in the financial markets.
 
 """
 
 # The current version of the EcoStock package
-__version__ = "1.2"
+__version__ = "1.3"
 
 # Import the FastAPI application from the api module
 from .api import app
 
 # Import the functions provided by the adalo module
 from .adalo import (
     candlestick,
```

### Comparing `ecostock-1.2/EcoStock/adalo.py` & `ecostock-1.3/EcoStock/adalo.py`

 * *Files identical despite different names*

### Comparing `ecostock-1.2/EcoStock/api.py` & `ecostock-1.3/EcoStock/api.py`

 * *Files identical despite different names*

### Comparing `ecostock-1.2/EcoStock/functions.py` & `ecostock-1.3/EcoStock/functions.py`

 * *Files identical despite different names*

### Comparing `ecostock-1.2/EcoStock.egg-info/PKG-INFO` & `ecostock-1.3/EcoStock.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 1.2
+Version: 1.3
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
-Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
+Author-email: antoniopaparo@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: fastapi
@@ -19,14 +19,15 @@
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: yfinance
 Requires-Dist: plotly
 Requires-Dist: requests
 Requires-Dist: seaborn
 Requires-Dist: statsmodels
+Requires-Dist: nbformat
 Requires-Dist: scikit-learn
 
 # EcoStock
 
 EcoStock is a comprehensive Python package designed for finance professionals and economists. It offers a suite of powerful tools for analyzing stock data and economic indicators, making it easier to extract insights and make informed decisions in today's dynamic markets.
 
 ## Key Features
```

### Comparing `ecostock-1.2/LICENSE.md` & `ecostock-1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ecostock-1.2/PKG-INFO` & `ecostock-1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: EcoStock
-Version: 1.2
+Version: 1.3
 Summary: A Python package designed for finance professionals and economists
 Home-page: https://github.com/Tonij10/EcoStock
 Author: Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo
-Author-email: antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com
+Author-email: antoniopaparo@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: fastapi
@@ -19,14 +19,15 @@
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: yfinance
 Requires-Dist: plotly
 Requires-Dist: requests
 Requires-Dist: seaborn
 Requires-Dist: statsmodels
+Requires-Dist: nbformat
 Requires-Dist: scikit-learn
 
 # EcoStock
 
 EcoStock is a comprehensive Python package designed for finance professionals and economists. It offers a suite of powerful tools for analyzing stock data and economic indicators, making it easier to extract insights and make informed decisions in today's dynamic markets.
 
 ## Key Features
```

### Comparing `ecostock-1.2/README.md` & `ecostock-1.3/README.md`

 * *Files identical despite different names*

### Comparing `ecostock-1.2/setup.py` & `ecostock-1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='EcoStock',
-    version='1.2',
+    version='1.3',
     author="Antonio Paparo, Giovanni Paparo, Ludovica De Giacomo, Francesco Caldo",
-    author_email="antoniopaparo@outlook.com, gio.paparo@outlook.it, ludovicadegiacomo@outlook.it, francesco.caldo00@gmail.com", 
+    author_email="antoniopaparo@outlook.com", 
     description='A Python package designed for finance professionals and economists',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tonij10/EcoStock",
     packages=find_packages(),
     install_requires=[
         'fastapi',
@@ -22,14 +22,15 @@
         'numpy',
         'matplotlib',
         'yfinance',
         'plotly',
         'requests',
         'seaborn',
         'statsmodels',
+        'nbformat',
         'scikit-learn',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

