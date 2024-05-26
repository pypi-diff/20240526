# Comparing `tmp/database_mysql_local-0.0.331.tar.gz` & `tmp/database_mysql_local-0.0.332.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.331.tar", last modified: Sat May 25 23:20:02 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.332.tar", last modified: Sat May 25 23:54:33 2024, max compression
```

## Comparing `database_mysql_local-0.0.331.tar` & `database_mysql_local-0.0.332.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:20:02.859233 database_mysql_local-0.0.331/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    56887 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 23:19:30.000000 database_mysql_local-0.0.331/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 23:20:02.000000 database_mysql_local-0.0.331/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 23:19:11.000000 database_mysql_local-0.0.331/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:20:02.867233 database_mysql_local-0.0.331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 23:19:03.000000 database_mysql_local-0.0.331/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:33.985340 database_mysql_local-0.0.332/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 23:54:33.985340 database_mysql_local-0.0.332/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:33.977340 database_mysql_local-0.0.332/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:33.981340 database_mysql_local-0.0.332/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56309 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30607 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 23:54:00.000000 database_mysql_local-0.0.332/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:33.981340 database_mysql_local-0.0.332/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 23:53:43.000000 database_mysql_local-0.0.332/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:54:33.985340 database_mysql_local-0.0.332/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/setup.py
```

### Comparing `database_mysql_local-0.0.331/PKG-INFO` & `database_mysql_local-0.0.332/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.331
+Version: 0.0.332
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.331/README.md` & `database_mysql_local-0.0.332/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.332/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.332/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.332/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.332/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .utils import (detect_if_is_test_data, generate_column_name,
                     generate_table_name, generate_view_name,
                     get_entity_type_by_table_name, get_where_params,
                     process_insert_data_dict, process_update_data_dict,
                     replace_view_with_table, validate_none_select_table_name,
                     validate_select_table_name, validate_single_clause_value,
                     where_skip_null_values, insert_is_undelete,
-                    is_end_timestamp_in_table)
+                    is_end_timestamp_in_table, get_table_columns)
 
 printed_dep_warning = []
 
 
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
     There are 4 main functions to create, read, update, and delete data from the database.
@@ -79,15 +79,15 @@
         #   get_id_of_existing_exact_match: bool = True) -> int:
         """Inserts a new row into the table and returns the id of the new row or -1 if an error occurred.
         ignore_duplicate should be False as default, because for example if a user register with existing name,
             he should get an error and not existing id
         """
         # if ignore_duplicate is not None:
         #     self.logger.warning("GenericCRUD.insert: ignore_duplicate is deprecated")
-        data_dict = data_json or self._data_json_to_dict(data_dict)
+        data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
         table_name = table_name or self.default_table_name
         schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
         if ignore_duplicate:
             self.logger.warning(f"GenericCRUD.insert({schema_name}.{table_name}) using ignore_duplicate, is it needed?",
                                 object={"data_dict": data_dict})
 
@@ -174,15 +174,15 @@
     def upsert(self, *, schema_name: str = None, table_name: str = None, view_table_name: str = None,
                data_dict: dict = None, data_json: dict = None,
                data_dict_compare: dict = None, data_json_compare: dict = None,
                order_by: str = None, compare_with_or: bool = False) -> Optional[int]:
         """Inserts a new row into the table, or updates an existing row if a row with the
           same values as data_dict_compare exists,
           and returns the id of the new row or None if an error occurred."""
-        data_dict = data_json or self._data_json_to_dict(data_dict)
+        data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
         data_dict_compare = data_json_compare or self._data_json_to_dict(data_dict_compare)
         old_schema_name = self.default_schema_name
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         view_table_name = view_table_name or self.default_view_table_name
         column_name = generate_column_name(table_name)
         self._validate_args(args=locals())
@@ -266,74 +266,82 @@
             existing_duplicate_id = self.__get_existing_duplicate_id_without_timestamp(
                 schema_name=schema_name, table_name=table_name, duplicate_column_name=duplicate_column_name,
                 duplicate_value=duplicate_value, column_name=column_name)
 
         self.logger.debug(object=locals())
         return existing_duplicate_id
 
