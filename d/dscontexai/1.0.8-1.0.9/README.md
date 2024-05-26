# Comparing `tmp/dscontexai-1.0.8.tar.gz` & `tmp/dscontexai-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-1.0.8.tar", last modified: Sun May 26 19:49:11 2024, max compression
+gzip compressed data, was "dscontexai-1.0.9.tar", last modified: Sun May 26 19:51:07 2024, max compression
```

## Comparing `dscontexai-1.0.8.tar` & `dscontexai-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:49:11.023692 dscontexai-1.0.8/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     5154 2024-05-26 19:49:11.023692 dscontexai-1.0.8/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:49:11.019692 dscontexai-1.0.8/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-1.0.8/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-1.0.8/dscontexai/dsc_grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-1.0.8/dscontexai/dsc_ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-1.0.8/dscontexai/dsc_xgboost.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     4653 2024-05-26 17:39:32.000000 dscontexai-1.0.8/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-1.0.8/dscontexai/grammar_with_box_latex.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:49:11.023692 dscontexai-1.0.8/dscontexai/latex/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-1.0.8/dscontexai/latex/neurips_2023.sty
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:49:11.023692 dscontexai-1.0.8/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     5154 2024-05-26 19:49:10.000000 dscontexai-1.0.8/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 19:49:10.000000 dscontexai-1.0.8/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 19:49:10.000000 dscontexai-1.0.8/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 19:49:10.000000 dscontexai-1.0.8/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 19:49:10.000000 dscontexai-1.0.8/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 19:49:11.023692 dscontexai-1.0.8/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     6406 2024-05-26 19:49:03.000000 dscontexai-1.0.8/setup.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:51:07.600329 dscontexai-1.0.9/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     5110 2024-05-26 19:51:07.600329 dscontexai-1.0.9/PKG-INFO
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:51:07.600329 dscontexai-1.0.9/dscontexai/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-1.0.9/dscontexai/__init__.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-1.0.9/dscontexai/dsc_grammar.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-1.0.9/dscontexai/dsc_ploting.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-1.0.9/dscontexai/dsc_xgboost.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     4653 2024-05-26 17:39:32.000000 dscontexai-1.0.9/dscontexai/generate_report.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-1.0.9/dscontexai/grammar_with_box_latex.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:51:07.600329 dscontexai-1.0.9/dscontexai/latex/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-1.0.9/dscontexai/latex/neurips_2023.sty
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:51:07.600329 dscontexai-1.0.9/dscontexai.egg-info/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     5110 2024-05-26 19:51:07.000000 dscontexai-1.0.9/dscontexai.egg-info/PKG-INFO
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 19:51:07.000000 dscontexai-1.0.9/dscontexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 19:51:07.000000 dscontexai-1.0.9/dscontexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 19:51:07.000000 dscontexai-1.0.9/dscontexai.egg-info/requires.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 19:51:07.000000 dscontexai-1.0.9/dscontexai.egg-info/top_level.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 19:51:07.600329 dscontexai-1.0.9/setup.cfg
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     6362 2024-05-26 19:51:00.000000 dscontexai-1.0.9/setup.py
```

### Comparing `dscontexai-1.0.8/PKG-INFO` & `dscontexai-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscontexai
-Version: 1.0.8
+Version: 1.0.9
 Summary: Contextualizing model's decisions with natural language explanations.
 Home-page: UNKNOWN
 Author: Jovana V., Haris K., Luka M.
 Author-email: hk8302@student.uni-lj.si
 License: UNKNOWN
 Description: 
         # ConteXAI - Contextualizing model's decisions with natural language explanations
@@ -100,16 +100,16 @@
         #### Example notebooks
         
         Working example, as well as the example of the generated report and the configuration file, can be found [here](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic).
          
         #### Examples
         Examples of the generated reports are shown below. Problem domain was diabetes prediction.
         
-        ![Example of a generated report]("https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg")
-        ![Example of a generated report]("https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg")
+        ![Example 1](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg)
+        ![Example 2](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg)
         
 Keywords: python,first package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `dscontexai-1.0.8/dscontexai/dsc_grammar.py` & `dscontexai-1.0.9/dscontexai/dsc_grammar.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.8/dscontexai/dsc_ploting.py` & `dscontexai-1.0.9/dscontexai/dsc_ploting.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.8/dscontexai/dsc_xgboost.py` & `dscontexai-1.0.9/dscontexai/dsc_xgboost.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.8/dscontexai/generate_report.py` & `dscontexai-1.0.9/dscontexai/generate_report.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.8/dscontexai/grammar_with_box_latex.py` & `dscontexai-1.0.9/dscontexai/grammar_with_box_latex.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.8/dscontexai/latex/neurips_2023.sty` & `dscontexai-1.0.9/dscontexai/latex/neurips_2023.sty`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.8/dscontexai.egg-info/PKG-INFO` & `dscontexai-1.0.9/dscontexai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscontexai
-Version: 1.0.8
+Version: 1.0.9
 Summary: Contextualizing model's decisions with natural language explanations.
 Home-page: UNKNOWN
 Author: Jovana V., Haris K., Luka M.
 Author-email: hk8302@student.uni-lj.si
 License: UNKNOWN
 Description: 
         # ConteXAI - Contextualizing model's decisions with natural language explanations
@@ -100,16 +100,16 @@
         #### Example notebooks
         
         Working example, as well as the example of the generated report and the configuration file, can be found [here](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic).
          
         #### Examples
         Examples of the generated reports are shown below. Problem domain was diabetes prediction.
         
-        ![Example of a generated report]("https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg")
-        ![Example of a generated report]("https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg")
+        ![Example 1](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg)
+        ![Example 2](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg)
         
 Keywords: python,first package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `dscontexai-1.0.8/dscontexai.egg-info/requires.txt` & `dscontexai-1.0.9/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.8/setup.py` & `dscontexai-1.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 DESCRIPTION = "Contextualizing model's decisions with natural language explanations."
 LONG_DESCRIPTION = """
 # ConteXAI - Contextualizing model's decisions with natural language explanations
 
 ConteXAI is a Python package developed as part of the Data Science Project Competition 2024. 
 
 The library **links local explainability methods with natural language explanations**, allowing users to gain detailed insights into model predictions.
@@ -96,16 +96,16 @@
 #### Example notebooks
 
 Working example, as well as the example of the generated report and the configuration file, can be found [here](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic).
  
 #### Examples
 Examples of the generated reports are shown below. Problem domain was diabetes prediction.
 
-![Example of a generated report]("https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg")
-![Example of a generated report]("https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg")
+![Example 1](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_10_page-0001.jpg)
+![Example 2](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/main/other/output_4130_page-0001.jpg)
 """
 
 # Setting up
 setup(
     name="dscontexai",
     version=VERSION,
     author="Jovana V., Haris K., Luka M.",
```

