# Comparing `tmp/medatechuk_landlord-0.0.2.tar.gz` & `tmp/medatechuk_landlord-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medatechuk_landlord-0.0.2.tar", last modified: Sun May 26 17:24:00 2024, max compression
+gzip compressed data, was "medatechuk_landlord-0.0.3.tar", last modified: Sun May 26 18:29:58 2024, max compression
```

## Comparing `medatechuk_landlord-0.0.2.tar` & `medatechuk_landlord-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 17:24:00.331885 medatechuk_landlord-0.0.2/
--rw-rw-rw-   0        0        0      571 2024-05-26 17:24:00.316295 medatechuk_landlord-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-05-26 17:22:37.000000 medatechuk_landlord-0.0.2/README.md
--rw-rw-rw-   0        0        0    35821 2021-11-12 12:26:07.000000 medatechuk_landlord-0.0.2/licence
--rw-rw-rw-   0        0        0      108 2021-11-12 12:29:41.000000 medatechuk_landlord-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      720 2024-05-26 17:24:00.366860 medatechuk_landlord-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-26 17:23:56.100749 medatechuk_landlord-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 17:23:56.431522 medatechuk_landlord-0.0.2/src/MedatechUK/
-drwxrwxrwx   0        0        0        0 2024-05-26 17:24:00.096609 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/
--rw-rw-rw-   0        0        0     1110 2024-05-25 19:22:50.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/LabelSpec.py
--rw-rw-rw-   0        0        0   442811 2024-05-26 15:23:07.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/LandlordIcons.py
--rw-rw-rw-   0        0        0     2473 2024-05-25 08:21:01.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/Unpack.py
--rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/__init__.py
--rw-rw-rw-   0        0        0      966 2024-05-20 10:29:44.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/buttonUI.py
--rw-rw-rw-   0        0        0      429 2024-05-24 17:19:43.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/dialogUI.py
--rw-rw-rw-   0        0        0      351 2024-05-20 06:20:07.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/dockUI.py
--rw-rw-rw-   0        0        0      613 2024-05-21 14:57:16.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/formUI.py
--rw-rw-rw-   0        0        0    12020 2024-05-26 06:42:13.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/labelDef.py
--rw-rw-rw-   0        0        0     3215 2024-05-20 06:01:08.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/labelUI.py
--rw-rw-rw-   0        0        0      163 2024-05-21 11:25:59.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/props.py
--rw-rw-rw-   0        0        0     1657 2024-05-25 10:01:55.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/settings.py
--rw-rw-rw-   0        0        0      383 2024-05-20 06:59:05.000000 medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/sliderUI.py
--rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.2/src/MedatechUK/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:24:00.237845 medatechuk_landlord-0.0.2/src/MedatechUK.Landlord.egg-info/
--rw-rw-rw-   0        0        0      571 2024-05-26 17:23:55.000000 medatechuk_landlord-0.0.2/src/MedatechUK.Landlord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2024-05-26 17:23:56.000000 medatechuk_landlord-0.0.2/src/MedatechUK.Landlord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 17:23:55.000000 medatechuk_landlord-0.0.2/src/MedatechUK.Landlord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-26 17:23:55.000000 medatechuk_landlord-0.0.2/src/MedatechUK.Landlord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 18:29:58.341137 medatechuk_landlord-0.0.3/
+-rw-rw-rw-   0        0        0      571 2024-05-26 18:29:58.246533 medatechuk_landlord-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2024-05-26 17:22:37.000000 medatechuk_landlord-0.0.3/README.md
+-rw-rw-rw-   0        0        0    35821 2021-11-12 12:26:07.000000 medatechuk_landlord-0.0.3/licence
+-rw-rw-rw-   0        0        0      108 2021-11-12 12:29:41.000000 medatechuk_landlord-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      822 2024-05-26 18:29:58.390639 medatechuk_landlord-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 18:29:55.318853 medatechuk_landlord-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:29:55.553259 medatechuk_landlord-0.0.3/src/MedatechUK/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:29:57.508287 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/
+-rw-rw-rw-   0        0        0     1110 2024-05-25 19:22:50.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/LabelSpec.py
+-rw-rw-rw-   0        0        0   442813 2024-05-26 18:29:45.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/LandlordIcons.py
+-rw-rw-rw-   0        0        0     2473 2024-05-25 08:21:01.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/Unpack.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/__init__.py
+-rw-rw-rw-   0        0        0      966 2024-05-20 10:29:44.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/buttonUI.py
+-rw-rw-rw-   0        0        0      429 2024-05-24 17:19:43.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/dialogUI.py
+-rw-rw-rw-   0        0        0      351 2024-05-20 06:20:07.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/dockUI.py
+-rw-rw-rw-   0        0        0      613 2024-05-21 14:57:16.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/formUI.py
+-rw-rw-rw-   0        0        0    12020 2024-05-26 06:42:13.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/labelDef.py
+-rw-rw-rw-   0        0        0     3215 2024-05-20 06:01:08.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/labelUI.py
+-rw-rw-rw-   0        0        0      163 2024-05-21 11:25:59.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/props.py
+-rw-rw-rw-   0        0        0     1657 2024-05-25 10:01:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/settings.py
+-rw-rw-rw-   0        0        0      383 2024-05-20 06:59:05.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/sliderUI.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.3/src/MedatechUK/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:29:57.742692 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/
+-rw-rw-rw-   0        0        0      571 2024-05-26 18:29:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      721 2024-05-26 18:29:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:29:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 18:29:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/top_level.txt
```

### Comparing `medatechuk_landlord-0.0.2/PKG-INFO` & `medatechuk_landlord-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MedatechUK.Landlord
-Version: 0.0.2
+Version: 0.0.3
 Summary: MedatechUK Labels
 Home-page: https://github.com/MedatechUK/Medatech.Landlord
 Author: Simon Barnett
 Author-email: si@medatechuk.com
 Project-URL: Bug Tracker, https://github.com/MedatechUK/Medatech.Landlord/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: licence
 
 # Landlord Labels
```

### Comparing `medatechuk_landlord-0.0.2/licence` & `medatechuk_landlord-0.0.3/licence`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/LabelSpec.py` & `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/LabelSpec.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/LandlordIcons.py` & `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/LandlordIcons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Resource object code (Python 3)
 # Created by: object code
 # Created by: The Resource Compiler for Qt version 6.7.0
 # WARNING! All changes made in this file will be lost!
 
-from PyQt6 import QtCore
+from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00)!\
 \x00\
 \x02\x84\xc2x\xda\xed]\x0b\x5cL\xd9\x1f?S\x91P\
 QZJT^\xabeI\xdeV\x0a\xd9E\x16\xeb\xcd\
 zd%\x92\xf5*o\xbbM\xecz'K\x0f\x12Z\
```

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/Unpack.py` & `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/Unpack.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/buttonUI.py` & `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/buttonUI.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/formUI.py` & `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/formUI.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/labelDef.py` & `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/labelDef.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/labelUI.py` & `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/labelUI.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK/Landlord/settings.py` & `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/settings.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK.Landlord.egg-info/PKG-INFO` & `medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MedatechUK.Landlord
-Version: 0.0.2
+Version: 0.0.3
 Summary: MedatechUK Labels
 Home-page: https://github.com/MedatechUK/Medatech.Landlord
 Author: Simon Barnett
 Author-email: si@medatechuk.com
 Project-URL: Bug Tracker, https://github.com/MedatechUK/Medatech.Landlord/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: licence
 
 # Landlord Labels
```

### Comparing `medatechuk_landlord-0.0.2/src/MedatechUK.Landlord.egg-info/SOURCES.txt` & `medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

