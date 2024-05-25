# Comparing `tmp/flamel_orm-0.0.3.tar.gz` & `tmp/flamel_orm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamel_orm-0.0.3.tar", last modified: Wed May 15 18:52:11 2024, max compression
+gzip compressed data, was "flamel_orm-0.0.4.tar", last modified: Sat May 25 22:31:40 2024, max compression
```

## Comparing `flamel_orm-0.0.3.tar` & `flamel_orm-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:52:11.491784 flamel_orm-0.0.3/
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1061 2024-05-06 19:53:28.000000 flamel_orm-0.0.3/LICENSE
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3116 2024-05-15 18:52:11.491784 flamel_orm-0.0.3/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     2684 2024-05-15 18:51:00.000000 flamel_orm-0.0.3/README.md
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:52:11.491784 flamel_orm-0.0.3/flamel/
--rw-rw-r--   0 fernando  (1000) fernando  (1000)       22 2024-05-15 18:51:36.000000 flamel_orm-0.0.3/flamel/__init__.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     2487 2024-05-11 19:46:26.000000 flamel_orm-0.0.3/flamel/base.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     4371 2024-05-05 19:07:21.000000 flamel_orm-0.0.3/flamel/column.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     1690 2024-05-11 19:54:50.000000 flamel_orm-0.0.3/flamel/dialect.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     3024 2024-05-12 19:14:23.000000 flamel_orm-0.0.3/flamel/query.py
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:52:11.491784 flamel_orm-0.0.3/flamel_orm.egg-info/
--rw-r--r--   0 fernando  (1000) fernando  (1000)     3116 2024-05-15 18:52:11.000000 flamel_orm-0.0.3/flamel_orm.egg-info/PKG-INFO
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      360 2024-05-15 18:52:11.000000 flamel_orm-0.0.3/flamel_orm.egg-info/SOURCES.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-15 18:52:11.000000 flamel_orm-0.0.3/flamel_orm.egg-info/dependency_links.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)        7 2024-05-15 18:52:11.000000 flamel_orm-0.0.3/flamel_orm.egg-info/top_level.txt
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      690 2024-05-15 18:51:42.000000 flamel_orm-0.0.3/pyproject.toml
--rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-15 18:52:11.491784 flamel_orm-0.0.3/setup.cfg
-drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-15 18:52:11.491784 flamel_orm-0.0.3/tests/
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     3350 2024-05-11 18:58:02.000000 flamel_orm-0.0.3/tests/test_base.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     3412 2024-05-11 00:54:52.000000 flamel_orm-0.0.3/tests/test_column.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      588 2024-05-11 00:54:52.000000 flamel_orm-0.0.3/tests/test_dialect.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)     5293 2024-05-11 19:52:40.000000 flamel_orm-0.0.3/tests/test_query.py
--rw-rw-r--   0 fernando  (1000) fernando  (1000)      982 2024-05-11 00:54:52.000000 flamel_orm-0.0.3/tests/test_sqlbuilder.py
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-25 22:31:40.489831 flamel_orm-0.0.4/
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1061 2024-05-06 19:53:28.000000 flamel_orm-0.0.4/LICENSE
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2107 2024-05-25 22:31:40.489831 flamel_orm-0.0.4/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1675 2024-05-25 20:22:54.000000 flamel_orm-0.0.4/README.md
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-25 22:31:40.489831 flamel_orm-0.0.4/flamel/
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       22 2024-05-25 20:02:52.000000 flamel_orm-0.0.4/flamel/__init__.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     4952 2024-05-25 22:28:23.000000 flamel_orm-0.0.4/flamel/base.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     4371 2024-05-05 19:07:21.000000 flamel_orm-0.0.4/flamel/column.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     1690 2024-05-11 19:54:50.000000 flamel_orm-0.0.4/flamel/dialect.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     3623 2024-05-25 22:31:28.000000 flamel_orm-0.0.4/flamel/query.py
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-25 22:31:40.489831 flamel_orm-0.0.4/flamel_orm.egg-info/
+-rw-r--r--   0 fernando  (1000) fernando  (1000)     2107 2024-05-25 22:31:40.000000 flamel_orm-0.0.4/flamel_orm.egg-info/PKG-INFO
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      360 2024-05-25 22:31:40.000000 flamel_orm-0.0.4/flamel_orm.egg-info/SOURCES.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)        1 2024-05-25 22:31:40.000000 flamel_orm-0.0.4/flamel_orm.egg-info/dependency_links.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       13 2024-05-25 22:31:40.000000 flamel_orm-0.0.4/flamel_orm.egg-info/top_level.txt
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      690 2024-05-25 20:02:48.000000 flamel_orm-0.0.4/pyproject.toml
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)       38 2024-05-25 22:31:40.489831 flamel_orm-0.0.4/setup.cfg
+drwxrwxr-x   0 fernando  (1000) fernando  (1000)        0 2024-05-25 22:31:40.489831 flamel_orm-0.0.4/tests/
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     5864 2024-05-25 22:29:56.000000 flamel_orm-0.0.4/tests/test_base.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     3412 2024-05-11 00:54:52.000000 flamel_orm-0.0.4/tests/test_column.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      588 2024-05-11 00:54:52.000000 flamel_orm-0.0.4/tests/test_dialect.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)     6726 2024-05-19 00:25:19.000000 flamel_orm-0.0.4/tests/test_query.py
+-rw-rw-r--   0 fernando  (1000) fernando  (1000)      982 2024-05-11 00:54:52.000000 flamel_orm-0.0.4/tests/test_sqlbuilder.py
```

### Comparing `flamel_orm-0.0.3/LICENSE` & `flamel_orm-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.3/flamel/column.py` & `flamel_orm-0.0.4/flamel/column.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.3/flamel/dialect.py` & `flamel_orm-0.0.4/flamel/dialect.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.3/flamel/query.py` & `flamel_orm-0.0.4/flamel/query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from typing import Any, Iterable, List, Optional, Tuple, Union
 
 
 class SQLQueryBuilder:
     @staticmethod
     def select(model: Any, columns: Optional[List[str]] = None) -> str:
         if columns is None or not columns:
