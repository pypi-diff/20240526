# Comparing `tmp/dscontexai-1.0.1.tar.gz` & `tmp/dscontexai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-1.0.1.tar", last modified: Sun May 26 19:31:31 2024, max compression
+gzip compressed data, was "dscontexai-1.0.2.tar", last modified: Sun May 26 19:37:44 2024, max compression
```

## Comparing `dscontexai-1.0.1.tar` & `dscontexai-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:31:31.792311 dscontexai-1.0.1/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     5128 2024-05-26 19:31:31.792311 dscontexai-1.0.1/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:31:31.788312 dscontexai-1.0.1/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-1.0.1/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-1.0.1/dscontexai/dsc_grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-1.0.1/dscontexai/dsc_ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-1.0.1/dscontexai/dsc_xgboost.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     4653 2024-05-26 17:39:32.000000 dscontexai-1.0.1/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-1.0.1/dscontexai/grammar_with_box_latex.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:31:31.788312 dscontexai-1.0.1/dscontexai/latex/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-1.0.1/dscontexai/latex/neurips_2023.sty
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:31:31.788312 dscontexai-1.0.1/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     5128 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 19:31:31.792311 dscontexai-1.0.1/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     6372 2024-05-26 19:31:26.000000 dscontexai-1.0.1/setup.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:37:44.829717 dscontexai-1.0.2/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     5156 2024-05-26 19:37:44.829717 dscontexai-1.0.2/PKG-INFO
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:37:44.825717 dscontexai-1.0.2/dscontexai/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-1.0.2/dscontexai/__init__.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-1.0.2/dscontexai/dsc_grammar.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-1.0.2/dscontexai/dsc_ploting.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-1.0.2/dscontexai/dsc_xgboost.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     4653 2024-05-26 17:39:32.000000 dscontexai-1.0.2/dscontexai/generate_report.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-1.0.2/dscontexai/grammar_with_box_latex.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:37:44.829717 dscontexai-1.0.2/dscontexai/latex/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-1.0.2/dscontexai/latex/neurips_2023.sty
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:37:44.829717 dscontexai-1.0.2/dscontexai.egg-info/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     5156 2024-05-26 19:37:44.000000 dscontexai-1.0.2/dscontexai.egg-info/PKG-INFO
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 19:37:44.000000 dscontexai-1.0.2/dscontexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 19:37:44.000000 dscontexai-1.0.2/dscontexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 19:37:44.000000 dscontexai-1.0.2/dscontexai.egg-info/requires.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 19:37:44.000000 dscontexai-1.0.2/dscontexai.egg-info/top_level.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 19:37:44.829717 dscontexai-1.0.2/setup.cfg
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     6400 2024-05-26 19:37:30.000000 dscontexai-1.0.2/setup.py
```

### Comparing `dscontexai-1.0.1/PKG-INFO` & `dscontexai-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscontexai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Contextualizing model's decisions with natural language explanations.
 Home-page: UNKNOWN
 Author: Jovana V., Haris K., Luka M.
 Author-email: hk8302@student.uni-lj.si
 License: UNKNOWN
 Description: 
         # ConteXAI - Contextualizing model's decisions with natural language explanations
@@ -34,15 +34,15 @@
           (2) Explanation of the instance's prediction, 
         
           (3) Visualization of local feature importances, 
           
           (4) Explanation of the visualization in natural language and context related to the domain and the prediction. 
         
         <p align="center">
-          <img src="https://github.com/jovanavidenovic/ConteXAI/blob/main/other/XAI_2_page-0001.jpg" alt="Report structure" width="85%">
+          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/blob/main/other/XAI_2_page-0001.jpg" alt="Report structure" width="85%">
         </p>
         
         ### Preparing configuration file
         To use this tool with your model and dataset, you need to provide a configuration JSON file for a dataset, structured like the one below.
         
         ```bash
         {
@@ -96,21 +96,21 @@
           general.generate_report(model_path= "path/to/model.pkl", dataset_path="path/to/data.csv", config="path/to/config.json", idx=sample_idx)
           ```
         
         After successful generation, you will find a PDF report in the directory prototype/ under the name output_{sample_idx}.pdf.
         
         #### Example notebooks
         
-        Working example, as well as the example of the generated report and the configuration file, can be found here: [Example notebook](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic)
+        Working example, as well as the example of the generated report and the configuration file, can be found [here](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic).
          
         #### Examples
         Examples of the generated reports are shown below. Problem domain was diabetes prediction.
         
