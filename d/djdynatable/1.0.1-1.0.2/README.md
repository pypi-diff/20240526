# Comparing `tmp/djdynatable-1.0.1.tar.gz` & `tmp/djdynatable-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djdynatable-1.0.1.tar", last modified: Sun May 26 09:16:38 2024, max compression
+gzip compressed data, was "djdynatable-1.0.2.tar", last modified: Sun May 26 09:20:49 2024, max compression
```

## Comparing `djdynatable-1.0.1.tar` & `djdynatable-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:16:38.985843 djdynatable-1.0.1/
--rw-r--r--   0 anand      (501) staff       (20)       64 2024-05-26 09:07:20.000000 djdynatable-1.0.1/MANIFEST.in
--rw-r--r--   0 anand      (501) staff       (20)     1311 2024-05-26 09:16:38.985951 djdynatable-1.0.1/PKG-INFO
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:16:38.984016 djdynatable-1.0.1/djdynatable/
--rw-r--r--   0 anand      (501) staff       (20)        0 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/__init__.py
--rw-r--r--   0 anand      (501) staff       (20)      128 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/admin.py
--rw-r--r--   0 anand      (501) staff       (20)      252 2024-05-26 09:08:02.000000 djdynatable-1.0.1/djdynatable/apps.py
--rw-r--r--   0 anand      (501) staff       (20)     2263 2024-05-26 09:08:36.000000 djdynatable-1.0.1/djdynatable/compat.py
--rw-r--r--   0 anand      (501) staff       (20)     9577 2024-05-26 09:09:23.000000 djdynatable-1.0.1/djdynatable/core.py
--rw-r--r--   0 anand      (501) staff       (20)      531 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/exception.py
--rw-r--r--   0 anand      (501) staff       (20)     8379 2024-05-26 09:10:30.000000 djdynatable-1.0.1/djdynatable/handler.py
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:16:38.985725 djdynatable-1.0.1/djdynatable/migrations/
--rw-r--r--   0 anand      (501) staff       (20)      877 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/migrations/0001_initial.py
--rw-r--r--   0 anand      (501) staff       (20)        0 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/migrations/__init__.py
--rw-r--r--   0 anand      (501) staff       (20)     3209 2024-05-26 09:10:43.000000 djdynatable-1.0.1/djdynatable/models.py
--rw-r--r--   0 anand      (501) staff       (20)     3155 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/response.py
--rw-r--r--   0 anand      (501) staff       (20)     1425 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/serializer.py
--rw-r--r--   0 anand      (501) staff       (20)       27 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/tests.py
--rw-r--r--   0 anand      (501) staff       (20)      509 2024-05-26 09:07:20.000000 djdynatable-1.0.1/djdynatable/urls.py
--rw-r--r--   0 anand      (501) staff       (20)     6639 2024-05-26 09:12:06.000000 djdynatable-1.0.1/djdynatable/utils.py
--rw-r--r--   0 anand      (501) staff       (20)     6639 2024-05-26 09:11:44.000000 djdynatable-1.0.1/djdynatable/views.py
-drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:16:38.985307 djdynatable-1.0.1/djdynatable.egg-info/
--rw-r--r--   0 anand      (501) staff       (20)     1311 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/PKG-INFO
--rw-r--r--   0 anand      (501) staff       (20)      613 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/SOURCES.txt
--rw-r--r--   0 anand      (501) staff       (20)        1 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/dependency_links.txt
--rw-r--r--   0 anand      (501) staff       (20)       27 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/requires.txt
--rw-r--r--   0 anand      (501) staff       (20)       12 2024-05-26 09:16:38.000000 djdynatable-1.0.1/djdynatable.egg-info/top_level.txt
--rw-r--r--   0 anand      (501) staff       (20)      100 2024-05-26 09:07:20.000000 djdynatable-1.0.1/pyproject.toml
--rw-r--r--   0 anand      (501) staff       (20)      908 2024-05-26 09:14:32.000000 djdynatable-1.0.1/readme.md
--rw-r--r--   0 anand      (501) staff       (20)      395 2024-05-26 09:16:38.986262 djdynatable-1.0.1/setup.cfg
--rw-r--r--   0 anand      (501) staff       (20)      468 2024-05-26 09:14:59.000000 djdynatable-1.0.1/setup.py
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:20:49.808869 djdynatable-1.0.2/
+-rw-r--r--   0 anand      (501) staff       (20)       64 2024-05-26 09:07:20.000000 djdynatable-1.0.2/MANIFEST.in
+-rw-r--r--   0 anand      (501) staff       (20)     1311 2024-05-26 09:20:49.809004 djdynatable-1.0.2/PKG-INFO
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:20:49.806858 djdynatable-1.0.2/djdynatable/
+-rw-r--r--   0 anand      (501) staff       (20)        0 2024-05-26 09:07:20.000000 djdynatable-1.0.2/djdynatable/__init__.py
+-rw-r--r--   0 anand      (501) staff       (20)      128 2024-05-26 09:07:20.000000 djdynatable-1.0.2/djdynatable/admin.py
+-rw-r--r--   0 anand      (501) staff       (20)      252 2024-05-26 09:08:02.000000 djdynatable-1.0.2/djdynatable/apps.py
+-rw-r--r--   0 anand      (501) staff       (20)     2263 2024-05-26 09:08:36.000000 djdynatable-1.0.2/djdynatable/compat.py
+-rw-r--r--   0 anand      (501) staff       (20)     9577 2024-05-26 09:09:23.000000 djdynatable-1.0.2/djdynatable/core.py
+-rw-r--r--   0 anand      (501) staff       (20)      531 2024-05-26 09:07:20.000000 djdynatable-1.0.2/djdynatable/exception.py
+-rw-r--r--   0 anand      (501) staff       (20)     8379 2024-05-26 09:10:30.000000 djdynatable-1.0.2/djdynatable/handler.py
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:20:49.808748 djdynatable-1.0.2/djdynatable/migrations/
+-rw-r--r--   0 anand      (501) staff       (20)      877 2024-05-26 09:07:20.000000 djdynatable-1.0.2/djdynatable/migrations/0001_initial.py
+-rw-r--r--   0 anand      (501) staff       (20)        0 2024-05-26 09:07:20.000000 djdynatable-1.0.2/djdynatable/migrations/__init__.py
+-rw-r--r--   0 anand      (501) staff       (20)     3209 2024-05-26 09:10:43.000000 djdynatable-1.0.2/djdynatable/models.py
+-rw-r--r--   0 anand      (501) staff       (20)     3155 2024-05-26 09:07:20.000000 djdynatable-1.0.2/djdynatable/response.py
+-rw-r--r--   0 anand      (501) staff       (20)     1425 2024-05-26 09:07:20.000000 djdynatable-1.0.2/djdynatable/serializer.py
+-rw-r--r--   0 anand      (501) staff       (20)       27 2024-05-26 09:07:20.000000 djdynatable-1.0.2/djdynatable/tests.py
+-rw-r--r--   0 anand      (501) staff       (20)      509 2024-05-26 09:07:20.000000 djdynatable-1.0.2/djdynatable/urls.py
+-rw-r--r--   0 anand      (501) staff       (20)     1221 2024-05-26 09:19:29.000000 djdynatable-1.0.2/djdynatable/utils.py
+-rw-r--r--   0 anand      (501) staff       (20)     6639 2024-05-26 09:11:44.000000 djdynatable-1.0.2/djdynatable/views.py
+drwxr-xr-x   0 anand      (501) staff       (20)        0 2024-05-26 09:20:49.808238 djdynatable-1.0.2/djdynatable.egg-info/
+-rw-r--r--   0 anand      (501) staff       (20)     1311 2024-05-26 09:20:49.000000 djdynatable-1.0.2/djdynatable.egg-info/PKG-INFO
+-rw-r--r--   0 anand      (501) staff       (20)      613 2024-05-26 09:20:49.000000 djdynatable-1.0.2/djdynatable.egg-info/SOURCES.txt
+-rw-r--r--   0 anand      (501) staff       (20)        1 2024-05-26 09:20:49.000000 djdynatable-1.0.2/djdynatable.egg-info/dependency_links.txt
+-rw-r--r--   0 anand      (501) staff       (20)       27 2024-05-26 09:20:49.000000 djdynatable-1.0.2/djdynatable.egg-info/requires.txt
+-rw-r--r--   0 anand      (501) staff       (20)       12 2024-05-26 09:20:49.000000 djdynatable-1.0.2/djdynatable.egg-info/top_level.txt
+-rw-r--r--   0 anand      (501) staff       (20)      100 2024-05-26 09:07:20.000000 djdynatable-1.0.2/pyproject.toml
+-rw-r--r--   0 anand      (501) staff       (20)      908 2024-05-26 09:14:32.000000 djdynatable-1.0.2/readme.md
+-rw-r--r--   0 anand      (501) staff       (20)      395 2024-05-26 09:20:49.809343 djdynatable-1.0.2/setup.cfg
+-rw-r--r--   0 anand      (501) staff       (20)      468 2024-05-26 09:20:41.000000 djdynatable-1.0.2/setup.py
```

### Comparing `djdynatable-1.0.1/PKG-INFO` & `djdynatable-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djdynatable
-Version: 1.0.1
+Version: 1.0.2
 Author: Anand Raj
 Author-email: anand98.ar@gmail.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
