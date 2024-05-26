# Comparing `tmp/open_meteo_solar_forecast-0.0.1.tar.gz` & `tmp/open_meteo_solar_forecast-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_meteo_solar_forecast-0.0.1.tar", max compression
+gzip compressed data, was "open_meteo_solar_forecast-0.0.2.tar", max compression
```

## Comparing `open_meteo_solar_forecast-0.0.1.tar` & `open_meteo_solar_forecast-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.1/LICENSE
--rw-r--r--   0        0        0     3976 2024-05-26 07:11:05.183188 open_meteo_solar_forecast-0.0.1/README.md
--rw-r--r--   0        0        0     3215 2024-05-26 07:11:28.616541 open_meteo_solar_forecast-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/__init__.py
--rw-r--r--   0        0        0      686 2024-05-26 05:48:41.429914 open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/constants.py
--rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/exceptions.py
--rw-r--r--   0        0        0     4526 2024-05-26 07:22:06.350425 open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/models.py
--rw-r--r--   0        0        0     7727 2024-05-26 07:21:32.570395 open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
--rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/py.typed
--rw-r--r--   0        0        0     5212 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3976 2024-05-26 07:11:05.183188 open_meteo_solar_forecast-0.0.2/README.md
+-rw-r--r--   0        0        0     3215 2024-05-26 07:47:42.418618 open_meteo_solar_forecast-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-05-26 07:14:47.676709 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/__init__.py
+-rw-r--r--   0        0        0      686 2024-05-26 05:48:41.429914 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/constants.py
+-rw-r--r--   0        0        0      822 2024-05-26 07:17:19.046840 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/exceptions.py
+-rw-r--r--   0        0        0     4526 2024-05-26 07:22:06.350425 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/models.py
+-rw-r--r--   0        0        0     7871 2024-05-26 07:47:18.794884 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py
+-rw-r--r--   0        0        0        0 2024-05-26 05:37:15.097554 open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/py.typed
+-rw-r--r--   0        0        0     5212 1970-01-01 00:00:00.000000 open_meteo_solar_forecast-0.0.2/PKG-INFO
```

### Comparing `open_meteo_solar_forecast-0.0.1/LICENSE` & `open_meteo_solar_forecast-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.1/README.md` & `open_meteo_solar_forecast-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.1/pyproject.toml` & `open_meteo_solar_forecast-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open-meteo-solar-forecast"
-version = "0.0.1"
+version = "0.0.2"
 description = "Asynchronous Python client for getting forecast solar information"
 authors = ["Klaas Schoute <hello@student-techlife.com>", "Rany <rany@riseup.net>"]
 maintainers = ["Rany <rany@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rany2/open-meteo-solar-forecast"
 repository = "https://github.com/rany2/open-meteo-solar-forecast"
```

### Comparing `open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/__init__.py` & `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/constants.py` & `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/constants.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/exceptions.py` & `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/exceptions.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/models.py` & `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/models.py`

 * *Files identical despite different names*

### Comparing `open_meteo_solar_forecast-0.0.1/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py` & `open_meteo_solar_forecast-0.0.2/src/open_meteo_solar_forecast/open_meteo_solar_forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,26 @@
 
     azimuth: float
     declination: float
     kwp: float
     latitude: float
     longitude: float
 
-    base_url: str = "https://api.open-meteo.com"
+    base_url: str | None = None
     api_key: str | None = None
     efficiency_factor: float = 1.0
 
     session: ClientSession | None = None
     _close_session: bool = False
 
+    def __post_init__(self) -> None:
+        """Initialize the class."""
+        if not self.base_url:
+            self.base_url = "https://api.forecast.solar"
+
     async def _request(
         self,
         uri: str,
         *,
         params: dict[str, Any] | None = None,
     ) -> Any:
         """Handle a request to the API.
```

### Comparing `open_meteo_solar_forecast-0.0.1/PKG-INFO` & `open_meteo_solar_forecast-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-meteo-solar-forecast
-Version: 0.0.1
+Version: 0.0.2
 Summary: Asynchronous Python client for getting forecast solar information
 Home-page: https://github.com/rany2/open-meteo-solar-forecast
 License: MIT
 Keywords: forecast,solar,power,energy,api,async,client
 Author: Klaas Schoute
 Author-email: hello@student-techlife.com
 Maintainer: Rany
```

