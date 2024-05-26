# Comparing `tmp/Maslib-0.1.2.tar.gz` & `tmp/Maslib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Maslib-0.1.2.tar", last modified: Tue May 21 16:50:50 2024, max compression
+gzip compressed data, was "Maslib-0.1.3.tar", last modified: Sun May 26 09:54:31 2024, max compression
```

## Comparing `Maslib-0.1.2.tar` & `Maslib-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 16:50:50.017732 Maslib-0.1.2/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.1.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-21 16:50:49.996714 Maslib-0.1.2/MasLib/
--rw-rw-rw-   0        0        0      854 2024-05-21 16:49:15.000000 Maslib-0.1.2/MasLib/__init__.py
--rw-rw-rw-   0        0        0     3909 2024-05-21 16:48:27.000000 Maslib-0.1.2/MasLib/classification.py
--rw-rw-rw-   0        0        0     4174 2024-05-19 12:40:05.000000 Maslib-0.1.2/MasLib/clustering.py
--rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.1.2/MasLib/correlation.py
--rw-rw-rw-   0        0        0     3197 2024-05-21 16:49:28.000000 Maslib-0.1.2/MasLib/encoding.py
--rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.1.2/MasLib/grid_search_optimization.py
--rw-rw-rw-   0        0        0      465 2024-05-19 11:52:03.000000 Maslib-0.1.2/MasLib/loading.py
--rw-rw-rw-   0        0        0     5232 2024-05-19 11:16:36.000000 Maslib-0.1.2/MasLib/regressions.py
--rw-rw-rw-   0        0        0    11608 2024-05-21 16:48:29.000000 Maslib-0.1.2/MasLib/text_coding.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:50:50.014731 Maslib-0.1.2/Maslib.egg-info/
--rw-rw-rw-   0        0        0      848 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 16:50:49.000000 Maslib-0.1.2/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      848 2024-05-21 16:50:50.015732 Maslib-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-19 12:47:41.000000 Maslib-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 16:50:50.017732 Maslib-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-05-21 16:49:53.000000 Maslib-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:50:50.012728 Maslib-0.1.2/tests/
--rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 Maslib-0.1.2/tests/test_clustering.py
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.1.2/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.1.2/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.1.2/tests/test_grid_search.py
--rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 Maslib-0.1.2/tests/test_loading.py
--rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 Maslib-0.1.2/tests/test_regression.py
--rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 Maslib-0.1.2/tests/test_text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:54:31.047184 Maslib-0.1.3/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.1.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-26 09:54:31.025743 Maslib-0.1.3/MasLib/
+-rw-rw-rw-   0        0        0     1310 2024-05-26 07:57:21.000000 Maslib-0.1.3/MasLib/__init__.py
+-rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 Maslib-0.1.3/MasLib/classification.py
+-rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 Maslib-0.1.3/MasLib/clustering.py
+-rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 Maslib-0.1.3/MasLib/correlation.py
+-rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 Maslib-0.1.3/MasLib/encoding.py
+-rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 Maslib-0.1.3/MasLib/loading.py
+-rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 Maslib-0.1.3/MasLib/regressions.py
+-rw-rw-rw-   0        0        0    11632 2024-05-26 09:23:14.000000 Maslib-0.1.3/MasLib/text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:54:31.044590 Maslib-0.1.3/Maslib.egg-info/
+-rw-rw-rw-   0        0        0      888 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 09:54:30.000000 Maslib-0.1.3/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      888 2024-05-26 09:54:31.045628 Maslib-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-26 09:52:47.000000 Maslib-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 09:54:31.047184 Maslib-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      811 2024-05-26 09:51:27.000000 Maslib-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 09:54:31.042425 Maslib-0.1.3/tests/
+-rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 Maslib-0.1.3/tests/test_clustering.py
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.1.3/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.1.3/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.1.3/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 Maslib-0.1.3/tests/test_loading.py
+-rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 Maslib-0.1.3/tests/test_regression.py
+-rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 Maslib-0.1.3/tests/test_text_coding.py
```

### Comparing `Maslib-0.1.2/MasLib/encoding.py` & `Maslib-0.1.3/MasLib/encoding.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,85 @@
 from sklearn import preprocessing
 import pandas as pd
 import numpy as np
 import pandas as pd
 
 def number_encode_features(init_df: pd.DataFrame) -> (pd.DataFrame, dict):
     """
-    Функция для кодирования категориальных признаков в числовые.
+    Eng: Function for encoding categorical features into numerical ones.
+    Fra: Fonction pour encoder les caractéristiques catégorielles en numériques.
+    Rus: Функция для кодирования категориальных признаков в числовые.
+    Ger: Funktion zum Codieren kategorischer Merkmale in numerische.
 
     Parameters:
-    init_df (pd.DataFrame): Исходный DataFrame.
+    init_df (pd.Data Frame): The original DataFrame.
 
     Returns:
-    result (pd.DataFrame): DataFrame с закодированными признаками.
-    encoders (dict): Словарь с LabelEncoder для каждого категориального признака.
+    result (pd.Data Frame): A DataFrame with encoded attributes.
+    encoders (dict): A dictionary with a LabelEncoder for each categorical feature.
     """
