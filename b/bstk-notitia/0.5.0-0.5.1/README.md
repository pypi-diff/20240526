# Comparing `tmp/bstk_notitia-0.5.0.tar.gz` & `tmp/bstk_notitia-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_notitia-0.5.0.tar", max compression
+gzip compressed data, was "bstk_notitia-0.5.1.tar", max compression
```

## Comparing `bstk_notitia-0.5.0.tar` & `bstk_notitia-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1705 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/README.md
--rw-r--r--   0        0        0     1080 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/__init__.py
--rw-r--r--   0        0        0      903 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/error.py
--rw-r--r--   0        0        0     1430 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/driver.py
--rw-r--r--   0        0        0     1086 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/informant.py
--rw-r--r--   0        0        0     5702 2024-05-24 09:31:23.536636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/investigator.py
--rw-r--r--   0        0        0     2037 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/observer.py
--rw-r--r--   0        0        0     1309 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/lib/abc/reporter.py
--rw-r--r--   0        0        0     9185 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/loader.py
--rw-r--r--   0        0        0     8904 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/driver/mongodb.py
--rw-r--r--   0        0        0      565 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/driver/null.py
--rw-r--r--   0        0        0     2463 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/driver/passthrough.py
--rw-r--r--   0        0        0      745 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/informant/internal/datetime.py
--rw-r--r--   0        0        0      400 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/informant/internal/http.py
--rw-r--r--   0        0        0     1466 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/clock.py
--rw-r--r--   0        0        0     1895 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py
--rw-r--r--   0        0        0     3313 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/notitia_casereporter.py
--rw-r--r--   0        0        0     2451 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_changestream.py
--rw-r--r--   0        0        0     4011 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_collectionstream.py
--rw-r--r--   0        0        0     1434 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_record.py
--rw-r--r--   0        0        0     1460 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/tick.py
--rw-r--r--   0        0        0      697 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/echo.py
--rw-r--r--   0        0        0     3528 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/mongo_record.py
--rw-r--r--   0        0        0     4025 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/notitia_case.py
--rw-r--r--   0        0        0    10372 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/notitia.py
--rw-r--r--   0        0        0    15705 2024-05-24 09:31:23.540636 bstk_notitia-0.5.0/bstk_notitia/roster.py
--rw-r--r--   0        0        0      815 2024-05-24 09:31:38.024966 bstk_notitia-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2307 1970-01-01 00:00:00.000000 bstk_notitia-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1705 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/README.md
+-rw-r--r--   0        0        0     1080 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/__init__.py
+-rw-r--r--   0        0        0      903 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/error.py
+-rw-r--r--   0        0        0     1430 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/lib/abc/driver.py
+-rw-r--r--   0        0        0     1086 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/lib/abc/informant.py
+-rw-r--r--   0        0        0     5702 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/lib/abc/investigator.py
+-rw-r--r--   0        0        0     2037 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/lib/abc/observer.py
+-rw-r--r--   0        0        0     1309 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/lib/abc/reporter.py
+-rw-r--r--   0        0        0     9185 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/loader.py
+-rw-r--r--   0        0        0     9004 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/driver/mongodb.py
+-rw-r--r--   0        0        0      565 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/driver/null.py
+-rw-r--r--   0        0        0     2463 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/driver/passthrough.py
+-rw-r--r--   0        0        0      745 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/informant/internal/datetime.py
+-rw-r--r--   0        0        0      400 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/informant/internal/http.py
+-rw-r--r--   0        0        0     1466 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/investigator/internal/clock.py
+-rw-r--r--   0        0        0     1895 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/investigator/internal/mongo_record_processor.py
+-rw-r--r--   0        0        0     3313 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/investigator/internal/notitia_casereporter.py
+-rw-r--r--   0        0        0     2451 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/observer/internal/mongo_changestream.py
+-rw-r--r--   0        0        0     4011 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/observer/internal/mongo_collectionstream.py
+-rw-r--r--   0        0        0     1434 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/observer/internal/mongo_record.py
+-rw-r--r--   0        0        0     1460 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/observer/internal/tick.py
+-rw-r--r--   0        0        0      697 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/reporter/internal/echo.py
+-rw-r--r--   0        0        0     3528 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/reporter/internal/mongo_record.py
+-rw-r--r--   0        0        0     4025 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/modules/reporter/internal/notitia_case.py
+-rw-r--r--   0        0        0    10372 2024-05-26 09:57:45.849493 bstk_notitia-0.5.1/bstk_notitia/notitia.py
+-rw-r--r--   0        0        0    15705 2024-05-26 09:57:45.853493 bstk_notitia-0.5.1/bstk_notitia/roster.py
+-rw-r--r--   0        0        0      815 2024-05-26 09:58:02.177482 bstk_notitia-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2307 1970-01-01 00:00:00.000000 bstk_notitia-0.5.1/PKG-INFO
```

### Comparing `bstk_notitia-0.5.0/README.md` & `bstk_notitia-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/__init__.py` & `bstk_notitia-0.5.1/bstk_notitia/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/error.py` & `bstk_notitia-0.5.1/bstk_notitia/error.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/lib/abc/driver.py` & `bstk_notitia-0.5.1/bstk_notitia/lib/abc/driver.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/lib/abc/informant.py` & `bstk_notitia-0.5.1/bstk_notitia/lib/abc/informant.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/lib/abc/investigator.py` & `bstk_notitia-0.5.1/bstk_notitia/lib/abc/investigator.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/lib/abc/observer.py` & `bstk_notitia-0.5.1/bstk_notitia/lib/abc/observer.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/lib/abc/reporter.py` & `bstk_notitia-0.5.1/bstk_notitia/lib/abc/reporter.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/loader.py` & `bstk_notitia-0.5.1/bstk_notitia/loader.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/driver/mongodb.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/driver/mongodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     which provides a functional wrapper around a mongo change stream.
     """
 
     name = "MongoDB (Motor) driver"
     key = "driver/mongodb"
 
     dsn: typing.Optional[typing.AnyStr] = field(kw_only=True, default=None)
+    params: typing.Optional[typing.Dict] = field(kw_only=True, default_factory=dict)
     database: typing.Optional[typing.AnyStr] = field(kw_only=True, default=None)
     collection: typing.Optional[typing.AnyStr] = field(kw_only=True, default=None)
     connections: typing.Dict[typing.AnyStr, motor.motor_asyncio.AsyncIOMotorClient] = (
         field(init=False, default_factory=dict)
     )
 
     def __post_init__(self):
@@ -127,15 +128,15 @@
         self, dsn: typing.Optional[typing.AnyStr] = None
     ) -> motor.motor_asyncio.AsyncIOMotorClient:
         if not dsn and self.dsn:
             dsn = self.dsn
 
         if dsn not in self.connections:
             self.connections[dsn] = motor.motor_asyncio.AsyncIOMotorClient(
-                dsn, **mongod_params
+                dsn, **mongod_params, **self.params
             )
 
         return self.connections[dsn]
 
     def disconnect(self, dsn: typing.Optional[str] = None):
         if dsn:
             if dsn not in self.connections:
```

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/driver/null.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/driver/null.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/driver/passthrough.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/driver/passthrough.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/informant/internal/datetime.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/informant/internal/datetime.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/clock.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/investigator/internal/clock.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/mongo_record_processor.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/investigator/internal/mongo_record_processor.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/investigator/internal/notitia_casereporter.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/investigator/internal/notitia_casereporter.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_changestream.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/observer/internal/mongo_changestream.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_collectionstream.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/observer/internal/mongo_collectionstream.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/mongo_record.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/observer/internal/mongo_record.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/observer/internal/tick.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/observer/internal/tick.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/echo.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/reporter/internal/echo.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/mongo_record.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/reporter/internal/mongo_record.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/modules/reporter/internal/notitia_case.py` & `bstk_notitia-0.5.1/bstk_notitia/modules/reporter/internal/notitia_case.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/notitia.py` & `bstk_notitia-0.5.1/bstk_notitia/notitia.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/bstk_notitia/roster.py` & `bstk_notitia-0.5.1/bstk_notitia/roster.py`

 * *Files identical despite different names*

### Comparing `bstk_notitia-0.5.0/pyproject.toml` & `bstk_notitia-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk_notitia"
-version = "0.5.0"
+version = "0.5.1"
 description = "notitia core runtime & modules"
 authors = ["colin <colin@broadstack.com.au>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = { extras = ["cli"], version = "^1.0.0" }
```

### Comparing `bstk_notitia-0.5.0/PKG-INFO` & `bstk_notitia-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk_notitia
-Version: 0.5.0
+Version: 0.5.1
 Summary: notitia core runtime & modules
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

