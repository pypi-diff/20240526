# Comparing `tmp/dscontexai-0.0.8.tar.gz` & `tmp/dscontexai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-0.0.8.tar", last modified: Sun May 26 15:05:54 2024, max compression
+gzip compressed data, was "dscontexai-0.1.0.tar", last modified: Sun May 26 13:57:54 2024, max compression
```

## Comparing `dscontexai-0.0.8.tar` & `dscontexai-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 15:05:54.348342 dscontexai-0.0.8/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 15:05:54.348342 dscontexai-0.0.8/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 15:05:54.348342 dscontexai-0.0.8/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       85 2024-05-26 14:00:13.000000 dscontexai-0.0.8/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10558 2024-05-26 15:03:11.000000 dscontexai-0.0.8/dscontexai/dsc_grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3569 2024-05-26 15:04:21.000000 dscontexai-0.0.8/dscontexai/dsc_ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:44:26.000000 dscontexai-0.0.8/dscontexai/dsc_xgboost.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     6117 2024-05-26 14:40:34.000000 dscontexai-0.0.8/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-0.0.8/dscontexai/grammar_with_box_latex.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 15:05:54.348342 dscontexai-0.0.8/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 15:05:54.000000 dscontexai-0.0.8/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      345 2024-05-26 15:05:54.000000 dscontexai-0.0.8/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 15:05:54.000000 dscontexai-0.0.8/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1059 2024-05-26 15:05:54.000000 dscontexai-0.0.8/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 15:05:54.000000 dscontexai-0.0.8/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 15:05:54.348342 dscontexai-0.0.8/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     2441 2024-05-26 15:05:41.000000 dscontexai-0.0.8/setup.py
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

### Comparing `dscontexai-0.0.8/dscontexai/dsc_grammar.py` & `dscontexai-0.1.0/dscontexai/dsc_grammar.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,16 +290,13 @@
 
     with doc.create(Itemize(options=["noitemsep"])) as itemize:
         for i in range(3):
             feature = sorted_feature_names[i]
             value = results[feature_names.index(feature)]
             itemize.add_item(NoEscape(f"\\textbf{{{feature}}}: {value}"))
 
-    if not os.path.exists("./prototypes"):
-        os.makedirs("./prototypes")
-
     doc.generate_pdf(
         os.path.join(f"./prototypes/output_{index}"),
         compiler="pdflatex",
         clean=True,
         clean_tex=True,
     )
```

### Comparing `dscontexai-0.0.8/dscontexai/dsc_ploting.py` & `dscontexai-0.1.0/dscontexai/dsc_ploting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 
 # Set visualization styles
 sns.set_theme(style="white", font_scale=2.5)
 sns.set_palette("deep")
@@ -109,12 +107,8 @@
     for spine in ["top", "right", "bottom", "left"]:
         ax.spines[spine].set_color("0.5")
         ax.spines[spine].set_visible(True)
     for spine in ["left", "bottom"]:
         ax.spines[spine].set_linewidth(1.2)
 
     fig.tight_layout()
-
-    if os.path.exists(fig_path):
-        os.remove(fig_path)
-
     fig.savefig(fig_path, format="pdf")
```

### Comparing `dscontexai-0.0.8/dscontexai/dsc_xgboost.py` & `dscontexai-0.1.0/dscontexai/dsc_xgboost.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from sklearn.metrics import f1_score
 from sklearn.model_selection import train_test_split
 
 
 def load_data(path: str) -> pd.DataFrame:
     return pd.read_csv(path)
 
-
 def preprocess_data(df: pd.DataFrame) -> tuple:
-    df["gender"] = df["gender"].astype("category").cat.codes
-    df = df[df["smoking_history"] != "No Info"]
-    smoker_status = ["current", "ever", "former"]
-    df["smoking_history"] = df["smoking_history"].apply(lambda x: 1 if x in smoker_status else 0)
-
-    X = df.drop(columns=["diabetes"])
-    y = df["diabetes"]
-
+    df['gender'] = df['gender'].astype('category').cat.codes
+    df = df[df['smoking_history'] != 'No Info']
+    smoker_status = ['current', 'ever', 'former']
+    df['smoking_history'] = df['smoking_history'].apply(lambda x: 1 if x in smoker_status else 0)
+
+    X = df.drop(columns=['diabetes'])
+    y = df['diabetes'] 
+    
     return X, y
 
-
 def train_model(X: pd.DataFrame, y: pd.Series) -> XGBClassifier:
     model = XGBClassifier()
     model.fit(X, y)
 
     pickle.dump(model, open("./models/model.pkl", "wb"))
     return model
 
 
 def predict(model: XGBClassifier, X: pd.DataFrame) -> np.ndarray:
     return model.predict(X)
 
-
 if __name__ == "__main__":
     _is_trained = False
     data = load_data("kaggle_data/diabetes_prediction_dataset_balanced.csv")
 
     X, y = preprocess_data(data)
 
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
 
     if not _is_trained:
         clf = train_model(X_train, y_train)
     else:
         clf = pickle.load(open("./models/diabetes_model.pkl", "rb"))
 
-    y_pred = predict(clf, X_test)
+    y_pred = predict(clf, X_test)
```

### Comparing `dscontexai-0.0.8/dscontexai/grammar_with_box_latex.py` & `dscontexai-0.1.0/dscontexai/grammar_with_box_latex.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     NoEscape,
     Package,
     Section,
     Subsection,
 )
 from pylatex.utils import bold
 
+import dscontexai.dsc_xgboost as xgb
 from dscontexai.dsc_ploting import plot_shap
 
 plt.rcParams["text.usetex"] = True
 
 
 def fixing_variable_names(variables: list) -> list:
     """
```

### Comparing `dscontexai-0.0.8/dscontexai.egg-info/requires.txt` & `dscontexai-0.1.0/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.8/setup.py` & `dscontexai-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.8"
+VERSION = "0.1.0"
 DESCRIPTION = "ConteXAI"
 LONG_DESCRIPTION = "xAI for everyone!"
 
 # Setting up
 setup(
     name="dscontexai",
     version=VERSION,
     author="Jovana V., Haris K., Luka M.",
     author_email="<youremail@email.com>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    package_data={"latex_styles": ["./.json"]},
     install_requires=[
         "asttokens==2.4.1",
         "backcall==0.2.0",
         "catboost==1.2.5",
         "cloudpickle==3.0.0",
         "comm==0.2.2",
         "contourpy==1.1.1",
```

