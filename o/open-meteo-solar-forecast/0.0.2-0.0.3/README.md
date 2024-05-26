# Comparing `tmp/open_meteo_solar_forecast-0.0.2.tar.gz` & `tmp/open_meteo_solar_forecast-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_meteo_solar_forecast-0.0.2.tar", max compression
+gzip compressed data, was "open_meteo_solar_forecast-0.0.3.tar", max compression
```

## Comparing `open_meteo_solar_forecast-0.0.2.tar` & `open_meteo_solar_forecast-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.2/LICENSE
--rw-r--r--   0        0        0     3976 2024-05-26 07:11:05.183188 open_meteo_solar_forecast-0.0.2/README.md
--rw-r--r--   0        0        0     3215 2024-05-26 07:47:42.418618 open_meteo_solar_forecast-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/__init__.py
--rw-r--r--   0        0        0      686 2024-05-26 05:48:41.429914 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/constants.py
--rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/exceptions.py
--rw-r--r--   0        0        0     4526 2024-05-26 07:22:06.350425 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/models.py
--rw-r--r--   0        0        0     7871 2024-05-26 07:47:18.794884 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
--rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/py.typed
--rw-r--r--   0        0        0     5212 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3976 2024-05-26 07:11:05.183188 open_meteo_solar_forecast-0.0.3/README.md
+-rw-r--r--   0        0        0     3215 2024-05-26 07:51:34.305595 open_meteo_solar_forecast-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/__init__.py
+-rw-r--r--   0        0        0      686 2024-05-26 05:48:41.429914 open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/constants.py
+-rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/exceptions.py
+-rw-r--r--   0        0        0     4526 2024-05-26 07:50:56.058359 open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/models.py
+-rw-r--r--   0        0        0     7899 2024-05-26 07:51:29.208853 open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
+-rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/py.typed
+-rw-r--r--   0        0        0     5212 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.0.3/PKG-INFO
```

### Comparing `open_meteo_solar_forecast-0.0.2/LICENSE` & `open_meteo_solar_forecast-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.2/README.md` & `open_meteo_solar_forecast-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.2/pyproject.toml` & `open_meteo_solar_forecast-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-meteo-solar-forecast"
-version = "0.0.2"
+version = "0.0.3"
 description = "Asynchronous Python client for getting forecast solar information"
 authors = ["Klaas Schoute <hello@student-techlife.com>", "Rany <rany@riseup.net>"]
 maintainers = ["Rany <rany@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rany2/open-meteo-solar-forecast"
 repository = "https://github.com/rany2/open-meteo-solar-forecast"
```

### Comparing `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/__init__.py` & `open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/constants.py` & `open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/constants.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/exceptions.py` & `open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/models.py` & `open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Data models for the Forecast.Solar API."""
 
 from __future__ import annotations
 
-from dataclasses import dataclass
 import datetime as dt
+from dataclasses import dataclass
 
 
 def _timed_value(at: dt.datetime, data: dict[dt.datetime, int]) -> int | None:
     """Return the value for a specific time."""
     value = None
     for timestamp, cur_value in data.items():
         if timestamp > at:
```

### Comparing `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py` & `open_meteo_solar_forecast-0.0.3/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     api_key: str | None = None
     efficiency_factor: float = 1.0
 
     session: ClientSession | None = None
     _close_session: bool = False
 
     def __post_init__(self) -> None:
-        """Initialize the class."""
-        if not self.base_url:
-            self.base_url = "https://api.forecast.solar"
+        """Initialize the OpenMeteoSolarForecast object."""
+        if self.base_url is None:
+            self.base_url = "https://api.open-meteo.com"
 
     async def _request(
         self,
         uri: str,
         *,
         params: dict[str, Any] | None = None,
     ) -> Any:
```

### Comparing `open_meteo_solar_forecast-0.0.2/PKG-INFO` & `open_meteo_solar_forecast-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-meteo-solar-forecast
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/rany2/open-meteo-solar-forecast
 License: MIT
 Keywords: forecast,solar,power,energy,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Rany
```

