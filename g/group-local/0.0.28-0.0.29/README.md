# Comparing `tmp/group_local-0.0.28.tar.gz` & `tmp/group_local-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "group_local-0.0.28.tar", last modified: Mon May 20 12:06:55 2024, max compression
+gzip compressed data, was "group_local-0.0.29.tar", last modified: Sun May 26 04:52:41 2024, max compression
```

## Comparing `group_local-0.0.28.tar` & `group_local-0.0.29.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:06:55.457085 group_local-0.0.28/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-20 12:06:55.457085 group_local-0.0.28/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:06:55.453085 group_local-0.0.28/group_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:06:55.453085 group_local-0.0.28/group_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:06:37.000000 group_local-0.0.28/group_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20959 2024-05-20 12:06:37.000000 group_local-0.0.28/group_local/src/group_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-20 12:06:37.000000 group_local-0.0.28/group_local/src/group_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:06:55.457085 group_local-0.0.28/group_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-20 12:06:55.000000 group_local-0.0.28/group_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-20 12:06:55.000000 group_local-0.0.28/group_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:06:55.000000 group_local-0.0.28/group_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 12:06:55.000000 group_local-0.0.28/group_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 12:06:55.000000 group_local-0.0.28/group_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-20 12:06:37.000000 group_local-0.0.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:06:55.457085 group_local-0.0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-20 12:06:37.000000 group_local-0.0.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:52:41.994829 group_local-0.0.29/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-26 04:52:41.994829 group_local-0.0.29/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:52:41.990829 group_local-0.0.29/group_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:52:41.994829 group_local-0.0.29/group_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 04:52:16.000000 group_local-0.0.29/group_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20102 2024-05-26 04:52:16.000000 group_local-0.0.29/group_local/src/group_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-26 04:52:16.000000 group_local-0.0.29/group_local/src/group_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 04:52:41.994829 group_local-0.0.29/group_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-26 04:52:41.000000 group_local-0.0.29/group_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-26 04:52:41.000000 group_local-0.0.29/group_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 04:52:41.000000 group_local-0.0.29/group_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-26 04:52:41.000000 group_local-0.0.29/group_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 04:52:41.000000 group_local-0.0.29/group_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-26 04:52:23.000000 group_local-0.0.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 04:52:41.994829 group_local-0.0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-26 04:52:16.000000 group_local-0.0.29/setup.py
```

### Comparing `group_local-0.0.28/PKG-INFO` & `group_local-0.0.29/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.28
+Version: 0.0.29
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
-Author-email: info@circles.life
+Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: PyMySQL>=1.0.2
-Requires-Dist: pytest>=7.4.0
-Requires-Dist: mysql-connector>=2.2.9
-Requires-Dist: logzio-python-handler>=4.1.0
-Requires-Dist: database-infrastructure-local>=0.0.23
-Requires-Dist: user-context-remote>=0.0.77
+Requires-Dist: database_mysql_local>=0.0.333
+Requires-Dist: logger_local>=0.0.145
+Requires-Dist: language_remote>=0.0.22
+Requires-Dist: user-context-remote>=0.0.84
 
 PyPI Package for Circles group-local Python
```

### Comparing `group_local-0.0.28/group_local/src/group_local.py` & `group_local-0.0.29/group_local/src/group_local.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from typing import Dict
+
+from database_mysql_local.generic_crud_ml import GenericCRUDML
+from language_remote.lang_code import LangCode
+from logger_local.MetaLogger import MetaLogger
+from user_context_remote.user_context import UserContext
+
 from .group_local_constants import GroupLocalConstants
-from database_mysql_local.generic_crud_ml import GenericCRUDML  # noqa: E402
-from user_context_remote.user_context import UserContext  # noqa: E402
-from logger_local.Logger import Logger  # noqa: E402
-from language_remote.lang_code import LangCode  # noqa: E402
 
