# Comparing `tmp/djantic2-1.0.1.tar.gz` & `tmp/djantic2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djantic2-1.0.1.tar", max compression
+gzip compressed data, was "djantic2-1.0.2.tar", last modified: Sun May 26 19:47:13 2024, max compression
```

## Comparing `djantic2-1.0.1.tar` & `djantic2-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,40 @@
--rw-r--r--   0        0        0     1072 2024-03-03 16:04:45.365131 djantic2-1.0.1/LICENSE
--rw-r--r--   0        0        0       57 2024-03-03 16:04:45.365480 djantic2-1.0.1/djantic/__init__.py
--rw-r--r--   0        0        0     5453 2024-03-15 10:04:29.102748 djantic2-1.0.1/djantic/fields.py
--rw-r--r--   0        0        0    10094 2024-03-15 10:04:29.102911 djantic2-1.0.1/djantic/main.py
--rw-r--r--   0        0        0        0 2024-03-03 16:04:45.365684 djantic2-1.0.1/djantic/py.typed
--rw-r--r--   0        0        0      868 2024-03-15 11:50:44.367792 djantic2-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 djantic2-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:47:13.458692 djantic2-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-26 19:46:59.000000 djantic2-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-05-26 19:47:13.458692 djantic2-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-05-26 19:46:59.000000 djantic2-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:47:13.454692 djantic2-1.0.2/djantic/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-26 19:46:59.000000 djantic2-1.0.2/djantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-05-26 19:46:59.000000 djantic2-1.0.2/djantic/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-05-26 19:46:59.000000 djantic2-1.0.2/djantic/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 19:46:59.000000 djantic2-1.0.2/djantic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:47:13.454692 djantic2-1.0.2/djantic2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-05-26 19:47:13.000000 djantic2-1.0.2/djantic2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-26 19:47:13.000000 djantic2-1.0.2/djantic2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:47:13.000000 djantic2-1.0.2/djantic2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 19:47:13.000000 djantic2-1.0.2/djantic2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-26 19:46:59.000000 djantic2-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-26 19:47:13.458692 djantic2-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-26 19:46:59.000000 djantic2-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:47:13.458692 djantic2-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/test_multiple_level_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33382 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/test_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:47:13.458692 djantic2-1.0.2/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/fields.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      627 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:47:13.458692 djantic2-1.0.2/tests/testapp/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/project/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/project/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-26 19:46:59.000000 djantic2-1.0.2/tests/testapp/settings.py
```

### Comparing `djantic2-1.0.1/LICENSE` & `djantic2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djantic2-1.0.1/djantic/fields.py` & `djantic2-1.0.2/djantic/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from enum import Enum
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Union, Optional
+import typing
 from uuid import UUID
 
 from django.utils.functional import Promise
 from pydantic import IPvAnyAddress, Json
 from pydantic.fields import FieldInfo
 from pydantic.v1.fields import Required
 from pydantic_core import PydanticUndefined
@@ -98,15 +99,24 @@
 
 def ModelSchemaField(field: Any, schema_name: str) -> tuple:
     default = Required
     default_factory = None
     description = None
     title = None
     max_length = None
-    python_type = None
+
+    try:
+        deconstructed = field.deconstruct()
+        field_options = deconstructed[3] or {}
+        blank = field_options.pop("blank", False)
+        null = field_options.pop("null", False)
+    except AttributeError:
+        # Field does not have `deconstruct` method, just default to false
+        blank = False
+        null = False
 
     if field.is_relation:
         if not field.related_model:
             internal_type = field.model._meta.pk.get_internal_type()
         else:
             internal_type = field.related_model._meta.pk.get_internal_type()
             if not field.concrete and field.auto_created or field.null:
@@ -114,16 +124,16 @@
 
         pk_type = FIELD_TYPES.get(internal_type, int)
         if field.one_to_many or field.many_to_many:
             python_type = List[Dict[str, pk_type]]
         else:
             python_type = pk_type
 
-        if field.related_model:
-            field = field.target_field
+        if blank or null:
+            python_type = Union[python_type, None]
 
     else:
         if field.choices:
             enum_choices = {}
             for k, v in field.choices:
                 if Promise in type(v).__mro__:
                     v = str(v)
@@ -149,19 +159,14 @@
 
         if python_type is None:
             logger.warning(
                 "%s is currently unhandled, defaulting to str.", field.__class__
             )
             python_type = str
 
-        deconstructed = field.deconstruct()
-        field_options = deconstructed[3] or {}
-        blank = field_options.pop("blank", False)
-        null = field_options.pop("null", False)
-
         if default is Required and field.has_default():
             if callable(field.default):
                 default_factory = field.default
                 default = PydanticUndefined
             else:
                 default = field.default
         elif field.primary_key or blank or null:
@@ -171,25 +176,41 @@
         if (default is not None or NOT_PROVIDED) and field.null:
             python_type = Union[python_type, None]
 
         description = field.help_text
         title = field.verbose_name.title()
 
     if not description:
-        description = field.name
+        related_field_name = None
+        if field.related_model:
+            related_field_name = field.target_field.name
+
+        description = related_field_name or field.name
 
     if (
         getattr(field, "get_internal_type", lambda: None)() in STR_TYPES
         and not field.choices
     ):
         max_length = field.max_length
 
+    field_info = FieldInfo(
+        default=default,
+        default_factory=default_factory,
+        title=title,
+        description=str(description),
+        max_length=max_length,
+    )
+
+    field_is_optional = all([
+        getattr(field, "null", None),
+        field.is_relation,
+        # A list that is null, is the empty list. So there is no need
+        # to make it nullable.
+        typing.get_origin(python_type) is not list
+    ])
+    if field_is_optional:
+        python_type = Optional[python_type]
+
     return (
         python_type,
-        FieldInfo(
-            default=default,
-            default_factory=default_factory,
-            title=title,
-            description=str(description),
-            max_length=max_length,
-        ),
+        field_info
     )
```

### Comparing `djantic2-1.0.1/djantic/main.py` & `djantic2-1.0.2/djantic/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+from enum import Enum
 from functools import reduce
 from itertools import chain
 from typing import Any, Dict, List, Optional, no_type_check, Union
 from typing_extensions import get_origin, get_args
 
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db.models import Manager, Model
@@ -168,14 +169,16 @@
 
         if is_manager and outer_type_ == List[Dict[str, int]]:
             attr = list(attr.all().values("id"))
         elif is_manager:
             attr = list(attr.all())
         elif outer_type_ == int and issubclass(type(attr), Model):
             attr = attr.id
+        elif inspect.isclass(type(attr)) and issubclass(type(attr), Enum):
+            attr = attr.value
         elif issubclass(attr.__class__, ImageFieldFile) and issubclass(
             outer_type_, str
         ):
             attr = attr.name
         return attr
 
     def _get_annotation_objects(self, value, annotation):
```

