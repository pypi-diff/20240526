# Comparing `tmp/djdynatable-1.0.0.tar.gz` & `tmp/djdynatable-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djdynatable-1.0.0.tar", last modified: Sun May 19 08:18:30 2024, max compression
+gzip compressed data, was "djdynatable-1.0.1.tar", last modified: Sun May 26 09:16:38 2024, max compression
```

## Comparing `djdynatable-1.0.0.tar` & `djdynatable-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-19 08:18:30.040388 djdynatable-1.0.0/
--rw-r--r--   0 anand      (501) staff       (20)       64 2024-05-19 08:16:57.000000 djdynatable-1.0.0/MANIFEST.in
--rw-r--r--   0 anand      (501) staff       (20)     1296 2024-05-19 08:18:30.040479 djdynatable-1.0.0/PKG-INFO
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-19 08:18:30.038828 djdynatable-1.0.0/djdynatable/
--rw-r--r--   0 anand      (501) staff       (20)        0 2024-05-03 12:00:23.000000 djdynatable-1.0.0/djdynatable/__init__.py
--rw-r--r--   0 anand      (501) staff       (20)      128 2024-05-17 16:35:24.000000 djdynatable-1.0.0/djdynatable/admin.py
--rw-r--r--   0 anand      (501) staff       (20)      536 2024-05-17 16:38:31.000000 djdynatable-1.0.0/djdynatable/apps.py
--rw-r--r--   0 anand      (501) staff       (20)        0 2024-05-03 12:00:23.000000 djdynatable-1.0.0/djdynatable/compat.py
--rw-r--r--   0 anand      (501) staff       (20)     8708 2024-05-19 03:58:11.000000 djdynatable-1.0.0/djdynatable/core.py
--rw-r--r--   0 anand      (501) staff       (20)      531 2024-05-06 09:07:00.000000 djdynatable-1.0.0/djdynatable/exception.py
--rw-r--r--   0 anand      (501) staff       (20)     7968 2024-05-19 03:58:17.000000 djdynatable-1.0.0/djdynatable/handler.py
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-19 08:18:30.040295 djdynatable-1.0.0/djdynatable/migrations/
--rw-r--r--   0 anand      (501) staff       (20)      877 2024-05-06 12:03:51.000000 djdynatable-1.0.0/djdynatable/migrations/0001_initial.py
--rw-r--r--   0 anand      (501) staff       (20)        0 2024-05-06 12:03:51.000000 djdynatable-1.0.0/djdynatable/migrations/__init__.py
--rw-r--r--   0 anand      (501) staff       (20)     3209 2024-05-17 11:12:52.000000 djdynatable-1.0.0/djdynatable/models.py
--rw-r--r--   0 anand      (501) staff       (20)     3155 2024-05-19 08:11:21.000000 djdynatable-1.0.0/djdynatable/response.py
--rw-r--r--   0 anand      (501) staff       (20)     1425 2024-05-14 10:09:07.000000 djdynatable-1.0.0/djdynatable/serializer.py
--rw-r--r--   0 anand      (501) staff       (20)       27 2024-05-17 16:38:31.000000 djdynatable-1.0.0/djdynatable/tests.py
--rw-r--r--   0 anand      (501) staff       (20)      509 2024-05-17 16:38:31.000000 djdynatable-1.0.0/djdynatable/urls.py
--rw-r--r--   0 anand      (501) staff       (20)     5522 2024-05-19 08:11:27.000000 djdynatable-1.0.0/djdynatable/views.py
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-19 08:18:30.039889 djdynatable-1.0.0/djdynatable.egg-info/
--rw-r--r--   0 anand      (501) staff       (20)     1296 2024-05-19 08:18:29.000000 djdynatable-1.0.0/djdynatable.egg-info/PKG-INFO
--rw-r--r--   0 anand      (501) staff       (20)      592 2024-05-19 08:18:30.000000 djdynatable-1.0.0/djdynatable.egg-info/SOURCES.txt
--rw-r--r--   0 anand      (501) staff       (20)        1 2024-05-19 08:18:29.000000 djdynatable-1.0.0/djdynatable.egg-info/dependency_links.txt
--rw-r--r--   0 anand      (501) staff       (20)       27 2024-05-19 08:18:29.000000 djdynatable-1.0.0/djdynatable.egg-info/requires.txt
--rw-r--r--   0 anand      (501) staff       (20)       12 2024-05-19 08:18:29.000000 djdynatable-1.0.0/djdynatable.egg-info/top_level.txt
--rw-r--r--   0 anand      (501) staff       (20)      100 2024-05-03 12:00:23.000000 djdynatable-1.0.0/pyproject.toml
--rw-r--r--   0 anand      (501) staff       (20)      893 2024-05-19 08:13:32.000000 djdynatable-1.0.0/readme.md
--rw-r--r--   0 anand      (501) staff       (20)      395 2024-05-19 08:18:30.040691 djdynatable-1.0.0/setup.cfg
--rw-r--r--   0 anand      (501) staff       (20)      468 2024-05-19 08:13:49.000000 djdynatable-1.0.0/setup.py
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:16:38.985843 djdynatable-1.0.1/
+-rw-r--r--   0 anand      (501) staff       (20)       64 2024-05-26 09:07:20.000000 djdynatable-1.0.1/MANIFEST.in
+-rw-r--r--   0 anand      (501) staff       (20)     1311 2024-05-26 09:16:38.985951 djdynatable-1.0.1/PKG-INFO
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:16:38.984016 djdynatable-1.0.1/djdynatable/
+-rw-r--r--   0 anand      (501) staff       (20)        0 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/__init__.py
+-rw-r--r--   0 anand      (501) staff       (20)      128 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/admin.py
+-rw-r--r--   0 anand      (501) staff       (20)      252 2024-05-26 09:08:02.000000 djdynatable-1.0.1/djdynatable/apps.py
+-rw-r--r--   0 anand      (501) staff       (20)     2263 2024-05-26 09:08:36.000000 djdynatable-1.0.1/djdynatable/compat.py
+-rw-r--r--   0 anand      (501) staff       (20)     9577 2024-05-26 09:09:23.000000 djdynatable-1.0.1/djdynatable/core.py
+-rw-r--r--   0 anand      (501) staff       (20)      531 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/exception.py
+-rw-r--r--   0 anand      (501) staff       (20)     8379 2024-05-26 09:10:30.000000 djdynatable-1.0.1/djdynatable/handler.py
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:16:38.985725 djdynatable-1.0.1/djdynatable/migrations/
+-rw-r--r--   0 anand      (501) staff       (20)      877 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/migrations/0001_initial.py
+-rw-r--r--   0 anand      (501) staff       (20)        0 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/migrations/__init__.py
+-rw-r--r--   0 anand      (501) staff       (20)     3209 2024-05-26 09:10:43.000000 djdynatable-1.0.1/djdynatable/models.py
+-rw-r--r--   0 anand      (501) staff       (20)     3155 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/response.py
+-rw-r--r--   0 anand      (501) staff       (20)     1425 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/serializer.py
+-rw-r--r--   0 anand      (501) staff       (20)       27 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/tests.py
+-rw-r--r--   0 anand      (501) staff       (20)      509 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/urls.py
+-rw-r--r--   0 anand      (501) staff       (20)     6639 2024-05-26 09:12:06.000000 djdynatable-1.0.1/djdynatable/utils.py
+-rw-r--r--   0 anand      (501) staff       (20)     6639 2024-05-26 09:11:44.000000 djdynatable-1.0.1/djdynatable/views.py
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:16:38.985307 djdynatable-1.0.1/djdynatable.egg-info/
+-rw-r--r--   0 anand      (501) staff       (20)     1311 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/PKG-INFO
+-rw-r--r--   0 anand      (501) staff       (20)      613 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/SOURCES.txt
+-rw-r--r--   0 anand      (501) staff       (20)        1 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/dependency_links.txt
+-rw-r--r--   0 anand      (501) staff       (20)       27 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/requires.txt
+-rw-r--r--   0 anand      (501) staff       (20)       12 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/top_level.txt
+-rw-r--r--   0 anand      (501) staff       (20)      100 2024-05-26 09:07:20.000000 djdynatable-1.0.1/pyproject.toml
+-rw-r--r--   0 anand      (501) staff       (20)      908 2024-05-26 09:14:32.000000 djdynatable-1.0.1/readme.md
+-rw-r--r--   0 anand      (501) staff       (20)      395 2024-05-26 09:16:38.986262 djdynatable-1.0.1/setup.cfg
+-rw-r--r--   0 anand      (501) staff       (20)      468 2024-05-26 09:14:59.000000 djdynatable-1.0.1/setup.py
```

### Comparing `djdynatable-1.0.0/PKG-INFO` & `djdynatable-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djdynatable
-Version: 1.0.0
+Version: 1.0.1
 Author: Anand Raj
 Author-email: anand98.ar@gmail.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
