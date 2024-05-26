# Comparing `tmp/database_mysql_local-0.0.333.tar.gz` & `tmp/database_mysql_local-0.0.334.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.333.tar", last modified: Sun May 26 00:08:13 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.334.tar", last modified: Sun May 26 03:31:04 2024, max compression
```

## Comparing `database_mysql_local-0.0.333.tar` & `database_mysql_local-0.0.334.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:08:13.383366 database_mysql_local-0.0.333/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    56529 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30607 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 00:07:31.000000 database_mysql_local-0.0.333/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 00:07:10.000000 database_mysql_local-0.0.333/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:31:04.579027 database_mysql_local-0.0.334/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 03:31:04.579027 database_mysql_local-0.0.334/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:31:04.575027 database_mysql_local-0.0.334/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:31:04.579027 database_mysql_local-0.0.334/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56364 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30607 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 03:30:30.000000 database_mysql_local-0.0.334/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:31:04.579027 database_mysql_local-0.0.334/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 03:30:13.000000 database_mysql_local-0.0.334/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 03:31:04.583027 database_mysql_local-0.0.334/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/setup.py
```

### Comparing `database_mysql_local-0.0.333/PKG-INFO` & `database_mysql_local-0.0.334/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.333
+Version: 0.0.334
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.333/README.md` & `database_mysql_local-0.0.334/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.334/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.334/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.334/database_mysql_local/src/cursor.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,17 @@
             quoted_parameters = tuple("'" + str(param) + "'" for param in sql_parameters)
             formatted_sql = sql_statement % quoted_parameters
             sql_parameters_str = ", ".join(quoted_parameters)
         else:
             formatted_sql = sql_statement
             sql_parameters_str = "None"
         self.logger.info('database-mysql-local cursor.py execute()', object={
-            "formatted_sql": formatted_sql,
+            "formatted_sql": formatted_sql.replace("\n", " "),
             "sql_parameters": sql_parameters_str,
-            "sql_statement": sql_statement
+            "sql_statement": sql_statement.replace("\n", " ")
         })
         self.cursor.execute(sql_statement, sql_parameters, multi=multi)
 
     def executemany(self, sql_statement: str, sql_parameters: tuple or list = None) -> None:
         try:
             if sql_parameters:  # sql_parameters is list of tuples, each tuple is a row
                 sql_parameters_str = [
@@ -46,17 +46,17 @@
                 placeholders = "[" + ", ".join([values] * len(sql_parameters)) + "]"
                 concat_params_tuple = tuple([param for tup in sql_parameters_str for param in tup])
                 formatted_sql = f"{sql} VALUES {placeholders}" % concat_params_tuple
             else:
                 formatted_sql = sql_statement
                 sql_parameters_str = "None"
             self.logger.info('database-mysql-local cursor.py executemany()', object={
-                "formatted_sql": formatted_sql,
+                "formatted_sql": formatted_sql.replace("\n", " "),
                 "sql_parameters": sql_parameters_str,
-                "sql_statement": sql_statement
+                "sql_statement": sql_statement.replace("\n", " ")
             })
         except Exception as e:
             self.logger.warning('Unable to format parameters', object={
                 "sql_statement": sql_statement,
                 "sql_parameters": sql_parameters,
                 "error": str(e)
             })
@@ -78,15 +78,15 @@
     def column_names(self) -> tuple:
         return self.cursor.column_names
 
     def lastrowid(self) -> int or None:
         """Returns the value generated for an AUTO_INCREMENT column by the previous INSERT or UPDATE statement."""
         return self.cursor.lastrowid
 
-    def get_row_count(self) -> int:
+    def get_affected_row_count(self) -> int:
         """Returns the number of rows produced or affected"""
         return self.cursor.rowcount
 
     def get_last_executed_statement(self) -> str:
         return self.cursor.statement
 
     def close(self) -> None:
```

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.334/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.334/database_mysql_local/src/generic_crud.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from .connector import Connector
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
 from .cursor import Cursor
 from .table_definition import table_definition
 from .utils import (detect_if_is_test_data, generate_column_name,
                     generate_table_name, generate_view_name,
                     get_entity_type_by_table_name, get_where_params,
-                    process_insert_data_dict, process_update_data_dict,
+                    process_insert_data_dict, process_update_data_dict, process_upsert_data_dict,
                     replace_view_with_table, validate_none_select_table_name,
                     validate_select_table_name, validate_single_clause_value,
                     where_skip_null_values, insert_is_undelete,
-                    is_end_timestamp_in_table, get_table_columns)
+                    is_end_timestamp_in_table, get_table_columns, group_list_by_columns)
 
 printed_dep_warning = []
 
 
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
     There are 4 main functions to create, read, update, and delete data from the database.
@@ -102,21 +102,21 @@
         #                         f"database-mysql-local.table_definition_table data structure, we might need to run sql2code")
 
         # TODO: In the future we may want to check this with table_definition
         #   and not with self.is_column_in_table for better performance
         data_dict = self.__add_create_updated_user_profile_ids(
             data_dict=data_dict, add_created_user_id=True, schema_name=schema_name, table_name=table_name)
 
-        columns, values, data_dict = process_insert_data_dict(data_dict=data_dict)
+        columns, values, params = process_insert_data_dict(data_dict=data_dict)
         # We removed the IGNORE from the SQL Statement as we want to return the id of the existing row
         insert_query = "INSERT " + \
                        f"INTO `{schema_name}`.`{table_name}` ({columns}) " \
                        f"VALUES ({values});"
         try:
-            self.cursor.execute(insert_query, tuple(data_dict.values()))
+            self.cursor.execute(insert_query, params)
             if commit_changes:
                 self.connection.commit()
             inserted_id = self.cursor.lastrowid()
         except mysql.connector.errors.IntegrityError as exception:
             if ignore_duplicate:
                 self.logger.warning("GenericCRUD.insert: existing record found, selecting it's id."
                                     f"(table_name={table_name}, data_dict={data_dict})")
@@ -124,33 +124,37 @@
             else:
                 raise exception
         finally:
             self.logger.debug(object=locals())
         return inserted_id
 
     def insert_many_dicts(self, *, schema_name: str = None, table_name: str = None, data_dicts: list[dict],
-                          commit_changes: bool = True) -> None:
+                          commit_changes: bool = True) -> int:
         """Inserts multiple rows into the table.
         data_dicts should be in the following format: [{col1: val1, col2: val2}, {col1: val3, col2: val4}, ...]
+        Returns the number of inserted rows.
         """
         if not data_dicts:
             self.logger.warning("GenericCRUD.insert_many_dicts: data_dicts is empty")
-            return
+            return 0
         converted_data_dicts = {col: [row[col] for row in data_dicts] for col in data_dicts[0]}
-        self.insert_many(schema_name=schema_name, table_name=table_name,
-                         data_dict=converted_data_dicts, commit_changes=commit_changes)
+        inserted_rows = self.insert_many(schema_name=schema_name, table_name=table_name,
+                                         data_dict=converted_data_dicts, commit_changes=commit_changes)
+
+        return inserted_rows
 
     def insert_many(self, *, schema_name: str = None, table_name: str = None, data_dict: dict[str, list or tuple],
-                    commit_changes: bool = True) -> None:
+                    commit_changes: bool = True) -> int:
         """Inserts multiple rows into the table.
         data_dict should be in the following format: {col1: [val1, val2], col2: [val3, val4], ...}
+        Returns the number of inserted rows.
         """
         if not data_dict:
             self.logger.warning("GenericCRUD.insert_many: data_dict is empty")
-            return
+            return 0
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
 
         self._validate_args(args=locals())
         # TODO: I am not sure we can use process_insert_data_dict here
 
         len_rows = len(next(v for v in data_dict.values()))
@@ -167,71 +171,53 @@
         INSERT INTO `{schema_name}`.`{table_name}` ({columns})
         VALUES ({values});
         """
         sql_parameters = list(zip(*data_dict.values()))
         self.cursor.executemany(sql_statement=sql_statement, sql_parameters=sql_parameters)
         if commit_changes:
             self.connection.commit()
+        inserted_rows = self.cursor.get_affected_row_count()
+        return inserted_rows
 
     def upsert(self, *, schema_name: str = None, table_name: str = None, view_table_name: str = None,
                data_dict: dict = None, data_json: dict = None,
                data_dict_compare: dict = None, data_json_compare: dict = None,
                order_by: str = None, compare_with_or: bool = False) -> Optional[int]:
         """Inserts a new row into the table, or updates an existing row if a row with the
           same values as data_dict_compare exists,
           and returns the id of the new row or None if an error occurred."""
         data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
         data_dict_compare = data_json_compare or self._data_json_to_dict(data_dict_compare)
-        old_schema_name = self.default_schema_name
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         view_table_name = view_table_name or self.default_view_table_name
         column_name = generate_column_name(table_name)
         self._validate_args(args=locals())
         if not data_dict:
             self.logger.warning(log_message="GenericCRUD.upsert: data_dict is empty")
             return
         if not data_dict_compare:
             inserted_id = self.insert(schema_name=schema_name,
                                       table_name=table_name, data_dict=data_dict)
             return inserted_id
 
-        columns, values, processed_data_dict_compare = process_insert_data_dict(
-            data_dict=data_dict_compare)
-        where_clauses = []
-        params = []
-        for key, value in processed_data_dict_compare.items():
-            if isinstance(value, list):
-                where_clauses.append(f"({' OR '.join([f'{key}=%s' for _ in value])})")
-                params.extend(value)
-            else:
-                where_clauses.append(f"{key}=%s")
-                params.append(value)
+        where_clause, params = process_upsert_data_dict(data_dict=data_dict_compare, compare_with_or=compare_with_or)
 
-        where_clause = " OR " if compare_with_or else " AND "
-        where_clause = where_clause.join(where_clauses)
+        table_id = self.select_one_value_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value=column_name,
+            where=where_clause, params=params, order_by=order_by)
+        if table_id:
+            self.update_by_column_and_value(
+                schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=table_id,
+                data_dict=data_dict)
+        else:
+            table_id = self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict,
+                                   ignore_duplicate=True)
 
-        try:
-            table_id = self.select_one_value_by_where(
-                schema_name=schema_name, view_table_name=view_table_name, select_clause_value=column_name,
-                where=where_clause, params=tuple(params), order_by=order_by)
-            if table_id:
-                self.update_by_column_and_value(
-                    schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=table_id,
-                    data_dict=data_dict, commit_changes=False)
-            else:
-                table_id = self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict,
-                                       commit_changes=False, ignore_duplicate=True)
-            self.connection.commit()
-        except Exception as exception:
-            self.connection.rollback()
-            raise exception
-        finally:
-            self.default_schema_name = old_schema_name
-            self.logger.debug(object=locals())
+        self.logger.debug(object=locals())
         return table_id
 
     def _get_existing_duplicate_id(self, schema_name: str, table_name: str, error: Exception) -> int or None:
         """Error examples:
         - Duplicate entry '1' for key 'test_mysql_table.PRIMARY'
         - Duplicate entry '7263200721327371865' for key 'test_mysql_table.number_UNIQUE
         - Duplicate entry 'test@gmail.com' for key 'email_address_table.email_address.unique'
@@ -330,36 +316,36 @@
             id_column_name=id_column_name, id_column_value=id_column_value, data_dict=data_dict, data_json=data_json,
             limit=limit, order_by=order_by, commit_changes=commit_changes)
         return updated_id
 
     def update_by_column_and_value(
             self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
-            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int or None:
+            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int:
         """Updates data in the table by ID."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
         table_name = table_name or self.default_table_name
         column_name = column_name or self.default_column_name
 
         if column_name:
             where, params = get_where_params(column_name, column_value)
-            last_row_id = self.update_by_where(
+            updated_rows = self.update_by_where(
                 schema_name=schema_name, table_name=table_name, where=where, data_dict=data_dict,
                 params=params, limit=limit, order_by=order_by, commit_changes=commit_changes)
-            return last_row_id
+            return updated_rows
 
         else:
             raise Exception("Update by id requires an column_name")
 
     def update_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
                         params: tuple = None, data_dict: dict = None, data_json: dict = None,
                         limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None,
-                        commit_changes: bool = True) -> int or None:
+                        commit_changes: bool = True) -> int:
         """Updates data in the table by WHERE.
         Example:
         "UPDATE table_name SET A=A_val, B=B_val WHERE C=C_val AND D=D_val"
         translates into:
         update_by_where(table_name="table_name",
                         data_dict={"A": A_val, "B": B_val},
                         where="C=%s AND D=%s",
@@ -368,83 +354,85 @@
         table_name = table_name or self.default_table_name
         schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
 
         data_dict = self.__add_create_updated_user_profile_ids(data_dict=data_dict, add_created_user_id=False,
                                                                schema_name=schema_name, table_name=table_name)
 
-        set_values, data_dict = process_update_data_dict(data_dict)
+        set_values, data_dict_params = process_update_data_dict(data_dict)
         if not where:
             raise Exception("update_by_where requires a 'where'")
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET {set_values} updated_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where} " + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
-        params = params or tuple()
+        where_params = params or tuple()
 
-        self.cursor.execute(update_query, tuple(data_dict.values()) + params)
+        self.cursor.execute(update_query, data_dict_params + where_params)
         if commit_changes:
             self.connection.commit()
-        last_row_id = self.cursor.lastrowid()
-        return last_row_id
+        updated_rows = self.cursor.get_affected_row_count()
+        return updated_rows
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
                      column_name: str = None, column_value: Any = None,
                      id_column_name: str = None, id_column_value: Any = None) -> int:
         if "delete_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.delete_by_id is deprecated, use delete_by_column_and_value instead.")
             printed_dep_warning.append("delete_by_id")
-        affected_rows = self.delete_by_column_and_value(schema_name=schema_name, table_name=table_name,
+        deleted_rows = self.delete_by_column_and_value(schema_name=schema_name, table_name=table_name,
                                                         column_name=column_name, column_value=column_value,
                                                         id_column_name=id_column_name, id_column_value=id_column_value)
-        return affected_rows
+        return deleted_rows
 
     def delete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None,
                                    column_name: str = None, column_value: Any = None,
                                    id_column_name: str = None, id_column_value: Any = None) -> int:
-        """Deletes data from the table by id"""
+        """Deletes data from the table by id.
+        Returns the number of deleted rows."""
         # checks are done inside delete_by_where
         column_name = self._deprecated_id_column(
             id_column_name, column_name) or self.default_column_name
         column_value = column_value or id_column_value
         if column_name:  # column_value can be empty
             where, params = get_where_params(column_name, column_value)
-            affected_rows = self.delete_by_where(schema_name=schema_name, table_name=table_name, where=where,
-                                                 params=params)
-            return affected_rows
+            deleted_rows = self.delete_by_where(schema_name=schema_name, table_name=table_name, where=where,
+                                                params=params)
+            return deleted_rows
         else:
             raise Exception("Delete by id requires an column_name and column_value.")
 
     def delete_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
                         params: tuple = None) -> int:
-        """Deletes data from the table by WHERE."""
+        """Deletes data from the table by WHERE.
+        Returns the number of deleted rows."""
 
         table_name = table_name or self.default_table_name
         schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
         if not where:
             raise Exception("delete_by_where requires a 'where'")
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET end_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where};"
 
         self.cursor.execute(update_query, params)
         self.connection.commit()
-        affected_rows = self.cursor.get_row_count()
-        return affected_rows
+        deleted_rows = self.cursor.get_affected_row_count()
+        return deleted_rows
 
     # Main select function
     def select_multi_tuple_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
-            order_by: str = "") -> list:
+            order_by: str = None) -> list:
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of tuples."""
 
         schema_name = schema_name or self.default_schema_name
         view_table_name = view_table_name or self.default_view_table_name
         select_clause_value = select_clause_value or self.default_select_clause_value
         where = where or self.default_where
         where = self.__where_security(where=where, view_name=view_table_name)
@@ -473,99 +461,101 @@
         result = self.cursor.fetchall()
 
         self.logger.debug(object=locals())
         return result
 
     def select_multi_dict_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            where: str = None, params: tuple = None, distinct: bool = False,
-            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
+            where: str = None, params: tuple = None, distinct: bool = False, group_by: str = None,
+            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list or dict[tuple or str, list]:
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of dictionaries."""
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         result_as_dicts = self.convert_multi_to_dict(result, select_clause_value)
+        if group_by:
+            result_as_dicts = group_list_by_columns(list_of_dicts=result_as_dicts, group_by=group_by)
         return result_as_dicts
 
     # TODO: test distinct
     def select_one_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                select_clause_value: str = None,
                                column_name: str = None, column_value: Any = None,
                                id_column_name: str = None, id_column_value: Any = None,
-                               distinct: bool = False, order_by: str = "") -> tuple:
+                               distinct: bool = False, order_by: str = None) -> tuple:
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
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
-            distinct: bool = False, order_by: str = "") -> tuple:
+            distinct: bool = False, order_by: str = None) -> tuple:
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
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
-            distinct: bool = False, order_by: str = "") -> dict:
+            distinct: bool = False, order_by: str = None) -> dict:
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
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
-            distinct: bool = False, order_by: str = "") -> dict:
+            distinct: bool = False, order_by: str = None) -> dict:
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
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
-            distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
+            distinct: bool = False, order_by: str = None, skip_null_values: bool = True) -> Any:
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
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
-            distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
+            distinct: bool = False, order_by: str = None, skip_null_values: bool = True) -> Any:
         """Selects one value from the table by ID and returns it."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
         select_clause_value = select_clause_value or self.default_select_clause_value
         validate_single_clause_value(select_clause_value)
         where, params = get_where_params(column_name, column_value)
@@ -574,52 +564,52 @@
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
         if result:  # TODO: the caller can't tell if not found, or found null
             return result[0]
 
     def select_one_tuple_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "") -> tuple:
+            where: str = None, params: tuple = None, distinct: bool = False, order_by: str = None) -> tuple:
         """Selects one row from the table based on a WHERE clause and returns it as a tuple."""
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=1, order_by=order_by)
         if result:
             return result[0]
         else:
             return tuple()
 
     def select_one_dict_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "") -> dict:
+            where: str = None, params: tuple = None, distinct: bool = False, order_by: str = None) -> dict:
         """Selects one row from the table based on a WHERE clause and returns it as a dictionary."""
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
         result = self.convert_to_dict(row=result, select_clause_value=select_clause_value)
         return result
 
     def select_one_value_by_where(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
-            where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "",
+            where: str = None, params: tuple = None, distinct: bool = False, order_by: str = None,
             skip_null_values: bool = True) -> Any:
         """Selects one value from the table based on a WHERE clause and returns it."""
         select_clause_value = select_clause_value or self.default_select_clause_value
         validate_single_clause_value(select_clause_value)
         where = where_skip_null_values(where, select_clause_value, skip_null_values)
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
         if result:
             return result[0]
 
     def select_multi_value_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
-            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
+            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None,
             skip_null_values: bool = True) -> list:
         if "select_multi_value_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_multi_value_by_id is deprecated, use select_multi_value_by_column_and_value instead.")
             printed_dep_warning.append("select_multi_value_by_id")
         result = self.select_multi_value_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
@@ -627,15 +617,15 @@
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by,
             skip_null_values=skip_null_values)
         return result
 
     def select_multi_value_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
-            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
+            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None,
             skip_null_values: bool = True) -> list:
         """Selects multiple values from the table by ID and returns them as a list."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
         select_clause_value = select_clause_value or self.default_select_clause_value
         validate_single_clause_value(select_clause_value)
@@ -645,15 +635,15 @@
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
 
     def select_multi_value_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
-            order_by: str = "", skip_null_values: bool = True) -> list:
+            order_by: str = None, skip_null_values: bool = True) -> list:
         select_clause_value = select_clause_value or self.default_select_clause_value
         validate_single_clause_value(select_clause_value)
         where = where_skip_null_values(where, select_clause_value, skip_null_values)
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
@@ -672,31 +662,21 @@
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_tuple_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
-        """Selects multiple rows from the table by ID and returns them as a
-        list of tuples.
-        send `column_name=''` if you want to select all rows and ignore default column"""
+        """Selects multiple rows from the table by ID and returns them as a list of tuples.
+        If column_value is list / tuple, it will be used as multiple values for the column_name (SQL IN)."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
 
-        if not column_name:
-            where = None
-            params = None
-        else:
-            if column_value is None:
-                where = f"`{column_name}` IS NULL"
-                params = None
-            else:
-                where = f"`{column_name}`=%s"
-                params = (column_value,)
+        where, params = get_where_params(column_name, column_value)
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
@@ -711,23 +691,26 @@
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_dict_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
-            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
+            distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None,
+            group_by: str = None) -> list or dict[tuple or str, list]:
         """Selects multiple rows from the table by ID and returns them as a list of dictionaries."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         result = self.select_multi_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, distinct=distinct, limit=limit, order_by=order_by)
-        result = self.convert_multi_to_dict(result, select_clause_value)
-        return result
+        result_as_dicts = self.convert_multi_to_dict(result, select_clause_value)
+        if group_by:
+            result_as_dicts = group_list_by_columns(list_of_dicts=result_as_dicts, group_by=group_by)
+        return result_as_dicts
 
     @lru_cache
     def get_primary_key(self, schema_name: str = None, table_name: str = None) -> str or None:
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         query = """
             SELECT COLUMN_NAME
@@ -930,29 +913,31 @@
         return cursor
 
     @cursor.setter
     def cursor(self, value: Cursor) -> None:
         """Set the cursor"""
         self._cursor = value
 
-    # TODO: test this method
-    def get_test_entity_id(self, *, entity_name: str, insert_function: callable, insert_kwargs: dict = None,
+    def get_test_entity_id(self, *, entity_name: str = None, insert_function: callable, insert_kwargs: dict = None,
                            entity_creator: callable = None, create_kwargs: dict = None,
-                           schema_name: str = None, view_name: str = None) -> int:
+                           schema_name: str = None, view_name: str = None,
+                           select_clause_value: str = None) -> int:
         """
         1. Check if there's an entity with is `is_test_data=True`.
         2. If there is, return its id.
         3. If not, create a new entity with `is_test_data=True` and return its id.
         (assuming entity_creator expects `is_test_data` as parameters,
             and returns the expected argument for insert_function)
 
         Example: get_test_entity_id(entity_name='person', entity_creator=Person, insert_function=PersonsLocal.insert)
         """
+        schema_name = schema_name or self.default_schema_name
+        entity_name = entity_name or schema_name
         view_name = view_name or self.default_view_table_name
-        select_clause_value = entity_name + "_id"
+        select_clause_value = select_clause_value or entity_name + "_id"
         test_entity_id = self.select_one_value_by_id(
             schema_name=schema_name or self.default_schema_name, view_table_name=view_name,
             column_name='is_test_data', column_value='1', select_clause_value=select_clause_value)
         if not test_entity_id:
             insert_kwargs = insert_kwargs or {}
             create_kwargs = create_kwargs or {}
             # is_test_data from the constructor should be used in the sons to avoid duplications
```

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.334/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.334/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/point.py` & `database_mysql_local-0.0.334/database_mysql_local/src/point.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 class Point(ToSQLInterface):
     def __init__(self, longitude: float, latitude: float) -> None:
         self.longitude = longitude
         self.latitude = latitude
 
+    # TODO: POINT(%s, %s) with params
     def to_sql(self) -> str:
         return f"POINT ({self.longitude}, {self.latitude})"
 
     @staticmethod
     def create_select_stmt(column_name: str) -> str:
         return f"ST_X({column_name}), ST_Y({column_name})"
```

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.334/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.334/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.334/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.334/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.334/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.334/database_mysql_local/src/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,115 @@
+import copy
 import inspect
 import os
 from functools import lru_cache
 from typing import Any, Optional
 
 from python_sdk_remote.utilities import get_environment_name
 from url_remote.environment_name_enum import EnvironmentName
 
 from .table_columns import table_columns
 from .table_definition import table_definition
 from .to_sql_interface import ToSQLInterface
 
-
+# TODO: class DatabaseMysqlUtils(metaclass=MetaLogger, object=object_database):
 def validate_select_table_name(view_table_name: str) -> None:
+    # TODO: try to detect the table name from the view name (with warning)
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
             and not view_table_name.endswith("_view")):
         raise Exception(
             f"View name must end with '_view' in this environment (got {view_table_name})")
 
 
-def validate_none_select_table_name(database_object_name: str) -> None:
+def validate_none_select_table_name(table_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
-            and not database_object_name.endswith("_table")):
+            and not table_name.endswith("_table")):
         raise Exception(
-            f"Table name must end with '_table' in this environment  (got {database_object_name})")
+            f"Table name must end with '_table' in this environment  (got {table_name})")
 
 
-def process_insert_data_dict(data_dict: dict or None) -> tuple[str, str, dict]:
+def process_insert_data_dict(data_dict: dict or None) -> (str, str, tuple):
+    """Example:
+    Input: {"name": "John", "coordinate": Point(1, 2)}
+    Output: ("`name`, `coordinate`",
+             "%s, Point(1, 2)",
+            ("John", ))
+    """
     if not data_dict:
         return '', '', {}
 
     columns = []
     values = []
+    params = tuple()
 
     for key, value in data_dict.items():
         columns.append(f"`{key}`")
         if isinstance(value, ToSQLInterface):
             values.append(value.to_sql())
         else:
             values.append('%s')
+            params += (value,)
+
+    columns_str = ','.join(columns)
+    values_str = ','.join(values)
 
-    filtered_data_dict = {key: value for key, value in data_dict.items() if
-                          not isinstance(value, ToSQLInterface)}
-    return ','.join(columns), ','.join(values), filtered_data_dict
+    return columns_str, values_str, params
 
+def process_upsert_data_dict(data_dict: dict or None, compare_with_or: bool) -> (str, str, tuple):
+    where_clauses = []
+    params = []
+    for column, value in data_dict.items():
+        if isinstance(value, list):
+            where_clauses.append(f"({' OR '.join([f'{column}=%s' for _ in value])})")
+            params.extend(value)
+        elif isinstance(value, ToSQLInterface):
+            where_clauses.append(f"{column}={value.to_sql()}")
+        else:
+            where_clauses.append(f"{column}=%s")
+            params.append(value)
 
-# Please add typing and example of input-output as docstring if possible.
-def process_update_data_dict(data_dict: dict or None) -> tuple[str, dict]:
+    where_clause = " OR " if compare_with_or else " AND "
+    where_clause = where_clause.join(where_clauses)
+    return where_clause, params
+
+def process_update_data_dict(data_dict: dict or None) -> (str, tuple):
+    """Example:
+    Input: {"name": "John", "coordinate": Point(1, 2)}
+    Output: ("name=%s, coordinate=Point(1, 2)", ("John", ))
+    """
     if not data_dict:
         return '', {}
 
     set_values = []
+    params = tuple()
     for key, value in data_dict.items():
         if isinstance(value, ToSQLInterface):
             set_values.append(f"`{key}`={value.to_sql()}")
         else:
             set_values.append(f"`{key}`=%s")
+            params += (value,)
 
-    filtered_data_dict = {key: value for key, value in data_dict.items() if
-                          not isinstance(value, ToSQLInterface)}
     # + "," because we add updated_timestamp in the update query
-    return ', '.join(set_values) + ",", filtered_data_dict
+    set_values_str = ', '.join(set_values) + ","
+    return set_values_str, params
 
 
 @lru_cache
 def detect_if_is_test_data() -> bool:
     """Check if running from a Unit Test file."""
     possible_current_files = [os.path.basename(frame.filename) for frame in inspect.stack()]
-
-    for file_name in possible_current_files:
-        if file_name.startswith('test_') or file_name.endswith('_test.py') or "pytest" in file_name:
-            return True
-    return False
+    is_test_data = any(file_name.startswith('test_') or file_name.endswith('_test.py') or "pytest" in file_name
+                       for file_name in possible_current_files)
+    return is_test_data
 
 
 def get_entity_type_by_table_name(table_name: str) -> int or None:
     """Returns the entity_type_id of the table."""
-    if table_name in table_definition:
-        entity_type_id = table_definition[table_name].get("entity_type_id1")
-        return entity_type_id
+    entity_type_id = table_definition.get(table_name, {}).get("entity_type_id1")
+    return entity_type_id
 
 
 def generate_table_name(schema_name: Optional[str]) -> Optional[str]:
     if schema_name:
         return schema_name + "_table"
 
 
@@ -95,34 +123,40 @@
 def generate_column_name(table_name: Optional[str]) -> Optional[str]:
     if table_name:
         column_name = table_name.replace("_table", "_id")
         return column_name
 
 
 def validate_single_clause_value(select_clause_value: str = None) -> None:
-    if "," in select_clause_value or select_clause_value == "*":
+    if not select_clause_value or "," in select_clause_value or select_clause_value == "*":
         raise ValueError("select value requires a single column name")
 
 
 def get_where_params(column_name: str, column_value: Any) -> tuple:
     # If we use "if column_value:" it will not work for 0, False, etc.
+    if not column_name:
+        raise ValueError(f"column_name is required, got {column_name}")
     if isinstance(column_value, ToSQLInterface):
         where = f"`{column_name}`={column_value.to_sql()}"
         params = None
     elif column_value is not None:
-        where = f"`{column_name}`=%s"
-        params = (column_value,)
+        if isinstance(column_value, (list, tuple, set)):
+            where = f"`{column_name}` IN (" + ",".join(["%s"] * len(column_value)) + ")"
+            params = tuple(column_value)
+        else:
+            where = f"`{column_name}`=%s"
+            params = (column_value,)
     else:
         where = f"`{column_name}` IS NULL"
         params = None
     return where, params
 
 
 def where_skip_null_values(where: str or None, select_clause_value: str,
-                           skip_null_values: bool = False) -> str:
+                           skip_null_values: bool = True) -> str:
     if skip_null_values:
         validate_single_clause_value(select_clause_value)
         where_skip = f"`{select_clause_value}` IS NOT NULL"
         if where:
             where += f" AND {where_skip}"
         else:
             where = where_skip
@@ -132,18 +166,15 @@
 @lru_cache(maxsize=64)
 def replace_view_with_table(view_table_name: str, select_clause_value: str = None) -> str:
     # test data does not appear in the view, but we still wants to access it in tests.
     if not view_table_name:
         return view_table_name
     # Guess the table name from the view name:
     table_name = view_table_name.replace("_view", "_table")
-    scan_table_definition_for_table_name = True
-    if table_name in table_definition:
-        if table_definition[table_name].get("view_name") == view_table_name:
-            scan_table_definition_for_table_name = False
+    scan_table_definition_for_table_name = table_definition.get(table_name, {}).get("view_name") != view_table_name
     if scan_table_definition_for_table_name:
         for table, values in table_definition.items():
             if values["view_name"] == view_table_name:
                 table_name = table  # got a better guess
                 break
     if select_clause_value and select_clause_value != "*":
         requiered_columns = tuple(col.strip() for col in select_clause_value.split(","))  # if columns are specified
@@ -172,14 +203,33 @@
     return column_name in columns
 
 
 def get_table_columns(table_name: str = None) -> tuple:
     table_columns_tuple = table_columns.get(table_name, [])
     return table_columns_tuple
 
+def group_list_by_columns(list_of_dicts: list, group_by: str) -> dict[tuple or str, list[dict]]:
+    group_by = tuple(map(str.strip, group_by.split(",")))
+    if not list_of_dicts:
+        return {}
+    list_of_dicts = copy.deepcopy(list_of_dicts)
+    if any(col not in list_of_dicts[0] for col in group_by):
+        raise ValueError(f"{group_by} should be a subset of {tuple(list_of_dicts[0].keys())}")
+    if len(group_by) == len(list_of_dicts[0]):
+        raise ValueError(f"Column names in group_by must be less than the number of columns in the list of dicts")
+    grouped = {}
+    for dict_row in list_of_dicts:
+        key = tuple(dict_row[col] for col in group_by) if len(group_by) > 1 else dict_row[group_by[0]]
+        if key not in grouped:
+            grouped[key] = []
+        for col in group_by:
+            dict_row.pop(col)
+        grouped[key].append(dict_row)
+    return grouped
+
 # def get_table_columns(schema_name: str = None, table_name: str = None) -> tuple:
 #     select_query = "SELECT column_name " \
 #                    "FROM information_schema.columns " \
 #                    "WHERE TABLE_SCHEMA = %s " \
 #                    "AND TABLE_NAME = %s;"
 #     params = (schema_name, table_name)
 #
```

### Comparing `database_mysql_local-0.0.333/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.334/database_mysql_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.333
+Version: 0.0.334
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.333/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.334/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/pyproject.toml` & `database_mysql_local-0.0.334/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.333/setup.py` & `database_mysql_local-0.0.334/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.333',
+    version='0.0.334',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

