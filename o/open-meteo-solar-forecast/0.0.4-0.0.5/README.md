# Comparing `tmp/open_meteo_solar_forecast-0.0.4.tar.gz` & `tmp/open_meteo_solar_forecast-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_meteo_solar_forecast-0.0.4.tar", max compression
+gzip compressed data, was "open_meteo_solar_forecast-0.0.5.tar", max compression
```

## Comparing `open_meteo_solar_forecast-0.0.4.tar` & `open_meteo_solar_forecast-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.4/LICENSE
--rw-r--r--   0        0        0     3976 2024-05-26 07:11:05.183188 open_meteo_solar_forecast-0.0.4/README.md
--rw-r--r--   0        0        0     3215 2024-05-26 08:11:53.304916 open_meteo_solar_forecast-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/__init__.py
--rw-r--r--   0        0        0      686 2024-05-26 05:48:41.429914 open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/constants.py
--rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/exceptions.py
--rw-r--r--   0        0        0     4559 2024-05-26 08:10:40.514709 open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/models.py
--rw-r--r--   0        0        0     7899 2024-05-26 07:51:29.208853 open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
--rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/py.typed
--rw-r--r--   0        0        0     5212 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3976 2024-05-26 07:11:05.183188 open_meteo_solar_forecast-0.0.5/README.md
+-rw-r--r--   0        0        0     3215 2024-05-26 08:18:31.883541 open_meteo_solar_forecast-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/__init__.py
+-rw-r--r--   0        0        0      686 2024-05-26 05:48:41.429914 open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/constants.py
+-rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/exceptions.py
+-rw-r--r--   0        0        0     4526 2024-05-26 08:17:25.493141 open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/models.py
+-rw-r--r--   0        0        0     7871 2024-05-26 08:18:26.876843 open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
+-rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/py.typed
+-rw-r--r--   0        0        0     5212 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.0.5/PKG-INFO
```

### Comparing `open_meteo_solar_forecast-0.0.4/LICENSE` & `open_meteo_solar_forecast-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.4/README.md` & `open_meteo_solar_forecast-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.4/pyproject.toml` & `open_meteo_solar_forecast-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-meteo-solar-forecast"
-version = "0.0.4"
+version = "0.0.5"
 description = "Asynchronous Python client for getting forecast solar information"
 authors = ["Klaas Schoute <hello@student-techlife.com>", "Rany <rany@riseup.net>"]
 maintainers = ["Rany <rany@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rany2/open-meteo-solar-forecast"
 repository = "https://github.com/rany2/open-meteo-solar-forecast"
```

### Comparing `open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/__init__.py` & `open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/constants.py` & `open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/constants.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/exceptions.py` & `open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/models.py` & `open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             if date == specific_date:
                 return production
 
         return 0
 
     def now(self) -> dt.datetime:
         """Return the current timestamp in the API timezone."""
-        return dt.datetime.now(self.api_timezone) + self.api_timezone.utcoffset(None)
+        return dt.datetime.now(tz=self.api_timezone)
 
     def peak_production_time(self, specific_date: dt.date) -> dt.datetime:
         """Return the peak time on a specific date."""
         value = max(
             (watt for date, watt in self.watts.items() if date.date() == specific_date),
             default=None,
         )
```

### Comparing `open_meteo_solar_forecast-0.0.4/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py` & `open_meteo_solar_forecast-0.0.5/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,16 @@
             params=params,
         )
         gti_avg_arr = data["minutely_15"]["global_tilted_irradiance"]
         gti_instant_arr = data["minutely_15"]["global_tilted_irradiance_instant"]
         temp_arr = data["minutely_15"]["temperature_2m"]
         utc_offset = data["utc_offset_seconds"]
         time_arr = [
-            dt.fromtimestamp(
-                mktime(strptime(time, "%Y-%m-%dT%H:%M")),
-                tz=timezone(timedelta(seconds=utc_offset)),
+            dt.strptime(time, "%Y-%m-%dT%H:%M").replace(
+                tzinfo=timezone(timedelta(seconds=utc_offset))
             )
             for time in data["minutely_15"]["time"]
         ]
 
         peak_power = self.kwp * 1000  # Convert kW to W
 
         power_avg: dict[dt, float] = {}
```

### Comparing `open_meteo_solar_forecast-0.0.4/PKG-INFO` & `open_meteo_solar_forecast-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-meteo-solar-forecast
-Version: 0.0.4
+Version: 0.0.5
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/rany2/open-meteo-solar-forecast
 License: MIT
 Keywords: forecast,solar,power,energy,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Rany
```

