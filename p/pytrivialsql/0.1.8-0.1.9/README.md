# Comparing `tmp/pytrivialsql-0.1.8.tar.gz` & `tmp/pytrivialsql-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrivialsql-0.1.8.tar", last modified: Fri May 10 19:04:41 2024, max compression
+gzip compressed data, was "pytrivialsql-0.1.9.tar", last modified: Sun May 26 03:46:56 2024, max compression
```

## Comparing `pytrivialsql-0.1.8.tar` & `pytrivialsql-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.534484 pytrivialsql-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/src/pytrivialsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/src/pytrivialsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/src/pytrivialsql/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/src/pytrivialsql/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/src/pytrivialsql/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 19:04:41.000000 pytrivialsql-0.1.8/src/pytrivialsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:04:41.538483 pytrivialsql-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/tests/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/tests/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-10 19:04:26.000000 pytrivialsql-0.1.8/tests/test_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:46:56.613683 pytrivialsql-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-26 03:46:56.613683 pytrivialsql-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 03:46:56.613683 pytrivialsql-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:46:56.609683 pytrivialsql-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:46:56.609683 pytrivialsql-0.1.9/src/pytrivialsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/src/pytrivialsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/src/pytrivialsql/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/src/pytrivialsql/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/src/pytrivialsql/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:46:56.613683 pytrivialsql-0.1.9/src/pytrivialsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-26 03:46:56.000000 pytrivialsql-0.1.9/src/pytrivialsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-26 03:46:56.000000 pytrivialsql-0.1.9/src/pytrivialsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 03:46:56.000000 pytrivialsql-0.1.9/src/pytrivialsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 03:46:56.000000 pytrivialsql-0.1.9/src/pytrivialsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 03:46:56.000000 pytrivialsql-0.1.9/src/pytrivialsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:46:56.613683 pytrivialsql-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/tests/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/tests/test_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-26 03:46:37.000000 pytrivialsql-0.1.9/tests/test_sqlite.py
```

### Comparing `pytrivialsql-0.1.8/LICENSE` & `pytrivialsql-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.8/PKG-INFO` & `pytrivialsql-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.8
+Version: 0.1.9
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.8/pyproject.toml` & `pytrivialsql-0.1.9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytrivialsql"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="inaimathi", email="leo.zovic@gmail.com" },
 ]
 description = "A trivial set of QOL bindings for SQL in Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pytrivialsql-0.1.8/src/pytrivialsql/postgres.py` & `pytrivialsql-0.1.9/src/pytrivialsql/postgres.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,20 @@
 
     def create(self, table_name, props):
         with self._conn.cursor() as cur:
             cur.execute(sql.create_q(table_name, props))
             self._commit()
             return True
 
+    def add_column(self, table_name, col):
+        with self._conn.cursor() as cur:
+            cur.execute(sql.add_column_q(table_name, col))
+            self._commit()
+            return True
+
     def select(
         self,
         table_name,
         columns,
         distinct=None,
         where=None,
         order_by=None,
```

### Comparing `pytrivialsql-0.1.8/src/pytrivialsql/sql.py` & `pytrivialsql-0.1.9/src/pytrivialsql/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,18 @@
     return f"DROP TABLE IF EXISTS {table_name}"
 
 
 def create_q(table_name, cols):
     return f"CREATE TABLE IF NOT EXISTS {table_name}({', '.join(cols)})"
 
 
+def add_column_q(table_name, col):
+    return f"ALTER TABLE {table_name} ADD COLUMN IF NOT EXISTS {col}"
+
+
 def insert_q(table_name, **args):
     placeholder = args.get("placeholder", "?")
     returning = args.get("RETURNING", args.get("returning", None))
     for k in ["placeholder", "RETURNING", "returning"]:
         if k in args:
             del args[k]
     ks = args.keys()
```

### Comparing `pytrivialsql-0.1.8/src/pytrivialsql/sqlite.py` & `pytrivialsql-0.1.9/src/pytrivialsql/sqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,22 @@
         try:
             with self._conn as cur:
                 cur.execute(sql.create_q(table_name, props))
                 return True
         except Exception:
             return False
 
+    def add_column(self, table_name, col):
+        try:
+            with self._conn as cur:
+                cur.execute(sql.add_column_q(table_name, col))
+                return True
+        except Exception:
+            return False
+
     def select(
         self,
         table_name,
         columns,
         distinct=None,
         where=None,
         order_by=None,
```

### Comparing `pytrivialsql-0.1.8/src/pytrivialsql.egg-info/PKG-INFO` & `pytrivialsql-0.1.9/src/pytrivialsql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrivialsql
-Version: 0.1.8
+Version: 0.1.9
 Summary: A trivial set of QOL bindings for SQL in Python
 Author-email: inaimathi <leo.zovic@gmail.com>
 Project-URL: Homepage, https://github.com/inaimathi/pytrivialsql
 Project-URL: Issues, https://github.com/inaimathi/pytrivialsql/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytrivialsql-0.1.8/tests/test_postgres.py` & `pytrivialsql-0.1.9/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.8/tests/test_sql.py` & `pytrivialsql-0.1.9/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `pytrivialsql-0.1.8/tests/test_sqlite.py` & `pytrivialsql-0.1.9/tests/test_sqlite.py`

 * *Files identical despite different names*

