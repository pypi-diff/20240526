# Comparing `tmp/dscontexai-1.0.0.tar.gz` & `tmp/dscontexai-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-1.0.0.tar", last modified: Sun May 26 17:41:04 2024, max compression
+gzip compressed data, was "dscontexai-1.0.1.tar", last modified: Sun May 26 19:31:31 2024, max compression
```

## Comparing `dscontexai-1.0.0.tar` & `dscontexai-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:41:04.837477 dscontexai-1.0.0/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3252 2024-05-26 17:41:04.837477 dscontexai-1.0.0/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:41:04.837477 dscontexai-1.0.0/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-1.0.0/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-1.0.0/dscontexai/dsc_grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-1.0.0/dscontexai/dsc_ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-1.0.0/dscontexai/dsc_xgboost.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     4653 2024-05-26 17:39:32.000000 dscontexai-1.0.0/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-1.0.0/dscontexai/grammar_with_box_latex.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:41:04.837477 dscontexai-1.0.0/dscontexai/latex/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-1.0.0/dscontexai/latex/neurips_2023.sty
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:41:04.837477 dscontexai-1.0.0/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3252 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 17:41:04.837477 dscontexai-1.0.0/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     4808 2024-05-26 17:41:02.000000 dscontexai-1.0.0/setup.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:31:31.792311 dscontexai-1.0.1/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     5128 2024-05-26 19:31:31.792311 dscontexai-1.0.1/PKG-INFO
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:31:31.788312 dscontexai-1.0.1/dscontexai/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-1.0.1/dscontexai/__init__.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-1.0.1/dscontexai/dsc_grammar.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-1.0.1/dscontexai/dsc_ploting.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-1.0.1/dscontexai/dsc_xgboost.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     4653 2024-05-26 17:39:32.000000 dscontexai-1.0.1/dscontexai/generate_report.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-1.0.1/dscontexai/grammar_with_box_latex.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:31:31.788312 dscontexai-1.0.1/dscontexai/latex/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-1.0.1/dscontexai/latex/neurips_2023.sty
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 19:31:31.788312 dscontexai-1.0.1/dscontexai.egg-info/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     5128 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/PKG-INFO
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/requires.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 19:31:31.000000 dscontexai-1.0.1/dscontexai.egg-info/top_level.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 19:31:31.792311 dscontexai-1.0.1/setup.cfg
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     6372 2024-05-26 19:31:26.000000 dscontexai-1.0.1/setup.py
```

### Comparing `dscontexai-1.0.0/dscontexai/dsc_grammar.py` & `dscontexai-1.0.1/dscontexai/dsc_grammar.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.0/dscontexai/dsc_ploting.py` & `dscontexai-1.0.1/dscontexai/dsc_ploting.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.0/dscontexai/dsc_xgboost.py` & `dscontexai-1.0.1/dscontexai/dsc_xgboost.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.0/dscontexai/generate_report.py` & `dscontexai-1.0.1/dscontexai/generate_report.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.0/dscontexai/grammar_with_box_latex.py` & `dscontexai-1.0.1/dscontexai/grammar_with_box_latex.py`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.0/dscontexai/latex/neurips_2023.sty` & `dscontexai-1.0.1/dscontexai/latex/neurips_2023.sty`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.0/dscontexai.egg-info/requires.txt` & `dscontexai-1.0.1/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-1.0.0/setup.py` & `dscontexai-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 from setuptools import find_packages, setup
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = "Contextualizing model's decisions with natural language explanations."
 LONG_DESCRIPTION = """
+# ConteXAI - Contextualizing model's decisions with natural language explanations
+
 ## Project description
-DSConteXAI is a Python package developed as part of the Data Science Project Competition 2024. 
+ConteXAI is a Python package developed as part of the Data Science Project Competition 2024. 
 
-It **links local explainability methods with natural language explanations**, allowing users to gain detailed insights into model predictions.
-By incorporating additional domain knowledge, users can obtain even more detailed insights into the model's predictions.
+The library **links local explainability methods with natural language explanations**, allowing users to gain detailed insights into model predictions.
+By incorporating additional domain knowledge, users can obtain even better insights into the model's predictions.
 
 ### Install
 
-DSConteXAI can be installed using pip:
+ConteXAI can be installed using pip:
 ```bash
 pip install dscontexai
 ```
 
-
 ### Generate XAI reports
-Using this package, you can fully automatically develop your XAI reports. Currently, it supports SHAP values, which is a local feature importance measure, to which we added textual explanations and domain-related context.
 
-SHAP values can be calculated for a variety of models, including the most popular ensemble models: XGBoost, CatBoost, and Random Forest. To use this tool with your dataset, you need to provide a configuration JSON file for a dataset, structured like the one below.
+Using this library, you can fully automatically develop your XAI reports. Currently, it supports SHAP values, which is a local feature importance measure, to which we added textual explanations and domain-related context.
+The library can be used for binary classification problems, for all models that output probabilities.
+
+The report consists of four main segments: 
+
+  (1) Description of local feature importances, 
+
+  (2) Explanation of the instance's prediction, 
+
+  (3) Visualization of local feature importances, 
+  
+  (4) Explanation of the visualization in natural language and context related to the domain and the prediction. 
+
+<p align="center">
+  <img src="https://github.com/jovanavidenovic/ConteXAI/blob/main/other/XAI_2_page-0001.jpg" alt="Report structure" width="85%">
+</p>
+
+### Preparing configuration file
+To use this tool with your model and dataset, you need to provide a configuration JSON file for a dataset, structured like the one below.
 
 ```bash
 {
   # domain-based context
   "optimal_values": [
   ...
     [0, 6.5],               # HbA1c level optimal range is from 0 to 6.5
@@ -60,22 +78,43 @@
   ],
   # variables needed for structuring the description
   "target1": "diabetes",    # Target variable the model is predicting
   "target2": "Person",      # The object representing a sample in a data
   "supporting": ["does", "have"]  # Supporting verbs used in descriptions
 }
 ```
+
+#### Running the generation
+Once you have model, dataset, and config file ready, to generate the report, you can use the following code snippet:
+  
+  ```python
+  from dscontexai.generate_report import general
+
+  general.generate_report(model_path= "path/to/model.pkl", dataset_path="path/to/data.csv", config="path/to/config.json", idx=sample_idx)
+  ```
+
+After successful generation, you will find a PDF report in the directory prototype/ under the name output_{sample_idx}.pdf.
+
+#### Example notebooks
+
+Working example, as well as the example of the generated report and the configuration file, can be found here: [Example notebook](https://github.com/jovanavidenovic/ConteXAI/tree/main/titanic)
+ 
+#### Examples
+Examples of the generated reports are shown below. Problem domain was diabetes prediction.
+
+![Example 1](https://github.com/jovanavidenovic/ConteXAI/blob/main/other/output_10_page-0001.jpg)
+![Example 2](https://github.com/jovanavidenovic/ConteXAI/blob/main/other/output_4130_page-0001.jpg)
 """
 
 # Setting up
 setup(
     name="dscontexai",
     version=VERSION,
     author="Jovana V., Haris K., Luka M.",
-    author_email="<youremail@email.com>",
+    author_email="hk8302@student.uni-lj.si",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     package_data={"dscontexai": ["latex/neurips_2023.sty"]},
     install_requires=[
         "asttokens==2.4.1",
         "backcall==0.2.0",
```

