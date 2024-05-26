# Comparing `tmp/medatechuk_landlord-0.0.5.tar.gz` & `tmp/medatechuk_landlord-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medatechuk_landlord-0.0.5.tar", last modified: Sun May 26 18:53:30 2024, max compression
+gzip compressed data, was "medatechuk_landlord-0.0.6.tar", last modified: Sun May 26 18:56:45 2024, max compression
```

## Comparing `medatechuk_landlord-0.0.5.tar` & `medatechuk_landlord-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 18:53:30.515461 medatechuk_landlord-0.0.5/
--rw-rw-rw-   0        0        0      571 2024-05-26 18:53:30.437373 medatechuk_landlord-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-05-26 17:22:37.000000 medatechuk_landlord-0.0.5/README.md
--rw-rw-rw-   0        0        0    35821 2021-11-12 12:26:07.000000 medatechuk_landlord-0.0.5/licence
--rw-rw-rw-   0        0        0      108 2021-11-12 12:29:41.000000 medatechuk_landlord-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      789 2024-05-26 18:53:30.531091 medatechuk_landlord-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-26 18:53:27.155415 medatechuk_landlord-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 18:53:27.506186 medatechuk_landlord-0.0.5/src/MedatechUK/
-drwxrwxrwx   0        0        0        0 2024-05-26 18:53:29.959800 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/
--rw-rw-rw-   0        0        0   442813 2024-05-26 18:53:19.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/LandlordIcons.py
--rw-rw-rw-   0        0        0     2473 2024-05-25 08:21:01.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/Unpack.py
--rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/__init__.py
--rw-rw-rw-   0        0        0      966 2024-05-20 10:29:44.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/buttonUI.py
--rw-rw-rw-   0        0        0      429 2024-05-24 17:19:43.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/dialogUI.py
--rw-rw-rw-   0        0        0      351 2024-05-20 06:20:07.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/dockUI.py
--rw-rw-rw-   0        0        0      613 2024-05-21 14:57:16.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/formUI.py
--rw-rw-rw-   0        0        0    12020 2024-05-26 06:42:13.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/labelDef.py
--rw-rw-rw-   0        0        0     3215 2024-05-20 06:01:08.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/labelUI.py
--rw-rw-rw-   0        0        0      163 2024-05-21 11:25:59.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/props.py
--rw-rw-rw-   0        0        0     1657 2024-05-25 10:01:55.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/settings.py
--rw-rw-rw-   0        0        0      383 2024-05-20 06:59:05.000000 medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/sliderUI.py
--rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.5/src/MedatechUK/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:53:30.262611 medatechuk_landlord-0.0.5/src/MedatechUK.Landlord.egg-info/
--rw-rw-rw-   0        0        0      571 2024-05-26 18:53:27.000000 medatechuk_landlord-0.0.5/src/MedatechUK.Landlord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      684 2024-05-26 18:53:27.000000 medatechuk_landlord-0.0.5/src/MedatechUK.Landlord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 18:53:27.000000 medatechuk_landlord-0.0.5/src/MedatechUK.Landlord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-26 18:53:27.000000 medatechuk_landlord-0.0.5/src/MedatechUK.Landlord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 18:56:44.384128 medatechuk_landlord-0.0.6/
+-rw-rw-rw-   0        0        0      571 2024-05-26 18:56:44.180883 medatechuk_landlord-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2024-05-26 17:22:37.000000 medatechuk_landlord-0.0.6/README.md
+-rw-rw-rw-   0        0        0    35821 2021-11-12 12:26:07.000000 medatechuk_landlord-0.0.6/licence
+-rw-rw-rw-   0        0        0      108 2021-11-12 12:29:41.000000 medatechuk_landlord-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      789 2024-05-26 18:56:44.681018 medatechuk_landlord-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 18:56:41.671958 medatechuk_landlord-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:56:41.903617 medatechuk_landlord-0.0.6/src/MedatechUK/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:56:43.346215 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/
+-rw-rw-rw-   0        0        0   442813 2024-05-26 18:56:32.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/LandlordIcons.py
+-rw-rw-rw-   0        0        0     2473 2024-05-25 08:21:01.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/Unpack.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/__init__.py
+-rw-rw-rw-   0        0        0      966 2024-05-20 10:29:44.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/buttonUI.py
+-rw-rw-rw-   0        0        0      429 2024-05-24 17:19:43.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/dialogUI.py
+-rw-rw-rw-   0        0        0      351 2024-05-20 06:20:07.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/dockUI.py
+-rw-rw-rw-   0        0        0      613 2024-05-21 14:57:16.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/formUI.py
+-rw-rw-rw-   0        0        0    12020 2024-05-26 06:42:13.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/labelDef.py
+-rw-rw-rw-   0        0        0     3215 2024-05-20 06:01:08.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/labelUI.py
+-rw-rw-rw-   0        0        0      163 2024-05-21 11:25:59.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/props.py
+-rw-rw-rw-   0        0        0     1657 2024-05-25 10:01:55.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/settings.py
+-rw-rw-rw-   0        0        0      383 2024-05-20 06:59:05.000000 medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/sliderUI.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.6/src/MedatechUK/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:56:43.857690 medatechuk_landlord-0.0.6/src/MedatechUK.Landlord.egg-info/
+-rw-rw-rw-   0        0        0      571 2024-05-26 18:56:41.000000 medatechuk_landlord-0.0.6/src/MedatechUK.Landlord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2024-05-26 18:56:41.000000 medatechuk_landlord-0.0.6/src/MedatechUK.Landlord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:56:41.000000 medatechuk_landlord-0.0.6/src/MedatechUK.Landlord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 18:56:41.000000 medatechuk_landlord-0.0.6/src/MedatechUK.Landlord.egg-info/top_level.txt
```

### Comparing `medatechuk_landlord-0.0.5/PKG-INFO` & `medatechuk_landlord-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedatechUK.Landlord
-Version: 0.0.5
+Version: 0.0.6
 Summary: MedatechUK Labels
 Home-page: https://github.com/MedatechUK/Medatech.Landlord
 Author: Simon Barnett
 Author-email: si@medatechuk.com
 Project-URL: Bug Tracker, https://github.com/MedatechUK/Medatech.Landlord/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `medatechuk_landlord-0.0.5/licence` & `medatechuk_landlord-0.0.6/licence`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.5/setup.cfg` & `medatechuk_landlord-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204d 6564 6174 6563 6855 4b2e 4c61   = MedatechUK.La
 00000020: 6e64 6c6f 7264 0d0a 7665 7273 696f 6e20  ndlord..version 