@@ -27,19 +27,19 @@
 - Django
 - Django-rest-framework
 
 ## 1. Installation
 
 ### 1.1 Initial setup
 
-- Install finflo using [pip](https://pypi.org/project/finflo/)
+- Install djdynatable using [pip](https://pypi.org/project/djdynatable/)
 
 ```bash
 
-pip install finflo
+pip install djdynatable
 
 ```
 
 - In your django application , browse to installed_apps section in settings.py and add this ,
 
 ```bash
```

### Comparing `djdynatable-1.0.0/djdynatable/core.py` & `djdynatable-1.0.1/djdynatable/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 import contextlib
 import importlib
-import os
 from dataclasses import dataclass
 from functools import wraps
 from importlib import import_module, reload
 from typing import Dict, List, Optional, Type
 
 from django.apps import apps
 from django.conf import settings
 from django.contrib import admin
-from django.core.exceptions import ImproperlyConfigured
 from django.db import ProgrammingError, connections, models
 from django.db.backends.base.base import BaseDatabaseWrapper
 from django.db.models import QuerySet
 from django.utils.asyncio import async_unsafe
 from rest_framework import serializers
 from .handler import DynamicTableQueryHandler
 from .exception import BaseException, TableDoesntExistException
-
+from .utils import schema_aware, check_dependencies
 from .models import (
     DEFAULT_FIELD_TYPES,
     DEFAULT_MODEL_ATTRS,
     RELATIONSHIP_FIELD,
     SchemaModel,
     Generated_model_objects,
 )
+from .compat import BASE_SCHEMA_NAME, DJANGO_PROJECT_NAME
 
 
 try:
-    django_project_name = os.environ.get("DJANGO_SETTINGS_MODULE").split(".")[0]
+    from django_tenants.utils import schema_context
 except Exception:
-    raise ImproperlyConfigured(
-        "DJANGO_SETTINGS_MODULE environment variable is not set."
-    )
-
-
+    pass
 """ POTENTIAL WARNING :
     mixed migration and schema model can mingle ,
     never ever use create_model for this below method ,
     causes migrations loss and db clash
 """
 
 
@@ -60,101 +55,116 @@
 @dataclass
 class DynamicTable:
 
     data: Dict
     new_table: bool = False
     model_cls: Optional[Type[models.Model]] = models.Model
     db_conn: Optional[None] = None
+    schema_name: Optional[str] = None
 
-    def __new__(cls, data: Dict, new_table: bool = True):
-        return super().__new__(cls)
+    # def __new__(cls, data: Dict, new_table: bool = True):
+    #     return super().__new__(cls)
 
     def __post_init__(self) -> None:
         self.model_cls: object = self.get_model_cls(self.data)
         self.db_conn: BaseDatabaseWrapper = connections["default"]
         if self.new_table:
             self.create_table()
+        if self.schema_name is None:
+            print("the schema name is ", self.schema_name)
+            self.schema_name = BASE_SCHEMA_NAME
 
     @property
-    def table_name(self):
+    def table_name(self) -> str:
         return self.model_cls._meta.db_table
 
     @property
-    def table_verbose_name(self):
+    def table_verbose_name(self) -> str:
         return self.model_cls._meta.verbose_name
 
     @staticmethod
-    def clear_all_objects():
+    def clear_all_objects() -> None:
         return Generated_model_objects.clear()
 
-    def clear_object(self):
+    def clear_object(self) -> None:
         return Generated_model_objects.pop(self.table_verbose_name)
 
+    @schema_aware(lambda self: self.schema_name)
     @property
     def table_exists(
         self,
     ) -> bool:
         """checks if table exists in database"""
         return bool(
             [
                 table
                 for table in self.db_conn.introspection.table_names()
                 if self.data["tblname"] in table
             ]
         )
 
     @classmethod
-    def load_table_schema(cls, tblname: str) -> "DynamicTable":
-        schema_model = SchemaModel.objects.filter(table_name=tblname)
+    def load_table_schema(cls, tblname: str, schema_name: str = None) -> "DynamicTable":
 
-        if schema_model.exists():
-            return cls(
-                {
-                    "tblname": schema_model.first().table_name,
-                    "columns": schema_model.first().columns,
-                },
-                new_table=False,
+        def get_dynamic_table():
+            schema_model = SchemaModel.objects.filter(table_name=tblname)
+            if schema_model.exists():
+                model_instance = schema_model.first()
+                return cls(
+                    {
+                        "tblname": model_instance.table_name,
+                        "columns": model_instance.columns,
+                    },
+                    new_table=False,
+                    schema_name=schema_name,
+                )
+            raise TableDoesntExistException(
+                code="table_doesnt_exist",
+                detail=f"Table {tblname} does not exist.",
             )
-        raise TableDoesntExistException(
-            code="table_doesnt_exist",
-            detail=f"Table {tblname} does not exists.",
-        )
+
+        if check_dependencies() and schema_name:
+            with schema_context(schema_name):
+                return get_dynamic_table()
+
+        return get_dynamic_table()
 
     @staticmethod
     def unregister_app(app_label, model_name) -> None:
-        try:
+        with contextlib.suppress(LookupError):
             app_config = apps.get_app_config(app_label)
             app_config.models_module = None
             app_config.import_models()
-        except LookupError:
-            pass
 
     def serialize_model_class(self, model_class):
         module_name = model_class.__module__
         class_name = model_class.__name__
         return f"{module_name}.{class_name}"
 
+    @schema_aware(lambda self: self.schema_name)
     def deserialize_model_class(self, model_class_string):
         module_name, class_name = model_class_string.rsplit(".", 1)
         module = importlib.import_module(module_name)
-        model_class = getattr(module, class_name)
-        return model_class
+        return getattr(module, class_name)
 
     @staticmethod
+    @schema_aware(lambda self: self.schema_name)
     def register_app() -> None:
         with contextlib.suppress(Exception):
             admin.site.register(DynamicTable.model_cls)
         reload(import_module(settings.ROOT_URLCONF))
 
     def handle_column_changes(
         self,
         coldef: Dict,
         serializer: serializers.Serializer,
-    ):
-        table_query = DynamicTableQueryHandler(data=self.data, model_cls=self.model_cls)
+    ) -> None:
+        table_query = DynamicTableQueryHandler(
+            data=self.data, model_cls=self.model_cls, schema_name=self.schema_name
+        )
         change_actions = {
             "add": table_query.add_column,
             "remove": table_query.remove_column,
             "alter": table_query.alter_column,
             "rename_table": lambda data: table_query.rename_db_table(
                 old_table_name=self.table_name, new_table_name=data["new_table_name"]
             ),
@@ -162,28 +172,29 @@
 
         change_type = coldef["change"]
         if change_type in change_actions:
             change_actions[change_type](serializer.data)
         else:
             raise ValueError(f"Unsupported change type: {change_type}")
 
+    @schema_aware(lambda self: self.schema_name)
     def get_model_cls(self, data: Dict) -> models.Model:
 
-        if Generated_model_objects.get(str(data["tblname"])):
-            return Generated_model_objects[str(data["tblname"])]
+        # if Generated_model_objects.get(str(data["tblname"])):
+        #     return Generated_model_objects[str(data["tblname"])]
 
         class Meta:
             app_label = "tables"
             verbose_name = data["tblname"]
             verbose_name_plural = data["tblname"]
             db_table = "tables_" + data["tblname"]
 
         model_attrs = {
             "__module__": models.Model.__module__,
-            "app_label": f"{django_project_name}.tables",
+            "app_label": f"{DJANGO_PROJECT_NAME}.tables",
             "Meta": Meta,
         }
 
         for col_dict in data["columns"]:
             model_attrs[col_dict["colname"]] = DEFAULT_FIELD_TYPES[col_dict["coltype"]](
                 **DEFAULT_MODEL_ATTRS[col_dict["coltype"]]
             )
@@ -196,33 +207,32 @@
 
         model_klass = type(data["tblname"], (models.Model,), model_attrs)
 
         Generated_model_objects[data["tblname"]] = model_klass
 
         return model_klass
 
+    @schema_aware(lambda self: self.schema_name)
     def create_table(self) -> None:
         try:
             with self.db_conn.schema_editor() as schema_editor:
                 schema_editor.create_model(self.model_cls)
-        except ProgrammingError:
+        except ProgrammingError as e:
             tblexc = BaseException(
                 code="table_create_error",
                 detail=f"Error while creating table: '{self.data['tblname']}.'",
             )
             tblexc.status_code = 400
-            raise tblexc
+            raise tblexc from e
         else:
             schema_model_obj = SchemaModel(
                 table_name=self.data["tblname"], columns=self.data["columns"]
             )
             schema_model_obj.save()
 
-       
-
     def get_fields(self) -> List:
         return [x["colname"] for x in self.data["columns"]]
 
     def get_fields_with_types(self) -> List:
         return [
             DEFAULT_FIELD_TYPES[x["coltype"]](DEFAULT_MODEL_ATTRS[x["coltype"]])
             for x in self.data["columns"]
@@ -238,14 +248,15 @@
                 "fields": self.get_fields(),
             },
         )
         return type(
             "DynamicTableSerializer", (serializers.ModelSerializer,), {"Meta": meta_cls}
         )
 
+    @schema_aware(lambda self: self.schema_name)
     def drop_table(self) -> None:
         """drops the table from database"""
         try:
             with self.db_conn.schema_editor() as schema_editor:
                 schema_editor.delete_model(self.model_cls)
             with contextlib.suppress(Exception) as e:
                 Generated_model_objects.pop(self.data["tblname"])
@@ -254,14 +265,15 @@
                 code="table_delete_error",
                 detail=f"Table {self.data['table_name']} does not exists.",
             )
         else:
             # self.unregister_app(self.data["tblname"], self.data["tblname"])
             SchemaModel.objects.filter(table_name=self.data["tblname"]).delete()
 
+    @schema_aware(lambda self: self.schema_name)
     def get_queryset(self) -> QuerySet:
         return self.model_cls.objects.all()
 
     def __delattr__(self, name: str) -> None:
         pass  # noqa
         # self.drop_table()
```

### Comparing `djdynatable-1.0.0/djdynatable/exception.py` & `djdynatable-1.0.1/djdynatable/exception.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.0/djdynatable/handler.py` & `djdynatable-1.0.1/djdynatable/handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,60 +10,63 @@
     DEFAULT_MODEL_ATTRS,
     RELATIONSHIP_FIELD,
     SchemaModel,
     Generated_model_objects,
 )
 from dataclasses import dataclass
 from django.db import connections
