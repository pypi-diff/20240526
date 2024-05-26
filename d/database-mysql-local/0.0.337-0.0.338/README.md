# Comparing `tmp/database_mysql_local-0.0.337.tar.gz` & `tmp/database_mysql_local-0.0.338.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.337.tar", last modified: Sun May 26 11:42:25 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.338.tar", last modified: Sun May 26 13:28:32 2024, max compression
```

## Comparing `database_mysql_local-0.0.337.tar` & `database_mysql_local-0.0.338.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:42:25.212522 database_mysql_local-0.0.337/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    56809 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30951 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 11:41:52.000000 database_mysql_local-0.0.337/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 11:42:25.000000 database_mysql_local-0.0.337/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 11:41:34.000000 database_mysql_local-0.0.337/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:42:25.220522 database_mysql_local-0.0.337/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 11:41:26.000000 database_mysql_local-0.0.337/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:28:32.250843 database_mysql_local-0.0.338/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56809 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-26 13:27:58.000000 database_mysql_local-0.0.338/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 13:28:32.000000 database_mysql_local-0.0.338/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 13:27:39.000000 database_mysql_local-0.0.338/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 13:28:32.258843 database_mysql_local-0.0.338/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 13:27:31.000000 database_mysql_local-0.0.338/setup.py
```

### Comparing `database_mysql_local-0.0.337/PKG-INFO` & `database_mysql_local-0.0.338/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.337
+Version: 0.0.338
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.337/README.md` & `database_mysql_local-0.0.338/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.338/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.338/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.338/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.338/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.338/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.338/database_mysql_local/src/generic_crud_ml.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,16 @@
                   is_main: bool or None = False, table_name: str = None,
                   ml_table_name: str = None) -> Optional[tuple]:
         schema_name = schema_name or self.default_schema_name
         data_dict = data_dict or self._data_json_to_dict(data_json=data_json)
         data_ml_dict = data_ml_dict or self._data_json_to_dict(data_json=data_ml_json)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, data_ml_dict=data_ml_dict)
         table_name = table_name or self.default_table_name
+        # I don't think column_name = self.default_column_name is correct, it has to be
+        # the id column name of table_name.
         column_name = column_name or self.default_column_name
         ml_view_name = generate_view_name(ml_table_name) if ml_table_name else self.default_ml_view_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
 
         old_cursor = self.cursor
         try:
             self.cursor = self.connection.cursor()
@@ -247,15 +249,16 @@
             column_name=column_name, order_by=order_by)
         ml_table_id = self.get_ml_id_by_name(
             schema_name=schema_name, ml_table_name=ml_table_name, name=name_compare, lang_code=lang_code,
             compare_view_name=compare_view_name, column_name=ml_column_name, order_by=order_by)
         if not table_id:
             table_id, ml_table_id = self.add_value(
                 schema_name=schema_name, data_ml_dict=data_ml_dict, table_id=table_id, lang_code=lang_code,
-                is_main=is_main, data_dict=data_dict, table_name=table_name, ml_table_name=ml_table_name)
+                is_main=is_main, data_dict=data_dict, table_name=table_name, ml_table_name=ml_table_name,
+                column_name=column_name)
         else:
             table_id, ml_table_id = self.update_value_by_id(
                 schema_name=schema_name, data_ml_dict=data_ml_dict, ml_table_id=ml_table_id, table_id=table_id,
                 lang_code=lang_code, is_main=is_main, data_dict=data_dict, table_name=table_name,
                 ml_table_name=ml_table_name, limit=limit, order_by=order_by)
         return table_id, ml_table_id
```

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.338/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/point.py` & `database_mysql_local-0.0.338/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.338/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.338/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.338/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.338/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.338/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.338/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.338/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.337
+Version: 0.0.338
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.337/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.338/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.337/pyproject.toml` & `database_mysql_local-0.0.338/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.338" # https://pypi.org/project/database-mysql-local
+version = "0.0.339" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.337/setup.py` & `database_mysql_local-0.0.338/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.337',
+    version='0.0.338',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

