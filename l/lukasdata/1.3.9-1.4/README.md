# Comparing `tmp/lukasdata-1.3.9.tar.gz` & `tmp/lukasdata-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.3.9.tar", last modified: Sat May 25 08:31:35 2024, max compression
+gzip compressed data, was "lukasdata-1.4.tar", last modified: Sun May 26 10:52:28 2024, max compression
```

## Comparing `lukasdata-1.3.9.tar` & `lukasdata-1.4.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.595510 lukasdata-1.3.9/
--rw-rw-rw-   0        0        0      128 2024-05-25 08:31:35.593512 lukasdata-1.3.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.487049 lukasdata-1.3.9/cleaning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/cleaning/__init__.py
--rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.9/cleaning/check_for_all_zeroes.py
--rw-rw-rw-   0        0        0      208 2024-05-23 09:45:03.000000 lukasdata-1.3.9/cleaning/clean_multiple_space.py
--rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.9/cleaning/drop_column_with_na.py
--rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.9/cleaning/mean_impute.py
--rw-rw-rw-   0        0        0      317 2024-05-21 21:30:45.000000 lukasdata-1.3.9/cleaning/my_strip.py
--rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.9/cleaning/na_counts.py
--rw-rw-rw-   0        0        0      130 2024-05-23 09:36:16.000000 lukasdata-1.3.9/cleaning/order_dict_by_key.py
--rw-rw-rw-   0        0        0      325 2024-05-22 11:05:51.000000 lukasdata-1.3.9/cleaning/replace_umlaut.py
--rw-rw-rw-   0        0        0      151 2024-05-23 09:45:03.000000 lukasdata-1.3.9/cleaning/rstrip_list.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.524030 lukasdata-1.3.9/datahandling/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/datahandling/__init__.py
--rw-rw-rw-   0        0        0      935 2024-05-25 08:04:29.000000 lukasdata-1.3.9/datahandling/change_directory.py
--rw-rw-rw-   0        0        0      546 2024-05-21 20:40:00.000000 lukasdata-1.3.9/datahandling/change_encoding.py
--rw-rw-rw-   0        0        0      184 2023-09-18 11:41:48.000000 lukasdata-1.3.9/datahandling/check_for_mismatches_in_list.py
--rw-rw-rw-   0        0        0      704 2023-10-29 15:04:54.000000 lukasdata-1.3.9/datahandling/create_text_for_all_files_in_pdf_dir.py
--rw-rw-rw-   0        0        0      503 2023-10-28 19:49:49.000000 lukasdata-1.3.9/datahandling/deconstruct_file_name.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.9/datahandling/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.9/datahandling/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.9/datahandling/dict_to_json.py
--rw-rw-rw-   0        0        0      257 2024-05-14 19:58:00.000000 lukasdata-1.3.9/datahandling/json_to_dict.py
--rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.9/datahandling/order_dict.py
--rw-rw-rw-   0        0        0     1171 2023-10-29 14:47:29.000000 lukasdata-1.3.9/datahandling/pdf_to_txt.py
--rw-rw-rw-   0        0        0      193 2024-05-17 17:01:50.000000 lukasdata-1.3.9/datahandling/read_txt.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.9/datahandling/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.529032 lukasdata-1.3.9/errorhandling/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/errorhandling/__init__.py
--rw-rw-rw-   0        0        0      587 2024-05-17 15:57:45.000000 lukasdata-1.3.9/errorhandling/custom_errors.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.542128 lukasdata-1.3.9/exploration/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/exploration/__init__.py
--rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.9/exploration/analyze_datasets.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.9/exploration/count_nans.py
--rw-rw-rw-   0        0        0     3566 2024-05-14 10:55:38.000000 lukasdata-1.3.9/exploration/desciptive_statistics.py
--rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.9/exploration/get_list_intersection.py
--rw-rw-rw-   0        0        0        0 2024-05-14 10:08:25.000000 lukasdata-1.3.9/exploration/kernel_density_estimation.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.591514 lukasdata-1.3.9/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1505 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       78 2024-05-25 08:31:35.000000 lukasdata-1.3.9/lukasdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.577521 lukasdata-1.3.9/machine_learning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.9/machine_learning/drop_columns_permutation_score.py
--rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.9/machine_learning/keras_input.py
--rw-rw-rw-   0        0        0     3768 2024-04-30 19:39:47.000000 lukasdata-1.3.9/machine_learning/missing_forest.py
--rw-rw-rw-   0        0        0     1746 2024-05-14 10:55:46.000000 lukasdata-1.3.9/machine_learning/ml_model.py
--rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.9/machine_learning/permutation_importance.py
-drwxrwxrwx   0        0        0        0 2024-05-25 08:31:35.588514 lukasdata-1.3.9/manipulation/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.9/manipulation/__init__.py
--rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.9/manipulation/concat_dfs.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.9/manipulation/create_mask.py
--rw-rw-rw-   0        0        0      466 2024-05-13 11:10:36.000000 lukasdata-1.3.9/manipulation/int_columns.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.9/manipulation/list_to_string.py
--rw-rw-rw-   0        0        0       42 2024-05-25 08:31:35.595510 lukasdata-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-05-25 08:31:28.000000 lukasdata-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:52:28.963469 lukasdata-1.4/
+-rw-rw-rw-   0        0        0      126 2024-05-26 10:52:28.961470 lukasdata-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 10:52:28.815560 lukasdata-1.4/cleaning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.4/cleaning/__init__.py
+-rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.4/cleaning/check_for_all_zeroes.py
+-rw-rw-rw-   0        0        0      208 2024-05-23 09:45:03.000000 lukasdata-1.4/cleaning/clean_multiple_space.py
+-rw-rw-rw-   0        0        0      467 2024-05-26 10:00:36.000000 lukasdata-1.4/cleaning/drop_column_with_na.py
+-rw-rw-rw-   0        0        0      317 2024-05-21 21:30:45.000000 lukasdata-1.4/cleaning/my_strip.py
+-rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.4/cleaning/na_counts.py
+-rw-rw-rw-   0        0        0      130 2024-05-23 09:36:16.000000 lukasdata-1.4/cleaning/order_dict_by_key.py
+-rw-rw-rw-   0        0        0      325 2024-05-22 11:05:51.000000 lukasdata-1.4/cleaning/replace_umlaut.py
+-rw-rw-rw-   0        0        0      151 2024-05-23 09:45:03.000000 lukasdata-1.4/cleaning/rstrip_list.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:52:28.873525 lukasdata-1.4/datahandling/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.4/datahandling/__init__.py
+-rw-rw-rw-   0        0        0      953 2024-05-25 14:35:09.000000 lukasdata-1.4/datahandling/change_directory.py
+-rw-rw-rw-   0        0        0      546 2024-05-21 20:40:00.000000 lukasdata-1.4/datahandling/change_encoding.py
+-rw-rw-rw-   0        0        0      184 2023-09-18 11:41:48.000000 lukasdata-1.4/datahandling/check_for_mismatches_in_list.py
+-rw-rw-rw-   0        0        0      704 2023-10-29 15:04:54.000000 lukasdata-1.4/datahandling/create_text_for_all_files_in_pdf_dir.py
+-rw-rw-rw-   0        0        0      503 2023-10-28 19:49:49.000000 lukasdata-1.4/datahandling/deconstruct_file_name.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.4/datahandling/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.4/datahandling/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.4/datahandling/dict_to_json.py
+-rw-rw-rw-   0        0        0      192 2024-05-26 10:20:31.000000 lukasdata-1.4/datahandling/import_data.py
+-rw-rw-rw-   0        0        0      257 2024-05-14 19:58:00.000000 lukasdata-1.4/datahandling/json_to_dict.py
+-rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.4/datahandling/order_dict.py
+-rw-rw-rw-   0        0        0     1171 2023-10-29 14:47:29.000000 lukasdata-1.4/datahandling/pdf_to_txt.py
+-rw-rw-rw-   0        0        0      193 2024-05-17 17:01:50.000000 lukasdata-1.4/datahandling/read_txt.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.4/datahandling/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:52:28.877523 lukasdata-1.4/errorhandling/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.4/errorhandling/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-05-17 15:57:45.000000 lukasdata-1.4/errorhandling/custom_errors.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:52:28.892513 lukasdata-1.4/exploration/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.4/exploration/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.4/exploration/analyze_datasets.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.4/exploration/count_nans.py
+-rw-rw-rw-   0        0        0     3566 2024-05-14 10:55:38.000000 lukasdata-1.4/exploration/desciptive_statistics.py
+-rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.4/exploration/get_list_intersection.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 10:08:25.000000 lukasdata-1.4/exploration/kernel_density_estimation.py
+-rw-rw-rw-   0        0        0      366 2024-05-25 14:55:28.000000 lukasdata-1.4/exploration/nan_heatmap.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:52:28.960470 lukasdata-1.4/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      126 2024-05-26 10:52:28.000000 lukasdata-1.4/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2024-05-26 10:52:28.000000 lukasdata-1.4/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:52:28.000000 lukasdata-1.4/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-26 10:52:28.000000 lukasdata-1.4/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       78 2024-05-26 10:52:28.000000 lukasdata-1.4/lukasdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 10:52:28.947479 lukasdata-1.4/machine_learning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.4/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.4/machine_learning/drop_columns_permutation_score.py
+-rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.4/machine_learning/keras_input.py
+-rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.4/machine_learning/mean_impute.py
+-rw-rw-rw-   0        0        0     3761 2024-05-26 10:33:27.000000 lukasdata-1.4/machine_learning/missing_forest.py
+-rw-rw-rw-   0        0        0     1746 2024-05-14 10:55:46.000000 lukasdata-1.4/machine_learning/ml_model.py
+-rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.4/machine_learning/permutation_importance.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:52:28.957472 lukasdata-1.4/manipulation/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.4/manipulation/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.4/manipulation/concat_dfs.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.4/manipulation/create_mask.py
+-rw-rw-rw-   0        0        0      466 2024-05-13 11:10:36.000000 lukasdata-1.4/manipulation/filter_numeric_columns.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.4/manipulation/list_to_string.py
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:52:28.964468 lukasdata-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      190 2024-05-26 10:52:22.000000 lukasdata-1.4/setup.py
```

### Comparing `lukasdata-1.3.9/datahandling/change_encoding.py` & `lukasdata-1.4/datahandling/change_encoding.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.9/datahandling/create_text_for_all_files_in_pdf_dir.py` & `lukasdata-1.4/datahandling/create_text_for_all_files_in_pdf_dir.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.9/datahandling/pdf_to_txt.py` & `lukasdata-1.4/datahandling/pdf_to_txt.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.9/errorhandling/custom_errors.py` & `lukasdata-1.4/errorhandling/custom_errors.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.9/exploration/desciptive_statistics.py` & `lukasdata-1.4/exploration/desciptive_statistics.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.9/lukasdata.egg-info/SOURCES.txt` & `lukasdata-1.4/lukasdata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 setup.py
 cleaning/__init__.py
 cleaning/check_for_all_zeroes.py
 cleaning/clean_multiple_space.py
 cleaning/drop_column_with_na.py
