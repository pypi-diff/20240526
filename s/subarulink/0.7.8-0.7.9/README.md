# Comparing `tmp/subarulink-0.7.8.tar.gz` & `tmp/subarulink-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subarulink-0.7.8.tar", last modified: Sat Oct 28 23:39:14 2023, max compression
+gzip compressed data, was "subarulink-0.7.9.tar", last modified: Fri Nov 10 01:27:02 2023, max compression
```

## Comparing `subarulink-0.7.8.tar` & `subarulink-0.7.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-10-28 23:39:14.415575 subarulink-0.7.8/
--rw-r--r--   0 gg         (501) wheel        (0)      195 2022-02-12 17:50:33.000000 subarulink-0.7.8/AUTHORS.md
--rw-r--r--   0 gg         (501) wheel        (0)     6362 2022-03-30 01:34:05.000000 subarulink-0.7.8/DEVELOPERS.md
--rw-r--r--   0 gg         (501) wheel        (0)    11358 2020-10-11 22:38:54.000000 subarulink-0.7.8/LICENSE
--rw-r--r--   0 gg         (501) wheel        (0)       30 2022-02-12 17:49:18.000000 subarulink-0.7.8/MANIFEST.in
--rw-r--r--   0 gg         (501) wheel        (0)     8197 2023-10-28 23:39:14.415647 subarulink-0.7.8/PKG-INFO
--rw-r--r--   0 gg         (501) wheel        (0)     7591 2023-05-21 15:44:58.000000 subarulink-0.7.8/README.md
--rw-r--r--   0 gg         (501) wheel        (0)     2479 2022-12-18 23:12:31.000000 subarulink-0.7.8/pyproject.toml
--rw-r--r--   0 gg         (501) wheel        (0)      509 2023-10-28 23:39:14.415923 subarulink-0.7.8/setup.cfg
--rw-r--r--   0 gg         (501) wheel        (0)     3971 2023-10-28 22:24:02.000000 subarulink-0.7.8/setup.py
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-10-28 23:39:14.412128 subarulink-0.7.8/subarulink/
--rw-r--r--   0 gg         (501) wheel        (0)      808 2023-10-28 22:24:02.000000 subarulink-0.7.8/subarulink/__init__.py
--rw-r--r--   0 gg         (501) wheel        (0)      264 2023-10-28 22:41:33.000000 subarulink-0.7.8/subarulink/__version__.py
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-10-28 23:39:14.413715 subarulink-0.7.8/subarulink/_subaru_api/
--rw-r--r--   0 gg         (501) wheel        (0)      204 2022-12-08 02:51:09.000000 subarulink-0.7.8/subarulink/_subaru_api/__init__.py
--rw-r--r--   0 gg         (501) wheel        (0)     7265 2023-10-28 22:31:53.000000 subarulink-0.7.8/subarulink/_subaru_api/const.py
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-10-28 23:39:14.414254 subarulink-0.7.8/subarulink/app/
--rw-r--r--   0 gg         (501) wheel        (0)      219 2022-02-12 17:50:33.000000 subarulink-0.7.8/subarulink/app/__init__.py
--rw-r--r--   0 gg         (501) wheel        (0)    29784 2023-10-28 22:24:02.000000 subarulink-0.7.8/subarulink/app/cli.py
--rw-r--r--   0 gg         (501) wheel        (0)    13734 2023-10-28 22:24:02.000000 subarulink-0.7.8/subarulink/connection.py
--rw-r--r--   0 gg         (501) wheel        (0)     7460 2023-10-28 22:24:02.000000 subarulink-0.7.8/subarulink/const.py
--rw-r--r--   0 gg         (501) wheel        (0)    56948 2023-10-28 22:24:02.000000 subarulink-0.7.8/subarulink/controller.py
--rw-r--r--   0 gg         (501) wheel        (0)     1187 2020-12-24 00:13:12.000000 subarulink-0.7.8/subarulink/exceptions.py
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-10-28 23:39:14.413211 subarulink-0.7.8/subarulink.egg-info/
--rw-r--r--   0 gg         (501) wheel        (0)     8197 2023-10-28 23:39:14.000000 subarulink-0.7.8/subarulink.egg-info/PKG-INFO
--rw-r--r--   0 gg         (501) wheel        (0)      656 2023-10-28 23:39:14.000000 subarulink-0.7.8/subarulink.egg-info/SOURCES.txt
--rw-r--r--   0 gg         (501) wheel        (0)        1 2023-10-28 23:39:14.000000 subarulink-0.7.8/subarulink.egg-info/dependency_links.txt
--rw-r--r--   0 gg         (501) wheel        (0)       55 2023-10-28 23:39:14.000000 subarulink-0.7.8/subarulink.egg-info/entry_points.txt
--rw-r--r--   0 gg         (501) wheel        (0)       18 2023-10-28 23:39:14.000000 subarulink-0.7.8/subarulink.egg-info/requires.txt
--rw-r--r--   0 gg         (501) wheel        (0)       11 2023-10-28 23:39:14.000000 subarulink-0.7.8/subarulink.egg-info/top_level.txt
-drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-10-28 23:39:14.415356 subarulink-0.7.8/tests/
--rw-r--r--   0 gg         (501) wheel        (0)     4575 2023-01-21 17:52:41.000000 subarulink-0.7.8/tests/test_cli.py
--rw-r--r--   0 gg         (501) wheel        (0)    15062 2023-10-28 22:24:02.000000 subarulink-0.7.8/tests/test_connection.py
--rw-r--r--   0 gg         (501) wheel        (0)    15911 2022-12-18 20:24:35.000000 subarulink-0.7.8/tests/test_remote_commands.py
--rw-r--r--   0 gg         (501) wheel        (0)     9684 2023-01-21 17:52:41.000000 subarulink-0.7.8/tests/test_vehicle_status.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-11-10 01:27:02.694262 subarulink-0.7.9/
+-rw-r--r--   0 gg         (501) wheel        (0)      195 2022-02-12 17:50:33.000000 subarulink-0.7.9/AUTHORS.md
+-rw-r--r--   0 gg         (501) wheel        (0)     6362 2022-03-30 01:34:05.000000 subarulink-0.7.9/DEVELOPERS.md
+-rw-r--r--   0 gg         (501) wheel        (0)    11358 2020-10-11 22:38:54.000000 subarulink-0.7.9/LICENSE
+-rw-r--r--   0 gg         (501) wheel        (0)       30 2022-02-12 17:49:18.000000 subarulink-0.7.9/MANIFEST.in
+-rw-r--r--   0 gg         (501) wheel        (0)     8197 2023-11-10 01:27:02.694351 subarulink-0.7.9/PKG-INFO
+-rw-r--r--   0 gg         (501) wheel        (0)     7591 2023-05-21 15:44:58.000000 subarulink-0.7.9/README.md
+-rw-r--r--   0 gg         (501) wheel        (0)     2479 2022-12-18 23:12:31.000000 subarulink-0.7.9/pyproject.toml
+-rw-r--r--   0 gg         (501) wheel        (0)      509 2023-11-10 01:27:02.694796 subarulink-0.7.9/setup.cfg
+-rw-r--r--   0 gg         (501) wheel        (0)     3971 2023-10-28 22:24:02.000000 subarulink-0.7.9/setup.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-11-10 01:27:02.691882 subarulink-0.7.9/subarulink/
+-rw-r--r--   0 gg         (501) wheel        (0)      808 2023-10-28 22:24:02.000000 subarulink-0.7.9/subarulink/__init__.py
+-rw-r--r--   0 gg         (501) wheel        (0)      264 2023-11-10 01:10:44.000000 subarulink-0.7.9/subarulink/__version__.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-11-10 01:27:02.692943 subarulink-0.7.9/subarulink/_subaru_api/
+-rw-r--r--   0 gg         (501) wheel        (0)      204 2022-12-08 02:51:09.000000 subarulink-0.7.9/subarulink/_subaru_api/__init__.py
+-rw-r--r--   0 gg         (501) wheel        (0)     7350 2023-11-10 01:23:10.000000 subarulink-0.7.9/subarulink/_subaru_api/const.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-11-10 01:27:02.693252 subarulink-0.7.9/subarulink/app/
+-rw-r--r--   0 gg         (501) wheel        (0)      219 2022-02-12 17:50:33.000000 subarulink-0.7.9/subarulink/app/__init__.py
+-rw-r--r--   0 gg         (501) wheel        (0)    29784 2023-10-28 22:24:02.000000 subarulink-0.7.9/subarulink/app/cli.py
+-rw-r--r--   0 gg         (501) wheel        (0)    13734 2023-10-28 22:24:02.000000 subarulink-0.7.9/subarulink/connection.py
+-rw-r--r--   0 gg         (501) wheel        (0)     7460 2023-10-28 22:24:02.000000 subarulink-0.7.9/subarulink/const.py
+-rw-r--r--   0 gg         (501) wheel        (0)    57108 2023-11-10 01:24:44.000000 subarulink-0.7.9/subarulink/controller.py
+-rw-r--r--   0 gg         (501) wheel        (0)     1187 2020-12-24 00:13:12.000000 subarulink-0.7.9/subarulink/exceptions.py
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-11-10 01:27:02.692628 subarulink-0.7.9/subarulink.egg-info/
+-rw-r--r--   0 gg         (501) wheel        (0)     8197 2023-11-10 01:27:02.000000 subarulink-0.7.9/subarulink.egg-info/PKG-INFO
+-rw-r--r--   0 gg         (501) wheel        (0)      656 2023-11-10 01:27:02.000000 subarulink-0.7.9/subarulink.egg-info/SOURCES.txt
+-rw-r--r--   0 gg         (501) wheel        (0)        1 2023-11-10 01:27:02.000000 subarulink-0.7.9/subarulink.egg-info/dependency_links.txt
+-rw-r--r--   0 gg         (501) wheel        (0)       55 2023-11-10 01:27:02.000000 subarulink-0.7.9/subarulink.egg-info/entry_points.txt
+-rw-r--r--   0 gg         (501) wheel        (0)       18 2023-11-10 01:27:02.000000 subarulink-0.7.9/subarulink.egg-info/requires.txt
+-rw-r--r--   0 gg         (501) wheel        (0)       11 2023-11-10 01:27:02.000000 subarulink-0.7.9/subarulink.egg-info/top_level.txt
+drwxr-xr-x   0 gg         (501) wheel        (0)        0 2023-11-10 01:27:02.694148 subarulink-0.7.9/tests/
+-rw-r--r--   0 gg         (501) wheel        (0)     4575 2023-01-21 17:52:41.000000 subarulink-0.7.9/tests/test_cli.py
+-rw-r--r--   0 gg         (501) wheel        (0)    15062 2023-10-28 22:24:02.000000 subarulink-0.7.9/tests/test_connection.py
+-rw-r--r--   0 gg         (501) wheel        (0)    15911 2022-12-18 20:24:35.000000 subarulink-0.7.9/tests/test_remote_commands.py
+-rw-r--r--   0 gg         (501) wheel        (0)     9684 2023-01-21 17:52:41.000000 subarulink-0.7.9/tests/test_vehicle_status.py
```

### Comparing `subarulink-0.7.8/DEVELOPERS.md` & `subarulink-0.7.9/DEVELOPERS.md`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/LICENSE` & `subarulink-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/PKG-INFO` & `subarulink-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subarulink
-Version: 0.7.8
+Version: 0.7.9
 Summary: A package for interacting with Subaru Starlink Remote Services API.
 Home-page: https://github.com/G-Two/subarulink
 Author: G-Two
 Author-email: 
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `subarulink-0.7.8/README.md` & `subarulink-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/pyproject.toml` & `subarulink-0.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/setup.py` & `subarulink-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/subarulink/__init__.py` & `subarulink-0.7.9/subarulink/__init__.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/subarulink/_subaru_api/const.py` & `subarulink-0.7.9/subarulink/_subaru_api/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,18 @@
 API_WINDOW_FRONT_LEFT_STATUS = "windowFrontLeftStatus"
 API_WINDOW_FRONT_RIGHT_STATUS = "windowFrontRightStatus"
 API_WINDOW_REAR_LEFT_STATUS = "windowRearLeftStatus"
 API_WINDOW_REAR_RIGHT_STATUS = "windowRearRightStatus"
 API_WINDOW_SUNROOF_STATUS = "windowSunroofStatus"
 
 # Timestamp formats
