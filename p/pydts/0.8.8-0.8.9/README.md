# Comparing `tmp/pydts-0.8.8.tar.gz` & `tmp/pydts-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydts-0.8.8.tar", max compression
+gzip compressed data, was "pydts-0.8.9.tar", max compression
```

## Comparing `pydts-0.8.8.tar` & `pydts-0.8.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.8.8/LICENSE
--rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.8.8/README.md
--rw-r--r--   0        0        0     1441 2024-03-24 10:49:54.359781 pydts-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.8.8/src/pydts/.DS_Store
--rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.8.8/src/pydts/__init__.py
--rw-r--r--   0        0        0    13253 2023-11-08 11:17:22.141397 pydts-0.8.8/src/pydts/base_fitters.py
--rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.8.8/src/pydts/config.py
--rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.8.8/src/pydts/cross_validation.py
--rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.8.8/src/pydts/data_generation.py
--rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.8.8/src/pydts/datasets/.DS_Store
--rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.8.8/src/pydts/datasets/LOS_simulated_data.csv
--rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.8.8/src/pydts/evaluation.py
--rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.8.8/src/pydts/examples_utils/__init__.py
--rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.8.8/src/pydts/examples_utils/datasets.py
--rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.8.8/src/pydts/examples_utils/generate_simulations_data.py
--rw-r--r--   0        0        0    14554 2023-06-22 21:08:27.939724 pydts-0.8.8/src/pydts/examples_utils/mimic_consts.py
--rw-r--r--   0        0        0    35688 2023-06-26 12:35:09.771826 pydts-0.8.8/src/pydts/examples_utils/plots.py
--rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.8.8/src/pydts/examples_utils/simulations_data_config.py
--rw-r--r--   0        0        0    34455 2024-03-24 10:41:54.864225 pydts-0.8.8/src/pydts/fitters.py
--rw-r--r--   0        0        0     8936 2023-06-28 07:27:17.982441 pydts-0.8.8/src/pydts/model_selection.py
--rw-r--r--   0        0        0    24281 2023-11-08 13:05:26.817721 pydts-0.8.8/src/pydts/screening.py
--rw-r--r--   0        0        0     6343 2024-03-24 10:41:54.861868 pydts-0.8.8/src/pydts/utils.py
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 pydts-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      757 2022-06-10 18:48:04.918673 pydts-0.8.9/LICENSE
+-rw-r--r--   0        0        0     2655 2023-03-03 09:40:33.185838 pydts-0.8.9/README.md
+-rw-r--r--   0        0        0     1441 2024-05-26 17:00:46.988966 pydts-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-07-28 20:14:40.680457 pydts-0.8.9/src/pydts/.DS_Store
+-rw-r--r--   0        0        0       21 2022-05-31 10:30:06.735807 pydts-0.8.9/src/pydts/__init__.py
+-rw-r--r--   0        0        0    13253 2023-11-08 11:17:22.141397 pydts-0.8.9/src/pydts/base_fitters.py
+-rw-r--r--   0        0        0      179 2022-05-31 10:30:06.735945 pydts-0.8.9/src/pydts/config.py
+-rw-r--r--   0        0        0    12393 2023-02-22 10:39:50.257509 pydts-0.8.9/src/pydts/cross_validation.py
+-rw-r--r--   0        0        0    15114 2023-05-03 10:21:44.094825 pydts-0.8.9/src/pydts/data_generation.py
+-rw-r--r--   0        0        0     6148 2022-07-30 20:46:05.091197 pydts-0.8.9/src/pydts/datasets/.DS_Store
+-rw-r--r--   0        0        0  4942233 2022-07-30 20:42:16.583147 pydts-0.8.9/src/pydts/datasets/LOS_simulated_data.csv
+-rw-r--r--   0        0        0    21459 2023-05-02 09:39:52.357498 pydts-0.8.9/src/pydts/evaluation.py
+-rw-r--r--   0        0        0        0 2022-05-31 10:30:06.739086 pydts-0.8.9/src/pydts/examples_utils/__init__.py
+-rw-r--r--   0        0        0      286 2022-05-31 10:30:06.739154 pydts-0.8.9/src/pydts/examples_utils/datasets.py
+-rw-r--r--   0        0        0    10244 2023-05-02 16:42:26.483452 pydts-0.8.9/src/pydts/examples_utils/generate_simulations_data.py
+-rw-r--r--   0        0        0    14554 2023-06-22 21:08:27.939724 pydts-0.8.9/src/pydts/examples_utils/mimic_consts.py
+-rw-r--r--   0        0        0    35688 2024-05-26 17:00:46.984906 pydts-0.8.9/src/pydts/examples_utils/plots.py
+-rw-r--r--   0        0        0     1708 2022-07-28 20:09:56.672834 pydts-0.8.9/src/pydts/examples_utils/simulations_data_config.py
+-rw-r--r--   0        0        0    34455 2024-03-24 10:41:54.864225 pydts-0.8.9/src/pydts/fitters.py
+-rw-r--r--   0        0        0     8936 2023-06-28 07:27:17.982441 pydts-0.8.9/src/pydts/model_selection.py
+-rw-r--r--   0        0        0    24281 2023-11-08 13:05:26.817721 pydts-0.8.9/src/pydts/screening.py
+-rw-r--r--   0        0        0     6343 2024-03-24 10:41:54.861868 pydts-0.8.9/src/pydts/utils.py
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 pydts-0.8.9/PKG-INFO
```

### Comparing `pydts-0.8.8/LICENSE` & `pydts-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/README.md` & `pydts-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/pyproject.toml` & `pydts-0.8.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydts"
-version = "0.8.8"
+version = "0.8.9"
 description = "Discrete time survival analysis with competing risks"
 authors = ["Tomer Meir <tomer1812@gmail.com>", "Rom Gutman <rom.gutman1@gmail.com>", "Malka Gorfine <malkago12@gmail.com>"]
 license = "GNU GPLv3"
 readme = "README.md"
 homepage = "https://github.com/tomer1812/pydts"
 repository = "https://github.com/tomer1812/pydts"
 keywords = ["Discrete Time", "Time to Event" ,"Survival Analysis", "Competing Events"]
