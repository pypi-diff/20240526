# Comparing `tmp/omnijp-2.2.0.tar.gz` & `tmp/omnijp-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnijp-2.2.0.tar", last modified: Tue Feb 13 11:39:18 2024, max compression
+gzip compressed data, was "omnijp-2.3.0.tar", last modified: Sun May 26 03:53:51 2024, max compression
```

## Comparing `omnijp-2.2.0.tar` & `omnijp-2.3.0.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:18.885739 omnijp-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-13 11:39:08.000000 omnijp-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-13 11:39:18.885739 omnijp-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-13 11:39:08.000000 omnijp-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:18.885739 omnijp-2.2.0/calc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:08.000000 omnijp-2.2.0/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-13 11:39:08.000000 omnijp-2.2.0/calc/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:18.885739 omnijp-2.2.0/dbdisk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:08.000000 omnijp-2.2.0/dbdisk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-13 11:39:08.000000 omnijp-2.2.0/dbdisk/database_ps_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-13 11:39:08.000000 omnijp-2.2.0/dbdisk/database_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-13 11:39:08.000000 omnijp-2.2.0/dbdisk/db_disk_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-13 11:39:08.000000 omnijp-2.2.0/dbdisk/db_disk_cache_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-13 11:39:08.000000 omnijp-2.2.0/dbdisk/db_disk_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-13 11:39:08.000000 omnijp-2.2.0/dbdisk/db_disk_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-13 11:39:08.000000 omnijp-2.2.0/dbdisk/file_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:18.885739 omnijp-2.2.0/omnijp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-13 11:39:18.000000 omnijp-2.2.0/omnijp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-13 11:39:18.000000 omnijp-2.2.0/omnijp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 11:39:18.000000 omnijp-2.2.0/omnijp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-13 11:39:18.000000 omnijp-2.2.0/omnijp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-13 11:39:18.000000 omnijp-2.2.0/omnijp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-13 11:39:18.000000 omnijp-2.2.0/omnijp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:18.885739 omnijp-2.2.0/restq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:08.000000 omnijp-2.2.0/restq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-02-13 11:39:08.000000 omnijp-2.2.0/restq/disk_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-13 11:39:08.000000 omnijp-2.2.0/restq/http_cached_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-13 11:39:08.000000 omnijp-2.2.0/restq/http_request.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 11:39:18.885739 omnijp-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-13 11:39:08.000000 omnijp-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:18.885739 omnijp-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:08.000000 omnijp-2.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-13 11:39:08.000000 omnijp-2.2.0/tests/test_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:18.885739 omnijp-2.2.0/xmlcreator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 11:39:08.000000 omnijp-2.2.0/xmlcreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-13 11:39:08.000000 omnijp-2.2.0/xmlcreator/xml_creator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:51.001221 omnijp-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-26 03:53:37.000000 omnijp-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-26 03:53:51.001221 omnijp-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 03:53:37.000000 omnijp-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:50.997221 omnijp-2.3.0/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:37.000000 omnijp-2.3.0/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-26 03:53:37.000000 omnijp-2.3.0/calc/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:50.997221 omnijp-2.3.0/dbdisk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:50.997221 omnijp-2.3.0/dbdisk/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/caches/db_disk_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/caches/db_disk_cache_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:50.997221 omnijp-2.3.0/dbdisk/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/database/database_pg_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/database/database_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/database/database_sybase_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/db_disk_cache_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/db_disk_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/db_disk_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-26 03:53:37.000000 omnijp-2.3.0/dbdisk/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:50.997221 omnijp-2.3.0/omnijp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-26 03:53:50.000000 omnijp-2.3.0/omnijp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 03:53:50.000000 omnijp-2.3.0/omnijp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 03:53:50.000000 omnijp-2.3.0/omnijp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 03:53:50.000000 omnijp-2.3.0/omnijp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 03:53:50.000000 omnijp-2.3.0/omnijp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-26 03:53:50.000000 omnijp-2.3.0/omnijp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:51.001221 omnijp-2.3.0/restq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:37.000000 omnijp-2.3.0/restq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-26 03:53:37.000000 omnijp-2.3.0/restq/disk_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-26 03:53:37.000000 omnijp-2.3.0/restq/http_cached_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-26 03:53:37.000000 omnijp-2.3.0/restq/http_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 03:53:51.001221 omnijp-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-26 03:53:37.000000 omnijp-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:51.001221 omnijp-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:37.000000 omnijp-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-26 03:53:37.000000 omnijp-2.3.0/tests/test_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:51.001221 omnijp-2.3.0/xmlcreator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:53:37.000000 omnijp-2.3.0/xmlcreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-26 03:53:37.000000 omnijp-2.3.0/xmlcreator/xml_creator.py
```

### Comparing `omnijp-2.2.0/LICENSE` & `omnijp-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omnijp-2.2.0/dbdisk/database_ps_service.py` & `omnijp-2.3.0/dbdisk/database/database_pg_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import psycopg2
 