@@ -34,14 +35,30 @@
     def limit(limit: int, offset: Optional[int] = None) -> str:
         if offset is None:
             return f" LIMIT {limit}"
         else:
             return f" LIMIT {limit} OFFSET {offset}"
 
 
+def validate_sql(query: str) -> bool:
+    patterns = [
+        re.compile(r"SELECT\s+[\w\*,\s]+\s+FROM\s+\w+(\s+WHERE\s+.+)?;", re.IGNORECASE),
+        re.compile(
+            r"INSERT\s+INTO\s+\w+\s*\(?.*\)?\s+VALUES\s*\(?.*\)?;", re.IGNORECASE
+        ),
+        re.compile(r"UPDATE\s+\w+\s+SET\s+[\w=,\s]+(\s+WHERE\s+.+)?;", re.IGNORECASE),
+        re.compile(r"DELETE\s+FROM\s+\w+(\s+WHERE\s+.+)?;", re.IGNORECASE),
+    ]
+
+    if not any(pattern.match(query) for pattern in patterns):
+        raise ValueError("Invalid SQL: Syntax error or unsupported query type.")
+
+    return True
+
+
 class Query:
     def __init__(self, model, conn):
         self.model = model
         self.conn = conn
         self.query_builder = SQLQueryBuilder()
         self.query = None
         self.values = []
```

### Comparing `flamel_orm-0.0.3/pyproject.toml` & `flamel_orm-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flamel-orm"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name = "fernando24164", email = "fernando24164@gmail.com" },
 ]
 description = "A simple declarative ORM for SQLite"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["ORM", "simple"]