-    def __get_existing_duplicate_id_with_timestamp(self, schema_name, table_name, duplicate_column_name,
-                                                   duplicate_value, column_name):
+    def __get_existing_duplicate_id_with_timestamp(
+            self, schema_name: str, table_name: str, duplicate_column_name: str,
+            duplicate_value: Any, column_name: str) -> int or None:
         select_query = (
             f"SELECT {column_name}, end_timestamp "
             f"FROM `{schema_name}`.`{table_name}` "
             f"WHERE {duplicate_column_name} = %s LIMIT 1;"
         )
         self.connection.commit()
         self.cursor.execute(select_query, (duplicate_value,))
         row = self.cursor.fetchone()
         if row is None:
-            existing_duplicate_id = end_timestamp = None
+            existing_duplicate_id = None
+            return existing_duplicate_id
         else:
             existing_duplicate_id, end_timestamp = row
         end_timestamp = end_timestamp.replace(tzinfo=timezone.utc)
         if datetime.now(timezone.utc) > end_timestamp:
-            self.__undelete(schema_name=schema_name, table_name=table_name, column_name=column_name,
-                            column_value=existing_duplicate_id)
+            self.undelete_by_column_and_value(schema_name=schema_name, table_name=table_name, column_name=column_name,
+                                              column_value=existing_duplicate_id)
         return existing_duplicate_id
 
-    def __get_existing_duplicate_id_without_timestamp(self, schema_name, table_name, duplicate_column_name,
-                                                      duplicate_value, column_name):
+    def __get_existing_duplicate_id_without_timestamp(
+            self, schema_name: str, table_name: str, duplicate_column_name: str,
+            duplicate_value: Any, column_name: str) -> int or None:
         select_query = (
             f"SELECT {column_name} "
             f"FROM `{schema_name}`.`{table_name}` "
             f"WHERE {duplicate_column_name} = %s LIMIT 1;"
         )
         self.connection.commit()
         self.cursor.execute(select_query, (duplicate_value,))
         existing_duplicate_id = (self.cursor.fetchone() or [None])[0]
         return existing_duplicate_id
 
-    def __undelete(self, schema_name: str, table_name: str, column_name: str, column_value: Any) -> None:
+    def undelete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None, column_name: str = None,
+                                     column_value: Any) -> None:
         """Undeletes a row by setting the end_timestamp to NULL."""
+        schema_name = schema_name or self.default_schema_name
+        table_name = table_name or self.default_table_name
+        column_name = column_name or self.default_column_name
+        self._validate_args(args=locals())
         self.update_by_column_and_value(
             schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=column_value,
-            data_dict={"end_timestamp": None}, commit_changes=True)
+            data_dict={"end_timestamp": None})
 
     def update_by_id(
-            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
+            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int or None:
         if "update_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.update_by_id is deprecated, use update_by_column_and_value instead.")
             printed_dep_warning.append("update_by_id")
         updated_id = self.update_by_column_and_value(
             schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=column_value,
             id_column_name=id_column_name, id_column_value=id_column_value, data_dict=data_dict, data_json=data_json,
             limit=limit, order_by=order_by, commit_changes=commit_changes)
         return updated_id
 
     def update_by_column_and_value(
-            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
+            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int or None:
         """Updates data in the table by ID."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
-        data_dict = data_json or self._data_json_to_dict(data_dict)
+        data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
         table_name = table_name or self.default_table_name
         column_name = column_name or self.default_column_name
 
         if column_name:
             where, params = get_where_params(column_name, column_value)
             last_row_id = self.update_by_where(
                 schema_name=schema_name, table_name=table_name, where=where, data_dict=data_dict,
@@ -351,15 +359,15 @@
         Example:
         "UPDATE table_name SET A=A_val, B=B_val WHERE C=C_val AND D=D_val"
         translates into:
         update_by_where(table_name="table_name",
                         data_dict={"A": A_val, "B": B_val},
                         where="C=%s AND D=%s",
                         params=(C_val, D_val)"""
-        data_dict = data_json or self._data_json_to_dict(data_dict)
+        data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
         table_name = table_name or self.default_table_name
         schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
 
         data_dict = self.__add_create_updated_user_profile_ids(data_dict=data_dict, add_created_user_id=False,
                                                                schema_name=schema_name, table_name=table_name)
 
@@ -377,27 +385,27 @@
         self.cursor.execute(update_query, tuple(data_dict.values()) + params)
         if commit_changes:
             self.connection.commit()
         last_row_id = self.cursor.lastrowid()
         return last_row_id
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
-                     column_name: str = None, column_value: Any = None,
+                     column_name: str = None, column_value: Any,
                      id_column_name: str = None, id_column_value: Any = None) -> int:
         if "delete_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.delete_by_id is deprecated, use delete_by_column_and_value instead.")
             printed_dep_warning.append("delete_by_id")
         affected_rows = self.delete_by_column_and_value(schema_name=schema_name, table_name=table_name,
                                                         column_name=column_name, column_value=column_value,
                                                         id_column_name=id_column_name, id_column_value=id_column_value)
         return affected_rows
 
     def delete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None,
