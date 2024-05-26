# Comparing `tmp/data_manipulation-0.8.tar.gz` & `tmp/data_manipulation-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/data_manipulation-0.8.tar", last modified: Mon Mar  2 15:33:11 2020, max compression
+gzip compressed data, was "dist/data_manipulation-0.9.tar", last modified: Sat Mar  7 04:22:42 2020, max compression
```

## Comparing `data_manipulation-0.8.tar` & `data_manipulation-0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.256878 data_manipulation-0.8/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       60 2020-02-29 08:00:46.000000 data_manipulation-0.8/MANIFEST.in
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      978 2020-03-02 15:33:11.256878 data_manipulation-0.8/PKG-INFO
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1143 2020-03-01 14:15:16.000000 data_manipulation-0.8/README.md
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.256878 data_manipulation-0.8/data_manipulation/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      186 2020-02-29 15:18:52.000000 data_manipulation-0.8/data_manipulation/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      495 2020-03-02 15:33:11.256878 data_manipulation-0.8/data_manipulation/_version.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.252878 data_manipulation-0.8/data_manipulation/data/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.8/data_manipulation/data/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1008 2020-02-23 11:11:02.000000 data_manipulation-0.8/data_manipulation/data/make_dataset.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.252878 data_manipulation-0.8/data_manipulation/data_types/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       22 2020-02-29 14:54:54.000000 data_manipulation-0.8/data_manipulation/data_types/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     4282 2020-03-02 02:32:36.000000 data_manipulation-0.8/data_manipulation/data_types/string_.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.252878 data_manipulation-0.8/data_manipulation/features/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.8/data_manipulation/features/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.8/data_manipulation/features/build_features.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.256878 data_manipulation-0.8/data_manipulation/geopandas/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       25 2020-02-29 14:54:54.000000 data_manipulation-0.8/data_manipulation/geopandas/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      957 2020-02-29 02:05:18.000000 data_manipulation-0.8/data_manipulation/geopandas/geopandas_.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.256878 data_manipulation-0.8/data_manipulation/models/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.8/data_manipulation/models/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.8/data_manipulation/models/predict_model.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.8/data_manipulation/models/train_model.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.256878 data_manipulation-0.8/data_manipulation/pandas/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       22 2020-02-29 14:54:54.000000 data_manipulation-0.8/data_manipulation/pandas/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)    15525 2020-02-29 01:46:36.000000 data_manipulation-0.8/data_manipulation/pandas/pandas_.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.256878 data_manipulation-0.8/data_manipulation/psycopg2/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       24 2020-02-29 14:54:54.000000 data_manipulation-0.8/data_manipulation/psycopg2/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1235 2020-02-29 02:32:41.000000 data_manipulation-0.8/data_manipulation/psycopg2/psycopg2_.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.256878 data_manipulation-0.8/data_manipulation/pyspark/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       23 2020-03-02 15:28:00.000000 data_manipulation-0.8/data_manipulation/pyspark/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     7589 2020-03-02 15:25:55.000000 data_manipulation-0.8/data_manipulation/pyspark/pyspark_.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.256878 data_manipulation-0.8/data_manipulation/visualization/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.8/data_manipulation/visualization/__init__.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.8/data_manipulation/visualization/visualize.py
-drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-02 15:33:11.252878 data_manipulation-0.8/data_manipulation.egg-info/
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      978 2020-03-02 15:33:11.000000 data_manipulation-0.8/data_manipulation.egg-info/PKG-INFO
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1075 2020-03-02 15:33:11.000000 data_manipulation-0.8/data_manipulation.egg-info/SOURCES.txt
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        1 2020-03-02 15:33:11.000000 data_manipulation-0.8/data_manipulation.egg-info/dependency_links.txt
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       30 2020-03-02 15:33:11.000000 data_manipulation-0.8/data_manipulation.egg-info/requires.txt
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       18 2020-03-02 15:33:11.000000 data_manipulation-0.8/data_manipulation.egg-info/top_level.txt
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      230 2020-03-02 15:33:11.256878 data_manipulation-0.8/setup.cfg
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1400 2020-03-01 14:15:16.000000 data_manipulation-0.8/setup.py
--rw-rw-r--   0 anonymous  (1000) anonymous  (1000)    68611 2020-02-29 09:17:25.000000 data_manipulation-0.8/versioneer.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.770809 data_manipulation-0.9/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       60 2020-02-29 08:00:46.000000 data_manipulation-0.9/MANIFEST.in
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      978 2020-03-07 04:22:42.770809 data_manipulation-0.9/PKG-INFO
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1143 2020-03-01 14:15:16.000000 data_manipulation-0.9/README.md
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.770809 data_manipulation-0.9/data_manipulation/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      186 2020-02-29 15:18:52.000000 data_manipulation-0.9/data_manipulation/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      495 2020-03-07 04:22:42.770809 data_manipulation-0.9/data_manipulation/_version.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.766809 data_manipulation-0.9/data_manipulation/data/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.9/data_manipulation/data/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1008 2020-02-23 11:11:02.000000 data_manipulation-0.9/data_manipulation/data/make_dataset.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.766809 data_manipulation-0.9/data_manipulation/data_types/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       22 2020-02-29 14:54:54.000000 data_manipulation-0.9/data_manipulation/data_types/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     3639 2020-03-07 04:16:23.000000 data_manipulation-0.9/data_manipulation/data_types/string_.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.766809 data_manipulation-0.9/data_manipulation/features/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.9/data_manipulation/features/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.9/data_manipulation/features/build_features.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.766809 data_manipulation-0.9/data_manipulation/geopandas/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       25 2020-02-29 14:54:54.000000 data_manipulation-0.9/data_manipulation/geopandas/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      957 2020-02-29 02:05:18.000000 data_manipulation-0.9/data_manipulation/geopandas/geopandas_.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.770809 data_manipulation-0.9/data_manipulation/models/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.9/data_manipulation/models/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.9/data_manipulation/models/predict_model.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.9/data_manipulation/models/train_model.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.770809 data_manipulation-0.9/data_manipulation/pandas/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       22 2020-02-29 14:54:54.000000 data_manipulation-0.9/data_manipulation/pandas/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)    16135 2020-03-07 03:58:56.000000 data_manipulation-0.9/data_manipulation/pandas/pandas_.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.770809 data_manipulation-0.9/data_manipulation/psycopg2/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       24 2020-02-29 14:54:54.000000 data_manipulation-0.9/data_manipulation/psycopg2/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1235 2020-02-29 02:32:41.000000 data_manipulation-0.9/data_manipulation/psycopg2/psycopg2_.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.770809 data_manipulation-0.9/data_manipulation/pyspark/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       23 2020-03-02 15:28:00.000000 data_manipulation-0.9/data_manipulation/pyspark/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     7589 2020-03-02 15:25:55.000000 data_manipulation-0.9/data_manipulation/pyspark/pyspark_.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.770809 data_manipulation-0.9/data_manipulation/visualization/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.9/data_manipulation/visualization/__init__.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        0 2020-02-23 11:11:02.000000 data_manipulation-0.9/data_manipulation/visualization/visualize.py
+drwxrwxr-x   0 anonymous  (1000) anonymous  (1000)        0 2020-03-07 04:22:42.766809 data_manipulation-0.9/data_manipulation.egg-info/
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      978 2020-03-07 04:22:42.000000 data_manipulation-0.9/data_manipulation.egg-info/PKG-INFO
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1075 2020-03-07 04:22:42.000000 data_manipulation-0.9/data_manipulation.egg-info/SOURCES.txt
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)        1 2020-03-07 04:22:42.000000 data_manipulation-0.9/data_manipulation.egg-info/dependency_links.txt
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       30 2020-03-07 04:22:42.000000 data_manipulation-0.9/data_manipulation.egg-info/requires.txt
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)       18 2020-03-07 04:22:42.000000 data_manipulation-0.9/data_manipulation.egg-info/top_level.txt
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)      230 2020-03-07 04:22:42.770809 data_manipulation-0.9/setup.cfg
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)     1400 2020-03-01 14:15:16.000000 data_manipulation-0.9/setup.py
+-rw-rw-r--   0 anonymous  (1000) anonymous  (1000)    68611 2020-02-29 09:17:25.000000 data_manipulation-0.9/versioneer.py
```

### Comparing `data_manipulation-0.8/PKG-INFO` & `data_manipulation-0.9/data_manipulation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: data_manipulation
-Version: 0.8
+Name: data-manipulation
+Version: 0.9
 Summary: Powerful data manipulation
 Home-page: https://github.com/shawnngtq/data-manipulation
 Author: Shawn Ng
 Author-email: shawn.coding.acc@gmail.com
 License: BSD-3
 Description: 
         Data Manipulation is a Python package providing powerful utility functions.
