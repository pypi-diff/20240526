# Comparing `tmp/vancouver_watching-3.354.1.tar.gz` & `tmp/vancouver_watching-3.360.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vancouver_watching-3.354.1.tar", last modified: Sun May 26 04:48:01 2024, max compression
+gzip compressed data, was "vancouver_watching-3.360.1.tar", last modified: Sun May 26 20:41:07 2024, max compression
```

## Comparing `vancouver_watching-3.354.1.tar` & `vancouver_watching-3.360.1.tar`

### file list

```diff
@@ -1,25 +1,43 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:48:01.713942 vancouver_watching-3.354.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-26 04:48:01.713449 vancouver_watching-3.354.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3611 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/README.md
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 04:48:01.714019 vancouver_watching-3.354.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      301 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/setup.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:48:01.709063 vancouver_watching-3.354.1/vancouver_watching/
--rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/vancouver_watching/QGIS.py
--rw-r--r--   0 kamangir   (502) staff       (20)      117 2024-05-26 04:47:57.000000 vancouver_watching-3.354.1/vancouver_watching/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1235 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/vancouver_watching/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/vancouver_watching/area.py
--rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/vancouver_watching/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/vancouver_watching/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/vancouver_watching/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/vancouver_watching/notebook.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 04:17:22.000000 vancouver_watching-3.354.1/vancouver_watching/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:48:01.712832 vancouver_watching-3.354.1/vancouver_watching.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-26 04:48:01.000000 vancouver_watching-3.354.1/vancouver_watching.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      538 2024-05-26 04:48:01.000000 vancouver_watching-3.354.1/vancouver_watching.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 04:48:01.000000 vancouver_watching-3.354.1/vancouver_watching.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:48:01.000000 vancouver_watching-3.354.1/vancouver_watching.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-05-26 04:48:01.000000 vancouver_watching-3.354.1/vancouver_watching.egg-info/top_level.txt
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:41:07.743056 vancouver_watching-3.360.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-26 20:41:07.742241 vancouver_watching-3.360.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3611 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/README.md
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 20:41:07.743234 vancouver_watching-3.360.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      385 2024-05-26 20:40:48.000000 vancouver_watching-3.360.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:41:07.731983 vancouver_watching-3.360.1/vancouver_watching/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:41:07.738434 vancouver_watching-3.360.1/vancouver_watching/.abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      166 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       74 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/aka.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       65 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/alias.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1109 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/discover.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:41:07.739310 vancouver_watching-3.360.1/vancouver_watching/.abcli/discovery/
+-rw-r--r--   0 kamangir   (502) staff       (20)      225 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/discovery/iran.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      458 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/discovery/vancouver.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2258 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1041 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      982 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/openai_vision.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1763 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/process.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:41:07.740729 vancouver_watching-3.360.1/vancouver_watching/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      549 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/tests/ingest.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      341 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/tests/list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      403 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/tests/process.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     2618 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/update.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      745 2024-05-26 17:36:39.000000 vancouver_watching-3.360.1/vancouver_watching/.abcli/vancouver_watching.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     4758 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/vancouver_watching/QGIS.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      151 2024-05-26 20:41:02.000000 vancouver_watching-3.360.1/vancouver_watching/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1235 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/vancouver_watching/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6783 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/vancouver_watching/area.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      127 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/vancouver_watching/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      284 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/vancouver_watching/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/vancouver_watching/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      355 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/vancouver_watching/notebook.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 04:17:22.000000 vancouver_watching-3.360.1/vancouver_watching/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:41:07.741273 vancouver_watching-3.360.1/vancouver_watching.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4633 2024-05-26 20:41:07.000000 vancouver_watching-3.360.1/vancouver_watching.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1133 2024-05-26 20:41:07.000000 vancouver_watching-3.360.1/vancouver_watching.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 20:41:07.000000 vancouver_watching-3.360.1/vancouver_watching.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      156 2024-05-26 20:41:07.000000 vancouver_watching-3.360.1/vancouver_watching.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       19 2024-05-26 20:41:07.000000 vancouver_watching-3.360.1/vancouver_watching.egg-info/top_level.txt
```

### Comparing `vancouver_watching-3.354.1/LICENSE` & `vancouver_watching-3.360.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.354.1/PKG-INFO` & `vancouver_watching-3.360.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.354.1
+Version: 3.360.1
 Summary: 🌈 Vancouver Watching with AI.
