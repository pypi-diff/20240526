# Comparing `tmp/open_meteo_solar_forecast-0.1.1.tar.gz` & `tmp/open_meteo_solar_forecast-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_meteo_solar_forecast-0.1.1.tar", max compression
+gzip compressed data, was "open_meteo_solar_forecast-0.1.2.tar", max compression
```

## Comparing `open_meteo_solar_forecast-0.1.1.tar` & `open_meteo_solar_forecast-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.1/LICENSE
--rw-r--r--   0        0        0     3977 2024-05-26 08:41:47.066511 open_meteo_solar_forecast-0.1.1/README.md
--rw-r--r--   0        0        0     3198 2024-05-26 08:58:26.610516 open_meteo_solar_forecast-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/__init__.py
--rw-r--r--   0        0        0      686 2024-05-26 05:48:41.429914 open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/constants.py
--rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/exceptions.py
--rw-r--r--   0        0        0     4526 2024-05-26 08:17:25.493141 open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/models.py
--rw-r--r--   0        0        0     7921 2024-05-26 08:58:04.803762 open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
--rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/py.typed
--rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3977 2024-05-26 08:41:47.066511 open_meteo_solar_forecast-0.1.2/README.md
+-rw-r--r--   0        0        0     3198 2024-05-26 13:16:44.381914 open_meteo_solar_forecast-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-26 13:16:24.211885 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/constants.py
+-rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/exceptions.py
+-rw-r--r--   0        0        0     4526 2024-05-26 08:17:25.493141 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/models.py
+-rw-r--r--   0        0        0     8129 2024-05-26 13:10:19.461385 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
+-rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/py.typed
+-rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.2/PKG-INFO
```

### Comparing `open_meteo_solar_forecast-0.1.1/LICENSE` & `open_meteo_solar_forecast-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.1/README.md` & `open_meteo_solar_forecast-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.1/pyproject.toml` & `open_meteo_solar_forecast-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-meteo-solar-forecast"
-version = "0.1.1"
+version = "0.1.2"
 description = "Asynchronous Python client for getting forecast solar information"
 authors = ["Klaas Schoute <hello@student-techlife.com>", "Rany <rany@riseup.net>"]
 maintainers = ["Rany <rany@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rany2/open-meteo-solar-forecast"
 repository = "https://github.com/rany2/open-meteo-solar-forecast"
```

### Comparing `open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/__init__.py` & `open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/exceptions.py` & `open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/models.py` & `open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/models.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.1/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py` & `open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 """Asynchronous Python client for the API."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from datetime import datetime as dt, timedelta, timezone
-from time import mktime, strptime
+from datetime import datetime as dt
+from datetime import timedelta, timezone
 from typing import Any, Self
 
-from aiohttp import BasicAuth, ClientSession
+from aiohttp import ClientSession
 
-from .constants import ALPHA_TEMP, G_STD, TEMP_STD
+from .constants import (
+    ALPHA_TEMP,
+    G_NOCT,
+    G_STC,
+    TEMP_NOCT_AMB,
+    TEMP_NOCT_CELL,
+    TEMP_STC,
+)
 from .exceptions import (
     OpenMeteoSolarForecastAuthenticationError,
     OpenMeteoSolarForecastConfigError,
     OpenMeteoSolarForecastConnectionError,
     OpenMeteoSolarForecastError,
     OpenMeteoSolarForecastRatelimitError,
     OpenMeteoSolarForecastRequestError,
@@ -153,24 +160,28 @@
         peak_power = self.kwp * 1000  # Convert kW to W
         peak_power *= self.efficiency_factor  # Apply efficiency factor
 
         power_avg: dict[dt, int] = {}
         watts_instant: dict[dt, int] = {}
         wh_days: dict[dt, int] = {}
 
-        def gen_power(gti: float, temp: float) -> int:
+        def gen_power(gti: float, t_amb: float) -> int:
             """Calculate the power generated by a solar panel.
 
             Formula:
-                PPV(t) = Ppeak(G/Gstandard) - αT (Tc - Tstandard)
-                Gstandard = 1000 W/m2, αT = 0.005°C-1, Tstandard = 25°C
-                Ppeak = max power output of PV, Tc = ambient temperature, G = radiation
+            --------
+                Tc = Ta + (NOCT - Tnoct) / Gnoct * G
+                P = Pmax * (G / Gstc) - α * (Tc - Tstc)
+                Source:
+                    - https://www.sciencedirect.com/science/article/pii/S2214157X21005244
+                    - https://downloads.hindawi.com/journals/ijp/2012/178175.pdf
             """
-            power = peak_power * (gti / G_STD) - ALPHA_TEMP * (temp - TEMP_STD)
-            return round(min(peak_power, max(0, power)))
+            temp_cell = t_amb + (TEMP_NOCT_CELL - TEMP_NOCT_AMB) / G_NOCT * gti
+            power = peak_power * (gti / G_STC) - ALPHA_TEMP * (temp_cell - TEMP_STC)
+            return round(max(0, power))
 
         for i, time in enumerate(time_arr):
             # If any of the values are missing, skip the iteration
             if None in (gti_avg_arr[i], gti_instant_arr[i], temp_arr[i]):
                 continue
 
             # Total radiation received on a tilted pane
```

### Comparing `open_meteo_solar_forecast-0.1.1/PKG-INFO` & `open_meteo_solar_forecast-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-meteo-solar-forecast
-Version: 0.1.1
+Version: 0.1.2
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/rany2/open-meteo-solar-forecast
 License: MIT
 Keywords: forecast,solar,power,energy,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Rany
```