-cleaning/mean_impute.py
 cleaning/my_strip.py
 cleaning/na_counts.py
 cleaning/order_dict_by_key.py
 cleaning/replace_umlaut.py
 cleaning/rstrip_list.py
 datahandling/__init__.py
 datahandling/change_directory.py
 datahandling/change_encoding.py
 datahandling/check_for_mismatches_in_list.py
 datahandling/create_text_for_all_files_in_pdf_dir.py
 datahandling/deconstruct_file_name.py
 datahandling/del_jpg.py
 datahandling/determine_file_type.py
 datahandling/dict_to_json.py
+datahandling/import_data.py
 datahandling/json_to_dict.py
 datahandling/order_dict.py
 datahandling/pdf_to_txt.py
 datahandling/read_txt.py
 datahandling/string_to_text.py
 errorhandling/__init__.py
 errorhandling/custom_errors.py
 exploration/__init__.py
 exploration/analyze_datasets.py
 exploration/count_nans.py
 exploration/desciptive_statistics.py
 exploration/get_list_intersection.py
 exploration/kernel_density_estimation.py
+exploration/nan_heatmap.py
 lukasdata.egg-info/PKG-INFO
 lukasdata.egg-info/SOURCES.txt
 lukasdata.egg-info/dependency_links.txt
 lukasdata.egg-info/requires.txt
 lukasdata.egg-info/top_level.txt
 machine_learning/__init__.py
 machine_learning/drop_columns_permutation_score.py
 machine_learning/keras_input.py