+from dbdisk.database.database_service import DatabaseService
 
-class DatabasePostgresService:
-    @staticmethod
-    def execute_query(connection_string, query):
+
+class DatabasePgService(DatabaseService):
+    def __init__(self, connection_string):
+        super().__init__(connection_string)
+
+    def execute(self, query):
         try:
-            connection = psycopg2.connect(connection_string)
+            connection = psycopg2.connect(self.connection_string)
             cursor = connection.cursor()
             cursor.execute(query)
 
         except psycopg2.Error as e:
-            print("Error connecting to PostgreSQL:", e)
+            print("Error connecting to PostgresSQL:", e)
 
         finally:
             header = [desc[0] for desc in cursor.description]
             return header, cursor.fetchall()
             if cursor:
                 cursor.close()
             if connection:
```

### Comparing `omnijp-2.2.0/omnijp.egg-info/SOURCES.txt` & `omnijp-2.3.0/omnijp.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 LICENSE
 README.md
 setup.py
 calc/__init__.py
 calc/calculator.py
 dbdisk/__init__.py
-dbdisk/database_ps_service.py
-dbdisk/database_service.py
-dbdisk/db_disk_cache.py
-dbdisk/db_disk_cache_csv.py
+dbdisk/db_disk_cache_builder.py
 dbdisk/db_disk_factory.py
 dbdisk/db_disk_request.py
-dbdisk/file_type.py
+dbdisk/helper.py
+dbdisk/types.py
+dbdisk/caches/__init__.py
+dbdisk/caches/db_disk_cache.py
+dbdisk/caches/db_disk_cache_csv.py
+dbdisk/database/__init__.py
+dbdisk/database/database_pg_service.py
+dbdisk/database/database_service.py
+dbdisk/database/database_sybase_service.py
 omnijp.egg-info/PKG-INFO
 omnijp.egg-info/SOURCES.txt
 omnijp.egg-info/dependency_links.txt
 omnijp.egg-info/entry_points.txt
 omnijp.egg-info/requires.txt
 omnijp.egg-info/top_level.txt
 restq/__init__.py
```

### Comparing `omnijp-2.2.0/restq/disk_cache.py` & `omnijp-2.3.0/restq/disk_cache.py`

 * *Files identical despite different names*

### Comparing `omnijp-2.2.0/restq/http_cached_request.py` & `omnijp-2.3.0/restq/http_cached_request.py`

 * *Files identical despite different names*

### Comparing `omnijp-2.2.0/restq/http_request.py` & `omnijp-2.3.0/restq/http_request.py`

 * *Files identical despite different names*

### Comparing `omnijp-2.2.0/tests/test_calculator.py` & `omnijp-2.3.0/tests/test_calculator.py`

 * *Files identical despite different names*

### Comparing `omnijp-2.2.0/xmlcreator/xml_creator.py` & `omnijp-2.3.0/xmlcreator/xml_creator.py`

 * *Files identical despite different names*

