# Comparing `tmp/carbon-registry-indexer-0.1.8.tar.gz` & `tmp/carbon-registry-indexer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon-registry-indexer-0.1.8.tar", last modified: Sat May 11 14:06:36 2024, max compression
+gzip compressed data, was "carbon-registry-indexer-0.1.9.tar", last modified: Tue May 14 07:08:47 2024, max compression
```

## Comparing `carbon-registry-indexer-0.1.8.tar` & `carbon-registry-indexer-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 14:06:36.678787 carbon-registry-indexer-0.1.8/
--rw-rw-rw-   0        0        0     1061 2024-05-11 06:08:04.000000 carbon-registry-indexer-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1400 2024-05-11 14:06:36.678787 carbon-registry-indexer-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      431 2024-05-10 15:34:37.000000 carbon-registry-indexer-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 14:06:36.626787 carbon-registry-indexer-0.1.8/carbon_registry_indexer/
--rw-rw-rw-   0        0        0    16993 2024-05-11 14:04:30.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:06:36.671785 carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/
--rw-rw-rw-   0        0        0      468 2024-05-11 12:47:27.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/__init__.py
--rw-rw-rw-   0        0        0    10128 2024-05-11 14:03:12.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/constants.py
--rw-rw-rw-   0        0        0    16830 2024-05-11 14:03:24.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/sync_acr.py
--rw-rw-rw-   0        0        0     4152 2024-05-11 14:03:31.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/sync_cadt.py
--rw-rw-rw-   0        0        0    18802 2024-05-11 14:03:48.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/sync_car.py
--rw-rw-rw-   0        0        0    11000 2024-05-11 14:04:02.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/sync_gs.py
--rw-rw-rw-   0        0        0    18985 2024-05-11 14:02:31.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:06:36.677786 carbon-registry-indexer-0.1.8/carbon_registry_indexer/models/
--rw-rw-rw-   0        0        0        0 2024-04-03 10:49:14.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/models/__init__.py
--rw-rw-rw-   0        0        0    54117 2024-05-09 16:06:08.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/models/enums.py
--rw-rw-rw-   0        0        0     8079 2024-05-11 14:02:22.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer/models/target.py
-drwxrwxrwx   0        0        0        0 2024-05-11 14:06:36.677786 carbon-registry-indexer-0.1.8/carbon_registry_indexer.egg-info/
--rw-rw-rw-   0        0        0     1400 2024-05-11 14:06:36.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      771 2024-05-11 14:06:36.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 14:06:36.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-11 14:06:36.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-11 14:06:36.000000 carbon-registry-indexer-0.1.8/carbon_registry_indexer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-11 14:06:36.679786 carbon-registry-indexer-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1232 2024-05-11 14:05:48.000000 carbon-registry-indexer-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:08:47.936059 carbon-registry-indexer-0.1.9/
+-rw-rw-rw-   0        0        0     1061 2024-05-11 06:08:04.000000 carbon-registry-indexer-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1400 2024-05-14 07:08:47.936059 carbon-registry-indexer-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-05-10 15:34:37.000000 carbon-registry-indexer-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 07:08:47.893055 carbon-registry-indexer-0.1.9/carbon_registry_indexer/
+-rw-rw-rw-   0        0        0    16993 2024-05-11 14:04:30.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:08:47.926058 carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/
+-rw-rw-rw-   0        0        0      468 2024-05-11 12:47:27.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/__init__.py
+-rw-rw-rw-   0        0        0    10128 2024-05-11 14:03:12.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/constants.py
+-rw-rw-rw-   0        0        0    16830 2024-05-11 14:03:24.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/sync_acr.py
+-rw-rw-rw-   0        0        0     4152 2024-05-11 14:03:31.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/sync_cadt.py
+-rw-rw-rw-   0        0        0    18802 2024-05-11 14:03:48.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/sync_car.py
+-rw-rw-rw-   0        0        0    11000 2024-05-11 14:04:02.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/sync_gs.py
+-rw-rw-rw-   0        0        0    18598 2024-05-14 07:07:25.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:08:47.934057 carbon-registry-indexer-0.1.9/carbon_registry_indexer/models/
+-rw-rw-rw-   0        0        0        0 2024-04-03 10:49:14.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/models/__init__.py
+-rw-rw-rw-   0        0        0    54117 2024-05-09 16:06:08.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/models/enums.py
+-rw-rw-rw-   0        0        0     8079 2024-05-11 14:02:22.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer/models/target.py
+drwxrwxrwx   0        0        0        0 2024-05-14 07:08:47.935058 carbon-registry-indexer-0.1.9/carbon_registry_indexer.egg-info/
+-rw-rw-rw-   0        0        0     1400 2024-05-14 07:08:47.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      771 2024-05-14 07:08:47.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 07:08:47.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-14 07:08:47.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-14 07:08:47.000000 carbon-registry-indexer-0.1.9/carbon_registry_indexer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-14 07:08:47.937058 carbon-registry-indexer-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2024-05-14 07:08:26.000000 carbon-registry-indexer-0.1.9/setup.py
```

### Comparing `carbon-registry-indexer-0.1.8/LICENSE` & `carbon-registry-indexer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/PKG-INFO` & `carbon-registry-indexer-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-registry-indexer
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python library designed to streamline the aggregation of carbon data from multiple registries, each with its own data format, into a unified schema in CSV/Parquet formats.
 Home-page: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer
 Download-URL: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer/archive/refs/tags/v_0.1.7.tar.gz
 Author: Gautam P
 Author-email: gautam@carbonmarketshq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer/__init__.py` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/constants.py` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/constants.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/sync_acr.py` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/sync_acr.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/sync_cadt.py` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/sync_cadt.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/sync_car.py` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/sync_car.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/sync_gs.py` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/sync_gs.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer/integrations/utils.py` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer/integrations/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,37 +58,25 @@
     
     existing_df = existing_df.reindex(columns=combined_columns)
     new_data_df = new_data_df.reindex(columns=combined_columns)
 
     final_df = pd.concat([existing_df, new_data_df], ignore_index=True)
     final_df.to_csv(csv_path, index=False)  
 
-def direct_merge_and_update_csv(data, csv_path):
+def direct_merge_and_update_csv(csv_path, row, pkey):
     """
-    Directly merge and update a CSV file with new data or creates a new file if it does not exist.
-
-    Parameters:
-        data (list of dict): The new data to be added.
-        csv_path (str): The path to the CSV file.
+    Update a single row in a csv file based on the primary key.
     """
-    if isinstance(data, list):
-        new_data_df = pd.DataFrame(data)
-    elif isinstance(data, pd.DataFrame):
-        new_data_df = data
+    if os.path.exists(csv_path):
+        df = pd.read_csv(csv_path)
+        df = df.set_index(pkey)
+        df.update(pd.DataFrame([row]).set_index(pkey))
+        df.reset_index().to_csv(csv_path, index=False)
     else:
-        raise ValueError("Data must be a list of dictionaries or a pandas DataFrame.")
-
-    if not os.path.exists(csv_path):
-        raise FileNotFoundError(f"File {csv_path} does not exist.")
-    
-    existing_df = pd.read_csv(csv_path)
-    final_df = pd.concat([existing_df, new_data_df], ignore_index=True)
-
-    final_df.to_csv(csv_path, index=False)
- 
+        raise FileNotFoundError(f"File {csv_path} not found.")
 
 def camel_to_snake(name):
     """
     Convert a camelCase string to snake_case.
     """
     name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
     return re.sub('([a-z0-9])([A-Z])', r'\1_\2', name).lower()
```

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer/models/enums.py` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer/models/enums.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer/models/target.py` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer/models/target.py`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer.egg-info/PKG-INFO` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-registry-indexer
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python library designed to streamline the aggregation of carbon data from multiple registries, each with its own data format, into a unified schema in CSV/Parquet formats.
 Home-page: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer
 Download-URL: https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer/archive/refs/tags/v_0.1.7.tar.gz
 Author: Gautam P
 Author-email: gautam@carbonmarketshq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `carbon-registry-indexer-0.1.8/carbon_registry_indexer.egg-info/SOURCES.txt` & `carbon-registry-indexer-0.1.9/carbon_registry_indexer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carbon-registry-indexer-0.1.8/setup.py` & `carbon-registry-indexer-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name='carbon-registry-indexer',
-    version='0.1.8',
+    version='0.1.9',
     license='MIT',
     description='A Python library designed to streamline the aggregation of carbon data from multiple registries, each with its own data format, into a unified schema in CSV/Parquet formats.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer', 
     download_url='https://github.com/CarbonMarketsHQ/Carbon-Registry-Indexer/archive/refs/tags/v_0.1.7.tar.gz',
     author='Gautam P',
```

