# Comparing `tmp/naturalexperiments-0.1.3.tar.gz` & `tmp/naturalexperiments-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.1.3.tar", last modified: Fri May 24 21:00:23 2024, max compression
+gzip compressed data, was "naturalexperiments-0.1.4.tar", last modified: Sun May 26 10:55:59 2024, max compression
```

## Comparing `naturalexperiments-0.1.3.tar` & `naturalexperiments-0.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.335017 naturalexperiments-0.1.3/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.1.3/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 21:00:23.334781 naturalexperiments-0.1.3/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.1.3/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.328308 naturalexperiments-0.1.3/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-24 16:16:52.000000 naturalexperiments-0.1.3/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    12686 2024-05-24 20:59:08.000000 naturalexperiments-0.1.3/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.329030 naturalexperiments-0.1.3/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      391 2024-05-24 13:38:10.000000 naturalexperiments-0.1.3/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.329358 naturalexperiments-0.1.3/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.1.3/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.329592 naturalexperiments-0.1.3/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.1.3/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.329805 naturalexperiments-0.1.3/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.1.3/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.330094 naturalexperiments-0.1.3/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.1.3/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.330603 naturalexperiments-0.1.3/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     2253 2024-05-24 13:38:42.000000 naturalexperiments-0.1.3/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.1.3/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.330874 naturalexperiments-0.1.3/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.1.3/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     6151 2024-05-24 13:47:10.000000 naturalexperiments-0.1.3/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.334258 naturalexperiments-0.1.3/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-23 17:30:11.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      690 2024-05-24 20:42:56.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.1.3/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3546 2024-05-24 13:44:37.000000 naturalexperiments-0.1.3/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     2185 2024-05-24 13:19:39.000000 naturalexperiments-0.1.3/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 21:00:23.334494 naturalexperiments-0.1.3/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 21:00:23.000000 naturalexperiments-0.1.3/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-24 21:00:23.000000 naturalexperiments-0.1.3/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-24 21:00:23.000000 naturalexperiments-0.1.3/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-24 21:00:23.000000 naturalexperiments-0.1.3/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-24 21:00:23.335077 naturalexperiments-0.1.3/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-24 20:59:47.000000 naturalexperiments-0.1.3/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.358684 naturalexperiments-0.1.4/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.1.4/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-26 10:55:59.358456 naturalexperiments-0.1.4/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.1.4/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.348035 naturalexperiments-0.1.4/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-24 16:16:52.000000 naturalexperiments-0.1.4/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    12686 2024-05-24 20:59:08.000000 naturalexperiments-0.1.4/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.348757 naturalexperiments-0.1.4/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      444 2024-05-25 15:10:16.000000 naturalexperiments-0.1.4/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.349009 naturalexperiments-0.1.4/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2267 2024-05-26 10:54:09.000000 naturalexperiments-0.1.4/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.349319 naturalexperiments-0.1.4/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1420 2024-05-25 15:07:51.000000 naturalexperiments-0.1.4/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.349566 naturalexperiments-0.1.4/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1283 2024-05-25 15:30:03.000000 naturalexperiments-0.1.4/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.349920 naturalexperiments-0.1.4/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-25 15:30:29.000000 naturalexperiments-0.1.4/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.350629 naturalexperiments-0.1.4/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2253 2024-05-25 15:30:41.000000 naturalexperiments-0.1.4/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.1.4/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.350955 naturalexperiments-0.1.4/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1731 2024-05-25 15:08:21.000000 naturalexperiments-0.1.4/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     6151 2024-05-24 13:47:10.000000 naturalexperiments-0.1.4/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.354144 naturalexperiments-0.1.4/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-26 10:26:15.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      690 2024-05-24 20:42:56.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.1.4/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3546 2024-05-24 13:44:37.000000 naturalexperiments-0.1.4/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2185 2024-05-24 13:19:39.000000 naturalexperiments-0.1.4/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-26 10:55:59.354306 naturalexperiments-0.1.4/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-26 10:55:59.000000 naturalexperiments-0.1.4/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-26 10:55:59.000000 naturalexperiments-0.1.4/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-26 10:55:59.000000 naturalexperiments-0.1.4/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-26 10:55:59.000000 naturalexperiments-0.1.4/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-26 10:55:59.358719 naturalexperiments-0.1.4/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-26 10:55:27.000000 naturalexperiments-0.1.4/setup.py
```

### Comparing `naturalexperiments-0.1.3/LICENSE` & `naturalexperiments-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/PKG-INFO` & `naturalexperiments-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.1.3
+Version: 0.1.4
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.1.3/naturalexperiments/benchmark.py` & `naturalexperiments-0.1.4/naturalexperiments/benchmark.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.1.4/naturalexperiments/data/acic/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import pandas as pd
 import os
 import pickle as pkl
 import numpy as np
 import requests
 