-                                   column_name: str = None, column_value: Any = None,
+                                   column_name: str = None, column_value: Any,
                                    id_column_name: str = None, id_column_value: Any = None) -> int:
         """Deletes data from the table by id"""
         # checks are done inside delete_by_where
         column_name = self._deprecated_id_column(
             id_column_name, column_name) or self.default_column_name
         column_value = column_value or id_column_value
         if column_name:  # column_value can be empty
@@ -476,86 +484,86 @@
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         result_as_dicts = self.convert_multi_to_dict(result, select_clause_value)
         return result_as_dicts
 
     # TODO: test distinct
     def select_one_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                select_clause_value: str = None,
-                               column_name: str = None, column_value: Any = None,
+                               column_name: str = None, column_value: Any,
                                id_column_name: str = None, id_column_value: Any = None,
                                distinct: bool = False, order_by: str = "") -> tuple:
         if "select_one_tuple_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_one_tuple_by_id is deprecated, use select_one_tuple_by_column_and_value instead.")
             printed_dep_warning.append("select_one_tuple_by_id")
         result = self.select_one_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by)
         return result
 
     def select_one_tuple_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "") -> tuple:
         """Selects one row from the table by ID and returns it as a tuple."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         result = self.select_multi_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, distinct=distinct, limit=1, order_by=order_by)
         if result:
             return result[0]
         else:
             return tuple()  # or None?
 
     def select_one_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "") -> dict:
         if "select_one_dict_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_one_dict_by_id is deprecated, use select_one_dict_by_column_and_value instead.")
             printed_dep_warning.append("select_one_dict_by_id")
         result = self.select_one_dict_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by)
         return result
 
     def select_one_dict_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "") -> dict:
         """Selects one row from the table by ID and returns it as a dictionary (column_name: value)"""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         result = self.select_one_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, distinct=distinct, order_by=order_by)
         result = self.convert_to_dict(row=result, select_clause_value=select_clause_value)
         return result
 
     def select_one_value_by_id(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         if "select_one_value_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_one_value_by_id is deprecated, use select_one_value_by_column_and_value instead.")
             printed_dep_warning.append("select_one_value_by_id")
         result = self.select_one_value_by_column_and_value(
             select_clause_value=select_clause_value, schema_name=schema_name, view_table_name=view_table_name,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, order_by=order_by, skip_null_values=skip_null_values)
         return result
 
     def select_one_value_by_column_and_value(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         """Selects one value from the table by ID and returns it."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
         select_clause_value = select_clause_value or self.default_select_clause_value
         validate_single_clause_value(select_clause_value)