-Home-page: https://github.com/kamangir/Vancouver-Watching
+Home-page: https://github.com/kamangir/vancouver-watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
@@ -102,25 +102,25 @@
 
 To discover the available cameras in an area type in,
 
 ```bash
 vanwatch discover area=vancouver
 ```
 
-You have generated a `geojson` of [traffic images in the City of Vancouver](https://raw.githubusercontent.com/kamangir/Vancouver-Watching/main/data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
+You have generated a `geojson` of [traffic images in the City of Vancouver](https://raw.githubusercontent.com/kamangir/vancouver-watching/main/data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
 
 ```bash
 vanwatch ingest area=vancouver,count=2,publish
 ```
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-25-openai-vision/DavieWestBute-inference.jpg?raw=true)
 
 model: https://hub.ultralytics.com/models/R6nMlK6kQjSsQ76MPqQM?tab=preview
 
-[![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-25-openai-vision/QGIS.png?raw=true)](https://raw.githubusercontent.com/kamangir/Vancouver-Watching/main/QGIS/2023-11-12-12-03-40-85851.geojson)
+[![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-25-openai-vision/QGIS.png?raw=true)](https://raw.githubusercontent.com/kamangir/vancouver-watching/main/QGIS/2023-11-12-12-03-40-85851.geojson)
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-12-14-42-23-96479.gif?raw=true?raw=1)
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2024-01-06-20-39-46-73614-QGIS.gif?raw=true?raw=1)
 
 dataset: [vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz](https://kamangir-public.s3.ca-central-1.amazonaws.com/vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz) ([details](https://medium.com/@arash-kamangir/vancouver-watching-with-ai-37-72b6a032b7fa)).
```

### Comparing `vancouver_watching-3.354.1/README.md` & `vancouver_watching-3.360.1/README.md`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.354.1/vancouver_watching/QGIS.py` & `vancouver_watching-3.360.1/vancouver_watching/QGIS.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.354.1/vancouver_watching/__main__.py` & `vancouver_watching-3.360.1/vancouver_watching/__main__.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.354.1/vancouver_watching/area.py` & `vancouver_watching-3.360.1/vancouver_watching/area.py`

 * *Files identical despite different names*

### Comparing `vancouver_watching-3.354.1/vancouver_watching.egg-info/PKG-INFO` & `vancouver_watching-3.360.1/vancouver_watching.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: vancouver_watching
-Version: 3.354.1
+Version: 3.360.1
 Summary: 🌈 Vancouver Watching with AI.
-Home-page: https://github.com/kamangir/Vancouver-Watching
+Home-page: https://github.com/kamangir/vancouver-watching
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
@@ -102,25 +102,25 @@
 
 To discover the available cameras in an area type in,
 
 ```bash
 vanwatch discover area=vancouver
 ```
 
-You have generated a `geojson` of [traffic images in the City of Vancouver](https://raw.githubusercontent.com/kamangir/Vancouver-Watching/main/data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
+You have generated a `geojson` of [traffic images in the City of Vancouver](https://raw.githubusercontent.com/kamangir/vancouver-watching/main/data/vancouver.geojson). Now, you can ingest the traffic images from this area and detect people and cars in them,
 
 ```bash
 vanwatch ingest area=vancouver,count=2,publish
 ```
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-25-openai-vision/DavieWestBute-inference.jpg?raw=true)
 
 model: https://hub.ultralytics.com/models/R6nMlK6kQjSsQ76MPqQM?tab=preview
 
-[![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-25-openai-vision/QGIS.png?raw=true)](https://raw.githubusercontent.com/kamangir/Vancouver-Watching/main/QGIS/2023-11-12-12-03-40-85851.geojson)
+[![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-25-openai-vision/QGIS.png?raw=true)](https://raw.githubusercontent.com/kamangir/vancouver-watching/main/QGIS/2023-11-12-12-03-40-85851.geojson)
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2023-11-12-14-42-23-96479.gif?raw=true?raw=1)
 
 ![image](https://github.com/kamangir/assets/blob/main/vanwatch/2024-01-06-20-39-46-73614-QGIS.gif?raw=true?raw=1)
 
 dataset: [vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz](https://kamangir-public.s3.ca-central-1.amazonaws.com/vanwatch-cache-2024-02-28-21-04-19-26236.tar.gz) ([details](https://medium.com/@arash-kamangir/vancouver-watching-with-ai-37-72b6a032b7fa)).
```

