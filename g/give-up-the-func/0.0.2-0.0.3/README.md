# Comparing `tmp/give_up_the_func-0.0.2.tar.gz` & `tmp/give_up_the_func-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "give_up_the_func-0.0.2.tar", last modified: Fri May 24 22:00:22 2024, max compression
+gzip compressed data, was "give_up_the_func-0.0.3.tar", last modified: Sun May 26 16:18:40 2024, max compression
```

## Comparing `give_up_the_func-0.0.2.tar` & `give_up_the_func-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jasonuechi   (501) staff       (20)        0 2024-05-24 22:00:22.245065 give_up_the_func-0.0.2/
--rw-r--r--   0 jasonuechi   (501) staff       (20)     1070 2024-05-24 11:49:23.000000 give_up_the_func-0.0.2/LICENSE
--rw-r--r--   0 jasonuechi   (501) staff       (20)     2205 2024-05-24 22:00:22.244747 give_up_the_func-0.0.2/PKG-INFO
--rw-r--r--   0 jasonuechi   (501) staff       (20)     1351 2024-05-24 19:42:32.000000 give_up_the_func-0.0.2/README.md
-drwxr-xr-x   0 jasonuechi   (501) staff       (20)        0 2024-05-24 22:00:22.242296 give_up_the_func-0.0.2/give_up_the_func/
--rw-r--r--   0 jasonuechi   (501) staff       (20)       60 2024-05-24 21:56:22.000000 give_up_the_func-0.0.2/give_up_the_func/__init__.py
--rw-r--r--   0 jasonuechi   (501) staff       (20)     9946 2024-05-24 21:08:19.000000 give_up_the_func-0.0.2/give_up_the_func/core.py
-drwxr-xr-x   0 jasonuechi   (501) staff       (20)        0 2024-05-24 22:00:22.244367 give_up_the_func-0.0.2/give_up_the_func.egg-info/
--rw-r--r--   0 jasonuechi   (501) staff       (20)     2205 2024-05-24 22:00:22.000000 give_up_the_func-0.0.2/give_up_the_func.egg-info/PKG-INFO
--rw-r--r--   0 jasonuechi   (501) staff       (20)      279 2024-05-24 22:00:22.000000 give_up_the_func-0.0.2/give_up_the_func.egg-info/SOURCES.txt
--rw-r--r--   0 jasonuechi   (501) staff       (20)        1 2024-05-24 22:00:22.000000 give_up_the_func-0.0.2/give_up_the_func.egg-info/dependency_links.txt
--rw-r--r--   0 jasonuechi   (501) staff       (20)       14 2024-05-24 22:00:22.000000 give_up_the_func-0.0.2/give_up_the_func.egg-info/requires.txt
--rw-r--r--   0 jasonuechi   (501) staff       (20)       17 2024-05-24 22:00:22.000000 give_up_the_func-0.0.2/give_up_the_func.egg-info/top_level.txt
--rw-r--r--   0 jasonuechi   (501) staff       (20)       38 2024-05-24 22:00:22.245136 give_up_the_func-0.0.2/setup.cfg
--rw-r--r--   0 jasonuechi   (501) staff       (20)     1277 2024-05-24 21:57:51.000000 give_up_the_func-0.0.2/setup.py
+drwxr-xr-x   0 jasonuechi   (501) staff       (20)        0 2024-05-26 16:18:40.910139 give_up_the_func-0.0.3/
+-rw-r--r--   0 jasonuechi   (501) staff       (20)     1070 2024-05-24 11:49:23.000000 give_up_the_func-0.0.3/LICENSE
+-rw-r--r--   0 jasonuechi   (501) staff       (20)     7909 2024-05-26 16:18:40.909772 give_up_the_func-0.0.3/PKG-INFO
+-rw-r--r--   0 jasonuechi   (501) staff       (20)     7056 2024-05-26 16:18:25.000000 give_up_the_func-0.0.3/README.md
+drwxr-xr-x   0 jasonuechi   (501) staff       (20)        0 2024-05-26 16:18:40.907118 give_up_the_func-0.0.3/give_up_the_func/
+-rw-r--r--   0 jasonuechi   (501) staff       (20)       60 2024-05-24 21:56:22.000000 give_up_the_func-0.0.3/give_up_the_func/__init__.py
+-rw-r--r--   0 jasonuechi   (501) staff       (20)     9946 2024-05-24 21:08:19.000000 give_up_the_func-0.0.3/give_up_the_func/core.py
+drwxr-xr-x   0 jasonuechi   (501) staff       (20)        0 2024-05-26 16:18:40.909309 give_up_the_func-0.0.3/give_up_the_func.egg-info/
+-rw-r--r--   0 jasonuechi   (501) staff       (20)     7909 2024-05-26 16:18:40.000000 give_up_the_func-0.0.3/give_up_the_func.egg-info/PKG-INFO
+-rw-r--r--   0 jasonuechi   (501) staff       (20)      279 2024-05-26 16:18:40.000000 give_up_the_func-0.0.3/give_up_the_func.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonuechi   (501) staff       (20)        1 2024-05-26 16:18:40.000000 give_up_the_func-0.0.3/give_up_the_func.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonuechi   (501) staff       (20)       14 2024-05-26 16:18:40.000000 give_up_the_func-0.0.3/give_up_the_func.egg-info/requires.txt
+-rw-r--r--   0 jasonuechi   (501) staff       (20)       17 2024-05-26 16:18:40.000000 give_up_the_func-0.0.3/give_up_the_func.egg-info/top_level.txt
+-rw-r--r--   0 jasonuechi   (501) staff       (20)       38 2024-05-26 16:18:40.910213 give_up_the_func-0.0.3/setup.cfg
+-rw-r--r--   0 jasonuechi   (501) staff       (20)     1277 2024-05-26 16:12:39.000000 give_up_the_func-0.0.3/setup.py
```

### Comparing `give_up_the_func-0.0.2/LICENSE` & `give_up_the_func-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `give_up_the_func-0.0.2/give_up_the_func/core.py` & `give_up_the_func-0.0.3/give_up_the_func/core.py`

 * *Files identical despite different names*

### Comparing `give_up_the_func-0.0.2/setup.py` & `give_up_the_func-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='give_up_the_func', 
-    version='0.0.2',  
+    version='0.0.3',  
     author='gravitymonkey',  
     author_email='jason@gravitymonkey.com',  
     description='A helper library for using function calling on local LLMs.',  
     long_description=open('README.md').read(),  # Long description read from the README.md
     long_description_content_type='text/markdown',  
     url='https://github.com/gravitymonkey/give_up_the_func', 
     packages=find_packages(),
```

