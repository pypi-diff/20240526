# Comparing `tmp/graphemy-1.0.0rc6.tar.gz` & `tmp/graphemy-1.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphemy-1.0.0rc6.tar", max compression
+gzip compressed data, was "graphemy-1.0.0rc7.tar", max compression
```

## Comparing `graphemy-1.0.0rc6.tar` & `graphemy-1.0.0rc7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1313 2024-05-04 06:58:42.123037 graphemy-1.0.0rc6/graphemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc6/graphemy/database/__init__.py
--rw-r--r--   0        0        0     5638 2024-05-04 06:58:42.139371 graphemy-1.0.0rc6/graphemy/database/operations.py
--rw-r--r--   0        0        0     1672 2024-05-13 03:58:55.132609 graphemy-1.0.0rc6/graphemy/database/utils.py
--rw-r--r--   0        0        0     4319 2024-05-04 06:58:42.142373 graphemy-1.0.0rc6/graphemy/dl.py
--rw-r--r--   0        0        0     3986 2024-05-04 06:58:42.143376 graphemy-1.0.0rc6/graphemy/models.py
--rw-r--r--   0        0        0     8165 2024-05-04 06:58:42.145372 graphemy-1.0.0rc6/graphemy/router.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc6/graphemy/schemas/__init__.py
--rw-r--r--   0        0        0     8141 2024-05-13 17:42:41.139980 graphemy-1.0.0rc6/graphemy/schemas/generators.py
--rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0rc6/graphemy/schemas/models.py
--rw-r--r--   0        0        0     4808 2024-05-04 06:58:42.147374 graphemy-1.0.0rc6/graphemy/setup.py
--rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0rc6/LICENSE
--rw-r--r--   0        0        0     2180 2024-05-13 17:43:30.599854 graphemy-1.0.0rc6/pyproject.toml
--rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0rc6/README.md
--rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 graphemy-1.0.0rc6/PKG-INFO
+-rw-r--r--   0        0        0     1313 2024-05-04 06:58:42.123037 graphemy-1.0.0rc7/graphemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc7/graphemy/database/__init__.py
+-rw-r--r--   0        0        0     5638 2024-05-04 06:58:42.139371 graphemy-1.0.0rc7/graphemy/database/operations.py
+-rw-r--r--   0        0        0     1771 2024-05-16 15:41:00.229255 graphemy-1.0.0rc7/graphemy/database/utils.py
+-rw-r--r--   0        0        0     4319 2024-05-04 06:58:42.142373 graphemy-1.0.0rc7/graphemy/dl.py
+-rw-r--r--   0        0        0     4005 2024-05-16 15:41:37.220215 graphemy-1.0.0rc7/graphemy/models.py
+-rw-r--r--   0        0        0     8273 2024-05-16 15:41:00.259464 graphemy-1.0.0rc7/graphemy/router.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0rc7/graphemy/schemas/__init__.py
+-rw-r--r--   0        0        0     8460 2024-05-16 15:42:16.520947 graphemy-1.0.0rc7/graphemy/schemas/generators.py
+-rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0rc7/graphemy/schemas/models.py
+-rw-r--r--   0        0        0     4822 2024-05-16 15:10:05.941065 graphemy-1.0.0rc7/graphemy/setup.py
+-rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0rc7/LICENSE
+-rw-r--r--   0        0        0     2180 2024-05-16 15:44:16.068116 graphemy-1.0.0rc7/pyproject.toml
+-rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0rc7/README.md
+-rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 graphemy-1.0.0rc7/PKG-INFO
```

### Comparing `graphemy-1.0.0rc6/graphemy/__init__.py` & `graphemy-1.0.0rc7/graphemy/__init__.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc6/graphemy/database/operations.py` & `graphemy-1.0.0rc7/graphemy/database/operations.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc6/graphemy/database/utils.py` & `graphemy-1.0.0rc7/graphemy/database/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,19 @@
     if isinstance(id, list):
         filter = []
         for j, key in enumerate(keys):
             f = []
             if None not in key:
                 for k in range(len(id)):
                     f.append(
-                        id[k] if type(id[k]) == int else id[k][1:] if id[k].startswith('_') else  getattr(model, id[k])
+                        id[k]
+                        if type(id[k]) == int
+                        else id[k][1:]
+                        if id[k].startswith('_')
+                        else getattr(model, id[k])
                         == bindparam(
                             f'p{i}_{j}_{k}',
                             literal_execute=not isinstance(key[k], date),
                         )
                     )
                     params[f'p{i}_{j}_{k}'] = key[k]
                 filter.append(and_(*f))
```

### Comparing `graphemy-1.0.0rc6/graphemy/dl.py` & `graphemy-1.0.0rc7/graphemy/dl.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc6/graphemy/models.py` & `graphemy-1.0.0rc7/graphemy/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,9 +72,9 @@
                     dl_field = get_dl_function(
                         attr_name, attr_type, attr_value
                     )
                     setattr(cls, attr_name, dl_field)
         for attr in to_remove:
             del cls.__annotations__[attr]
 
-    async def permission_getter(info: Info) -> bool:
+    async def permission_getter(info: Info, request_type: str) -> bool:
         return True
```

### Comparing `graphemy-1.0.0rc6/graphemy/router.py` & `graphemy-1.0.0rc7/graphemy/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import sys
 from types import GenericAlias
 from typing import Callable, Dict
 
 import strawberry
