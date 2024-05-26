# Comparing `tmp/dataframe_short-0.1.5.tar.gz` & `tmp/dataframe_short-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_short-0.1.5.tar", last modified: Mon Apr 29 05:08:13 2024, max compression
+gzip compressed data, was "dataframe_short-0.1.6.tar", last modified: Sun May 26 03:42:36 2024, max compression
```

## Comparing `dataframe_short-0.1.5.tar` & `dataframe_short-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 05:08:13.831220 dataframe_short-0.1.5/
--rw-rw-rw-   0        0        0      267 2024-04-29 05:08:13.831220 dataframe_short-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 05:08:13.815845 dataframe_short-0.1.5/dataframe_short/
--rw-rw-rw-   0        0        0      119 2024-04-29 05:06:15.000000 dataframe_short-0.1.5/dataframe_short/__init__.py
--rw-rw-rw-   0        0        0     7713 2024-04-29 04:40:51.000000 dataframe_short-0.1.5/dataframe_short/dataframe_test.py
--rw-rw-rw-   0        0        0     2803 2024-03-11 03:40:50.000000 dataframe_short-0.1.5/dataframe_short/func_24_Feb.py
--rw-rw-rw-   0        0        0    49373 2024-04-29 04:41:04.000000 dataframe_short-0.1.5/dataframe_short/lib02_dataframe.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:08:13.829225 dataframe_short-0.1.5/dataframe_short.egg-info/
--rw-rw-rw-   0        0        0      267 2024-04-29 05:08:13.000000 dataframe_short-0.1.5/dataframe_short.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2024-04-29 05:08:13.000000 dataframe_short-0.1.5/dataframe_short.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 05:08:13.000000 dataframe_short-0.1.5/dataframe_short.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-29 05:08:13.000000 dataframe_short-0.1.5/dataframe_short.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 05:08:13.000000 dataframe_short-0.1.5/dataframe_short.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 05:08:13.832217 dataframe_short-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      387 2024-04-29 05:06:07.000000 dataframe_short-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:42:36.025867 dataframe_short-0.1.6/
+-rw-rw-rw-   0        0        0     1090 2024-04-29 08:07:37.000000 dataframe_short-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      238 2024-05-26 03:42:36.025867 dataframe_short-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-04-29 08:07:37.000000 dataframe_short-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 03:42:35.995948 dataframe_short-0.1.6/dataframe_short/
+-rw-rw-rw-   0        0        0      112 2024-05-25 02:41:43.000000 dataframe_short-0.1.6/dataframe_short/__init__.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:07.000000 dataframe_short-0.1.6/dataframe_short/cant_use_ds.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:00.000000 dataframe_short-0.1.6/dataframe_short/fix_bug_ds.py
+-rw-rw-rw-   0        0        0     2803 2024-05-01 01:56:28.000000 dataframe_short-0.1.6/dataframe_short/func_24_Feb.py
+-rw-rw-rw-   0        0        0        0 2024-05-25 03:11:45.000000 dataframe_short-0.1.6/dataframe_short/sandbox1_ds.py
+-rw-rw-rw-   0        0        0    48011 2024-05-25 04:27:04.000000 dataframe_short-0.1.6/dataframe_short/utils_ds.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:42:36.023872 dataframe_short-0.1.6/dataframe_short.egg-info/
+-rw-rw-rw-   0        0        0      238 2024-05-26 03:42:35.000000 dataframe_short-0.1.6/dataframe_short.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2024-05-26 03:42:35.000000 dataframe_short-0.1.6/dataframe_short.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 03:42:35.000000 dataframe_short-0.1.6/dataframe_short.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-26 03:42:35.000000 dataframe_short-0.1.6/dataframe_short.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-26 03:42:35.000000 dataframe_short-0.1.6/dataframe_short.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 03:42:36.026865 dataframe_short-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      433 2024-05-26 03:41:26.000000 dataframe_short-0.1.6/setup.py
```

### Comparing `dataframe_short-0.1.5/dataframe_short/func_24_Feb.py` & `dataframe_short-0.1.6/dataframe_short/func_24_Feb.py`

 * *Files identical despite different names*

### Comparing `dataframe_short-0.1.5/dataframe_short/lib02_dataframe.py` & `dataframe_short-0.1.6/dataframe_short/utils_ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,71 @@
 @author: Heng2020
 """
 import pandas as pd
 import numpy as np
 from itertools import product
 from collections import defaultdict
 import sys
-
-# from lib01_xgb import *
-# import string_01 as pst
+from typing import List, Tuple, Literal, Union
 import py_string_tool as pst
 
-def indexAlignedAppend(df1, df2, col_name):
+
+def rename_col_by_index(df, index, new_name, inplace=True):
+    """
+    medium tested
+    Rename a column in a DataFrame based on its index (this can handle repeated name)
+
+    Parameters:
+    df (pd.DataFrame): The DataFrame whose column you want to rename.
+    index (int): The index of the column to rename.
+    new_name (str): The new name for the column.
+    inplace (bool): If True, modifies the DataFrame in place (default is True).
+
+    Returns:
+    pd.DataFrame or None: The DataFrame with the renamed column if inplace is False, otherwise None.
+    """
+    # Ensure the index is within the valid range
+    if not 0 <= index < len(df.columns):
+        raise IndexError("Column index out of range.")
+    
+    # Copy df if not inplace
+    if not inplace:
+        df = df.copy()
+    
+    # Set new column name
+    df.columns = df.columns[:index].tolist() + [new_name] + df.columns[index+1:].tolist()
+    
+    if not inplace:
+        return df
+
+def to_list(df_sr_list):
+    import pandas as pd
+    # can only be used in this code bc it select 1st column(not all column)
+    # convert pd.Dataframe, series, list, or 1string to list
+    out_list = []
+    # select only 1st column
+    if isinstance(df_sr_list, list):
+        out_list = df_sr_list
+        
+    elif isinstance(df_sr_list, pd.DataFrame):
+        out_list = df_sr_list.iloc[:, 0].values.tolist()
+        
+    elif isinstance(df_sr_list, pd.Series):
+        out_list = df_sr_list.tolist()
+        
+    elif isinstance(df_sr_list, (int,float,complex,str)):
+        out_list = [df_sr_list]
+    
+    else:
+        print("This datatype is not suppored by this function")
+        return False
+    
+    return out_list
+
+def index_aligned_append(df1, df2, col_name):
     # it works: medium tested
     import pandas as pd
     """
     Appends rows from df2 to df1 based on a specific column (col_name).
     And readjust the index in each episode via (col_name)
     
     Inspired by BigBang theory script