```

### Comparing `data_manipulation-0.8/README.md` & `data_manipulation-0.9/README.md`

 * *Files identical despite different names*

### Comparing `data_manipulation-0.8/data_manipulation/data/make_dataset.py` & `data_manipulation-0.9/data_manipulation/data/make_dataset.py`

 * *Files identical despite different names*

### Comparing `data_manipulation-0.8/data_manipulation/geopandas/geopandas_.py` & `data_manipulation-0.9/data_manipulation/geopandas/geopandas_.py`

 * *Files identical despite different names*

### Comparing `data_manipulation-0.8/data_manipulation/pandas/pandas_.py` & `data_manipulation-0.9/data_manipulation/pandas/pandas_.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,29 +17,29 @@
 
 def add_type_columns(dataframe):
     """
     Returns Pandas dataframe where each columns has their type column right next to it
 
     Parameters
     ----------
-    dataframe: pandas.core.frame.DataFrame
+    dataframe: pandas.DataFrame
         Dataframe to add type columns
 
     Examples
     --------
     >>> values = [[0, '0', [], {}, None, ""]]
     >>> cols = ["int_", "str_", "list_", "set_", "none_", "_"]
     >>> df = pd.DataFrame(values, columns=cols)
     >>> add_type_columns(df)
        int_      int__type str_      str__type list_      list__type set_       set__type none_          none__type _         __type
     0     0  <class 'int'>    0  <class 'str'>    []  <class 'list'>   {}  <class 'dict'>  None  <class 'NoneType'>    <class 'str'>
 
     Returns
     -------
-    pandas.core.frame.DataFrame
+    pandas.DataFrame
         For each dataframe's column, add a column with it's dtype next to it
     """
     if not isinstance(dataframe, (pd.DataFrame)):
         raise TypeError("Argument must be a Pandas dataframe ...")
 
     suffix = "_type"
     for column in dataframe.columns:
