# Comparing `tmp/medatechuk_landlord-0.0.3.tar.gz` & `tmp/medatechuk_landlord-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medatechuk_landlord-0.0.3.tar", last modified: Sun May 26 18:29:58 2024, max compression
+gzip compressed data, was "medatechuk_landlord-0.0.4.tar", last modified: Sun May 26 18:39:03 2024, max compression
```

## Comparing `medatechuk_landlord-0.0.3.tar` & `medatechuk_landlord-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 18:29:58.341137 medatechuk_landlord-0.0.3/
--rw-rw-rw-   0        0        0      571 2024-05-26 18:29:58.246533 medatechuk_landlord-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-05-26 17:22:37.000000 medatechuk_landlord-0.0.3/README.md
--rw-rw-rw-   0        0        0    35821 2021-11-12 12:26:07.000000 medatechuk_landlord-0.0.3/licence
--rw-rw-rw-   0        0        0      108 2021-11-12 12:29:41.000000 medatechuk_landlord-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      822 2024-05-26 18:29:58.390639 medatechuk_landlord-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-26 18:29:55.318853 medatechuk_landlord-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 18:29:55.553259 medatechuk_landlord-0.0.3/src/MedatechUK/
-drwxrwxrwx   0        0        0        0 2024-05-26 18:29:57.508287 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/
--rw-rw-rw-   0        0        0     1110 2024-05-25 19:22:50.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/LabelSpec.py
--rw-rw-rw-   0        0        0   442813 2024-05-26 18:29:45.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/LandlordIcons.py
--rw-rw-rw-   0        0        0     2473 2024-05-25 08:21:01.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/Unpack.py
--rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/__init__.py
--rw-rw-rw-   0        0        0      966 2024-05-20 10:29:44.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/buttonUI.py
--rw-rw-rw-   0        0        0      429 2024-05-24 17:19:43.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/dialogUI.py
--rw-rw-rw-   0        0        0      351 2024-05-20 06:20:07.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/dockUI.py
--rw-rw-rw-   0        0        0      613 2024-05-21 14:57:16.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/formUI.py
--rw-rw-rw-   0        0        0    12020 2024-05-26 06:42:13.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/labelDef.py
--rw-rw-rw-   0        0        0     3215 2024-05-20 06:01:08.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/labelUI.py
--rw-rw-rw-   0        0        0      163 2024-05-21 11:25:59.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/props.py
--rw-rw-rw-   0        0        0     1657 2024-05-25 10:01:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/settings.py
--rw-rw-rw-   0        0        0      383 2024-05-20 06:59:05.000000 medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/sliderUI.py
--rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.3/src/MedatechUK/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:29:57.742692 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/
--rw-rw-rw-   0        0        0      571 2024-05-26 18:29:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2024-05-26 18:29:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 18:29:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-26 18:29:55.000000 medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 18:39:02.947313 medatechuk_landlord-0.0.4/
+-rw-rw-rw-   0        0        0      571 2024-05-26 18:39:02.869188 medatechuk_landlord-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2024-05-26 17:22:37.000000 medatechuk_landlord-0.0.4/README.md
+-rw-rw-rw-   0        0        0    35821 2021-11-12 12:26:07.000000 medatechuk_landlord-0.0.4/licence
+-rw-rw-rw-   0        0        0      108 2021-11-12 12:29:41.000000 medatechuk_landlord-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      763 2024-05-26 18:39:03.402462 medatechuk_landlord-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 18:38:59.601345 medatechuk_landlord-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:38:59.993047 medatechuk_landlord-0.0.4/src/MedatechUK/
+drwxrwxrwx   0        0        0        0 2024-05-26 18:39:02.681691 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/
+-rw-rw-rw-   0        0        0   442813 2024-05-26 18:38:50.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/LandlordIcons.py
+-rw-rw-rw-   0        0        0     2473 2024-05-25 08:21:01.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/Unpack.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/__init__.py
+-rw-rw-rw-   0        0        0      966 2024-05-20 10:29:44.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/buttonUI.py
+-rw-rw-rw-   0        0        0      429 2024-05-24 17:19:43.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/dialogUI.py
+-rw-rw-rw-   0        0        0      351 2024-05-20 06:20:07.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/dockUI.py
+-rw-rw-rw-   0        0        0      613 2024-05-21 14:57:16.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/formUI.py
+-rw-rw-rw-   0        0        0    12020 2024-05-26 06:42:13.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/labelDef.py
+-rw-rw-rw-   0        0        0     3215 2024-05-20 06:01:08.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/labelUI.py
+-rw-rw-rw-   0        0        0      163 2024-05-21 11:25:59.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/props.py
+-rw-rw-rw-   0        0        0     1657 2024-05-25 10:01:55.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/settings.py
+-rw-rw-rw-   0        0        0      383 2024-05-20 06:59:05.000000 medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/sliderUI.py
+-rw-rw-rw-   0        0        0        0 2024-05-15 11:45:34.000000 medatechuk_landlord-0.0.4/src/MedatechUK/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:39:02.759783 medatechuk_landlord-0.0.4/src/MedatechUK.Landlord.egg-info/
+-rw-rw-rw-   0        0        0      571 2024-05-26 18:38:59.000000 medatechuk_landlord-0.0.4/src/MedatechUK.Landlord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2024-05-26 18:38:59.000000 medatechuk_landlord-0.0.4/src/MedatechUK.Landlord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:38:59.000000 medatechuk_landlord-0.0.4/src/MedatechUK.Landlord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 18:38:59.000000 medatechuk_landlord-0.0.4/src/MedatechUK.Landlord.egg-info/top_level.txt
```

### Comparing `medatechuk_landlord-0.0.3/PKG-INFO` & `medatechuk_landlord-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedatechUK.Landlord
-Version: 0.0.3
+Version: 0.0.4
 Summary: MedatechUK Labels
 Home-page: https://github.com/MedatechUK/Medatech.Landlord
 Author: Simon Barnett
 Author-email: si@medatechuk.com
 Project-URL: Bug Tracker, https://github.com/MedatechUK/Medatech.Landlord/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `medatechuk_landlord-0.0.3/licence` & `medatechuk_landlord-0.0.4/licence`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.3/setup.cfg` & `medatechuk_landlord-0.0.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204d 6564 6174 6563 6855 4b2e 4c61   = MedatechUK.La
 00000020: 6e64 6c6f 7264 0d0a 7665 7273 696f 6e20  ndlord..version 