@@ -100,22 +151,22 @@
 
         if extract_pattern is None:
             name_filter = filename
         else:
             name_filter = re.search(extract_pattern, filename).group()
         # curr_df.columns.values[0] = 'NoSentence'
         curr_df[filename_col_name] = name_filter
-        pd_move_col_front(curr_df, filename_col_name)
+        move_col_front(curr_df, filename_col_name)
         out_df = pd.concat([out_df,curr_df])
 
     return out_df
 
 
 # ########################################## imported from work Mar 17, 2024 #######################################################################
-def df_to_str_decimal(df,cols,decimal_place = 1, inplace = True, except_level = []):
+def to_str_decimal(df,cols,decimal_place = 1, inplace = True, except_level = []):
     # based on pd = 2.1.0
     # Next: add except_level
     from pandas.api.types import is_numeric_dtype
 
     if isinstance(cols,list):
         except_level_in = list(cols)
     else:
@@ -127,61 +178,15 @@
         cols_in = [cols]
     
     for col in cols_in:
         if is_numeric_dtype(df[col]):
             df[col] = df[col].apply(lambda row: f"{row:.{decimal_place}f}")
         # df[col] = df[col].apply(lambda row: f"{row:.{decimal_place}f}" if row not in except_level, axis = 1)
 
-
-def df_XLookup(df_main, df_lookup, lookup_col, key_col, return_col, inplace=True):
-    """
-    Perform an XLOOKUP-like operation on DataFrames.
-
-    Parameters:
-        df_main (pd.DataFrame): Main DataFrame.
-        df_lookup (pd.DataFrame): Lookup DataFrame.
-        lookup_col (str or list[str]): Column(s) in df_main to use for lookup.
-        key_col (str): Column in df_lookup to match with lookup_col.
-        return_col (str or list[str]): Column(s) in df_lookup to return.
-        inplace (bool, optional): If True, modifies df_main in-place. Otherwise, returns a new DataFrame. Default is True.
-
-    Returns:
-        pd.DataFrame: Modified df_main if inplace=True, otherwise a new DataFrame.
-    """
-    # Ensure lookup_col is a list
-    if not isinstance(lookup_col, list):
-        lookup_col = [lookup_col]
-
-    # Merge DataFrames
-    merged_df = pd.merge(df_main, df_lookup, left_on=lookup_col, right_on=key_col, how='left')
-
-    # Keep only the specified return columns
-    if isinstance(return_col, str):
-        return_col = [return_col]  # Convert single column name to list
-
-    if inplace:
-        for col in return_col:
-            df_main[col] = merged_df[col]
-        return df_main
-    else:
-        return merged_df[return_col]
-
-def pd_shape(df):
-    # originally from lib01
-    # but upgraded
-    # medium tested
-    import pandas as pd
-    if isinstance(df, pd.DataFrame):
-        print("The shape ({:,} * {:,})".format(*df.shape))
-    # to support when df.shape is an input
-    elif isinstance(df, tuple):
-        print("The shape ({:,} * {:,})".format(*df))
-
-
-def pd_to_datetime(df,cols = None,inplace=True, print_col = True):
+def to_datetime(df,cols = None,inplace=True, print_col = True):
     # little tested
     # required: pd_get_col
     """
     Convert columns of a DataFrame to datetime dtype.
 
     This function uses the pd.to_datetime() function to convert the columns
     of a DataFrame that contain date-like values to datetime dtype. It can
@@ -228,15 +233,15 @@
     0 2020-01-01 1970-01-01
     1 2020-01-02 1970-01-02
     """
 
     import pandas as pd
 
     if cols is None:
