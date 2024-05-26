# Comparing `tmp/foctopus-1.1.tar.gz` & `tmp/foctopus-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foctopus-1.1.tar", last modified: Sat May 18 20:56:36 2024, max compression
+gzip compressed data, was "foctopus-1.2.tar", last modified: Sun May 26 06:04:37 2024, max compression
```

## Comparing `foctopus-1.1.tar` & `foctopus-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 20:56:36.361425 foctopus-1.1/
--rw-rw-rw-   0        0        0      568 2024-05-18 20:56:36.361425 foctopus-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-05-18 20:25:15.000000 foctopus-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 20:56:36.353592 foctopus-1.1/foctopus/
--rw-rw-rw-   0        0        0       23 2024-05-18 20:38:07.000000 foctopus-1.1/foctopus/__init__.py
--rw-rw-rw-   0        0        0     4439 2024-05-18 20:52:42.000000 foctopus-1.1/foctopus/foctopus.py
-drwxrwxrwx   0        0        0        0 2024-05-18 20:56:36.360307 foctopus-1.1/foctopus.egg-info/
--rw-rw-rw-   0        0        0      568 2024-05-18 20:56:36.000000 foctopus-1.1/foctopus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-18 20:56:36.000000 foctopus-1.1/foctopus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 20:56:36.000000 foctopus-1.1/foctopus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-18 20:56:36.000000 foctopus-1.1/foctopus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 20:56:36.000000 foctopus-1.1/foctopus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 20:56:36.362535 foctopus-1.1/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-05-18 20:56:27.000000 foctopus-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 06:04:37.343100 foctopus-1.2/
+-rw-rw-rw-   0        0        0      568 2024-05-26 06:04:37.342103 foctopus-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2024-05-18 20:25:15.000000 foctopus-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 06:04:37.332163 foctopus-1.2/foctopus/
+-rw-rw-rw-   0        0        0       23 2024-05-18 20:38:07.000000 foctopus-1.2/foctopus/__init__.py
+-rw-rw-rw-   0        0        0     4441 2024-05-19 06:12:49.000000 foctopus-1.2/foctopus/foctopus.py
+drwxrwxrwx   0        0        0        0 2024-05-26 06:04:37.341106 foctopus-1.2/foctopus.egg-info/
+-rw-rw-rw-   0        0        0      568 2024-05-26 06:04:37.000000 foctopus-1.2/foctopus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-26 06:04:37.000000 foctopus-1.2/foctopus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 06:04:37.000000 foctopus-1.2/foctopus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 06:04:37.000000 foctopus-1.2/foctopus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-26 06:04:37.000000 foctopus-1.2/foctopus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 06:04:37.343100 foctopus-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-05-26 06:02:23.000000 foctopus-1.2/setup.py
```

### Comparing `foctopus-1.1/PKG-INFO` & `foctopus-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foctopus
-Version: 1.1
+Version: 1.2
 Summary: Many functions for python
 Home-page: https://github.com/ForestBu/foctopus
 Author: ForestBu
 Author-email: tvc55.admn@gmail.com
 Keywords: login password logout reg register regitration functions pause time sleep stop shell
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `foctopus-1.1/foctopus/foctopus.py` & `foctopus-1.2/foctopus/foctopus.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,16 @@
             if message: print('Registration completed successfully.')
 
     all_return['logins'] = array_login
     all_return['passwords'] = array_password
     return all_return
 
 def login(logins, language='ru', loading=True, count=1): 
-    array_login = logins["login"]
-    array_password = logins["password"]
+    array_login = logins["logins"]
+    array_password = logins["passwords"]
 
     array_loginf = []
     array_passwordf = []
 
     all_return = {}
 
     if language == 'ru':
```

### Comparing `foctopus-1.1/foctopus.egg-info/PKG-INFO` & `foctopus-1.2/foctopus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foctopus
-Version: 1.1
+Version: 1.2
 Summary: Many functions for python
 Home-page: https://github.com/ForestBu/foctopus
 Author: ForestBu
 Author-email: tvc55.admn@gmail.com
 Keywords: login password logout reg register regitration functions pause time sleep stop shell
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `foctopus-1.1/setup.py` & `foctopus-1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='foctopus',
-    version='1.1',
+    version='1.2',
     author='ForestBu',
     author_email='tvc55.admn@gmail.com',
     description='Many functions for python',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/ForestBu/foctopus',
     packages=find_packages(),
```

