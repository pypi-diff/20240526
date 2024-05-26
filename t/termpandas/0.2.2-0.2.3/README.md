# Comparing `tmp/termpandas-0.2.2.tar.gz` & `tmp/termpandas-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termpandas-0.2.2.tar", last modified: Thu May 23 08:14:59 2024, max compression
+gzip compressed data, was "termpandas-0.2.3.tar", last modified: Sun May 26 04:50:12 2024, max compression
```

## Comparing `termpandas-0.2.2.tar` & `termpandas-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-23 08:14:59.510530 termpandas-0.2.2/
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)      428 2024-05-23 08:12:22.000000 termpandas-0.2.2/CHANGELOG.txt
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1076 2024-04-11 15:26:31.000000 termpandas-0.2.2/LICENSE
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       75 2024-04-11 16:34:42.000000 termpandas-0.2.2/MANIFEST.in
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)     2780 2024-05-23 08:14:59.510530 termpandas-0.2.2/PKG-INFO
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)     1923 2024-05-23 08:14:02.000000 termpandas-0.2.2/README.md
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)       38 2024-05-23 08:14:59.510530 termpandas-0.2.2/setup.cfg
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)     1214 2024-05-23 08:11:57.000000 termpandas-0.2.2/setup.py
-drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-23 08:14:59.510530 termpandas-0.2.2/termpandas/
--rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       31 2024-04-11 15:57:50.000000 termpandas-0.2.2/termpandas/__init__.py
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)    16509 2024-05-22 22:10:51.000000 termpandas-0.2.2/termpandas/scrollable.py
-drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-23 08:14:59.510530 termpandas-0.2.2/termpandas.egg-info/
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)     2780 2024-05-23 08:14:59.000000 termpandas-0.2.2/termpandas.egg-info/PKG-INFO
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)      284 2024-05-23 08:14:59.000000 termpandas-0.2.2/termpandas.egg-info/SOURCES.txt
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)        1 2024-05-23 08:14:59.000000 termpandas-0.2.2/termpandas.egg-info/dependency_links.txt
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)       60 2024-05-23 08:14:59.000000 termpandas-0.2.2/termpandas.egg-info/requires.txt
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)       11 2024-05-23 08:14:59.000000 termpandas-0.2.2/termpandas.egg-info/top_level.txt
-drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-23 08:14:59.510530 termpandas-0.2.2/tests/
--rw-r--r--   0 juanesh   (1000) juanesh   (1000)     3048 2024-05-22 22:10:51.000000 termpandas-0.2.2/tests/tests.py
+drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-26 04:50:12.804180 termpandas-0.2.3/
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)      524 2024-05-26 04:49:32.000000 termpandas-0.2.3/CHANGELOG.txt
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)     1076 2024-04-11 15:26:31.000000 termpandas-0.2.3/LICENSE
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       75 2024-04-11 16:34:42.000000 termpandas-0.2.3/MANIFEST.in
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     2788 2024-05-26 04:50:12.804180 termpandas-0.2.3/PKG-INFO
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     1931 2024-05-23 08:51:51.000000 termpandas-0.2.3/README.md
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)       38 2024-05-26 04:50:12.804180 termpandas-0.2.3/setup.cfg
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     1214 2024-05-26 04:47:00.000000 termpandas-0.2.3/setup.py
+drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-26 04:50:12.800847 termpandas-0.2.3/termpandas/
+-rw-rw-r--   0 juanesh   (1000) juanesh   (1000)       31 2024-04-11 15:57:50.000000 termpandas-0.2.3/termpandas/__init__.py
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)    16509 2024-05-22 22:10:51.000000 termpandas-0.2.3/termpandas/scrollable.py
+drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-26 04:50:12.804180 termpandas-0.2.3/termpandas.egg-info/
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     2788 2024-05-26 04:50:12.000000 termpandas-0.2.3/termpandas.egg-info/PKG-INFO
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)      284 2024-05-26 04:50:12.000000 termpandas-0.2.3/termpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)        1 2024-05-26 04:50:12.000000 termpandas-0.2.3/termpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)       60 2024-05-26 04:50:12.000000 termpandas-0.2.3/termpandas.egg-info/requires.txt
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)       11 2024-05-26 04:50:12.000000 termpandas-0.2.3/termpandas.egg-info/top_level.txt
+drwxr-xr-x   0 juanesh   (1000) juanesh   (1000)        0 2024-05-26 04:50:12.804180 termpandas-0.2.3/tests/
+-rw-r--r--   0 juanesh   (1000) juanesh   (1000)     3048 2024-05-22 22:10:51.000000 termpandas-0.2.3/tests/tests.py
```

### Comparing `termpandas-0.2.2/LICENSE` & `termpandas-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `termpandas-0.2.2/PKG-INFO` & `termpandas-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termpandas
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scrollable pandas dataframes in the terminal.
 Home-page: https://github.com/juan-esteban-berger/termpandas
 Author: Juan Esteban Berger
 Author-email: juanestebanberger@gmail.com
 Project-URL: Source Code, https://github.com/juan-esteban-berger/termpandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: blessings>=1.7
 Requires-Dist: curtsies>=0.4.2
-Requires-Dist: polars>=0.20.3
+Requires-Dist: polars>=0.18.0
 
 # termpandas
 Scrollable Pandas and Polars DataFrames in the Terminal.
 
 ![tprint_demo.gif](https://raw.githubusercontent.com/juan-esteban-berger/termpandas/main/tprint_demo.gif)
 
 ## Installation
@@ -61,15 +61,15 @@
 - `highlight`: Highlights the selected row. Default is `True`.
 ```python
 tprint(df, highlight=True)
 ```
 
 - `highlight_color`: Color of the selected row. Default is `Gray`.
 ```python