-def load_acic():
+def load_acic(year):
     # Print absolute path
     # Get absolute path to this file
-    filename = __file__.replace('__init__.py', 'acic_data.csv')
+    assert year in ['16', '17'], "Year must be '16' or '17'"
+    filename = __file__.replace('__init__.py', f'acic{year}_data.csv')
 
     if not os.path.exists(filename):
         print('Downloading ACIC data...')
         # Download the data 
-        url = 'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/acic/acic_data.csv'
+        url = f'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/acic/acic{year}_data.csv'
 
         r = requests.get(url)
         open(filename, 'wb').write(r.content)
     
     data = pd.read_csv(filename)
 
     # Remove string columns
     data = data.select_dtypes(include = ['int16', 'int32', 'int64', 'float16', 'float32', 'float64'])
     data = data.astype(np.float32)
 
     # Set data type of columns to float32
-    
-    
+
     # No data description available
     # Assuming the first binary column is the treatment indicator
     binary_cols = []
     for col in data.columns:
         if data[col].nunique() == 2:
             binary_cols += [col]
     binary_col = binary_cols[0]
@@ -45,21 +45,29 @@
 
     
 
     X = np.array(data.drop(columns=[binary_col, target_col]).values, dtype=np.float32)
 
     return X, y, z
 
+def load_acic16():
+    return load_acic('16')
+
+def load_acic17():
+    return load_acic('17')
+
 if __name__ == '__main__':
-    if os.path.exists('input_2016.RData'):
-        import rdata
-        parsed = rdata.parser.parse_file('input_2016.RData')
-
-        converted = rdata.conversion.convert(parsed)
-
-        data = pd.DataFrame(converted['input_2016'])
-
-        pkl.dump(data, open('acic_data.pkl', 'wb'))
-    else:
-        print('Please download the ACIC data from https://github.com/vdorie/aciccomp/blob/master/2016/data/input_2016.RData')
-        print('Place the input_2016.RData file in the data folder')
-        print('Then run this script again')
+    for year in ['16', '17']:
+        if os.path.exists(f'input_20{year}.RData'):
+            import rdata
+            parsed = rdata.parser.parse_file(f'input_20{year}.RData')
+
+            converted = rdata.conversion.convert(parsed)
+
+            data = pd.DataFrame(converted[f'input_20{year}'])
+
+            data.to_csv(f'acic{year}_data.csv', index=False)
+        else: 
+            print(f'Please download the ACIC{year} data from https://github.com/vdorie/aciccomp/blob/master/20{year}/data/input_20{year}.RData')
+            print(f'Place the input_20{year}.RData file in the data folder')
+            print('Then run this script again')
+
```

### Comparing `naturalexperiments-0.1.3/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.1.4/naturalexperiments/data/ihdp/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,20 +24,17 @@
     }, dtype=float)
 
     X = data.drop(['treatment', 'y_factual', 'y_cfactual', 'mu0', 'mu1'], axis=1).values
     
     return X, y, z
 
 if __name__ == '__main__':