@@ -601,15 +609,15 @@
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
         if result:
             return result[0]
 
     def select_multi_value_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
         if "select_multi_value_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_multi_value_by_id is deprecated, use select_multi_value_by_column_and_value instead.")
             printed_dep_warning.append("select_multi_value_by_id")
         result = self.select_multi_value_by_column_and_value(
@@ -617,15 +625,15 @@
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by,
             skip_null_values=skip_null_values)
         return result
 
     def select_multi_value_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
         """Selects multiple values from the table by ID and returns them as a list."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
         select_clause_value = select_clause_value or self.default_select_clause_value
@@ -647,29 +655,29 @@
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
 
     def select_multi_tuple_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         if "select_multi_tuple_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_multi_tuple_by_id is deprecated, use select_multi_tuple_by_column_and_value instead.")
             printed_dep_warning.append("select_multi_tuple_by_id")
         result = self.select_multi_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_tuple_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a
         list of tuples.
         send `column_name=''` if you want to select all rows and ignore default column"""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
@@ -687,59 +695,39 @@
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         if "select_multi_dict_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_multi_dict_by_id is deprecated, use select_multi_dict_by_column_and_value instead.")
             printed_dep_warning.append("select_multi_dict_by_id")
         result = self.select_multi_dict_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_dict_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a list of dictionaries."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         result = self.select_multi_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, distinct=distinct, limit=limit, order_by=order_by)
         result = self.convert_multi_to_dict(result, select_clause_value)
         return result
 
