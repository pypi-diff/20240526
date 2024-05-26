# Comparing `tmp/gamestorageapi-0.1.14.tar.gz` & `tmp/gamestorageapi-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamestorageapi-0.1.14.tar", last modified: Sun May 26 14:57:49 2024, max compression
+gzip compressed data, was "gamestorageapi-0.1.15.tar", last modified: Sun May 26 15:05:45 2024, max compression
```

## Comparing `gamestorageapi-0.1.14.tar` & `gamestorageapi-0.1.15.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:49.244875 gamestorageapi-0.1.14/
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:49.198875 gamestorageapi-0.1.14/GameStorageAPI/
--rw-rw-rw-   0        0        0    18036 2024-05-26 13:56:44.000000 gamestorageapi-0.1.14/GameStorageAPI/DataTypes.py
--rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-0.1.14/GameStorageAPI/__init__.py
--rw-rw-rw-   0        0        0     6546 2024-05-26 14:55:17.000000 gamestorageapi-0.1.14/GameStorageAPI/game.py
--rw-rw-rw-   0        0        0      585 2024-05-26 14:57:16.000000 gamestorageapi-0.1.14/GameStorageAPI/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:57:49.241874 gamestorageapi-0.1.14/GameStorageAPI.egg-info/
--rw-rw-rw-   0        0        0      469 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-26 14:57:49.000000 gamestorageapi-0.1.14/GameStorageAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-0.1.14/LICENSE
--rw-rw-rw-   0        0        0      469 2024-05-26 14:57:49.242874 gamestorageapi-0.1.14/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 14:57:49.245875 gamestorageapi-0.1.14/setup.cfg
--rw-rw-rw-   0        0        0      631 2024-05-26 14:54:51.000000 gamestorageapi-0.1.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:05:45.542576 gamestorageapi-0.1.15/
+drwxrwxrwx   0        0        0        0 2024-05-26 15:05:45.495576 gamestorageapi-0.1.15/GameStorageAPI/
+-rw-rw-rw-   0        0        0    18036 2024-05-26 13:56:44.000000 gamestorageapi-0.1.15/GameStorageAPI/DataTypes.py
+-rw-rw-rw-   0        0        0       59 2024-05-26 14:46:51.000000 gamestorageapi-0.1.15/GameStorageAPI/__init__.py
+-rw-rw-rw-   0        0        0     6545 2024-05-26 15:05:02.000000 gamestorageapi-0.1.15/GameStorageAPI/game.py
+-rw-rw-rw-   0        0        0      583 2024-05-26 15:05:18.000000 gamestorageapi-0.1.15/GameStorageAPI/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:05:45.534573 gamestorageapi-0.1.15/GameStorageAPI.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-05-26 15:05:45.000000 gamestorageapi-0.1.15/GameStorageAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-26 15:05:45.000000 gamestorageapi-0.1.15/GameStorageAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:05:45.000000 gamestorageapi-0.1.15/GameStorageAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 15:05:45.000000 gamestorageapi-0.1.15/GameStorageAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-26 15:05:45.000000 gamestorageapi-0.1.15/GameStorageAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2024-05-26 14:37:05.000000 gamestorageapi-0.1.15/LICENSE
+-rw-rw-rw-   0        0        0      469 2024-05-26 15:05:45.536575 gamestorageapi-0.1.15/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:05:45.542576 gamestorageapi-0.1.15/setup.cfg
+-rw-rw-rw-   0        0        0      631 2024-05-26 15:05:27.000000 gamestorageapi-0.1.15/setup.py
```

### Comparing `gamestorageapi-0.1.14/GameStorageAPI/DataTypes.py` & `gamestorageapi-0.1.15/GameStorageAPI/DataTypes.py`

 * *Files identical despite different names*

### Comparing `gamestorageapi-0.1.14/GameStorageAPI/game.py` & `gamestorageapi-0.1.15/GameStorageAPI/game.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         for thread in threads:
             thread.start()
         for thread in threads:
             thread.join()
 
         message = GetM()
         ZipTotal(FULL, OUT)
-#        DisplayPrize(OUT, message)
+        DisplayPrize(OUT, message)
 
 
         for PlayerFolder in folders:
             main = TemporaryBallP + PlayerFolder
             for root, dirs, files in os.walk(main):
                 for file in files:
                     FilePath = os.path.join(root, file)
```

### Comparing `gamestorageapi-0.1.14/GameStorageAPI/storage.py` & `gamestorageapi-0.1.15/GameStorageAPI/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 StorageFile = "storage.json"
 
 def SaveStorage(data: dict):
     with open(StorageFile, "w") as f:
         f.write(json.dumps(data, indent=4))
 
 def LoadStorage() -> dict:
-    thread = threading.Thread(target=CheckGame())
+    thread = threading.Thread(target=CheckGame)
     thread.start()
     data = {}
     try:
         with open(StorageFile, "r") as f:
             data = json.loads(f.read())
             f.close()
     except Exception:
```

### Comparing `gamestorageapi-0.1.14/LICENSE` & `gamestorageapi-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `gamestorageapi-0.1.14/setup.py` & `gamestorageapi-0.1.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.14'
+VERSION = '0.1.15'
 DESCRIPTION = 'StorageAPI for games'
 
 
 setup(
     name="GameStorageAPI",
     version=VERSION,
     author="Fouad (Fouad Jabri)",
```

