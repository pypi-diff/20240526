# Comparing `tmp/lazyins-0.1.0.tar.gz` & `tmp/lazyins-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyins-0.1.0.tar", last modified: Thu Mar 28 16:19:33 2024, max compression
+gzip compressed data, was "lazyins-0.1.1.tar", last modified: Sun May 26 20:22:56 2024, max compression
```

## Comparing `lazyins-0.1.0.tar` & `lazyins-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:19:33.403771 lazyins-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-28 16:19:20.000000 lazyins-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-28 16:19:33.403771 lazyins-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-28 16:19:20.000000 lazyins-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:19:33.399772 lazyins-0.1.0/lazyins/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-28 16:19:20.000000 lazyins-0.1.0/lazyins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-03-28 16:19:20.000000 lazyins-0.1.0/lazyins/lazyins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:19:33.403771 lazyins-0.1.0/lazyins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-03-28 16:19:33.000000 lazyins-0.1.0/lazyins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-28 16:19:33.000000 lazyins-0.1.0/lazyins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 16:19:33.000000 lazyins-0.1.0/lazyins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 16:19:33.000000 lazyins-0.1.0/lazyins.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-28 16:19:20.000000 lazyins-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-28 16:19:33.403771 lazyins-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 16:19:33.403771 lazyins-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-28 16:19:20.000000 lazyins-0.1.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:22:56.741244 lazyins-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-26 20:22:52.000000 lazyins-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-26 20:22:56.741244 lazyins-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-26 20:22:52.000000 lazyins-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:22:56.741244 lazyins-0.1.1/lazyins/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-26 20:22:52.000000 lazyins-0.1.1/lazyins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-26 20:22:52.000000 lazyins-0.1.1/lazyins/lazyins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:22:56.741244 lazyins-0.1.1/lazyins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-26 20:22:56.000000 lazyins-0.1.1/lazyins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-26 20:22:56.000000 lazyins-0.1.1/lazyins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:22:56.000000 lazyins-0.1.1/lazyins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-26 20:22:56.000000 lazyins-0.1.1/lazyins.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 20:22:52.000000 lazyins-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-26 20:22:56.741244 lazyins-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:22:56.741244 lazyins-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-26 20:22:52.000000 lazyins-0.1.1/tests/test.py
```

### Comparing `lazyins-0.1.0/LICENSE` & `lazyins-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazyins-0.1.0/PKG-INFO` & `lazyins-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyins
-Version: 0.1.0
+Version: 0.1.1
 Summary: A stupid MySQL insert helper
 Home-page: https://github.com/mzks/lazyins
 Author: Keita Mizukoshi
 Author-email: keita@mzks.dev
 Project-URL: Bug Tracker, https://github.com/mzks/lazyins/issue
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyins-0.1.0/README.md` & `lazyins-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lazyins-0.1.0/lazyins/lazyins.py` & `lazyins-0.1.1/lazyins/lazyins.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,19 @@
 
         
         if self.db != 'sqlite':
             self.cursor.execute("CREATE DATABASE IF NOT EXISTS {};".format(self.db_name))
             self.cursor.execute("USE {};".format(self.db_name))
 
         self.cursor.execute(self.table_query)
-        self.cursor.execute(f'CREATE INDEX IF NOT EXISTS time_index ON {self.table_name} (time);')
+
+        self.cursor.execute(f"SHOW INDEX FROM {self.table_name} WHERE Key_name = 'time_index'")
+        index_exists = bool(self.cursor.fetchone())
+        if not index_exists:
+            self.cursor.execute(f'CREATE INDEX time_index ON {self.table_name} (time)')
 
         self.before_initial_execute = False
 
 
     def register(self, values, names=None, explicit_types=[]):
 
         # unpack list of tuple : [('name1', 1), ('name2', 2)]
```

### Comparing `lazyins-0.1.0/lazyins.egg-info/PKG-INFO` & `lazyins-0.1.1/lazyins.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyins
-Version: 0.1.0
+Version: 0.1.1
 Summary: A stupid MySQL insert helper
 Home-page: https://github.com/mzks/lazyins
 Author: Keita Mizukoshi
 Author-email: keita@mzks.dev
 Project-URL: Bug Tracker, https://github.com/mzks/lazyins/issue
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lazyins-0.1.0/tests/test.py` & `lazyins-0.1.1/tests/test.py`

 * *Files identical despite different names*

