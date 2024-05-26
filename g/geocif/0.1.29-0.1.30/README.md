# Comparing `tmp/geocif-0.1.29.tar.gz` & `tmp/geocif-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocif-0.1.29.tar", last modified: Tue May 21 22:35:58 2024, max compression
+gzip compressed data, was "geocif-0.1.30.tar", last modified: Sun May 26 14:57:26 2024, max compression
```

## Comparing `geocif-0.1.29.tar` & `geocif-0.1.30.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:58.315176 geocif-0.1.29/
--rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.29/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.29/MANIFEST.in
--rw-rw-rw-   0        0        0     1586 2024-05-21 22:35:58.310177 geocif-0.1.29/PKG-INFO
--rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.29/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:57.912031 geocif-0.1.29/geocif/
--rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.29/geocif/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:58.019451 geocif-0.1.29/geocif/agmet/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.29/geocif/agmet/__init__.py
--rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.29/geocif/agmet/geoagmet.py
--rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.29/geocif/agmet/plot.py
--rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.29/geocif/agmet/utils.py
--rw-rw-rw-   0        0        0    34486 2024-05-16 01:28:20.000000 geocif-0.1.29/geocif/analysis.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:58.089911 geocif-0.1.29/geocif/backup/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.29/geocif/backup/__init__.py
--rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.29/geocif/backup/constants.py
--rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.29/geocif/backup/features.py
--rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.29/geocif/backup/geo.py
--rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.29/geocif/backup/geocif.py
--rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.29/geocif/backup/metadata.py
--rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.29/geocif/backup/models.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:58.121522 geocif-0.1.29/geocif/cei/
--rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.29/geocif/cei/__init__.py
--rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.29/geocif/cei/definitions.py
--rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.29/geocif/cei/indices.py
--rw-rw-rw-   0        0        0    42243 2024-05-17 16:05:26.000000 geocif-0.1.29/geocif/geocif.py
--rw-rw-rw-   0        0        0     6660 2024-05-21 22:35:07.000000 geocif-0.1.29/geocif/indices_runner.py
--rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.29/geocif/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:58.248027 geocif-0.1.29/geocif/ml/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.29/geocif/ml/__init__.py
--rw-rw-rw-   0        0        0    12360 2024-05-14 02:40:35.000000 geocif-0.1.29/geocif/ml/correlations.py
--rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.29/geocif/ml/embedding.py
--rw-rw-rw-   0        0        0    12671 2024-05-12 03:53:54.000000 geocif-0.1.29/geocif/ml/feature_engineering.py
--rw-rw-rw-   0        0        0     8953 2024-05-15 14:01:01.000000 geocif-0.1.29/geocif/ml/feature_selection.py
--rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.29/geocif/ml/outliers.py
--rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.29/geocif/ml/outlook.py
--rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.29/geocif/ml/output.py
--rw-rw-rw-   0        0        0     8286 2024-05-12 14:57:40.000000 geocif-0.1.29/geocif/ml/stages.py
--rw-rw-rw-   0        0        0     8393 2024-05-13 20:11:22.000000 geocif-0.1.29/geocif/ml/stats.py
--rw-rw-rw-   0        0        0     9433 2024-05-16 16:45:11.000000 geocif-0.1.29/geocif/ml/trainers.py
--rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.29/geocif/ml/trend.py
--rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.29/geocif/ml/xai.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:58.272734 geocif-0.1.29/geocif/playground/
--rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.29/geocif/playground/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.29/geocif/playground/automl.py
--rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.29/geocif/playground/misc.py
--rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.29/geocif/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:58.289745 geocif-0.1.29/geocif/viz/
--rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.29/geocif/viz/__init__.py
--rw-rw-rw-   0        0        0    15867 2024-05-15 21:02:40.000000 geocif-0.1.29/geocif/viz/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:57.987586 geocif-0.1.29/geocif.egg-info/
--rw-rw-rw-   0        0        0     1586 2024-05-21 22:35:54.000000 geocif-0.1.29/geocif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1107 2024-05-21 22:35:56.000000 geocif-0.1.29/geocif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 22:35:54.000000 geocif-0.1.29/geocif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.29/geocif.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-05-21 22:35:54.000000 geocif-0.1.29/geocif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.29/requirements.txt
--rw-rw-rw-   0        0        0      415 2024-05-21 22:35:58.337878 geocif-0.1.29/setup.cfg
--rw-rw-rw-   0        0        0     1617 2024-05-21 22:35:30.000000 geocif-0.1.29/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:35:58.300610 geocif-0.1.29/tests/
--rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.29/tests/test_geocif.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.872530 geocif-0.1.30/
+-rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.30/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.30/MANIFEST.in
+-rw-rw-rw-   0        0        0     1586 2024-05-26 14:57:26.866878 geocif-0.1.30/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.30/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.407786 geocif-0.1.30/geocif/
+-rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.30/geocif/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.549939 geocif-0.1.30/geocif/agmet/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.30/geocif/agmet/__init__.py
+-rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.30/geocif/agmet/geoagmet.py
+-rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.30/geocif/agmet/plot.py
+-rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.30/geocif/agmet/utils.py
+-rw-rw-rw-   0        0        0    34486 2024-05-16 01:28:20.000000 geocif-0.1.30/geocif/analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.627091 geocif-0.1.30/geocif/backup/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.30/geocif/backup/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.30/geocif/backup/constants.py
+-rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.30/geocif/backup/features.py
+-rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.30/geocif/backup/geo.py
+-rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.30/geocif/backup/geocif.py
+-rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.30/geocif/backup/metadata.py
+-rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.30/geocif/backup/models.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.654883 geocif-0.1.30/geocif/cei/
+-rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.30/geocif/cei/__init__.py
+-rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.30/geocif/cei/definitions.py
+-rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.30/geocif/cei/indices.py
+-rw-rw-rw-   0        0        0    42711 2024-05-26 14:55:15.000000 geocif-0.1.30/geocif/geocif.py
+-rw-rw-rw-   0        0        0     6660 2024-05-25 01:23:08.000000 geocif-0.1.30/geocif/indices_runner.py
+-rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.30/geocif/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.791637 geocif-0.1.30/geocif/ml/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.30/geocif/ml/__init__.py
+-rw-rw-rw-   0        0        0    12623 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/correlations.py
+-rw-rw-rw-   0        0        0     5098 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/embedding.py
+-rw-rw-rw-   0        0        0    13882 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/feature_engineering.py
+-rw-rw-rw-   0        0        0     9120 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/feature_selection.py
+-rw-rw-rw-   0        0        0    10035 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/outliers.py
+-rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.30/geocif/ml/outlook.py
+-rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.30/geocif/ml/output.py
+-rw-rw-rw-   0        0        0     5139 2024-05-26 02:21:56.000000 geocif-0.1.30/geocif/ml/spatial_autocorrelation.py
+-rw-rw-rw-   0        0        0     8348 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/stages.py
+-rw-rw-rw-   0        0        0     9038 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/stats.py
+-rw-rw-rw-   0        0        0     9515 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/trainers.py
+-rw-rw-rw-   0        0        0     3171 2024-05-25 18:55:01.000000 geocif-0.1.30/geocif/ml/trend.py
+-rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.30/geocif/ml/xai.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.816876 geocif-0.1.30/geocif/playground/
+-rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.30/geocif/playground/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.30/geocif/playground/automl.py
+-rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.30/geocif/playground/misc.py
+-rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.30/geocif/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.840642 geocif-0.1.30/geocif/viz/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.30/geocif/viz/__init__.py
+-rw-rw-rw-   0        0        0    15867 2024-05-15 21:02:40.000000 geocif-0.1.30/geocif/viz/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.521676 geocif-0.1.30/geocif.egg-info/
+-rw-rw-rw-   0        0        0     1586 2024-05-26 14:57:24.000000 geocif-0.1.30/geocif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2024-05-26 14:57:25.000000 geocif-0.1.30/geocif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:57:24.000000 geocif-0.1.30/geocif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.30/geocif.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-05-26 14:57:24.000000 geocif-0.1.30/geocif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.30/requirements.txt
+-rw-rw-rw-   0        0        0      415 2024-05-26 14:57:26.902391 geocif-0.1.30/setup.cfg
+-rw-rw-rw-   0        0        0     1617 2024-05-26 14:57:15.000000 geocif-0.1.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:26.855306 geocif-0.1.30/tests/
+-rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.30/tests/test_geocif.py
```

### Comparing `geocif-0.1.29/LICENSE` & `geocif-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/PKG-INFO` & `geocif-0.1.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.29
+Version: 0.1.30
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.29/README.md` & `geocif-0.1.30/README.md`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/agmet/geoagmet.py` & `geocif-0.1.30/geocif/agmet/geoagmet.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/agmet/plot.py` & `geocif-0.1.30/geocif/agmet/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/agmet/utils.py` & `geocif-0.1.30/geocif/agmet/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/analysis.py` & `geocif-0.1.30/geocif/analysis.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/backup/features.py` & `geocif-0.1.30/geocif/backup/features.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/backup/geo.py` & `geocif-0.1.30/geocif/backup/geo.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/backup/geocif.py` & `geocif-0.1.30/geocif/backup/geocif.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/backup/metadata.py` & `geocif-0.1.30/geocif/backup/metadata.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/cei/definitions.py` & `geocif-0.1.30/geocif/cei/definitions.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/cei/indices.py` & `geocif-0.1.30/geocif/cei/indices.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/geocif.py` & `geocif-0.1.30/geocif/geocif.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import pandas as pd
 import sklearn
 from tqdm import tqdm
 
 from geocif import logger as log
 from .cei import definitions as di
 from .ml import correlations
+from .ml import spatial_autocorrelation as sa
 from .ml import feature_engineering as fe
 from .ml import feature_selection as fs
 from .ml import output
 from .ml import stages
 from .ml import stats
 from .ml import trainers
 from .ml import trend
@@ -108,14 +109,18 @@
         ====================================================================
         """
         self.model_type = self.parser.get("ML", "model_type")
         self.fraction_simulate = self.parser.getint("ML", "fraction_simulate")
         self.analogous_year_yield_as_feature = self.parser.getboolean(
             "ML", "analogous_year_yield_as_feature"
         )
+        self.spatial_autocorrelation = self.parser.getboolean(
+            "ML", "spatial_autocorrelation"
+        )
+        self.sa_method = self.parser.get("ML", "sa_method")
         self.last_year_yield_as_feature = self.parser.getboolean(
             "ML", "last_year_yield_as_feature"
         )
         self.panel_model = self.parser.getboolean("ML", "panel_model")
         self.panel_model_region = self.parser.get("ML", "panel_model_region")
         self.use_outlook_as_feature = self.parser.getboolean(
             "ML", "use_outlook_as_feature"
@@ -363,18 +368,18 @@
                 "Best Hyperparameters": np.full(shp, best_hyperparameters),
                 "Stage_ID": np.full(shp, self.stage_info["Stage_ID"]),
                 "Stage Range": np.full(shp, self.stage_info["Stage Range"]),
                 "Stage Name": np.full(shp, self.stage_info["Stage Name"]),
                 "Starting Stage": np.full(shp, self.stage_info["Starting Stage"]),
                 "Ending Stage": np.full(shp, self.stage_info["Ending Stage"]),
                 "Model": np.full(shp, self.model_name),
-                "Area (ha)": df_region["Area (ha)"].values,
                 "Region_ID": df_region["Region_ID"].values,
                 "Region": df_region["Region"].values,
                 "Harvest Year": df_region["Harvest Year"].values,
+                "Area (ha)": df_region["Area (ha)"].values,
                 f"Observed {self.target}": np.around(y_test, 3).ravel(),
                 f"Predicted {self.target}": np.around(y_pred, 3).ravel(),
             }
         )
 
         if self.median_yield_as_feature:
             # Add median yield to dataframe
@@ -408,28 +413,34 @@
                 df.loc[:, "Analogous Year"] = df_region["Analogous Year"].values
                 df.loc[:, "Analogous Year Yield"] = np.around(
                     df_region["Analogous Year Yield"].values, 3
                 )
             except:
                 breakpoint()
 
+        # if self.spatial_autocorrelation:
+        #     # Compute spatial autocorrelation
+        #     df = sa.compute_spatial_autocorrelation(
+        #         self.dg_country
+        #     )
+
         for col in [
             f"Median {self.target}",
             "Analogous Year",
             "Analogous Year Yield",
             "Detrended Model Type",
             "Detrended Model",
         ]:
             if col not in df.columns:
                 df.loc[:, col] = np.NaN
 
         # Create an index based on following columns
         index_columns = [
             "Model",
-            "Cluster Strategy"
+            "Cluster Strategy",
             "Country",
             "Region",
             "Crop",
             "Harvest Year",
             "Stage Name",
         ]
         df.index = df.apply(
@@ -714,15 +725,14 @@
         os.makedirs(dir_output, exist_ok=True)
         df.to_csv(
             dir_output / f"{self.country}_{self.crop}_{self.forecast_season}.csv",
             index=False,
         )
 
         # cat_features should be converted to category type
-
         df[self.cat_features] = df[self.cat_features].astype("category")
 
         """  Heatmap of correlation of various features with yield at each time step"""
         # For each time step, determine the number of occurences of each feature
         # when it is most correlated with the target for a region
         # Use this to plot a heatmap showing which features are most correlated
         # with yield at each time step
@@ -735,40 +745,43 @@
         # Only use geometry column from self.dg
         self.dg_country = self.dg_country[["Country Region", "geometry"]].merge(
             df[["Country Region", self.correlation_plot_groupby]],
             on="Country Region",
             how="outer",
         )
 
-        if self.correlation_plots:
-            dict_kwargs = {}
-            dict_kwargs["all_stages"] = self.all_stages
-            dict_kwargs["target_col"] = self.target
-            dict_kwargs["country"] = self.country
-            dict_kwargs["crop"] = self.crop
-            dict_kwargs["dir_output"] = (
-                self.dir_analysis
-                / self.country
-                / self.crop
-                / self.model_name
-                / str(self.forecast_season)
-            )
-            dict_kwargs["forecast_season"] = self.forecast_season
-            dict_kwargs["method"] = self.method
-            dict_kwargs["national_correlation"] = self.national_correlation
-            dict_kwargs["groupby"] = self.correlation_plot_groupby
-            dict_kwargs["dg_country"] = self.dg_country
-            dict_kwargs["combined_dict"] = self.combined_dict
+        dict_kwargs = {}
+        dict_kwargs["all_stages"] = self.all_stages
+        dict_kwargs["target_col"] = self.target
+        dict_kwargs["country"] = self.country
+        dict_kwargs["crop"] = self.crop
+        dict_kwargs["dir_output"] = (
+            self.dir_analysis
+            / self.country
+            / self.crop
+            / self.model_name
+            / str(self.forecast_season)
+        )
+        dict_kwargs["forecast_season"] = self.forecast_season
+        dict_kwargs["method"] = self.method
+        dict_kwargs["national_correlation"] = self.national_correlation
+        dict_kwargs["groupby"] = self.correlation_plot_groupby
+        dict_kwargs["dg_country"] = self.dg_country
+        dict_kwargs["combined_dict"] = self.combined_dict
 
+        if self.correlation_plots:
             self.logger.info(f"Correlation plot for {self.country} {self.crop}")
             (
                 dict_selected_features,
                 dict_best_cei,
             ) = correlations.all_correlated_feature_by_time(df, **dict_kwargs)
 
+        if self.spatial_autocorrelation:
+           sa.compute_spatial_autocorrelation(self.df_results, **dict_kwargs)
+
         """ Separate into train and test datasets based on forecast_season """
         mask = df["Harvest Year"] == self.forecast_season
         self.df_train = df[~mask]
         self.df_test = df[mask]
 
         # Drop rows with missing values for self.target_col in df_train
         self.df_train = self.df_train.dropna(subset=[self.target])
```

