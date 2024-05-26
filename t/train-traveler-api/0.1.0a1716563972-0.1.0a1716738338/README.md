# Comparing `tmp/train_traveler_api-0.1.0a1716563972.tar.gz` & `tmp/train_traveler_api-0.1.0a1716738338.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "train_traveler_api-0.1.0a1716563972.tar", last modified: Fri May 24 15:19:32 2024, max compression
+gzip compressed data, was "train_traveler_api-0.1.0a1716738338.tar", last modified: Sun May 26 15:45:37 2024, max compression
```

## Comparing `train_traveler_api-0.1.0a1716563972.tar` & `train_traveler_api-0.1.0a1716738338.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.460365 train_traveler_api-0.1.0a1716563972/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4432 2024-05-24 15:19:32.460365 train_traveler_api-0.1.0a1716563972/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4001 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-05-24 15:19:32.460365 train_traveler_api-0.1.0a1716563972/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      836 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/connections/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/connections/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      231 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/connections/connection_manager.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/entities/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1681 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/disruption_entity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      136 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/entity_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      621 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/information_entity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1749 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/journey_entity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      444 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/line_entity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      295 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/link_entity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      529 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/place_entity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      409 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/public_transport_entity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/stop_date_time_entity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      729 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/stop_entity.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/models/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/models/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      191 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/models/area_model.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      295 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/models/journey_model.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      270 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/models/next_journey_model.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/repositories/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4395 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/disruption_repository.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8339 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/journey_repository.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1833 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/line_repository.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1323 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/link_repository.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1619 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/place_repository.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2261 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/repository_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3637 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/stop_area_repository.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      392 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/stop_point_repository.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/services/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      449 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/area_service.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      379 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/info_service.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6944 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/journey_service.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       70 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/service_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9035 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/train_traveler.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.460365 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4432 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1320 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       60 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        5 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4432 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4001 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      836 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/sncf/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/sncf/connections/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/connections/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      231 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/connections/connection_manager.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/sncf/entities/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1678 2024-05-26 15:11:28.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/disruption_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      136 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/entity_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      621 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/information_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1749 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/journey_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      444 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/line_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      295 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/link_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      529 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/place_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      409 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/public_transport_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/stop_date_time_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      729 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/entities/stop_entity.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/sncf/models/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/models/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      191 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/models/area_model.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      295 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/models/journey_model.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      270 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/models/next_journey_model.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/sncf/repositories/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/repositories/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4389 2024-05-26 15:12:27.000000 train_traveler_api-0.1.0a1716738338/sncf/repositories/disruption_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8469 2024-05-26 15:09:58.000000 train_traveler_api-0.1.0a1716738338/sncf/repositories/journey_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1833 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/repositories/line_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1323 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/repositories/link_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1619 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/repositories/place_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2261 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/repositories/repository_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3637 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/repositories/stop_area_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      392 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/repositories/stop_point_repository.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/sncf/services/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/services/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      449 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/services/area_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      379 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/services/info_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6971 2024-05-25 08:34:58.000000 train_traveler_api-0.1.0a1716738338/sncf/services/journey_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       70 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/services/service_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9035 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716738338/sncf/train_traveler.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-26 15:45:37.737378 train_traveler_api-0.1.0a1716738338/train_traveler_api.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4432 2024-05-26 15:45:37.000000 train_traveler_api-0.1.0a1716738338/train_traveler_api.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1320 2024-05-26 15:45:37.000000 train_traveler_api-0.1.0a1716738338/train_traveler_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-26 15:45:37.000000 train_traveler_api-0.1.0a1716738338/train_traveler_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       60 2024-05-26 15:45:37.000000 train_traveler_api-0.1.0a1716738338/train_traveler_api.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        5 2024-05-26 15:45:37.000000 train_traveler_api-0.1.0a1716738338/train_traveler_api.egg-info/top_level.txt
```

### Comparing `train_traveler_api-0.1.0a1716563972/LICENSE` & `train_traveler_api-0.1.0a1716738338/LICENSE`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/PKG-INFO` & `train_traveler_api-0.1.0a1716738338/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: train-traveler-api
-Version: 0.1.0a1716563972
+Version: 0.1.0a1716738338
 Summary: Train traveler is a backend for SNCF API
 Home-page: https://github.com/Matthyeux/train-traveler-api
 Author: Matthieu DURINDEL
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `train_traveler_api-0.1.0a1716563972/README.md` & `train_traveler_api-0.1.0a1716738338/README.md`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/setup.py` & `train_traveler_api-0.1.0a1716738338/setup.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/entities/disruption_entity.py` & `train_traveler_api-0.1.0a1716738338/sncf/entities/disruption_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,22 +24,22 @@
         
 
 class ImpactedStopsEntity(Entity):
     def __init__(
             self, 
             stop_point: StopPointEntity, 
             base_arrival_time: datetime, 
-            ammended_arrival_time: datetime, 
+            amended_arrival_time: datetime, 
             base_departure_time: datetime, 
             ammended_departure_time: datetime,
             departure_status: str,
             arrival_status: str,
             cause: str
         ):
         self.stop_point = stop_point
         self.base_arrival_time = base_arrival_time
-        self.ammended_arrival_time = ammended_arrival_time
+        self.amended_arrival_time = amended_arrival_time
         self.base_departure_time = base_departure_time
         self.ammended_departure_time = ammended_departure_time
         self.departure_status = departure_status
         self.arrival_status = arrival_status
         self.cause = cause
```

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/entities/information_entity.py` & `train_traveler_api-0.1.0a1716738338/sncf/entities/information_entity.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/entities/journey_entity.py` & `train_traveler_api-0.1.0a1716738338/sncf/entities/journey_entity.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/entities/place_entity.py` & `train_traveler_api-0.1.0a1716738338/sncf/entities/place_entity.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/entities/stop_date_time_entity.py` & `train_traveler_api-0.1.0a1716738338/sncf/entities/stop_date_time_entity.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/entities/stop_entity.py` & `train_traveler_api-0.1.0a1716738338/sncf/entities/stop_entity.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/repositories/disruption_repository.py` & `train_traveler_api-0.1.0a1716738338/sncf/repositories/disruption_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,29 +55,29 @@
                     base_departure_time = datetime.strptime(impacted_stop["base_departure_time"],"%H%M%S")
 
                 if "base_arrival_time" not in impacted_stop:
                     base_arrival_time = None
                 else:
                     base_arrival_time = datetime.strptime(impacted_stop["base_arrival_time"],"%H%M%S")
 