-logger = Logger.create_logger(object=GroupLocalConstants.GROUP_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 user_context = UserContext()
 
 DEFAULT_SCHEMA_NAME = "group"
 DEFAULT_TABLE_NAME = "group_table"
 DEFAULT_VIEW_TABLE_NAME = "group_view"
 DEFAULT_ID_COLUMN_NAME = "group_id"
 DEFAULT_IS_MAIN_COLUMN_NAME = "is_main_title"
 
 
-# TODO Change to GroupsLocal. GroupLocal is object of one Group.
-class GroupLocal(GenericCRUDML):
+class GroupsLocal(GenericCRUDML, metaclass=MetaLogger,
+                  object=GroupLocalConstants.GROUP_PYTHON_PACKAGE_CODE_LOGGER_OBJECT):
 
     def __init__(self, is_test_data: bool = False):
-        GenericCRUDML.__init__(self, default_schema_name=DEFAULT_SCHEMA_NAME, default_table_name=DEFAULT_TABLE_NAME,
-                               default_id_column_name=DEFAULT_ID_COLUMN_NAME,
-                               is_main_column_name=DEFAULT_IS_MAIN_COLUMN_NAME,
-                               is_test_data=is_test_data)
-
-    def insert_group(self, group_dict: Dict[str, any], ignore_duplicate: bool = False,
-                     lang_code: LangCode = None) -> tuple[int, int]:
+        super().__init__(default_schema_name=DEFAULT_SCHEMA_NAME, default_table_name=DEFAULT_TABLE_NAME,
+                         default_id_column_name=DEFAULT_ID_COLUMN_NAME,
+                         is_main_column_name=DEFAULT_IS_MAIN_COLUMN_NAME,
+                         is_test_data=is_test_data)
+
+    def insert(  # noqa
+            self, *, group_dict: Dict[str, any], ignore_duplicate: bool = False,
+            lang_code: LangCode = None) -> tuple[int, int]:
         """
             Returns the new group_id
             group_dict has to include the following
             for group_ml_table:
             title: str, lang_code: str = None,
             is_main_title: bool = True,
             "description": None,
@@ -56,15 +58,15 @@
                 "members_visibility_id": 1,
                 "description": "description",
                 "is_title_approved": True,
                 "is_description_approved": True,
                 "created_user_id": 1
             }
         """
-        logger.start(object={'data': str(group_dict)})
+
         group_data_dict = {
             "name": group_dict.get('name'),
             "hashtag": group_dict.get('hashtag'),
             "is_approved": group_dict.get('is_approved', None),
             "parent_group_id": group_dict.get('parent_group_id'),
             "is_interest": group_dict.get('is_interest'),
             "non_members_visibility_id": group_dict.get('non_members_visibility_id', 1),
@@ -102,15 +104,15 @@
             "system_group_name": group_dict.get('system_group_name', None),
             "main_group_type": group_dict.get('main_group_type', None),
             "is_event": group_dict.get('is_event', False),
             "event_id": group_dict.get('event_id', None),
             "visibility_id": group_dict.get('visibility_id', 1),
         }
 
-        group_id = GenericCRUDML.insert(self, data_dict=group_data_dict, ignore_duplicate=ignore_duplicate)
+        group_id = super().insert(data_dict=group_data_dict, ignore_duplicate=ignore_duplicate)
 
         if not lang_code:
             lang_code = group_dict.get('lang_code') or LangCode.detect_lang_code(group_dict.get('title'))
             if lang_code != LangCode.ENGLISH and lang_code != LangCode.HEBREW:
                 lang_code = LangCode.ENGLISH
         group_ml_data_dict = {
             "lang_code": lang_code.value,
@@ -125,23 +127,22 @@
             "updated_user_id": user_context.get_effective_user_id(),
             "updated_real_user_id": user_context.get_real_user_id(),
             "updated_effective_user_id": user_context.get_effective_user_id(),
             "updated_effective_profile_id": user_context.get_effective_profile_id(),
             "is_title_approved": group_dict.get('is_title_approved', None),
             "is_description_approved": group_dict.get('is_description_approved', None)
         }
-        group_ml_id = GenericCRUDML.insert(self, table_name="group_ml_table", data_dict=group_ml_data_dict,
-                                           ignore_duplicate=ignore_duplicate)
+        group_ml_id = super().insert(table_name="group_ml_table", data_dict=group_ml_data_dict,
+                                     ignore_duplicate=ignore_duplicate)
 
-        logger.end(object={'group_id': group_id, 'group_ml_id': group_ml_id})
         return group_id, group_ml_id
 
-    def upsert_group(self, group_dict: Dict[str, any], data_dict_compare: dict = None,
-                     lang_code: LangCode = None,
-                     order_by: str = "") -> dict:
+    def upsert(self, *,  # noqa
+               group_dict: Dict[str, any], data_dict_compare: dict = None,
+               lang_code: LangCode = None, order_by: str = None) -> dict:
         """
             Returns the new group_id
             group_dict has to include the following
             for group_ml_table:
             title: str, lang_code: str = None,
             is_main_title: bool = True,
             "description": None,
@@ -168,15 +169,15 @@
                 "members_visibility_id": 1,
                 "description": "description",
                 "is_title_approved": True,
                 "is_description_approved": True,
                 "created_user_id": 1
             }
         """
-        logger.start(object={'data': str(group_dict)})
+
         if not lang_code:
             lang_code = group_dict.get('lang_code') or LangCode.detect_lang_code(group_dict.get('title'))
             if lang_code != LangCode.ENGLISH and lang_code != LangCode.HEBREW:
                 lang_code = LangCode.ENGLISH
         if not data_dict_compare:
             data_dict_compare = {
                 "name": group_dict.get('name'),
@@ -234,42 +235,42 @@
             "updated_real_user_id": user_context.get_real_user_id(),
             "updated_effective_user_id": user_context.get_effective_user_id(),
             "updated_effective_profile_id": user_context.get_effective_profile_id(),
             "is_title_approved": group_dict.get('is_title_approved', None),
             "is_description_approved": group_dict.get('is_description_approved', None)
         }
         if "(" and ")" in group_dict.get('title'):
-            group_id, group_ml_ids_list = GenericCRUDML.upsert_value_with_abbreviations(
-                self, table_name="group_table", data_dict=group_data_dict,
+            group_id, group_ml_ids_list = super().upsert_value_with_abbreviations(
+                table_name="group_table", data_dict=group_ml_data_dict,
                 data_ml_dict=group_ml_data_dict,
                 ml_table_name="group_ml_table",
                 lang_code=lang_code,
                 data_dict_compare=data_dict_compare,
                 compare_view_name="group_ml_also_not_approved_view",
                 order_by=order_by
             )
         else:
-            group_id, group_ml_id = GenericCRUDML.upsert_value(
-                self, data_dict=group_data_dict, data_ml_dict=group_ml_data_dict,
+            group_id, group_ml_id = super().upsert_value(
+                data_dict=group_data_dict, data_ml_dict=group_ml_data_dict,
                 ml_table_name="group_ml_table", data_dict_compare=data_dict_compare,
                 lang_code=lang_code, compare_view_name="group_ml_also_not_approved_view",
                 order_by=order_by
             )
             group_ml_ids_list = [group_ml_id]
         upsert_information = {
             "group_id": group_id,
             "group_ml_ids_list": group_ml_ids_list
         }
 
-        # TODO Shall we add upsert_informaiton to the logger.end()?
-        logger.end(object={'group_id': group_id, 'group_ml_ids_list': group_ml_ids_list})
+        # TODO Shall we add upsert_informaiton to the 
+
         return upsert_information
 
-    def update_group(self, group_id: int, group_dict: Dict[str, any], lang_code: LangCode = None) -> None:
-        logger.start(object={'group_id': group_id, 'data': str(group_dict)})
+    def update(self, *, group_id: int, group_dict: Dict[str, any], lang_code: LangCode = None) -> None:
+
         group_data_dict = {
             "name": group_dict.get('name'),
             "hashtag": group_dict.get('hashtag'),
             "is_approved": group_dict.get('is_approved', None),
             "parent_group_id": group_dict.get('parent_group_id'),
             "is_interest": group_dict.get('is_interest'),
             "non_members_visibility_id": group_dict.get('non_members_visibility_id', 1),
@@ -306,15 +307,15 @@
             "profile_id": group_dict.get('profile_id', None),
             "system_group_name": group_dict.get('system_group_name', None),
             "main_group_type": group_dict.get('main_group_type', None),
             "is_event": group_dict.get('is_event', False),
             "event_id": group_dict.get('event_id', None),
             "visibility_id": group_dict.get('visibility_id', 1),
         }
-        GenericCRUDML.update_by_id(self, id_column_value=group_id, data_dict=group_data_dict)
+        super().update_by_column_and_value(column_value=group_id, data_dict=group_data_dict)
         if not lang_code:
             lang_code = group_dict.get('lang_code') or LangCode.detect_lang_code(group_dict.get('title'))
             if lang_code != LangCode.ENGLISH and lang_code != LangCode.HEBREW:
                 lang_code = LangCode.ENGLISH
         group_ml_data_dict = {
             "group_id": group_id,
             "lang_code": lang_code.value,
@@ -325,59 +326,58 @@
             "updated_real_user_id": user_context.get_real_user_id(),
             "updated_effective_user_id": user_context.get_effective_user_id(),
             "updated_effective_profile_id": user_context.get_effective_profile_id(),
             "is_title_approved": group_dict.get('is_title_approved', None),
             "is_description_approved": group_dict.get('is_description_approved', None)
         }
         where_clause = "group_id = %s AND lang_code = %s"
-        GenericCRUDML.update_by_where(
-            self, table_name="group_ml_table",
-            where=where_clause,
-            params=(group_id, lang_code.value),
+        super().update_by_where(
+            table_name="group_ml_table",
+            where=where_clause, params=(group_id, lang_code.value),
             data_dict=group_ml_data_dict
         )
-        logger.end()
 
-    def get_group_dict_by_group_id(self, group_id: int, group_ml_id: int = None,
-                                   view_name: str = "group_view",
-                                   ml_view_name: str = "group_ml_also_not_approved_view") -> Dict[str, any]:
-        logger.start(object={'group_id': group_id})
+    def get_group_dict_by_group_id(
+            self, *, group_id: int, group_ml_id: int = None, view_name: str = "group_view",
+            ml_view_name: str = "group_ml_also_not_approved_view") -> Dict[str, any]:
+
         group_ml_dict = {}
         if group_ml_id:
-            group_ml_dict = self.select_one_dict_by_id(view_table_name=ml_view_name,
-                                                       id_column_value=group_ml_id,
-                                                       id_column_name="group_ml_id")
-        group_dict = self.select_one_dict_by_id(view_table_name=view_name, id_column_value=group_id,
-                                                id_column_name="group_id")
-        logger.end(object={'group_ml_dict': str(group_ml_dict), 'group_dict': str(group_dict)})
+            group_ml_dict = self.select_one_dict_by_column_and_value(view_table_name=ml_view_name,
+                                                                     column_value=group_ml_id,
+                                                                     id_column_name="group_ml_id")
+        group_dict = self.select_one_dict_by_column_and_value(view_table_name=view_name, column_value=group_id,
+                                                              id_column_name="group_id")
+
         return {**group_dict, **group_ml_dict}
 
     def delete_by_group_id(self, group_id: int, group_ml_id: int = None) -> None:
-        logger.start(object={'group_id': group_id})
+
         # Delete from group_table
-        self.delete_by_id(table_name="group_table", id_column_name="group_id", id_column_value=group_id)
+        self.delete_by_column_and_value(table_name="group_table", id_column_name="group_id", column_value=group_id)
         # Delete from group_ml_table
         if group_ml_id:
-            self.delete_by_id(table_name="group_ml_table", id_column_name="group_ml_id", id_column_value=group_ml_id)
-        logger.end()
+            self.delete_by_column_and_value(table_name="group_ml_table", id_column_name="group_ml_id",
+                                            column_value=group_ml_id)
 
     def get_groups_by_group_title(self, group_title: str) -> list:
-        logger.start(object={'group_title': group_title})
+
         groups = []
-        group_ids_dicts_list = self.select_multi_dict_by_id(
-            view_table_name="group_ml_also_not_approved_view", id_column_value=group_title, id_column_name="title",
+        group_ids_dicts_list = self.select_multi_dict_by_column_and_value(
+            view_table_name="group_ml_also_not_approved_view", column_value=group_title, id_column_name="title",
             select_clause_value="group_id, group_ml_id")
         for group_ids_dict in group_ids_dicts_list:
-            group_dict = self.get_group_dict_by_group_id(group_ids_dict.get('group_id'), group_ids_dict.get('group_ml_id'))
+            group_dict = self.get_group_dict_by_group_id(
+                group_id=group_ids_dict.get('group_id'), group_ml_id=group_ids_dict.get('group_ml_id'))
             groups.append(group_dict)
-        logger.end(object={'groups': str(groups)})
+
         return groups
 
     def get_all_groups_names(self, view_table_name: str = "group_ml_also_not_approved_view") -> list[str]:
-        logger.start()
+
         if "ml" in view_table_name:
             select_clause_value = "title"
         else:
             select_clause_value = "name"
         groups_names_dict = self.select_multi_dict_by_where(
             view_table_name="group_ml_also_not_approved_view",
             where="end_timestamp IS NOT %s",
@@ -385,9 +385,9 @@
             distinct=True,
             select_clause_value=select_clause_value
         )
         groups_names = []
         for group_name_dict in groups_names_dict:
             groups_name = group_name_dict.get(select_clause_value)
             groups_names.append(groups_name)
-        logger.end(object={'groups_names': groups_names})
+
         return groups_names
```

### Comparing `group_local-0.0.28/group_local/src/group_local_constants.py` & `group_local-0.0.29/group_local/src/group_local_constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 
 class GroupLocalConstants:
-
     ENGLISH_GROUP_ID = 50001176
     VENTURE_CAPITAL_GROUP_ID = 50001177
     ADVOCATE_GROUP_ID = 50001175
     GROUP_LOCAL_PYTHON_COMPONENT_ID = 285
     GROUP_LOCAL_PYTHON_COMPONENT_NAME = "group-local-python-package"
     DEVELOPER_EMAIL = "tal.g@circ.zone"
     GROUP_PYTHON_PACKAGE_CODE_LOGGER_OBJECT = {
```

### Comparing `group_local-0.0.28/group_local.egg-info/PKG-INFO` & `group_local-0.0.29/group_local.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: group-local
-Version: 0.0.28
+Version: 0.0.29
 Summary: PyPI Package for Circles group-local Python
 Home-page: https://github.com/circles-zone/group-main-local-python-package
 Author: Circles
-Author-email: info@circles.life
+Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: PyMySQL>=1.0.2
-Requires-Dist: pytest>=7.4.0
-Requires-Dist: mysql-connector>=2.2.9
-Requires-Dist: logzio-python-handler>=4.1.0
-Requires-Dist: database-infrastructure-local>=0.0.23
-Requires-Dist: user-context-remote>=0.0.77
+Requires-Dist: database_mysql_local>=0.0.333
+Requires-Dist: logger_local>=0.0.145
+Requires-Dist: language_remote>=0.0.22
+Requires-Dist: user-context-remote>=0.0.84
 
 PyPI Package for Circles group-local Python
```

### Comparing `group_local-0.0.28/setup.py` & `group_local-0.0.29/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import setuptools
 
 PACKAGE_NAME = "group-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/group-local
-    version='0.0.28',
+    version='0.0.29',
     author="Circles",
-    author_email="info@circles.life",
+    author_email="info@circles.ai",
     description="PyPI Package for Circles group-local Python",
     long_description="PyPI Package for Circles group-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/group-main-local-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'PyMySQL>=1.0.2',
-        'pytest>=7.4.0',
-        'mysql-connector>=2.2.9',
-        'logzio-python-handler>= 4.1.0',
-        'database-infrastructure-local>=0.0.23',
-        'user-context-remote>=0.0.77'
+        'database_mysql_local>=0.0.333',
+        'logger_local>=0.0.145',
+        'language_remote>=0.0.22',
+        'user-context-remote>=0.0.84',
     ],
 )
```