### Comparing `geocif-0.1.29/geocif/indices_runner.py` & `geocif-0.1.30/geocif/indices_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                 filename,
                 admin_zone,
                 category,
                 year,
                 "ndvi",
                 False,  # redo
             )
-            for year in range(2023, ar.utcnow().year + 1)
+            for year in range(2001, ar.utcnow().year + 1)
             for status, path, filename, admin_zone, category in combinations
         ]
 
         # Only keep those entries in combinations where the third elemt is
         # mozambique, south_africa, angola or dem_people's_rep_of_korea
         # This is done to test the code for these countries
         combinations = [i for i in combinations if "angola_maize" in i[3] or
```

### Comparing `geocif-0.1.29/geocif/logger.py` & `geocif-0.1.30/geocif/logger.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/ml/correlations.py` & `geocif-0.1.30/geocif/ml/correlations.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,28 +24,32 @@
     """
     frames = []
 
     stages = [simulation_stages[: idx + 1] for idx in range(len(simulation_stages))]
 
     # Only select columns that have been observed till the current stage
     for stage in tqdm(stages, leave=False, desc="Compute most correlated feature"):
-        current_feature_set = [col for col in df_train.columns if col.endswith(f"_{stage[-1]}")]
+        current_feature_set = [
+            col for col in df_train.columns if col.endswith(f"_{stage[-1]}")
+        ]
 
         # Get the most correlated feature for each region
         top_feature_by_region, counter = embedding.get_top_correlated_features(
             df_train[current_feature_set + ["Region"]],
             df_train[target_col],
         )
 
         # Create a dataframe with the most common top feature and number of occurrences over timestep
         _feature = counter.most_common(1)[0][0]
         # Loop through top_feature_by_region and find the average score for _feature
         # Calculate the average score for 'DTR_36'
         _feature_scores = [
-            value[1][0] for key, value in top_feature_by_region.items() if _feature in value[0]
+            value[1][0]
+            for key, value in top_feature_by_region.items()
+            if _feature in value[0]
         ]
         average_score = sum(_feature_scores) / len(_feature_scores)
         _feature = utils.remove_last_part(_feature)
 
         df = pd.DataFrame(
             {
                 "Stage": [stage[-1]],
@@ -133,15 +137,17 @@
     ax_map.spines["left"].set_visible(False)
     # ax4 should not be visible
     ax4.axis("off")
 
     # Add colorbar label
     # cbar_ax.set_xlabel("Correlation Coefficient", labelpad=3, size="small")
     cbar_ax.set_title("Correlation Coefficient", loc="left", size="small")
-    ax_heatmap.set_xticklabels(ax_heatmap.get_xticklabels(), size="x-small", rotation=0, fontsize=5)
+    ax_heatmap.set_xticklabels(
+        ax_heatmap.get_xticklabels(), size="x-small", rotation=0, fontsize=5
+    )
     ax_heatmap.set_yticklabels(ax_heatmap.get_yticklabels(), size="x-small", fontsize=5)
     ax_heatmap.set_xlabel("")
     ax_heatmap.set_ylabel(" ")
     # Reduce font size of ticks of colorbar
     cbar_ax.tick_params(axis="both", which="major", labelsize=5)
 
     _country = country.title().replace("_", " ")
@@ -186,15 +192,17 @@
 
     # Only select columns that have been observed till the current stage
     pbar = tqdm(stages_features, total=len(stages_features), leave=False)
     for stage in pbar:
         pbar.set_description(f"Calculating correlations")
         pbar.update()
 
-        stage_name = stages.get_stage_information_dict(f"GD4_{stage}", method)["Stage Name"]
+        stage_name = stages.get_stage_information_dict(f"GD4_{stage}", method)[
+            "Stage Name"
+        ]
         # starting_stage = stage_name.split("-")[0]
         current_feature_set = [col for col in df.columns if stage_name in col]
 
         # Get the most correlated feature for each region
         df_tmp = embedding.get_all_features_correlation(
             df[current_feature_set + ["Region"]], df[target_col], method
         )
@@ -206,15 +214,17 @@
         # Exclude Region column
         df_results = df_results.drop(columns="Region")
         # Groupby Dekad and compute mean of all columns apart from Region
         df_results = df_results.groupby(method).mean()
 
         all_stage_names = []
         for stage in stages_features:
-            _tmp = stages.get_stage_information_dict(f"GD4_{stage}", method)["Stage Name"]
+            _tmp = stages.get_stage_information_dict(f"GD4_{stage}", method)[
+                "Stage Name"
+            ]
             all_stage_names.append(_tmp)
 
         df_results = df_results.reindex(all_stage_names)
 
         # Drop rows with all NaN values
         df_results = df_results.dropna(how="all")
 
@@ -250,15 +260,20 @@
         ):
             df_corr = _all_correlated_feature_by_time(group, **kwargs)
 
             if not df_corr.empty:
                 df_tmp = df_corr[df_corr.columns[(df_corr.mean() > 0.1)]]
                 dict_selected_features[region_id] = df_tmp.columns
 
-                df_tmp2 = df_tmp.median(axis=0).abs().sort_values(ascending=False).reset_index()
+                df_tmp2 = (
+                    df_tmp.median(axis=0)
+                    .abs()
+                    .sort_values(ascending=False)
+                    .reset_index()
+                )
                 df_tmp2.columns = ["Metric", "Value"]
                 # Add another column based on Type of Metric
                 for idx, row in df_tmp2.iterrows():
                     df_tmp2.loc[idx, "Type"] = combined_dict[row[0]][0]
 
                 # Compute median of each CEI and sort the dataframe based on the absolute value of the median
                 dict_best_cei[region_id] = (
@@ -274,16 +289,16 @@
                 # For each element in dict_best_cei, add the type of the cei
             else:
                 # HACK
                 df_corr = _all_correlated_feature_by_time(df, **kwargs)
                 dict_selected_features[region_id] = df_corr.columns
                 dict_best_cei[region_id] = {}
 
-                #dict_selected_features[region_id] = dict_selected_features[0]
-                #dict_best_cei[region_id] = dict_best_cei[0]
+                # dict_selected_features[region_id] = dict_selected_features[0]
+                # dict_best_cei[region_id] = dict_best_cei[0]
                 # Combine all unique values from the existing dictionary elements
                 # combined_metrics = set()
                 # for key in dict_selected_features:
                 #     breakpoint()
                 #     combined_metrics.update(dict_selected_features[key])
                 #
                 # # Add the combined set as a new element with key 3
@@ -306,29 +321,33 @@
     df_train = kwargs.get("df_train")
     target_col = kwargs.get("target_col")
 
     stages = [simulation_stages[: idx + 1] for idx in range(len(simulation_stages))]
 
     # Only select columns that have been observed till the current stage
     for stage in tqdm(stages, leave=False, desc="Compute feature correlation by time"):
-        current_feature_set = [col for col in df_train.columns if col.endswith(f"_{stage[-1]}")]
+        current_feature_set = [
+            col for col in df_train.columns if col.endswith(f"_{stage[-1]}")
+        ]
 
         # Get the most correlated feature for each region
         top_feature_by_region, counter = embedding.compute_feature_correlations(
             df_train[current_feature_set + ["Region"]],
             df_train[target_col],
             "all",
         )
 
         # Create a dataframe with the most common top feature and number of occurrences over timestep
         _feature = counter.most_common(1)[0][0]
         # Loop through top_feature_by_region and find the average score for _feature
         # Calculate the average score for 'DTR_36'
         _feature_scores = [
-            value[1][0] for key, value in top_feature_by_region.items() if _feature in value[0]
+            value[1][0]
+            for key, value in top_feature_by_region.items()
+            if _feature in value[0]
         ]
         average_score = sum(_feature_scores) / len(_feature_scores)
         _feature = utils.remove_last_part(_feature)
 
         df = pd.DataFrame(
             {
                 "Stage": [stage[-1]],
```

### Comparing `geocif-0.1.29/geocif/ml/embedding.py` & `geocif-0.1.30/geocif/ml/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,17 @@
 
     for region_id in inputs["Region"].unique():
         X, y = extract_regions(inputs, targets, regions=[region_id])
 
         feature_correlations = _compute_correlations(X, y)
 
         # Exclude any nan values
-        feature_correlations = {k: v for k, v in feature_correlations.items() if not np.isnan(v)}
+        feature_correlations = {
+            k: v for k, v in feature_correlations.items() if not np.isnan(v)
+        }
 
         if not feature_correlations:
             continue
 
         # Sorts the items of feature_correlations, a dictionary mapping features to their
         # correlation values, by the absolute value of the correlation in descending order,
         # resulting in a list of tuples with the feature and its corresponding correlation value
@@ -109,15 +111,17 @@
     frames = []
     for region_id in inputs["Region"].unique():
         X, y = extract_regions(inputs, targets, regions=[region_id])
 
         feature_correlations = _compute_correlations(X, y)
 
         # Exclude any nan values
-        feature_correlations = {k: v for k, v in feature_correlations.items() if not np.isnan(v)}
+        feature_correlations = {
+            k: v for k, v in feature_correlations.items() if not np.isnan(v)
+        }
 
         if not feature_correlations:
             continue
 
         split_keys = []
         for key in feature_correlations.keys():
             parts = key.split(" ")
```

### Comparing `geocif-0.1.29/geocif/ml/feature_engineering.py` & `geocif-0.1.30/geocif/ml/feature_engineering.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,19 +17,23 @@
         DataFrame: The original DataFrame enhanced with a new column for the previous year yield.
     """
     # Ensure 'Harvest Year' is treated as integer for accurate comparisons
     df["Harvest Year"] = df["Harvest Year"].astype(int)
     # Initialize the new column with NaNs
     df[f"Last Year {target_col}"] = np.nan
 
-    for region, group in tqdm(df.groupby("Region"), desc="Last year yields", leave=False):
+    for region, group in tqdm(
+        df.groupby("Region"), desc="Last year yields", leave=False
+    ):
         unique_years = group["Harvest Year"].unique()
 
         for harvest_year in unique_years:
-            mask = (group["Harvest Year"] == harvest_year - 1) & (group["Region"] == region)
+            mask = (group["Harvest Year"] == harvest_year - 1) & (
+                group["Region"] == region
+            )
             last_year_yield = group.loc[mask, target_col].values
             if last_year_yield:
                 df.loc[
                     (df["Region"] == region) & (df["Harvest Year"] == harvest_year),
                     f"Last Year {target_col}",
                 ] = last_year_yield[0]
 
@@ -85,25 +89,29 @@
         if group[target_col].isnull().all():
             continue
 
         for harvest_year in unique_years:
             closest_years = compute_closest_years(
                 all_seasons_with_yield, harvest_year, number_median_years
             )
-            mask = (group["Harvest Year"].isin(closest_years)) & (group["Region"] == region)
+            mask = (group["Harvest Year"].isin(closest_years)) & (
+                group["Region"] == region
+            )
             median_yield = group.loc[mask, target_col].median()
             df.loc[
                 (df["Region"] == region) & (df["Harvest Year"] == harvest_year),
                 f"Median {target_col}",
             ] = median_yield
 
     return df
 
 
-def compute_lag_yield(df, all_seasons_with_yield, number_lag_years, target_col="Yield (tn per ha)"):
+def compute_lag_yield(
+    df, all_seasons_with_yield, number_lag_years, target_col="Yield (tn per ha)"
+):
     # For the number of years specified in self.number_lag_years, add the yield of that number of years
     # ago to the dataframe
     # For example, if number_lag_years is 3, then the yield of each year upto 3 years ago will be added
     # to the dataframe
     # The yield of the previous year is already added to the dataframe
     # Ensure 'Harvest Year' is treated as integer for accurate comparisons
     df["Harvest Year"] = df["Harvest Year"].astype(int)
@@ -121,15 +129,17 @@
             )
 
             # For each year in the closest years, add the yield to the dataframe as a new column
             for idx, year in enumerate(closest_years):
                 col = f"t -{idx + 1} {target_col}"
 
                 mask_group_year = group["Harvest Year"] == year
