# Comparing `tmp/database_mysql_local-0.0.335.tar.gz` & `tmp/database_mysql_local-0.0.336.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.335.tar", last modified: Sun May 26 04:20:18 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.336.tar", last modified: Sun May 26 06:36:17 2024, max compression
```

## Comparing `database_mysql_local-0.0.335.tar` & `database_mysql_local-0.0.336.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:18.946184 database_mysql_local-0.0.335/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    56398 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30617 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 04:19:47.000000 database_mysql_local-0.0.335/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 04:19:31.000000 database_mysql_local-0.0.335/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 06:36:17.163195 database_mysql_local-0.0.336/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56398 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30951 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 06:35:43.000000 database_mysql_local-0.0.336/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 06:36:17.000000 database_mysql_local-0.0.336/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 06:35:25.000000 database_mysql_local-0.0.336/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 06:36:17.171194 database_mysql_local-0.0.336/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 06:35:17.000000 database_mysql_local-0.0.336/setup.py
```

### Comparing `database_mysql_local-0.0.335/PKG-INFO` & `database_mysql_local-0.0.336/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.335
+Version: 0.0.336
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.335/README.md` & `database_mysql_local-0.0.336/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.336/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.336/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.336/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.336/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.336/database_mysql_local/src/generic_crud_ml.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 
     @lru_cache
     def sql_in_list_by_entity_list_id(self, *, schema_name: str = None, entity_name: str = None,
                                       entity_list_id: int) -> str:
         """Example: select group_id from group.group_list_member_table WHERE group_list_id=1"""
         schema_name = schema_name or self.default_schema_name
         entity_name = entity_name or schema_name
-        ids = self.select_multi_dict_by_id(schema_name=schema_name,
-                                           view_table_name=f"{entity_name}_list_member_view",
-                                           select_clause_value=f"{entity_name}_id",
-                                           column_name=f"{entity_name}_list_id",
-                                           column_value=entity_list_id)
+        ids = super().select_multi_dict_by_id(schema_name=schema_name,
+                                              view_table_name=f"{entity_name}_list_member_view",
+                                              select_clause_value=f"{entity_name}_id",
+                                              column_name=f"{entity_name}_list_id",
+                                              column_value=entity_list_id)
         if ids:
             result = f" IN ({','.join([str(_id[f'{entity_name}_id']) for _id in ids])})"
         else:
             result = " = TRUE"
 
         return result
 
@@ -106,22 +106,22 @@
 
             data_ml_dict[column_name] = table_id
             data_ml_dict["lang_code"] = lang_code_str
 
             # ml_id is the id value of the row in the ml_table_name table
             # we do not allow inserting a new value if exist and there's not is_main column
             if not is_main and not table_definition.get(ml_table_name, {}).get("is_main_column"):
