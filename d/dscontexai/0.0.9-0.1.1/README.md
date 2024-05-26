# Comparing `tmp/dscontexai-0.0.9.tar.gz` & `tmp/dscontexai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-0.0.9.tar", last modified: Sun May 26 15:11:18 2024, max compression
+gzip compressed data, was "dscontexai-0.1.1.tar", last modified: Sun May 26 17:13:22 2024, max compression
```

## Comparing `dscontexai-0.0.9.tar` & `dscontexai-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 15:11:18.736042 dscontexai-0.0.9/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 15:11:18.736042 dscontexai-0.0.9/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 15:11:18.736042 dscontexai-0.0.9/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       85 2024-05-26 14:00:13.000000 dscontexai-0.0.9/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10558 2024-05-26 15:03:11.000000 dscontexai-0.0.9/dscontexai/dsc_grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3569 2024-05-26 15:04:21.000000 dscontexai-0.0.9/dscontexai/dsc_ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-0.0.9/dscontexai/dsc_xgboost.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     6117 2024-05-26 14:40:34.000000 dscontexai-0.0.9/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-0.0.9/dscontexai/grammar_with_box_latex.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 15:11:18.736042 dscontexai-0.0.9/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 15:11:18.000000 dscontexai-0.0.9/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      345 2024-05-26 15:11:18.000000 dscontexai-0.0.9/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 15:11:18.000000 dscontexai-0.0.9/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1059 2024-05-26 15:11:18.000000 dscontexai-0.0.9/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 15:11:18.000000 dscontexai-0.0.9/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 15:11:18.736042 dscontexai-0.0.9/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     2454 2024-05-26 15:11:03.000000 dscontexai-0.0.9/setup.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:13:22.039013 dscontexai-0.1.1/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3252 2024-05-26 17:13:22.039013 dscontexai-0.1.1/PKG-INFO
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:13:22.039013 dscontexai-0.1.1/dscontexai/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      112 2024-05-26 17:06:58.000000 dscontexai-0.1.1/dscontexai/__init__.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11270 2024-05-26 17:08:54.000000 dscontexai-0.1.1/dscontexai/dsc_grammar.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3641 2024-05-26 17:03:49.000000 dscontexai-0.1.1/dscontexai/dsc_ploting.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-0.1.1/dscontexai/dsc_xgboost.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     6111 2024-05-26 17:01:06.000000 dscontexai-0.1.1/dscontexai/generate_report.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-0.1.1/dscontexai/grammar_with_box_latex.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:13:22.039013 dscontexai-0.1.1/dscontexai/latex/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    11461 2024-05-26 15:10:26.000000 dscontexai-0.1.1/dscontexai/latex/neurips_2023.sty
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 17:13:22.039013 dscontexai-0.1.1/dscontexai.egg-info/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3252 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/PKG-INFO
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      379 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1074 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/requires.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 17:13:21.000000 dscontexai-0.1.1/dscontexai.egg-info/top_level.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 17:13:22.039013 dscontexai-0.1.1/setup.cfg
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     4808 2024-05-26 17:13:12.000000 dscontexai-0.1.1/setup.py
```

### Comparing `dscontexai-0.0.9/dscontexai/dsc_grammar.py` & `dscontexai-0.1.1/dscontexai/dsc_grammar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,42 @@
 import os
+import shutil
 
 import matplotlib.pyplot as plt
 import numpy as np
+import pkg_resources
 import shap
 from pylatex import Document, Figure, Itemize, NoEscape, Package, Section, Subsection
 from pylatex.utils import bold
 
 from dscontexai.dsc_ploting import plot_shap
 
 plt.rcParams["text.usetex"] = True
 
 