```

### Comparing `pydts-0.8.8/src/pydts/.DS_Store` & `pydts-0.8.9/src/pydts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/base_fitters.py` & `pydts-0.8.9/src/pydts/base_fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/cross_validation.py` & `pydts-0.8.9/src/pydts/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/data_generation.py` & `pydts-0.8.9/src/pydts/data_generation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/datasets/.DS_Store` & `pydts-0.8.9/src/pydts/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/datasets/LOS_simulated_data.csv` & `pydts-0.8.9/src/pydts/datasets/LOS_simulated_data.csv`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/evaluation.py` & `pydts-0.8.9/src/pydts/evaluation.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/examples_utils/generate_simulations_data.py` & `pydts-0.8.9/src/pydts/examples_utils/generate_simulations_data.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/examples_utils/mimic_consts.py` & `pydts-0.8.9/src/pydts/examples_utils/mimic_consts.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/examples_utils/plots.py` & `pydts-0.8.9/src/pydts/examples_utils/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -684,15 +684,15 @@
     for idp, pref in enumerate(['hazard', 'prob', 'cif', 'overall_survival']):
         for ide, event in enumerate(['j1', 'j2']):
             if idp*2+ide > 6:
                 break
             ax = ax_lst[idp*2+ide]
             add_panel_text(ax, letters[idp*2+ide])
             for patient in pred_df.columns:
-                times = [m for m in range(1, 31)]
+                times = [m for m in range(1, 30)]
                 if pref == 'overall_survival':
                     index_val = [f'{pref}_t{m}' for m in times]
                 elif pref == 'hazard':
                     index_val = [f'{pref}_{event}_t{m}' for m in times]
                 else:
                     index_val = [f'{pref}_{event}_at_t{m}' for m in times]
                 tmp = pred_df.loc[index_val, patient]
```

### Comparing `pydts-0.8.8/src/pydts/examples_utils/simulations_data_config.py` & `pydts-0.8.9/src/pydts/examples_utils/simulations_data_config.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/fitters.py` & `pydts-0.8.9/src/pydts/fitters.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/model_selection.py` & `pydts-0.8.9/src/pydts/model_selection.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/screening.py` & `pydts-0.8.9/src/pydts/screening.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/src/pydts/utils.py` & `pydts-0.8.9/src/pydts/utils.py`

 * *Files identical despite different names*

### Comparing `pydts-0.8.8/PKG-INFO` & `pydts-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydts
-Version: 0.8.8
+Version: 0.8.9
 Summary: Discrete time survival analysis with competing risks
 Home-page: https://github.com/tomer1812/pydts
 License: GNU GPLv3
 Keywords: Discrete Time,Time to Event,Survival Analysis,Competing Events
 Author: Tomer Meir
 Author-email: tomer1812@gmail.com
 Requires-Python: >=3.8,<3.11
```