@@ -78,15 +78,15 @@
     2     1     3           False
     3     1     2           False
     4     1     3           False
     5     2     3           False
 
     Returns
     -------
-    pandas.core.frame.DataFrame
+    pandas.DataFrame
         Each row represent 1 of all combinations
     """
     if not isinstance(list_, (list)):
         raise TypeError("Argument must be a list ...")
 
     from itertools import combinations
     result = []
@@ -94,34 +94,34 @@
         row = {"item1": repr(a), "item2": repr(b), "item1_eq_item2": a == b}
         result.append(row)
 
     df = pd.DataFrame(result, columns=["item1", "item2", "item1_eq_item2"])
     return df
 
 
-def columns_dictionary(dataframe):
+def dtypes_dictionary(dataframe):
     """
     Create a dictionary {dtype: [column1, column2 ...]} from Pandas dataframe
 
     Parameters
     ----------
-    dataframe: pandas.core.frame.DataFrame
+    dataframe: pandas.DataFrame
         Base dataframe
 
     Examples
     --------
-    >>> columns_dictionary(pd.DataFrame())
+    >>> dtypes_dictionary(pd.DataFrame())
     Traceback (most recent call last):
       ...
-    ValueError: Argument can't be empty Pandas dataframe ...
+    ValueError: Argument can't be a empty Pandas dataframe ...
 
     >>> values = [[0, '0', [], {}, None, ""]]
     >>> cols = ["int_", "str_", "list_", "set_", "none_", "_"]
     >>> df = pd.DataFrame(values, columns=cols)