-tprint(df, highlight=True)
+tprint(df, highlight_color='Gray')
 ```
 
 - `masks`: Dictionary of masks to highlight rows. Default is `{}`. The keys are the colors and the values are the masks.
 ```python
 mask_1 = df['Survived'] == 1
 mask_2 = df['Sex'] == 'male'
 tprint(df.head(20), masks={'Red': mask_1,'Blue': mask_2})
```

### Comparing `termpandas-0.2.2/README.md` & `termpandas-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 - `highlight`: Highlights the selected row. Default is `True`.
 ```python
 tprint(df, highlight=True)
 ```
 
 - `highlight_color`: Color of the selected row. Default is `Gray`.
 ```python
-tprint(df, highlight=True)
+tprint(df, highlight_color='Gray')
 ```
 
 - `masks`: Dictionary of masks to highlight rows. Default is `{}`. The keys are the colors and the values are the masks.
 ```python
 mask_1 = df['Survived'] == 1
 mask_2 = df['Sex'] == 'male'
 tprint(df.head(20), masks={'Red': mask_1,'Blue': mask_2})
```

### Comparing `termpandas-0.2.2/setup.py` & `termpandas-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 # Load the README file and use it as the long_description.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='termpandas',
-    version='0.2.2',
+    version='0.2.3',
     url='https://github.com/juan-esteban-berger/termpandas',
     author='Juan Esteban Berger',
     author_email='juanestebanberger@gmail.com',
     description='Scrollable pandas dataframes in the terminal.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=['pandas>=2.1.4',
                       'blessings>=1.7',
                       'curtsies>=0.4.2',
-                      'polars>=0.20.3'
+                      'polars>=0.18.0'
                       ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `termpandas-0.2.2/termpandas/scrollable.py` & `termpandas-0.2.3/termpandas/scrollable.py`

 * *Files identical despite different names*

### Comparing `termpandas-0.2.2/termpandas.egg-info/PKG-INFO` & `termpandas-0.2.3/termpandas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termpandas
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scrollable pandas dataframes in the terminal.
 Home-page: https://github.com/juan-esteban-berger/termpandas
 Author: Juan Esteban Berger
 Author-email: juanestebanberger@gmail.com
 Project-URL: Source Code, https://github.com/juan-esteban-berger/termpandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: blessings>=1.7
 Requires-Dist: curtsies>=0.4.2
-Requires-Dist: polars>=0.20.3
+Requires-Dist: polars>=0.18.0
 
 # termpandas
 Scrollable Pandas and Polars DataFrames in the Terminal.
 
 ![tprint_demo.gif](https://raw.githubusercontent.com/juan-esteban-berger/termpandas/main/tprint_demo.gif)
 
 ## Installation
@@ -61,15 +61,15 @@
 - `highlight`: Highlights the selected row. Default is `True`.
 ```python
 tprint(df, highlight=True)
 ```
 
 - `highlight_color`: Color of the selected row. Default is `Gray`.
 ```python
-tprint(df, highlight=True)
+tprint(df, highlight_color='Gray')
 ```
 
 - `masks`: Dictionary of masks to highlight rows. Default is `{}`. The keys are the colors and the values are the masks.
 ```python
 mask_1 = df['Survived'] == 1
 mask_2 = df['Sex'] == 'male'
 tprint(df.head(20), masks={'Red': mask_1,'Blue': mask_2})
```

### Comparing `termpandas-0.2.2/tests/tests.py` & `termpandas-0.2.3/tests/tests.py`

 * *Files identical despite different names*