-                if "amended_departure_time" not in impacted_stop:
-                    ammended_arrival_time = None
+                if "amended_arrival_time" not in impacted_stop:
+                    amended_arrival_time = None
                 else:
-                    ammended_arrival_time = datetime.strptime(impacted_stop["amended_arrival_time"],"%H%M%S")
+                    amended_arrival_time = datetime.strptime(impacted_stop["amended_arrival_time"],"%H%M%S")
 
                 if "amended_departure_time" not in impacted_stop:
                     ammended_departure_time = None
                 else:
                     ammended_departure_time = datetime.strptime(impacted_stop["amended_departure_time"],"%H%M%S")
 
 
                 impactedStopEntity = ImpactedStopsEntity(
                     stop_point=stop_point_entity,
                     base_arrival_time=base_arrival_time,
-                    ammended_arrival_time=ammended_arrival_time,
+                    amended_arrival_time=amended_arrival_time,
                     base_departure_time=base_departure_time,
                     ammended_departure_time=ammended_departure_time,
                     departure_status=impacted_stop["departure_status"],
                     arrival_status=impacted_stop["arrival_status"],
                     cause=impacted_stop["cause"]
                 )
```

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/repositories/journey_repository.py` & `train_traveler_api-0.1.0a1716738338/sncf/repositories/journey_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,20 @@
 
         journeys_entities = []
         for journey in journeys:  
 
             sections_entities = []
             for section in journey["sections"]:
                 
+                if section["type"] != "public_transport":
+                    continue
+                
                 # In some cases, to and from are equals and informations are still retrieved, so we skip it
                 if section["to"]["stop_point"]["stop_area"]["id"] == section["from"]["stop_point"]["stop_area"]["id"]:
-                    continue
+                    continue                
 
                 informations = section["display_informations"]
 
                 disruptions_ids = []
                 for link in informations["links"]:
                     if link["type"] == "disruption":
                         disruptions_ids.append(link["id"])
@@ -61,17 +64,17 @@
                     color=informations["color"],
                     name=informations["name"],
                     physical_mode=informations["physical_mode"],
                     trip_short_name=informations["trip_short_name"],
                     disruptions_ids=disruptions_ids
                 )
 
-                next_stop_date_times = section["stop_date_times"]
-                
                 next_stop_date_times_entities = []
+                next_stop_date_times = section["stop_date_times"]
+
                 for stop_date_time in next_stop_date_times:
 
                     departure_date_time = datetime.strptime(stop_date_time["departure_date_time"],"%Y%m%dT%H%M%S")
                     arrival_date_time = datetime.strptime(stop_date_time["arrival_date_time"],"%Y%m%dT%H%M%S")
 
                     # In case of modified services, base_departure_date_time and base_arrival_date_time cannot be filled
                     if "base_departure_date_time" not in stop_date_time:
@@ -96,15 +99,15 @@
                             coord={
                                 "lon": stop_date_time["stop_point"]["coord"]["lon"],
                                 "lat": stop_date_time["stop_point"]["coord"]["lat"]
                             },
                             stop_area=[]
                         )
                     )
-                next_stop_date_times_entities.append(stop_date_time_entity)
+                    next_stop_date_times_entities.append(stop_date_time_entity)
 
                 if section["from"]["embedded_type"] == "stop_point":
 
                     start_point = section["from"]["stop_point"]
 
                     start_stop_entity = StopPointEntity(
                         id=start_point["id"],
@@ -145,16 +148,16 @@
                 if "base_departure_date_time" not in stop_date_time:
                     scheduled_departure_date_time = departure_date_time
                 else:
                     scheduled_departure_date_time = datetime.strptime(section["base_departure_date_time"],"%Y%m%dT%H%M%S")
 
                 if "base_arrival_date_time" not in stop_date_time:
                     scheduled_arrival_date_time = arrival_date_time
-                else:
-                    scheduled_arrival_date_time=datetime.strptime(section["base_arrival_date_time"],"%Y%m%dT%H%M%S")
+                else:                    
+                    scheduled_arrival_date_time = datetime.strptime(section["base_arrival_date_time"],"%Y%m%dT%H%M%S")
 
                 section_entity = SectionEntity(
                     id=section["id"],
                     duration=section["duration"],
                     departure_date_time=departure_date_time,
                     scheduled_departure_date_time=scheduled_departure_date_time,
                     arrival_date_time=arrival_date_time,
```

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/repositories/line_repository.py` & `train_traveler_api-0.1.0a1716738338/sncf/repositories/line_repository.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/repositories/link_repository.py` & `train_traveler_api-0.1.0a1716738338/sncf/repositories/link_repository.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/repositories/place_repository.py` & `train_traveler_api-0.1.0a1716738338/sncf/repositories/place_repository.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/repositories/repository_manager.py` & `train_traveler_api-0.1.0a1716738338/sncf/repositories/repository_manager.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/repositories/stop_area_repository.py` & `train_traveler_api-0.1.0a1716738338/sncf/repositories/stop_area_repository.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/services/journey_service.py` & `train_traveler_api-0.1.0a1716738338/sncf/services/journey_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                             datetime=last_journeys[0].departure_date_time + timedelta(seconds=1), 
                             datetime_represents="departure",
                             data_freshness="realtime"
                         )
 
                         
 
-                        while next_journeys[0].departure_date_time.date() == datetime.today().date():
+                        while len(next_journeys) > 0 and next_journeys[0].departure_date_time.date() == datetime.today().date():
                             last_journeys = next_journeys
 
                             next_journeys = self.journey_repository.find_journeys(
                                 start_stop_point.id, 
                                 end_stop_point.id, 
                                 allowed_id=[line.id], 
                                 max_nb_transfers=0,
```

### Comparing `train_traveler_api-0.1.0a1716563972/sncf/train_traveler.py` & `train_traveler_api-0.1.0a1716738338/sncf/train_traveler.py`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/PKG-INFO` & `train_traveler_api-0.1.0a1716738338/train_traveler_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: train-traveler-api
-Version: 0.1.0a1716563972
+Version: 0.1.0a1716738338
 Summary: Train traveler is a backend for SNCF API
 Home-page: https://github.com/Matthyeux/train-traveler-api
 Author: Matthieu DURINDEL
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/SOURCES.txt` & `train_traveler_api-0.1.0a1716738338/train_traveler_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

