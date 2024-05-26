# Comparing `tmp/sqlalchemy_crud_plus-0.0.2.tar.gz` & `tmp/sqlalchemy_crud_plus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_crud_plus-0.0.2.tar", last modified: Sat Apr 27 04:14:41 2024, max compression
+gzip compressed data, was "sqlalchemy_crud_plus-0.0.3.tar", last modified: Sun May 26 05:53:30 2024, max compression
```

## Comparing `sqlalchemy_crud_plus-0.0.2.tar` & `sqlalchemy_crud_plus-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2024-03-31 13:58:32.068501 sqlalchemy_crud_plus-0.0.2/LICENSE
--rw-r--r--   0        0        0      707 2024-04-26 15:52:26.717913 sqlalchemy_crud_plus-0.0.2/README.md
--rw-r--r--   0        0        0     1518 2024-04-27 04:14:41.302998 sqlalchemy_crud_plus-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      167 2024-04-27 04:14:35.025020 sqlalchemy_crud_plus-0.0.2/sqlalchemy_crud_plus/__init__.py
--rw-r--r--   0        0        0     5943 2024-04-27 04:00:57.436643 sqlalchemy_crud_plus-0.0.2/sqlalchemy_crud_plus/crud.py
--rw-r--r--   0        0        0      590 2024-04-27 04:00:57.437280 sqlalchemy_crud_plus-0.0.2/sqlalchemy_crud_plus/errors.py
--rw-r--r--   0        0        0        0 2024-04-26 15:52:26.721993 sqlalchemy_crud_plus-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      613 2024-04-26 15:52:26.722448 sqlalchemy_crud_plus-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0      738 2024-04-26 15:52:26.722662 sqlalchemy_crud_plus-0.0.2/tests/model.py
--rw-r--r--   0        0        0     3542 2024-04-27 04:00:57.437764 sqlalchemy_crud_plus-0.0.2/tests/test_crud.py
--rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 sqlalchemy_crud_plus-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-31 13:58:32.068501 sqlalchemy_crud_plus-0.0.3/LICENSE
+-rw-r--r--   0        0        0      707 2024-04-26 15:52:26.717913 sqlalchemy_crud_plus-0.0.3/README.md
+-rw-r--r--   0        0        0     1518 2024-05-26 05:53:30.554271 sqlalchemy_crud_plus-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      167 2024-05-26 05:49:06.159951 sqlalchemy_crud_plus-0.0.3/sqlalchemy_crud_plus/__init__.py
+-rw-r--r--   0        0        0     7144 2024-05-26 05:47:55.708370 sqlalchemy_crud_plus-0.0.3/sqlalchemy_crud_plus/crud.py
+-rw-r--r--   0        0        0      590 2024-04-27 04:00:57.437280 sqlalchemy_crud_plus-0.0.3/sqlalchemy_crud_plus/errors.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:52:26.721993 sqlalchemy_crud_plus-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      613 2024-04-26 15:52:26.722448 sqlalchemy_crud_plus-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0      738 2024-04-26 15:52:26.722662 sqlalchemy_crud_plus-0.0.3/tests/model.py
+-rw-r--r--   0        0        0     4458 2024-05-26 05:47:55.708786 sqlalchemy_crud_plus-0.0.3/tests/test_crud.py
+-rw-r--r--   0        0        0     1517 1970-01-01 00:00:00.000000 sqlalchemy_crud_plus-0.0.3/PKG-INFO
```

### Comparing `sqlalchemy_crud_plus-0.0.2/LICENSE` & `sqlalchemy_crud_plus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_crud_plus-0.0.2/README.md` & `sqlalchemy_crud_plus-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_crud_plus-0.0.2/pyproject.toml` & `sqlalchemy_crud_plus-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "v0.0.2"
+version = "v0.0.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/fastapi-practices/sqlalchemy-crud-plus"
 repository = "https://github.com/fastapi-practices/sqlalchemy-crud-plus"
