# Comparing `tmp/dscontexai-0.0.5.tar.gz` & `tmp/dscontexai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-0.0.5.tar", last modified: Sun May 26 14:27:45 2024, max compression
+gzip compressed data, was "dscontexai-0.1.0.tar", last modified: Sun May 26 13:57:54 2024, max compression
```

## Comparing `dscontexai-0.0.5.tar` & `dscontexai-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 14:27:45.935604 dscontexai-0.0.5/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 14:27:45.931604 dscontexai-0.0.5/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 14:27:45.927604 dscontexai-0.0.5/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       85 2024-05-26 14:00:13.000000 dscontexai-0.0.5/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10478 2024-05-26 13:57:24.000000 dscontexai-0.0.5/dscontexai/dsc_grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3495 2024-05-26 09:49:20.000000 dscontexai-0.0.5/dscontexai/dsc_ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1404 2024-05-26 14:25:29.000000 dscontexai-0.0.5/dscontexai/dsc_xgboost.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     6215 2024-05-26 14:21:42.000000 dscontexai-0.0.5/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10169 2024-05-26 13:59:57.000000 dscontexai-0.0.5/dscontexai/grammar_with_box_latex.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 14:27:45.931604 dscontexai-0.0.5/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 14:27:45.000000 dscontexai-0.0.5/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      345 2024-05-26 14:27:45.000000 dscontexai-0.0.5/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 14:27:45.000000 dscontexai-0.0.5/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1059 2024-05-26 14:27:45.000000 dscontexai-0.0.5/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 14:27:45.000000 dscontexai-0.0.5/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 14:27:45.935604 dscontexai-0.0.5/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     2393 2024-05-26 14:27:27.000000 dscontexai-0.0.5/setup.py
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

### Comparing `dscontexai-0.0.5/dscontexai/dsc_grammar.py` & `dscontexai-0.1.0/dscontexai/dsc_grammar.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.5/dscontexai/dsc_ploting.py` & `dscontexai-0.1.0/dscontexai/dsc_ploting.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.5/dscontexai/dsc_xgboost.py` & `dscontexai-0.1.0/dscontexai/dsc_xgboost.py`

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

### Comparing `dscontexai-0.0.5/dscontexai/grammar_with_box_latex.py` & `dscontexai-0.1.0/dscontexai/grammar_with_box_latex.py`

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

### Comparing `dscontexai-0.0.5/dscontexai.egg-info/requires.txt` & `dscontexai-0.1.0/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.5/setup.py` & `dscontexai-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.5"
+VERSION = "0.1.0"
 DESCRIPTION = "ConteXAI"
 LONG_DESCRIPTION = "xAI for everyone!"
 
 # Setting up
 setup(
     name="dscontexai",
     version=VERSION,
```

