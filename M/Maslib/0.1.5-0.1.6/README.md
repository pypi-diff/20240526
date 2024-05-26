# Comparing `tmp/Maslib-0.1.5.tar.gz` & `tmp/maslib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Maslib-0.1.5.tar", last modified: Sun May 26 15:49:59 2024, max compression
+gzip compressed data, was "maslib-0.1.6.tar", last modified: Sun May 26 16:41:57 2024, max compression
```

## Comparing `Maslib-0.1.5.tar` & `maslib-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:49:59.717412 Maslib-0.1.5/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.1.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-26 15:49:59.693390 Maslib-0.1.5/MasLib/
--rw-rw-rw-   0        0        0     1289 2024-05-26 15:49:25.000000 Maslib-0.1.5/MasLib/__init__.py
--rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 Maslib-0.1.5/MasLib/classification.py
--rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 Maslib-0.1.5/MasLib/clustering.py
--rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 Maslib-0.1.5/MasLib/correlation.py
--rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 Maslib-0.1.5/MasLib/encoding.py
--rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 Maslib-0.1.5/MasLib/loading.py
--rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 Maslib-0.1.5/MasLib/regressions.py
--rw-rw-rw-   0        0        0    11006 2024-05-26 15:49:15.000000 Maslib-0.1.5/MasLib/text_coding.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:49:59.714409 Maslib-0.1.5/Maslib.egg-info/
--rw-rw-rw-   0        0        0      863 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      863 2024-05-26 15:49:59.715411 Maslib-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-26 09:52:47.000000 Maslib-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 15:49:59.717412 Maslib-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      790 2024-05-26 15:49:39.000000 Maslib-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:49:59.711407 Maslib-0.1.5/tests/
--rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 Maslib-0.1.5/tests/test_clustering.py
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.1.5/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.1.5/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.1.5/tests/test_grid_search.py
--rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 Maslib-0.1.5/tests/test_loading.py
--rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 Maslib-0.1.5/tests/test_regression.py
--rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 Maslib-0.1.5/tests/test_text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:57.217957 maslib-0.1.6/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 maslib-0.1.6/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:57.194936 maslib-0.1.6/MasLib/
+-rw-rw-rw-   0        0        0     1289 2024-05-26 16:09:16.000000 maslib-0.1.6/MasLib/__init__.py
+-rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 maslib-0.1.6/MasLib/classification.py
+-rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 maslib-0.1.6/MasLib/clustering.py
+-rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 maslib-0.1.6/MasLib/correlation.py
+-rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 maslib-0.1.6/MasLib/encoding.py
+-rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 maslib-0.1.6/MasLib/loading.py
+-rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 maslib-0.1.6/MasLib/regressions.py
+-rw-rw-rw-   0        0        0    11006 2024-05-26 15:49:15.000000 maslib-0.1.6/MasLib/text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:57.213954 maslib-0.1.6/Maslib.egg-info/
+-rw-rw-rw-   0        0        0      884 2024-05-26 16:41:57.000000 maslib-0.1.6/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-05-26 16:41:57.000000 maslib-0.1.6/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 16:41:57.000000 maslib-0.1.6/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-05-26 16:41:57.000000 maslib-0.1.6/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 16:41:57.000000 maslib-0.1.6/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      884 2024-05-26 16:41:57.215956 maslib-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-26 09:52:47.000000 maslib-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 16:41:57.217957 maslib-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-05-26 16:41:49.000000 maslib-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:57.212952 maslib-0.1.6/tests/
+-rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 maslib-0.1.6/tests/test_clustering.py
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 maslib-0.1.6/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 maslib-0.1.6/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 maslib-0.1.6/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 maslib-0.1.6/tests/test_loading.py
+-rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 maslib-0.1.6/tests/test_regression.py
+-rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 maslib-0.1.6/tests/test_text_coding.py
```

### Comparing `Maslib-0.1.5/MasLib/__init__.py` & `maslib-0.1.6/MasLib/__init__.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/MasLib/classification.py` & `maslib-0.1.6/MasLib/classification.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/MasLib/clustering.py` & `maslib-0.1.6/MasLib/clustering.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/MasLib/correlation.py` & `maslib-0.1.6/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/MasLib/encoding.py` & `maslib-0.1.6/MasLib/encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/MasLib/loading.py` & `maslib-0.1.6/MasLib/loading.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/MasLib/regressions.py` & `maslib-0.1.6/MasLib/regressions.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/MasLib/text_coding.py` & `maslib-0.1.6/MasLib/text_coding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/Maslib.egg-info/PKG-INFO` & `maslib-0.1.6/Maslib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is a library for optimizing code for python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -14,14 +14,15 @@
 Requires-Dist: phik
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: joblib
 Requires-Dist: wordcloud
 Requires-Dist: xgboost
+Requires-Dist: nltk
 
 # MasLib
 
 MasLib - this is a Python library for code reduction
 
 My library can safely optimize everyday tasks for python
```

### Comparing `Maslib-0.1.5/Maslib.egg-info/SOURCES.txt` & `maslib-0.1.6/Maslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/PKG-INFO` & `maslib-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is a library for optimizing code for python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -14,14 +14,15 @@
 Requires-Dist: phik
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: joblib
 Requires-Dist: wordcloud
 Requires-Dist: xgboost
+Requires-Dist: nltk
 
 # MasLib
 
 MasLib - this is a Python library for code reduction
 
 My library can safely optimize everyday tasks for python
```

### Comparing `Maslib-0.1.5/setup.py` & `maslib-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'phik',
         'matplotlib',
         'scikit-learn',
         'catboost',
         'joblib',
         'wordcloud',
         'xgboost',
+        'nltk'
 
     ],
     author='Alecsandr_C.V.V',
     author_email='dxomko@gmail.com',
     description='This is a library for optimizing code for python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `Maslib-0.1.5/tests/test_clustering.py` & `maslib-0.1.6/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/tests/test_correlation.py` & `maslib-0.1.6/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/tests/test_encoding.py` & `maslib-0.1.6/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/tests/test_grid_search.py` & `maslib-0.1.6/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/tests/test_regression.py` & `maslib-0.1.6/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.5/tests/test_text_coding.py` & `maslib-0.1.6/tests/test_text_coding.py`

 * *Files identical despite different names*

