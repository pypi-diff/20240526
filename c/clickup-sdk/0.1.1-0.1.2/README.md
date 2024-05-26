# Comparing `tmp/clickup_sdk-0.1.1.tar.gz` & `tmp/clickup_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickup_sdk-0.1.1.tar", max compression
+gzip compressed data, was "clickup_sdk-0.1.2.tar", max compression
```

## Comparing `clickup_sdk-0.1.1.tar` & `clickup_sdk-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-01 17:03:51.711789 clickup_sdk-0.1.1/README.md
--rw-r--r--   0        0        0       74 2024-04-03 17:22:31.904183 clickup_sdk-0.1.1/clickup_sdk/__init__.py
--rw-r--r--   0        0        0     2511 2024-04-03 17:24:11.052677 clickup_sdk-0.1.1/clickup_sdk/client.py
--rw-r--r--   0        0        0     1539 2024-04-01 17:52:49.404937 clickup_sdk-0.1.1/clickup_sdk/helpers.py
--rw-r--r--   0        0        0      640 2024-04-01 22:44:23.809508 clickup_sdk-0.1.1/clickup_sdk/schemas.py
--rw-r--r--   0        0        0      196 2024-04-03 17:23:40.359050 clickup_sdk-0.1.1/clickup_sdk/settings.py
--rw-r--r--   0        0        0      326 2024-04-03 17:25:07.595146 clickup_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 clickup_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 05:21:21.182882 clickup_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0       44 2024-05-26 14:08:35.681803 clickup_sdk-0.1.2/clickup_sdk/__init__.py
+-rw-r--r--   0        0        0     3248 2024-05-26 14:47:35.219179 clickup_sdk-0.1.2/clickup_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 14:04:07.141190 clickup_sdk-0.1.2/clickup_sdk/common/__init__.py
+-rw-r--r--   0        0        0     1601 2024-05-26 14:42:15.628095 clickup_sdk-0.1.2/clickup_sdk/common/utilities.py
+-rw-r--r--   0        0        0       31 2024-05-26 14:05:44.847386 clickup_sdk-0.1.2/clickup_sdk/core/__init__.py
+-rw-r--r--   0        0        0      758 2024-05-26 14:39:03.289105 clickup_sdk-0.1.2/clickup_sdk/core/models.py
+-rw-r--r--   0        0        0      196 2024-05-26 14:05:39.307488 clickup_sdk-0.1.2/clickup_sdk/core/settings.py
+-rw-r--r--   0        0        0      346 2024-05-26 13:56:37.537591 clickup_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 clickup_sdk-0.1.2/PKG-INFO
```

### Comparing `clickup_sdk-0.1.1/clickup_sdk/helpers.py` & `clickup_sdk-0.1.2/clickup_sdk/common/utilities.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import datetime as dt
 from typing import Any
 
-from .schemas import DropDownTypeConfig
+from clickup_sdk.core import models
 
 
 def microseconds_string_to_date(
-    microseconds_string: str,
+    microseconds_string: str | None,
 ) -> dt.date | None:
+    if not microseconds_string:
+        return None
     try:
         return dt.datetime.fromtimestamp(
             timestamp=int(microseconds_string) / 1000,
             tz=dt.UTC,
         ).date()
     except ValueError:
         return None
@@ -36,13 +38,13 @@
                         ndigits=2,
                     )
                 case _:
                     custom_field_value = value
         else:
             custom_field_value = value
     elif custom_field_type == "drop_down":
-        drop_down_type_config = DropDownTypeConfig(**custom_field["type_config"])
+        drop_down_type_config = models.DropDownTypeConfig(**custom_field["type_config"])
         option: int = value if value is not None else drop_down_type_config.default
         custom_field_value = drop_down_type_config.options[option].name
     else:
         custom_field_value = value
     return custom_field_value
```

### Comparing `clickup_sdk-0.1.1/clickup_sdk/schemas.py` & `clickup_sdk-0.1.2/clickup_sdk/core/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,26 +14,33 @@
 
 
 class DropDownTypeConfig(BaseModel):
     default: int
     options: list[DropDownOption]
 
 
+class Tag(BaseModel):
+    name: str
+
+
 class CustomField(BaseModel):
     name: str
     value: str | float | dt.date | None
 
 
 class Task(BaseModel):
     id: str
     name: str
     status: str
-    date_updated: dt.date | None
-    date_created: dt.date | None
+    update_date: dt.date | None
+    creation_date: dt.date | None
+    due_date: dt.date | None
+    start_date: dt.date | None
     custom_fields: list[CustomField]
+    tags: list[Tag]
 
 
 # Parameters
 
 
 # Payloads
```