-                mask_region = (df["Region"] == region) & (df["Harvest Year"] == harvest_year)
+                mask_region = (df["Region"] == region) & (
+                    df["Harvest Year"] == harvest_year
+                )
                 yield_value = group.loc[mask_group_year, target_col].values
 
                 if yield_value.size > 0:
                     df.loc[mask_region, col] = yield_value[0]
                 else:
                     # Add median yield
                     mask_group_median = group["Harvest Year"].isin(closest_years)
@@ -177,19 +187,23 @@
     # Initialize the new columns to NaN
     df["Analogous Year"] = np.nan
     df["Analogous Year Yield"] = np.nan
 
     all_years = df["Harvest Year"].unique()
 
     for harvest_year in tqdm(all_years, desc="Computing analogous yields", leave=False):
-        lag_years = compute_closest_years(all_seasons_with_yield, harvest_year, number_lag_years)
+        lag_years = compute_closest_years(
+            all_seasons_with_yield, harvest_year, number_lag_years
+        )
 
         for region in df["Region"].unique():
             # Filter current year and region dataset
-            df_current = df[(df["Harvest Year"] == harvest_year) & (df["Region"] == region)]
+            df_current = df[
+                (df["Harvest Year"] == harvest_year) & (df["Region"] == region)
+            ]
             # Filter dataset for lag years and the same region
             df_lag = df[(df["Harvest Year"].isin(lag_years)) & (df["Region"] == region)]
 
             if df_current.empty or df_lag.empty:
                 continue  # Skip if no data available for comparison
 
             # Calculate RMSE between the current year's profile and each of the lag years' profiles