-API_TIMESTAMP_FMT = "%Y-%m-%dT%H:%M:%S%z"  # "2020-04-25T23:35:55+0000"
+API_TIMESTAMP_FMT = "%Y-%m-%dT%H:%M:%S.%f%z"  # "2020-04-25T23:35:55.000+0000"
+API_TIMESTAMP_FMT_OLD = "%Y-%m-%dT%H:%M:%S%z"  # "2020-04-25T23:35:55+0000"
 API_VS_TIMESTAMP_FMT = "%Y-%m-%dT%H:%M%z"  # "2020-04-25T23:35+0000"
-API_POSITION_TIMESTAMP_FMT = "%Y-%m-%dT%H:%M:%SZ"  # "2020-04-25T23:35:55Z"
+API_POSITION_TIMESTAMP_FMT = "%Y-%m-%dT%H:%M:%S%fZ"  # "2020-04-25T23:35:55Z"
 
 # selectVehicle.json keys
 API_VEHICLE_ATTRIBUTES = "attributes"
 API_VEHICLE_ID = "id"
 API_VEHICLE_MODEL_NAME = "modelName"
 API_VEHICLE_MODEL_YEAR = "modelYear"
 API_VEHICLE_NAME = "nickname"
```

### Comparing `subarulink-0.7.8/subarulink/app/cli.py` & `subarulink-0.7.9/subarulink/app/cli.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/subarulink/connection.py` & `subarulink-0.7.9/subarulink/connection.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/subarulink/const.py` & `subarulink-0.7.9/subarulink/const.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/subarulink/controller.py` & `subarulink-0.7.9/subarulink/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1297,15 +1297,18 @@
             sc.DOOR_ENGINE_HOOD_POSITION: data[api.API_DOOR_ENGINE_HOOD_POSITION],
             sc.DOOR_FRONT_LEFT_POSITION: data[api.API_DOOR_FRONT_LEFT_POSITION],
             sc.DOOR_FRONT_RIGHT_POSITION: data[api.API_DOOR_FRONT_RIGHT_POSITION],
             sc.DOOR_REAR_LEFT_POSITION: data[api.API_DOOR_REAR_LEFT_POSITION],
             sc.DOOR_REAR_RIGHT_POSITION: data[api.API_DOOR_REAR_RIGHT_POSITION],
             sc.LAST_UPDATED_DATE: data[api.API_LAST_UPDATED_DATE],
         }