-    # TODO: use table_definition_table to improve performance
-    # TODO: replace with redis in the future with table_definition_table
-    @lru_cache
-    def get_table_columns(self, schema_name: str = None, table_name: str = None) -> tuple:
-        schema_name = schema_name or self.default_schema_name
-        table_name = table_name or self.default_table_name
-        select_query = "SELECT column_name " \
-                       "FROM information_schema.columns " \
-                       "WHERE TABLE_SCHEMA = %s " \
-                       "AND TABLE_NAME = %s;"
-        params = (schema_name, table_name)
-
-        self.connection.commit()
-        self.cursor.execute(select_query, params)
-        result = self.cursor.fetchall()
-
-        columns_tuple = tuple(x[0] for x in result)
-        self.logger.debug(object=locals())
-        return columns_tuple
-
     @lru_cache
     def get_primary_key(self, schema_name: str = None, table_name: str = None) -> str or None:
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         query = """
             SELECT COLUMN_NAME
             FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
@@ -779,15 +767,15 @@
             if arg_name in ("self", "__class__"):
                 continue
             elif arg_name in required_args and not arg_value:
                 message = f"Invalid value for {arg_name}: {arg_value}"
             elif arg_name == "table_name":
                 validate_none_select_table_name(arg_value)
             elif arg_name == "view_table_name":
-                validate_select_table_name(database_object_name=arg_value)
+                validate_select_table_name(view_table_name=arg_value)
 
             # data_dict values are allowed to contain ';', as we use them with %s (TODO: unless it's ToSQLInterface)
             if ((arg_name.startswith("data_") and arg_value and any(
                     ";" in str(x) for x in arg_value.keys())) or  # check columns
                     (not arg_name.startswith("data_") and arg_name != "params" and ";" in str(arg_value))):
                 message = f"Invalid value for {arg_name}: {arg_value} (contains ';')"
 
@@ -815,15 +803,15 @@
     def __add_create_updated_user_profile_ids(self, data_dict: dict, add_created_user_id: bool = False,
                                               schema_name: str = None, table_name: str = None) -> dict:
         """Adds created_user_id and updated_user_id to data_dict."""
         # if get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value):
         data_dict = data_dict or {}
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
-        table_columns = self.get_table_columns(schema_name=schema_name, table_name=table_name)
+        table_columns = get_table_columns(table_name=table_name)
         if add_created_user_id:
             if "created_user_id" in table_columns:
                 data_dict["created_user_id"] = self.user_context.get_effective_user_id()
             else:
                 self.__log_warning("created_user_id", schema_name, table_name)
             if "created_real_user_id" in table_columns:
                 data_dict["created_real_user_id"] = self.user_context.get_real_user_id()
```

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.332/database_mysql_local/src/generic_crud_ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 
     def add_value(self, *, schema_name: str = None, data_dict: dict = None, data_ml_dict: dict = None,
                   data_json: dict = None, data_ml_json: dict = None, column_name: str = None,
                   table_id: int = None, lang_code: LangCode = None,
                   is_main: bool or None = False, table_name: str = None,
                   ml_table_name: str = None) -> Optional[tuple]:
         schema_name = schema_name or self.default_schema_name
-        data_dict = data_json or self._data_json_to_dict(data_dict)
-        data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
+        data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
+        data_ml_dict = data_ml_dict or self._data_json_to_dict(data_json=data_ml_json)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, data_ml_dict=data_ml_dict)
         table_name = table_name or self.default_table_name
         column_name = column_name or self.default_column_name
         ml_view_name = generate_view_name(ml_table_name) if ml_table_name else self.default_ml_view_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
 
         old_cursor = self.cursor
@@ -132,16 +132,16 @@
             self, *, data_dict: dict = None, data_ml_dict: dict = None, data_json: dict = None,
             data_ml_json: dict = None, table_id: int = None, lang_code: LangCode = None,
             is_main: bool = False, table_name: str = None, ml_table_name: str = None, schema_name: str = None,
             order_by: str = None) -> (int, int):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for add_value_if_not_exist")
-        data_dict = data_json or self._data_json_to_dict(data_dict)
-        data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
+        data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
+        data_ml_dict = data_ml_dict or self._data_json_to_dict(data_json=data_ml_json)
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = generate_column_name(table_name)
         ml_column_name = generate_column_name(ml_table_name)
 
         # check if the row exists in the ml_table
@@ -164,16 +164,16 @@
             self, *, data_dict: dict = None, data_ml_dict: dict = None, data_json: dict = None,
             data_ml_json: dict = None, ml_table_id: int, table_id: int, lang_code: LangCode = None,
             is_main: bool = False, table_name: str = None, ml_table_name: str = None, schema_name: str = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> (int, int):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for update_value")
-        data_dict = data_json or self._data_json_to_dict(data_dict)
-        data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
+        data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
+        data_ml_dict = data_ml_dict or self._data_json_to_dict(data_json=data_ml_json)
         schema_name = schema_name or self.default_schema_name
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, data_ml_dict=data_ml_dict)
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = generate_column_name(table_name)
 
         if table_id is None:
@@ -216,16 +216,16 @@
             table_id: int = None, lang_code: LangCode = None, is_main: bool = False, table_name: str = None,
             ml_table_name: str = None, schema_name: str = None, compare_view_name: str = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> (int, int):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
         compare_view_name = compare_view_name or self.default_ml_view_table_name
-        data_dict = data_json or self._data_json_to_dict(data_dict)
-        data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
+        data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
+        data_ml_dict = data_ml_dict or self._data_json_to_dict(data_json=data_ml_json)
         data_dict_compare = data_json_compare or self._data_json_to_dict(data_dict_compare)
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = generate_column_name(table_name)
         ml_column_name = generate_column_name(ml_table_name)
 
@@ -260,16 +260,16 @@
             data_json_compare: dict = None, data_dict_compare: dict = None, table_id: int = None, order_by: str = None,
             table_name: str = None, ml_table_name: str = None, schema_name: str = None, lang_code: LangCode = None,
             compare_view_name: str = None, limit: int = DEFAULT_SQL_SELECT_LIMIT) -> (int, list[int]):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
         compare_view_name = compare_view_name or self.default_ml_view_table_name
-        data_dict = data_json or self._data_json_to_dict(data_dict)
-        data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
+        data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
+        data_ml_dict = data_ml_dict or self._data_json_to_dict(data_json=data_ml_json)
         data_dict_compare = data_json_compare or self._data_json_to_dict(data_dict_compare)
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = generate_column_name(table_name)
         ml_column_name = generate_column_name(ml_table_name)
 
@@ -360,15 +360,15 @@
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
         column_name = column_name or generate_column_name(
             self.default_table_name)
         result = self.select_one_dict_by_where(view_table_name=self.default_ml_view_table_name,
                                                where=f"{column_name}=%s AND lang_code=%s",
                                                params=(table_id, lang_code_str),
-                                               order_by=order_by or f"{column_name} DESC")
+                                               order_by=order_by)
 
         return result
 
     def get_values_dict_list(self, *, table_id: int, lang_code: LangCode = None,
                              column_name: str = None, id_column_name: str = None,
                              order_by: str = None, schema_name: str = None) -> list:
         schema_name = schema_name or self.default_schema_name
@@ -388,15 +388,15 @@
         schema_name = schema_name or self.default_schema_name
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_name = column_name or generate_column_name(
             self.default_table_name)
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=self.default_ml_view_table_name,
             where=f"{column_name}=%s AND is_main=True", params=(table_id,),
-            select_clause_value=select_clause_value, order_by=order_by or f"{column_name} DESC")
+            select_clause_value=select_clause_value, order_by=order_by)
 
         return result
 
     def get_main_values_dict(self, *, table_id: int, column_name: str = None, id_column_name: str = None,
                              select_clause_value: str = "*", order_by: str = None, schema_name: str = None) -> dict:
         schema_name = schema_name or self.default_schema_name
         column_name = self._deprecated_id_column(id_column_name, column_name)
@@ -487,15 +487,15 @@
         where = f"{column_name}=%s AND {self.is_main_column_name} = True"
         updated_id = self.update_by_where(schema_name=schema_name, table_name=self.default_ml_table_name,
                                           data_dict=data_ml_dict, where=where, params=(table_id,))
         return updated_id
 
     def _get_lang_code_str(self, *, name: str = None, lang_code: LangCode = None,
                            data_ml_dict: dict = None, data_ml_json: dict = None) -> str:
-        data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
+        data_ml_dict = data_ml_dict or self._data_json_to_dict(data_json=data_ml_json)
         if lang_code is None and name is not None:
             lang_code_str = LangCode.detect_lang_code_str(name)
         elif lang_code is None and data_ml_dict is not None:
             text = data_ml_dict.get("title") or data_ml_dict.get("name")
             lang_code_str = LangCode.detect_lang_code_str(text)
         elif lang_code is None:
             lang_code_str = self.user_context.get_effective_profile_preferred_lang_code_string()
```

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.332/database_mysql_local/src/generic_mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,18 @@
                  default_view_table_name: str = None,
                  default_view_with_deleted_and_test_data: str = None,
                  default_id_column_name: str = None, default_column_name: str = None,
                  default_entity_name1: str = None,
                  default_entity_name2: str = None,
                  is_test_data: bool = False):
         default_column_name = default_column_name or default_id_column_name
-        GenericCRUD.__init__(self, default_schema_name=default_schema_name,
-                             default_table_name=default_table_name, default_view_table_name=default_view_table_name,
-                             default_view_with_deleted_and_test_data=default_view_with_deleted_and_test_data,
-                             default_id_column_name=default_column_name, is_test_data=is_test_data)
+        super().__init__(default_schema_name=default_schema_name,
+                         default_table_name=default_table_name, default_view_table_name=default_view_table_name,
+                         default_view_with_deleted_and_test_data=default_view_with_deleted_and_test_data,
+                         default_column_name=default_column_name, is_test_data=is_test_data)
         self.default_entity_name1 = default_entity_name1
         self.default_entity_name2 = default_entity_name2
 
     # We added the schema_name parameter to avoid using USE and void creating a new instance/object
     # of the database for mapping.
     def insert_mapping(self, *, entity_id1: int, entity_id2: int,
                        entity_name1: str = None, entity_name2: str = None,
@@ -34,24 +34,24 @@
         :param entity_id1: The id of the first entity.
         :param entity_id2: The id of the second entity.
         :param schema_name: The name of the schema.
         :param data_dict: The data to insert.
         :param ignore_duplicate: If True, ignore duplicate rows.
         :return: The id of the new row or -1 if an error occurred.
         """
