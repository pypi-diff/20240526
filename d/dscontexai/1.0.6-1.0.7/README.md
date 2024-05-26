# Comparing `tmp/dscontexai-1.0.6.tar.gz` & `tmp/dscontexai-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-1.0.6.tar", last modified: Sun May 26 19:46:26 2024, max compression
+gzip compressed data, was "dscontexai-1.0.7.tar", last modified: Sun May 26 19:47:32 2024, max compression
```

## Comparing `dscontexai-1.0.6.tar` & `dscontexai-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:46:26.970984 dscontexai-1.0.6/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     5226 2024-05-26 19:46:26.970984 dscontexai-1.0.6/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:46:26.966984 dscontexai-1.0.6/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-1.0.6/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-1.0.6/dscontexai/dsc_grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-1.0.6/dscontexai/dsc_ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-1.0.6/dscontexai/dsc_xgboost.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     4653 2024-05-26 17:39:32.000000 dscontexai-1.0.6/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-1.0.6/dscontexai/grammar_with_box_latex.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:46:26.966984 dscontexai-1.0.6/dscontexai/latex/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-1.0.6/dscontexai/latex/neurips_2023.sty
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:46:26.966984 dscontexai-1.0.6/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     5226 2024-05-26 19:46:26.000000 dscontexai-1.0.6/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 19:46:26.000000 dscontexai-1.0.6/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 19:46:26.000000 dscontexai-1.0.6/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 19:46:26.000000 dscontexai-1.0.6/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 19:46:26.000000 dscontexai-1.0.6/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 19:46:26.970984 dscontexai-1.0.6/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     6462 2024-05-26 19:46:18.000000 dscontexai-1.0.6/setup.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:47:32.724539 dscontexai-1.0.7/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     5226 2024-05-26 19:47:32.724539 dscontexai-1.0.7/PKG-INFO
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:47:32.720539 dscontexai-1.0.7/dscontexai/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-1.0.7/dscontexai/__init__.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-1.0.7/dscontexai/dsc_grammar.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-1.0.7/dscontexai/dsc_ploting.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-1.0.7/dscontexai/dsc_xgboost.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     4653 2024-05-26 17:39:32.000000 dscontexai-1.0.7/dscontexai/generate_report.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-1.0.7/dscontexai/grammar_with_box_latex.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:47:32.724539 dscontexai-1.0.7/dscontexai/latex/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-1.0.7/dscontexai/latex/neurips_2023.sty
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:47:32.724539 dscontexai-1.0.7/dscontexai.egg-info/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     5226 2024-05-26 19:47:32.000000 dscontexai-1.0.7/dscontexai.egg-info/PKG-INFO
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 19:47:32.000000 dscontexai-1.0.7/dscontexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 19:47:32.000000 dscontexai-1.0.7/dscontexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 19:47:32.000000 dscontexai-1.0.7/dscontexai.egg-info/requires.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 19:47:32.000000 dscontexai-1.0.7/dscontexai.egg-info/top_level.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 19:47:32.724539 dscontexai-1.0.7/setup.cfg
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     6462 2024-05-26 19:47:25.000000 dscontexai-1.0.7/setup.py
```

### Comparing `dscontexai-1.0.6/PKG-INFO` & `dscontexai-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscontexai
-Version: 1.0.6
+Version: 1.0.7
 Summary: Contextualizing model's decisions with natural language explanations.
 Home-page: UNKNOWN
 Author: Jovana V., Haris K., Luka M.
 Author-email: hk8302@student.uni-lj.si
 License: UNKNOWN
 Description: 
         # ConteXAI - Contextualizing model's decisions with natural language explanations
@@ -101,16 +101,16 @@
         
         Working example, as well as the example of the generated report and the configuration file, can be found [here](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic).
          
         #### Examples
         Examples of the generated reports are shown below. Problem domain was diabetes prediction.
         
         <p align="center">
-          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg" alt="Example of a report" width="48%">
-          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg" alt="Example of a report" width="48%">
+          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg" alt="Example of a report" width="60%">
+          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg" alt="Example of a report" width="60%">
         </p>
         
 Keywords: python,first package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dscontexai-1.0.6/dscontexai/dsc_grammar.py` & `dscontexai-1.0.7/dscontexai/dsc_grammar.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.6/dscontexai/dsc_ploting.py` & `dscontexai-1.0.7/dscontexai/dsc_ploting.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.6/dscontexai/dsc_xgboost.py` & `dscontexai-1.0.7/dscontexai/dsc_xgboost.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.6/dscontexai/generate_report.py` & `dscontexai-1.0.7/dscontexai/generate_report.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.6/dscontexai/grammar_with_box_latex.py` & `dscontexai-1.0.7/dscontexai/grammar_with_box_latex.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.6/dscontexai/latex/neurips_2023.sty` & `dscontexai-1.0.7/dscontexai/latex/neurips_2023.sty`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.6/dscontexai.egg-info/PKG-INFO` & `dscontexai-1.0.7/dscontexai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscontexai
-Version: 1.0.6
+Version: 1.0.7
 Summary: Contextualizing model's decisions with natural language explanations.
 Home-page: UNKNOWN
 Author: Jovana V., Haris K., Luka M.
 Author-email: hk8302@student.uni-lj.si
 License: UNKNOWN
 Description: 
         # ConteXAI - Contextualizing model's decisions with natural language explanations
@@ -101,16 +101,16 @@
         
         Working example, as well as the example of the generated report and the configuration file, can be found [here](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic).
          
         #### Examples
         Examples of the generated reports are shown below. Problem domain was diabetes prediction.
         
         <p align="center">
-          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg" alt="Example of a report" width="48%">
-          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg" alt="Example of a report" width="48%">
+          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg" alt="Example of a report" width="60%">
+          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg" alt="Example of a report" width="60%">
         </p>
         
 Keywords: python,first package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dscontexai-1.0.6/dscontexai.egg-info/requires.txt` & `dscontexai-1.0.7/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.6/setup.py` & `dscontexai-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 DESCRIPTION = "Contextualizing model's decisions with natural language explanations."
 LONG_DESCRIPTION = """
 # ConteXAI - Contextualizing model's decisions with natural language explanations
 
 ConteXAI is a Python package developed as part of the Data Science Project Competition 2024. 
 
 The library **links local explainability methods with natural language explanations**, allowing users to gain detailed insights into model predictions.
@@ -97,16 +97,16 @@
 
 Working example, as well as the example of the generated report and the configuration file, can be found [here](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic).
  
 #### Examples
 Examples of the generated reports are shown below. Problem domain was diabetes prediction.
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg" alt="Example of a report" width="48%">
-  <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg" alt="Example of a report" width="48%">
+  <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg" alt="Example of a report" width="60%">
+  <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg" alt="Example of a report" width="60%">
 </p>
 """
 
 # Setting up
 setup(
     name="dscontexai",
     version=VERSION,
```