```

### Comparing `sqlalchemy_crud_plus-0.0.2/sqlalchemy_crud_plus/crud.py` & `sqlalchemy_crud_plus-0.0.3/sqlalchemy_crud_plus/crud.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-from typing import Any, Generic, Literal, Sequence, Type, TypeVar
+from typing import Any, Generic, Iterable, Literal, Sequence, Type, TypeVar
 
 from pydantic import BaseModel
 from sqlalchemy import Row, RowMapping, and_, asc, desc, or_, select
 from sqlalchemy import delete as sa_delete
 from sqlalchemy import update as sa_update
 from sqlalchemy.ext.asyncio import AsyncSession
 
@@ -30,14 +30,27 @@
         """
         if kwargs:
             instance = self.model(**obj.model_dump(), **kwargs)
         else:
             instance = self.model(**obj.model_dump())
         session.add(instance)
 
+    async def create_models(self, session: AsyncSession, obj: Iterable[_CreateSchema]) -> None:
+        """
+        Create new instances of a model
+
+        :param session:
+        :param obj:
+        :return:
+        """
+        instance_list = []
+        for i in obj:
+            instance_list.append(self.model(**i.model_dump()))
+        session.add_all(instance_list)
+
     async def select_model_by_id(self, session: AsyncSession, pk: int) -> _Model | None:
         """
         Query by ID
 
         :param session:
         :param pk:
         :return:
@@ -98,48 +111,45 @@
         query = await session.execute(select(self.model))
         return query.scalars().all()
 
     async def select_models_order(
         self,
         session: AsyncSession,
         *columns,
-        model_sort: Literal['skip', 'asc', 'desc'] = 'skip',
+        model_sort: Literal['default', 'asc', 'desc'] = 'default',
     ) -> Sequence[Row | RowMapping | Any] | None:
         """
         Query all rows asc or desc
 
         :param session:
         :param columns:
         :param model_sort:
         :return:
         """
-        if model_sort != 'skip':
-            if len(columns) != 1:
-                raise SelectExpressionError('ACS and DESC only allow you to specify one column for sorting')
         sort_list = []
         for column in columns:
             if hasattr(self.model, column):
                 model_column = getattr(self.model, column)
                 sort_list.append(model_column)
             else:
                 raise ModelColumnError(f'Model column {column} is not found')
         match model_sort:
-            case 'skip':
+            case 'default':
                 query = await session.execute(select(self.model).order_by(*sort_list))
             case 'asc':
                 query = await session.execute(select(self.model).order_by(asc(*sort_list)))
             case 'desc':
                 query = await session.execute(select(self.model).order_by(desc(*sort_list)))
             case _:
                 raise SelectExpressionError(f'select sort expression {model_sort} is not supported')
         return query.scalars().all()
 
     async def update_model(self, session: AsyncSession, pk: int, obj: _UpdateSchema | dict[str, Any], **kwargs) -> int:
         """
-        Update an instance of a model
+        Update an instance of model's primary key
 
         :param session:
         :param pk:
         :param obj:
         :param kwargs:
         :return:
         """
@@ -148,21 +158,49 @@
         else:
             instance_data = obj.model_dump(exclude_unset=True)
         if kwargs:
             instance_data.update(kwargs)
         result = await session.execute(sa_update(self.model).where(self.model.id == pk).values(**instance_data))
         return result.rowcount  # type: ignore
 
