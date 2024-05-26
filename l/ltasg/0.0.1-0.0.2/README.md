# Comparing `tmp/ltasg-0.0.1.tar.gz` & `tmp/ltasg-0.0.2.tar.gz`

## Comparing `ltasg-0.0.1.tar` & `ltasg-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ltasg-0.0.1/requirements.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ltasg-0.0.1/src/ltasg/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 ltasg-0.0.1/src/ltasg/api.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 ltasg-0.0.1/src/ltasg/constants.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ltasg-0.0.1/src/ltasg/traffic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ltasg-0.0.1/src/ltasg/transport/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 ltasg-0.0.1/src/ltasg/transport/bus.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 ltasg-0.0.1/src/ltasg/transport/taxi.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ltasg-0.0.1/src/ltasg/transport/train.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ltasg-0.0.1/src/ltasg/transport/transport.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ltasg-0.0.1/test/__init__.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ltasg-0.0.1/test/test.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ltasg-0.0.1/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ltasg-0.0.1/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ltasg-0.0.1/README.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ltasg-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 ltasg-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ltasg-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ltasg-0.0.2/src/ltasg/__init__.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 ltasg-0.0.2/src/ltasg/api.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ltasg-0.0.2/src/ltasg/constants.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ltasg-0.0.2/src/ltasg/traffic.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 ltasg-0.0.2/src/ltasg/transport/__init__.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 ltasg-0.0.2/src/ltasg/transport/bus.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 ltasg-0.0.2/src/ltasg/transport/taxi.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ltasg-0.0.2/src/ltasg/transport/train.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ltasg-0.0.2/src/ltasg/transport/transport.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ltasg-0.0.2/test/__init__.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 ltasg-0.0.2/test/test.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 ltasg-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ltasg-0.0.2/LICENSE
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ltasg-0.0.2/README.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ltasg-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 ltasg-0.0.2/PKG-INFO
```

### Comparing `ltasg-0.0.1/src/ltasg/api.py` & `ltasg-0.0.2/src/ltasg/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from aiohttp import ClientSession, ClientConnectionError
 import traceback
 class LTADataMall:
-    def __init__(self, api_key) -> None:
-        self.BASE_URL = "http://datamall2.mytransport.sg/ltaodataservice/"
+    def __init__(self, base_url, api_key) -> None:
+        self.BASE_URL = base_url
         self.API_KEY = api_key
         self.HEADERS = {
             "Accept": "application/json",
             "AccountKey": self.API_KEY
         }
 
     async def fetch(self, service_endpoint: str, query_params: dict=None, data:dict=None):
@@ -22,8 +22,8 @@
                 async with session.get(url, headers=self.HEADERS) as response:
                     if response.status == 200:
                         return await response.json()
                     else:
                         raise Exception("Error calling api for {} with status code: {}".format(
                             service_endpoint, response.status)) from None
             except ClientConnectionError as e:
-                raise e
+                raise e
```

### Comparing `ltasg-0.0.1/src/ltasg/constants.py` & `ltasg-0.0.2/src/ltasg/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 class TransportType(Enum):
     BUS = "bus"
     TRAIN = "mrt"
     TAXI = "taxi"
 
-
 LTA_SERVICES = {
     "PUBLIC_TRANSPORT_SERVICES": {
         TransportType.BUS: {
             "ARRIVAL": "BusArrivalv2",
             "SERVICES": "BusServices",
             "ROUTES": "BusRoutes",
             "STOPS": "BusStops",
```

### Comparing `ltasg-0.0.1/src/ltasg/transport/bus.py` & `ltasg-0.0.2/src/ltasg/transport/bus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from api import LTADataMall
-from transport.transport import Transport
-from constants import TransportType
+from ..transport.transport import Transport
+from ..constants import TransportType
 
 class Bus(Transport):
-    def __init__(self, api_key):
-        super().__init__(api_key)
+    def __init__(self, base_url, api_key) -> None:
+        super().__init__(base_url=base_url,api_key= api_key)
         self.bus_services = self.transport_services[TransportType.BUS]
 
     async def arrival(self, bus_stop_code: int, bus_no: int):
         data = await self.lta_api.fetch(self.bus_services['ARRIVAL'], query_params={
             "BusStopCode": bus_stop_code,
             "ServiceNo": bus_no
         })
```

### Comparing `ltasg-0.0.1/src/ltasg/transport/train.py` & `ltasg-0.0.2/src/ltasg/transport/train.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from transport.transport import Transport
-from constants import TransportType
+from ..transport.transport import Transport
+from ..constants import TransportType
 from typing import Literal
 
 class Train(Transport):
-    def __init__(self, api_key) -> None:
-        super().__init__(api_key)
+    def __init__(self, base_url, api_key) -> None:
+        super().__init__(base_url=base_url,api_key= api_key)
         self.train_services = self.transport_services[TransportType.TRAIN]
 
     async def service_alerts(self):
         data = await self.lta_api.fetch(self.train_services['SERVICE_ALERTS'])
         return data['value']
     
     # API currently results in Error 404 not found
```

### Comparing `ltasg-0.0.1/test/test.py` & `ltasg-0.0.2/test/test.py`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.1/.gitignore` & `ltasg-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.1/LICENSE` & `ltasg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ltasg-0.0.1/pyproject.toml` & `ltasg-0.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "ltasg"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Aw Sheng Xiang", email="awshengxiang@hotmail.com" },
 ]
 description = "A LTA Datamall API Wrapper Library for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+  "aiohttp >= 3.9.5"
+]
+
 [project.urls]
 Homepage = "https://github.com/ashe/ltasg"
 Issues = "https://github.com/ashe/ltasg/issues"
```

