# Comparing `tmp/dscontexai-0.1.1.tar.gz` & `tmp/dscontexai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-0.1.1.tar", last modified: Sun May 26 17:13:22 2024, max compression
+gzip compressed data, was "dscontexai-1.0.0.tar", last modified: Sun May 26 17:41:04 2024, max compression
```

## Comparing `dscontexai-0.1.1.tar` & `dscontexai-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:13:22.039013 dscontexai-0.1.1/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3252 2024-05-26 17:13:22.039013 dscontexai-0.1.1/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:13:22.039013 dscontexai-0.1.1/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-0.1.1/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-0.1.1/dscontexai/dsc_grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-0.1.1/dscontexai/dsc_ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-0.1.1/dscontexai/dsc_xgboost.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     6111 2024-05-26 17:01:06.000000 dscontexai-0.1.1/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-0.1.1/dscontexai/grammar_with_box_latex.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:13:22.039013 dscontexai-0.1.1/dscontexai/latex/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-0.1.1/dscontexai/latex/neurips_2023.sty
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:13:22.039013 dscontexai-0.1.1/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3252 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 17:13:22.039013 dscontexai-0.1.1/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     4808 2024-05-26 17:13:12.000000 dscontexai-0.1.1/setup.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:41:04.837477 dscontexai-1.0.0/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3252 2024-05-26 17:41:04.837477 dscontexai-1.0.0/PKG-INFO
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:41:04.837477 dscontexai-1.0.0/dscontexai/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-1.0.0/dscontexai/__init__.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-1.0.0/dscontexai/dsc_grammar.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-1.0.0/dscontexai/dsc_ploting.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-1.0.0/dscontexai/dsc_xgboost.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     4653 2024-05-26 17:39:32.000000 dscontexai-1.0.0/dscontexai/generate_report.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-1.0.0/dscontexai/grammar_with_box_latex.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:41:04.837477 dscontexai-1.0.0/dscontexai/latex/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-1.0.0/dscontexai/latex/neurips_2023.sty
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:41:04.837477 dscontexai-1.0.0/dscontexai.egg-info/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3252 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/PKG-INFO
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/requires.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 17:41:04.000000 dscontexai-1.0.0/dscontexai.egg-info/top_level.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 17:41:04.837477 dscontexai-1.0.0/setup.cfg
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     4808 2024-05-26 17:41:02.000000 dscontexai-1.0.0/setup.py
```

### Comparing `dscontexai-0.1.1/PKG-INFO` & `dscontexai-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscontexai
-Version: 0.1.1
+Version: 1.0.0
 Summary: Contextualizing model's decisions with natural language explanations.
 Home-page: UNKNOWN
 Author: Jovana V., Haris K., Luka M.
 Author-email: <youremail@email.com>
 License: UNKNOWN
 Description: 
         ## Project description
```

### Comparing `dscontexai-0.1.1/dscontexai/dsc_grammar.py` & `dscontexai-1.0.0/dscontexai/dsc_grammar.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.1.1/dscontexai/dsc_ploting.py` & `dscontexai-1.0.0/dscontexai/dsc_ploting.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.1.1/dscontexai/dsc_xgboost.py` & `dscontexai-1.0.0/dscontexai/dsc_xgboost.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.1.1/dscontexai/generate_report.py` & `dscontexai-1.0.0/dscontexai/generate_report.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,34 @@
 import argparse
 import json
 import pickle
 
 import pandas as pd
 import shap
+import xgboost as xgb
 from catboost import CatBoostClassifier
+from sklearn.ensemble import RandomForestClassifier
 
 from dscontexai.dsc_grammar import analyze_shap_values
 
 
+def get_shap(model, X: pd.DataFrame, index: int) -> shap.Explainer:
+    if isinstance(model, xgb.XGBClassifier):
+        explainer = shap.Explainer(model, X, model_output="probability")
+        shap_values = explainer(X.iloc[index])
+    else:
+        explainer = shap.KernelExplainer(model.predict_proba, shap.sample(X, 1000))
+        shap_values = explainer(X.iloc[index])
+        if shap_values.values.shape[1] == 2:
+            shap_values.values = shap_values.values[:, 1]
+            shap_values.base_values = shap_values.base_values[:, 1][0]
+
+    return shap_values
+
+
 def diabetes_case() -> None:
     """
     Load the diabetes model and data, and generate a report for a specific instance.
     """
     df = pd.read_csv("./kaggle_data/processed_data.csv")
     X = df.drop(columns=["diabetes"])
     y = df["diabetes"]
@@ -52,64 +68,14 @@
         below_optimal_descriptions,
         optimal_descriptions,
         above_optimal_descriptions,
         transformations,
     )
 
 
