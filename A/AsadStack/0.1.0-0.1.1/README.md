# Comparing `tmp/AsadStack-0.1.0.tar.gz` & `tmp/AsadStack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AsadStack-0.1.0.tar", last modified: Sun May 26 06:06:40 2024, max compression
+gzip compressed data, was "AsadStack-0.1.1.tar", last modified: Sun May 26 06:58:15 2024, max compression
```

## Comparing `AsadStack-0.1.0.tar` & `AsadStack-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 asadtop4ik  (1000) asadtop4ik  (1000)        0 2024-05-26 06:06:40.011870 AsadStack-0.1.0/
-drwxrwxr-x   0 asadtop4ik  (1000) asadtop4ik  (1000)        0 2024-05-26 06:06:40.011870 AsadStack-0.1.0/AsadStack.egg-info/
--rw-r--r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      820 2024-05-26 06:06:39.000000 AsadStack-0.1.0/AsadStack.egg-info/PKG-INFO
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      261 2024-05-26 06:06:39.000000 AsadStack-0.1.0/AsadStack.egg-info/SOURCES.txt
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)        1 2024-05-26 06:06:39.000000 AsadStack-0.1.0/AsadStack.egg-info/dependency_links.txt
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      105 2024-05-26 06:06:39.000000 AsadStack-0.1.0/AsadStack.egg-info/requires.txt
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)       11 2024-05-26 06:06:39.000000 AsadStack-0.1.0/AsadStack.egg-info/top_level.txt
-drwxrwxr-x   0 asadtop4ik  (1000) asadtop4ik  (1000)        0 2024-05-26 06:06:40.011870 AsadStack-0.1.0/Asad_Stack/
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)        0 2024-05-26 05:49:41.000000 AsadStack-0.1.0/Asad_Stack/__init__.py
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)     3760 2024-05-26 05:51:40.000000 AsadStack-0.1.0/Asad_Stack/app.py
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      673 2024-05-25 18:02:07.000000 AsadStack-0.1.0/Asad_Stack/middleware.py
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      945 2024-05-26 05:39:54.000000 AsadStack-0.1.0/Asad_Stack/response.py
--rw-r--r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      820 2024-05-26 06:06:40.011870 AsadStack-0.1.0/PKG-INFO
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)       38 2024-05-26 06:06:40.011870 AsadStack-0.1.0/setup.cfg
--rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)     3888 2024-05-26 05:59:13.000000 AsadStack-0.1.0/setup.py
+drwxrwxr-x   0 asadtop4ik  (1000) asadtop4ik  (1000)        0 2024-05-26 06:58:15.781424 AsadStack-0.1.1/
+drwxrwxr-x   0 asadtop4ik  (1000) asadtop4ik  (1000)        0 2024-05-26 06:58:15.777424 AsadStack-0.1.1/AsadStack.egg-info/
+-rw-r--r--   0 asadtop4ik  (1000) asadtop4ik  (1000)     4788 2024-05-26 06:58:15.000000 AsadStack-0.1.1/AsadStack.egg-info/PKG-INFO
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      271 2024-05-26 06:58:15.000000 AsadStack-0.1.1/AsadStack.egg-info/SOURCES.txt
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)        1 2024-05-26 06:58:15.000000 AsadStack-0.1.1/AsadStack.egg-info/dependency_links.txt
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      105 2024-05-26 06:58:15.000000 AsadStack-0.1.1/AsadStack.egg-info/requires.txt
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)       11 2024-05-26 06:58:15.000000 AsadStack-0.1.1/AsadStack.egg-info/top_level.txt
+drwxrwxr-x   0 asadtop4ik  (1000) asadtop4ik  (1000)        0 2024-05-26 06:58:15.777424 AsadStack-0.1.1/Asad_Stack/
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)        0 2024-05-26 05:49:41.000000 AsadStack-0.1.1/Asad_Stack/__init__.py
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)     3760 2024-05-26 05:51:40.000000 AsadStack-0.1.1/Asad_Stack/app.py
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      673 2024-05-25 18:02:07.000000 AsadStack-0.1.1/Asad_Stack/middleware.py
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)      945 2024-05-26 05:39:54.000000 AsadStack-0.1.1/Asad_Stack/response.py
+-rw-r--r--   0 asadtop4ik  (1000) asadtop4ik  (1000)     4788 2024-05-26 06:58:15.777424 AsadStack-0.1.1/PKG-INFO
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)     3987 2024-05-26 06:55:30.000000 AsadStack-0.1.1/README.md
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)       38 2024-05-26 06:58:15.781424 AsadStack-0.1.1/setup.cfg
+-rw-rw-r--   0 asadtop4ik  (1000) asadtop4ik  (1000)     3888 2024-05-26 06:58:06.000000 AsadStack-0.1.1/setup.py
```

### Comparing `AsadStack-0.1.0/Asad_Stack/app.py` & `AsadStack-0.1.1/Asad_Stack/app.py`

 * *Files identical despite different names*

### Comparing `AsadStack-0.1.0/Asad_Stack/middleware.py` & `AsadStack-0.1.1/Asad_Stack/middleware.py`

 * *Files identical despite different names*

### Comparing `AsadStack-0.1.0/Asad_Stack/response.py` & `AsadStack-0.1.1/Asad_Stack/response.py`

 * *Files identical despite different names*

### Comparing `AsadStack-0.1.0/setup.py` & `AsadStack-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'AsadStack'
 DESCRIPTION = 'Python Web Framework'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'asadbek.backend@gmail.com'
 AUTHOR = 'Azamatov Asadbek'
 REQUIRES_PYTHON = '>=3.11.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```

