# Comparing `tmp/lapa_authentication-0.0.8.tar.gz` & `tmp/lapa_authentication-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lapa_authentication-0.0.8.tar", last modified: Sat Apr 13 16:07:07 2024, max compression
+gzip compressed data, was "lapa_authentication-0.0.9.tar", last modified: Sun May  5 12:25:14 2024, max compression
```

## Comparing `lapa_authentication-0.0.8.tar` & `lapa_authentication-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:07:07.125023 lapa_authentication-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-13 16:07:07.125023 lapa_authentication-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:07:07.121024 lapa_authentication-0.0.8/lapa_authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/lapa_authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/lapa_authentication/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:07:07.125023 lapa_authentication-0.0.8/lapa_authentication/data/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/lapa_authentication/data/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/lapa_authentication/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:07:07.125023 lapa_authentication-0.0.8/lapa_authentication/pydantic_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/lapa_authentication/pydantic_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/lapa_authentication/pydantic_models/pydantic_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:07:07.125023 lapa_authentication-0.0.8/lapa_authentication/routes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/lapa_authentication/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/lapa_authentication/routes/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/lapa_authentication/routes/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:07:07.125023 lapa_authentication-0.0.8/lapa_authentication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-13 16:07:07.000000 lapa_authentication-0.0.8/lapa_authentication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-13 16:07:07.000000 lapa_authentication-0.0.8/lapa_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:07:07.000000 lapa_authentication-0.0.8/lapa_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-13 16:07:07.000000 lapa_authentication-0.0.8/lapa_authentication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 16:07:07.000000 lapa_authentication-0.0.8/lapa_authentication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:07:07.125023 lapa_authentication-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-13 16:06:56.000000 lapa_authentication-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:14.959688 lapa_authentication-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-05 12:25:14.959688 lapa_authentication-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:14.959688 lapa_authentication-0.0.9/lapa_authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/lapa_authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/lapa_authentication/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:14.959688 lapa_authentication-0.0.9/lapa_authentication/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/lapa_authentication/data/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/lapa_authentication/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:14.959688 lapa_authentication-0.0.9/lapa_authentication/pydantic_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/lapa_authentication/pydantic_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/lapa_authentication/pydantic_models/pydantic_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:14.959688 lapa_authentication-0.0.9/lapa_authentication/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/lapa_authentication/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/lapa_authentication/routes/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/lapa_authentication/routes/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 12:25:14.959688 lapa_authentication-0.0.9/lapa_authentication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-05 12:25:14.000000 lapa_authentication-0.0.9/lapa_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-05 12:25:14.000000 lapa_authentication-0.0.9/lapa_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 12:25:14.000000 lapa_authentication-0.0.9/lapa_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-05 12:25:14.000000 lapa_authentication-0.0.9/lapa_authentication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-05 12:25:14.000000 lapa_authentication-0.0.9/lapa_authentication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 12:25:14.959688 lapa_authentication-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-05 12:25:07.000000 lapa_authentication-0.0.9/setup.py
```

### Comparing `lapa_authentication-0.0.8/PKG-INFO` & `lapa_authentication-0.0.9/lapa_authentication.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lapa_authentication
-Version: 0.0.8
+Name: lapa-authentication
+Version: 0.0.9
 Summary: authentication service for my personal server.
 Home-page: https://github.com/lavvsharma/lapa_authentication
 Author: Lav Sharma, thePmSquare
 Author-email: lavsharma2016@gmail.com, thepmsquare@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,18 @@
 
 ## Env
 
 - python>=3.12.0
 
 ## Changelog
 
+### v0.0.9
+
+- fix missing dependencies in setup.py
+
 ### v0.0.8
 
 - remove salt storing from register.
 - implement login route.
 
 ### v0.0.7
```

### Comparing `lapa_authentication-0.0.8/README.md` & `lapa_authentication-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 ## Env
 
 - python>=3.12.0
 
 ## Changelog
 
+### v0.0.9
+
+- fix missing dependencies in setup.py
+
 ### v0.0.8
 
 - remove salt storing from register.
 - implement login route.
 
 ### v0.0.7
```

### Comparing `lapa_authentication-0.0.8/lapa_authentication/configuration.py` & `lapa_authentication-0.0.9/lapa_authentication/configuration.py`

 * *Files identical despite different names*

### Comparing `lapa_authentication-0.0.8/lapa_authentication/main.py` & `lapa_authentication-0.0.9/lapa_authentication/main.py`

 * *Files identical despite different names*

### Comparing `lapa_authentication-0.0.8/lapa_authentication/routes/core.py` & `lapa_authentication-0.0.9/lapa_authentication/routes/core.py`

 * *Files identical despite different names*

### Comparing `lapa_authentication-0.0.8/lapa_authentication.egg-info/PKG-INFO` & `lapa_authentication-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lapa-authentication
-Version: 0.0.8
+Name: lapa_authentication
+Version: 0.0.9
 Summary: authentication service for my personal server.
 Home-page: https://github.com/lavvsharma/lapa_authentication
 Author: Lav Sharma, thePmSquare
 Author-email: lavsharma2016@gmail.com, thepmsquare@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,18 @@
 
 ## Env
 
 - python>=3.12.0
 
 ## Changelog
 
+### v0.0.9
+
+- fix missing dependencies in setup.py
+
 ### v0.0.8
 
 - remove salt storing from register.
 - implement login route.
 
 ### v0.0.7
```

### Comparing `lapa_authentication-0.0.8/lapa_authentication.egg-info/SOURCES.txt` & `lapa_authentication-0.0.9/lapa_authentication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lapa_authentication-0.0.8/setup.py` & `lapa_authentication-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import find_packages, setup
 
 package_name = "lapa_authentication"
 
 setup(
     name=package_name,
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     package_data={
         package_name: ["data/*"],
     },
     install_requires=[
         "uvicorn>=0.24.0.post1",
         "fastapi>=0.104.1",
-        "square_logger~=1.0",
         "pydantic>=2.5.3",
-        "lapa_commons>=0.0.1",
         "bcrypt>=4.1.2",
-        "pyjwt>=2.8.0"
+        "pyjwt>=2.8.0",
+
+        "lapa_commons>=0.0.1",
+        "square_logger~=1.0",
+        "lapa_database_helper>=0.0.5",
+        "lapa_database_structure>=0.0.11"
     ],
     extras_require={},
     author="Lav Sharma, thePmSquare",
     author_email="lavsharma2016@gmail.com, thepmsquare@gmail.com",
     description="authentication service for my personal server.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
```

