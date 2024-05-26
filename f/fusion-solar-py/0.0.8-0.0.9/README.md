# Comparing `tmp/fusion_solar_py-0.0.8.tar.gz` & `tmp/fusion_solar_py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion_solar_py-0.0.8.tar", last modified: Sat Jan 28 20:50:35 2023, max compression
+gzip compressed data, was "fusion_solar_py-0.0.9.tar", last modified: Wed Feb  1 14:17:47 2023, max compression
```

## Comparing `fusion_solar_py-0.0.8.tar` & `fusion_solar_py-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 jg        (1000) jg        (1000)        0 2023-01-28 20:50:35.343515 fusion_solar_py-0.0.8/
--rw-rw-r--   0 jg        (1000) jg        (1000)     1057 2022-04-01 18:22:08.000000 fusion_solar_py-0.0.8/LICENSE.txt
--rw-rw-r--   0 jg        (1000) jg        (1000)     3371 2023-01-28 20:50:35.343515 fusion_solar_py-0.0.8/PKG-INFO
--rw-rw-r--   0 jg        (1000) jg        (1000)     2814 2023-01-28 20:47:42.000000 fusion_solar_py-0.0.8/README.md
--rw-rw-r--   0 jg        (1000) jg        (1000)       84 2022-04-01 18:17:20.000000 fusion_solar_py-0.0.8/pyproject.toml
--rw-rw-r--   0 jg        (1000) jg        (1000)      685 2023-01-28 20:50:35.347515 fusion_solar_py-0.0.8/setup.cfg
-drwxrwxr-x   0 jg        (1000) jg        (1000)        0 2023-01-28 20:50:35.343515 fusion_solar_py-0.0.8/src/
-drwxrwxr-x   0 jg        (1000) jg        (1000)        0 2023-01-28 20:50:35.343515 fusion_solar_py-0.0.8/src/fusion_solar_py/
--rw-rw-r--   0 jg        (1000) jg        (1000)        0 2022-03-29 14:27:39.000000 fusion_solar_py-0.0.8/src/fusion_solar_py/__init__.py
--rw-rw-r--   0 jg        (1000) jg        (1000)    15666 2023-01-28 20:38:29.000000 fusion_solar_py-0.0.8/src/fusion_solar_py/client.py
--rw-rw-r--   0 jg        (1000) jg        (1000)      442 2022-07-21 18:27:03.000000 fusion_solar_py-0.0.8/src/fusion_solar_py/exceptions.py
-drwxrwxr-x   0 jg        (1000) jg        (1000)        0 2023-01-28 20:50:35.343515 fusion_solar_py-0.0.8/src/fusion_solar_py.egg-info/
--rw-rw-r--   0 jg        (1000) jg        (1000)     3371 2023-01-28 20:50:35.000000 fusion_solar_py-0.0.8/src/fusion_solar_py.egg-info/PKG-INFO
--rw-rw-r--   0 jg        (1000) jg        (1000)      356 2023-01-28 20:50:35.000000 fusion_solar_py-0.0.8/src/fusion_solar_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jg        (1000) jg        (1000)        1 2023-01-28 20:50:35.000000 fusion_solar_py-0.0.8/src/fusion_solar_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jg        (1000) jg        (1000)        9 2023-01-28 20:50:35.000000 fusion_solar_py-0.0.8/src/fusion_solar_py.egg-info/requires.txt
--rw-rw-r--   0 jg        (1000) jg        (1000)       16 2023-01-28 20:50:35.000000 fusion_solar_py-0.0.8/src/fusion_solar_py.egg-info/top_level.txt
+drwxrwxr-x   0 jg        (1000) jg        (1000)        0 2023-02-01 14:17:47.336499 fusion_solar_py-0.0.9/
+-rw-rw-r--   0 jg        (1000) jg        (1000)     1057 2022-04-01 18:22:08.000000 fusion_solar_py-0.0.9/LICENSE.txt
+-rw-rw-r--   0 jg        (1000) jg        (1000)     3371 2023-02-01 14:17:47.336499 fusion_solar_py-0.0.9/PKG-INFO
+-rw-rw-r--   0 jg        (1000) jg        (1000)     2814 2023-01-28 20:47:42.000000 fusion_solar_py-0.0.9/README.md
+-rw-rw-r--   0 jg        (1000) jg        (1000)       84 2022-04-01 18:17:20.000000 fusion_solar_py-0.0.9/pyproject.toml
+-rw-rw-r--   0 jg        (1000) jg        (1000)      685 2023-02-01 14:17:47.336499 fusion_solar_py-0.0.9/setup.cfg
+drwxrwxr-x   0 jg        (1000) jg        (1000)        0 2023-02-01 14:17:47.336499 fusion_solar_py-0.0.9/src/
+drwxrwxr-x   0 jg        (1000) jg        (1000)        0 2023-02-01 14:17:47.336499 fusion_solar_py-0.0.9/src/fusion_solar_py/
+-rw-rw-r--   0 jg        (1000) jg        (1000)        0 2022-03-29 14:27:39.000000 fusion_solar_py-0.0.9/src/fusion_solar_py/__init__.py
+-rw-rw-r--   0 jg        (1000) jg        (1000)    16021 2023-02-01 13:00:42.000000 fusion_solar_py-0.0.9/src/fusion_solar_py/client.py
+-rw-rw-r--   0 jg        (1000) jg        (1000)      442 2022-07-21 18:27:03.000000 fusion_solar_py-0.0.9/src/fusion_solar_py/exceptions.py
+drwxrwxr-x   0 jg        (1000) jg        (1000)        0 2023-02-01 14:17:47.336499 fusion_solar_py-0.0.9/src/fusion_solar_py.egg-info/
+-rw-rw-r--   0 jg        (1000) jg        (1000)     3371 2023-02-01 14:17:47.000000 fusion_solar_py-0.0.9/src/fusion_solar_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jg        (1000) jg        (1000)      356 2023-02-01 14:17:47.000000 fusion_solar_py-0.0.9/src/fusion_solar_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jg        (1000) jg        (1000)        1 2023-02-01 14:17:47.000000 fusion_solar_py-0.0.9/src/fusion_solar_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jg        (1000) jg        (1000)        9 2023-02-01 14:17:47.000000 fusion_solar_py-0.0.9/src/fusion_solar_py.egg-info/requires.txt
+-rw-rw-r--   0 jg        (1000) jg        (1000)       16 2023-02-01 14:17:47.000000 fusion_solar_py-0.0.9/src/fusion_solar_py.egg-info/top_level.txt
```

### Comparing `fusion_solar_py-0.0.8/LICENSE.txt` & `fusion_solar_py-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fusion_solar_py-0.0.8/PKG-INFO` & `fusion_solar_py-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion_solar_py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simply API to the Huawei Fusion Solar web interface.
 Home-page: https://github.com/jgriss/fusion_solar_py
 Author: Johannes Griss
 Author-email: johannes.griss@meduniwien.ac.at
 Project-URL: Bug Tracker, https://github.com/jgriss/fusion_solar_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fusion_solar_py-0.0.8/README.md` & `fusion_solar_py-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fusion_solar_py-0.0.8/setup.cfg` & `fusion_solar_py-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fusion_solar_py
