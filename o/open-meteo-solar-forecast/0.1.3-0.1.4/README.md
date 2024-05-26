# Comparing `tmp/open_meteo_solar_forecast-0.1.3.tar.gz` & `tmp/open_meteo_solar_forecast-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_meteo_solar_forecast-0.1.3.tar", max compression
+gzip compressed data, was "open_meteo_solar_forecast-0.1.4.tar", max compression
```

## Comparing `open_meteo_solar_forecast-0.1.3.tar` & `open_meteo_solar_forecast-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.3/LICENSE
--rw-r--r--   0        0        0     3979 2024-05-26 15:30:43.288800 open_meteo_solar_forecast-0.1.3/README.md
--rw-r--r--   0        0        0     3198 2024-05-26 15:48:22.480825 open_meteo_solar_forecast-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/__init__.py
--rw-r--r--   0        0        0     1174 2024-05-26 15:32:37.183207 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/constants.py
--rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/exceptions.py
--rw-r--r--   0        0        0     4526 2024-05-26 08:17:25.493141 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/models.py
--rw-r--r--   0        0        0     8271 2024-05-26 15:46:24.090490 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
--rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/py.typed
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3979 2024-05-26 15:30:43.288800 open_meteo_solar_forecast-0.1.4/README.md
+-rw-r--r--   0        0        0     3198 2024-05-26 16:23:39.277351 open_meteo_solar_forecast-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/__init__.py
+-rw-r--r--   0        0        0     1175 2024-05-26 16:19:42.844528 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/constants.py
+-rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/exceptions.py
+-rw-r--r--   0        0        0     4526 2024-05-26 08:17:25.493141 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/models.py
+-rw-r--r--   0        0        0     8291 2024-05-26 16:22:00.280825 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
+-rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/py.typed
+-rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.4/PKG-INFO
```

### Comparing `open_meteo_solar_forecast-0.1.3/LICENSE` & `open_meteo_solar_forecast-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.3/README.md` & `open_meteo_solar_forecast-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.3/pyproject.toml` & `open_meteo_solar_forecast-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-meteo-solar-forecast"
-version = "0.1.3"
+version = "0.1.4"
 description = "Asynchronous Python client for getting forecast solar information"
 authors = ["Klaas Schoute <hello@student-techlife.com>", "Rany <rany@riseup.net>"]
 maintainers = ["Rany <rany@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rany2/open-meteo-solar-forecast"
 repository = "https://github.com/rany2/open-meteo-solar-forecast"
```

### Comparing `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/__init__.py` & `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/constants.py` & `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Constants for the solar forecast module."""
 
 # Most solar PV modules have a temperature coefficient of around -0.3%/°C to -0.5%/°C.
 # Source: https://www.eco-greenenergy.com/temperature-coefficient-of-solar-pv-module/
-ALPHA_TEMP = -0.05  # °C-1 (temperature coefficient)
+ALPHA_TEMP = -0.005  # °C-1 (temperature coefficient)
 
 # STC is an industry-wide standard to indicate the performance of PV modules
 # and specifies cell temperature of 25°C and an irradiance of 1000 W/m2.
 # Source: https://sinovoltaics.com/learning-center/quality/standard-test-conditions-stc-definition-and-problems/
 G_STC = 1000.0  # W/m2 (standard irradiance)
 TEMP_STC = 25.0  # °C (standard cell temperature)
```

### Comparing `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/exceptions.py` & `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/models.py` & `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/models.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py` & `open_meteo_solar_forecast-0.1.4/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,23 +168,24 @@
 
         def gen_power(gti: float, t_amb: float) -> int:
             """Calculate the power generated by a solar panel.
 
             Formula:
             --------
                 Tc = Ta + (NOCT - Tnoct) / Gnoct * G
-                P = Pmax * (G / Gstc) - α * (Tc - Tstc) * η
+                P = Pmax * ((G / Gstc) - α * (Tc - Tstc)) * η
                 Source:
                     - https://www.sciencedirect.com/science/article/pii/S2214157X21005244
                     - https://repositorio.uniandes.edu.co/server/api/core/bitstreams/f3e7256f-50ad-47d2-962c-77d4fef35482/content
             """
             temp_cell = t_amb + (TEMP_NOCT_CELL - TEMP_NOCT_AMB) / G_NOCT * gti
             power = (
-                peak_power * (gti / G_STC)
-                - ALPHA_TEMP * (temp_cell - TEMP_STC) * self.efficiency_factor
+                peak_power
+                * ((gti / G_STC) - ALPHA_TEMP * (temp_cell - TEMP_STC))
+                * self.efficiency_factor
             )
             return round(max(0, power))
 
         for i, time in enumerate(time_arr):
             # If any of the values are missing, skip the iteration
             if None in (gti_avg_arr[i], gti_instant_arr[i], temp_arr[i]):
                 continue
```

### Comparing `open_meteo_solar_forecast-0.1.3/PKG-INFO` & `open_meteo_solar_forecast-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-meteo-solar-forecast
-Version: 0.1.3
+Version: 0.1.4
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/rany2/open-meteo-solar-forecast
 License: MIT
 Keywords: forecast,solar,power,energy,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Rany
```