-        data_dict = data_dict or GenericCRUD._data_json_to_dict(self, data_json)
+        data_dict = data_dict or self._data_json_to_dict(data_json)
         entity_name1 = entity_name1 or self.default_entity_name1
         entity_name2 = entity_name2 or self.default_entity_name2
         schema_name = schema_name or self.default_schema_name
         table_name = f"{entity_name1}_{entity_name2}_table"
         data_dict = data_dict or {}
         data_dict[f"{entity_name1}_id"] = entity_id1
         data_dict[f"{entity_name2}_id"] = entity_id2
-        mapping_id = GenericCRUD.insert(self, schema_name=schema_name, data_dict=data_dict, table_name=table_name,
-                                        ignore_duplicate=ignore_duplicate)
+        mapping_id = super().insert(schema_name=schema_name, data_dict=data_dict, table_name=table_name,
+                                    ignore_duplicate=ignore_duplicate)
         return mapping_id
 
     # TODO: do we need delete_mapping_by_id?
     def delete_mapping_by_two_ids(self, *, entity_id1: int, entity_id2: int,
                                   entity_name1: str = None, entity_name2: str = None,
                                   schema_name: str = None) -> None:
         """ Deletes a link between two entities.
@@ -66,15 +66,15 @@
         entity_name1 = entity_name1 or self.default_entity_name1
         entity_name2 = entity_name2 or self.default_entity_name2
         schema_name = schema_name or self.default_schema_name
         table_name = f"{entity_name1}_{entity_name2}_table"
 
         where = f"{entity_name1}_id=%s AND {entity_name2}_id=%s"
         params = (entity_id1, entity_id2)
-        GenericCRUD.delete_by_where(self, schema_name=schema_name, table_name=table_name, where=where, params=params)
+        super().delete_by_where(schema_name=schema_name, table_name=table_name, where=where, params=params)
 
     # TODO: remove _by_id, as there's no by_where. Plus, it's by ids. make it backward compatible
     def select_multi_mapping_tuple_by_id(self, *, entity_id1: int, entity_id2: int,
                                          entity_name1: str = None, entity_name2: str = None,
                                          schema_name: str = None, select_clause_value: str = "*") -> list:
         """Selects a row from the database by id.
         :param entity_name1: The name of the first entity's table.
