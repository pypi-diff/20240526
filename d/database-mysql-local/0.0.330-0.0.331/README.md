# Comparing `tmp/database_mysql_local-0.0.330.tar.gz` & `tmp/database_mysql_local-0.0.331.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.330.tar", last modified: Sat May 25 15:23:53 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.331.tar", last modified: Sat May 25 23:20:02 2024, max compression
```

## Comparing `database_mysql_local-0.0.330.tar` & `database_mysql_local-0.0.331.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:23:53.857298 database_mysql_local-0.0.330/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    56240 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30519 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 15:23:16.000000 database_mysql_local-0.0.330/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 15:22:59.000000 database_mysql_local-0.0.330/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:20:02.859233 database_mysql_local-0.0.331/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56887 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 23:19:30.000000 database_mysql_local-0.0.331/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 23:19:11.000000 database_mysql_local-0.0.331/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/setup.py
```

### Comparing `database_mysql_local-0.0.330/PKG-INFO` & `database_mysql_local-0.0.331/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.330
+Version: 0.0.331
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.330/README.md` & `database_mysql_local-0.0.331/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,38 +63,38 @@
 # GenericCRUD Class
 
 The GenericCRUD class is a Python utility for simplifying common SQL database operations. It provides an easy-to-use
 interface to perform basic CRUD (Create, Read, Update, Delete) operations on database tables.
 
 ## Usage
 
-You can use either a where condition or an id_column_name and id_column_value to specify which records to
+You can use either a where condition or an column_name and column_value to specify which records to
 select/update/delete.  
 You can also specify the columns to select (default is all columns).
 
 Here's a simple example of how to use the `GenericCRUD` class:
 
 ```python
 from database_mysql_local.generic_crud import GenericCRUD
 
 # Initialize the CRUD object with your schema name and connection (or let it create a default connection).
 crud = GenericCRUD('your_database')  # if you have a cunnector object, you can pass it as a second argument
 
 # Insert a new record into a table.
 data = {'name': 'John', 'age': 30, 'city': 'New York'}
-crud.insert(table_name='my_table', data_json=data)
+crud.insert(table_name='my_table', data_dict=data)
 
-# Select records from a table using id_column_name and id_column_value.
-result = crud.select(table_name='my_table', select_clause_value="age, city", id_column_name="name",
-                     id_column_value="John", limit=10)
+# Select records from a table using column_name and column_value.
+result = crud.select(table_name='my_table', select_clause_value="age, city", column_name="name",
+                     column_value="John", limit=10)
 print(result)  # (30, 'New York')
 
 # Update records in a table using where condition.
 update_data = {'age': 31}
-crud.update(table_name='my_table', data_json=update_data, where="name='John'")
+crud.update(table_name='my_table', data_dict=update_data, where="name='John'")
 
 # Selecting all columns using where condition.
 result = crud.select(table_name='my_table', where="name='John'", limit=10)
 print(result)  # age is now 31
 
 # select one:
 result = crud.select_one(table_name='my_table')
```

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.331/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.331/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.331/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.331/database_mysql_local/src/generic_crud.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 from logger_local.MetaLogger import MetaLogger
 from user_context_remote.user_context import UserContext
 
 from .connector import Connector
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
 from .cursor import Cursor
 from .table_definition import table_definition
