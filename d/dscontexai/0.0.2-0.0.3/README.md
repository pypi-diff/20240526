# Comparing `tmp/dscontexai-0.0.2.tar.gz` & `tmp/dscontexai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-0.0.2.tar", last modified: Sun May 26 13:46:46 2024, max compression
+gzip compressed data, was "dscontexai-0.0.3.tar", last modified: Sun May 26 13:56:05 2024, max compression
```

## Comparing `dscontexai-0.0.2.tar` & `dscontexai-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:46:46.526155 dscontexai-0.0.2/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:46:46.526155 dscontexai-0.0.2/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:46:46.526155 dscontexai-0.0.2/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      100 2024-05-26 13:46:04.000000 dscontexai-0.0.2/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3601 2024-05-26 10:20:02.000000 dscontexai-0.0.2/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10463 2024-05-26 09:55:24.000000 dscontexai-0.0.2/dscontexai/grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10176 2024-05-26 09:38:15.000000 dscontexai-0.0.2/dscontexai/grammar_with_box_latex.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3495 2024-05-26 09:49:20.000000 dscontexai-0.0.2/dscontexai/ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1405 2024-05-26 05:49:34.000000 dscontexai-0.0.2/dscontexai/xgboost.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:46:46.526155 dscontexai-0.0.2/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      333 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1059 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 13:46:46.526155 dscontexai-0.0.2/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     2393 2024-05-26 13:46:20.000000 dscontexai-0.0.2/setup.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:56:05.983088 dscontexai-0.0.3/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:56:05.983088 dscontexai-0.0.3/PKG-INFO
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:56:05.983088 dscontexai-0.0.3/dscontexai/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      104 2024-05-26 13:54:22.000000 dscontexai-0.0.3/dscontexai/__init__.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10463 2024-05-26 09:55:24.000000 dscontexai-0.0.3/dscontexai/dsc_grammar.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3604 2024-05-26 13:54:56.000000 dscontexai-0.0.3/dscontexai/generate_report.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10176 2024-05-26 09:38:15.000000 dscontexai-0.0.3/dscontexai/grammar_with_box_latex.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3495 2024-05-26 09:49:20.000000 dscontexai-0.0.3/dscontexai/ploting.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1405 2024-05-26 05:49:34.000000 dscontexai-0.0.3/dscontexai/xgboost.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:56:05.983088 dscontexai-0.0.3/dscontexai.egg-info/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/PKG-INFO
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      337 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1059 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/requires.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 13:56:05.000000 dscontexai-0.0.3/dscontexai.egg-info/top_level.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 13:56:05.983088 dscontexai-0.0.3/setup.cfg
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     2393 2024-05-26 13:55:47.000000 dscontexai-0.0.3/setup.py
```

### Comparing `dscontexai-0.0.2/dscontexai/generate_report.py` & `dscontexai-0.0.3/dscontexai/generate_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import argparse
 import json
 import pickle
 
 import pandas as pd
 import shap
 from catboost import CatBoostClassifier
-
-from grammar import analyze_shap_values
+from dsc_grammar import analyze_shap_values
 
 
 def diabetes_case() -> None:
     """
     Load the diabetes model and data, and generate a report for a specific instance.
     """
     df = pd.read_csv("./kaggle_data/processed_data.csv")
```

### Comparing `dscontexai-0.0.2/dscontexai/grammar.py` & `dscontexai-0.0.3/dscontexai/dsc_grammar.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.2/dscontexai/grammar_with_box_latex.py` & `dscontexai-0.0.3/dscontexai/grammar_with_box_latex.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.2/dscontexai/ploting.py` & `dscontexai-0.0.3/dscontexai/ploting.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.2/dscontexai/xgboost.py` & `dscontexai-0.0.3/dscontexai/xgboost.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.2/dscontexai.egg-info/requires.txt` & `dscontexai-0.0.3/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.2/setup.py` & `dscontexai-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "ConteXAI"
 LONG_DESCRIPTION = "xAI for everyone!"
 
 # Setting up
 setup(
     name="dscontexai",
     version=VERSION,
```