@@ -90,17 +90,17 @@
 
         entity_name1 = entity_name1 or self.default_entity_name1
         entity_name2 = entity_name2 or self.default_entity_name2
         schema_name = schema_name or self.default_schema_name
         table_name = f"{entity_name1}_{entity_name2}_view"
         where = f"{entity_name1}_id=%s AND {entity_name2}_id=%s"
         params = (entity_id1, entity_id2)
-        result = GenericCRUD.select_multi_tuple_by_where(self, schema_name=schema_name, view_table_name=table_name,
-                                                         select_clause_value=select_clause_value,
-                                                         where=where, params=params)
+        result = super().select_multi_tuple_by_where(schema_name=schema_name, view_table_name=table_name,
+                                                     select_clause_value=select_clause_value,
+                                                     where=where, params=params)
         return result
 
     def select_multi_mapping_dict_by_id(self, *, entity_id1: int, entity_id2: int,
                                         entity_name1: str = None, entity_name2: str = None,
                                         schema_name: str = None, select_clause_value: str = "*") -> list:
         """Selects a row from the database by id.
         :param entity_name1: The name of the first entity's table.
@@ -113,10 +113,11 @@
         """
 
         result = self.select_multi_mapping_tuple_by_id(entity_name1=entity_name1, entity_name2=entity_name2,
                                                        entity_id1=entity_id1, entity_id2=entity_id2,
                                                        schema_name=schema_name,
                                                        select_clause_value=select_clause_value)
 
-        return GenericCRUD.convert_multi_to_dict(self, result, select_clause_value)
+        result = super().convert_multi_to_dict(result, select_clause_value)
+        return result
 
     # TODO: add select_one_dict/tuple/value, and select_multi_value