+from .utils import schema_aware
 
 
 @dataclass(slots=True)
 class DynamicTableQueryHandler:
 
     data: Dict
     model_cls: Type[models.Model] = models.Model
+    schema_name: Type[str] = None
     db_conn: Optional[None] = None
 
     def __post_init__(self) -> None:
         self.db_conn: BaseDatabaseWrapper = connections["default"]
 
     def get_modifiers(self, coldef: Dict) -> Dict:
         """returns the column that is being modified"""
         return list(
             filter(
                 lambda col: col["colname"] == coldef["oldcolname"],
                 self.data["columns"],
             )
         )[0]
 
+    @schema_aware(lambda self: self.schema_name)
     def column_to_db(self, coldef: Dict, change: str = "add") -> None:
         schema_table_obj = SchemaModel.objects.filter(
             table_name=self.data["tblname"]
         ).first()
         if change == "add":
             del coldef["change"]
             schema_table_obj.columns.append(coldef)
             schema_table_obj.save()
-        elif change == "remove":
-            schema_table_obj.columns = list(
-                filter(
-                    lambda col: col["colname"] != coldef["colname"],
-                    schema_table_obj.columns,
-                )
-            )
-            schema_table_obj.save()
         elif change == "alter":
             for i in range(len(schema_table_obj.columns)):
                 col = schema_table_obj.columns[i]
                 if col["colname"] == coldef["oldcolname"]:
                     schema_table_obj.columns[i] = {
                         "colname": coldef["colname"],
                         "coltype": coldef["coltype"],
                     }
             schema_table_obj.save()
