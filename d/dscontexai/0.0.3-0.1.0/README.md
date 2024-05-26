# Comparing `tmp/dscontexai-0.0.3.tar.gz` & `tmp/dscontexai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-0.0.3.tar", last modified: Sun May 26 13:56:05 2024, max compression
+gzip compressed data, was "dscontexai-0.1.0.tar", last modified: Sun May 26 13:57:54 2024, max compression
```

## Comparing `dscontexai-0.0.3.tar` & `dscontexai-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:56:05.983088 dscontexai-0.0.3/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:56:05.983088 dscontexai-0.0.3/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:56:05.983088 dscontexai-0.0.3/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      104 2024-05-26 13:54:22.000000 dscontexai-0.0.3/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10463 2024-05-26 09:55:24.000000 dscontexai-0.0.3/dscontexai/dsc_grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3604 2024-05-26 13:54:56.000000 dscontexai-0.0.3/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10176 2024-05-26 09:38:15.000000 dscontexai-0.0.3/dscontexai/grammar_with_box_latex.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3495 2024-05-26 09:49:20.000000 dscontexai-0.0.3/dscontexai/ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1405 2024-05-26 05:49:34.000000 dscontexai-0.0.3/dscontexai/xgboost.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:56:05.983088 dscontexai-0.0.3/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      337 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1059 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 13:56:05.983088 dscontexai-0.0.3/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     2393 2024-05-26 13:55:47.000000 dscontexai-0.0.3/setup.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:57:54.485668 dscontexai-0.1.0/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:57:54.481668 dscontexai-0.1.0/PKG-INFO
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:57:54.481668 dscontexai-0.1.0/dscontexai/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 13:57:39.000000 dscontexai-0.1.0/dscontexai/__init__.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10478 2024-05-26 13:57:24.000000 dscontexai-0.1.0/dscontexai/dsc_grammar.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3495 2024-05-26 09:49:20.000000 dscontexai-0.1.0/dscontexai/dsc_ploting.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1405 2024-05-26 05:49:34.000000 dscontexai-0.1.0/dscontexai/dsc_xgboost.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3604 2024-05-26 13:54:56.000000 dscontexai-0.1.0/dscontexai/generate_report.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10206 2024-05-26 13:57:37.000000 dscontexai-0.1.0/dscontexai/grammar_with_box_latex.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:57:54.481668 dscontexai-0.1.0/dscontexai.egg-info/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:57:54.000000 dscontexai-0.1.0/dscontexai.egg-info/PKG-INFO
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      345 2024-05-26 13:57:54.000000 dscontexai-0.1.0/dscontexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 13:57:54.000000 dscontexai-0.1.0/dscontexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1059 2024-05-26 13:57:54.000000 dscontexai-0.1.0/dscontexai.egg-info/requires.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 13:57:54.000000 dscontexai-0.1.0/dscontexai.egg-info/top_level.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 13:57:54.485668 dscontexai-0.1.0/setup.cfg
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     2393 2024-05-26 13:57:44.000000 dscontexai-0.1.0/setup.py
```

### Comparing `dscontexai-0.0.3/dscontexai/dsc_grammar.py` & `dscontexai-0.1.0/dscontexai/dsc_grammar.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import shap
 from pylatex import Document, Figure, Itemize, NoEscape, Package, Section, Subsection
 from pylatex.utils import bold
 
-from ploting import plot_shap
+from dscontexai.dsc_ploting import plot_shap
 
 plt.rcParams["text.usetex"] = True
 
 
 def fixing_variable_names(variables: list) -> list:
     """
     Fix the variable names by removing underscores and capitalizing the first letter of each word.
```

### Comparing `dscontexai-0.0.3/dscontexai/generate_report.py` & `dscontexai-0.1.0/dscontexai/generate_report.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.3/dscontexai/grammar_with_box_latex.py` & `dscontexai-0.1.0/dscontexai/grammar_with_box_latex.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     NoEscape,
     Package,
     Section,
     Subsection,
 )
 from pylatex.utils import bold
 
-import xgboost as xgb
-from ploting import plot_shap
+import dscontexai.dsc_xgboost as xgb
+from dscontexai.dsc_ploting import plot_shap
 
 plt.rcParams["text.usetex"] = True
 
 
 def fixing_variable_names(variables: list) -> list:
     """
     Fix the variable names by removing underscores and capitalizing the first letter of each word.
```

### Comparing `dscontexai-0.0.3/dscontexai/ploting.py` & `dscontexai-0.1.0/dscontexai/dsc_ploting.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.3/dscontexai/xgboost.py` & `dscontexai-0.1.0/dscontexai/dsc_xgboost.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.3/dscontexai.egg-info/requires.txt` & `dscontexai-0.1.0/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.3/setup.py` & `dscontexai-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.3"
+VERSION = "0.1.0"
 DESCRIPTION = "ConteXAI"
 LONG_DESCRIPTION = "xAI for everyone!"
 
 # Setting up
 setup(
     name="dscontexai",
     version=VERSION,
```