```

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/point.py` & `database_mysql_local-0.0.332/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.332/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.332/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     def __init__(self, default_schema_name: str = None, default_table_name: str = None,
                  default_view_table_name: str = None,
                  default_view_with_deleted_and_test_data: str = None,
                  default_id_column_name: str = None, default_column_name: str = None,
                  default_select_clause_value: str = "updated_timestamp",
                  default_where: str = None):
         default_column_name = default_id_column_name or default_column_name
-        GenericCRUD.__init__(self, default_schema_name=default_schema_name, default_table_name=default_table_name,
-                             default_view_table_name=default_view_table_name,
-                             default_view_with_deleted_and_test_data=default_view_with_deleted_and_test_data,
-                             default_id_column_name=default_column_name,
-                             default_select_clause_value=default_select_clause_value, default_where=default_where)
+        super().__init__(default_schema_name=default_schema_name, default_table_name=default_table_name,
+                         default_view_table_name=default_view_table_name,
+                         default_view_with_deleted_and_test_data=default_view_with_deleted_and_test_data,
+                         default_column_name=default_column_name,
+                         default_select_clause_value=default_select_clause_value, default_where=default_where)
 
     def get_update_status_by_where(self, *, schema_name: str = None, view_table_name: str = None,
                                    where: str = None, params: tuple, select_clause_value: str = None,
                                    remote_last_modified_timestamp: str, ) -> UpdateStatus:
         """
         Get the status of the update by the where clause
         :param remote_last_modified_timestamp str
```

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.332/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.332/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.332/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.332/database_mysql_local/src/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from url_remote.environment_name_enum import EnvironmentName
 
 from .table_columns import table_columns
 from .table_definition import table_definition
 from .to_sql_interface import ToSQLInterface
 
 
-def validate_select_table_name(database_object_name: str) -> None:
+def validate_select_table_name(view_table_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
-            and not database_object_name.endswith("_view")):
+            and not view_table_name.endswith("_view")):
         raise Exception(
-            f"View name must end with '_view' in this environment (got {database_object_name})")
+            f"View name must end with '_view' in this environment (got {view_table_name})")
 
 
 def validate_none_select_table_name(database_object_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
             and not database_object_name.endswith("_table")):
         raise Exception(
             f"Table name must end with '_table' in this environment  (got {database_object_name})")
@@ -166,7 +166,27 @@
     is_end_timestamp_in_table = is_column_in_table(table_name, "end_timestamp")
     return is_end_timestamp_in_table
 
 
 def is_column_in_table(table_name: str, column_name: str) -> bool:
     columns = table_columns.get(table_name, [])
     return column_name in columns
+
+
+def get_table_columns(table_name: str = None) -> tuple:
+    table_columns_tuple = table_columns.get(table_name, [])
+    return table_columns_tuple
+
+# def get_table_columns(schema_name: str = None, table_name: str = None) -> tuple:
+#     select_query = "SELECT column_name " \
+#                    "FROM information_schema.columns " \
+#                    "WHERE TABLE_SCHEMA = %s " \
+#                    "AND TABLE_NAME = %s;"
+#     params = (schema_name, table_name)
+#
+#     self.connection.commit()
+#     self.cursor.execute(select_query, params)
+#     result = self.cursor.fetchall()
+#
+#     columns_tuple = tuple(x[0] for x in result)
+#     self.logger.debug(object=locals())
+#     return columns_tuple
```

### Comparing `database_mysql_local-0.0.331/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.332/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.331
+Version: 0.0.332
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.331/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.332/database_mysql_local.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 database_mysql_local.egg-info/dependency_links.txt
 database_mysql_local.egg-info/requires.txt
 database_mysql_local.egg-info/top_level.txt
 database_mysql_local/src/__init__.py
 database_mysql_local/src/connector.py
 database_mysql_local/src/constants.py
 database_mysql_local/src/cursor.py
+database_mysql_local/src/generate_table_columns.py
 database_mysql_local/src/generic_crud.py
 database_mysql_local/src/generic_crud_ml.py
 database_mysql_local/src/generic_mapping.py
 database_mysql_local/src/point.py
 database_mysql_local/src/polygon.py
 database_mysql_local/src/sync_conflict_resolution.py
 database_mysql_local/src/table_columns.py
```

### Comparing `database_mysql_local-0.0.331/pyproject.toml` & `database_mysql_local-0.0.332/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.331/setup.py` & `database_mysql_local-0.0.332/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.331',
+    version='0.0.332',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