-version = 0.0.8
+version = 0.0.9
 author = Johannes Griss
 author_email = johannes.griss@meduniwien.ac.at
 description = A simply API to the Huawei Fusion Solar web interface.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jgriss/fusion_solar_py
 project_urls =
```

### Comparing `fusion_solar_py-0.0.8/src/fusion_solar_py/client.py` & `fusion_solar_py-0.0.9/src/fusion_solar_py/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -121,14 +121,23 @@
 
         # get the main id
         r = self._session.get(
             url=f"https://{self._huawei_subdomain}.fusionsolar.huawei.com/rest/neteco/web/organization/v2/company/current",
             params={"_": round(time.time() * 1000)},
         )
         r.raise_for_status()
+
+        response_data = r.json()
+
+        if "data" not in response_data:
+            _LOGGER.error(f"Failed to retrieve data object. {json.dumps(response_data)}")
+            raise AuthenticationException(
+                f"Failed to login into FusionSolarAPI."
+            )
+
         self._company_id = r.json()["data"]["moDn"]
 
         # get the roarand, which is needed for non-GET requests, thus to change device settings
         r = self._session.get(
             url=f"https://{self._huawei_subdomain}.fusionsolar.huawei.com/unisess/v1/auth/session"
         )
         r.raise_for_status()