@@ -238,14 +252,15 @@
     Returns:
 
     """
     os.environ["OMP_NUM_THREADS"] = "1"
 
     # Suppress warnings in this function
     import warnings
+
     warnings.filterwarnings("ignore")
 
     from kneed import KneeLocator
     from sklearn.cluster import KMeans
 
     # Get the yield of each region in df_results
     df_yield = df[["Region", "Harvest Year", target_col]]
@@ -287,40 +302,81 @@
         try:
             kmeans.fit(df_yield_pivot)
         except:
             breakpoint()
         inertia.append(kmeans.inertia_)
 
     # Use KneeLocator to find the elbow point automatically
-    knee_locator = KneeLocator(range_of_clusters, inertia, curve="convex", direction="decreasing")
+    knee_locator = KneeLocator(
+        range_of_clusters, inertia, curve="convex", direction="decreasing"
+    )
 
     # # Plot the Elbow Method for visual confirmation
     # plt.figure(figsize=(10, 6))
     # plt.plot(range_of_clusters, inertia, marker='o', linestyle='--')
     # plt.title('Elbow Method For Optimal k')
     # plt.xlabel('Number of clusters')
     # plt.ylabel('Inertia')
     # plt.xticks(range_of_clusters)
     # plt.vlines(knee_locator.knee, plt.ylim()[0], plt.ylim()[1], linestyles='dashed')
     # plt.show()
 
     # Use the detected number of clusters
     optimal_clusters = knee_locator.knee
     if optimal_clusters:
-        optimal_clusters = optimal_clusters + 1 if optimal_clusters > 1 else optimal_clusters
+        optimal_clusters = (
+            optimal_clusters + 1 if optimal_clusters > 1 else optimal_clusters
+        )
 
         # Apply K-Means clustering with the detected optimal number of clusters
         kmeans = KMeans(n_clusters=optimal_clusters, random_state=42)
         kmeans.fit(df_yield_pivot)
 
         # Assign cluster labels to each region
         cluster_labels = kmeans.labels_
 
         # Create a DataFrame with region names and their respective cluster IDs
         clusters_assigned = pd.DataFrame(
             {"Region": df_yield_pivot.index, "Region_ID": cluster_labels}
         )
     else:
         # If no optimal_clusters is found, then assign all regions to a single cluster
-        clusters_assigned = pd.DataFrame({"Region": df_yield_pivot.index, "Region_ID": 1})
+        clusters_assigned = pd.DataFrame(
+            {"Region": df_yield_pivot.index, "Region_ID": 1}
+        )
 
     return clusters_assigned
+
+
+# breakpoint()
+
+# from libpysal.weights import Queen, Rook
+# from pysal.lib import weights
+# from scipy.linalg import eigh
+#
+# breakpoint()
+# df = pd.DataFrame()
+#
+# # Create a spatial weights matrix (e.g., Queen contiguity)
+# w = weights.Queen.from_dataframe(dg)
+#
+# # Transform weights to row-standardized form
+# w.transform = 'r'
+#
+# # Convert the weights matrix to a dense format for eigen decomposition
+# W_dense = w.full()[0]
+#
+# # Compute eigenvalues and eigenvectors
+# eigenvalues, eigenvectors = eigh(W_dense)
+#
+# # Sort eigenvalues and corresponding eigenvectors
+# sorted_indices = np.argsort(eigenvalues)[::-1]
+# eigenvalues = eigenvalues[sorted_indices]
+# eigenvectors = eigenvectors[:, sorted_indices]
+#
+# # Select a subset of eigenvectors (e.g., first 10)
+# selected_eigenvectors = eigenvectors[:, :2]
+#
+# breakpoint()
+# # Add eigenvectors to the GeoDataFrame
+# for i in range(selected_eigenvectors.shape[1]):
+#     df[f'EV_{i + 1}'] = selected_eigenvectors[:, i]
```

### Comparing `geocif-0.1.29/geocif/ml/feature_selection.py` & `geocif-0.1.30/geocif/ml/feature_selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,38 +73,46 @@
         model.fit(X, y)
 
         explainer = FastTreeExplainer(model)
         shap_values = explainer.shap_values(X)
 
         # Step 5: Summarize the SHAP values for feature importance
         shap_importances = np.mean(np.abs(shap_values), axis=0)
-        shap_importance_df = pd.DataFrame({
-            'feature': X.columns,
-            'importance': shap_importances
-        }).sort_values(by='importance', ascending=False)
+        shap_importance_df = pd.DataFrame(
+            {"feature": X.columns, "importance": shap_importances}
+        ).sort_values(by="importance", ascending=False)
 
         def evaluate_model_with_n_features(N, X_train, y_train):
-            top_features = shap_importance_df['feature'].head(N).values
+            top_features = shap_importance_df["feature"].head(N).values
             X_train_selected = X_train[top_features]
             selector = CatBoostRegressor(n_estimators=500, random_state=42, verbose=0)
-            scores = cross_val_score(selector, X_train_selected, y_train, cv=5, scoring='neg_mean_squared_error', n_jobs=-1)
+            scores = cross_val_score(
+                selector,
+                X_train_selected,
+                y_train,
+                cv=5,
+                scoring="neg_mean_squared_error",
+                n_jobs=-1,
+            )
 
             return np.mean(scores)
 
         # Evaluate model performance with different number of features
         nrange = [5, 10, 15, 20, 25, 30]
         cv_scores = []
         for N in tqdm(nrange):
             cv_scores.append(evaluate_model_with_n_features(N, X, y))
 
         # Select the number of features that gives the best cross-validation score (lowest MSE)
         optimal_N = nrange[np.argmax(cv_scores)]
 
         # Use optimal N to select features
-        selected_features = shap_importance_df['feature'].head(optimal_N).values.tolist()
+        selected_features = (
+            shap_importance_df["feature"].head(optimal_N).values.tolist()
+        )
     elif method == "feature_engine":
         from feature_engine.selection import SmartCorrelatedSelection
 
         selector = SmartCorrelatedSelection(
             method="pearson",
             threshold=0.7,
             selection_method="model_performance",
@@ -198,15 +206,17 @@
             "loss_function": "RMSE",
             "early_stopping_rounds": 25,
             "random_seed": 42,
             "verbose": False,
         }
         model = CatBoostRegressor(**hyperparams)
 
-        selector = BorutaShap(model=model, importance_measure="shap", classification=False)
+        selector = BorutaShap(
+            model=model, importance_measure="shap", classification=False
+        )
         selector.fit(
             X=X,
             y=y,
             n_trials=100,
             sample=False,
             train_or_test="test",
             normalize=True,
@@ -233,15 +243,17 @@
         )
         selector.fit(X, y)
         selected_features_mask = selector.support_
         selected_features = X.columns[selected_features_mask].tolist()
     elif method == "RFE":
         from sklearn.feature_selection import RFE
 
-        selector = RFE(forest, n_features_to_select=min_features_to_select, step=1, verbose=1)
+        selector = RFE(
+            forest, n_features_to_select=min_features_to_select, step=1, verbose=1
+        )
         selector = selector.fit(X, y)
         selected_features_mask = selector.support_
         selected_features = X.columns[selected_features_mask].tolist()
     else:
         raise ValueError("Method not recognized. Use BorutaPy, Genetic, or RFE")
     # tentative_features = X.columns[selector.support_weak_].tolist()
```

### Comparing `geocif-0.1.29/geocif/ml/outliers.py` & `geocif-0.1.30/geocif/ml/outliers.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,27 +90,31 @@
 
     for crop in crops:
         os.makedirs(BASE_DIR / crop, exist_ok=True)
         df_fewsnet_sub = df_fewsnet[df_fewsnet["product"] == crop]
 
         if not os.path.isfile(BASE_DIR / crop / f"adm_crop_production_z_{crop}.csv"):
             # In rows where admin_2 != "none", replace admin_1 with admin_2
-            df_fewsnet_sub.loc[df_fewsnet_sub["admin_2"] != "none", "admin_1"] = df_fewsnet_sub[
-                "admin_2"
-            ]
+            df_fewsnet_sub.loc[
+                df_fewsnet_sub["admin_2"] != "none", "admin_1"
+            ] = df_fewsnet_sub["admin_2"]
 
             df_output = find_outlier(df_fewsnet_sub)
 
-            df_output.to_csv(BASE_DIR / crop / f"adm_crop_production_z_{crop}.csv", index=False)
+            df_output.to_csv(
+                BASE_DIR / crop / f"adm_crop_production_z_{crop}.csv", index=False
+            )
         else:
-            df_output = pd.read_csv(BASE_DIR / crop / f"adm_crop_production_z_{crop}.csv")
+            df_output = pd.read_csv(
+                BASE_DIR / crop / f"adm_crop_production_z_{crop}.csv"
+            )
 
-        df_fewsnet_sub.loc[df_fewsnet_sub["admin_2"] != "none", "admin_1"] = df_fewsnet_sub[
-            "admin_2"
-        ]
+        df_fewsnet_sub.loc[
+            df_fewsnet_sub["admin_2"] != "none", "admin_1"
+        ] = df_fewsnet_sub["admin_2"]
 
         # Create a column called Z-Score Category based on the value of the z-score
         # The categories are:
         # < -2 : Extremely Low
         # -2 to -1: Very Low
         # -1 to 0: Low
         # 0 to 1: Average
@@ -138,15 +142,17 @@
                 & (df_fewsnet_sub["season_name"] == season_name)
                 & (df_fewsnet_sub["crop_production_system"] == crop_production_system)
             )
             # convert harvest_year column in df_fewsnet to int
             df_fewsnet_sub["harvest_year"] = df_fewsnet_sub["harvest_year"].astype(int)
 
             df_yield = df_fewsnet_sub[mask & (df_fewsnet_sub["indicator"] == "yield")]
-            df_production = df_fewsnet_sub[mask & (df_fewsnet_sub["indicator"] == "production")]
+            df_production = df_fewsnet_sub[
+                mask & (df_fewsnet_sub["indicator"] == "production")
+            ]
             df_area = df_fewsnet_sub[mask & (df_fewsnet_sub["indicator"] == "area")]
 
             df_yield["harvest_year"] = df_yield["harvest_year"].astype(int)
             df_production["harvest_year"] = df_production["harvest_year"].astype(int)
             df_area["harvest_year"] = df_area["harvest_year"].astype(int)
 
             if df_yield[mask].empty:
@@ -154,17 +160,21 @@
 
             outlier_year = int(group["harvest_year"].values[0])
             fnid = group["fnid"].values[0]
 
             # Add 3 subplots, first for area
             plt.figure(figsize=(10, 10))
             plt.subplot(3, 1, 1)
-            plt.plot(df_yield[mask]["harvest_year"].astype(int), df_yield[mask]["value"])
+            plt.plot(
+                df_yield[mask]["harvest_year"].astype(int), df_yield[mask]["value"]
+            )
             # Add a circle for each year where yield is available
-            plt.scatter(df_yield[mask]["harvest_year"].astype(int), df_yield[mask]["value"])
+            plt.scatter(
+                df_yield[mask]["harvest_year"].astype(int), df_yield[mask]["value"]
+            )
             # Draw a horizontal line at the average df_yield[mask]["value"]
             plt.axhline(df_yield[mask]["value"].mean(), color="red", linestyle="--")
             # Place a tick on x-axis at every year and make labels vertical
             plt.xticks(df_yield[mask]["harvest_year"].astype(int)[::2], rotation=90)
             # Draw a * at the outlier year
             try:
                 plt.scatter(
@@ -191,30 +201,36 @@
                 df_production[mask]["value"],
             )
             plt.scatter(
                 df_production[mask]["harvest_year"].astype(int),
                 df_production[mask]["value"],
             )
             # Place a tick on x-axis at every year
-            plt.xticks(df_production[mask]["harvest_year"].astype(int)[::2], rotation=90)
+            plt.xticks(
+                df_production[mask]["harvest_year"].astype(int)[::2], rotation=90
+            )
             plt.xlabel("Year")
             plt.ylabel("Production")
 
             plt.subplot(3, 1, 3)
             plt.plot(df_area[mask]["harvest_year"].astype(int), df_area[mask]["value"])
-            plt.scatter(df_area[mask]["harvest_year"].astype(int), df_area[mask]["value"])
+            plt.scatter(
+                df_area[mask]["harvest_year"].astype(int), df_area[mask]["value"]
+            )
             # Place a tick on x-axis at every year
             plt.xticks(df_area[mask]["harvest_year"].astype(int)[::2], rotation=90)
             plt.xlabel("Year")
             plt.ylabel("Area")
 
             try:
                 os.makedirs(BASE_DIR / crop, exist_ok=True)
                 plt.savefig(
-                    BASE_DIR / crop / f"{fnid}_{country}_{admin_1}_{crop}_{season_name}.png"
+                    BASE_DIR
+                    / crop
+                    / f"{fnid}_{country}_{admin_1}_{crop}_{season_name}.png"
                 )
             except:
                 breakpoint()
             plt.tight_layout()
             plt.close()
 
     breakpoint()
```

### Comparing `geocif-0.1.29/geocif/ml/outlook.py` & `geocif-0.1.30/geocif/ml/outlook.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/ml/output.py` & `geocif-0.1.30/geocif/ml/output.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/ml/stages.py` & `geocif-0.1.30/geocif/ml/stages.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     Returns:
 
     """
     # Change to type string
     df["Stage"] = df["Stage"].astype(str)
 
     df["Stage_ID"] = df["Stage"]