-00000030: 3d20 302e 302e 350d 0a61 7574 686f 7220  = 0.0.5..author 
+00000030: 3d20 302e 302e 360d 0a61 7574 686f 7220  = 0.0.6..author 
 00000040: 3d20 5369 6d6f 6e20 4261 726e 6574 740d  = Simon Barnett.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 7369 406d 6564 6174 6563 6875 6b2e 636f  si@medatechuk.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 204d 6564 6174 6563 6855 4b20 4c61 6265   MedatechUK Labe
 00000090: 6c73 0d0a 6c6f 6e67 5f64 6573 6372 6970  ls..long_descrip
 000000a0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
```

### Comparing `medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/LandlordIcons.py` & `medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/LandlordIcons.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/Unpack.py` & `medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/Unpack.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/buttonUI.py` & `medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/buttonUI.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/formUI.py` & `medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/formUI.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/labelDef.py` & `medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/labelDef.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/labelUI.py` & `medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/labelUI.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.5/src/MedatechUK/Landlord/settings.py` & `medatechuk_landlord-0.0.6/src/MedatechUK/Landlord/settings.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.5/src/MedatechUK.Landlord.egg-info/PKG-INFO` & `medatechuk_landlord-0.0.6/src/MedatechUK.Landlord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedatechUK.Landlord
-Version: 0.0.5
+Version: 0.0.6
 Summary: MedatechUK Labels
 Home-page: https://github.com/MedatechUK/Medatech.Landlord
 Author: Simon Barnett
 Author-email: si@medatechuk.com
 Project-URL: Bug Tracker, https://github.com/MedatechUK/Medatech.Landlord/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `medatechuk_landlord-0.0.5/src/MedatechUK.Landlord.egg-info/SOURCES.txt` & `medatechuk_landlord-0.0.6/src/MedatechUK.Landlord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