@@ -331,51 +340,51 @@
         extracted_data = {}
 
         if plant_data["existInverter"]:
             (index, value) = self._get_last_value(plant_data["productPower"])
             if index:
                 extracted_data["productPower"] = {
                     "time": measurement_times[index],
-                    "value": value,
+                    "value": float(value),
                 }
             else:
                 extracted_data["productPower"] = {
                     "time": datetime.now().strftime("%Y-%m-%d %H:%M"),
                     "value": None,
                 }
 
-            extracted_data["totalPower"] = plant_data["totalProductPower"]
+            extracted_data["totalPower"] = float(plant_data["totalProductPower"])
         else:
             extracted_data["productPower"] = {"time": None, "value": None}
             extracted_data["totalPower"] = None
 
         if plant_data["totalUsePower"] != "--":
             (index, value) = self._get_last_value(plant_data["usePower"])
             if index:
                 extracted_data["usePower"] = {
                     "time": measurement_times[index],
-                    "value": value,
+                    "value": float(value),
                 }
             else:
                 # updated data is now
                 extracted_data["usePower"] = {
                     "time": datetime.now().strftime("%Y-%m-%d %H:%M"),
                     "value": None,
                 }
 
-            extracted_data["totalUsePower"] = plant_data["totalUsePower"]
-            extracted_data["totalSelfUsePower"] = plant_data["totalSelfUsePower"]
-            extracted_data["buyPowerRatio"] = plant_data["buyPowerRatio"]
-            extracted_data["totalOnGridPower"] = plant_data["totalOnGridPower"]
+            extracted_data["totalUsePower"]     = float(plant_data["totalUsePower"])
+            extracted_data["totalSelfUsePower"] = float(plant_data["totalSelfUsePower"])
+            extracted_data["buyPowerRatio"]     = float(plant_data["buyPowerRatio"])
+            extracted_data["totalOnGridPower"]  = float(plant_data["totalOnGridPower"])
         else:
-            extracted_data["usePower"] = {"time": None, "value": None}
-            extracted_data["totalUsePower"] = None
+            extracted_data["usePower"]          = {"time": None, "value": None}
+            extracted_data["totalUsePower"]     = None
             extracted_data["totalSelfUsePower"] = None
-            extracted_data["buyPowerRatio"] = None
-            extracted_data["totalOnGridPower"] = None
+            extracted_data["buyPowerRatio"]     = None
+            extracted_data["totalOnGridPower"]  = None
 
         if plant_data["existEnergyStore"]:
             (index, value) = self._get_last_value(plant_data["chargePower"])
             if index:
                 extracted_data["chargePower"] = {
                     "time": measurement_times[index],
                     "value": value,
```

### Comparing `fusion_solar_py-0.0.8/src/fusion_solar_py.egg-info/PKG-INFO` & `fusion_solar_py-0.0.9/src/fusion_solar_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-solar-py
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simply API to the Huawei Fusion Solar web interface.
 Home-page: https://github.com/jgriss/fusion_solar_py
 Author: Johannes Griss
 Author-email: johannes.griss@meduniwien.ac.at
 Project-URL: Bug Tracker, https://github.com/jgriss/fusion_solar_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