+machine_learning/mean_impute.py
 machine_learning/missing_forest.py
 machine_learning/ml_model.py
 machine_learning/permutation_importance.py
 manipulation/__init__.py
 manipulation/concat_dfs.py
 manipulation/create_mask.py
-manipulation/int_columns.py
+manipulation/filter_numeric_columns.py
 manipulation/list_to_string.py
```

### Comparing `lukasdata-1.3.9/machine_learning/keras_input.py` & `lukasdata-1.4/machine_learning/keras_input.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.9/machine_learning/missing_forest.py` & `lukasdata-1.4/machine_learning/missing_forest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import pandas as pd
-from lukasdata.change_directory import chdir_data
+from datahandling.change_directory import chdir_data
 chdir_data()
 
-from lukasdata.count_nans import count_nan
-from lukasdata.drop_column_with_na import drop_column_with_na
-from lukasdata.mean_impute import mean_impute
-from lukasdata.get_number_columns import filter_numeric_columns
+from exploration.count_nans import count_nan
+from cleaning.drop_column_with_na import drop_column_with_na
+import mean_impute
+from manipulation.filter_numeric_columns import filter_numeric_columns
 from sklearn.metrics import mean_squared_error
 
 def reorder_columns_by_na(df):
     missing_values_dict=count_nan(df)
     sorted_by_value=dict(sorted(missing_values_dict.items(),key=lambda x: x[1]))
     sorted_list_of_column_names=[]
     for number,entry in enumerate(sorted_by_value):
         sorted_list_of_column_names.append(entry)
     new_df=df[sorted_list_of_column_names]
     return new_df
 
 
