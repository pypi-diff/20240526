# Comparing `tmp/database_mysql_local-0.0.332.tar.gz` & `tmp/database_mysql_local-0.0.333.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.332.tar", last modified: Sat May 25 23:54:33 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.333.tar", last modified: Sun May 26 00:08:13 2024, max compression
```

## Comparing `database_mysql_local-0.0.332.tar` & `database_mysql_local-0.0.333.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:33.985340 database_mysql_local-0.0.332/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 23:54:33.985340 database_mysql_local-0.0.332/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:33.977340 database_mysql_local-0.0.332/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:33.981340 database_mysql_local-0.0.332/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    56309 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30607 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 23:54:00.000000 database_mysql_local-0.0.332/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:54:33.981340 database_mysql_local-0.0.332/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 23:54:33.000000 database_mysql_local-0.0.332/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 23:53:43.000000 database_mysql_local-0.0.332/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:54:33.985340 database_mysql_local-0.0.332/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 23:53:34.000000 database_mysql_local-0.0.332/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:08:13.383366 database_mysql_local-0.0.333/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56529 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30607 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 00:07:31.000000 database_mysql_local-0.0.333/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 00:08:13.000000 database_mysql_local-0.0.333/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 00:07:10.000000 database_mysql_local-0.0.333/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 00:08:13.387366 database_mysql_local-0.0.333/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 00:06:59.000000 database_mysql_local-0.0.333/setup.py
```

### Comparing `database_mysql_local-0.0.332/PKG-INFO` & `database_mysql_local-0.0.333/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.332
+Version: 0.0.333
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.332/README.md` & `database_mysql_local-0.0.333/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.333/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.333/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.333/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.333/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.333/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
                     "GenericCRUD: data_json is deprecated and scheduled to be removed by 12/06/2024, use data_dict instead. "
                     "In general, use _dict when the the typing is dict and _json when the typing is json / str.")
                 printed_dep_warning.append(data_json)
 
             return data_json
 
     def _deprecated_id_column(self, id_column_name: str, column_name: str) -> str:
+        # TODO: once removed, replace `column_value: Any = None` with `column_value: Any` everywhere
         if id_column_name:
             # We let the developers migrate quietly for a week
             if "id_column_name" not in printed_dep_warning:
                 # TODO: print the caller filename
                 self.logger.warning(
                     "GenericCRUD: id_column_name and id_column_value are deprecated and scheduled to be removed by 12/06/2024, use column_name and column_value instead.")
                 printed_dep_warning.append("id_column_name")
@@ -302,40 +303,40 @@
         )
         self.connection.commit()
         self.cursor.execute(select_query, (duplicate_value,))
         existing_duplicate_id = (self.cursor.fetchone() or [None])[0]
         return existing_duplicate_id
 
     def undelete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None, column_name: str = None,
-                                     column_value: Any) -> None:
+                                     column_value: Any = None) -> None:
         """Undeletes a row by setting the end_timestamp to NULL."""
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         column_name = column_name or self.default_column_name
         self._validate_args(args=locals())
         self.update_by_column_and_value(
             schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=column_value,
             data_dict={"end_timestamp": None})
 
     def update_by_id(
-            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any,
+            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
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
-            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any,
+            self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int or None:
         """Updates data in the table by ID."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
         table_name = table_name or self.default_table_name
@@ -385,27 +386,27 @@
         self.cursor.execute(update_query, tuple(data_dict.values()) + params)
         if commit_changes:
             self.connection.commit()
         last_row_id = self.cursor.lastrowid()
         return last_row_id
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
-                     column_name: str = None, column_value: Any,
+                     column_name: str = None, column_value: Any = None,
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
-                                   column_name: str = None, column_value: Any,
+                                   column_name: str = None, column_value: Any = None,
                                    id_column_name: str = None, id_column_value: Any = None) -> int:
         """Deletes data from the table by id"""
         # checks are done inside delete_by_where
         column_name = self._deprecated_id_column(
             id_column_name, column_name) or self.default_column_name
         column_value = column_value or id_column_value
         if column_name:  # column_value can be empty
@@ -484,86 +485,86 @@
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         result_as_dicts = self.convert_multi_to_dict(result, select_clause_value)
         return result_as_dicts
 
     # TODO: test distinct
     def select_one_tuple_by_id(self, *, schema_name: str = None, view_table_name: str = None,
                                select_clause_value: str = None,
-                               column_name: str = None, column_value: Any,
+                               column_name: str = None, column_value: Any = None,
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
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
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
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
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
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
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
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
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
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         """Selects one value from the table by ID and returns it."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
         select_clause_value = select_clause_value or self.default_select_clause_value
         validate_single_clause_value(select_clause_value)
@@ -609,15 +610,15 @@
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
         if result:
             return result[0]
 
     def select_multi_value_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
         if "select_multi_value_by_id" not in printed_dep_warning:
             self.logger.warning(
                 "GenericCRUD.select_multi_value_by_id is deprecated, use select_multi_value_by_column_and_value instead.")
             printed_dep_warning.append("select_multi_value_by_id")
         result = self.select_multi_value_by_column_and_value(
@@ -625,15 +626,15 @@
             column_name=column_name, column_value=column_value, id_column_name=id_column_name,
             id_column_value=id_column_value, distinct=distinct, limit=limit, order_by=order_by,
             skip_null_values=skip_null_values)
         return result
 
     def select_multi_value_by_column_and_value(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
         """Selects multiple values from the table by ID and returns them as a list."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
         select_clause_value = select_clause_value or self.default_select_clause_value
@@ -655,29 +656,29 @@
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
 
     def select_multi_tuple_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
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
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a
         list of tuples.
         send `column_name=''` if you want to select all rows and ignore default column"""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         column_name = column_name or self.default_column_name
@@ -695,29 +696,29 @@
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return result
 
     def select_multi_dict_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
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
-            column_name: str = None, column_value: Any, id_column_name: str = None, id_column_value: Any = None,
+            column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
         """Selects multiple rows from the table by ID and returns them as a list of dictionaries."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         result = self.select_multi_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, distinct=distinct, limit=limit, order_by=order_by)
```

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.333/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.333/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/point.py` & `database_mysql_local-0.0.333/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.333/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.333/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.333/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.333/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.333/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.333/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.333/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.332
+Version: 0.0.333
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.332/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.333/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/pyproject.toml` & `database_mysql_local-0.0.333/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.332/setup.py` & `database_mysql_local-0.0.333/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.332',
+    version='0.0.333',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