-from .utils import (is_end_timestamp_in_table, detect_if_is_test_data, generate_column_name,
+from .utils import (detect_if_is_test_data, generate_column_name,
                     generate_table_name, generate_view_name,
                     get_entity_type_by_table_name, get_where_params,
                     process_insert_data_dict, process_update_data_dict,
                     replace_view_with_table, validate_none_select_table_name,
                     validate_select_table_name, validate_single_clause_value,
                     where_skip_null_values, insert_is_undelete,
-                    is_end_timestamp_in_table, is_column_in_table)
+                    is_end_timestamp_in_table)
+
+printed_dep_warning = []
 
 
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
     There are 4 main functions to create, read, update, and delete data from the database.
     The rest of the functions are helper functions or wrappers around the main functions."""
 
@@ -48,28 +50,30 @@
         self.default_where = default_where
         self.is_test_data = is_test_data or detect_if_is_test_data()
         self.user_context = UserContext()
 
     def _data_json_to_dict(self, data_json: dict = None) -> dict:
         if data_json is not None:
             # We let the developers migrate quietly for a week
-            if datetime.now() > datetime(2024, 5, 25):
+            if data_json not in printed_dep_warning:
                 self.logger.warning(
                     "GenericCRUD: data_json is deprecated and scheduled to be removed by 12/06/2024, use data_dict instead. "
                     "In general, use _dict when the the typing is dict and _json when the typing is json / str.")
+                printed_dep_warning.append(data_json)
 
             return data_json
 
     def _deprecated_id_column(self, id_column_name: str, column_name: str) -> str:
         if id_column_name:
             # We let the developers migrate quietly for a week
-            if datetime.now() > datetime(2024, 5, 25):
+            if "id_column_name" not in printed_dep_warning:
                 # TODO: print the caller filename
                 self.logger.warning(
                     "GenericCRUD: id_column_name and id_column_value are deprecated and scheduled to be removed by 12/06/2024, use column_name and column_value instead.")
+                printed_dep_warning.append("id_column_name")
             return id_column_name
         return column_name
 
     def insert(self, *, schema_name: str = None, table_name: str = None, data_dict: dict = None, data_json: dict = None,
                ignore_duplicate: bool = False, commit_changes: bool = True) -> int:
         # TODO raise_if_database_raise: bool = True, insert_is_undelete
         #   get_id_of_existing_exact_match: bool = True) -> int:
@@ -136,18 +140,16 @@
 
     def insert_many(self, *, schema_name: str = None, table_name: str = None, data_dict: dict[str, list or tuple],
                     commit_changes: bool = True) -> None:
         """Inserts multiple rows into the table.
         data_dict should be in the following format: {col1: [val1, val2], col2: [val3, val4], ...}
         """
         if not data_dict:
-            error = "GenericCRUD.insert_many: data_dict is empty"
-            self.logger.error(error)
-            raise ValueError(error)
-
+            self.logger.warning("GenericCRUD.insert_many: data_dict is empty")
+            return
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
 
         self._validate_args(args=locals())
         # TODO: I am not sure we can use process_insert_data_dict here
 
         len_rows = len(next(v for v in data_dict.values()))
@@ -306,17 +308,18 @@
             schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=column_value,
             data_dict={"end_timestamp": None}, commit_changes=True)
 
     def update_by_id(
             self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int or None:
-        if datetime.now() > datetime(2024, 5, 25):
+        if "update_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.update_by_id is deprecated, use update_by_column_and_value instead.")
+            printed_dep_warning.append("update_by_id")
         updated_id = self.update_by_column_and_value(
             schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=column_value,
             id_column_name=id_column_name, id_column_value=id_column_value, data_dict=data_dict, data_json=data_json,
             limit=limit, order_by=order_by, commit_changes=commit_changes)
         return updated_id
 
     def update_by_column_and_value(
@@ -376,17 +379,18 @@
             self.connection.commit()
         last_row_id = self.cursor.lastrowid()
         return last_row_id
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
                      column_name: str = None, column_value: Any = None,
                      id_column_name: str = None, id_column_value: Any = None) -> int:
-        if datetime.now() > datetime(2024, 5, 25):
+        if "delete_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.delete_by_id is deprecated, use delete_by_column_and_value instead.")
+            printed_dep_warning.append("delete_by_id")
         affected_rows = self.delete_by_column_and_value(schema_name=schema_name, table_name=table_name,
                                                         column_name=column_name, column_value=column_value,
                                                         id_column_name=id_column_name, id_column_value=id_column_value)
         return affected_rows
 
     def delete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None,
                                    column_name: str = None, column_value: Any = None,
@@ -475,17 +479,18 @@
 
     # TODO: test distinct
     def select_one_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                select_clause_value: str = None,
                                column_name: str = None, column_value: Any = None,
                                id_column_name: str = None, id_column_value: Any = None,
                                distinct: bool = False, order_by: str = "") -> tuple:
-        if datetime.now() > datetime(2024, 5, 25):
+        if "select_one_tuple_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_one_tuple_by_id is deprecated, use select_one_tuple_by_column_and_value instead.")
+            printed_dep_warning.append("select_one_tuple_by_id")
         result = self.select_one_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by)
         return result
 
     def select_one_tuple_by_column_and_value(
@@ -503,17 +508,18 @@
         else:
             return tuple()  # or None?
 
     def select_one_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "") -> dict:
-        if datetime.now() > datetime(2024, 5, 25):
+        if "select_one_dict_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_one_dict_by_id is deprecated, use select_one_dict_by_column_and_value instead.")
+            printed_dep_warning.append("select_one_dict_by_id")
         result = self.select_one_dict_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by)
         return result
 
     def select_one_dict_by_column_and_value(
@@ -529,17 +535,18 @@
         result = self.convert_to_dict(row=result, select_clause_value=select_clause_value)
         return result
 
     def select_one_value_by_id(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
-        if datetime.now() > datetime(2024, 5, 25):
+        if "select_one_value_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_one_value_by_id is deprecated, use select_one_value_by_column_and_value instead.")
+            printed_dep_warning.append("select_one_value_by_id")
         result = self.select_one_value_by_column_and_value(
             select_clause_value=select_clause_value, schema_name=schema_name, view_table_name=view_table_name,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by, skip_null_values=skip_null_values)
         return result
 
     def select_one_value_by_column_and_value(
@@ -597,17 +604,18 @@
             return result[0]
 
     def select_multi_value_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
-        if datetime.now() > datetime(2024, 5, 25):
+        if "select_multi_value_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_multi_value_by_id is deprecated, use select_multi_value_by_column_and_value instead.")
+            printed_dep_warning.append("select_multi_value_by_id")
         result = self.select_multi_value_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by,
             skip_null_values=skip_null_values)
         return result
 
@@ -641,17 +649,18 @@
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
 
     def select_multi_tuple_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
-        if datetime.now() > datetime(2024, 5, 25):
+        if "select_multi_tuple_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_multi_tuple_by_id is deprecated, use select_multi_tuple_by_column_and_value instead.")
+            printed_dep_warning.append("select_multi_tuple_by_id")
         result = self.select_multi_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_tuple_by_column_and_value(
@@ -680,17 +689,18 @@
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
-        if datetime.now() > datetime(2024, 5, 25):
+        if "select_multi_dict_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_multi_dict_by_id is deprecated, use select_multi_dict_by_column_and_value instead.")
+            printed_dep_warning.append("select_multi_dict_by_id")
         result = self.select_multi_dict_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_dict_by_column_and_value(
```

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.331/database_mysql_local/src/generic_crud_ml.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,24 +184,24 @@
         try:
             self.cursor = self.connection.cursor()
             if is_main is not None:
                 if is_main:
                     self._update_old_main_value_to_false(schema_name=schema_name, table_name=table_name,
                                                          table_id=table_id)
                 if data_dict:
-                    self.update_by_id(schema_name=schema_name, table_name=table_name, column_name=column_name,
+                    self.update_by_column_and_value(schema_name=schema_name, table_name=table_name, column_name=column_name,
                                       column_value=table_id, data_dict=data_dict, limit=limit, order_by=order_by,
                                       commit_changes=False)
                 data_ml_dict[self.is_main_column_name] = is_main
 
             data_ml_dict[column_name] = table_id
             data_ml_dict["lang_code"] = lang_code_str
             column_name = generate_column_name(ml_table_name)
 
-            self.update_by_id(schema_name=schema_name, table_name=ml_table_name, data_dict=data_ml_dict,
+            self.update_by_column_and_value(schema_name=schema_name, table_name=ml_table_name, data_dict=data_ml_dict,
                               column_name=column_name, column_value=ml_table_id, limit=limit, order_by=order_by,
                               commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
             self.connection.rollback()
             raise e
```

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.331/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/point.py` & `database_mysql_local-0.0.331/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.331/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.331/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         schema_name = schema_name or self.default_schema_name
         view_table_name = view_table_name or self.default_view_table_name
         column_name = id_column_name or column_name or self.default_column_name
         column_value = column_value or id_column_value
         if not view_table_name or not column_name or not schema_name:
             self.logger.error("view_table_name, id_column_name or schema was not provided")
             return "error"  # TODO: why not raise?
-        local_updated_timestamp = self.select_one_value_by_id(
+        local_updated_timestamp = self.select_one_value_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value)
         remote_last_modified_timestamp: datetime = datetime.strptime(remote_last_modified_timestamp,
                                                                      '%Y-%m-%d %H:%M:%S')
         if local_updated_timestamp is None or remote_last_modified_timestamp > local_updated_timestamp:
             return UpdateStatus.UPDATE_CIRCLEZ
         elif remote_last_modified_timestamp < local_updated_timestamp:
```

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.331/database_mysql_local/src/table_columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "start_timestamp",
         "end_timestamp"
     ),
     "activity_group_location_occurrence_profile_table": (
-        "id",
+        "activity_group_location_occurrence_profile_id",
         "activity_id",
         "activity_list_id",
         "group_id",
         "group_list_id",
         "location_id",
         "location_list_id",
         "occurrence_id",
@@ -1506,50 +1506,24 @@
         "updated_effective_profile_id"
     ),
     "contact_user_external_view": (
         "contact_user_external_id",
         "contact_id",
         "user_external_id"
     ),
-    "criteria_general_view": (
-        "criteria_id",
-        "criteria_name",
-        "entity_type_id",
-        "entity_type.name",
-        "entity_type.title",
-        "min_age",
-        "max_age",
-        "group_list_id",
-        "group_list.name",
-        "gender_list_id",
-        "name",
-        "location_id",
-        "title"
-    ),
     "criteria_set_general_view": (
         "parent_criteria_set_id",
         "parent_name",
         "child_criteria_set_id",
         "child_name",
         "criteria_id",
         "name",
         "entity_type_id",
         "entity_type_name",
-        "min_age",
-        "max_age",
         "group_list_id",
-        "min_number_of_kids",
-        "max_number_of_kids",
-        "min_kids_age",
-        "max_kids_age",
-        "gender_list_id",
-        "min_height",
-        "max_height",
-        "partner_experience_level",
-        "number_of_partners",
         "location_id",
         "location_list_id",
         "coordinate",
         "radius",
         "radius_measure",
         "radius_km",
         "job_group_list_id",
@@ -1586,30 +1560,38 @@
     "criteria_set_table": (
         "criteria_set_id",
         "name",
         "condition_type_id",
         "include_exclude_type_id",
         "criteria_id"
     ),
+    "criteria_set_view": (
+        "criteria_set_id",
+        "name",
+        "condition_type_id",
+        "include_exclude_type_id",
+        "criteria_id"
+    ),
     "criteria_table": (
         "criteria_id",
         "name",
         "entity_type_id",
-        "min_age",
-        "max_age",
+        "min_age_old",
+        "max_age_old",
+        "group_id",
         "group_list_id",
-        "min_number_of_kids",
-        "max_number_of_kids",
-        "min_kids_age",
-        "max_kids_age",
-        "gender_list_id",
-        "min_height",
-        "max_height",
-        "partner_experience_level",
-        "number_of_partners",
+        "min_number_of_kids_old",
+        "max_number_of_kids_old",
+        "min_kids_age_old",
+        "max_kids_age_old",
+        "gender_list_id_old",
+        "min_height_old",
+        "max_height_old",
+        "partner_experience_level_old",
+        "number_of_partners_old",
         "location_id",
         "location_list_id",
         "coordinate",
         "radius",
         "radius_measure",
         "radius_km",
         "job_group_list_id",
@@ -1628,34 +1610,25 @@
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "internet_domain_id",
         "internet_domain_list_id",
         "organization_name",
-        "group_id",
         "profile_list_id",
-        "international_code"
+        "international_code",
+        "country_id",
+        "county_id",
+        "label_id"
     ),
     "criteria_view": (
         "criteria_id",
         "name",
         "entity_type_id",
-        "min_age",
-        "max_age",
         "group_list_id",
-        "min_number_of_kids",
-        "max_number_of_kids",
-        "min_kids_age",
-        "max_kids_age",
-        "gender_list_id",
-        "min_height",
-        "max_height",
-        "partner_experience_level",
-        "number_of_partners",
         "location_id",
         "location_list_id",
         "coordinate",
         "radius",
         "radius_measure",
         "radius_km",
         "job_group_list_id",
@@ -1678,14 +1651,70 @@
         "internet_domain_id",
         "internet_domain_list_id",
         "organization_name",
         "group_id",
         "profile_list_id",
         "international_code"
     ),
+    "criteria_profile_table": (
+        "criteria_profile_id",
+        "number",
+        "identifier",
+        "batch_timestamp",
+        "criteria_id",
+        "profile_id",
+        "visibility_id",
+        "is_approved",
+        "is_test_data",
+        "created_timestamp",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id"
+    ),
+    "criteria_profile_view": (
+        "criteria_profile_id",
+        "number",
+        "identifier",
+        "batch_timestamp",
+        "criteria_id",
+        "profile_id",
+        "visibility_id",
+        "is_approved",
+        "is_test_data",
+        "created_timestamp",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id"
+    ),
+    "criteria_set_profile_table": (
+        "criteria_set_profile_id",
+        "number",
+        "identifier",
+        "batch_timestamp",
+        "criteria_set_id",
+        "profile_id",
+        "visibility_id",
+        "is_test_data",
+        "created_timestamp",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id"
+    ),
     "criteria_promotional_message_to_person_table": (
         "criteria_promotional_message_to_person_id",
         "criteria_id",
         "multiply_from_yesterday",
         "promotional_message_to_person_id",
         "created_timestamp",
         "created_user_id",
@@ -1903,15 +1932,16 @@
         "is_graph",
         "is_metrics",
         "is_visibility",
         "is_pii",
         "is_sensative",
         "sensative_columns",
         "description",
-        "end_timestamp"
+        "end_timestamp",
+        "insert_is_undelete"
     ),
     "table_definition_view": (
         "table_definition_id",
         "entity_type_id1",
         "entity_type_id2",
         "schema",
         "table_name",
@@ -2315,15 +2345,16 @@
         "criteria_view_name",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
-        "updated_user_id"
+        "updated_user_id",
+        "view_with_deleted_and_test_data"
     ),
     "entity_type_view": (
         "entity_type_id",
         "name",
         "system_id",
         "is_item_type",
         "schema_name",
@@ -3728,28 +3759,14 @@
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "start_timestamp",
         "end_timestamp"
     ),
-    "importer_recent_contact_phone_view": (
-        "created_timestamp",
-        "importer_id",
-        "data_source_type.title",
-        "importer_country_name",
-        "entity_type.title",
-        "entity_id",
-        "first_name",
-        "last_name",
-        "number_original",
-        "local_number_normalized",
-        "label.name",
-        "label_phone_ml.title"
-    ),
     "importer_recent_view": (
         "created_timestamp",
         "importer_id",
         "data_source_type.title",
         "importer_country_name",
         "entity_type_id",
         "entity_type_ml.title",
@@ -3912,21 +3929,22 @@
     ),
     "label_ml_table": (
         "label_ml_id",
         "label_id",
         "lang_code",
         "title",
         "is_title_approved",
+        "is_main",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
-        "is_main"
+        "is_test_data"
     ),
     "label_profile_table_old": (
         "id",
         "label_id",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
@@ -3944,14 +3962,15 @@
         "label_id",
         "number",
         "is_approved",
         "name",
         "name_approved",
         "parent_label_id",
         "location_id",
+        "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id"
     ),
@@ -4042,15 +4061,15 @@
         "number",
         "identifier",
         "country_id",
         "country_id_old",
         "lang_code",
         "is_main",
         "title",
-        "title_approved",
+        "is_title_approved",
         "visibility_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "created_real_user_id",
@@ -4060,52 +4079,51 @@
         "updated_user_id",
         "updated_real_user_id",
         "updated_effective_user_id",
         "updated_effective_profile_id"
     ),
     "country_ml_view": (
         "country_id",
-        "coordiante",
+        "coordinate",
         "iso",
         "name",
         "nicename",
         "iso3",
         "numcode",
         "phonecode",
         "lang_code",
         "title",
-        "title_approved"
+        "is_title_approved"
     ),
     "country_table": (
         "country_id",
         "country_id_old",
-        "number",
         "identifier",
         "coordinate",
         "iso",
         "name",
         "nicename",
         "iso3",
         "numcode",
         "phonecode",
         "group_id",
-        "id_temp",
+        "is_test_data",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id"
     ),
     "county_ml_general_view": (
         "county_ml_id",
         "number",
         "identifier",
         "county_id",
         "lang_code",
         "title",
-        "title_approved",
+        "is_title_approved",
         "visibility_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "created_real_user_id",
@@ -4120,15 +4138,15 @@
     "county_ml_table": (
         "county_ml_id",
         "number",
         "identifier",
         "county_id",
         "lang_code",
         "title",
-        "title_approved",
+        "is_title_approved",
         "visibility_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "created_real_user_id",
@@ -4142,40 +4160,66 @@
     ),
     "county_ml_view": (
         "county_id",
         "state_id",
         "coordinate",
         "lang_code",
         "title",
-        "title_approved"
+        "is_title_approved"
+    ),
+    "county_ml_with_deleted_and_test_data_view": (
+        "county_ml_id",
+        "number",
+        "identifier",
+        "county_id",
+        "lang_code",
+        "title",
+        "is_title_approved",
+        "visibility_id",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id",
+        "state_id"
     ),
     "county_table": (
         "county_id",
+        "number",
         "state_id",
         "country_id",
         "name",
         "coordinate",
         "group_id",
+        "is_test_data",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
-        "number",
-        "is_test_data"
+        "end_timestamp"
     ),
     "location_criteria_table": (
         "criteria_id",
         "state_id",
         "country_id",
         "county_id",
         "city_id",
         "neighbourhood_id",
         "street_id",
         "location_id",
-        "location_list_id"
+        "location_list_id",
+        "city_list_id"
     ),
     "location_field_ml_table": (
         "locaton_field_ml_id",
         "location_id",
         "field_name",
         "prime",
         "lang_code",
@@ -4207,26 +4251,27 @@
         "start_timestamp",
         "end_timestamp",
         "country_name",
         "state_name",
         "city_name"
     ),
     "location_list_member_table": (
-        "id",
+        "location_list_member_id",
         "location_list_id",
         "location_id",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "start_timestamp",
         "end_timestamp"
     ),
     "location_list_table": (
-        "id",
+        "location_list_id",
+        "name",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "start_timestamp",
         "end_timestamp"
     ),
@@ -4362,14 +4407,28 @@
     "neighborhood_ml_view": (
         "neighborhood_id",
         "city_id",
         "lang_code",
         "title",
         "end_timestamp"
     ),
+    "neighborhood_ml_with_deleted_and_test_data_view": (
+        "neighborhood_ml_id",
+        "neighborhood_id",
+        "lang_code",
+        "is_main",
+        "title",
+        "title_approved",
+        "created_timestamp",
+        "created_user_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "is_test_data",
+        "city_id"
+    ),
     "neighborhood_table": (
         "neighborhood_id",
         "number",
         "city_id",
         "coordinate",
         "group_id",
         "is_test_data",
@@ -4406,14 +4465,27 @@
     ),
     "region_ml_view": (
         "region_id",
         "country_id",
         "lang_code",
         "title"
     ),
+    "region_ml_with_deleted_and_test_data_view": (
+        "region_ml_id",
+        "region_id",
+        "lang_code",
+        "title",
+        "title_approved",
+        "created_timestamp",
+        "created_user_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "is_test_data",
+        "country_id"
+    ),
     "region_table": (
         "region_id",
         "country_id",
         "coordinate",
         "group_id",
         "created_timestamp",
         "created_user_id",
@@ -4448,15 +4520,87 @@
         "country_id",
         "coordinate",
         "group_id",
         "is_test_data",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
-        "updated_user_id"
+        "updated_user_id",
+        "end_timestmap"
+    ),
+    "location_profile_general_view": (
+        "location_id",
+        "name",
+        "number",
+        "identifier",
+        "coordinate",
+        "address_local_language",
+        "address_english",
+        "neighborhood_id",
+        "county_id",
+        "city_id",
+        "region_id",
+        "state_id",
+        "country_id",
+        "postal_code",
+        "plus_code",
+        "is_approved",
+        "is_community_active",
+        "group_id",
+        "visibility_id",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id",
+        "profile_id"
+    ),
+    "location_profile_label_general_view": (
+        "location_id",
+        "name",
+        "number",
+        "identifier",
+        "coordinate",
+        "address_local_language",
+        "address_english",
+        "neighborhood_id",
+        "county_id",
+        "city_id",
+        "region_id",
+        "state_id",
+        "country_id",
+        "postal_code",
+        "plus_code",
+        "is_approved",
+        "is_community_active",
+        "group_id",
+        "visibility_id",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id",
+        "profile_id",
+        "label_id"
     ),
     "location_profile_ml_table": (
         "location_profile_ml_id",
         "location_profile_id",
         "lang_code",
         "title",
         "title_approved",
@@ -6477,26 +6621,15 @@
         "updated_effective_user_id",
         "updated_effective_profile_id"
     ),
     "people_criteria_general_view": (
         "criteria_id",
         "name",
         "entity_type_id",
-        "min_age_old",
-        "max_age_old",
         "group_list_id",
-        "min_number_of_kids_old",
-        "max_number_of_kids_old",
-        "min_kids_age_old",
-        "max_kids_age_old",
-        "gender_list_id_old",
-        "min_height_old",
-        "max_height_old",
-        "partner_experience_level_old",
-        "number_of_partners_old",
         "location_id",
         "location_list_id",
         "coordinate",
         "radius",
         "radius_measure",
         "radius_km",
         "job_group_list_id_old",
@@ -6549,15 +6682,17 @@
         "international_code",
         "people_criteria.is_test_data",
         "people_criteria.start_timestamp",
         "people_criteria.end_timestamp",
         "people_criteria.created_timestamp",
         "people_criteria.created_user_id",
         "people_criteria.updated_timestamp",
-        "people_criteria.updated_user_id"
+        "people_criteria.updated_user_id",
+        "country_id",
+        "label_id"
     ),
     "people_criteria_table": (
         "criteria_id",
         "name",
         "min_age",
         "max_age",
         "min_number_of_kids",
@@ -6619,14 +6754,15 @@
         "first_name",
         "last_name",
         "main_email_person",
         "person_is_test_data",
         "person_created_timestamp",
         "person_end_timestamp",
         "person_profile_end_timestamp",
+        "person_birthday_date",
         "profile_id",
         "profile_main_email_address",
         "profile_name",
         "user_id",
         "profile_main_email",
         "profile_is_test_data",
         "profile_end_timestamp",
@@ -6694,49 +6830,51 @@
         "profile_is_test_data",
         "profile_end_timestamp"
     ),
     "person_table": (
         "person_id",
         "number",
         "identifier",
+        "name",
         "is_approved",
         "is_identity_confirmed",
         "birthday_original",
         "birthday_timestamp",
         "birthday_date",
         "day",
         "month",
         "year",
         "year_cira",
         "gender_id",
         "first_name",
-        "first_name_approved",
+        "is_first_name_approved",
         "nickname",
-        "nickname_approved",
+        "is_nickname_approved",
         "father_name",
         "last_name",
         "main_email_person",
+        "main_full_number_normalized",
         "last_coordinate",
         "last_location_id",
         "location_id",
         "is_rip",
+        "visibility_id",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "created_real_user_id",
         "created_effective_user_id",
         "created_effective_profile_id",
         "updated_timestamp",
         "updated_user_id",
         "updated_real_user_id",
         "updated_effective_user_id",
-        "updated_effective_profile_id",
-        "visibility_id"
+        "updated_effective_profile_id"
     ),
     "person_user_profile_view": (
         "person_id",
         "person_first_name",
         "person_is_approve",
         "user_id",
         "user_created_timestamp",
@@ -6747,54 +6885,14 @@
         "profile_id",
         "is_main",
         "profile_preferred_lang_code",
         "profile stars",
         "brand_id",
         "login_timestamp"
     ),
-    "person_view": (
-        "person_id",
-        "number",
-        "identifier",
-        "is_approved",
-        "is_identity_confirmed",
-        "birthday_original",
-        "birthday_timestamp",
-        "birthday_date",
-        "day",
-        "month",
-        "year",
-        "year_cira",
-        "gender_id",
-        "first_name",
-        "first_name_approved",
-        "nickname",
-        "nickname_approved",
-        "father_name",
-        "last_name",
-        "main_email_person",
-        "last_coordinate",
-        "last_location_id",
-        "location_id",
-        "is_rip",
-        "is_test_data",
-        "start_timestamp",
-        "end_timestamp",
-        "created_timestamp",
-        "created_user_id",
-        "created_real_user_id",
-        "created_effective_user_id",
-        "created_effective_profile_id",
-        "updated_timestamp",
-        "updated_user_id",
-        "updated_real_user_id",
-        "updated_effective_user_id",
-        "updated_effective_profile_id",
-        "visibility_id"
-    ),
     "person_profile_table": (
         "person_profile_id",
         "number",
         "identifier",
         "person_id",
         "profile_id",
         "person_profile_role_id",
@@ -7138,15 +7236,15 @@
         "is_approved",
         "profile_type_id",
         "preferred_lang_code",
         "experience_years_min",
         "main_phone_id",
         "profile_main_email",
         "is_rip",
-        "gender_id",
+        "profile_gender_id",
         "stars",
         "last_dialog_workflow_state_id",
         "is_system",
         "internal_description",
         "is_test_data",
         "start_timestamp",
         "end_timestamp",
@@ -7318,48 +7416,14 @@
         "updated_user_id"
     ),
     "profile_ml_view": (
         "profile_id",
         "lang_code",
         "title"
     ),
-    "profile_recent_general_view": (
-        "profile_id",
-        "number",
-        "profile_name",
-        "user_id",
-        "person_id",
-        "is_main",
-        "visibility_id",
-        "is_approved",
-        "profile_type_id",
-        "preferred_lang_code",
-        "experience_years_min",
-        "main_phone_id",
-        "profile_main_email",
-        "is_rip",
-        "gender_id",
-        "stars",
-        "last_dialog_workflow_state_id",
-        "is_system",
-        "internal_description",
-        "is_test_data",
-        "start_timestamp",
-        "end_timestamp",
-        "created_timestamp",
-        "created_user_id",
-        "updated_timestamp",
-        "updated_user_id",
-        "title",
-        "profile_ml.title",
-        "person_id_in_profile_table",
-        "person_id_in_person_table",
-        "person_first_name",
-        "person_last_name"
-    ),
     "profile_table": (
         "profile_id",
         "number",
         "identifier",
         "name",
         "user_id",
         "person_id",
@@ -7749,14 +7813,19 @@
         "lang_code"
     ),
     "profile_storage_type_table": (
         "profile_storage_type_id",
         "name",
         "file_type_id"
     ),
+    "profile_storage_view": (
+        "profile_storage_id",
+        "profile_id",
+        "storage_id"
+    ),
     "profile_text_block_table": (
         "profile_text_block_id",
         "number",
         "identifier",
         "profile_id",
         "text_block_id",
         "is_test_data",
@@ -8485,14 +8554,76 @@
         "start_timestamp",
         "end_timestamp",
         "created_timestamp",
         "created_user_id",
         "updated_timestamp",
         "updated_user_id"
     ),
+    "test_county_ml_table": (
+        "county_ml_id",
+        "number",
+        "identifier",
+        "county_id",
+        "lang_code",
+        "title",
+        "is_title_approved",
+        "visibility_id",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id"
+    ),
+    "test_county_ml_with_deleted_and_test_data_view": (
+        "county_ml_id",
+        "number",
+        "identifier",
+        "county_id",
+        "lang_code",
+        "title",
+        "is_title_approved",
+        "visibility_id",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp",
+        "created_timestamp",
+        "created_user_id",
+        "created_real_user_id",
+        "created_effective_user_id",
+        "created_effective_profile_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "updated_real_user_id",
+        "updated_effective_user_id",
+        "updated_effective_profile_id",
+        "state_id"
+    ),
+    "test_county_table": (
+        "county_id",
+        "number",
+        "state_id",
+        "country_id",
+        "name",
+        "coordinate",
+        "group_id",
+        "is_test_data",
+        "created_timestamp",
+        "created_user_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "end_timestamp"
+    ),
     "test_location_profile_ml_table": (
         "test_location_profile_ml_id",
         "test_location_profile_id",
         "lang_code",
         "title",
         "title_approved"
     ),
@@ -8965,14 +9096,47 @@
         "created_user_id",
         "updated_timestamp",
         "updated_user_id",
         "presence",
         "start_timestamp",
         "end_timestamp"
     ),
+    "user_review_users_with_same_main_email_address_view": (
+        "user_id",
+        "number",
+        "brand_id",
+        "username",
+        "is_approved",
+        "main_email",
+        "first_name",
+        "last_name",
+        "name_approved",
+        "identity_id",
+        "stars",
+        "default_time_zone",
+        "current_time_zone",
+        "preferred_lang_code",
+        "active_location_id",
+        "gender_id",
+        "interested_in_gender_id",
+        "user_approval_to_get_emails_from_us",
+        "password",
+        "birthday_original_moved_to_person",
+        "birthday_moved_to_person",
+        "region",
+        "created_timestamp",
+        "created_user_id",
+        "updated_timestamp",
+        "updated_user_id",
+        "presence",
+        "is_system",
+        "is_test_data",
+        "start_timestamp",
+        "end_timestamp"
+    ),
     "user_status_history_table": (
         "id",
         "start_timestamp",
         "end_timestamp",
         "user_status_id"
     ),
     "user_status_ml_table": (
```

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.331/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.331/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.331/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.331/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.330
+Version: 0.0.331
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.330/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.331/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/pyproject.toml` & `database_mysql_local-0.0.331/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.330/setup.py` & `database_mysql_local-0.0.331/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.330',
+    version='0.0.331',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