-        cols = pd_get_col(df,contain='date',print_col=print_col)
+        cols = get_col(df,contain='date',print_col=print_col)
 
     
     out_df = pd.DataFrame()
     
     if not inplace:
         out_df = df.copy()
     
@@ -245,15 +250,108 @@
             df[col] = pd.to_datetime(df[col]) 
         else:
             out_df[col] = pd.to_datetime(out_df[col]) 
     
     if not inplace:
         return out_df
 
-def df_sum_all(df,value_col,exclude = None, inplace = False, dropna = False):
+def to_num(df,cols,num_type = "int64",inplace = True,fill_na = 0):
+    # fill_na has to be 0 for it to work properly ----> need more investigation
+    
+    # it seems to work even when it's already number
+    # must import
+    from pandas.api.types import is_object_dtype
+    if isinstance(cols, str):
+        # convert to list
+        cols_ = [cols]
+    else:
+        cols_ = [x for x in cols]
+        
+    if isinstance(cols_, list):
+        for col in cols_:
+            if is_object_dtype(df[col]):
+                try:
+                    df[col] = df[col].str.replace("," ,  "")
+                    if fill_na is not False: 
+                        df[col] = df[col].fillna(fill_na)
+                    # df[col] = df[col].astype(num_type)
+                    df[col] = pd.to_numeric(df[col],errors='coerce')
+                except Exception as e:
+                    e_str = str(e)
+                    print(e_str)
+                    print(f"'{col}' has an error")
+
+    else:
+        pass
+
+def to_str(df,cols = None,inplace = True,fill_na = False):
+    # if cols is None convert all columns to string
+    if cols is None:
+        cols_ = list(df.columns)
+    elif isinstance(cols, str):
+        # convert to list
+        cols_ = [cols]
+    else:
+        cols_ = [x for x in cols]
+        
+    if isinstance(cols_, list):
+        for col in cols_:
+            df[col] = df[col].astype(str)
+    else:
+        pass
+
+
+def x_lookup(df_main, df_lookup, lookup_col, key_col, return_col, inplace=True):
+    """
+    Perform an XLOOKUP-like operation on DataFrames.
+
+    Parameters:
+        df_main (pd.DataFrame): Main DataFrame.
+        df_lookup (pd.DataFrame): Lookup DataFrame.
+        lookup_col (str or list[str]): Column(s) in df_main to use for lookup.
+        key_col (str): Column in df_lookup to match with lookup_col.
+        return_col (str or list[str]): Column(s) in df_lookup to return.
+        inplace (bool, optional): If True, modifies df_main in-place. Otherwise, returns a new DataFrame. Default is True.
+
+    Returns:
+        pd.DataFrame: Modified df_main if inplace=True, otherwise a new DataFrame.
+    """
+    # Ensure lookup_col is a list
+    if not isinstance(lookup_col, list):
+        lookup_col = [lookup_col]
+
+    # Merge DataFrames
+    merged_df = pd.merge(df_main, df_lookup, left_on=lookup_col, right_on=key_col, how='left')
+
+    # Keep only the specified return columns
+    if isinstance(return_col, str):
+        return_col = [return_col]  # Convert single column name to list
+
+    if inplace:
+        for col in return_col:
+            df_main[col] = merged_df[col]
+        return df_main
+    else:
+        return merged_df[return_col]
+
+def shape(df):
+    # originally from lib01
+    # but upgraded
+    # medium tested
+    import pandas as pd
+    if isinstance(df, pd.DataFrame):
+        print("The shape ({:,} * {:,})".format(*df.shape))
+    # to support when df.shape is an input
+    elif isinstance(df, tuple):
+        print("The shape ({:,} * {:,})".format(*df))
+
+
+
+
+def sum_all(df,value_col,exclude = None, inplace = False, dropna = False):
     """ This will sum the value_col grouped by other_column """
 
     test01 = df.groupby(['aPol_CalYear'])[['exposure','claim_count','total_paid']].sum()
     if exclude is None:
         exclude = []
 
     other_column = list(df.columns.difference(value_col))
@@ -265,15 +363,15 @@
     test02 = df_agg.groupby(['aPol_CalYear'], dropna = False)[['exposure','claim_count','total_paid']].sum()
     if inplace: 
         df = df_agg
         return df
     else:
         return df_agg
 