-complete_financial=pd.read_csv("complete_financial.csv")
+#complete_financial=pd.read_csv("complete_financial.csv")
 
 
-complete_financial_numerical=filter_numeric_columns(complete_financial)
+#complete_financial_numerical=filter_numeric_columns(complete_financial)
 
 import numpy as np
 from sklearn.ensemble import RandomForestRegressor
 
 class MissForestImputer:
     def __init__(self, max_iter=10, n_estimators=100):
         self.max_iter = max_iter
@@ -65,15 +65,16 @@
                 #muss ich hier column feature_idxs rausnehmen?
                 #print(f"predicted values ist {len(predicted_values)} lang")
                 #print(f"missing_mask  ist {len(missing_mask)} lang")
                 self.X.iloc[missing_mask, feature_idx] = predicted_values[missing_mask]
         print(self.X)
         mse_df=pd.DataFrame(mse_list)
         return self.X
+
     
 
 
-imputer = MissForestImputer()
-X_imputed = imputer.fit_transform(complete_financial_numerical)
-X_imputed.insert(loc=1,value=complete_financial["idnr"],column="idnr")
-X_imputed.set_index("idnr")
-X_imputed.to_csv("rf_imputed.csv")
+#imputer = MissForestImputer()
+#X_imputed = imputer.fit_transform(complete_financial_numerical)
+#X_imputed.insert(loc=1,value=complete_financial["idnr"],column="idnr")
+#X_imputed.set_index("idnr")
+#X_imputed.to_csv("rf_imputed.csv")
```

### Comparing `lukasdata-1.3.9/machine_learning/ml_model.py` & `lukasdata-1.4/machine_learning/ml_model.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.9/machine_learning/permutation_importance.py` & `lukasdata-1.4/machine_learning/permutation_importance.py`

 * *Files identical despite different names*