-    df["Stage Range"] = df["Stage"].apply(lambda x: "_".join([x.split("_")[0], x.split("_")[-1]]))
+    df["Stage Range"] = df["Stage"].apply(
+        lambda x: "_".join([x.split("_")[0], x.split("_")[-1]])
+    )
 
     # Create a column with starting stage and ending stage
     # Stage looks like this: 13_12_11
     # Starting Stage will look like this: 13
     # Ending Stage will look like this: 11
     df["Starting Stage"] = df["Stage"].apply(lambda x: int(x.split("_")[0]))
     df["Ending Stage"] = df["Stage"].apply(lambda x: int(x.split("_")[-1]))
@@ -30,22 +32,26 @@
     # to the Starting Stage and Ending Stage
     if "dekad" in method:
         dict = utils.dict_growth_stages
     elif "biweekly" in method:
         dict = utils.dict_growth_stages_biweekly
     elif "monthly" in method:
         dict = utils.dict_growth_stages_monthly
-    df["Stage Names"] = df["Starting Stage"].map(dict) + " - " + df["Ending Stage"].map(dict)
+    df["Stage Names"] = (
+        df["Starting Stage"].map(dict) + " - " + df["Ending Stage"].map(dict)
+    )
 
     # Group by Region, Harvest Year
     # For each group, add a column called Percentage Season
     # that is the percentage of the season that has passed based on the number of rows
     # in the group
     grouped = df.groupby(["Region", "Harvest Year"])