```

### Comparing `flamel_orm-0.0.3/tests/test_column.py` & `flamel_orm-0.0.4/tests/test_column.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.3/tests/test_dialect.py` & `flamel_orm-0.0.4/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `flamel_orm-0.0.3/tests/test_query.py` & `flamel_orm-0.0.4/tests/test_query.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest import TestCase
 from unittest.mock import MagicMock, patch
 
 from flamel.base import Base
 from flamel.column import Column, Integer, String, ForeignKey
-from flamel.query import Query, SQLQueryBuilder
+from flamel.query import Query, SQLQueryBuilder, validate_sql
 
 
 class TestQuery(TestCase):
     def test_initializes_query_builder_attribute(self):
         model = "TestModel"
         conn = "TestConnection"
         query = Query(model, conn)
@@ -60,15 +60,19 @@
     def test_sql_builder_order_by_multiple_columns(self):
         class SubClass5(Base):
             id = Column("id", Integer, primary_key=True, autoincrement=True)
             name = Column("name", String, nullable=False)
             age = Column("age", Integer, nullable=False)
 
         Base.set_engine(":memory:")
-        query = SubClass5.query().select("id", "name", "age").order_by("name", "age", direction="DESC")
+        query = (
+            SubClass5.query()
+            .select("id", "name", "age")
+            .order_by("name", "age", direction="DESC")
+        )
         query = str(query)
         assert query == "SELECT id, name, age FROM SubClass5 ORDER BY name, age DESC"
 
     def test_sql_builder_limit_and_offset(self):
         class SubClass6(Base):
             id = Column("id", Integer, primary_key=True, autoincrement=True)
             name = Column("name", String, nullable=False)
@@ -92,29 +96,39 @@
                 Integer,
                 foreign_key=ForeignKey("sub_class7_id", "SubClass7", "id"),
             )
 
         Base.set_engine(":memory:")
 
         with self.assertRaises(ValueError):
-            query = SubClass8.query().join("LEFT", "SubClass7", "SubClass8.sub_class7_id = SubClass7.id")
+            query = SubClass8.query().join(
+                "LEFT", "SubClass7", "SubClass8.sub_class7_id = SubClass7.id"
+            )
             query = str(query)
 
     def test_sql_builder_multiple_joins(self):
         class SubClass9(Base):
             id = Column("id", Integer, primary_key=True, autoincrement=True)
             name = Column("name", String, nullable=False)
 
         class SubClass10(Base):
             id = Column("id", Integer, primary_key=True, autoincrement=True)
-            sub_class9_id = Column("sub_class9_id", Integer, foreign_key=ForeignKey("sub_class9_id", "SubClass9", "id"))
+            sub_class9_id = Column(
+                "sub_class9_id",
+                Integer,
+                foreign_key=ForeignKey("sub_class9_id", "SubClass9", "id"),
+            )
 
         class SubClass11(Base):
             id = Column("id", Integer, primary_key=True, autoincrement=True)
-            sub_class10_id = Column("sub_class10_id", Integer, foreign_key=ForeignKey("sub_class10_id", "SubClass10", "id"))
+            sub_class10_id = Column(
+                "sub_class10_id",
+                Integer,
+                foreign_key=ForeignKey("sub_class10_id", "SubClass10", "id"),
+            )
 
         Base.set_engine(":memory:")
 
         query = (
             SubClass11.query()
             .select("SubClass11.id", "SubClass9.name", "SubClass10.id")
             .join("LEFT", "SubClass10", "SubClass11.sub_class10_id = SubClass10.id")
@@ -124,7 +138,37 @@
 
         assert query == (
             "SELECT SubClass11.id, SubClass9.name, SubClass10.id "
             "FROM SubClass11 "
             "LEFT JOIN SubClass10 ON SubClass11.sub_class10_id = SubClass10.id "
             "LEFT JOIN SubClass9 ON SubClass10.sub_class9_id = SubClass9.id"
         )
+
+
+class TestValidateSQL(TestCase):
+    def test_valid_select_query(self):
+        query = "SELECT name, age FROM users WHERE age > 21;"
+        self.assertTrue(validate_sql(query), "Valid SELECT query should pass.")
+
+    def test_valid_insert_query(self):
+        query = "INSERT INTO users (name, age) VALUES ('Alice', 30);"
+        self.assertTrue(validate_sql(query), "Valid INSERT query should pass.")
+
+    def test_invalid_sql_missing_keyword(self):
+        query = "SELECT name, age users WHERE age > 21;"
+        with self.assertRaises(ValueError) as context:
+            validate_sql(query)
+        self.assertEqual(
+            str(context.exception),
+            "Invalid SQL: Syntax error or unsupported query type.",
+            "Invalid SQL missing keyword should raise ValueError.",
+        )
+
+    def test_invalid_sql_unsupported_structure(self):
+        query = "CREATE TABLE users (id INT, name TEXT);"
+        with self.assertRaises(ValueError) as context:
+            validate_sql(query)
+        self.assertEqual(
+            str(context.exception),
+            "Invalid SQL: Syntax error or unsupported query type.",
+            "Unsupported SQL structure should raise ValueError.",
+        )
```

### Comparing `flamel_orm-0.0.3/tests/test_sqlbuilder.py` & `flamel_orm-0.0.4/tests/test_sqlbuilder.py`

 * *Files identical despite different names*