-        ![Example 1](https://github.com/jovanavidenovic/ConteXAI/blob/main/other/output_10_page-0001.jpg)
-        ![Example 2](https://github.com/jovanavidenovic/ConteXAI/blob/main/other/output_4130_page-0001.jpg)
+        ![Example 1](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/blob/main/other/output_10_page-0001.jpg)
+        ![Example 2](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/blob/main/other/output_4130_page-0001.jpg)
         
 Keywords: python,first package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `dscontexai-1.0.1/dscontexai/dsc_grammar.py` & `dscontexai-1.0.2/dscontexai/dsc_grammar.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.1/dscontexai/dsc_ploting.py` & `dscontexai-1.0.2/dscontexai/dsc_ploting.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.1/dscontexai/dsc_xgboost.py` & `dscontexai-1.0.2/dscontexai/dsc_xgboost.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.1/dscontexai/generate_report.py` & `dscontexai-1.0.2/dscontexai/generate_report.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.1/dscontexai/grammar_with_box_latex.py` & `dscontexai-1.0.2/dscontexai/grammar_with_box_latex.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.1/dscontexai/latex/neurips_2023.sty` & `dscontexai-1.0.2/dscontexai/latex/neurips_2023.sty`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.1/dscontexai.egg-info/PKG-INFO` & `dscontexai-1.0.2/dscontexai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscontexai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Contextualizing model's decisions with natural language explanations.
 Home-page: UNKNOWN
 Author: Jovana V., Haris K., Luka M.
 Author-email: hk8302@student.uni-lj.si
 License: UNKNOWN
 Description: 
         # ConteXAI - Contextualizing model's decisions with natural language explanations
@@ -34,15 +34,15 @@
           (2) Explanation of the instance's prediction, 
         
           (3) Visualization of local feature importances, 
           
           (4) Explanation of the visualization in natural language and context related to the domain and the prediction. 
         
         <p align="center">
-          <img src="https://github.com/jovanavidenovic/ConteXAI/blob/main/other/XAI_2_page-0001.jpg" alt="Report structure" width="85%">
+          <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/blob/main/other/XAI_2_page-0001.jpg" alt="Report structure" width="85%">
         </p>
         
         ### Preparing configuration file
         To use this tool with your model and dataset, you need to provide a configuration JSON file for a dataset, structured like the one below.
         
         ```bash
         {
@@ -96,21 +96,21 @@
           general.generate_report(model_path= "path/to/model.pkl", dataset_path="path/to/data.csv", config="path/to/config.json", idx=sample_idx)
           ```
         
         After successful generation, you will find a PDF report in the directory prototype/ under the name output_{sample_idx}.pdf.
         
         #### Example notebooks
         
-        Working example, as well as the example of the generated report and the configuration file, can be found here: [Example notebook](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic)
+        Working example, as well as the example of the generated report and the configuration file, can be found [here](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic).
          
         #### Examples
         Examples of the generated reports are shown below. Problem domain was diabetes prediction.
         
-        ![Example 1](https://github.com/jovanavidenovic/ConteXAI/blob/main/other/output_10_page-0001.jpg)
-        ![Example 2](https://github.com/jovanavidenovic/ConteXAI/blob/main/other/output_4130_page-0001.jpg)
+        ![Example 1](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/blob/main/other/output_10_page-0001.jpg)
+        ![Example 2](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/blob/main/other/output_4130_page-0001.jpg)
         
 Keywords: python,first package
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `dscontexai-1.0.1/dscontexai.egg-info/requires.txt` & `dscontexai-1.0.2/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.1/setup.py` & `dscontexai-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "Contextualizing model's decisions with natural language explanations."
 LONG_DESCRIPTION = """
 # ConteXAI - Contextualizing model's decisions with natural language explanations
 
 ## Project description
 ConteXAI is a Python package developed as part of the Data Science Project Competition 2024. 
 
@@ -30,15 +30,15 @@
   (2) Explanation of the instance's prediction, 
 
   (3) Visualization of local feature importances, 
   
   (4) Explanation of the visualization in natural language and context related to the domain and the prediction. 
 
 <p align="center">
-  <img src="https://github.com/jovanavidenovic/ConteXAI/blob/main/other/XAI_2_page-0001.jpg" alt="Report structure" width="85%">
+  <img src="https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/blob/main/other/XAI_2_page-0001.jpg" alt="Report structure" width="85%">
 </p>
 
 ### Preparing configuration file
 To use this tool with your model and dataset, you need to provide a configuration JSON file for a dataset, structured like the one below.
 
 ```bash
 {
@@ -92,21 +92,21 @@
   general.generate_report(model_path= "path/to/model.pkl", dataset_path="path/to/data.csv", config="path/to/config.json", idx=sample_idx)
   ```
 
 After successful generation, you will find a PDF report in the directory prototype/ under the name output_{sample_idx}.pdf.
 
 #### Example notebooks
 
-Working example, as well as the example of the generated report and the configuration file, can be found here: [Example notebook](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic)
+Working example, as well as the example of the generated report and the configuration file, can be found [here](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic).
  
 #### Examples
 Examples of the generated reports are shown below. Problem domain was diabetes prediction.
 
-![Example 1](https://github.com/jovanavidenovic/ConteXAI/blob/main/other/output_10_page-0001.jpg)
-![Example 2](https://github.com/jovanavidenovic/ConteXAI/blob/main/other/output_4130_page-0001.jpg)
+![Example 1](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/blob/main/other/output_10_page-0001.jpg)
+![Example 2](https://raw.githubusercontent.com/jovanavidenovic/ConteXAI/blob/main/other/output_4130_page-0001.jpg)
 """
 
 # Setting up
 setup(
     name="dscontexai",
     version=VERSION,
     author="Jovana V., Haris K., Luka M.",
```