```

### Comparing `djdynatable-1.0.1/djdynatable/compat.py` & `djdynatable-1.0.2/djdynatable/compat.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/djdynatable/core.py` & `djdynatable-1.0.2/djdynatable/core.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/djdynatable/exception.py` & `djdynatable-1.0.2/djdynatable/exception.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/djdynatable/handler.py` & `djdynatable-1.0.2/djdynatable/handler.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/djdynatable/migrations/0001_initial.py` & `djdynatable-1.0.2/djdynatable/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/djdynatable/models.py` & `djdynatable-1.0.2/djdynatable/models.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/djdynatable/response.py` & `djdynatable-1.0.2/djdynatable/response.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/djdynatable/serializer.py` & `djdynatable-1.0.2/djdynatable/serializer.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/djdynatable/utils.py` & `djdynatable-1.0.2/djdynatable/views.py`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/djdynatable.egg-info/PKG-INFO` & `djdynatable-1.0.2/djdynatable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djdynatable
-Version: 1.0.1
+Version: 1.0.2
 Author: Anand Raj
 Author-email: anand98.ar@gmail.com
 License: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python :: 3
```

### Comparing `djdynatable-1.0.1/djdynatable.egg-info/SOURCES.txt` & `djdynatable-1.0.2/djdynatable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djdynatable-1.0.1/readme.md` & `djdynatable-1.0.2/readme.md`

 * *Files identical despite different names*