-def pd_count_freq(df, groupby_col, value_col):
+def count_freq(df, groupby_col, value_col):
     """
     Count the frequency of values in a column and return a dataframe.
 
     This function creates dummy variables for the values in the value_col
     column of the input dataframe df, and then groups by the groupby_col
     column and sums the dummy variables. The result is a dataframe with
     the groupby_col as the index and the n_ prefixed value_col values as
@@ -336,19 +434,19 @@
     for n, df in enumerate(list_dfs):
         if isinstance(sheet_name,list):
             df.to_excel(writer, sheet_name = sheet_name[n])
         else:
             df.to_excel(writer,'sheet%s' % n)
     writer.save()
 
-def pd_common_col(df1,df2):
+def common_col(df1,df2):
     common_col = [x for x in list(df1.columns) if x in list(df2.columns) ]
     return common_col
 
-def pd_get_col(df,start_with = "",end_with ="", contain = "", case_sensitive=False, print_col=True):
+def get_col(df,start_with = "",end_with ="", contain = "", case_sensitive=False, print_col=True):
 
 # this is from print_col 
 # !!! TODO start_with, end_with, contain is list
 # add 2 logic options
 
     cols = list(df.columns)
     
@@ -376,15 +474,15 @@
     if print_col:
         for col in cols:
             print(col)
 
     return cols
 
 
-def pd_merge2(left, 
+def merge2(left, 
              right, 
              how='inner', 
              on=None, 
              left_on=None, 
              right_on=None,
              keep = "left"):
     
@@ -417,17 +515,17 @@
     
     df_merged = pd.merge(left,right,how,on,left_on,right_on)
     # if keep == "left":
     #     df_merged = pd.merge(left,right,how,on,left_on,right_on,suffixes=('', '_remove'))
     # elif keep == "right":
     #     df_merged = pd.merge(left,right,how,on,left_on,right_on,suffixes=('_remove', ''))
     
-    x_col = pd_get_col(df_merged,end_with = "_x",print_col=False)
+    x_col = get_col(df_merged,end_with = "_x",print_col=False)
     
-    xy_col = list(zip(pd_get_col(df_merged,end_with = "_x",print_col=False),pd_get_col(df_merged,end_with = "_y",print_col=False) ))
+    xy_col = list(zip(get_col(df_merged,end_with = "_x",print_col=False),get_col(df_merged,end_with = "_y",print_col=False) ))
 
     for x_col, y_col in xy_col:
         col_name = x_col.split("_")[0]
         df_merged[col_name] = df_merged.apply(lambda row: func_keep(row[x_col],row[y_col],keep), axis = 1)
         
         # df_merged = df_merged.sort_index(axis=1)
         
@@ -437,15 +535,15 @@
 
         
     # df_merged.drop([i for i in df_merged.columns if 'remove' in i],
     #            axis=1, inplace=True)
     return df_merged
 
 
-def pd_merge(left, 
+def merge(left, 
              right, 
              how='inner', 
              on=None, 
              left_on=None, 
              right_on=None,
              keep = "left"):
 
@@ -466,20 +564,20 @@
     
     df_merged = pd.merge(left,right,how,on,left_on,right_on)
     # if keep == "left":
     #     df_merged = pd.merge(left,right,how,on,left_on,right_on,suffixes=('', '_remove'))
     # elif keep == "right":
     #     df_merged = pd.merge(left,right,how,on,left_on,right_on,suffixes=('_remove', ''))
     
-    x_col_list = pd_get_col(df_merged,end_with = "_x",print_col=False)
-    y_col_list = pd_get_col(df_merged,end_with = "_y",print_col=False)
+    x_col_list = get_col(df_merged,end_with = "_x",print_col=False)
+    y_col_list = get_col(df_merged,end_with = "_y",print_col=False)
     
     xy_col_list = x_col_list + y_col_list
     
-    xy_col = list(zip(pd_get_col(df_merged,end_with = "_x",print_col=False),pd_get_col(df_merged,end_with = "_y",print_col=False) ))
+    xy_col = list(zip(get_col(df_merged,end_with = "_x",print_col=False),get_col(df_merged,end_with = "_y",print_col=False) ))
 
     for x_col, y_col in xy_col:
         col_name = x_col.split("_x")[0]
         
         if col_name == "Effective Date":
             # for debug
             print("")
@@ -511,44 +609,16 @@
 
         
     # df_merged.drop([i for i in df_merged.columns if 'remove' in i],
     #            axis=1, inplace=True)
     return df_merged
 
 
-def pd_to_num(df,cols,num_type = "int64",inplace = True,fill_na = 0):
-    # fill_na has to be 0 for it to work properly ----> need more investigation
-    
-    # it seems to work even when it's already number
-    # must import
-    from pandas.api.types import is_object_dtype
-    if isinstance(cols, str):
-        # convert to list
-        cols_ = [cols]
-    else:
-        cols_ = [x for x in cols]
-        
-    if isinstance(cols_, list):
-        for col in cols_:
-            if is_object_dtype(df[col]):
-                try:
-                    df[col] = df[col].str.replace("," ,  "")
-                    if fill_na is not False: 
-                        df[col] = df[col].fillna(fill_na)
-                    # df[col] = df[col].astype(num_type)
-                    df[col] = pd.to_numeric(df[col],errors='coerce')
-                except Exception as e:
-                    e_str = str(e)
-                    print(e_str)
-                    print(f"'{col}' has an error")
-
-    else:
-        pass
 
-def pd_move_col_front(df, cols, inplace=True):
+def move_col_front(df, cols, inplace=True):
     """
     old code
     # based on pd version == 2.1.3
     
     Reorder the columns of a dataframe by moving some columns to the front.
 
     Parameters
