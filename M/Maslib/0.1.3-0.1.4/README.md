# Comparing `tmp/Maslib-0.1.3.tar.gz` & `tmp/Maslib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Maslib-0.1.3.tar", last modified: Sun May 26 09:54:31 2024, max compression
+gzip compressed data, was "Maslib-0.1.4.tar", last modified: Sun May 26 15:43:18 2024, max compression
```

## Comparing `Maslib-0.1.3.tar` & `Maslib-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 09:54:31.047184 Maslib-0.1.3/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.1.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-26 09:54:31.025743 Maslib-0.1.3/MasLib/
--rw-rw-rw-   0        0        0     1310 2024-05-26 07:57:21.000000 Maslib-0.1.3/MasLib/__init__.py
--rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 Maslib-0.1.3/MasLib/classification.py
--rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 Maslib-0.1.3/MasLib/clustering.py
--rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 Maslib-0.1.3/MasLib/correlation.py
--rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 Maslib-0.1.3/MasLib/encoding.py
--rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 Maslib-0.1.3/MasLib/loading.py
--rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 Maslib-0.1.3/MasLib/regressions.py
--rw-rw-rw-   0        0        0    11632 2024-05-26 09:23:14.000000 Maslib-0.1.3/MasLib/text_coding.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:54:31.044590 Maslib-0.1.3/Maslib.egg-info/
--rw-rw-rw-   0        0        0      888 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      888 2024-05-26 09:54:31.045628 Maslib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-26 09:52:47.000000 Maslib-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 09:54:31.047184 Maslib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      811 2024-05-26 09:51:27.000000 Maslib-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:54:31.042425 Maslib-0.1.3/tests/
--rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 Maslib-0.1.3/tests/test_clustering.py
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.1.3/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.1.3/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.1.3/tests/test_grid_search.py
--rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 Maslib-0.1.3/tests/test_loading.py
--rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 Maslib-0.1.3/tests/test_regression.py
--rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 Maslib-0.1.3/tests/test_text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:43:18.122193 Maslib-0.1.4/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.1.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-26 15:43:18.097172 Maslib-0.1.4/MasLib/
+-rw-rw-rw-   0        0        0     1310 2024-05-26 07:57:21.000000 Maslib-0.1.4/MasLib/__init__.py
+-rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 Maslib-0.1.4/MasLib/classification.py
+-rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 Maslib-0.1.4/MasLib/clustering.py
+-rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 Maslib-0.1.4/MasLib/correlation.py
+-rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 Maslib-0.1.4/MasLib/encoding.py
+-rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 Maslib-0.1.4/MasLib/loading.py
+-rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 Maslib-0.1.4/MasLib/regressions.py
+-rw-rw-rw-   0        0        0    11632 2024-05-26 09:23:14.000000 Maslib-0.1.4/MasLib/text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:43:18.119191 Maslib-0.1.4/Maslib.egg-info/
+-rw-rw-rw-   0        0        0      912 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      912 2024-05-26 15:43:18.120192 Maslib-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-26 09:52:47.000000 Maslib-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:43:18.122193 Maslib-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      830 2024-05-26 15:42:47.000000 Maslib-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:43:18.117189 Maslib-0.1.4/tests/
+-rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 Maslib-0.1.4/tests/test_clustering.py
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.1.4/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.1.4/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.1.4/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 Maslib-0.1.4/tests/test_loading.py
+-rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 Maslib-0.1.4/tests/test_regression.py
+-rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 Maslib-0.1.4/tests/test_text_coding.py
```

### Comparing `Maslib-0.1.3/MasLib/__init__.py` & `Maslib-0.1.4/MasLib/__init__.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/MasLib/classification.py` & `Maslib-0.1.4/MasLib/classification.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/MasLib/clustering.py` & `Maslib-0.1.4/MasLib/clustering.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/MasLib/correlation.py` & `Maslib-0.1.4/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/MasLib/encoding.py` & `Maslib-0.1.4/MasLib/encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/MasLib/loading.py` & `Maslib-0.1.4/MasLib/loading.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/MasLib/regressions.py` & `Maslib-0.1.4/MasLib/regressions.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/MasLib/text_coding.py` & `Maslib-0.1.4/MasLib/text_coding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/Maslib.egg-info/PKG-INFO` & `Maslib-0.1.4/Maslib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is a library for optimizing code for python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,14 +15,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: joblib
 Requires-Dist: wordcloud
 Requires-Dist: xgboost
 Requires-Dist: bertopic
+Requires-Dist: hdbscan
 
 # MasLib
 
 MasLib - this is a Python library for code reduction
 
 My library can safely optimize everyday tasks for python
```

### Comparing `Maslib-0.1.3/Maslib.egg-info/SOURCES.txt` & `Maslib-0.1.4/Maslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/PKG-INFO` & `Maslib-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is a library for optimizing code for python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,14 +15,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: joblib
 Requires-Dist: wordcloud
 Requires-Dist: xgboost
 Requires-Dist: bertopic
+Requires-Dist: hdbscan
 
 # MasLib
 
 MasLib - this is a Python library for code reduction
 
 My library can safely optimize everyday tasks for python
```

### Comparing `Maslib-0.1.3/setup.py` & `Maslib-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.1.3',
+    version='0.1.4',
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
         'bertopic',
+        'hdbscan'
 
     ],
     author='Alecsandr_C.V.V',
     author_email='dxomko@gmail.com',
     description='This is a library for optimizing code for python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `Maslib-0.1.3/tests/test_clustering.py` & `Maslib-0.1.4/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/tests/test_correlation.py` & `Maslib-0.1.4/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/tests/test_encoding.py` & `Maslib-0.1.4/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/tests/test_grid_search.py` & `Maslib-0.1.4/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/tests/test_regression.py` & `Maslib-0.1.4/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.3/tests/test_text_coding.py` & `Maslib-0.1.4/tests/test_text_coding.py`

 * *Files identical despite different names*

