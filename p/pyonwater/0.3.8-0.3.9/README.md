# Comparing `tmp/pyonwater-0.3.8.tar.gz` & `tmp/pyonwater-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyonwater-0.3.8.tar", max compression
+gzip compressed data, was "pyonwater-0.3.9.tar", max compression
```

## Comparing `pyonwater-0.3.8.tar` & `pyonwater-0.3.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1072 2024-02-27 05:04:18.392179 pyonwater-0.3.8/LICENSE
--rw-r--r--   0        0        0     1271 2024-02-27 05:04:18.392179 pyonwater-0.3.8/README.md
--rw-r--r--   0        0        0      366 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/__init__.py
--rw-r--r--   0        0        0     2257 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/account.py
--rw-r--r--   0        0        0     3938 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/client.py
--rw-r--r--   0        0        0      890 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/exceptions.py
--rw-r--r--   0        0        0     3781 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/meter.py
--rw-r--r--   0        0        0     4505 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/meter_reader.py
--rw-r--r--   0        0        0      158 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/models/__init__.py
--rw-r--r--   0        0        0     3703 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/models/eow_historical_models.py
--rw-r--r--   0        0        0    13604 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/models/eow_models.py
--rw-r--r--   0        0        0      309 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/models/models.py
--rw-r--r--   0        0        0      585 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/models/units.py
--rw-r--r--   0        0        0     2502 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyonwater/units.py
--rw-r--r--   0        0        0     1908 2024-02-27 05:04:18.392179 pyonwater-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1942 1970-01-01 00:00:00.000000 pyonwater-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-03-29 17:42:18.577305 pyonwater-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1271 2024-03-29 17:42:18.577305 pyonwater-0.3.9/README.md
+-rw-r--r--   0        0        0      366 2024-03-29 17:42:18.577305 pyonwater-0.3.9/pyonwater/__init__.py
+-rw-r--r--   0        0        0     2257 2024-03-29 17:42:18.577305 pyonwater-0.3.9/pyonwater/account.py
+-rw-r--r--   0        0        0     3938 2024-03-29 17:42:18.577305 pyonwater-0.3.9/pyonwater/client.py
+-rw-r--r--   0        0        0      890 2024-03-29 17:42:18.577305 pyonwater-0.3.9/pyonwater/exceptions.py
+-rw-r--r--   0        0        0     3781 2024-03-29 17:42:18.581305 pyonwater-0.3.9/pyonwater/meter.py
+-rw-r--r--   0        0        0     4593 2024-03-29 17:42:18.581305 pyonwater-0.3.9/pyonwater/meter_reader.py
+-rw-r--r--   0        0        0      158 2024-03-29 17:42:18.581305 pyonwater-0.3.9/pyonwater/models/__init__.py
+-rw-r--r--   0        0        0     3723 2024-03-29 17:42:18.581305 pyonwater-0.3.9/pyonwater/models/eow_historical_models.py
+-rw-r--r--   0        0        0    13604 2024-03-29 17:42:18.581305 pyonwater-0.3.9/pyonwater/models/eow_models.py
+-rw-r--r--   0        0        0      309 2024-03-29 17:42:18.581305 pyonwater-0.3.9/pyonwater/models/models.py
+-rw-r--r--   0        0        0      585 2024-03-29 17:42:18.581305 pyonwater-0.3.9/pyonwater/models/units.py
+-rw-r--r--   0        0        0     2502 2024-03-29 17:42:18.581305 pyonwater-0.3.9/pyonwater/units.py
+-rw-r--r--   0        0        0     1908 2024-03-29 17:42:18.581305 pyonwater-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1942 1970-01-01 00:00:00.000000 pyonwater-0.3.9/PKG-INFO
```

### Comparing `pyonwater-0.3.8/LICENSE` & `pyonwater-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyonwater-0.3.8/README.md` & `pyonwater-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pyonwater-0.3.8/pyonwater/account.py` & `pyonwater-0.3.9/pyonwater/account.py`

 * *Files identical despite different names*

### Comparing `pyonwater-0.3.8/pyonwater/client.py` & `pyonwater-0.3.9/pyonwater/client.py`

 * *Files identical despite different names*

### Comparing `pyonwater-0.3.8/pyonwater/exceptions.py` & `pyonwater-0.3.9/pyonwater/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyonwater-0.3.8/pyonwater/meter.py` & `pyonwater-0.3.9/pyonwater/meter.py`

 * *Files identical despite different names*

### Comparing `pyonwater-0.3.8/pyonwater/meter_reader.py` & `pyonwater-0.3.9/pyonwater/meter_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,17 @@
 
         timezones = data.hit.meter_timezone
         timezone = pytz.timezone(timezones[0])
 
         ts = data.timeseries[key].series
         statistics = []
         for d in ts:
+            if d.bill_read is None or d.display_unit is None:
+                continue
+
             statistics.append(
                 DataPoint(
                     dt=timezone.localize(d.date),
                     reading=d.bill_read,
                     unit=d.display_unit,
                 ),
             )
```

### Comparing `pyonwater-0.3.8/pyonwater/models/eow_historical_models.py` & `pyonwater-0.3.9/pyonwater/models/eow_historical_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     adjust_to: Optional[bool] = None
     combine_group: Optional[bool] = None
 
 
 class Series(BaseModel):
     # Mandatory fields
     date: datetime
-    display_unit: EOWUnits
-    bill_read: float
+    display_unit: Optional[EOWUnits]
+    bill_read: Optional[float]
 
     # Optional fields
     end_date: Optional[datetime] = None
     meter_uuid: Optional[int] = None
     value: Optional[float] = None
     start_date: Optional[datetime] = None
     register_number: Optional[int] = None
```

### Comparing `pyonwater-0.3.8/pyonwater/models/eow_models.py` & `pyonwater-0.3.9/pyonwater/models/eow_models.py`

 * *Files identical despite different names*

### Comparing `pyonwater-0.3.8/pyonwater/models/units.py` & `pyonwater-0.3.9/pyonwater/models/units.py`

 * *Files identical despite different names*

### Comparing `pyonwater-0.3.8/pyonwater/units.py` & `pyonwater-0.3.9/pyonwater/units.py`

 * *Files identical despite different names*

### Comparing `pyonwater-0.3.8/pyproject.toml` & `pyonwater-0.3.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyonwater"
-version = "0.3.8"
+version = "0.3.9"
 description = "EyeOnWater client library."
 authors = []
 license = "MIT"
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pyonwater-0.3.8/PKG-INFO` & `pyonwater-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyonwater
-Version: 0.3.8
+Version: 0.3.9
 Summary: EyeOnWater client library.
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

