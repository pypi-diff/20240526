# Comparing `tmp/database_mysql_local-0.0.329.tar.gz` & `tmp/database_mysql_local-0.0.330.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.329.tar", last modified: Sat May 25 15:09:38 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.330.tar", last modified: Sat May 25 15:23:53 2024, max compression
```

## Comparing `database_mysql_local-0.0.329.tar` & `database_mysql_local-0.0.330.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:09:38.566106 database_mysql_local-0.0.329/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    56240 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30343 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 15:09:06.000000 database_mysql_local-0.0.329/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 15:09:38.000000 database_mysql_local-0.0.329/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 15:08:49.000000 database_mysql_local-0.0.329/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 15:09:38.570106 database_mysql_local-0.0.329/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 15:08:40.000000 database_mysql_local-0.0.329/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:23:53.857298 database_mysql_local-0.0.330/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56240 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30519 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   650975 2024-05-25 15:23:16.000000 database_mysql_local-0.0.330/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 15:23:53.000000 database_mysql_local-0.0.330/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-25 15:22:59.000000 database_mysql_local-0.0.330/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 15:23:53.865298 database_mysql_local-0.0.330/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 15:22:51.000000 database_mysql_local-0.0.330/setup.py
```

### Comparing `database_mysql_local-0.0.329/PKG-INFO` & `database_mysql_local-0.0.330/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.329
+Version: 0.0.330
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.329/README.md` & `database_mysql_local-0.0.330/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.330/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.330/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.330/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.330/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.330/database_mysql_local/src/generic_crud_ml.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,27 +21,29 @@
 class GenericCRUDML(GenericCRUD, metaclass=MetaLogger, object=LOGGER_CRUD_ML_CODE_OBJECT):
     """A class that provides generic CRUD functionality for tables with multi-language support."""
 
     # TODO: allow overiding all default values in all methods
     def __init__(self, default_schema_name: str,
                  default_table_name: str = None, default_view_table_name: str = None,
                  default_ml_table_name: str = None, default_ml_view_table_name: str = None,
+                 default_view_with_deleted_and_test_data: str = None,
                  default_column_name: str = None, default_id_column_name: str = None,
                  is_main_column_name: str = IS_MAIN_COLUMN_NAME, is_test_data: bool = False) -> None:
         """Initializes the GenericCRUDML class. If connection is not provided,
         a new connection will be created."""
         self.default_table_name = default_table_name or (default_ml_table_name or "").replace("_ml", "")
         self.default_ml_table_name = default_ml_table_name or self.generate_ml_table_name(default_table_name)
         self.default_ml_view_table_name = default_ml_view_table_name or generate_view_name(self.default_ml_table_name)
         self.logger.info("GenericCRUDML.__init__", object={
             "default_ml_table_name": self.default_ml_table_name,
             "default_ml_view_table_name": self.default_ml_view_table_name})
         super().__init__(default_schema_name=default_schema_name,
                          default_table_name=self.default_table_name,
                          default_view_table_name=default_view_table_name,
+                         default_view_with_deleted_and_test_data=default_view_with_deleted_and_test_data,
                          default_column_name=default_column_name or default_id_column_name,
                          is_test_data=is_test_data)
         self.user_context = UserContext()
         # TODO: we may have to change it to a list when we will have multiple is_main columns
         self.is_main_column_name = is_main_column_name
 
     @lru_cache
```

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.330/database_mysql_local/src/generic_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from .generic_crud import GenericCRUD
 
 
 class GenericMapping(GenericCRUD, metaclass=MetaLogger, object=LOGGER_MAPPING_CODE_OBJECT):
     def __init__(self, default_schema_name: str = None,
                  default_table_name: str = None,
                  default_view_table_name: str = None,
+                 default_view_with_deleted_and_test_data: str = None,
                  default_id_column_name: str = None, default_column_name: str = None,
                  default_entity_name1: str = None,
                  default_entity_name2: str = None,
                  is_test_data: bool = False):
         default_column_name = default_column_name or default_id_column_name
         GenericCRUD.__init__(self, default_schema_name=default_schema_name,
                              default_table_name=default_table_name, default_view_table_name=default_view_table_name,
+                             default_view_with_deleted_and_test_data=default_view_with_deleted_and_test_data,
                              default_id_column_name=default_column_name, is_test_data=is_test_data)
         self.default_entity_name1 = default_entity_name1
         self.default_entity_name2 = default_entity_name2
 
     # We added the schema_name parameter to avoid using USE and void creating a new instance/object
     # of the database for mapping.
     def insert_mapping(self, *, entity_id1: int, entity_id2: int,
```

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/point.py` & `database_mysql_local-0.0.330/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.330/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.330/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from .generic_crud import GenericCRUD
 
 
 # TODO: use meta logger
 class SyncConflictResolution(GenericCRUD):
     def __init__(self, default_schema_name: str = None, default_table_name: str = None,
                  default_view_table_name: str = None,
+                 default_view_with_deleted_and_test_data: str = None,
                  default_id_column_name: str = None, default_column_name: str = None,
                  default_select_clause_value: str = "updated_timestamp",
                  default_where: str = None):
         default_column_name = default_id_column_name or default_column_name
         GenericCRUD.__init__(self, default_schema_name=default_schema_name, default_table_name=default_table_name,
                              default_view_table_name=default_view_table_name,
+                             default_view_with_deleted_and_test_data=default_view_with_deleted_and_test_data,
                              default_id_column_name=default_column_name,
                              default_select_clause_value=default_select_clause_value, default_where=default_where)
 
     def get_update_status_by_where(self, *, schema_name: str = None, view_table_name: str = None,
                                    where: str = None, params: tuple, select_clause_value: str = None,
                                    remote_last_modified_timestamp: str, ) -> UpdateStatus:
         """
```

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.330/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.330/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.330/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.330/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.330/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.329
+Version: 0.0.330
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.329/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.330/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.329/pyproject.toml` & `database_mysql_local-0.0.330/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.330" # https://pypi.org/project/database-mysql-local
+version = "0.0.331" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.329/setup.py` & `database_mysql_local-0.0.330/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.329',
+    version='0.0.330',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