-    df["Percentage Season"] = grouped.cumcount() * 100.0 / grouped["CEI"].transform("size")
+    df["Percentage Season"] = (
+        grouped.cumcount() * 100.0 / grouped["CEI"].transform("size")
+    )
 
     return df
 
 
 def remove_duplicates(arrays):
     """
 
@@ -182,15 +188,17 @@
 
     parts = stage_str.split("_")
     cei = parts[0] if parts[1].isdigit() else "_".join(parts[:2])
     start_stage = parts[1] if parts[1].isdigit() else parts[2]
     end_stage = parts[-1]
 
     # Exclude cei from the stage_str string
-    stage_info["Stage_ID"] = "_".join(parts[1:]) if parts[1].isdigit() else "_".join(parts[2:])
+    stage_info["Stage_ID"] = (
+        "_".join(parts[1:]) if parts[1].isdigit() else "_".join(parts[2:])
+    )
 
     stage_info["CEI"] = cei
     stage_info["Stage Range"] = "_".join([start_stage, end_stage])
 
     stage_info["Starting Stage"] = int(start_stage)
     stage_info["Ending Stage"] = int(end_stage)
```

### Comparing `geocif-0.1.29/geocif/ml/stats.py` & `geocif-0.1.30/geocif/ml/stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,41 +25,62 @@
         # Find if country and region exists in calendar
         # mask_adm1 = (df['ADM1_NAME'].str.lower() == reg.lower())
 
         # if not df['ADM1_NAME'].isnull().all():
         #    df_tmp = df.loc[mask_adm1]
 
         df_tmp = df.copy()
-        if name_crop == 'rice':
-            if cntr == 'Viet nam':
-                df_tmp = df.loc[df.Season == 'Spring Paddy']
-            elif cntr == 'Thailand':
-                df_tmp = df.loc[df.Season == 'Major Season']
-            elif cntr == 'China':
-                df_tmp = df.loc[df.Season == 'Single-cropping and Middle-season Rice']
-            elif cntr == 'India':
-                df_tmp = df.loc[df.Season == 'Kharif']
-        elif name_crop == 'maize' and \
-                cntr in ['Austria', 'Belgium', 'Bulgaria', 'Croatia', 'Czech  Republic', 'Denmark','Germany', 'Greece', 'Hungary',
-                         'Italy', 'Lithuania', 'Luxembourg', 'Netherlands', 'Poland', 'Portugal', 'Romania', 'Slovakia', 'Slovenia', 'Spain',
-                         'Sweden', 'United Kingdom']:
-            df_tmp = df.loc[df.Season == 'Grain Maize and Corn-cob-mix']
-        elif name_crop == 'maize' and cntr in ['France']:
-            df_tmp = df.loc[df.Season == 'Green Maize']
+        if name_crop == "rice":
+            if cntr == "Viet nam":
+                df_tmp = df.loc[df.Season == "Spring Paddy"]
+            elif cntr == "Thailand":
+                df_tmp = df.loc[df.Season == "Major Season"]
+            elif cntr == "China":
+                df_tmp = df.loc[df.Season == "Single-cropping and Middle-season Rice"]
+            elif cntr == "India":
+                df_tmp = df.loc[df.Season == "Kharif"]
+        elif name_crop == "maize" and cntr in [
+            "Austria",
+            "Belgium",
+            "Bulgaria",
+            "Croatia",
+            "Czech  Republic",
+            "Denmark",
+            "Germany",
+            "Greece",
+            "Hungary",
+            "Italy",
+            "Lithuania",
+            "Luxembourg",
+            "Netherlands",
+            "Poland",
+            "Portugal",
+            "Romania",
+            "Slovakia",
+            "Slovenia",
+            "Spain",
+            "Sweden",
+            "United Kingdom",
+        ]:
+            df_tmp = df.loc[df.Season == "Grain Maize and Corn-cob-mix"]
+        elif name_crop == "maize" and cntr in ["France"]:
+            df_tmp = df.loc[df.Season == "Green Maize"]
 
         if not df_tmp.empty:
-            if cntr != 'Vietnam':
-                mask_tmp_country = (df_tmp['ADM0_NAME'].str.lower() == cntr.replace('_', ' ').lower())
+            if cntr != "Vietnam":
+                mask_tmp_country = (
+                    df_tmp["ADM0_NAME"].str.lower() == cntr.replace("_", " ").lower()
+                )
             else:
-                mask_tmp_country = (df_tmp['ADM0_NAME'].str.lower() == 'viet nam')
+                mask_tmp_country = df_tmp["ADM0_NAME"].str.lower() == "viet nam"
             if region:
-                mask_tmp_adm1 = (df_tmp[region_column].str.lower() == region.lower())
+                mask_tmp_adm1 = df_tmp[region_column].str.lower() == region.lower()
             else:
                 # ADM1_NAME column should be NaN to get country level stats
-                mask_tmp_adm1 = (df_tmp[region_column].isnull())
+                mask_tmp_adm1 = df_tmp[region_column].isnull()
 
             val = df_tmp.loc[mask_tmp_country & mask_tmp_adm1][calendar_year]
 
             try:
                 if val.isnull().all():
                     val = np.NaN
                 else:
@@ -141,15 +162,24 @@
 
             # Add the statistic to the dataframe
             df.loc[group.index, stat] = val
 
     return df
 
 
-def add_statistics(dir_stats, df, country, crop, admin_zone, stats, method, target_col="Yield (tn per ha)"):
+def add_statistics(
+    dir_stats,
+    df,
+    country,
+    crop,
+    admin_zone,
+    stats,
+    method,
+    target_col="Yield (tn per ha)",
+):
     """
 
     Args:
         df:
         country:
         crop:
         admin_zone:
@@ -162,15 +192,17 @@
     """
     # First check if country and crop are in the admin_crop_production.csv file
     fn = "afghanistan.csv" if country == "Afghanistan" else "adm_crop_production.csv"
     df_fewsnet = pd.read_csv(dir_stats / fn, low_memory=False)
 
     # HACK
     if country == "Afghanistan":
-        df_fewsnet.loc[:, "product"] = df_fewsnet["season_name"] + " " + df_fewsnet["product"]
+        df_fewsnet.loc[:, "product"] = (
+            df_fewsnet["season_name"] + " " + df_fewsnet["product"]
+        )
     # Check if country and crop exist in the fewsnet database
     mask = (df_fewsnet["country"] == country) & (df_fewsnet["product"] == crop)
 
     if mask.sum() == 0 or country == "Malawi" or country == "Zambia":
         df = add_GEOGLAM_statistics(dir_stats, df, stats, method, admin_zone)
     else:
         group_by = ["Region", "Harvest Year"]
@@ -179,20 +211,35 @@
         # Define processing for each group
         def process_group(group, region, harvest_year):
             mask = (df["Region"] == region) & (df["Harvest Year"] == harvest_year)
 
             mask_region = df_fewsnet[admin_zone] == region
             mask_yield = (
                 df_fewsnet["crop_production_system"].isin(
-                    ["none", "Small-scale (PS)", "Commercial (PS)", "All (PS)", "irrigated", "rainfed"]
+                    [
+                        "none",
+                        "Small-scale (PS)",
+                        "Commercial (PS)",
+                        "All (PS)",
+                        "irrigated",
+                        "rainfed",
+                    ]
                 )
                 & (df_fewsnet["harvest_year"] == harvest_year)
                 & (df_fewsnet["product"] == crop)
                 & df_fewsnet["season_name"].isin(
-                    ["Main", "Meher", "Main harvest", "Annual", "Summer", "Spring", "Winter"]
+                    [
+                        "Main",
+                        "Meher",
+                        "Main harvest",
+                        "Annual",
+                        "Summer",
+                        "Spring",
+                        "Winter",
+                    ]
                 )
                 & (df_fewsnet["indicator"].isin(["yield", "area", "production"]))
             )
 
             # Fetching values for each indicator
             yield_value = df_fewsnet.loc[
                 mask_yield & mask_region & (df_fewsnet["indicator"] == "yield"), "value"
```

### Comparing `geocif-0.1.29/geocif/ml/trainers.py` & `geocif-0.1.30/geocif/ml/trainers.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,17 @@
     Returns:
 
     """
     X = df[feature_names + cat_features]
     y = df[target_col]
 
     # Divide the data into training and validation sets