-    >>> columns_dictionary(df)
+    >>> dtypes_dictionary(df)
     {<class 'numpy.int64'>: ['int_'], <class 'str'>: ['str_', '_'], <class 'list'>: ['list_'], <class 'dict'>: ['set_'], <class 'NoneType'>: ['none_']}
 
     Returns
     -------
     dict
         {str: [column1, column2, ...], int: [column5, ...], ...}
     """
@@ -143,15 +143,15 @@
 
 def head_tail(dataframe, n=5):
     """
     Print the Pandas dataframe first n head and last n tail
 
     Parameters
     ----------
-    dataframe: pandas.core.frame.DataFrame
+    dataframe: pandas.DataFrame
         Base dataframe
 
     Examples
     --------
     >>> values = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
     >>> cols = ["test"]
     >>> df = pd.DataFrame(values, columns=cols)
@@ -166,15 +166,15 @@
     6     7
     7     8
     8     9
     9    10
 
     Returns
     -------
-    pandas.core.frame.DataFrame
+    pandas.DataFrame
         A dataframe containing n head and tail of base dataframe
     """
     if not isinstance(dataframe, (pd.DataFrame)):
         raise TypeError("Argument must be a Pandas dataframe ...")
 
     result = dataframe.head(n).append(dataframe.tail(n))
     return result
@@ -209,15 +209,15 @@
 
 def chunking_dataframe(dataframe, chunk_size):
     """
     Split Pandas dataframe into dataframes with specific chunk_size
 
     Parameters
     ----------
-    dataframe: pandas.core.frame.DataFrame
+    dataframe: pandas.DataFrame
 
     chunk_size: int
         The chunk size of each smaller dataframes
 
     Examples
     --------
     >>> chunking_dataframe(pd.DataFrame(), 2)
@@ -279,15 +279,15 @@
         - Excel limit of 65,530 urls per worksheet
         - Excel does not keep url > 255 characters
 
     Parameters
     ----------
     filepath: str
         Filepath
-    dataframe: pandas.core.frame.DataFrame
+    dataframe: pandas.DataFrame
         Dataframe to export into excel
 
     Examples
     --------
     >>> values = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
     >>> cols = ["test"]
     >>> df = pd.DataFrame(values, columns=cols)
@@ -311,17 +311,17 @@
 
 def compare_dataframes(dataframe, dataframe2):
     """
     Compare the before & after Pandas dataframe going through data transformation (DT)
 
     Parameters
     ----------
-    dataframe: pandas.core.frame.DataFrame
+    dataframe: pandas.DataFrame
         The Pandas dataframe before DT
-    dataframe2: pandas.core.frame.DataFrame
+    dataframe2: pandas.DataFrame
         The Pandas dataframe after DT
 
     Returns
     -------
     None
         Print output comparison between 2 Pandas dataframes
     """
@@ -383,15 +383,15 @@
        count  percent
     1      2     50.0
     3      1     25.0
     2      1     25.0
 
     Returns
     -------
-    pandas.core.frame.DataFrame
+    pandas.DataFrame
         Enhanced value_counts() in dataframe
     """
     if not isinstance(series, (pd.Series)):
         raise TypeError("Argument must be a Pandas series ...")
 
     result = series.value_counts().to_frame(name="count")
     total = result.sum()["count"]
@@ -401,15 +401,15 @@
 
 def print_dataframe_overview(dataframe, stats=False):
     """
     Print the value_counts() of each column in dataframe
 
     Parameters
     ----------
