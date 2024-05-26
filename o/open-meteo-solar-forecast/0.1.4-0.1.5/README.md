# Comparing `tmp/open_meteo_solar_forecast-0.1.4.tar.gz` & `tmp/open_meteo_solar_forecast-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_meteo_solar_forecast-0.1.4.tar", max compression
+gzip compressed data, was "open_meteo_solar_forecast-0.1.5.tar", max compression
```

## Comparing `open_meteo_solar_forecast-0.1.4.tar` & `open_meteo_solar_forecast-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.4/LICENSE
--rw-r--r--   0        0        0     3979 2024-05-26 15:30:43.288800 open_meteo_solar_forecast-0.1.4/README.md
--rw-r--r--   0        0        0     3198 2024-05-26 16:23:39.277351 open_meteo_solar_forecast-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/__init__.py
--rw-r--r--   0        0        0     1175 2024-05-26 16:19:42.844528 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/constants.py
--rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/exceptions.py
--rw-r--r--   0        0        0     4526 2024-05-26 08:17:25.493141 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/models.py
--rw-r--r--   0        0        0     8291 2024-05-26 16:22:00.280825 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
--rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/py.typed
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3979 2024-05-26 15:30:43.288800 open_meteo_solar_forecast-0.1.5/README.md
+-rw-r--r--   0        0        0     3198 2024-05-26 16:30:44.584209 open_meteo_solar_forecast-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/__init__.py
+-rw-r--r--   0        0        0     1175 2024-05-26 16:19:42.844528 open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/constants.py
+-rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/exceptions.py
+-rw-r--r--   0        0        0     4526 2024-05-26 08:17:25.493141 open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/models.py
+-rw-r--r--   0        0        0     8323 2024-05-26 16:30:00.217479 open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
+-rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/py.typed
+-rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.5/PKG-INFO
```

### Comparing `open_meteo_solar_forecast-0.1.4/LICENSE` & `open_meteo_solar_forecast-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.4/README.md` & `open_meteo_solar_forecast-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.4/pyproject.toml` & `open_meteo_solar_forecast-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-meteo-solar-forecast"
-version = "0.1.4"
+version = "0.1.5"
 description = "Asynchronous Python client for getting forecast solar information"
 authors = ["Klaas Schoute <hello@student-techlife.com>", "Rany <rany@riseup.net>"]
 maintainers = ["Rany <rany@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rany2/open-meteo-solar-forecast"
 repository = "https://github.com/rany2/open-meteo-solar-forecast"
```

### Comparing `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/__init__.py` & `open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/constants.py` & `open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/constants.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/exceptions.py` & `open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/models.py` & `open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/models.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py` & `open_meteo_solar_forecast-0.1.5/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                 continue
 
             # Total radiation received on a tilted pane
             gti_avg = gti_avg_arr[i]
             gti_instant = gti_instant_arr[i]
 
             # Get the temperature
-            temp_instant = temp_arr[i]
+            temp_instant = (temp_arr[i - 1] if i > 0 else temp_arr[i])
             temp_avg = (temp_arr[i] + temp_arr[i - 1]) / 2 if i > 0 else temp_arr[i]
 
             # For minutely data, the time_start is 15 minutes before the current time
             time_start = time - timedelta(minutes=15)
 
             # Calculate and store the power generated
             power_avg[time_start] = gen_power(gti_avg, temp_avg)
```

### Comparing `open_meteo_solar_forecast-0.1.4/PKG-INFO` & `open_meteo_solar_forecast-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-meteo-solar-forecast
-Version: 0.1.4
+Version: 0.1.5
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/rany2/open-meteo-solar-forecast
 License: MIT
 Keywords: forecast,solar,power,energy,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Rany
```