@@ -601,15 +671,15 @@
     if inplace:
         df.columns = df_new.columns
         df[:] = df_new
         # return None
     else:
         return df_new
 
-# def pd_move_col_front(df, cols, inplace=True):
+# def move_col_front(df, cols, inplace=True):
 #     """
 #     from Claude 3(solo)
 #     # based on pd version == 2.1.3
 
 #     Reorder the columns of a dataframe by moving some columns to the front.
 
 #     Parameters
@@ -671,15 +741,15 @@
 #             df[col] = df[col].astype(dtypes[col])
 #         # return None
 #     else:
 #         return df_new
 
 
 
-def pd_check_col(df, columns):
+def check_col(df, columns):
     # Create an empty list to store the tuples
     result = []
     
     # Loop through the columns list
     for col in columns:
         # Check if the column is in df.columns using the isin() method
         # This will return a boolean Series with one element
@@ -688,83 +758,14 @@
         
         # Append a tuple of the column name and the boolean value to the result list
         result.append((col, is_in))
     
     # Return the result list
     return result
 
-def custom_sort(lst, begin_with, end_with,ascending=True, string_last = True):
-    import re
-    # medium tested
-    
-    # what if there's no begin_with or end_with?
-
-    # cover when begin_with is string
-    # cover when end_with is string
-    
-    sort_by = []
-    
-    have_begin = []
-    have_end = []
-    
-    large_num = 2*len(lst)
-    count = 0
-    # ['m.>30', 'b.-30to-20', 'a.<-30', 'l.21to30', 'd.-14to-10', 'j.11to15', 'i.6to10', 'h.1to5', 'e.-9to-5', 'f.-4to-1', 'c.-19to-15', 'g.0', 'k.16to20']
-    # check only first element
-    if isinstance(lst[0], str):
-        match = re.search(r'[a-zA-Z]\.', lst[0])
-    else:
-        # If it's a number 
-        match = False
-    
-    if match:
-        sorted_list = sorted(lst,reverse=not ascending)
-        return sorted_list
-    for val in lst:
-        try:
-            num = float(val)
-            sort_by.append(num)
-        except ValueError:
-            num_02 = val.split(" ")[0]
-            num_03 = pst.St_GetNum(num_02)
-            
-            # string case
-            if val in begin_with:
-                order_index = -large_num + begin_with.index(val)
-                sort_by.append(order_index)
-                
-            elif val in end_with:
-                order_index = large_num + begin_with.index(val)
-                sort_by.append(order_index)
-                
-            else:
-                if num_03 is False:
-                    
-                    # if val not in either begin_with nor end_with
-                    if string_last:
-                        # put string at the end
-                        order_index = large_num + count
-                        count += 1
-                    else:
-                        # put string at the beginning
-                        order_index = -large_num + count
-                        count += 1
-                    sort_by.append(order_index)
-                else:
-                    sort_by.append(num_03)
-                
-                    
-                    
-    # sort_by.sort(reverse = not ascending)
-
-                    
-    
-    sorted_list = [x for x, y in sorted(zip(lst, sort_by), key=lambda pair: pair[1])]
-    # print(sorted_list01)
-    return sorted_list
 
 
 def unique_element(df, include=None, 
                exclude=None, 
                sort_by='n_elements',
                ascending=True,
                list_ascending = True
@@ -840,66 +841,14 @@
     
     out_df = out_df.reset_index(drop=True)
 
     # Return the output dataframe
     return out_df
 
 
-def emblem_base(df, value_col="exposure", choose="max"):
-    # medium tested
-    """
-    For each column except for value_col, sum value_col grouped by the unique elements of each column.
-    Then, depending on the choose parameter, create a dictionary with the key being that column name and the value being the element with the highest or lowest sum of value_col.
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        The input data frame.
-    value_col : str, optional
-        The name of the column that contains the values to be summed. The default is "exposure".
-    choose : str, optional
-        The option to select the element with the highest or lowest sum of value_col. The default is "max".
-
-    Returns
-    -------
-    dictt : dict
-        The output dictionary with the column names as keys and the selected elements as values.
-
-    Examples
-    --------
-    >>> df = pd.DataFrame({'country': ['USA', 'USA', 'Canada', 'Canada', 'Mexico', 'Mexico'],
-                           'gender': ['M', 'F', 'M', 'F', 'M', 'F'],
-                           'exposure': [100, 200, 300, 400, 500, 600]})
-    >>> emblem_base(df)
-    {'country': 'Mexico', 'gender': 'F'}
-    >>> emblem_base(df, choose='min')
-    {'country': 'USA', 'gender': 'M'}
-    """
-    
-    # create an empty dictionary to store the results
-    dictt = {}
-    
-    # loop through each column except for value_col
-    for col in df.columns:
-        if col != value_col:
-            # group by the column and sum the value_col
-            grouped = df.groupby(col)[value_col].sum()
-            # depending on the choose parameter, select the element with the highest or lowest sum
-            if choose == "max":
-                element = grouped.idxmax()
-            elif choose == "min":
-                element = grouped.idxmin()
-            else:
-                raise ValueError("Invalid choose parameter. It must be either 'max' or 'min'.")
-            # add the column name and the element to the dictionary
-            dictt[col] = element
-    
-    # return the dictionary
-    return dictt
-
 
 
 
 def cat_report(df, include=None, 
                exclude=None, 
                cut_off=15, 
                sort_by='n_elements',
@@ -995,28 +944,28 @@
 
     df_temp = df[col]
     order_df = unique_element(df_temp)
     order_df['element_sorted'] = order_df['elements'].apply(lambda x: custom_sort(x,begin_with,end_with))
     out_dict = dict(zip(order_df['col_name'], order_df['element_sorted']))
     return out_dict
 
-def pd_reorder(df,col,begin_with = None,end_with = None):
+def reorder(df,col,begin_with = None,end_with = None):
     mapping_dict = reorder_dict(df,col,begin_with,end_with)
     
     for col, new_order in mapping_dict.items():
         df[col] = df[col].cat.reorder_categories(new_order)
     
     return df
 
 
-def pd_shape(df):
+def shape(df):
     print("The shape ({:,} * {:,})".format(*df.shape))
 
 
-def pd_duplicate_col(df):
+def duplicate_col(df):
     # Get the column names of the DataFrame
     col_names = df.columns
     
     # Create an empty list to store the duplicated column names
     dup_cols = []
     
     # Loop through the column names and check if there are duplicates
@@ -1040,47 +989,32 @@
         print("There's no duplicated columns")
         return False
     else:
         # If not empty, return the dup_cols list
         return dup_cols
 
 
-def pd_to_str(df,cols = None,inplace = True,fill_na = False):
-    # if cols is None convert all columns to string
-    if cols is None:
-        cols_ = list(df.columns)
-    elif isinstance(cols, str):
-        # convert to list
-        cols_ = [cols]
-    else:
-        cols_ = [x for x in cols]
-        
-    if isinstance(cols_, list):
-        for col in cols_:
-            df[col] = df[col].astype(str)
-    else:
-        pass
 
 # -------------------------------------------------- imported from work Mar 17, 2024 ------------------------------------------------------
 
 
 
-def swap_columns(df, col1, col2):
+def swap_col(df, col1, col2):
     """Swap two columns in a DataFrame."""
     column_list = list(df.columns)
     col1_index, col2_index = column_list.index(col1), column_list.index(col2)
     
     # Swap the positions in the column list
     column_list[col2_index], column_list[col1_index] = column_list[col1_index], column_list[col2_index]
     
     # Reorder the DataFrame according to the new column list
     return df[column_list]
 
 
-def df_value_index(df, value):
+def value_index(df, value):
     """
     Searches for a specific value in the DataFrame using a vectorized approach
     and returns a new DataFrame with the row and column indices where the value
     is found.
 
     Parameters:
     - df: The input pandas DataFrame to search.
@@ -1116,15 +1050,15 @@
     total_rows = df.shape[0]
     # Compute the proportion of null values in each column
     null_proportions = null_counts / total_rows
     # Create a dictionary mapping column names to null proportions
     result = dict(zip(df.columns, null_proportions))
     return result
 
-def pd_common_elements(series_1,series_2):
+def common_element(series_1,series_2):
     # imported from "C:\Users\Heng2020\OneDrive\Python NLP\NLP 08_VocabList\VocatList_func01.py"
 
     """
     series_1 
 
     Parameters
     ----------
@@ -1138,29 +1072,29 @@
     common_elements : list
 
     """
     common_elements = list(set(series_1).intersection(series_2))
     return common_elements
 
 
-def pd_is_same(df1,df2):
+def is_same(df1,df2):
     # imported from "C:\Users\Heng2020\OneDrive\Python NLP\NLP 08_VocabList\VocatList_func01.py"
     
     """ check if each row is the same or not regardless of their row index?
     
     """
     sorted_df1 = df1.sort_values(by=df1.columns.tolist()).reset_index(drop=True)
     sorted_df2 = df2.sort_values(by=df2.columns.tolist()).reset_index(drop=True)
     
     # Check if the sorted DataFrames are exactly the same
     are_rows_identical = sorted_df1.equals(sorted_df2)
     
     return are_rows_identical
 
-# def pd_read_excel(filepath,sheet_name = 0, header = 1):
+# def read_excel(filepath,sheet_name = 0, header = 1):
 #     # this function is designed to read to pd.df that allow me to open the workbook
 #     # at the same time
 #     # medium tested
 #     import xlwings as xw
     
 #     if header is None:
 #         header = False
@@ -1173,17 +1107,18 @@
     
 #     # Convert the used range to a Pandas DataFrame
 #     df = used_range.options(pd.DataFrame, header=header, index=False).value
     
 #     return df
 
 
-def pd_read_excel(filepath, sheet_name=0, header_row=1, start_row=None, end_row=None):
+def read_excel(filepath, sheet_name=0, header_row=1, start_row=None, end_row=None):
     import pandas as pd
     import xlwings as xw
+    import numpy as np
     # Hard for both Cluade3 & GPT4
     # medium tested
     # took about 1.5 hr(include testing)
     """
     
     Read an Excel file into a Pandas DataFrame.
 
@@ -1233,15 +1168,15 @@
     out_df.columns = out_df.iloc[0]
     out_df = out_df[1:]
     out_df.reset_index(drop=True, inplace=True)
 
     return out_df
 
 
-def pd_regex_index(df,regex, column):
+def regex_index(df,regex, column):
     # from C:/Users/Heng2020/OneDrive/Python NLP/NLP 07_Sentence Alignment
     # middle tested by read_movie_script
     
     # used by: pd_split_into_dict_df
     
     """
     
@@ -1280,49 +1215,71 @@
     ans_index = boolean_df[boolean_df].index.tolist()
     
     if len(ans_index) == 1:
         ans_index = ans_index[0]
     
     return ans_index
 
-def pd_split_into_dict_df(df,regex = None, regex_column = None, index_list = None):
+def split_into_dict_df(df,regex = None, regex_column = None, index_list = None,add_prefix_index = False):
     # from C:/Users/Heng2020/OneDrive/Python NLP/NLP 07_Sentence Alignment
     # middle tested by read_movie_script
     # if index_list is supplied then ignore regex, regex_column
     
     # dependency: pd_split_into_dict_df, pd_regex_index
+    from collections import OrderedDict
+    df_dict = OrderedDict()
 
-
-    if index_list is None:
-        index_list_used = pd_regex_index(df,regex,regex_column)
+    # split using header
+    if (regex is None) and (regex_column is None) and (index_list is None):
+        # imported from C:/Users/Heng2020/OneDrive/D_Code/Python/Python NLP/NLP 02/NLP_2024/NLP 11_Local_TTS
+        index_list_used = df.index[df.iloc[:, 1:].isnull().all(axis=1) & df.iloc[:, 0].notnull()].tolist()
+
+        # Use the values of the first column as keys and the slices between the found indices as dictionary values
+        n_dict = len(index_list_used)
+        i = 1
+        for start, end in zip(index_list_used, index_list_used[1:] + [None]):  # Adding None to handle till the end of the DataFrame
+            format_num = pst.format_index_num(i, n_dict)
+            if add_prefix_index:
+                key = format_num + "_" + df.iloc[start, 0]  # The key is the value in the first column
+            else:
+                key = df.iloc[start, 0]
+            # Slice the DataFrame from the current index to the next one in the list
+            each_df = df.iloc[start+1:end].reset_index(drop=True)
+            each_df = each_df.dropna(how='all')
+            
+            df_dict[key] = each_df
+            i += 1
     else:
-        index_list_used = [x for x in index_list]
-    
-    df_dict = {}
-    start_index = 0
-    
-    temp_df : pd.DataFrame
-    
-    for end_index in index_list_used:
-        # Slice the dataframe for each episode
-        temp_df = df.iloc[start_index:end_index, :]
+        if index_list is None:
+            index_list_used = pd_regex_index(df,regex,regex_column)
+        else:
+            index_list_used = [x for x in index_list]
+        
+        
+        start_index = 0
+        
+        temp_df : pd.DataFrame
+        
+        for end_index in index_list_used:
+            # Slice the dataframe for each episode
+            temp_df = df.iloc[start_index:end_index, :]
 
-        if not temp_df.empty:
-            # Get the episode identifier from the first row
-            episode_identifier = temp_df.iloc[0, 0]
-            temp_df = temp_df.reset_index(drop=True)
-            temp_df = temp_df.drop(0)
-            # Store the dataframe in the dictionary
-            df_dict[episode_identifier] = temp_df
+            if not temp_df.empty:
+                # Get the episode identifier from the first row
+                episode_identifier = temp_df.iloc[0, 0]
+                temp_df = temp_df.reset_index(drop=True)
+                temp_df = temp_df.drop(0)
+                # Store the dataframe in the dictionary
+                df_dict[episode_identifier] = temp_df
 
-        start_index = end_index
+            start_index = end_index
         
     return df_dict
 
-def pd_by_column(df, columns):
+def by_col(df, columns):
     # from C:/Users/Heng2020/OneDrive/Python NLP/NLP 07_Sentence Alignment
     # middle tested by read_movie_script
     # slice the dataFrame refer to by str or int
     
     if isinstance(columns, (str,int,float)):
         column_list = [columns]
     else:
@@ -1336,57 +1293,60 @@
         elif isinstance(col, (int,float)):
             col_index.append(int(col))
     
     out_df = df.iloc[:,col_index]
     return out_df
 
 
-def pd_num_to_cat(data,num_to_cat_col):
+def num_to_cat(data,num_to_cat_col):
     if type(num_to_cat_col) == str:
         data[num_to_cat_col] = data[num_to_cat_col].astype(str)
     else:
         for col_name in num_to_cat_col:
             data[col_name] = data[col_name].astype(str)
     return data
 
-def pd_num_to_cat02(data,num_to_cat_col):
+def num_to_cat02(data,num_to_cat_col):
     # change to category instead of str()
     # this also convert column(object) to category
     if type(num_to_cat_col) == str:
         data[num_to_cat_col] = data[num_to_cat_col].astype("category")
     else:
         for col_name in num_to_cat_col:
             data[col_name] = data[col_name].astype("category")
             
         obj_cols = data.select_dtypes(include=['object']).columns
         data[obj_cols] = data[obj_cols].astype('category')
     return data
 
-def pd_drop_column(data, drop_col):
+def drop_column(data, drop_col):
+    """
+    it will not throw an error when there's no column in data.columns
+    """
     for col in drop_col:
         if col in data.columns:
             data.drop(col, axis=1, inplace=True)
         else:
             print(f"This column doesn't exist:  '{col}' ")
     
     return data
 
 
-def pd_cat_column(data):
+def cat_col(data):
     cat_cols = data.select_dtypes(include=['object','category']).columns.tolist()
     return cat_cols
 
-def pd_num_column(data):
+def num_col(data):
     num_cols = data.select_dtypes(include=np.number).columns.tolist()
     return num_cols
 
-def pd_select_column(data,used_col,drop_col):
+def select_col(data,used_col,drop_col):
     pass
     
-def pd_to_category(data):
+def to_category(data):
     object_cols = data.select_dtypes(include=['object']).columns
     data[object_cols] = data[object_cols].astype('category')
     return data
 
 def create_dummy(data,exclude=None):
     # Get the list of categorical and object columns
     categorical_cols = data.select_dtypes(include=['category', 'object']).columns
@@ -1400,39 +1360,39 @@
     data_with_dummies = pd.concat([data, dummy_variables], axis=1)
     
     # Drop the original categorical columns
     data_with_dummies.drop(categorical_cols, axis=1, inplace=True)
     
     return data_with_dummies
 
-def pd_combination(dict_in):
+def combination(dict_in):
     # Get all combinations of values for each key in the dictionary
     combinations = product(*dict_in.values())
     
     # Create a list of dictionaries with all combinations of key-value pairs
     list_of_dicts = [dict(zip(dict_in.keys(), combo)) for combo in combinations]
     
     # Convert the list of dictionaries to a pandas DataFrame
     pd_combinations = pd.DataFrame(list_of_dicts)
     
     return pd_combinations
 
-def pd_cat_combi(pd_in):
+def cat_combi(pd_in):
 
     cat_dict = defaultdict(list)
 
     for col in pd_in.columns:
         if pd_in[col].dtype == 'object':
             for elem in pd_in[col].unique():
                 cat_dict[col].append(elem)
 
     cat_combi = pd_combination(cat_dict)
     return cat_combi
 
-def pd_num_combi(pd_in,n_sample = 30):
+def num_combi(pd_in,n_sample = 30):
     num_dict = defaultdict(list)
     # n_sample = # of sample to generate
     numeric_cols = pd_in.select_dtypes(include=['number']).columns.tolist()
     num = 30
     for col in numeric_cols:
         min_val = pd_in[col].min()
         max_val = pd_in[col].max()
@@ -1452,17 +1412,17 @@
     # not sure what it does
     """
     Merge two dataframes into all combinations from every row of df1 to every row of df2.
     """
     result = pd.merge(df1.assign(key=1), df2.assign(key=1), on='key').drop('key', axis=1)
     return result
 
-def model_values(xgb_pipeline,X,y_name=""):
-    # In case y_name="" means that X doesn't have the y values already
+# def model_values(xgb_pipeline,X,y_name=""):
+#     # In case y_name="" means that X doesn't have the y values already
     
-    if y_name != "":
-        X_NO_y = X.drop(y_name,axis=1)
-    else:
-        X_NO_y = X
-    test_val = make_testing_val(X_NO_y)
-    model_val = xgb_predict_append(xgb_pipeline, test_val)
-    return model_val
+#     if y_name != "":
+#         X_NO_y = X.drop(y_name,axis=1)
+#     else:
+#         X_NO_y = X
+#     test_val = make_testing_val(X_NO_y)
+#     model_val = xgb_predict_append(xgb_pipeline, test_val)
+#     return model_val
```