-    if not os.path.exists('ihdp_data.pkl'):
-        datasets = []
-        url_prefix = "https://raw.githubusercontent.com/AMLab-Amsterdam/CEVAE/9081f863e24ce21bd34c8d6a41bf0edc7d1b65dd/datasets/IHDP/csv/ihdp_npci_"
-        url_suffix = ".csv" 
-        colnames = ['treatment', 'y_factual', 'y_cfactual', 'mu0', 'mu1']
-        for i in range(1,26):
-            colnames += ['x' + str(i)]
+    url_prefix = "https://raw.githubusercontent.com/AMLab-Amsterdam/CEVAE/9081f863e24ce21bd34c8d6a41bf0edc7d1b65dd/datasets/IHDP/csv/ihdp_npci_"
+    url_suffix = ".csv" 
+    colnames = ['treatment', 'y_factual', 'y_cfactual', 'mu0', 'mu1']
+    for i in range(1,26):
+        colnames += ['x' + str(i)]
 
-        for i in range(1,11):
-            url = url_prefix + str(i) + url_suffix
-            data = pd.read_csv(url, header=None, names=colnames)
-            datasets.append(data)
-        pkl.dump(datasets, open('ihdp_data.pkl', 'wb'))
+    for i in range(1,11):
+        url = url_prefix + str(i) + url_suffix
+        data = pd.read_csv(url, header=None, names=colnames)
+        data.to_csv(f'ihdp_data_{i}.csv', index=False)
```

### Comparing `naturalexperiments-0.1.3/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.1.4/naturalexperiments/data/jobs/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,19 +23,19 @@
     }, dtype=float)
 
     X = data.drop(columns=['treat', 're78']).values
 
     return X, y, z
 
 if __name__ == '__main__':
-    if not os.path.exists('jobs_data.pkl'):
-        url_treatment = "https://users.nber.org/~rdehejia/data/nsw_treated.txt"
-        url_control = "https://users.nber.org/~rdehejia/data/nsw_control.txt"
 
-        col_names = ["treat", "age", "educ", "black", "hisp", "married", "nodegr", "re75", "re78"]
+    url_treatment = "https://users.nber.org/~rdehejia/data/nsw_treated.txt"
+    url_control = "https://users.nber.org/~rdehejia/data/nsw_control.txt"
 
-        treatment = pd.read_csv(url_treatment, names=col_names, sep="  ", engine='python')
-        control = pd.read_csv(url_control, names=col_names, sep="  ", engine='python')
+    col_names = ["treat", "age", "educ", "black", "hisp", "married", "nodegr", "re75", "re78"]
 
-        data = pd.concat([treatment, control], ignore_index=True)
+    treatment = pd.read_csv(url_treatment, names=col_names, sep="  ", engine='python')
+    control = pd.read_csv(url_control, names=col_names, sep="  ", engine='python')
 
-        pkl.dump(data, open('jobs_data.pkl', 'wb'))
+    data = pd.concat([treatment, control], ignore_index=True)
+
+    data.to_csv('jobs_data.csv', index=False)
```

### Comparing `naturalexperiments-0.1.3/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.1.4/naturalexperiments/data/news/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/data/rorco/__init__.py` & `naturalexperiments-0.1.4/naturalexperiments/data/rorco/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.1.4/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.1.4/naturalexperiments/data/twins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,21 +31,20 @@
     cols_to_drop = [x for x in data.columns if '_0' in x or '_1' in x]
 
     X = data.drop(columns=cols_to_drop).values
 
     return X, y, z 
 
 if __name__ == '__main__':
-    if not os.path.exists('twins_data.pkl'):
-        url_weight = "https://raw.githubusercontent.com/AMLab-Amsterdam/CEVAE/9081f863e24ce21bd34c8d6a41bf0edc7d1b65dd/datasets/TWINS/twin_pairs_T_3years_samesex.csv"
+    url_weight = "https://raw.githubusercontent.com/AMLab-Amsterdam/CEVAE/9081f863e24ce21bd34c8d6a41bf0edc7d1b65dd/datasets/TWINS/twin_pairs_T_3years_samesex.csv"
 