-    train_X, val_X, train_y, val_y = train_test_split(X, y, test_size=0.2, random_state=0)
+    train_X, val_X, train_y, val_y = train_test_split(
+        X, y, test_size=0.2, random_state=0
+    )
 
     model.fit(
         train_X,
         train_y,
         cat_features=cat_features,
         eval_set=(val_X, val_y),
         early_stopping_rounds=100,
@@ -130,15 +132,17 @@
     # Define objecive function for optuna Hyperparameter tuning
     def _optuna_objective(trial):
         try:
             if model_name == "catboost":
                 params = {
                     "depth": trial.suggest_int("depth", 1, 7),
                     "learning_rate": trial.suggest_float("learning_rate", 0.01, 0.1),
-                    "iterations": trial.suggest_int("iterations", low=1000, high=5000, step=500),
+                    "iterations": trial.suggest_int(
+                        "iterations", low=1000, high=5000, step=500
+                    ),
                     "subsample": trial.suggest_float("subsample", 1.0, 1.0),
                     "random_strength": trial.suggest_float("random_strength", 0.3, 1.0),
                     "reg_lambda": trial.suggest_float("reg_lambda", 1e-8, 1.0),
                     "loss_function": "MAPE",
                     "early_stopping_rounds": 50,
                     "random_seed": seed,
                     "verbose": False,
@@ -173,15 +177,17 @@
 
     try:
         # Optimize hyperparameters
         n_trials = min(20, int(mp.cpu_count() * 0.9))
         optuna.logging.set_verbosity(optuna.logging.WARNING)  # Disable verbose
         sampler = optuna.samplers.TPESampler(seed=seed)
         study = optuna.create_study(sampler=sampler, direction="minimize")
-        study.optimize(_optuna_objective, n_trials=n_trials, n_jobs=int(mp.cpu_count() * 0.4))
+        study.optimize(
+            _optuna_objective, n_trials=n_trials, n_jobs=int(mp.cpu_count() * 0.4)
+        )
         if study.best_trial is None:
             raise ValueError("Optimization failed to complete any trials.")
         hyperparams = study.best_trial.params
 
     except Exception as e:
         print(f"Optimization failed: {e}")
         hyperparams = {
```

### Comparing `geocif-0.1.29/geocif/ml/trend.py` & `geocif-0.1.30/geocif/ml/trend.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,17 @@
     # if future_time_points is not of type pandas dataframe then convert it to one
     future_time_points = np.array(future_time_points)
 
     model_type = detrended_data.model_type[0]
     model = detrended_data.trend_model[0]
 
     if model_type == "mean":
-        trend_component = model.predict(np.ones(len(future_time_points)), has_constant="add")
+        trend_component = model.predict(
+            np.ones(len(future_time_points)), has_constant="add"
+        )
     elif model_type == "linear":
         X_linear = add_constant(future_time_points, has_constant="add")
         trend_component = model.predict(X_linear)
     else:  # quadratic
         X_quad = add_constant(
             np.column_stack((future_time_points, future_time_points**2)),
             has_constant="add",
```

### Comparing `geocif-0.1.29/geocif/ml/xai.py` & `geocif-0.1.30/geocif/ml/xai.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/playground/misc.py` & `geocif-0.1.30/geocif/playground/misc.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/utils.py` & `geocif-0.1.30/geocif/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif/viz/plot.py` & `geocif-0.1.30/geocif/viz/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.29/geocif.egg-info/PKG-INFO` & `geocif-0.1.30/geocif.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.29
+Version: 0.1.30
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `geocif-0.1.29/geocif.egg-info/SOURCES.txt` & `geocif-0.1.30/geocif.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 geocif/ml/correlations.py
 geocif/ml/embedding.py
 geocif/ml/feature_engineering.py
 geocif/ml/feature_selection.py
 geocif/ml/outliers.py
 geocif/ml/outlook.py
 geocif/ml/output.py
+geocif/ml/spatial_autocorrelation.py
 geocif/ml/stages.py
 geocif/ml/stats.py
 geocif/ml/trainers.py
 geocif/ml/trend.py
 geocif/ml/xai.py
 geocif/playground/__init__.py
 geocif/playground/automl.py
```

### Comparing `geocif-0.1.29/setup.py` & `geocif-0.1.30/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords="geocif",
     name="geocif",
     packages=find_packages(include=["geocif", "geocif.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://ritviksahajpal.github.io/yield_forecasting/",
-    version="0.1.29",
+    version="0.1.30",
     zip_safe=False,
 )
```

