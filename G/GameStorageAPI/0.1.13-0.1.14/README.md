# Comparing `tmp/gamestorageapi-0.1.13.tar.gz` & `tmp/gamestorageapi-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamestorageapi-0.1.13.tar", last modified: Sun May 26 14:50:24 2024, max compression
+gzip compressed data, was "gamestorageapi-0.1.14.tar", last modified: Sun May 26 14:57:49 2024, max compression
```

## Comparing `gamestorageapi-0.1.13.tar` & `gamestorageapi-0.1.14.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:50:24.772006 gamestorageapi-0.1.13/
-drwxrwxrwx   0        0        0        0 2024-05-26 14:50:24.737998 gamestorageapi-0.1.13/GameStorageAPI/
--rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-0.1.13/GameStorageAPI/__init__.py
--rw-rw-rw-   0        0        0      439 2024-05-26 14:21:02.000000 gamestorageapi-0.1.13/GameStorageAPI/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:50:24.766998 gamestorageapi-0.1.13/GameStorageAPI.egg-info/
--rw-rw-rw-   0        0        0      469 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-26 14:50:24.000000 gamestorageapi-0.1.13/GameStorageAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-0.1.13/LICENSE
--rw-rw-rw-   0        0        0      469 2024-05-26 14:50:24.769002 gamestorageapi-0.1.13/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 14:50:24.775000 gamestorageapi-0.1.13/setup.cfg
--rw-rw-rw-   0        0        0      643 2024-05-26 14:50:06.000000 gamestorageapi-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:49.244875 gamestorageapi-0.1.14/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:49.198875 gamestorageapi-0.1.14/GameStorageAPI/
+-rw-rw-rw-   0        0        0    18036 2024-05-26 13:56:44.000000 gamestorageapi-0.1.14/GameStorageAPI/DataTypes.py
+-rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-0.1.14/GameStorageAPI/__init__.py
+-rw-rw-rw-   0        0        0     6546 2024-05-26 14:55:17.000000 gamestorageapi-0.1.14/GameStorageAPI/game.py
+-rw-rw-rw-   0        0        0      585 2024-05-26 14:57:16.000000 gamestorageapi-0.1.14/GameStorageAPI/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:57:49.241874 gamestorageapi-0.1.14/GameStorageAPI.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-0.1.14/LICENSE
+-rw-rw-rw-   0        0        0      469 2024-05-26 14:57:49.242874 gamestorageapi-0.1.14/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:57:49.245875 gamestorageapi-0.1.14/setup.cfg
+-rw-rw-rw-   0        0        0      631 2024-05-26 14:54:51.000000 gamestorageapi-0.1.14/setup.py
```

### Comparing `gamestorageapi-0.1.13/LICENSE` & `gamestorageapi-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `gamestorageapi-0.1.13/setup.py` & `gamestorageapi-0.1.14/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.13'
+VERSION = '0.1.14'
 DESCRIPTION = 'StorageAPI for games'
 
-# Setting up
+
 setup(
     name="GameStorageAPI",
     version=VERSION,
     author="Fouad (Fouad Jabri)",
     author_email="<fouad.jabri@proton.me>",
     description=DESCRIPTION,
     packages=find_packages(),
```