-        keep_data[sc.TIMESTAMP] = datetime.strptime(data[api.API_LAST_UPDATED_DATE], api.API_TIMESTAMP_FMT)
+        try:
+            keep_data[sc.TIMESTAMP] = datetime.strptime(data[api.API_LAST_UPDATED_DATE], api.API_TIMESTAMP_FMT)
+        except ValueError:
+            keep_data[sc.TIMESTAMP] = datetime.strptime(data[api.API_LAST_UPDATED_DATE], api.API_TIMESTAMP_FMT_OLD)
 
         # Only some (probably G3) vehicles properly report fuel remaining
         if data[api.API_REMAINING_FUEL_PERCENT]:
             keep_data[sc.REMAINING_FUEL_PERCENT] = data[api.API_REMAINING_FUEL_PERCENT]
 
         # Parse window/sunroof status for supported vehicles
         if await self.has_power_windows(vin) or self.has_sunroof(vin):
```

### Comparing `subarulink-0.7.8/subarulink/exceptions.py` & `subarulink-0.7.9/subarulink/exceptions.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/subarulink.egg-info/PKG-INFO` & `subarulink-0.7.9/subarulink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subarulink
-Version: 0.7.8
+Version: 0.7.9
 Summary: A package for interacting with Subaru Starlink Remote Services API.
 Home-page: https://github.com/G-Two/subarulink
 Author: G-Two
 Author-email: 
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `subarulink-0.7.8/subarulink.egg-info/SOURCES.txt` & `subarulink-0.7.9/subarulink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/tests/test_cli.py` & `subarulink-0.7.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/tests/test_connection.py` & `subarulink-0.7.9/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/tests/test_remote_commands.py` & `subarulink-0.7.9/tests/test_remote_commands.py`

 * *Files identical despite different names*

### Comparing `subarulink-0.7.8/tests/test_vehicle_status.py` & `subarulink-0.7.9/tests/test_vehicle_status.py`

 * *Files identical despite different names*