-    dataframe: pandas.core.frame.DataFrame
+    dataframe: pandas.DataFrame
         Base dataframe
 
     Examples
     --------
     >>> print_dataframe_overview(pd.DataFrame())
 
     >>> data = {"int_": [1, 1, 2], "str_": ["a", "b", "b"]}
@@ -457,15 +457,15 @@
 
 def useless_columns(dataframe):
     """
     Return useless columns
 
     Parameters
     ----------
-    dataframe: pandas.core.frame.DataFrame
+    dataframe: pandas.DataFrame
         Base dataframe
 
     Returns
     -------
     tuple
         (empty_columns, single_columns)
     """
@@ -481,17 +481,17 @@
 
 def split_left_merged_dataframe(dataframe, dataframe2, columns):
     """
     Split left merged dataframe into dataframes ("both", "left_only")
 
     Parameters
     ----------
-    dataframe: pandas.core.frame.DataFrame
+    dataframe: pandas.DataFrame
         Based dataframe
-    dataframe2: pandas.core.frame.DataFrame
+    dataframe2: pandas.DataFrame
         Dataframe to merged with
     columns: list
         Columns to join on
 
     Examples
     --------
     >>> df1 = pd.DataFrame({'key': ['foo', 'bar', 'baz', 'foo'], 'value': [1, 2, 3, 5]})
@@ -528,11 +528,43 @@
     df_merged = dataframe.merge(dataframe2, on=columns, how="left", indicator=True, suffixes=("", "_y"))
     df_both = df_merged[df_merged["_merge"] == "both"].copy()
     df_left = df_merged[df_merged["_merge"] == "left_only"].copy()
     display(series_count(df_merged["_merge"]))
     return df_both, df_left
 
 
+def series_to_columns(dataframe, column):
+    """
+    Convert a pandas dictionary column to pandas column(s)
+
+    Parameters
+    ----------
+    dataframe: pandas.DataFrame
+        Pandas dataframe
+    column: pd.Series
+        Pandas series with dict dtype
+
+    Examples
+    --------
+    >>> values = [[1, {'a':1, 'b':2}]]
+    >>> cols = ["c1", "c2"]
+    >>> df = pd.DataFrame(values, columns=cols)
+    >>> df
+       c1                c2
+    0   1  {'a': 1, 'b': 2}
+    >>> series_to_columns(df, "c2")
+       c1  a  b
+    0   1  1  2
+
+    Returns
+    -------
+    pandas.DataFrame
+        A Pandas dataframe with dictionary column converted to column(s)
+    """
+    df = pd.concat([dataframe.drop([column], axis=1), dataframe[column].apply(pd.Series)], axis=1)
+    return df
+
+
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
```

### Comparing `data_manipulation-0.8/data_manipulation/psycopg2/psycopg2_.py` & `data_manipulation-0.9/data_manipulation/psycopg2/psycopg2_.py`

 * *Files identical despite different names*

### Comparing `data_manipulation-0.8/data_manipulation/pyspark/pyspark_.py` & `data_manipulation-0.9/data_manipulation/pyspark/pyspark_.py`

 * *Files identical despite different names*

### Comparing `data_manipulation-0.8/data_manipulation.egg-info/PKG-INFO` & `data_manipulation-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: data-manipulation
-Version: 0.8
+Name: data_manipulation
+Version: 0.9
 Summary: Powerful data manipulation
 Home-page: https://github.com/shawnngtq/data-manipulation
 Author: Shawn Ng
 Author-email: shawn.coding.acc@gmail.com
 License: BSD-3
 Description: 
         Data Manipulation is a Python package providing powerful utility functions.
```

### Comparing `data_manipulation-0.8/data_manipulation.egg-info/SOURCES.txt` & `data_manipulation-0.9/data_manipulation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_manipulation-0.8/setup.py` & `data_manipulation-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `data_manipulation-0.8/versioneer.py` & `data_manipulation-0.9/versioneer.py`

 * *Files identical despite different names*

