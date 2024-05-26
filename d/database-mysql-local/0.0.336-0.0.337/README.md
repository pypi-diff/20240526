# Comparing `tmp/database_mysql_local-0.0.336.tar.gz` & `tmp/database_mysql_local-0.0.337.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.336.tar", last modified: Sun May 26 06:36:17 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.337.tar", last modified: Sun May 26 11:42:25 2024, max compression
```

## Comparing `database_mysql_local-0.0.336.tar` & `database_mysql_local-0.0.337.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 06:36:17.163195 database_mysql_local-0.0.336/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    56398 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30951 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 06:35:43.000000 database_mysql_local-0.0.336/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 06:35:25.000000 database_mysql_local-0.0.336/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:42:25.212522 database_mysql_local-0.0.337/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56809 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30951 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 11:41:52.000000 database_mysql_local-0.0.337/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 11:41:34.000000 database_mysql_local-0.0.337/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/setup.py
```

### Comparing `database_mysql_local-0.0.336/PKG-INFO` & `database_mysql_local-0.0.337/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.336
+Version: 0.0.337
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.336/README.md` & `database_mysql_local-0.0.337/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.337/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.337/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.337/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.337/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.337/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,21 @@
             existing_duplicate_id = self.__get_existing_duplicate_id_with_timestamp(
                 schema_name=schema_name, table_name=table_name, duplicate_column_name=duplicate_column_name,
                 duplicate_value=duplicate_value, column_name=column_name)
         else:
             existing_duplicate_id = self.__get_existing_duplicate_id_without_timestamp(
                 schema_name=schema_name, table_name=table_name, duplicate_column_name=duplicate_column_name,
                 duplicate_value=duplicate_value, column_name=column_name)
-
+        if existing_duplicate_id is None:
+            self.logger.error(
+                f"GenericCRUD._get_existing_duplicate_id_without_timestamp: no existing row found for "
+                f"{schema_name}.{table_name}.{duplicate_column_name}={duplicate_value}",
+                object={"duplicate_column_name": duplicate_column_name, "duplicate_value": duplicate_value}
+            )
+            raise error
         self.logger.debug(object=locals())
         return existing_duplicate_id
 
     def __get_existing_duplicate_id_with_timestamp(
             self, schema_name: str, table_name: str, duplicate_column_name: str,
             duplicate_value: Any, column_name: str) -> int or None:
         select_query = (
```

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.337/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.337/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/point.py` & `database_mysql_local-0.0.337/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.337/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.337/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.337/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.337/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.337/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.337/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.337/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.336
+Version: 0.0.337
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.336/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.337/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.336/pyproject.toml` & `database_mysql_local-0.0.337/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.331" # https://pypi.org/project/database-mysql-local
+version = "0.0.338" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.336/setup.py` & `database_mysql_local-0.0.337/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.336',
+    version='0.0.337',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

