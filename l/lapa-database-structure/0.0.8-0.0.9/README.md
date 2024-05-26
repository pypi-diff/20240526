# Comparing `tmp/lapa_database_structure-0.0.8.tar.gz` & `tmp/lapa_database_structure-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_database_structure-0.0.8.tar", last modified: Wed Apr 10 17:14:47 2024, max compression
+gzip compressed data, was "lapa_database_structure-0.0.9.tar", last modified: Thu Apr 11 14:20:55 2024, max compression
```

## Comparing `lapa_database_structure-0.0.8.tar` & `lapa_database_structure-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.968013 lapa_database_structure-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-10 17:14:47.968013 lapa_database_structure-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/authentication/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/authentication/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa/file_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/file_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/file_storage/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa/public/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa/public/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/authentication/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/authentication/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/file_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/file_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/file_storage/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.968013 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/public/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/public/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/lapa_database_structure/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:14:47.964013 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 17:14:47.000000 lapa_database_structure-0.0.8/lapa_database_structure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:14:47.968013 lapa_database_structure-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-10 17:14:33.000000 lapa_database_structure-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.480370 lapa_database_structure-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure/lapa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure/lapa/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa/authentication/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa/authentication/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure/lapa/file_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa/file_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa/file_storage/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure/lapa/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa/public/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/authentication/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/authentication/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/file_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/file_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/file_storage/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/public/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/lapa_database_structure/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:20:55.476370 lapa_database_structure-0.0.9/lapa_database_structure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-11 14:20:55.000000 lapa_database_structure-0.0.9/lapa_database_structure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-11 14:20:55.000000 lapa_database_structure-0.0.9/lapa_database_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:20:55.000000 lapa_database_structure-0.0.9/lapa_database_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 14:20:55.000000 lapa_database_structure-0.0.9/lapa_database_structure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 14:20:55.000000 lapa_database_structure-0.0.9/lapa_database_structure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:20:55.480370 lapa_database_structure-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-11 14:20:46.000000 lapa_database_structure-0.0.9/setup.py
```

### Comparing `lapa_database_structure-0.0.8/PKG-INFO` & `lapa_database_structure-0.0.9/lapa_database_structure.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lapa_database_structure
-Version: 0.0.8
+Name: lapa-database-structure
+Version: 0.0.9
 Summary: database layer for my personal server.
 Home-page: https://github.com/B21amish/lapa_database_structure
 Author: Amish Palkar, thePmSquare, Lav Sharma, Aaditya Sangishetty
 Author-email: amishpalkar302001@gmail.com, thepmsquare@gmail.com, lavsharma2016@gmail.com, adityasehtty35@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -55,14 +55,19 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.9
+
+- rename authentication_username_hashed_access_token and authentication_username_hashed_refresh_token.
+- update enum in main.py.
+
 ### v0.0.8
 
 - Overhauled authentication schema, again.
 
 ### v0.0.7
 
 - Overhauled authentication schema,
```

### Comparing `lapa_database_structure-0.0.8/README.md` & `lapa_database_structure-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.9
+
+- rename authentication_username_hashed_access_token and authentication_username_hashed_refresh_token.
+- update enum in main.py.
+
 ### v0.0.8
 
 - Overhauled authentication schema, again.
 
 ### v0.0.7
 
 - Overhauled authentication schema,
```

### Comparing `lapa_database_structure-0.0.8/lapa_database_structure/lapa/authentication/tables.py` & `lapa_database_structure-0.0.9/lapa_database_structure/lapa/authentication/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     authentication_username_username = Column(
         String,
         nullable=False,
         unique=True,
     )
     authentication_username_hashed_password = Column(String, nullable=False)
     authentication_username_password_salt = Column(String, nullable=False, unique=True)
-    authentication_username_access_token = Column(String, nullable=False)
-    authentication_username_refresh_token = Column(String, nullable=False)
+    authentication_username_hashed_access_token = Column(String, nullable=False)
+    authentication_username_hashed_refresh_token = Column(String, nullable=False)
 
 
 class UserProfile(Base):
     __tablename__ = "user_profile"
 
     user_profile_id = Column(
         Integer,
```

### Comparing `lapa_database_structure-0.0.8/lapa_database_structure/lapa/file_storage/tables.py` & `lapa_database_structure-0.0.9/lapa_database_structure/lapa/file_storage/tables.py`

 * *Files identical despite different names*

### Comparing `lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/authentication/tables.py` & `lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/authentication/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     authentication_username_username = Column(
         String,
         nullable=False,
         unique=True,
     )
     authentication_username_hashed_password = Column(String, nullable=False)
     authentication_username_password_salt = Column(String, nullable=False, unique=True)
-    authentication_username_access_token = Column(String, nullable=False)
-    authentication_username_refresh_token = Column(String, nullable=False)
+    authentication_username_hashed_access_token = Column(String, nullable=False)
+    authentication_username_hashed_refresh_token = Column(String, nullable=False)
 
 
 class UserProfile(Base):
     __tablename__ = "user_profile"
 
     user_profile_id = Column(
         Integer,
```

### Comparing `lapa_database_structure-0.0.8/lapa_database_structure/lapa_testing/file_storage/tables.py` & `lapa_database_structure-0.0.9/lapa_database_structure/lapa_testing/file_storage/tables.py`

 * *Files identical despite different names*

### Comparing `lapa_database_structure-0.0.8/lapa_database_structure.egg-info/PKG-INFO` & `lapa_database_structure-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lapa-database-structure
-Version: 0.0.8
+Name: lapa_database_structure
+Version: 0.0.9
 Summary: database layer for my personal server.
 Home-page: https://github.com/B21amish/lapa_database_structure
 Author: Amish Palkar, thePmSquare, Lav Sharma, Aaditya Sangishetty
 Author-email: amishpalkar302001@gmail.com, thepmsquare@gmail.com, lavsharma2016@gmail.com, adityasehtty35@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -55,14 +55,19 @@
 
 ## env
 
 - python>=3.12.0
 
 ## changelog
 
+### v0.0.9
+
+- rename authentication_username_hashed_access_token and authentication_username_hashed_refresh_token.
+- update enum in main.py.
+
 ### v0.0.8
 
 - Overhauled authentication schema, again.
 
 ### v0.0.7
 
 - Overhauled authentication schema,
```

### Comparing `lapa_database_structure-0.0.8/lapa_database_structure.egg-info/SOURCES.txt` & `lapa_database_structure-0.0.9/lapa_database_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lapa_database_structure-0.0.8/setup.py` & `lapa_database_structure-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_database_structure"
 
 setup(
     name=package_name,
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     package_data={
         package_name: [],
     },
     install_requires=[
         "sqlalchemy>=2.0.23",
     ],
```