+        elif change == "remove":
+            schema_table_obj.columns = list(
+                filter(
+                    lambda col: col["colname"] != coldef["colname"],
+                    schema_table_obj.columns,
+                )
+            )
+            schema_table_obj.save()
 
     def get_relation_table_object(self, data: Dict) -> models.Model:
         return (
             get_object_or_404(
                 Generated_model_objects[data["to_table"]], pk=data["to_row_id"]
             )
             if "to_row_id" in data
@@ -75,14 +78,15 @@
     #         self.load_table_schema(data["to_table"]).model_cls.objects.all(),
     #         pk=data["to_row_id"],
     #     )
     #     if "to_row_id" in data
     #     else self.load_table_schema(data["to_table"]).model_cls
     # )
 
+    @schema_aware(lambda self: self.schema_name)
     def add_column(self, coldef: Dict) -> None:
         """adds column to dynamic table and saves metadata to schema table"""
 
         if coldef["coltype"] in RELATIONSHIP_FIELD:
 
             field = DEFAULT_FIELD_TYPES[coldef["coltype"]](
                 to=self.get_relation_table_object(coldef),
@@ -99,120 +103,123 @@
                 **DEFAULT_MODEL_ATTRS[coldef["coltype"]]
             )
         field.column = coldef["colname"]
 
         try:
             with self.db_conn.schema_editor() as schema_editor:
                 schema_editor.add_field(self.model_cls, field)
-        except ProgrammingError:
+        except ProgrammingError as e:
             tblexc = BaseException(
                 code="field_add_error",
                 detail=f"Error while creating field: '{coldef['colname']}'. Field already exists.",
             )
             tblexc.status_code = 400
-            raise tblexc
+            raise tblexc from e
         else:
             self.column_to_db(coldef, "add")
 
+    @schema_aware(lambda self: self.schema_name)
     def remove_column(self, coldef: Dict) -> None:
         """removes column to dynamic table and saves metadata to schema  table"""
         try:
             local_coldef = list(
                 filter(
                     lambda col: col["colname"] == coldef["colname"],
                     self.data["columns"],
                 )
             )[0]
-        except IndexError:
+        except IndexError as e:
             tblexc = BaseException(
                 code="not_found", detail=f"Column '{coldef['colname']}' was not found"
             )
             tblexc.status_code = 404
-            raise tblexc
+            raise tblexc from e
         if local_coldef["coltype"] in RELATIONSHIP_FIELD:
             field = DEFAULT_FIELD_TYPES[local_coldef["coltype"]](
                 to=self.get_relation_table_object(coldef),
                 on_delete=models.DO_NOTHING,
                 blank=True,
                 null=True,
             )
         field = DEFAULT_FIELD_TYPES[local_coldef["coltype"]]()
         field.column = coldef["colname"]
 
         try:
             with self.db_conn.schema_editor() as schema_editor:
                 schema_editor.remove_field(self.model_cls, field)
-        except ProgrammingError:
+        except ProgrammingError as e:
             tblexc = BaseException(
                 code="remove_column_error",
                 detail=f"Error while removing column '{coldef['colname']}'",
             )
             tblexc.status_code = 400
-            raise tblexc
+            raise tblexc from e
         else:
             self.column_to_db(coldef, "remove")
 
+    @schema_aware(lambda self: self.schema_name)
     def alter_column(self, coldef: Dict) -> None:
         try:
             old_column = self.get_modifiers(coldef)
-        except IndexError:
+        except IndexError as e:
             tblexc = BaseException(
                 code="not_found",
                 detail=f"Column '{coldef['oldcolname']}' was not found",
             )
             tblexc.status_code = 404
-            raise tblexc
+            raise tblexc from e
 
         old_field = DEFAULT_FIELD_TYPES[old_column["coltype"]]()
         old_field.column = old_column["colname"]
 
         new_field = DEFAULT_FIELD_TYPES[coldef["coltype"]](
             **DEFAULT_MODEL_ATTRS[coldef["coltype"]]
         )
         new_field.column = coldef["colname"]
         try:
             if old_column["coltype"] != coldef["coltype"]:
                 """check current column type and new column type"""
                 try:
                     self.model_cls.objects.all().update(**{old_column["colname"]: None})
-                except:
+                except Exception:
                     try:
                         self.model_cls.objects.all().update(
                             **{old_column["colname"]: False}
                         )
-                    except:
+                    except Exception:
                         self.model_cls.objects.all().update(
                             **{old_column["colname"]: None}
                         )
             with self.db_conn.schema_editor() as schema_editor:
                 schema_editor.alter_field(self.model_cls, old_field, new_field)
-        except ProgrammingError:
+        except ProgrammingError as exc:
             tblexc = BaseException(
                 code="column_error",
                 detail=f"Column '{coldef['colname']}' already exists.",
             )
             tblexc.status_code = 404
-            raise tblexc
-        except DataError:
+            raise tblexc from exc
+        except DataError as exc:
             tblexc = BaseException(
                 code="data_convert_error",
                 detail=f"Column '{coldef['oldcolname']}' cannot be converted to '{coldef['coltype']}'",
             )
             tblexc.status_code = 404
-            raise tblexc
+            raise tblexc from exc
         else:
             self.column_to_db(coldef, "alter")
 
+    @schema_aware(lambda self: self.schema_name)
     def rename_db_table(self, new_table_name: str, old_table_name: str) -> None:
         """renames the table name"""
         try:
             with self.db_conn.schema_editor() as schema_editor:
                 schema_editor.alter_db_table(
                     model=self.model_cls,
                     old_db_table=old_table_name,
-                    new_db_table="tables_" + new_table_name,
+                    new_db_table=f"tables_{new_table_name}",
                 )
         except ProgrammingError as e:
             BaseException(
                 code="table_rename_error",
                 detail=f"Table {self.data['table_name']} does not exists.",
             )
```

### Comparing `djdynatable-1.0.0/djdynatable/migrations/0001_initial.py` & `djdynatable-1.0.1/djdynatable/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.0/djdynatable/models.py` & `djdynatable-1.0.1/djdynatable/models.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.0/djdynatable/response.py` & `djdynatable-1.0.1/djdynatable/response.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.0/djdynatable/serializer.py` & `djdynatable-1.0.1/djdynatable/serializer.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.0/djdynatable/views.py` & `djdynatable-1.0.1/djdynatable/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,159 @@
-import contextlib
-
 from django.shortcuts import get_object_or_404
-from .response import FailureResponse, SuccessResponse
+from djeasyview.response import FailureResponse, SuccessResponse
 from rest_framework import status
 from rest_framework.parsers import JSONParser
 from rest_framework.permissions import AllowAny
 from rest_framework.response import Response
 from rest_framework.views import APIView
-
+import contextlib
 from .core import DynamicTable
 from .models import DEFAULT_MODEL_ATTRS, SchemaModel
 from .serializer import ColumnChangeSerializer, TableSerializer
+from .utils import schema_aware, BaseDispath
 
 
-class TableListCreateApiView(APIView):
+class TableListCreateApiView(BaseDispath, APIView):
     queryset = None
     serializer_class = TableSerializer
     permission_classes = [AllowAny]
 
+    @schema_aware(lambda self: self.schema_name)
     def base_queryset(self, table_name):
         schema_table = get_object_or_404(SchemaModel, table_name=table_name)
         columns = ["id"] + [x["colname"] for x in schema_table.columns]
         try:
-            table = DynamicTable.load_table_schema(table_name)
-        except:
-            table = DynamicTable.load_table_schema(table_name).clear_all_objects()
+            table = DynamicTable.load_table_schema(
+                table_name, schema_name=str(self.schema_name)
+            )
+        except Exception:
+            table = DynamicTable.load_table_schema(
+                table_name, schema_name=str(self.schema_name)
+            ).clear_all_objects()
 
         return schema_table, table, columns
 
+    @schema_aware(lambda self: self.schema_name)
     def get(self, request):
-        """to get all the rows in that table"""
         with contextlib.suppress(Exception):
-
             table_name = self.request.query_params.get("table_name")
+            table = DynamicTable.load_table_schema(
+                tblname=table_name, schema_name=self.schema_name
+            )
+
             schema_table, table, columns = self.base_queryset(table_name)
             if schema_table:
+                rows = table.get_queryset().values(*columns).order_by("id")
                 return SuccessResponse(
                     {
                         "columns": schema_table.columns,
-                        "rows": (table.get_queryset().values(*columns).order_by("id")),
+                        "rows": (list(rows)),
                     }
                 )
             return SuccessResponse([])
         return FailureResponse("Matching data not found")
 
+    @schema_aware(lambda self: self.schema_name)
     def post(self, request):
         """for table creation"""
         table_serializer = TableSerializer(data=request.data)
         if table_serializer.is_valid():
-            DynamicTable(table_serializer.data, new_table=True)
+            DynamicTable(
+                table_serializer.data,
+                new_table=True,
+                schema_name=self.schema_name,
+            )
             return SuccessResponse(table_serializer.data)
         return FailureResponse(table_serializer.errors, status=400)
 
 
-class TableUpdateDeleteApiView(APIView):
+class TableUpdateDeleteApiView(BaseDispath, APIView):
     queryset = None
     serializer_class = TableSerializer
     permission_classes = [AllowAny]
 
+    @schema_aware(lambda self: self.schema_name)
     def put(self, request, table_name):
         body_data = JSONParser().parse(request)
         serializer = ColumnChangeSerializer(data=body_data)
         if serializer.is_valid():
-            table = DynamicTable.load_table_schema(table_name)
+            table = DynamicTable.load_table_schema(
+                table_name, schema_name=self.schema_name
+            )
             if table.table_exists:
                 table.clear_object()
                 table.handle_column_changes(coldef=body_data, serializer=serializer)
                 return SuccessResponse("Data updated successfully")
             return FailureResponse(f"Table {table_name} does not exists")
         return Response("Something went wrong", status=status.HTTP_400_BAD_REQUEST)
 
+    @schema_aware(lambda self: self.schema_name)
     def delete(self, request, table_name):
-        table = DynamicTable.load_table_schema(table_name)
+        table = DynamicTable.load_table_schema(table_name, schema_name=self.schema_name)
         if table.table_exists:
             table.drop_table()
             return SuccessResponse(f"table {table_name} deleted successfully")
         return FailureResponse(f"table {table_name} does not exists")
 
 
-class RowListCreateUpdateDeleteApiView(APIView):
+class RowListCreateUpdateDeleteApiView(BaseDispath, APIView):
     queryset = None
     permission_classes = [AllowAny]
 
+    @schema_aware(lambda self: self.schema_name)
     def post(self, request, table_name):
-        table = DynamicTable.load_table_schema(table_name)
-        if any(value == "" for value in request.data.values()) == True:
+        table = DynamicTable.load_table_schema(table_name, schema_name=self.schema_name)
+        if any(value == "" for value in request.data.values()):
             table.model_cls.objects.create()
             return SuccessResponse("row created successfully")
         table_serializer = table.get_serializer()(data=request.data)
         if table_serializer.is_valid():
             table_serializer.save()
             return SuccessResponse(table_serializer.data)
         return FailureResponse(table_serializer.errors)
 
+    @schema_aware(lambda self: self.schema_name)
     def get(self, request, table_name):
-        table = DynamicTable.load_table_schema(table_name)
+        table = DynamicTable.load_table_schema(table_name, schema_name=self.schema_name)
         rows = table.model_cls.objects.all()
-        return Response({"rows": rows.values()})
+        return Response({"rows": list(rows.values())})
 
+    @schema_aware(lambda self: self.schema_name)
     def put(self, request, table_name):
         body_data = request.data
-        table = DynamicTable.load_table_schema(table_name)
+        table = DynamicTable.load_table_schema(table_name, schema_name=self.schema_name)
         queryset = table.get_queryset()
-        if any(value is None or value == "" for value in body_data.values()) == True:
+        if any(value is None or value == "" for value in body_data.values()):
             qryst = queryset.filter(id=body_data["id"])
             body_data.pop("id")
             qryst.update(**body_data)
             return SuccessResponse("row updated successfully")
         serializer = table.get_serializer()(
             instance=queryset.get(id=body_data["id"]), data=body_data
         )
         if serializer.is_valid():
             serializer.update(
                 instance=serializer.instance, validated_data=serializer.validated_data
             )
             return SuccessResponse(serializer.data)
         return FailureResponse(serializer.errors)
 
+    @schema_aware(lambda self: self.schema_name)
     def delete(self, request, table_name):
         row_id = self.request.query_params.get("id")
-        table = DynamicTable.load_table_schema(table_name)
+        table = DynamicTable.load_table_schema(
+            table_name,
+            schema_name=self.schema_name,
+        )
         if table.table_exists:
             queryset = table.get_queryset().filter(id=row_id)
             if queryset.exists():
                 queryset.delete()
                 return SuccessResponse(f"row  {row_id} deleted successfully")
-            return FailureResponse(f"matching row not found")
+            return FailureResponse("matching row not found")
         return FailureResponse(f"table {table_name} does not exists")
 
 
 class FieldListApiview(APIView):
     queryset = None
     serializer_class = None
     permission_classes = [AllowAny]
```

### Comparing `djdynatable-1.0.0/djdynatable.egg-info/PKG-INFO` & `djdynatable-1.0.1/djdynatable.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djdynatable
-Version: 1.0.0
+Version: 1.0.1
 Author: Anand Raj
 Author-email: anand98.ar@gmail.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
@@ -27,19 +27,19 @@
 - Django
 - Django-rest-framework
 
 ## 1. Installation
 
 ### 1.1 Initial setup
 
-- Install finflo using [pip](https://pypi.org/project/finflo/)
+- Install djdynatable using [pip](https://pypi.org/project/djdynatable/)
 
 ```bash
 
-pip install finflo
+pip install djdynatable
 
 ```
 
 - In your django application , browse to installed_apps section in settings.py and add this ,
 
 ```bash
```

### Comparing `djdynatable-1.0.0/djdynatable.egg-info/SOURCES.txt` & `djdynatable-1.0.1/djdynatable.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 djdynatable/exception.py
 djdynatable/handler.py
 djdynatable/models.py
 djdynatable/response.py
 djdynatable/serializer.py
 djdynatable/tests.py
 djdynatable/urls.py
+djdynatable/utils.py
 djdynatable/views.py
 djdynatable.egg-info/PKG-INFO
 djdynatable.egg-info/SOURCES.txt
 djdynatable.egg-info/dependency_links.txt
 djdynatable.egg-info/requires.txt
 djdynatable.egg-info/top_level.txt
 djdynatable/migrations/0001_initial.py
```

### Comparing `djdynatable-1.0.0/readme.md` & `djdynatable-1.0.1/readme.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 - Django
 - Django-rest-framework
 
 ## 1. Installation
 
 ### 1.1 Initial setup
 
-- Install finflo using [pip](https://pypi.org/project/finflo/)
+- Install djdynatable using [pip](https://pypi.org/project/djdynatable/)
 
 ```bash
 
-pip install finflo
+pip install djdynatable
 
 ```
 
 - In your django application , browse to installed_apps section in settings.py and add this ,
 
 ```bash
```