-def insurance_case() -> None:
-    """
-    Load the insurance model and data, and generate a report for a specific instance.
-    """
-
-    df = pd.read_csv("../../malaysia_churn_model/data/data_sample.csv", index_col=0)
-
-    # Load churn prediction model
-    model = CatBoostClassifier()
-    model.load_model("../../malaysia_churn_model/model/gigt_model_exp1.bin")
-
-    # Expert descriptions for values below, within, and above optimal ranges
-    # read from json file
-    with open("./configurations/insurance.json") as f:
-        data = json.load(f)
-
-    optimal_values = data["optimal_values"]
-    below_optimal_descriptions = data["descriptions"]["below_optimal"]
-    optimal_descriptions = data["descriptions"]["optimal"]
-    above_optimal_descriptions = data["descriptions"]["above_optimal"]
-
-    transformations = data["transformation"]
-
-    feature_names = data["feature_names"]
-    target1 = data["target1"]
-    target2 = data["target2"]
-    supporting = data["supporting"]
-    index = data["index"]
-
-    explainer = shap.KernelExplainer(model.predict_proba, shap.sample(df, 5))
-    shap_values_array = explainer(df.iloc[index])
-
-    shap_values_array.values = shap_values_array.values[:, 1]
-    shap_values_array.base_values = shap_values_array.base_values[1]
-
-    analyze_shap_values(
-        shap_values_array,
-        index,
-        target1,
-        target2,
-        feature_names,
-        supporting,
-        optimal_values,
-        below_optimal_descriptions,
-        optimal_descriptions,
-        above_optimal_descriptions,
-        transformations,
-    )
-
-
 def general(model_path, dataset_path, config, idx):
     """
     Load the insurance model and data, and generate a report for a specific instance.
     """
 
     # Load prediction model
     with open(model_path, "rb") as f:
@@ -132,16 +98,15 @@
     target2 = data["target2"]
     supporting = data["supporting"]
 
     df = pd.read_csv(dataset_path)
     X = df.drop(columns=[target1])
     y = df[target1]
 
-    explainer = shap.Explainer(model, X, model_output="probability")
-    shap_values_array = explainer(X.iloc[idx])
+    shap_values_array = get_shap(model, X, idx)
 
     analyze_shap_values(
         shap_values_array,
         idx,
         target1,
         target2,
         feature_names,
@@ -153,39 +118,34 @@
         transformations,
     )
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Automatic Report Generator for xAI")
 
-    parser.add_argument("--domain", help="Dataset domain", action="store", default="diabetes")
     parser.add_argument("--instance", help="Instance index", action="store", default=1, type=int)
     parser.add_argument("--model", help="Model path", action="store", default=None)
     parser.add_argument("--dataset", help="Data path", action="store", default=None)
     parser.add_argument("--config", help="Config path", action="store", default=None)
     parser.add_argument("--index", help="Instance index", action="store", default=1, type=int)
+    parser.add_argument(
+        "--example",
+        help="Shows working example of the library",
+        action="store_true",
+        required=False,
+    )
 
     args = parser.parse_args()
 
     if args.index < 0:
         print("Index has to be positive!")
         exit()
-    if args.domain not in ["diabetes", "insurance"]:
-        print("Invalid domain. Please enter either 'diabetes' or 'insurance'.")
-        exit()
 
-    if args.domain == "diabetes":
+    if args.example:
         model_path = "./models/diabetes_model.pkl"
         df = pd.read_csv("./kaggle_data/processed_data.csv")
         diabetes_case()
-    elif args.domain == "insurance":
-        model_path = "../../malaysia_churn_model/model/gigt_model_exp1.bin"
-        df = pd.read_csv("../../malaysia_churn_model/data/data_sample.csv", index_col=0)
-        insurance_case()
-    elif args.domain == "general":
+    else:
         model_path = args.model
         data = args.dataset
         config = args.config
         general(model_path, data, config, args.index)
-    else:
-        print("Invalid domain. Please enter either 'diabetes', 'insurance' or 'general'.")
-        exit()
```

### Comparing `dscontexai-0.1.1/dscontexai/grammar_with_box_latex.py` & `dscontexai-1.0.0/dscontexai/grammar_with_box_latex.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.1.1/dscontexai/latex/neurips_2023.sty` & `dscontexai-1.0.0/dscontexai/latex/neurips_2023.sty`

 * *Files identical despite different names*

### Comparing `dscontexai-0.1.1/dscontexai.egg-info/PKG-INFO` & `dscontexai-1.0.0/dscontexai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dscontexai
-Version: 0.1.1
+Version: 1.0.0
 Summary: Contextualizing model's decisions with natural language explanations.
 Home-page: UNKNOWN
 Author: Jovana V., Haris K., Luka M.
 Author-email: <youremail@email.com>
 License: UNKNOWN
 Description: 
         ## Project description
```

### Comparing `dscontexai-0.1.1/dscontexai.egg-info/requires.txt` & `dscontexai-1.0.0/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-0.1.1/setup.py` & `dscontexai-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.1.1"
+VERSION = "1.0.0"
 DESCRIPTION = "Contextualizing model's decisions with natural language explanations."
 LONG_DESCRIPTION = """
 ## Project description
 DSConteXAI is a Python package developed as part of the Data Science Project Competition 2024. 
 
 It **links local explainability methods with natural language explanations**, allowing users to gain detailed insights into model predictions.
 By incorporating additional domain knowledge, users can obtain even more detailed insights into the model's predictions.
```