-        url_X = "https://raw.githubusercontent.com/AMLab-Amsterdam/CEVAE/9081f863e24ce21bd34c8d6a41bf0edc7d1b65dd/datasets/TWINS/twin_pairs_X_3years_samesex.csv"
+    url_X = "https://raw.githubusercontent.com/AMLab-Amsterdam/CEVAE/9081f863e24ce21bd34c8d6a41bf0edc7d1b65dd/datasets/TWINS/twin_pairs_X_3years_samesex.csv"
 
-        url_y = "https://raw.githubusercontent.com/AMLab-Amsterdam/CEVAE/9081f863e24ce21bd34c8d6a41bf0edc7d1b65dd/datasets/TWINS/twin_pairs_Y_3years_samesex.csv"
+    url_y = "https://raw.githubusercontent.com/AMLab-Amsterdam/CEVAE/9081f863e24ce21bd34c8d6a41bf0edc7d1b65dd/datasets/TWINS/twin_pairs_Y_3years_samesex.csv"
 
-        weight = pd.read_csv(url_weight) # Birth weight 
-        X = pd.read_csv(url_X) # Covariates
-        y = pd.read_csv(url_y) # Mortality (binary)
+    weight = pd.read_csv(url_weight) # Birth weight 
+    X = pd.read_csv(url_X) # Covariates
+    y = pd.read_csv(url_y) # Mortality (binary)
 
-        data = pd.concat([weight, X, y], axis=1).drop(columns=['Unnamed: 0', 'Unnamed: 0.1'])
+    data = pd.concat([weight, X, y], axis=1).drop(columns=['Unnamed: 0', 'Unnamed: 0.1'])
 
-        pkl.dump(data, open('twins_data.pkl', 'wb'))
+    data.to_csv('twins_data.csv', index=False)
```

### Comparing `naturalexperiments-0.1.3/naturalexperiments/data_summary.py` & `naturalexperiments-0.1.4/naturalexperiments/data_summary.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.1.4/naturalexperiments/estimators/__init__.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     'Regression Discontinuity' : compute_regression_discontinuity, 
     'Propensity Stratification' : compute_propensity_stratification,
     'Direct Difference' : compute_direct_difference, 
     'Adjusted Direct' : compute_learned_direct,
     'Horvitz-Thompson' : compute_horvitz_thompson,
     'Doubly Robust' : compute_doubly_robust,
     'TMLE' : compute_TMLE,
+    'Off-policy' : compute_off_policy,
+    'Double-Double' : compute_double_double,
     'Direct Prediction' : compute_direct_prediction,
     'SNet' : wrap_catenet('SNet'),
     'FlexTENet' : wrap_catenet('FlexTENet'),
     'OffsetNet' : wrap_catenet('OffsetNet'),
     'TNet' : wrap_catenet('TNet'),
     'TARNet' : wrap_catenet('TARNet'),
     'DragonNet' : wrap_catenet('DragonNet'),
     'SNet3' : wrap_catenet('SNet3'),
     'DRNet' : wrap_catenet('DRNet'),
     'RANet' : wrap_catenet('RANet'),
     'PWNet' : wrap_catenet('PWNet'),
     'RNet' : wrap_catenet('RNet'),
     'XNet' : wrap_catenet('XNet'),
-    'Off-policy' : compute_off_policy,
-    'Double-Double' : compute_double_double,
 }
```

### Comparing `naturalexperiments-0.1.3/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.1.4/naturalexperiments/estimators/catenet.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.1.4/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.1.4/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.1.4/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.1.4/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/model.py` & `naturalexperiments-0.1.4/naturalexperiments/model.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments/utils.py` & `naturalexperiments-0.1.4/naturalexperiments/utils.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.1.4/naturalexperiments.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.1.3
+Version: 0.1.4
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.1.3/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.1.4/naturalexperiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.3/setup.py` & `naturalexperiments-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.1.3",
+    version="0.1.4",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