+def extract_neur_sty(target_directory):
+    # Ensure the target directory exists
+    if not os.path.exists(target_directory):
+        os.makedirs(target_directory)
+
+    # Get the path to neur.sty within the package
+    sty_path = pkg_resources.resource_filename("dscontexai", "latex/neurips_2023.sty")
+
+    # Define the target path where the file should be copied
+    target_path = os.path.join(target_directory, "neurips_2023.sty")
+
+    # Copy the file to the target directory
+    shutil.copyfile(sty_path, target_path)
+
+    return target_path
+
+
+extracted_path = extract_neur_sty("./latex/")
+
+
 def fixing_variable_names(variables: list) -> list:
     """
     Fix the variable names by removing underscores and capitalizing the first letter of each word.
 
     Parameters
     ----------
     variables : list
@@ -236,15 +258,16 @@
     sorted_features = [feature_values_named[i] for i in sorted_indices]
     sorted_shap_values = [shap_values[i] for i in sorted_indices]
 
     # Set up the plot
     plot_shap(sorted_shap_values, sorted_features, "./plots/shap.pdf")
 
     doc = Document(documentclass="article", document_options="a4paper", page_numbers=False)
-    doc.preamble.append(NoEscape(r"\usepackage{../latex/neurips_2023}"))
+    nips_style = pkg_resources.resource_filename("dscontexai", "latex/neurips_2023")
+    doc.preamble.append(NoEscape(r"\usepackage{" + nips_style + "}"))
     doc.preamble.append(NoEscape(r"\usepackage{setspace}"))
     doc.packages.append(Package("graphicx"))
     doc.packages.append(Package("enumitem"))
 
     # Adding a section without numbering
     with doc.create(Section("Feature importance with included context and text", numbering=False)):
```

### Comparing `dscontexai-0.0.9/dscontexai/dsc_ploting.py` & `dscontexai-0.1.1/dscontexai/dsc_ploting.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,9 +112,11 @@
     for spine in ["left", "bottom"]:
         ax.spines[spine].set_linewidth(1.2)
 
     fig.tight_layout()
 
     if os.path.exists(fig_path):
         os.remove(fig_path)
+    else:
+        os.makedirs(os.path.dirname(fig_path), exist_ok=True)
 
     fig.savefig(fig_path, format="pdf")
```

### Comparing `dscontexai-0.0.9/dscontexai/dsc_xgboost.py` & `dscontexai-0.1.1/dscontexai/dsc_xgboost.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.9/dscontexai/generate_report.py` & `dscontexai-0.1.1/dscontexai/generate_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,18 +107,14 @@
 
 
 def general(model_path, dataset_path, config, idx):
     """
     Load the insurance model and data, and generate a report for a specific instance.
     """
 
-    df = pd.read_csv(dataset_path)
-    X = df.drop(columns=["diabetes"])
-    y = df["diabetes"]
-
     # Load prediction model
     with open(model_path, "rb") as f:
         model = pickle.load(f)
 
     # Expert descriptions for values below, within, and above optimal ranges
     # read from json file
     with open(config) as f:
@@ -132,14 +128,18 @@
     transformations = data["transformation"]
 
     feature_names = data["feature_names"]
     target1 = data["target1"]
     target2 = data["target2"]
     supporting = data["supporting"]
 
+    df = pd.read_csv(dataset_path)
+    X = df.drop(columns=[target1])
+    y = df[target1]
+
     explainer = shap.Explainer(model, X, model_output="probability")
     shap_values_array = explainer(X.iloc[idx])
 
     analyze_shap_values(
         shap_values_array,
         idx,
         target1,
```

### Comparing `dscontexai-0.0.9/dscontexai/grammar_with_box_latex.py` & `dscontexai-0.1.1/dscontexai/grammar_with_box_latex.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.9/dscontexai.egg-info/requires.txt` & `dscontexai-0.1.1/dscontexai.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -55,8 +55,9 @@
 threadpoolctl==3.4.0
 tornado==6.4
 tqdm==4.66.2
 traitlets==5.14.2
 typing-extensions==4.11.0
 tzdata==2024.1
 wcwidth==0.2.13
+xgboost==2.0.3
 zipp==3.18.1
```