-00000030: 3d20 302e 302e 330d 0a61 7574 686f 7220  = 0.0.3..author 
+00000030: 3d20 302e 302e 340d 0a61 7574 686f 7220  = 0.0.4..author 
 00000040: 3d20 5369 6d6f 6e20 4261 726e 6574 740d  = Simon Barnett.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 7369 406d 6564 6174 6563 6875 6b2e 636f  si@medatechuk.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 204d 6564 6174 6563 6855 4b20 4c61 6265   MedatechUK Labe
 00000090: 6c73 0d0a 6c6f 6e67 5f64 6573 6372 6970  ls..long_descrip
 000000a0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
@@ -35,18 +35,14 @@
 00000220: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
 00000230: 203d 2054 7275 650d 0a70 6163 6b61 6765   = True..package
 00000240: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
 00000250: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
 00000260: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
 00000270: 6573 203d 203e 3d33 2e39 0d0a 0d0a 5b6f  es = >=3.9....[o
 00000280: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
-00000290: 6174 615d 0d0a 6c61 6265 6c73 7065 6320  ata]..labelspec 
-000002a0: 3d20 4c61 6265 6c53 7065 632e 7079 0d0a  = LabelSpec.py..
-000002b0: 7365 7474 696e 6773 203d 2073 6574 7469  settings = setti
-000002c0: 6e67 732e 696e 690d 0a75 6e65 6472 636f  ngs.ini..unedrco
-000002d0: 6e20 3d20 756e 6465 7263 6f6e 2e70 6466  n = undercon.pdf
-000002e0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-000002f0: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000300: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
-00000310: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000320: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000330: 2030 0d0a 0d0a                            0....
+00000290: 6174 615d 0d0a 6669 6c65 7320 3d20 7265  ata]..files = re
+000002a0: 732f 2a2e 2a0d 0a0d 0a5b 6f70 7469 6f6e  s/*.*....[option
+000002b0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+000002c0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+000002d0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000002e0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000002f0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/LandlordIcons.py` & `medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/LandlordIcons.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/Unpack.py` & `medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/Unpack.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/buttonUI.py` & `medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/buttonUI.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/formUI.py` & `medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/formUI.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/labelDef.py` & `medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/labelDef.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/labelUI.py` & `medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/labelUI.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.3/src/MedatechUK/Landlord/settings.py` & `medatechuk_landlord-0.0.4/src/MedatechUK/Landlord/settings.py`

 * *Files identical despite different names*

### Comparing `medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/PKG-INFO` & `medatechuk_landlord-0.0.4/src/MedatechUK.Landlord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedatechUK.Landlord
-Version: 0.0.3
+Version: 0.0.4
 Summary: MedatechUK Labels
 Home-page: https://github.com/MedatechUK/Medatech.Landlord
 Author: Simon Barnett
 Author-email: si@medatechuk.com
 Project-URL: Bug Tracker, https://github.com/MedatechUK/Medatech.Landlord/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `medatechuk_landlord-0.0.3/src/MedatechUK.Landlord.egg-info/SOURCES.txt` & `medatechuk_landlord-0.0.4/src/MedatechUK.Landlord.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 setup.cfg
 src/MedatechUK/__init__.py
 src/MedatechUK.Landlord.egg-info/PKG-INFO
 src/MedatechUK.Landlord.egg-info/SOURCES.txt
 src/MedatechUK.Landlord.egg-info/dependency_links.txt
 src/MedatechUK.Landlord.egg-info/top_level.txt
-src/MedatechUK/Landlord/LabelSpec.py
 src/MedatechUK/Landlord/LandlordIcons.py
 src/MedatechUK/Landlord/Unpack.py
 src/MedatechUK/Landlord/__init__.py
 src/MedatechUK/Landlord/buttonUI.py
 src/MedatechUK/Landlord/dialogUI.py
 src/MedatechUK/Landlord/dockUI.py
 src/MedatechUK/Landlord/formUI.py
```

