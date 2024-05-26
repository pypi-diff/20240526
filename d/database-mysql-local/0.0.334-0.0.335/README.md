# Comparing `tmp/database_mysql_local-0.0.334.tar.gz` & `tmp/database_mysql_local-0.0.335.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.334.tar", last modified: Sun May 26 03:31:04 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.335.tar", last modified: Sun May 26 04:20:18 2024, max compression
```

## Comparing `database_mysql_local-0.0.334.tar` & `database_mysql_local-0.0.335.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:31:04.579027 database_mysql_local-0.0.334/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 03:31:04.579027 database_mysql_local-0.0.334/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:31:04.575027 database_mysql_local-0.0.334/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:31:04.579027 database_mysql_local-0.0.334/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    56364 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30607 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 03:30:30.000000 database_mysql_local-0.0.334/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:31:04.579027 database_mysql_local-0.0.334/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 03:31:04.000000 database_mysql_local-0.0.334/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 03:30:13.000000 database_mysql_local-0.0.334/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 03:31:04.583027 database_mysql_local-0.0.334/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 03:30:05.000000 database_mysql_local-0.0.334/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:18.946184 database_mysql_local-0.0.335/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56398 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30617 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 04:19:47.000000 database_mysql_local-0.0.335/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 04:20:18.000000 database_mysql_local-0.0.335/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 04:19:31.000000 database_mysql_local-0.0.335/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 04:20:18.954184 database_mysql_local-0.0.335/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 04:19:23.000000 database_mysql_local-0.0.335/setup.py
```

### Comparing `database_mysql_local-0.0.334/PKG-INFO` & `database_mysql_local-0.0.335/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.334
+Version: 0.0.335
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.334/README.md` & `database_mysql_local-0.0.335/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.335/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.335/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.335/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.335/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.335/database_mysql_local/src/generic_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,16 +275,17 @@
             existing_duplicate_id, end_timestamp = row
         end_timestamp = end_timestamp.replace(tzinfo=timezone.utc)
         if datetime.now(timezone.utc) > end_timestamp:
             self.undelete_by_column_and_value(schema_name=schema_name, table_name=table_name, column_name=column_name,
                                               column_value=existing_duplicate_id)
         return existing_duplicate_id
 
+    # TODO: test
     def __get_existing_duplicate_id_without_timestamp(
-            self, schema_name: str, table_name: str, duplicate_column_name: str,
+            self, *, schema_name: str, table_name: str, duplicate_column_name: str,
             duplicate_value: Any, column_name: str) -> int or None:
         select_query = (
             f"SELECT {column_name} "
             f"FROM `{schema_name}`.`{table_name}` "
             f"WHERE {duplicate_column_name} = %s LIMIT 1;"
         )
         self.connection.commit()
@@ -933,15 +934,15 @@
         schema_name = schema_name or self.default_schema_name
         entity_name = entity_name or schema_name
         view_name = view_name or self.default_view_table_name
         select_clause_value = select_clause_value or entity_name + "_id"
         test_entity_id = self.select_one_value_by_id(
             schema_name=schema_name or self.default_schema_name, view_table_name=view_name,
             column_name='is_test_data', column_value='1', select_clause_value=select_clause_value)
-        if not test_entity_id:
+        if not test_entity_id:  # TODO: test
             insert_kwargs = insert_kwargs or {}
             create_kwargs = create_kwargs or {}
             # is_test_data from the constructor should be used in the sons to avoid duplications
             if entity_creator:
                 entity_result = entity_creator(**create_kwargs)
                 test_entity_id = insert_function(entity_result, **insert_kwargs)
             else:
```

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.335/database_mysql_local/src/generic_crud_ml.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = generate_column_name(table_name)
         ml_column_name = generate_column_name(ml_table_name)
 
         # check if the row exists in the ml_table
         name = data_ml_dict.get("title") or data_ml_dict.get("name")
         if not name:
-            raise ValueError("name or title is required for upsert_value")
+            raise ValueError("name or title is required for add_value_if_not_exist")
         table_id = table_id or self.get_id_by_name(
             schema_name=schema_name, table_name=table_name, ml_table_name=ml_table_name, name=name,
             lang_code=lang_code, column_name=column_name, order_by=order_by)
         ml_table_id = self.get_ml_id_by_name(
             schema_name=schema_name, ml_table_name=ml_table_name, name=name, lang_code=lang_code,
             column_name=ml_column_name, order_by=order_by)
         if not table_id:
```

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.335/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/point.py` & `database_mysql_local-0.0.335/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.335/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.335/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.335/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.335/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.335/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.335/database_mysql_local/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     if table_name:
         column_name = table_name.replace("_table", "_id")
         return column_name
 
 
 def validate_single_clause_value(select_clause_value: str = None) -> None:
     if not select_clause_value or "," in select_clause_value or select_clause_value == "*":
-        raise ValueError("select value requires a single column name")
+        raise ValueError(f"select value requires a single column name, got {select_clause_value}")
 
 
 def get_where_params(column_name: str, column_value: Any) -> tuple:
     # If we use "if column_value:" it will not work for 0, False, etc.
     if not column_name:
         raise ValueError(f"column_name is required, got {column_name}")
     if isinstance(column_value, ToSQLInterface):
```

### Comparing `database_mysql_local-0.0.334/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.335/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.334
+Version: 0.0.335
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.334/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.335/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/pyproject.toml` & `database_mysql_local-0.0.335/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.334/setup.py` & `database_mysql_local-0.0.335/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.334',
+    version='0.0.335',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

