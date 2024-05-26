# Comparing `tmp/open_meteo_solar_forecast-0.1.2.tar.gz` & `tmp/open_meteo_solar_forecast-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_meteo_solar_forecast-0.1.2.tar", max compression
+gzip compressed data, was "open_meteo_solar_forecast-0.1.3.tar", max compression
```

## Comparing `open_meteo_solar_forecast-0.1.2.tar` & `open_meteo_solar_forecast-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.2/LICENSE
--rw-r--r--   0        0        0     3977 2024-05-26 08:41:47.066511 open_meteo_solar_forecast-0.1.2/README.md
--rw-r--r--   0        0        0     3198 2024-05-26 13:16:44.381914 open_meteo_solar_forecast-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/__init__.py
--rw-r--r--   0        0        0     1048 2024-05-26 13:16:24.211885 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/constants.py
--rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/exceptions.py
--rw-r--r--   0        0        0     4526 2024-05-26 08:17:25.493141 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/models.py
--rw-r--r--   0        0        0     8129 2024-05-26 13:10:19.461385 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
--rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/py.typed
--rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3979 2024-05-26 15:30:43.288800 open_meteo_solar_forecast-0.1.3/README.md
+-rw-r--r--   0        0        0     3198 2024-05-26 15:48:22.480825 open_meteo_solar_forecast-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/__init__.py
+-rw-r--r--   0        0        0     1174 2024-05-26 15:32:37.183207 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/constants.py
+-rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/exceptions.py
+-rw-r--r--   0        0        0     4526 2024-05-26 08:17:25.493141 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/models.py
+-rw-r--r--   0        0        0     8271 2024-05-26 15:46:24.090490 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
+-rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/py.typed
+-rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.1.3/PKG-INFO
```

### Comparing `open_meteo_solar_forecast-0.1.2/LICENSE` & `open_meteo_solar_forecast-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.2/README.md` & `open_meteo_solar_forecast-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 exit
 ```
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2024 Klaas Schoute
+Copyright (c) 2021-2024 Klaas Schoute  
 Copyright (c) 2024 Rany
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `open_meteo_solar_forecast-0.1.2/pyproject.toml` & `open_meteo_solar_forecast-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-meteo-solar-forecast"
-version = "0.1.2"
+version = "0.1.3"
 description = "Asynchronous Python client for getting forecast solar information"
 authors = ["Klaas Schoute <hello@student-techlife.com>", "Rany <rany@riseup.net>"]
 maintainers = ["Rany <rany@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rany2/open-meteo-solar-forecast"
 repository = "https://github.com/rany2/open-meteo-solar-forecast"
```

### Comparing `open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/__init__.py` & `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/constants.py` & `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 # STC is an industry-wide standard to indicate the performance of PV modules
 # and specifies cell temperature of 25°C and an irradiance of 1000 W/m2.
 # Source: https://sinovoltaics.com/learning-center/quality/standard-test-conditions-stc-definition-and-problems/
 G_STC = 1000.0  # W/m2 (standard irradiance)
 TEMP_STC = 25.0  # °C (standard cell temperature)
 
 # To calculate the Nominal Operating Cell Temperature (NOCT) of a solar panel,
-# an irradiance of 800 W/m2 and a cell temperature of 20°C are used.
+# an irradiance of 800 W/m2 and a cell temperature of 20°C are used. Most cells
+# are rated at 45°C. The NOCT is used to estimate the temperature of a solar panel
+# under real-world conditions.
 # Source:
 #   - https://www.pveducation.org/pvcdrom/modules-and-arrays/nominal-operating-cell-temperature
 #   - https://www.sciencedirect.com/science/article/pii/S2214157X21005244
 G_NOCT = 800.0  # W/m2
 TEMP_NOCT_AMB = 20.0  # °C
 TEMP_NOCT_CELL = 45.0  # °C
```

### Comparing `open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/exceptions.py` & `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/models.py` & `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/models.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.1.2/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py` & `open_meteo_solar_forecast-0.1.3/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
     azimuth: float
     declination: float
     kwp: float
     latitude: float
     longitude: float
 
+    past_days: int = 92
+    forecast_days: int = 16
+
     base_url: str | None = None
     api_key: str | None = None
     efficiency_factor: float = 1.0
 
     session: ClientSession | None = None
     _close_session: bool = False
 
@@ -134,16 +137,16 @@
         """
         params = {
             "latitude": str(self.latitude),
             "longitude": str(self.longitude),
             "azimuth": str(self.azimuth),
             "tilt": str(self.declination),
             "minutely_15": "temperature_2m,global_tilted_irradiance,global_tilted_irradiance_instant",
-            "forecast_days": "16",
-            "past_days": "92",
+            "forecast_days": str(self.forecast_days),
+            "past_days": str(self.past_days),
             "timezone": "auto",
         }
         data = await self._request(
             "/v1/forecast",
             params=params,
         )
         gti_avg_arr = data["minutely_15"]["global_tilted_irradiance"]
@@ -154,33 +157,35 @@
             dt.strptime(time, "%Y-%m-%dT%H:%M").replace(
                 tzinfo=timezone(timedelta(seconds=utc_offset))
             )
             for time in data["minutely_15"]["time"]
         ]
 
         peak_power = self.kwp * 1000  # Convert kW to W
-        peak_power *= self.efficiency_factor  # Apply efficiency factor
 
         power_avg: dict[dt, int] = {}
         watts_instant: dict[dt, int] = {}
         wh_days: dict[dt, int] = {}
 
         def gen_power(gti: float, t_amb: float) -> int:
             """Calculate the power generated by a solar panel.
 
             Formula:
             --------
                 Tc = Ta + (NOCT - Tnoct) / Gnoct * G
-                P = Pmax * (G / Gstc) - α * (Tc - Tstc)
+                P = Pmax * (G / Gstc) - α * (Tc - Tstc) * η
                 Source:
                     - https://www.sciencedirect.com/science/article/pii/S2214157X21005244
-                    - https://downloads.hindawi.com/journals/ijp/2012/178175.pdf
+                    - https://repositorio.uniandes.edu.co/server/api/core/bitstreams/f3e7256f-50ad-47d2-962c-77d4fef35482/content
             """
             temp_cell = t_amb + (TEMP_NOCT_CELL - TEMP_NOCT_AMB) / G_NOCT * gti
-            power = peak_power * (gti / G_STC) - ALPHA_TEMP * (temp_cell - TEMP_STC)
+            power = (
+                peak_power * (gti / G_STC)
+                - ALPHA_TEMP * (temp_cell - TEMP_STC) * self.efficiency_factor
+            )
             return round(max(0, power))
 
         for i, time in enumerate(time_arr):
             # If any of the values are missing, skip the iteration
             if None in (gti_avg_arr[i], gti_instant_arr[i], temp_arr[i]):
                 continue
```

### Comparing `open_meteo_solar_forecast-0.1.2/PKG-INFO` & `open_meteo_solar_forecast-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-meteo-solar-forecast
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/rany2/open-meteo-solar-forecast
 License: MIT
 Keywords: forecast,solar,power,energy,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Rany
@@ -139,15 +139,15 @@
 exit
 ```
 
 ## License
 
 MIT License
 
-Copyright (c) 2021-2024 Klaas Schoute
+Copyright (c) 2021-2024 Klaas Schoute  
 Copyright (c) 2024 Rany
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

