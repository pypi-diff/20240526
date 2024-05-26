# Comparing `tmp/database_mysql_local-0.0.338.tar.gz` & `tmp/database_mysql_local-0.0.339.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.338.tar", last modified: Sun May 26 13:28:32 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.339.tar", last modified: Sun May 26 13:55:08 2024, max compression
```

## Comparing `database_mysql_local-0.0.338.tar` & `database_mysql_local-0.0.339.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:28:32.250843 database_mysql_local-0.0.338/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    56809 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 13:27:58.000000 database_mysql_local-0.0.338/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 13:27:39.000000 database_mysql_local-0.0.338/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:55:08.002328 database_mysql_local-0.0.339/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 13:55:08.002328 database_mysql_local-0.0.339/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:55:07.994328 database_mysql_local-0.0.339/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:55:08.002328 database_mysql_local-0.0.339/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56809 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31229 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 13:54:35.000000 database_mysql_local-0.0.339/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:55:08.002328 database_mysql_local-0.0.339/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 13:55:07.000000 database_mysql_local-0.0.339/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 13:55:07.000000 database_mysql_local-0.0.339/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:55:07.000000 database_mysql_local-0.0.339/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 13:55:07.000000 database_mysql_local-0.0.339/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 13:55:07.000000 database_mysql_local-0.0.339/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 13:54:16.000000 database_mysql_local-0.0.339/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 13:55:08.002328 database_mysql_local-0.0.339/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 13:54:08.000000 database_mysql_local-0.0.339/setup.py
```

### Comparing `database_mysql_local-0.0.338/PKG-INFO` & `database_mysql_local-0.0.339/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.338
+Version: 0.0.339
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.338/README.md` & `database_mysql_local-0.0.339/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.339/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.339/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.339/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.339/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.339/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.339/database_mysql_local/src/generic_crud_ml.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,16 @@
             self.cursor = self.connection.cursor()
             # if this is the first insert of this data, is_main should be True
             if is_main is not None:
                 if table_id is None:
                     is_main = True
                 elif is_main:
                     self._update_old_main_value_to_false(
-                        schema_name=schema_name, table_name=table_name, table_id=table_id)
+                        schema_name=schema_name, table_name=table_name, table_id=table_id,
+                        ml_table_name=ml_table_name)
                 if table_definition.get(ml_table_name, {}).get("is_main_column"):
                     data_ml_dict[self.is_main_column_name] = is_main
 
             # id is the id value of the row in the table_name table
             table_id = table_id or super().insert(
                 schema_name=schema_name, table_name=table_name, data_dict=data_dict,
                 ignore_duplicate=True, commit_changes=False)
@@ -184,22 +185,22 @@
             raise ValueError("ml_table_id is required for update_value")
         old_cursor = self.cursor
         try:
             self.cursor = self.connection.cursor()
             if is_main is not None:
                 if is_main:
                     self._update_old_main_value_to_false(schema_name=schema_name, table_name=table_name,
-                                                         table_id=table_id)
-                if data_dict:
-                    super().update_by_column_and_value(schema_name=schema_name, table_name=table_name,
-                                                       column_name=column_name,
-                                                       column_value=table_id, data_dict=data_dict, limit=limit,
-                                                       order_by=order_by,
-                                                       commit_changes=False)
+                                                         table_id=table_id, ml_table_name=ml_table_name)
                 data_ml_dict[self.is_main_column_name] = is_main
+            if data_dict:
+                super().update_by_column_and_value(schema_name=schema_name, table_name=table_name,
+                                                   column_name=column_name,
+                                                   column_value=table_id, data_dict=data_dict, limit=limit,
+                                                   order_by=order_by,
+                                                   commit_changes=False)
 
             data_ml_dict[column_name] = table_id
             data_ml_dict["lang_code"] = lang_code_str
             column_name = generate_column_name(ml_table_name)
 
             super().update_by_column_and_value(schema_name=schema_name, table_name=ml_table_name,
                                                data_dict=data_ml_dict,
@@ -483,19 +484,20 @@
     @staticmethod
     def generate_ml_table_name(table_name: str) -> str:
         if table_name:
             ml_table_name = re.sub(r'(_table)$', '_ml_table', table_name)
             return ml_table_name
 
     # Change the old row with is_main=True to is_main=False
-    def _update_old_main_value_to_false(self, *, schema_name: str, table_id: int, table_name: str) -> int:
+    def _update_old_main_value_to_false(self, *, schema_name: str, table_id: int, table_name: str,
+                                        ml_table_name: str) -> int:
         data_ml_dict = {self.is_main_column_name: False}
         column_name = generate_column_name(table_name)
         where = f"{column_name}=%s AND {self.is_main_column_name} = True"
-        updated_id = super().update_by_where(schema_name=schema_name, table_name=self.default_ml_table_name,
+        updated_id = super().update_by_where(schema_name=schema_name, table_name=ml_table_name,
                                              data_dict=data_ml_dict, where=where, params=(table_id,))
         return updated_id
 
     def _get_lang_code_str(self, *, name: str = None, lang_code: LangCode = None,
                            data_ml_dict: dict = None, data_ml_json: dict = None) -> str:
         data_ml_dict = data_ml_dict or self._data_json_to_dict(data_json=data_ml_json)
         if lang_code is None and name is not None:
```

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.339/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/point.py` & `database_mysql_local-0.0.339/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.339/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.339/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.339/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.339/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.339/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.339/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.339/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.338
+Version: 0.0.339
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.338/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.339/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.338/pyproject.toml` & `database_mysql_local-0.0.339/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.339" # https://pypi.org/project/database-mysql-local
+version = "0.0.340" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.338/setup.py` & `database_mysql_local-0.0.339/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.338',
+    version='0.0.339',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