-    result = init_df.copy()  # копируем нашу исходную таблицу
+    result = init_df.copy()
     encoders = {}
     for column in result.columns:
         if result.dtypes[column] == object:
             encoders[column] = preprocessing.LabelEncoder()
             result[column] = encoders[column].fit_transform(result[column])
     return result, encoders
 
-def process_column_and_merge(df_main, df_additional, column_name, merge_column):
+def process_column_and_merge(df_main, column_name):
     """
-    Process a specified column of a dataframe to extract values and merge with an additional dataframe.
-    
+    Eng: Function for processing the specified column of a DataFrame, extracting values, and merging with an additional DataFrame.
+    Fra: Fonction pour le traitement de la colonne spécifiée d'un DataFrame, l'extraction des valeurs et la fusion avec un DataFrame supplémentaire.
+    Rus: Функция для обработки указанного столбца DataFrame, извлечения значений и объединения с дополнительным DataFrame.
+    Ger: Funktion zur Verarbeitung der angegebenen Spalte eines DataFrame, Extrahierung von Werten und Zusammenführung mit einem zusätzlichen DataFrame.
+
     Parameters:
-    df_main (pd.DataFrame): The main dataframe.
-    df_additional (pd.DataFrame): The additional dataframe to be merged.
-    column_name (str): The name of the column to process.
-    merge_column (str): The column to which the processed data will be added in df_main.
-    
+    df_main (pd.DataFrame): The main DataFrame.
+    column_name (str): The name of the column to be processed.
+
     Returns:
-    pd.DataFrame: The main dataframe with the processed and merged column.
+    pd.Data Frame: The main DataFrame with the processed and merged column.
+
     """
     
     danger = []
     except_value = [np.nan, np.nan]
     
     for row in range(df_main.shape[0]):
         try:
             danger.append(list(df_main[column_name])[row].values())
         except:
             danger.append(except_value)
     
-    # Create a DataFrame from the extracted values
-    data_points = pd.DataFrame(columns=list(df_additional[column_name])[0].keys(), data=danger)
+    data_points = pd.DataFrame(columns=list(df_main[column_name])[0].keys(), data=danger)
     
-    # Merge the new DataFrame with the main DataFrame
     df_main = pd.concat([df_main, data_points], axis=1)
     
-    # Optionally, we could drop the original column if it's no longer needed
-    # df_main.drop(columns=[column_name], inplace=True)
-    
     return df_main
 
-# Example usage
-# df_main = pd.read_csv('path_to_main_dataframe.csv')
-# df_additional = pd.read_csv('path_to_additional_dataframe.csv')
-# updated_df = process_column_and_merge(df_main, df_additional, 'column_name_to_process', 'merge_column_name')
-# print(updated_df.head())
-
 def json_to_dataframe(json_path,name,name1,name3):
+    """
+    Eng: Function for converting data from JSON to DataFrame and creating a dictionary.
+    Fra: Fonction pour convertir les données de JSON en DataFrame et créer un dictionnaire.
+    Rus: Функция для преобразования данных из JSON в DataFrame и создания словаря.
+    Ger: Funktion zum Konvertieren von Daten aus JSON in DataFrame und Erstellen eines Wörterbuchs.
+
+    Parameters:
+    json_path (str): The path to the JSON file.
+    name (str): The name of the key for uploading data to the Data Frame.
+    name 1 (str): The name of the column with the company name.
+    name 3 (str): The name of the column with the nomination.
+
+    Returns:
+    df_json (pd.Data Frame): Data Frame with data from JSON.
+    dict1 (dict): A dictionary where the keys are companies and the values are nominations.
+    """
     with open(json_path, 'r', encoding='utf-8') as f:
         target = json.load(f)
     df_json = pd.DataFrame(target[name])
     dict1 = {}
     for company, nomination in zip(df_json[name2], df_json[name3]):
         dict1[company] = nomination
     return df_json, dict1
 
-# Пример использования:
-# df_main = pd.read_csv('path_to_main_dataframe.csv')
-# df_additional = pd.read_csv('path_to_additional_dataframe.csv')
-# df_main = process_column_and_merge(df_main, df_additional, 'point', 'merge_column')
-# df_json, dict1 = json_to_dataframe('path_to_json_file.json')
+
```

### Comparing `Maslib-0.1.2/setup.py` & `Maslib-0.1.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'phik',
         'matplotlib',
         'scikit-learn',
         'catboost',
         'joblib',
-        'wordcloud'
+        'wordcloud',
+        'xgboost',
+        'bertopic',
+
     ],
     author='Alecsandr_C.V.V',
     author_email='dxomko@gmail.com',
-    description='Это моя библиотека для оптимизации кода для python',
+    description='This is a library for optimizing code for python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Maslib-0.1.2/tests/test_clustering.py` & `Maslib-0.1.3/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.2/tests/test_correlation.py` & `Maslib-0.1.3/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.2/tests/test_encoding.py` & `Maslib-0.1.3/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.2/tests/test_grid_search.py` & `Maslib-0.1.3/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.2/tests/test_regression.py` & `Maslib-0.1.3/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.2/tests/test_text_coding.py` & `Maslib-0.1.3/tests/test_text_coding.py`

 * *Files identical despite different names*

