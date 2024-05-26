# Comparing `tmp/gamestorageapi-0.0.13.tar.gz` & `tmp/gamestorageapi-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamestorageapi-0.0.13.tar", last modified: Sun May 26 14:39:16 2024, max compression
+gzip compressed data, was "gamestorageapi-0.1.13.tar", last modified: Sun May 26 14:50:24 2024, max compression
```

## Comparing `gamestorageapi-0.0.13.tar` & `gamestorageapi-0.1.13.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:39:16.708280 gamestorageapi-0.0.13/
-drwxrwxrwx   0        0        0        0 2024-05-26 14:39:16.659039 gamestorageapi-0.0.13/GameStorageAPI/
--rw-rw-rw-   0        0        0       44 2024-05-26 14:29:42.000000 gamestorageapi-0.0.13/GameStorageAPI/__init__.py
--rw-rw-rw-   0        0        0      439 2024-05-26 14:21:02.000000 gamestorageapi-0.0.13/GameStorageAPI/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:39:16.702042 gamestorageapi-0.0.13/GameStorageAPI.egg-info/
--rw-rw-rw-   0        0        0      469 2024-05-26 14:39:16.000000 gamestorageapi-0.0.13/GameStorageAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-26 14:39:16.000000 gamestorageapi-0.0.13/GameStorageAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:39:16.000000 gamestorageapi-0.0.13/GameStorageAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 14:39:16.000000 gamestorageapi-0.0.13/GameStorageAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-26 14:39:16.000000 gamestorageapi-0.0.13/GameStorageAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-0.0.13/LICENSE
--rw-rw-rw-   0        0        0      469 2024-05-26 14:39:16.704045 gamestorageapi-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 14:39:16.708280 gamestorageapi-0.0.13/setup.cfg
--rw-rw-rw-   0        0        0      643 2024-05-26 14:35:58.000000 gamestorageapi-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:50:24.772006 gamestorageapi-0.1.13/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:50:24.737998 gamestorageapi-0.1.13/GameStorageAPI/
+-rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-0.1.13/GameStorageAPI/__init__.py
+-rw-rw-rw-   0        0        0      439 2024-05-26 14:21:02.000000 gamestorageapi-0.1.13/GameStorageAPI/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:50:24.766998 gamestorageapi-0.1.13/GameStorageAPI.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-0.1.13/LICENSE
+-rw-rw-rw-   0        0        0      469 2024-05-26 14:50:24.769002 gamestorageapi-0.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:50:24.775000 gamestorageapi-0.1.13/setup.cfg
+-rw-rw-rw-   0        0        0      643 2024-05-26 14:50:06.000000 gamestorageapi-0.1.13/setup.py
```

### Comparing `gamestorageapi-0.0.13/LICENSE` & `gamestorageapi-0.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `gamestorageapi-0.0.13/setup.py` & `gamestorageapi-0.1.13/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.13'
+VERSION = '0.1.13'
 DESCRIPTION = 'StorageAPI for games'
 
 # Setting up
 setup(
     name="GameStorageAPI",
     version=VERSION,
     author="Fouad (Fouad Jabri)",
```