-from fastapi import Request
+from fastapi import Request, Response
 from graphql.error import GraphQLError
 from graphql.error.graphql_error import format_error as format_graphql_error
 from sqlalchemy.engine.base import Engine
 from strawberry.fastapi import GraphQLRouter
 from strawberry.http import GraphQLHTTPResponse
 from strawberry.types import ExecutionResult
 
@@ -161,16 +161,20 @@
         if need_query:
             setattr(
                 query,
                 'hello_world',
                 strawberry.field(hello_world),
             )
 
-        async def get_context(request: Request) -> dict:
-            context = await context_getter(request) if context_getter else {}
+        async def get_context(request: Request, response: Response) -> dict:
+            context = (
+                await context_getter(request, response)
+                if context_getter
+                else {}
+            )
             for k, (func, return_class) in functions.items():
                 context[k] = GraphemyDataLoader(
                     load_fn=func
                     if await Setup.get_permission(
                         return_class, context, 'query'
                     )
                     else fake_dl_list
```

### Comparing `graphemy-1.0.0rc6/graphemy/schemas/generators.py` & `graphemy-1.0.0rc7/graphemy/schemas/generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,18 +65,29 @@
             source = (
                 attr.source if isinstance(attr.source, list) else [attr.source]
             )
             target = (
                 attr.target if isinstance(attr.target, list) else [attr.target]
             )
             target = [returned_class.__tablename__ + '.' + t for t in target]
-            filtered_pairs = [(s, t) for s, t in zip(source, target) if not (isinstance(s, int) or s.startswith('_') or isinstance(t, int) or t.startswith('_'))]
-            source, target = zip(*filtered_pairs) if filtered_pairs else ([], [])
-            
-            if len(source)>0 and len(target)>0:
+            filtered_pairs = [
+                (s, t)
+                for s, t in zip(source, target)
+                if not (
+                    isinstance(s, int)
+                    or s.startswith('_')
+                    or isinstance(t, int)
+                    or t.startswith('_')
+                )
+            ]
+            source, target = (
+                zip(*filtered_pairs) if filtered_pairs else ([], [])
+            )
+
+            if len(source) > 0 and len(target) > 0:
                 cls.__table__.append_constraint(
                     ForeignKeyConstraint(source, target)
                 )
                 foreign_keys_info.append((source, target))
         if not attr.dl_name in functions:
             functions[attr.dl_name] = (
                 get_dl_field(attr, returned_class),
@@ -148,15 +159,22 @@
             strawberry.lazy('graphemy.router'),
         ]
         | None = None,
     ) -> return_type:
         """The dynamically generated DataLoader function."""
         filter_args = vars(filters) if filters else None
         source_value = (
-            [ attr if type(attr) == int else attr[1:] if attr.startswith('_') else  getattr(self, attr) for attr in field_value.source]
+            [
+                attr
+                if type(attr) == int
+                else attr[1:]
+                if attr.startswith('_')
+                else getattr(self, attr)
+                for attr in field_value.source
+            ]
             if isinstance(field_value.source, list)
             else getattr(self, field_value.source)
         )
         return await info.context[dl_name].load(
             source_value, {'filters': filter_args}
         )
 
@@ -189,15 +207,15 @@
         )
     filter = strawberry.input(name=f'{cls.__name__}Filter')(Filter)
 
     async def query(
         self, info: Info, filters: filter | None = None
     ) -> list[cls.__strawberry_schema__]:
         if not await cls.permission_getter(
-            info
+            info, 'query'
         ) or not await Setup.get_permission(cls, info.context, 'query'):
             return []
         data = await get_all(cls, filters, Setup.query_filter(cls, info))
         return data
 
     return (
         strawberry.field(
```

### Comparing `graphemy-1.0.0rc6/graphemy/setup.py` & `graphemy-1.0.0rc7/graphemy/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         Returns:
             An instance of a Strawberry permission class that can be used to control access to GraphQL operations.
         """
 
         class IsAuthenticated(BasePermission):
             async def has_permission(self, source, info, **kwargs) -> bool:
                 if not await module.permission_getter(
-                    info
+                    info, request_type
                 ) or not await cls.get_permission(
                     module, info.context, request_type
                 ):
                     info.context['response'].status_code = 403
                     if not 'errors' in info.context['request'].scope:
                         info.context['request'].scope['errors'] = [module]
                     elif not module in info.context['request'].scope['errors']:
```

### Comparing `graphemy-1.0.0rc6/LICENSE` & `graphemy-1.0.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc6/pyproject.toml` & `graphemy-1.0.0rc7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphemy"
-version = "1.0.0-rc.6"
+version = "1.0.0-rc.7"
 description = "A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions."
 authors = ["Matheus Doreto <matheusdoreto.md@gmail.com>"]
 readme = "README.md"
 packages = [{include = "graphemy"}]
 homepage = "https://github.com/MDoreto/graphemy"
 documentation = "https://graphemy.readthedocs.io/en/latest/"
 repository = "https://github.com/MDoreto/graphemy"
```

### Comparing `graphemy-1.0.0rc6/README.md` & `graphemy-1.0.0rc7/README.md`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0rc6/PKG-INFO` & `graphemy-1.0.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphemy
-Version: 1.0.0rc6
+Version: 1.0.0rc7
 Summary: A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions.
 Home-page: https://github.com/MDoreto/graphemy
 License: MIT
 Author: Matheus Doreto
 Author-email: matheusdoreto.md@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 4 - Beta
```