-                already_exists = self.select_one_value_by_where(
+                already_exists = super().select_one_value_by_where(
                     schema_name=schema_name, view_table_name=ml_view_name,
                     where=f"{column_name}=%s AND lang_code=%s", params=(table_id, lang_code_str),
                     select_clause_value=column_name)
                 if already_exists:
                     raise Exception(f"Value already exists in {ml_table_name} table. Use delete / update.")
-            ml_table_id = self.insert(schema_name=schema_name, data_dict=data_ml_dict, table_name=ml_table_name,
-                                      ignore_duplicate=True, commit_changes=False)
+            ml_table_id = super().insert(schema_name=schema_name, data_dict=data_ml_dict, table_name=ml_table_name,
+                                         ignore_duplicate=True, commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
             self.connection.rollback()
             raise e
         finally:
             self.cursor.close()
@@ -184,26 +184,30 @@
         try:
             self.cursor = self.connection.cursor()
             if is_main is not None:
                 if is_main:
                     self._update_old_main_value_to_false(schema_name=schema_name, table_name=table_name,
                                                          table_id=table_id)
                 if data_dict:
-                    self.update_by_column_and_value(schema_name=schema_name, table_name=table_name, column_name=column_name,
-                                      column_value=table_id, data_dict=data_dict, limit=limit, order_by=order_by,
-                                      commit_changes=False)
+                    super().update_by_column_and_value(schema_name=schema_name, table_name=table_name,
+                                                       column_name=column_name,
+                                                       column_value=table_id, data_dict=data_dict, limit=limit,
+                                                       order_by=order_by,
+                                                       commit_changes=False)
                 data_ml_dict[self.is_main_column_name] = is_main
 
             data_ml_dict[column_name] = table_id
             data_ml_dict["lang_code"] = lang_code_str
             column_name = generate_column_name(ml_table_name)
 
-            self.update_by_column_and_value(schema_name=schema_name, table_name=ml_table_name, data_dict=data_ml_dict,
-                              column_name=column_name, column_value=ml_table_id, limit=limit, order_by=order_by,
-                              commit_changes=False)
+            super().update_by_column_and_value(schema_name=schema_name, table_name=ml_table_name,
+                                               data_dict=data_ml_dict,
+                                               column_name=column_name, column_value=ml_table_id, limit=limit,
+                                               order_by=order_by,
+                                               commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
             self.connection.rollback()
             raise e
         finally:
             self.cursor.close()
@@ -252,15 +256,16 @@
             table_id, ml_table_id = self.update_value_by_id(
                 schema_name=schema_name, data_ml_dict=data_ml_dict, ml_table_id=ml_table_id, table_id=table_id,
                 lang_code=lang_code, is_main=is_main, data_dict=data_dict, table_name=table_name,
                 ml_table_name=ml_table_name, limit=limit, order_by=order_by)
         return table_id, ml_table_id
 
     def upsert_value_with_abbreviations(
-            self, *, data_dict: dict = None, data_ml_dict: dict, data_json: dict = None, data_ml_json: dict = None,
+            self, *, data_dict: dict = None, data_ml_dict: dict = None, data_json: dict = None,
+            data_ml_json: dict = None,
             data_json_compare: dict = None, data_dict_compare: dict = None, table_id: int = None, order_by: str = None,
             table_name: str = None, ml_table_name: str = None, schema_name: str = None, lang_code: LangCode = None,
             compare_view_name: str = None, limit: int = DEFAULT_SQL_SELECT_LIMIT) -> (int, list[int]):
         # TODO: after we delete data_ml_json parameter, make data_ml_dict without default value and we can delete the following raise
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
         compare_view_name = compare_view_name or self.default_ml_view_table_name
@@ -344,31 +349,30 @@
                          lang_code: LangCode = None, column_name: str = None, id_column_name: str = None,
                          select_clause_value: str = "*", order_by: str = None) -> (int, int):
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
         ml_view_table_name = ml_view_table_name or self.default_ml_view_table_name
         column_name = column_name or self.default_column_name
         schema_name = schema_name or self.default_schema_name
-        result = self.select_one_tuple_by_where(
+        result = super().select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=ml_view_table_name,
             where=f"{column_name}=%s AND lang_code=%s", params=(table_id, lang_code_str),
             select_clause_value=select_clause_value, order_by=order_by)
 
         return result
 
     def get_values_dict(self, table_id: int, lang_code: LangCode = None,
                         column_name: str = None, id_column_name: str = None, order_by: str = None) -> dict:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
-        column_name = column_name or generate_column_name(
-            self.default_table_name)
-        result = self.select_one_dict_by_where(view_table_name=self.default_ml_view_table_name,
-                                               where=f"{column_name}=%s AND lang_code=%s",
-                                               params=(table_id, lang_code_str),
-                                               order_by=order_by)
+        column_name = column_name or generate_column_name(self.default_table_name)
+        result = super().select_one_dict_by_where(view_table_name=self.default_ml_view_table_name,
+                                                  where=f"{column_name}=%s AND lang_code=%s",
+                                                  params=(table_id, lang_code_str),
+                                                  order_by=order_by)
 
         return result
 
     def get_values_dict_list(self, *, table_id: int, lang_code: LangCode = None,
                              column_name: str = None, id_column_name: str = None,
                              order_by: str = None, schema_name: str = None) -> list:
         schema_name = schema_name or self.default_schema_name
@@ -383,29 +387,28 @@
         return result
 
     def get_main_values_tuple(self, *, table_id: int, column_name: str = None, id_column_name: str = None,
                               select_clause_value: str = "*", order_by: str = None, schema_name: str = None) -> (
             int, int):
         schema_name = schema_name or self.default_schema_name
         column_name = self._deprecated_id_column(id_column_name, column_name)
-        column_name = column_name or generate_column_name(
-            self.default_table_name)
+        column_name = column_name or generate_column_name(self.default_table_name)
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=self.default_ml_view_table_name,
             where=f"{column_name}=%s AND is_main=True", params=(table_id,),
             select_clause_value=select_clause_value, order_by=order_by)
 
         return result
 
     def get_main_values_dict(self, *, table_id: int, column_name: str = None, id_column_name: str = None,
                              select_clause_value: str = "*", order_by: str = None, schema_name: str = None) -> dict:
         schema_name = schema_name or self.default_schema_name
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_name = column_name or self.default_column_name
-        result = self.select_one_dict_by_where(
+        result = super().select_one_dict_by_where(
             schema_name=schema_name, view_table_name=self.default_ml_view_table_name,
             where=f"{column_name}=%s AND is_main=True", params=(table_id,),
             select_clause_value=select_clause_value, order_by=order_by)
 
         return result
 
     def get_id_by_name(self, *, name: str, schema_name: str = None, table_name: str = None, ml_table_name: str = None,
@@ -419,15 +422,15 @@
         ml_table_name = ml_table_name or self.default_ml_table_name
         compare_view_name = compare_view_name or generate_view_name(ml_table_name)
         column_name = column_name or generate_column_name(table_name)
         if is_column_in_table(table_name=ml_table_name, column_name="title"):
             where = "`title`=%s AND lang_code=%s"
         else:
             where = "`name`=%s AND lang_code=%s"
-        result = self.select_one_value_by_where(
+        result = super().select_one_value_by_where(
             schema_name=schema_name, view_table_name=compare_view_name,
             where=where, params=(name, lang_code_str),
             select_clause_value=column_name, order_by=order_by)
         return result
 
     def get_ml_id_by_name(self, *, name: str, schema_name: str = None, ml_table_name: str = None,
                           lang_code: LangCode = None,
@@ -439,58 +442,58 @@
         schema_name = schema_name or self.default_schema_name
         compare_view_name = compare_view_name or generate_view_name(ml_table_name)
         ml_column_name = column_name or generate_column_name(ml_table_name)
         if is_column_in_table(table_name=ml_table_name, column_name="title"):
             where = "title=%s AND lang_code=%s"
         else:
             where = "`name`=%s AND lang_code=%s"
-        result = self.select_one_value_by_where(
+        result = super().select_one_value_by_where(
             schema_name=schema_name, view_table_name=compare_view_name,
             select_clause_value=ml_column_name, order_by=order_by,
             where=where, params=(name, lang_code_str))
         return result
 
     def get_ml_ids_by_id(self, table_id: int, ml_table_name: str = None, lang_code: LangCode = None,
                          column_name: str = None, id_column_name: str = None,
                          ml_column_name: str = None, ml_id_column_name: str = None,
                          order_by: str = None, compare_view_name: str = None, schema_name: str = None) -> list:
         schema_name = schema_name or self.default_schema_name
         column_name = self._deprecated_id_column(id_column_name, column_name)
         ml_column_name = self._deprecated_id_column(ml_id_column_name, ml_column_name)
         lang_code_str = None if lang_code is None else lang_code.value
         compare_view_name = compare_view_name or generate_view_name(ml_table_name)
-        result = self.select_multi_value_by_where(
+        result = super().select_multi_value_by_where(
             schema_name=schema_name, view_table_name=compare_view_name,
             select_clause_value=ml_column_name, order_by=order_by,
             where=f"{column_name}=%s AND lang_code=%s", params=(table_id, lang_code_str))
         return result
 
     def delete_by_name(self, *, name: str, lang_code: LangCode = None) -> int:
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, name=name)
         if is_column_in_table(table_name=self.default_ml_view_table_name, column_name="title"):
             where = "title=%s AND lang_code=%s"
         else:
             where = "`name`=%s AND lang_code=%s"
-        deleted_id = self.delete_by_where(table_name=self.default_ml_table_name, where=where,
-                                          params=(name, lang_code_str))
+        deleted_id = super().delete_by_where(table_name=self.default_ml_table_name, where=where,
+                                             params=(name, lang_code_str))
         return deleted_id
 
     @staticmethod
     def generate_ml_table_name(table_name: str) -> str:
         if table_name:
             ml_table_name = re.sub(r'(_table)$', '_ml_table', table_name)
             return ml_table_name
 
     # Change the old row with is_main=True to is_main=False
     def _update_old_main_value_to_false(self, *, schema_name: str, table_id: int, table_name: str) -> int:
         data_ml_dict = {self.is_main_column_name: False}
         column_name = generate_column_name(table_name)
         where = f"{column_name}=%s AND {self.is_main_column_name} = True"
-        updated_id = self.update_by_where(schema_name=schema_name, table_name=self.default_ml_table_name,
-                                          data_dict=data_ml_dict, where=where, params=(table_id,))
+        updated_id = super().update_by_where(schema_name=schema_name, table_name=self.default_ml_table_name,
+                                             data_dict=data_ml_dict, where=where, params=(table_id,))
         return updated_id
 
     def _get_lang_code_str(self, *, name: str = None, lang_code: LangCode = None,
                            data_ml_dict: dict = None, data_ml_json: dict = None) -> str:
         data_ml_dict = data_ml_dict or self._data_json_to_dict(data_json=data_ml_json)
         if lang_code is None and name is not None:
             lang_code_str = LangCode.detect_lang_code_str(name)
```

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.336/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/point.py` & `database_mysql_local-0.0.336/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.336/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.336/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.336/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.336/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.336/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.336/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.336/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.335
+Version: 0.0.336
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.335/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.336/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/pyproject.toml` & `database_mysql_local-0.0.336/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.335/setup.py` & `database_mysql_local-0.0.336/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.335',
+    version='0.0.336',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