+    async def update_model_by_column(
+        self, session: AsyncSession, column: str, column_value: Any, obj: _UpdateSchema | dict[str, Any], **kwargs
+    ) -> int:
+        """
+        Update an instance of model column
+
+        :param session:
+        :param column:
+        :param column_value:
+        :param obj:
+        :param kwargs:
+        :return:
+        """
+        if isinstance(obj, dict):
+            instance_data = obj
+        else:
+            instance_data = obj.model_dump(exclude_unset=True)
+        if kwargs:
+            instance_data.update(kwargs)
+        if hasattr(self.model, column):
+            model_column = getattr(self.model, column)
+        else:
+            raise ModelColumnError(f'Model column {column} is not found')
+        result = await session.execute(
+            sa_update(self.model).where(model_column == column_value).values(**instance_data)
+        )
+        return result.rowcount  # type: ignore
+
     async def delete_model(self, session: AsyncSession, pk: int, **kwargs) -> int:
         """
         Delete an instance of a model
 
         :param session:
         :param pk:
-        :param kwargs:
+        :param kwargs: for soft deletion only
         :return:
         """
         if not kwargs:
             result = await session.execute(sa_delete(self.model).where(self.model.id == pk))
         else:
             result = await session.execute(sa_update(self.model).where(self.model.id == pk).values(**kwargs))
         return result.rowcount  # type: ignore
```

### Comparing `sqlalchemy_crud_plus-0.0.2/sqlalchemy_crud_plus/errors.py` & `sqlalchemy_crud_plus-0.0.3/sqlalchemy_crud_plus/errors.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_crud_plus-0.0.2/tests/conftest.py` & `sqlalchemy_crud_plus-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_crud_plus-0.0.2/tests/model.py` & `sqlalchemy_crud_plus-0.0.3/tests/model.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_crud_plus-0.0.2/tests/test_crud.py` & `sqlalchemy_crud_plus-0.0.3/tests/test_crud.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,14 +31,28 @@
     async with async_db_session() as session:
         for i in range(1, 10):
             query = await session.scalar(select(Ins).where(Ins.id == i))
             assert query.name == f'test_name_{i}'
 
 
 @pytest.mark.asyncio
+async def test_create_models():
+    async with async_db_session.begin() as session:
+        crud = CRUDPlus(Ins)
+        data = []
+        for i in range(1, 10):
+            data.append(ModelSchema(name=f'test_name_{i}'))
+        await crud.create_models(session, data)
+    async with async_db_session() as session:
+        for i in range(1, 10):
+            query = await session.scalar(select(Ins).where(Ins.id == i))
+            assert query.name == f'test_name_{i}'
+
+
+@pytest.mark.asyncio
 async def test_select_model_by_id():
     await create_test_model()
     async with async_db_session() as session:
         crud = CRUDPlus(Ins)
         for i in range(1, 10):
             result = await crud.select_model_by_id(session, i)
             assert result.name == f'test_name_{i}'
@@ -92,15 +106,27 @@
 async def test_update_model():
     await create_test_model()
     async with async_db_session.begin() as session:
         crud = CRUDPlus(Ins)
         data = ModelSchema(name='test_name_update_1')
         result = await crud.update_model(session, 1, data)
         assert result == 1
-        result = await crud.select_model_by_id(session, 1)
+        result = await session.get(Ins, 1)
+        assert result.name == 'test_name_update_1'
+
+
+@pytest.mark.asyncio
+async def test_update_model_by_column():
+    await create_test_model()
+    async with async_db_session.begin() as session:
+        crud = CRUDPlus(Ins)
+        data = ModelSchema(name='test_name_update_1')
+        result = await crud.update_model_by_column(session, 'name', 'test_name_1', data)
+        assert result == 1
+        result = await session.get(Ins, 1)
         assert result.name == 'test_name_update_1'
 
 
 @pytest.mark.asyncio
 async def test_delete_model():
     await create_test_model()
     async with async_db_session.begin() as session:
```

### Comparing `sqlalchemy_crud_plus-0.0.2/PKG-INFO` & `sqlalchemy_crud_plus-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-crud-plus
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asynchronous CRUD operation based on SQLAlchemy2 model
 Home-page: https://github.com/fastapi-practices/sqlalchemy-crud-plus
 Author-Email: Wu Clan <jianhengwu0407@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

