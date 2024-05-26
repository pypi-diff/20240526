# Comparing `tmp/pyecotrend-ista-3.0.0.tar.gz` & `tmp/pyecotrend-ista-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecotrend-ista-3.0.0.tar", last modified: Fri Jan 26 09:29:19 2024, max compression
+gzip compressed data, was "pyecotrend-ista-3.1.0.tar", last modified: Sun May 26 07:37:11 2024, max compression
```

## Comparing `pyecotrend-ista-3.0.0.tar` & `pyecotrend-ista-3.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:29:19.399070 pyecotrend-ista-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-01-26 09:29:19.399070 pyecotrend-ista-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 09:29:19.399070 pyecotrend-ista-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:29:19.399070 pyecotrend-ista-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:29:19.399070 pyecotrend-ista-3.0.0/src/pyecotrend_ista/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista/exception_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista/helper_object_de.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista/ista_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista/login_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    27448 2024-01-26 09:29:06.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista/pyecotrend_ista.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:29:19.399070 pyecotrend-ista-3.0.0/src/pyecotrend_ista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-01-26 09:29:19.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-01-26 09:29:19.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 09:29:19.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-26 09:29:19.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-26 09:29:19.000000 pyecotrend-ista-3.0.0/src/pyecotrend_ista.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:37:11.554849 pyecotrend-ista-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-26 07:37:11.554849 pyecotrend-ista-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:37:11.554849 pyecotrend-ista-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:37:11.550849 pyecotrend-ista-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:37:11.554849 pyecotrend-ista-3.1.0/src/pyecotrend_ista/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista/exception_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista/helper_object_de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista/ista_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista/login_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28110 2024-05-26 07:37:01.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista/pyecotrend_ista.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:37:11.554849 pyecotrend-ista-3.1.0/src/pyecotrend_ista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-26 07:37:11.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-26 07:37:11.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:37:11.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-26 07:37:11.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 07:37:11.000000 pyecotrend-ista-3.1.0/src/pyecotrend_ista.egg-info/top_level.txt
```

### Comparing `pyecotrend-ista-3.0.0/LICENSE` & `pyecotrend-ista-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-3.0.0/PKG-INFO` & `pyecotrend-ista-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
```

### Comparing `pyecotrend-ista-3.0.0/README.md` & `pyecotrend-ista-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-3.0.0/setup.py` & `pyecotrend-ista-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-3.0.0/src/pyecotrend_ista/__init__.py` & `pyecotrend-ista-3.1.0/src/pyecotrend_ista/__init__.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-3.0.0/src/pyecotrend_ista/const.py` & `pyecotrend-ista-3.1.0/src/pyecotrend_ista/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-VERSION = "3.0.0"
+VERSION = "3.1.0"
 
 BASE_URL = "https://api.prod.eed.ista.com/"
 ACCOUNT_URL = BASE_URL + "account"
 CONSUMPTIONS_URL = BASE_URL + "consumptions?consumptionUnitUuid="
+CONSUMPTION_UNIT_DETAILS_URL = BASE_URL + "menu"
 
 PROVIDER_URL = "https://keycloak.ista.com/realms/eed-prod/protocol/openid-connect/"
 REDIRECT_URI = "https://ecotrend.ista.de/login-redirect"
 CLIENT_ID = "ecotrend"
 SCOPE = "openid"
 RESPONSE_MODE = "fragment"
 RESPONSE_TPYE = "code"
```

### Comparing `pyecotrend-ista-3.0.0/src/pyecotrend_ista/exception_classes.py` & `pyecotrend-ista-3.1.0/src/pyecotrend_ista/exception_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Exception Class."""
+
 from __future__ import annotations
 
 from typing import Any
 
 
 class Error(Exception):
     """This is a class to catch exceptions that are thrown when trying to create a node."""
```

### Comparing `pyecotrend-ista-3.0.0/src/pyecotrend_ista/helper_object_de.py` & `pyecotrend-ista-3.1.0/src/pyecotrend_ista/helper_object_de.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dataclasses."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
 
 from dataclasses_json import DataClassJsonMixin, dataclass_json
```

### Comparing `pyecotrend-ista-3.0.0/src/pyecotrend_ista/ista_object.py` & `pyecotrend-ista-3.1.0/src/pyecotrend_ista/ista_object.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-3.0.0/src/pyecotrend_ista/login_helper.py` & `pyecotrend-ista-3.1.0/src/pyecotrend_ista/login_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Login helper file."""
+
 from __future__ import annotations
 
 import base64
 import hashlib
 import html
 import json
 import logging
```

### Comparing `pyecotrend-ista-3.0.0/src/pyecotrend_ista/pyecotrend_ista.py` & `pyecotrend-ista-3.1.0/src/pyecotrend_ista/pyecotrend_ista.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import os
 import time
 from typing import Any
 
 import requests
 
-from .const import ACCOUNT_URL, CONSUMPTIONS_URL, MAX_RETRIES, RETRY_DELAY, VERSION
+from .const import ACCOUNT_URL, CONSUMPTION_UNIT_DETAILS_URL, CONSUMPTIONS_URL, MAX_RETRIES, RETRY_DELAY, VERSION
 from .exception_classes import Error, InternalServerError, LoginError, ServerError
 from .helper_object_de import CustomRaw
 from .login_helper import LoginHelper
 
 
 class PyEcotrendIsta:
     def __init__(
@@ -567,14 +567,28 @@
                     raise Exception("Login fail, check your input!", raw["key"])
             except requests.Timeout as error:
                 self._LOGGER.debug("TimeoutError", error)
             except requests.JSONDecodeError as err:
                 self._LOGGER.debug("JSONDecodeError", err)
         return raw
 
+    def get_consumption_unit_details(self) -> dict[str, Any]:
+        """Get consumption unit details."""
+        try:
+            with self.session.get(CONSUMPTION_UNIT_DETAILS_URL, headers=self._header) as r:
+                r.raise_for_status()
+                try:
+                    return r.json()
+                except requests.JSONDecodeError as e:
+                    self._LOGGER.debug("JSONDecodeError: %s", e)
+                    raise ServerError from e
+        except (requests.RequestException, requests.Timeout) as e:
+            self._LOGGER.debug("RequestException: %s", e)
+            raise ServerError from e
+
     def getSupportCode(self) -> str | None:
         """Returns the support code associated with the instance."""
         return self._supportCode
 
     def getUA(self) -> str:
         """Set User-Agent string."""
         return (
```

### Comparing `pyecotrend-ista-3.0.0/src/pyecotrend_ista.egg-info/PKG-INFO` & `pyecotrend-ista-3.1.0/src/pyecotrend_ista.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
```

