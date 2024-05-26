# Comparing `tmp/unyts-0.8.3.tar.gz` & `tmp/unyts-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unyts-0.8.3.tar", last modified: Fri May  3 22:42:47 2024, max compression
+gzip compressed data, was "unyts-0.8.9.tar", last modified: Tue May 21 22:24:59 2024, max compression
```

## Comparing `unyts-0.8.3.tar` & `unyts-0.8.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 22:42:47.220000 unyts-0.8.3/
--rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 unyts-0.8.3/LICENSE
--rw-rw-rw-   0        0        0       66 2024-02-11 22:13:34.000000 unyts-0.8.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6631 2024-05-03 22:42:48.000000 unyts-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     4522 2024-05-03 22:25:22.000000 unyts-0.8.3/README.md
--rw-rw-rw-   0        0        0      982 2024-05-03 22:42:08.000000 unyts-0.8.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-03 22:42:48.000000 unyts-0.8.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-03 22:42:47.230000 unyts-0.8.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 22:42:47.230000 unyts-0.8.3/src/unyts/
--rw-rw-rw-   0        0        0      495 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/Empty.py
--rw-rw-rw-   0        0        0     1400 2024-05-03 22:42:08.000000 unyts-0.8.3/src/unyts/__init__.py
--rw-rw-rw-   0        0        0      146 2024-05-03 22:18:52.000000 unyts-0.8.3/src/unyts/__main__.py
--rw-rw-rw-   0        0        0    26470 2024-05-03 22:18:52.000000 unyts-0.8.3/src/unyts/converter.py
--rw-rw-rw-   0        0        0    48716 2024-05-03 22:18:52.000000 unyts-0.8.3/src/unyts/database.py
--rw-rw-rw-   0        0        0    23518 2024-05-03 22:18:52.000000 unyts-0.8.3/src/unyts/dictionaries.py
--rw-rw-rw-   0        0        0      862 2022-12-29 13:49:38.000000 unyts-0.8.3/src/unyts/errors.py
--rw-rw-rw-   0        0        0     7147 2024-05-03 22:18:52.000000 unyts-0.8.3/src/unyts/gui.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:42:47.230000 unyts-0.8.3/src/unyts/helpers/
--rw-rw-rw-   0        0        0      158 2022-09-20 21:54:58.000000 unyts-0.8.3/src/unyts/helpers/__init__.py
--rw-rw-rw-   0        0        0     7475 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/helpers/caster.py
--rw-rw-rw-   0        0        0     2100 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/helpers/common_classes.py
--rw-rw-rw-   0        0        0      952 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/helpers/is_number.py
--rw-rw-rw-   0        0        0     1142 2023-01-18 21:37:24.000000 unyts-0.8.3/src/unyts/helpers/is_unit.py
--rw-rw-rw-   0        0        0     1987 2023-01-17 21:17:22.000000 unyts-0.8.3/src/unyts/helpers/multi_split.py
--rw-rw-rw-   0        0        0     3538 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/helpers/unit_string_tools.py
--rw-rw-rw-   0        0        0     6576 2024-05-03 22:18:52.000000 unyts-0.8.3/src/unyts/network.py
--rw-rw-rw-   0        0        0    11085 2023-07-24 18:15:20.000000 unyts-0.8.3/src/unyts/operations.py
--rw-rw-rw-   0        0        0      149 2024-05-03 22:18:52.000000 unyts-0.8.3/src/unyts/parameters.ini
--rw-rw-rw-   0        0        0     6289 2024-05-03 22:18:52.000000 unyts-0.8.3/src/unyts/parameters.py
--rw-rw-rw-   0        0        0     2695 2024-02-11 22:13:34.000000 unyts-0.8.3/src/unyts/searches.py
--rw-rw-rw-   0        0        0    28535 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/unit_class.py
--rw-rw-rw-   0        0        0     2078 2023-01-30 12:24:34.000000 unyts-0.8.3/src/unyts/unitary.py
-drwxrwxrwx   0        0        0        0 2024-05-03 22:42:47.240000 unyts-0.8.3/src/unyts/units/
--rw-rw-rw-   0        0        0      129 2022-09-08 15:55:48.000000 unyts-0.8.3/src/unyts/units/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/custom.py
--rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/data.py
--rw-rw-rw-   0        0        0     1230 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/date.py
--rw-rw-rw-   0        0        0     2288 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/define.py
--rw-rw-rw-   0        0        0     6288 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/energy.py
--rw-rw-rw-   0        0        0     2301 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/force.py
--rw-rw-rw-   0        0        0     1881 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/geometry.py
--rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/mass.py
--rw-rw-rw-   0        0        0     1629 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/rates.py
--rw-rw-rw-   0        0        0     1999 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/ratios.py
--rw-rw-rw-   0        0        0     1198 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/temperature.py
--rw-rw-rw-   0        0        0     1328 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/time.py
--rw-rw-rw-   0        0        0     2601 2023-12-30 23:46:12.000000 unyts-0.8.3/src/unyts/units/unitless.py
--rw-rw-rw-   0        0        0   248691 2024-05-03 22:18:52.000000 unyts-0.8.3/src/unyts/unyts_icon.ico
-drwxrwxrwx   0        0        0        0 2024-05-03 22:42:47.230000 unyts-0.8.3/src/unyts.egg-info/
--rw-rw-rw-   0        0        0     6631 2024-05-03 22:42:48.000000 unyts-0.8.3/src/unyts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1282 2024-05-03 22:42:48.000000 unyts-0.8.3/src/unyts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 22:42:48.000000 unyts-0.8.3/src/unyts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-03 22:42:48.000000 unyts-0.8.3/src/unyts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 22:42:48.000000 unyts-0.8.3/src/unyts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 22:42:47.240000 unyts-0.8.3/tests/
--rw-rw-rw-   0        0        0     5512 2023-05-23 22:04:30.000000 unyts-0.8.3/tests/test_converter.py
--rw-rw-rw-   0        0        0     2241 2023-01-30 12:24:34.000000 unyts-0.8.3/tests/test_dictionaries.py
--rw-rw-rw-   0        0        0     1597 2023-01-17 21:17:22.000000 unyts-0.8.3/tests/test_operations.py
--rw-rw-rw-   0        0        0      808 2023-01-30 12:24:34.000000 unyts-0.8.3/tests/test_uncertain_units.py
--rw-rw-rw-   0        0        0     6368 2024-05-03 22:18:52.000000 unyts-0.8.3/tests/test_units.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:24:59.190000 unyts-0.8.9/
+-rw-rw-rw-   0        0        0     1077 2020-11-01 00:39:44.000000 unyts-0.8.9/LICENSE
+-rw-rw-rw-   0        0        0       68 2024-05-21 22:24:54.000000 unyts-0.8.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6631 2024-05-21 22:25:00.000000 unyts-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4522 2024-05-03 22:25:22.000000 unyts-0.8.9/README.md
+-rw-rw-rw-   0        0        0      982 2024-05-21 22:11:48.000000 unyts-0.8.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 22:25:00.000000 unyts-0.8.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 22:24:59.200000 unyts-0.8.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 22:24:59.200000 unyts-0.8.9/src/unyts/
+-rw-rw-rw-   0        0        0      495 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/Empty.py
+-rw-rw-rw-   0        0        0     1433 2024-05-21 21:25:36.000000 unyts-0.8.9/src/unyts/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-05-03 22:18:52.000000 unyts-0.8.9/src/unyts/__main__.py
+-rw-rw-rw-   0        0        0    36806 2024-05-21 21:26:06.000000 unyts-0.8.9/src/unyts/converter.py
+-rw-rw-rw-   0        0        0    49804 2024-05-21 21:26:30.000000 unyts-0.8.9/src/unyts/database.py
+-rw-rw-rw-   0        0        0    25812 2024-05-21 22:02:42.000000 unyts-0.8.9/src/unyts/dictionaries.py
+-rw-rw-rw-   0        0        0      862 2022-12-29 13:49:38.000000 unyts-0.8.9/src/unyts/errors.py
+-rw-rw-rw-   0        0        0     9567 2024-05-21 21:26:56.000000 unyts-0.8.9/src/unyts/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:24:59.210000 unyts-0.8.9/src/unyts/helpers/
+-rw-rw-rw-   0        0        0      158 2022-09-20 21:54:58.000000 unyts-0.8.9/src/unyts/helpers/__init__.py
+-rw-rw-rw-   0        0        0     7475 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/helpers/caster.py
+-rw-rw-rw-   0        0        0     2100 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/helpers/common_classes.py
+-rw-rw-rw-   0        0        0      952 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/helpers/is_number.py
+-rw-rw-rw-   0        0        0     1142 2023-01-18 21:37:24.000000 unyts-0.8.9/src/unyts/helpers/is_unit.py
+-rw-rw-rw-   0        0        0     1987 2023-01-17 21:17:22.000000 unyts-0.8.9/src/unyts/helpers/multi_split.py
+-rw-rw-rw-   0        0        0     3538 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/helpers/unit_string_tools.py
+-rw-rw-rw-   0        0        0     6576 2024-05-03 22:18:52.000000 unyts-0.8.9/src/unyts/network.py
+-rw-rw-rw-   0        0        0    11161 2024-05-21 21:27:20.000000 unyts-0.8.9/src/unyts/operations.py
+-rw-rw-rw-   0        0        0      170 2024-05-21 22:17:14.000000 unyts-0.8.9/src/unyts/parameters.ini
+-rw-rw-rw-   0        0        0     8130 2024-05-21 21:27:48.000000 unyts-0.8.9/src/unyts/parameters.py
+-rw-rw-rw-   0        0        0     2695 2024-02-11 22:13:34.000000 unyts-0.8.9/src/unyts/searches.py
+-rw-rw-rw-   0        0        0    28535 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/unit_class.py
+-rw-rw-rw-   0        0        0     2078 2023-01-30 12:24:34.000000 unyts-0.8.9/src/unyts/unitary.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:24:59.210000 unyts-0.8.9/src/unyts/units/
+-rw-rw-rw-   0        0        0      129 2022-09-08 15:55:48.000000 unyts-0.8.9/src/unyts/units/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/custom.py
+-rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/data.py
+-rw-rw-rw-   0        0        0     1230 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/date.py
+-rw-rw-rw-   0        0        0     2288 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/define.py
+-rw-rw-rw-   0        0        0     6288 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/energy.py
+-rw-rw-rw-   0        0        0     2301 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/force.py
+-rw-rw-rw-   0        0        0     1881 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/geometry.py
+-rw-rw-rw-   0        0        0      726 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/mass.py
+-rw-rw-rw-   0        0        0     1629 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/rates.py
+-rw-rw-rw-   0        0        0     1999 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/ratios.py
+-rw-rw-rw-   0        0        0     1198 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/temperature.py
+-rw-rw-rw-   0        0        0     1328 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/time.py
+-rw-rw-rw-   0        0        0     2601 2023-12-30 23:46:12.000000 unyts-0.8.9/src/unyts/units/unitless.py
+-rw-rw-rw-   0        0        0   248691 2024-05-03 22:18:52.000000 unyts-0.8.9/src/unyts/unyts_icon.ico
+drwxrwxrwx   0        0        0        0 2024-05-21 22:24:59.210000 unyts-0.8.9/src/unyts.egg-info/
+-rw-rw-rw-   0        0        0     6631 2024-05-21 22:25:00.000000 unyts-0.8.9/src/unyts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1282 2024-05-21 22:25:00.000000 unyts-0.8.9/src/unyts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 22:25:00.000000 unyts-0.8.9/src/unyts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-21 22:25:00.000000 unyts-0.8.9/src/unyts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 22:25:00.000000 unyts-0.8.9/src/unyts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 22:24:59.210000 unyts-0.8.9/tests/
+-rw-rw-rw-   0        0        0     5512 2023-05-23 22:04:30.000000 unyts-0.8.9/tests/test_converter.py
+-rw-rw-rw-   0        0        0     2269 2024-05-21 22:14:16.000000 unyts-0.8.9/tests/test_dictionaries.py
+-rw-rw-rw-   0        0        0     1597 2023-01-17 21:17:22.000000 unyts-0.8.9/tests/test_operations.py
+-rw-rw-rw-   0        0        0      808 2023-01-30 12:24:34.000000 unyts-0.8.9/tests/test_uncertain_units.py
+-rw-rw-rw-   0        0        0     6368 2024-05-03 22:18:52.000000 unyts-0.8.9/tests/test_units.py
```

### Comparing `unyts-0.8.3/LICENSE` & `unyts-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/PKG-INFO` & `unyts-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unyts
-Version: 0.8.3
+Version: 0.8.9
 Summary: a unit converter based on graph network and classes to operate with units.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `unyts-0.8.3/README.md` & `unyts-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/pyproject.toml` & `unyts-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2022 7365 7475 7074 6f6f 6c73 2e62 7569   "setuptools.bui
 00000050: 6c64 5f6d 6574 6122 0d0a 0d0a 5b74 6f6f  ld_meta"....[too
 00000060: 6c2e 7365 7475 7074 6f6f 6c73 2e70 6163  l.setuptools.pac
 00000070: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
 00000080: 7265 203d 205b 2273 7263 225d 0d0a 0d0a  re = ["src"]....
 00000090: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 000000a0: 3d20 2275 6e79 7473 220d 0a76 6572 7369  = "unyts"..versi
-000000b0: 6f6e 203d 2022 302e 382e 3322 0d0a 6175  on = "0.8.3"..au
+000000b0: 6f6e 203d 2022 302e 382e 3922 0d0a 6175  on = "0.8.9"..au
 000000c0: 7468 6f72 7320 3d20 5b0d 0a20 207b 206e  thors = [..  { n
 000000d0: 616d 653d 224d 6172 7469 6e20 4361 726c  ame="Martin Carl
 000000e0: 6f73 2041 7261 7961 222c 2065 6d61 696c  os Araya", email
 000000f0: 3d22 6d61 7274 696e 6172 6179 6140 676d  ="martinaraya@gm
 00000100: 6169 6c2e 636f 6d22 207d 2c0d 0a5d 0d0a  ail.com" },..]..
 00000110: 6465 7363 7269 7074 696f 6e20 3d20 2261  description = "a
 00000120: 2075 6e69 7420 636f 6e76 6572 7465 7220   unit converter
```

### Comparing `unyts-0.8.3/src/unyts/__init__.py` & `unyts-0.8.9/src/unyts/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 18:24:20 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.8.3'
-__release__ = 20240504
+__version__ = '0.8.9'
+__release__ = 20240521
 __all__ = ['units', 'convert', 'convertible', 'Unit', 'is_Unit',
-           'set_unit', 'set_conversion', 'set_density',
+           'set_unit', 'set_conversion', 'set_density', 'get_density'
            'save', 'start_gui', 'set_fvf']
 
-from .parameters import unyts_parameters_, print_path, reload, raise_error, cache, set_density, get_density
+from .parameters import unyts_parameters_, print_path, reload, raise_error, cache, set_density, get_density, recursion_limit
 from .database import network_to_frame, save_memory, load_memory, set_fvf
 from .units.define import units
 from .converter import convert, convertible
 from .Empty import Empty
 from .unit_class import Unit, is_Unit
 from .units.custom import set_unit, set_conversion
 from .gui import start_gui
 
+
 if unyts_parameters_.show_version_:
     print(f"loaded unyts version {str(__version__)}")
     unyts_parameters_.show_version_ = False
     unyts_parameters_.save_params()
 
 from .unitary import *
```

### Comparing `unyts-0.8.3/src/unyts/converter.py` & `unyts-0.8.9/src/unyts/converter.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 15:57:27 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.6.4'
-__release__ = 20240502
+__version__ = '0.6.5'
+__release__ = 20240521
 __all__ = ['convert', 'convertible']
 
 from .database import units_network
 from .dictionaries import dictionary, temperatureRatioConversions, uncertain_names
 from .Empty import Empty, str_Empty
 from .searches import BFS, print_path
 from .errors import NoConversionFoundError
@@ -199,14 +199,26 @@
                 pair_child = sorted(pair_grandchild, key=len)[0]
                 break
 
     if type(pair_child) is str:
         return pair_child
 
 
+def _get_recursion_limit(recursion=None):
+    if recursion is None:
+        recursion = min(getrecursionlimit() - 15, unyts_parameters_.max_recursion_)
+    elif recursion > 1:
+        recursion = min(getrecursionlimit() - 15, recursion)
+    elif recursion <= 1:
+        recursion = 0
+    else:
+        recursion -= 1
+    return recursion
+
+
 def _get_conversion(value, from_unit, to_unit, recursion=None):
     """
     Helper function to handle looking for the conversion factor of special cases and through the units network.
 
     Parameters
     ----------
     value: numeric or None
@@ -215,20 +227,17 @@
 
     Returns
     -------
         (conversion, conversion_path)
 
     """
     # get and set recursion limit
-    if recursion is None:
-        recursion = min(getrecursionlimit()-15, 250)
-    elif recursion == 1:
+    recursion = _get_recursion_limit(recursion)
+    if recursion == 0:
         return None, None
-    else:
-        recursion -= 1
     # print(f"_get_conversion: {from_unit=}, {to_unit=}")
 
     # check if already solved and memorized
     if (from_unit, to_unit) in units_network.memory:
         conversion_lambda, conversion_path = units_network.memory[(from_unit, to_unit)]
         return (conversion_lambda, conversion_path) if (conversion_lambda is None or value is None) \
             else (conversion_lambda(value), conversion_path)
@@ -313,35 +322,30 @@
     else:
         return None, None
 
 
 def _converter(value, from_unit, to_unit, recursion=None):
     """
     Transform the received value (integer, float, array, series, frame, ...)
-    from the units `from_unit` to the units `to_units`
-    as well as conversion path.
+    from the units `from_unit` to the units `to_units` and report the conversion path used.
 
     Parameters
     ----------
     value: numeric or None
     from_unit: str
     to_unit: str
 
     Returns
     -------
         (conversion, conversion_path)
     """
     # get and set recursion limit
-    if recursion is None:
-        recursion = min(getrecursionlimit()-15, 250)
-    elif recursion == 1:
+    recursion = _get_recursion_limit(recursion)
+    if recursion == 0:
         return None, None
-    else:
-        recursion -= 1
-    # print(f"_converter: {from_unit=}, {to_unit=}")
 
     # reset memory for this variable
     units_network.previous = []
 
     # try to convert
     conv, conv_path = _get_conversion(value, from_unit, to_unit, recursion=recursion)
 
@@ -387,44 +391,187 @@
         conversion_path = [node for path in list_conversion_path for node in path]
         units_network.memory[(from_unit, to_unit)] = lambda x: x * conversion_factor, conversion_path
         if value is None:
             return units_network.memory[(from_unit, to_unit)]
         else:
             return value * conversion_factor, conversion_path
 
-    # look for one to pair conversion path
+    # look for one-to-pair conversion path
     if ('/' in to_unit or '*' in to_unit) and ('/' not in from_unit and '*' not in from_unit):
         from_unit_child = _get_pair_child(from_unit)
         if from_unit_child is not None:
             base_conversion, base_conversion_path = _get_conversion(None, from_unit, from_unit_child, recursion=recursion)
             pair_conversion, pair_conversion_path = _converter(None, from_unit_child, to_unit, recursion=recursion)
             if pair_conversion is not None and base_conversion is not None:
                 conversion_path = base_conversion_path + pair_conversion_path
                 conversion = lambda x: pair_conversion(base_conversion(x))
                 units_network.memory[(from_unit, to_unit)] = conversion, conversion_path
                 if value is None:
                     return units_network.memory[(from_unit, to_unit)]
                 else:
                     return conversion(value), conversion_path
 
-    # look for pair to one conversion path
-    elif ('/' in from_unit or '*' in from_unit) and ('/' not in to_unit or '*' not in to_unit):
+    # look for pair-to-one conversion path
+    elif ('/' in from_unit or '*' in from_unit) and ('/' not in to_unit and '*' not in to_unit):
         to_unit_child = _get_pair_child(to_unit)
         if to_unit_child is not None:
             final_conversion, final_conversion_path = _get_conversion(None, to_unit_child, to_unit, recursion=recursion)
             pair_conversion, pair_conversion_path = _converter(None, from_unit, to_unit_child, recursion=recursion)
             if pair_conversion is not None and final_conversion is not None:
                 conversion_path = pair_conversion_path + final_conversion_path
                 conversion = lambda x: final_conversion(pair_conversion(x))
                 units_network.memory[(from_unit, to_unit)] = conversion, conversion_path
                 if value is None:
                     return units_network.memory[(from_unit, to_unit)]
                 else:
                     return conversion(value), conversion_path
 
+    # look for pair to pair conversion path
+    if ('/' in from_unit) and ('/' in to_unit) and len(from_unit.split('/')) == 2 and len(to_unit.split('/')) == 2:
+        # calculate the children and grandchildren of from_unit
+        from_unit_num, from_unit_den = from_unit.split('/')
+        # numerator children
+        from_unit_children_num = units_network.children_of(units_network.get_node(from_unit_num))
+        # numerator grandchildren
+        from_unit_grandchildren_num = [units_network.children_of(each)
+                                       for each in from_unit_children_num]
+        from_unit_grandchildren_num = [each
+                                       for grandchildren in from_unit_grandchildren_num
+                                       for each in grandchildren
+                                       if each not in from_unit_children_num]
+        # numerator grandgrandchildren
+        from_unit_grandgrandchildren_num = [units_network.children_of(each)
+                                       for each in from_unit_grandchildren_num]
+        from_unit_grandgrandchildren_num = [each
+                                            for grandchildren in from_unit_grandgrandchildren_num
+                                            for each in grandchildren
+                                            if each not in from_unit_children_num + from_unit_grandchildren_num]
+        # denominator children
+        from_unit_children_den = units_network.children_of(units_network.get_node(from_unit_den))
+        # denominator grandchildren
+        from_unit_grandchildren_den = [units_network.children_of(each)
+                                       for each in from_unit_children_den]
+        from_unit_grandchildren_den = [each
+                                       for grandchildren in from_unit_grandchildren_den
+                                       for each in grandchildren
+                                       if each not in from_unit_children_den]
+        # denominator grandgrandchildren
+        from_unit_grandgrandchildren_den = [units_network.children_of(each)
+                                            for each in from_unit_grandchildren_den]
+        from_unit_grandgrandchildren_den = [each
+                                            for grandchildren in from_unit_grandgrandchildren_den
+                                            for each in grandchildren
+                                            if each not in from_unit_children_den + from_unit_grandchildren_den]
+        
+        # get all the combinations of numerator/denominator
+        from_unit_children = sorted([f"{str(num)}/{str(den)}"
+                                     for num in set(from_unit_children_num)
+                                     for den in set(from_unit_children_den)],
+                                    key=len)
+        from_unit_grandchildren = sorted(list(set([f"{str(num)}/{str(den)}"
+                                                   for num in set(from_unit_children_num + from_unit_grandchildren_num)
+                                                   for den in set(from_unit_children_den + from_unit_grandchildren_den)
+                                                   if f"{str(num)}/{str(den)}" not in from_unit_children])),
+                                         key=len)  
+        from_unit_grandgrandchildren = sorted(list(set([f"{str(num)}/{str(den)}"
+                                                        for num in set(from_unit_children_num + from_unit_grandchildren_num + from_unit_grandgrandchildren_num)
+                                                        for den in set(from_unit_children_den + from_unit_grandchildren_den + from_unit_grandgrandchildren_den)
+                                                        if f"{str(num)}/{str(den)}" not in from_unit_children + from_unit_grandchildren])),
+                                              key=len) 
+
+        # calculate the children and grandchildren of to_unit
+        to_unit_num, to_unit_den = to_unit.split('/')
+        # numerator children
+        to_unit_children_num = units_network.children_of(units_network.get_node(to_unit_num))
+        # numerator grandchildren
+        to_unit_grandchildren_num = [units_network.children_of(each)
+                                     for each in to_unit_children_num]
+        to_unit_grandchildren_num = [each
+                                     for grandchildren in to_unit_grandchildren_num
+                                     for each in grandchildren
+                                     if each not in to_unit_children_num]
+        to_unit_grandgrandchildren_num = [units_network.children_of(each)
+                                          for each in to_unit_grandchildren_num]
+        to_unit_grandgrandchildren_num = [each
+                                          for grandchildren in to_unit_grandgrandchildren_num
+                                          for each in grandchildren
+                                          if each not in to_unit_children_num + to_unit_grandchildren_num]
+        # denominator children        
+        to_unit_children_den = units_network.children_of(units_network.get_node(to_unit_den))
+        # denominator grandchildren
+        to_unit_grandchildren_den = [units_network.children_of(each)
+                                     for each in to_unit_children_den]
+        to_unit_grandchildren_den = [each
+                                     for grandchildren in to_unit_grandchildren_den
+                                     for each in grandchildren
+                                     if each not in to_unit_children_den]
+        to_unit_grandgrandchildren_den = [units_network.children_of(each)
+                                          for each in to_unit_grandchildren_den]
+        to_unit_grandgrandchildren_den = [each
+                                          for grandchildren in to_unit_grandgrandchildren_den
+                                          for each in grandchildren
+                                          if each not in to_unit_children_den + to_unit_grandchildren_den]
+        # get all the combinations of numerator/denominator
+        to_unit_children = sorted([f"{str(num)}/{str(den)}"
+                                   for num in set(to_unit_children_num)
+                                   for den in set(to_unit_children_den)],
+                                  key=len)
+        to_unit_grandchildren = sorted(list(set([f"{str(num)}/{str(den)}"
+                                                 for num in set(to_unit_children_num + to_unit_grandchildren_num)
+                                                 for den in set(to_unit_children_den + to_unit_grandchildren_den)
+                                                 if f"{str(num)}/{str(den)}" not in to_unit_children])),
+                                       key=len)  
+        to_unit_grandgrandchildren = sorted(list(set([f"{str(num)}/{str(den)}"
+                                                      for num in set(to_unit_children_num + to_unit_grandchildren_num + to_unit_grandgrandchildren_num)
+                                                      for den in set(to_unit_children_den + to_unit_grandchildren_den + to_unit_grandgrandchildren_den)
+                                                      if f"{str(num)}/{str(den)}" not in to_unit_children + to_unit_grandchildren])),
+                                            key=len) 
+
+        from_family = [from_unit] + from_unit_children # + from_unit_grandchildren + from_unit_grandgrandchildren
+        to_family = [to_unit] + to_unit_children # + to_unit_grandchildren + to_unit_grandgrandchildren
+        for child_from in from_family:
+            for child_to in to_family:
+                child_conversion, child_conversion_path = _get_conversion(None, child_from, child_to, recursion=recursion)
+                # child_conversion, child_conversion_path = _converter(None, child_from, child_to, recursion=recursion)
+                if child_conversion is not None:
+                    break
+            if child_conversion is not None:
+                break
+
+        if child_conversion is not None:
+            if child_from != from_unit:
+                # base_conversion, base_conversion_path = _get_conversion(None, from_unit, child_from, recursion=recursion)
+                # if base_conversion is None:
+                base_conversion, base_conversion_path = _converter(None, from_unit, child_from, recursion=recursion)
+                if base_conversion is None:
+                    if unyts_parameters_.verbose_:
+                        logging.warning(f"<converter> failed to obtain base conversion {from_unit} {child_from}")
+                    return None, None
+                conversion_path = base_conversion_path + child_conversion_path
+                conversion_ = lambda x: child_conversion(base_conversion(x))
+            else:
+                conversion_, conversion_path = child_conversion, child_conversion_path
+            if child_to != to_unit:
+                # final_conversion, final_conversion_path = _get_conversion(None, child_to, to_unit, recursion=recursion)
+                # if final_conversion is None:
+                final_conversion, final_conversion_path = _converter(None, child_to, to_unit, recursion=recursion)
+                if final_conversion is None:
+                    if unyts_parameters_.verbose_:
+                        logging.warning(f"<converter> failed to obtain final conversion {child_to} {to_unit}")
+                    return None, None
+                conversion_path = conversion_path + final_conversion_path
+                conversion = lambda x: final_conversion(conversion_(x))
+            else:
+                conversion = conversion_
+            units_network.memory[(from_unit, to_unit)] = conversion, conversion_path
+            if value is None:
+                return units_network.memory[(from_unit, to_unit)]
+            else:
+                return conversion(value), conversion_path
+
     units_network.memory[(from_unit, to_unit)] = None, None
     return None, None
 
 
 def _clean_input(value: numeric, from_unit: str, to_unit: str_Empty) -> (numeric, str, str):
     """
     Helper function to preprocess the input parameters from the user
```

### Comparing `unyts-0.8.3/src/unyts/database.py` & `unyts-0.8.9/src/unyts/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 12:36:48 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.5.32'
-__release__ = 20240502
+__version__ = '0.5.33'
+__release__ = 20240521
 __all__ = ['units_network', 'network_to_frame', 'save_memory', 'load_memory', 'clean_memory', 'delete_cache']
 
 import logging
 import os
 
 from .dictionaries import SI, SI_order, OGF, OGF_order, DATA, DATA_order, dictionary, StandardAirDensity, \
     StandardEarthGravity
@@ -350,15 +350,15 @@
             pass
 
     # Percentage & fraction :
     network.add_edge(Conversion(network.get_node('fraction'), network.get_node('percentage'), lambda x: x * 100))
     network.add_edge(Conversion(network.get_node('percentage'), network.get_node('fraction'), lambda p: p / 100))
 
     # Time conversions
-    # network.addEdge(Conversion(network.getNode('second'), network.getNode('millisecond'), lambda t: t*1000))
+    network.add_edge(Conversion(network.get_node('second'), network.get_node('millisecond'), lambda t: t*1000))
     network.add_edge(Conversion(network.get_node('minute'), network.get_node('second'), lambda t: t * 60))
     network.add_edge(Conversion(network.get_node('hour'), network.get_node('minute'), lambda t: t * 60))
     network.add_edge(Conversion(network.get_node('day'), network.get_node('hour'), lambda t: t * 24))
     network.add_edge(Conversion(network.get_node('day'), network.get_node('month'), lambda t: t / 365.25 * 12))
     network.add_edge(Conversion(network.get_node('week'), network.get_node('day'), lambda t: t * 7))
     network.add_edge(Conversion(network.get_node('year'), network.get_node('month'), lambda t: t * 12))
     network.add_edge(Conversion(network.get_node('year'), network.get_node('day'), lambda t: t * 36525 / 100))
@@ -389,35 +389,37 @@
     network.add_edge(Conversion(network.get_node('mile'), network.get_node('furlong'), lambda d: d * 8))
     network.add_edge(Conversion(network.get_node('league'), network.get_node('mile'), lambda d: d * 3))
     network.add_edge(
         Conversion(network.get_node('nautical league'), network.get_node('nautical mile'), lambda d: d * 3))
     network.add_edge(Conversion(network.get_node('nautical mile'), network.get_node('meter'), lambda d: d * 1852))
     network.add_edge(Conversion(network.get_node('rod'), network.get_node('yard'), lambda d: d * 55 / 10))
 
+    # Velocity conversion
+    network.add_edge(Conversion(network.get_node('mile per hour'), network.get_node('kilometer per hour'),
+                                lambda v: v * 8 * 10 * 22 * 9144 / 10000 / 1000))
+
     # Area conversions
     network.add_edge(Conversion(network.get_node('square mile'), network.get_node('acre'), lambda d: d * 640))
     network.add_edge(Conversion(network.get_node('acre'), network.get_node('square yard'), lambda d: d * 4840))
     network.add_edge(
         Conversion(network.get_node('square rod'), network.get_node('square yard'), lambda d: d * 3025 / 100))
     network.add_edge(Conversion(network.get_node('square yard'), network.get_node('square foot'), lambda d: d * 9))
     network.add_edge(Conversion(network.get_node('square foot'), network.get_node('square inch'), lambda d: d * 144))
     network.add_edge(Conversion(network.get_node('square foot'), network.get_node('square meter'),
                                 lambda d: d * (3048 ** 2) / (10000 ** 2)))
-    # network.add_edge(Conversion(network.get_node('Darcy'), network.get_node('mD'), lambda d: d * 1000))
+    # network.addEdge(Conversion(network.getNode('foot'), network.getNode('meter'), lambda d: d*0.3048))
+    network.add_edge(Conversion(network.get_node('square inch'), network.get_node('square thou'), lambda d: d * (1000 ** 2)))
+    network.add_edge(Conversion(network.get_node('square inch'), network.get_node('square tenth'), lambda d: d * (10 ** 2)))
+    network.add_edge(Conversion(network.get_node('square chain'), network.get_node('square yard'), lambda d: d * (22 ** 2)))
+    network.add_edge(Conversion(network.get_node('square furlong'), network.get_node('square chain'), lambda d: d * (10 ** 2)))
+    network.add_edge(Conversion(network.get_node('square mile'), network.get_node('square furlong'), lambda d: d * (8 ** 2)))
+    network.add_edge(Conversion(network.get_node('square league'), network.get_node('square mile'), lambda d: d * (3 ** 2)))
+
     network.add_edge(Conversion(network.get_node('Darcy'), network.get_node('µm2'), lambda d: d * 0.9869233))
-    # network.addEdge(Conversion(network.getNode('m*m'), network.getNode('m'), lambda d: d**0.5))
-    # network.addEdge(Conversion(network.getNode('m'), network.getNode('m*m'), lambda d: d**2))
-    # network.addEdge(Conversion(network.getNode('rd*rd'), network.getNode('rd'), lambda d: d**0.5))
-    # network.addEdge(Conversion(network.getNode('rd'), network.getNode('rd*rd'), lambda d: d**2))
-    # network.addEdge(Conversion(network.getNode('yd*yd'), network.getNode('yd'), lambda d: d**0.5))
-    # network.addEdge(Conversion(network.getNode('yd'), network.getNode('yd*yd'), lambda d: d**2))
-    # network.addEdge(Conversion(network.getNode('ft*ft'), network.getNode('ft'), lambda d: d**0.5))
-    # network.addEdge(Conversion(network.getNode('ft'), network.getNode('ft*ft'), lambda d: d**2))
-    # network.addEdge(Conversion(network.getNode('in*in'), network.getNode('in'), lambda d: d**0.5))
-    # network.addEdge(Conversion(network.getNode('in'), network.getNode('in*in'), lambda d: d**2))
+
 
     # Volume conversions
     network.add_edge(Conversion(network.get_node('gill'), network.get_node('fluid ounce'), lambda v: v * 4))
     network.add_edge(Conversion(network.get_node('pint'), network.get_node('gill'), lambda v: v * 4))
     network.add_edge(Conversion(network.get_node('quart'), network.get_node('pint'), lambda v: v * 2))
     network.add_edge(Conversion(network.get_node('gallonUS'), network.get_node('fluid ounce'), lambda v: v * 128))
     network.add_edge(Conversion(network.get_node('gallonUS'), network.get_node('quart'), lambda v: v * 4))
@@ -444,14 +446,23 @@
                    lambda v: v * 5.614584))
     network.add_edge(Conversion(network.get_node('reservoir cubic meter'), network.get_node('reservoir barrel'),
                                 lambda v: v * 6.289814))
     network.add_edge(Conversion(network.get_node('reservoir cubic meter'), network.get_node('standard cubic meter'),
                                 lambda v: v / network.get_fvf()))
     # network.addEdge(Conversion(network.getNode('standard cubic meter'), network.getNode('standard cubic foot'), lambda v: v/5.614584))
 
+    network.add_edge(Conversion(network.get_node('cubic inch'), network.get_node('cubic thou'), lambda d: d * (1000 ** 3)))
+    network.add_edge(Conversion(network.get_node('cubic inch'), network.get_node('cubic tenth'), lambda d: d * (10 ** 3)))
+    network.add_edge(Conversion(network.get_node('cubic foot'), network.get_node('cubic inch'), lambda d: d * (12 ** 3)))
+    network.add_edge(Conversion(network.get_node('cubic yard'), network.get_node('cubic foot'), lambda d: d * (3 ** 3)))
+    network.add_edge(Conversion(network.get_node('cubic chain'), network.get_node('cubic yard'), lambda d: d * (22 ** 3)))
+    network.add_edge(Conversion(network.get_node('cubic furlong'), network.get_node('cubic chain'), lambda d: d * (10 ** 3)))
+    network.add_edge(Conversion(network.get_node('cubic mile'), network.get_node('cubic furlong'), lambda d: d * (8 ** 3)))
+    network.add_edge(Conversion(network.get_node('cubic league'), network.get_node('cubic mile'), lambda d: d * (3 ** 3)))
+
     # Pressure conversions
     network.add_edge(Conversion(network.get_node('psi gauge'), network.get_node('absolute psi'), lambda p: p + 14.6959))
     network.add_edge(Conversion(network.get_node('absolute psi'), network.get_node('psi gauge'), lambda p: p - 14.6959))
     network.add_edge(Conversion(network.get_node('bar gauge'), network.get_node('absolute bar'), lambda p: p + 1.01325))
     network.add_edge(Conversion(network.get_node('absolute bar'), network.get_node('bar gauge'), lambda p: p - 1.01325))
 
     network.add_edge(
@@ -465,15 +476,15 @@
     network.add_edge(Conversion(network.get_node('atmosphere'), network.get_node('Pascal'), lambda p: p * 101325))
     network.add_edge(Conversion(network.get_node('atmosphere'), network.get_node('Torr'), lambda p: p * 760))
     network.add_edge(Conversion(network.get_node('absolute bar'), network.get_node('bar'), lambda p: p))
     network.add_edge(Conversion(network.get_node('absolute psi'), network.get_node('psi'), lambda p: p))
     network.add_edge(Conversion(network.get_node('bar gauge'), network.get_node('bar'), lambda p: p))
     network.add_edge(Conversion(network.get_node('psi gauge'), network.get_node('psi'), lambda p: p))
 
-    # mass Conversion
+    # Mass conversion
     network.add_edge(Conversion(network.get_node('grain'), network.get_node('milligrams'), lambda w: w * 64.7989))
     network.add_edge(Conversion(network.get_node('pennyweight'), network.get_node('grain'), lambda w: w * 24))
     network.add_edge(Conversion(network.get_node('dram'), network.get_node('pound'), lambda w: w / 256))
     network.add_edge(Conversion(network.get_node('stone'), network.get_node('pound'), lambda w: w * 14))
     network.add_edge(Conversion(network.get_node('quarter'), network.get_node('stone'), lambda w: w * 2))
     network.add_edge(Conversion(network.get_node('weight ounce'), network.get_node('dram'), lambda w: w * 16))
     network.add_edge(Conversion(network.get_node('pound'), network.get_node('weight ounce'), lambda w: w * 16))
@@ -485,15 +496,15 @@
 
     network.add_edge(Conversion(network.get_node('metric ton'), network.get_node('kilogram'), lambda w: w * 1000))
     network.add_edge(Conversion(network.get_node('kilogram'), network.get_node('gram'), lambda w: w * 1000))
     # network.addEdge(Conversion(network.getNode('pound'), network.getNode('gram'), lambda w: w*453.59237))
     network.add_edge(
         Conversion(network.get_node('pound'), network.get_node('kilogram'), lambda w: w * 45359237 / 100000000))
 
-    # force Conversion
+    # Force conversion
     # network.addEdge(Conversion(network.getNode('kilogram'), network.getNode('kilogram force'), lambda f: f* converter(StandardEarthGravity,'m/s2','cm/s2',False)))
     network.add_edge(Conversion(network.get_node('kilogram mass'), network.get_node('kilogram force'),
                                 lambda f: f * StandardEarthGravity))
     network.add_edge(Conversion(network.get_node('kilogram force'), network.get_node('kilogram mass'),
                                 lambda f: f / StandardEarthGravity))
     network.add_edge(Conversion(network.get_node('Dyne'), network.get_node('Newton'), lambda f: f * 1E-5))
     network.add_edge(Conversion(network.get_node('Newton'), network.get_node('Dyne'), lambda f: f * 1E5))
@@ -501,34 +512,35 @@
     # Energy Conversion
     network.add_edge(Conversion(network.get_node('Joule'), network.get_node('gram calorie'), lambda e: e / 4.184))
     network.add_edge(Conversion(network.get_node('Kilojoule'), network.get_node('Joule'), lambda e: e * 1000))
     network.add_edge(Conversion(network.get_node('Kilojoule'), network.get_node('kilowatt hour'), lambda e: e / 3600))
     network.add_edge(
         Conversion(network.get_node('Kilojoule'), network.get_node('British thermal unit'), lambda e: e / 1.055))
 
-    # Power Conversion
+    # Power conversion
     network.add_edge(Conversion(network.get_node('Horsepower'), network.get_node('Watt'), lambda e: e * 745.699872))
 
-    # Density Conversion
+    # Density conversion
     network.add_edge(Conversion(network.get_node('API'), network.get_node('SgO'), lambda d: 141.5 / (131.5 + d)))
     network.add_edge(Conversion(network.get_node('SgO'), network.get_node('API'), lambda d: 141.5 / d - 131.5))
     network.add_edge(Conversion(network.get_node('API'), network.get_node('g/cc'), lambda d: 141.5 / (131.5 + d)))
     network.add_edge(Conversion(network.get_node('g/cc'), network.get_node('API'), lambda d: 141.5 / d - 131.5))
     network.add_edge(Conversion(network.get_node('SgO'), network.get_node('g/cc'), lambda d: d))
     network.add_edge(Conversion(network.get_node('SgW'), network.get_node('g/cc'), lambda d: d))
     network.add_edge(Conversion(network.get_node('SgG'), network.get_node('kg/m3'), lambda d: d * StandardAirDensity))
     network.add_edge(Conversion(network.get_node('psia/ft'), network.get_node('lb/ft3'), lambda d: d * 144))
+    network.add_edge(Conversion(network.get_node('bara/m'), network.get_node('kg/m3'), lambda d: d * 100000))
     network.add_edge(
         Conversion(network.get_node('g/cm3'), network.get_node('lb/ft3'), lambda d: d * 62.427960576144606))
     network.add_edge(Conversion(network.get_node('lb/ft3'), network.get_node('lb/stb'), lambda d: d * 5.614584))
 
-    # viscosity conversions
+    # Viscosity conversions
     network.add_edge(Conversion(network.get_node('Pa*s'), network.get_node('Poise'), lambda v: v * 10))
 
-    # data conversions
+    # Data conversions
     network.add_edge(Conversion(network.get_node('byte'), network.get_node('bit'), lambda d: d * 8))
 
     for unit_kind in list(dictionary.keys()):
         if '_REVERSE' in unit_kind:
             if type(dictionary[unit_kind]) is dict:
                 nameList = list(dictionary[unit_kind].keys())
             else:
```

### Comparing `unyts-0.8.3/src/unyts/dictionaries.py` & `unyts-0.8.9/src/unyts/dictionaries.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 12:14:51 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.5.31'
-__release__ = 20240502
+__version__ = '0.5.42'
+__release__ = 20240521
 __all__ = ['dictionary', 'SI', 'OGF', 'DATA', 'StandardAirDensity', 'StandardEarthGravity', 'unitless_names',
            'uncertain_names']
 
 import logging
 from json import load as json_load
 from pickle import load as pickle_load, dump as pickle_dump
 from os.path import isfile
@@ -44,15 +44,16 @@
     'p': (lambda X: X * 1E-12, lambda X: X * 1E-24, lambda X: X * 1E-36),  # pico
     'f': (lambda X: X * 1E-15, lambda X: X * 1E-30, lambda X: X * 1E-45),  # femto
     'a': (lambda X: X * 1E-18, lambda X: X * 1E-36, lambda X: X * 1E-54),  # atto
     'z': (lambda X: X * 1E-21, lambda X: X * 1E-42, lambda X: X * 1E-63),  # zepto
     'y': (lambda X: X * 1E-24, lambda X: X * 1E-48, lambda X: X * 1E-72),  # yocto
 }
 
-SI_order = (('Length', 'Pressure', 'Weight', 'Mass', 'Time', 'Frequency', 'Power', 'Voltage', 'Current', 'Resistance',),
+SI_order = (('Length', 'Pressure', 'Weight', 'Mass', 'Time', 'Frequency', 'Power', 'Voltage', 'Current', 'Resistance',
+             'Impedance', 'Conductance', 'Capacitance', 'Charge', 'Inductance', 'Energy', 'Permeability'),
             ('Area',),
             ('Rate', 'Volume',),)
 
 DATA = {
     'Y': (lambda X: X * 1E+24, lambda X: X * 2 ** 80),  # yotta
     'Z': (lambda X: X * 1E+21, lambda X: X * 2 ** 70),  # zetta
     'E': (lambda X: X * 1E+18, lambda X: X * 2 ** 60),  # exa
@@ -140,47 +141,57 @@
         'quartUK': ('qtUK', 'UKquart'),
     }
     dictionary['Volume_NAMES_SPACES_REVERSE'] = {
         'litre': ('l', 'liter', 'litro'),
         'millilitre': ('ml', 'milliliter', 'cubic centimeter'),
         'centilitre': ('cl', 'centiliter'),
         'decilitre': ('dl', 'deciliter'),
-        'cubic meter': ('CM', 'm3'),
-        'standard cubic meter': ('scm', 'sm3', 'stm3', 'm3', 'Sm3'),
-        'cubic centimeter': ('cc', 'cm3', 'standard cubic centimeter'),
-        'standard cubic centimeter': ('scc', 'scm3'),
-        'reservoir cubic meter': ('rm3', 'Rm3'),
-        'reservoir cubic centimeter': ('rcc', 'rcm3'),
-        'cubic foot': ('cubic feet', 'ft3', 'cf', 'pie cúbico', 'pie cubico', 'pc', 'pies cúbicos', 'pies cubicos'),
+        'cubic meter': ('CM', 'm3', 'm³'),
+        'standard cubic meter': ('scm', 'sm3', 'stm3', 'm3', 'Sm3', 'sm³'),
+        'cubic centimeter': ('cc', 'cm3', 'standard cubic centimeter', 'cm³'),
+        'standard cubic centimeter': ('scc', 'scm3', 'scm³'),
+        'reservoir cubic meter': ('rm3', 'Rm3', 'rm³'),
+        'reservoir cubic centimeter': ('rcc', 'rcm3', 'rcm³'),
+        'cubic thou': ('th3', 'th2*th', 'th*th2', 'th³'),
+        'cubic tenth': ('te3', 'te2*te', 'te*te2', 'te³'),
+        'cubic inch': ('cubic inches', 'in3', 'in2*in', 'in*in2', 'in³'),
+        'cubic foot': ('cubic feet', 'ft3', 'ft³', 'cf', 'ft2*ft', 'ft*ft2',
+                       'pie cúbico', 'pie cubico', 'pc', 'pies cúbicos', 'pies cubicos',),
+        'cubic yard': ('yd3', 'yd³', 'yd2*yd' 'yd*yd2'),
+        'cubic chain': ('ch3', 'ch³', 'ch2*ch', 'ch*ch2'),
+        'cubic rod': ('rd3', 'rd³', 'rd2*rd', 'rd*rd2'),
+        'cubic furlong': ('fur3', 'fur³', 'fur2*fur', 'fur*fur2'),
+        'cubic mile': ('mi3', 'mi³', 'mi2*mi', 'mi*mi2'),
+        'cubic league': ('lea3', 'lea³', 'lea2*lea', 'lea*lea2'),
         'standard cubic foot': ('scf', 'cf'),
-        'cubic inch': ('in3', 'cubic inches'),
         'barrel': ('bbl', 'stb', 'oil barrel'),
         'reservoir barrel': ('rb',),
         'standard barrel': ('stb', 'stbo', 'stbw', 'stbl', 'oil barrel'),
     }
-    dictionary['Volume_UPPER'] = ('sm3', 'rm3', 'kstm3', 'Mstm3')
+    dictionary['Volume_UPPER'] = ('sm3', 'sm³', 'rm3', 'rm³', 'kstm3', 'kstm³', 'Mstm3', 'Mstm³')
     dictionary['Volume_PLURALwS_UPPER_LOWER'] = tuple(dictionary['Volume_NAMES_SPACES_REVERSE'].keys()) + \
                                                 tuple(dictionary['Volume_UK_NAMES_REVERSE'].keys()) + \
                                                 ('fl oz', 'oz', 'ounce', 'gallon', 'imperial gallon', 'barrel', 'gal',
                                                  'oil barrel', 'oil gallon',
                                                  'USgallon', 'UKgallon', 'USounce', 'UKounce',
                                                  'cubic centimeter', 'standard cubic centimeter',
                                                  'liter', 'milliliter', 'centiliter', 'deciliter')
-    dictionary['Volume_OGF'] = ('scf', 'cf', 'ft3', 'stb', 'bbl', 'rb', 'stbo', 'stbw', 'stbl')
+    dictionary['Volume_OGF'] = ('scf', 'cf', 'ft3', 'ft³', 'stb', 'bbl', 'rb', 'stbo', 'stbw', 'stbl')
     # dictionary['Volume_oilgas_NAMES'] = ('scf','cf','ft3','stb','bbl','rb','stbo','stbw','stbl')
     dictionary['Volume_oilgas_UPPER'] = ('sm3', 'Sm3', 'm3', 'rm3', 'Rm3', 'ksm3', 'Msm3', 'Gsm3',
                                          'scf', 'cf', 'ft3', 'Mscf', 'MMscf', 'Bscf', 'Tscf', 'Mcf', 'MMcf', 'Bcf',
                                          'Tcf',
                                          'stb', 'bbl', 'rb', 'Mstb', 'MMstb', 'Bstb', 'Tstb', 'Mbbl', 'MMbbl', 'Mrb',
                                          'MMrb')
     dictionary['Volume_product_NAMES_REVERSE'] = {
-        'm3': ('m2*m',),
-        'cm3': ('cm2*cm',),
-        'ft3': ('ft2*ft',),
-        'in3': ('in2*in',)
+        'm3': ('m³', 'm2*m', 'm*m2', 'm²*m', 'm*m²'),
+        'cm3': ('cm³', 'cm2*cm', 'cm*cm2', 'cm²*cm', 'cm*cm²'),
+        'yd3': ('yd³', 'yd2*yd', 'yd*yd2', 'yd²*yd', 'yd*yd²'),
+        'ft3': ('ft³', 'ft2*ft', 'ft*ft2', 'ft²ft', 'ft*ft²'),
+        'in3': ('in³', 'in2*in', 'in*in2', 'in²*in', 'in*in²'),
     }
     dictionary['Volume_linearSI'] = ('sm3', 'rm3',)
 
     # Length
     dictionary['Length'] = []
     dictionary['Length_NAMES_REVERSE_UPPER'] = {'meter': ('m', 'meter', 'metro')}
     dictionary['Length_SI'] = ('m', 'l',)  # litre, sm3 and rm3 are Volume but the conversion of SI prefixes is linear
@@ -195,81 +206,89 @@
         'furlong': ('fur',),
         'mile': ('mi',),
         'league': ('lea',),
         'nautical mile': ('nmi',),
         'nautical league': ('nlea',),
     }
     dictionary['Length_UK_UPPER'] = tuple(dictionary['Length_UK_NAMES_REVERSE'].keys()) + \
-                                    ('feet', 'in', 'ft', 'yd', '0.1 in', '0.1in', '.1in')
+                                    ('feet', 'in', 'ft', '0.1 in', '0.1in', '.1in')  # 'yd' uppercase is confused with yottaDarcy
 
     # Area
     dictionary['Area'] = []
-    dictionary['Area_NAMES_REVERSE_UPPER'] = {'square meter': ('sq m', 'm2', 'sqmeter', 'm*m', 'm3/m')}
-    dictionary['Area_SI'] = ('m2',)
+    dictionary['Area_NAMES_REVERSE_UPPER'] = {'square meter': ('sq m', 'm2', 'm²', 'sqmeter', 'm*m', 'm3/m')}
+    dictionary['Area_SI'] = ('m2', 'm²',)
     dictionary['Area_UK_NAMES_REVERSE_UPPER'] = {
-        'square mile': ('sq mi', 'mi2', 'sqmile', 'mi*mi'),
         'acre': tuple(),
-        'square rod': ('sq rd', 'sqrd', 'rd2', 'rd*rd'),
-        'square yard': ('sq yd', 'sqyd', 'yd2', 'yd*yd'),
-        'square foot': ('sq ft', 'sqft', 'ft2', 'ft*ft', 'ft3/ft'),
-        'square inch': ('sq in', 'sqin', 'in2', 'in*in', 'in3/in')
+        'square thou': ('sq th', 'sqth', 'th2', 'th²', 'th*th', 'th3/th'),
+        'square tenth': ('sq te', 'sqte', 'te2', 'te²', 'te*te', 'te3/te'),
+        'square inch': ('sq in', 'sqin', 'in2', 'in²', 'in*in', 'in3/in'),
+        'square foot': ('sq ft', 'sqft', 'ft2', 'ft²', 'ft*ft', 'ft3/ft'),
+        'square yard': ('sq yd', 'sqyd', 'yd2', 'yd²', 'yd*yd', 'yd3/yd'),
+        'square chain': ('sq ch', 'sqch', 'ch2', 'ch²', 'ch*ch', 'ch3/ch'),
+        'square rod': ('sq rd', 'sqrd', 'rd2', 'rd²', 'rd*rd', 'rd3/rd'),
+        'square furlong': ('sq fur', 'sqfur', 'fur2', 'fur²', 'fur*fur', 'fur3/fur'),
+        'square mile': ('sq mi', 'mi2', 'mi²', 'sqmile', 'mi*mi', 'mi3/mi'),
+        'square league': ('sq lea', 'sqlea', 'lea2', 'lea²', 'lea*lea', 'lea3/lea'),
     }
 
     # Pressure
     dictionary['Pressure'] = []
     dictionary['Pressure_NAMES_REVERSE_SPACES'] = {
         'Pascal': ('Pa',),
     }
     dictionary['Pressure_NAMES_REVERSE_UPPER_SPACES'] = {
         'absolute psi': ('psia', 'lb/in2', 'absolute pound/square inch', 'psi absolute',
-                         'libras/pulgada cuadrada absoluta', 'lpca'),
-        'psi gauge': ('psi', 'pound/square inch', 'psig', 'gauge psi'),
+                         'lpca', 'libras/pulgada cuadrada absoluta'),
+        'psi gauge': ('psi', 'pound/square inch', 'psig', 'gauge psi', 'lpc', 'lpcm', 'libras/pulgada cuadrada'),
         'absolute bar': ('bara', 'barsa', 'abs bar', 'bar absolute'),
         'bar gauge': ('bar', 'barg', 'gauge bar', 'bars'),
         'atmosphere': ('atm', 'atma'),
         'Pascal': ('Newton/m2',),
         'kPa': ('KPa', 'kilopascal'),
         'hPa': ('hectopascal',),
         'Torr': ('millimeters of mercury',),
         'millimeters of mercury': ('mmHg',),
     }
     dictionary['Pressure_SI'] = ('Pa', 'bara', 'barsa', 'bar', 'barg')
 
     dictionary['PressureGradient'] = []
-    dictionary['PressureGradient'] = ('psi/ft', 'psia/ft', 'psig/ft', 'psi/m', 'psia/m', 'psig/m', 'bar/m', 'bars/m',
-                                      'barsa/m', 'bara/m', 'barg/m')
+    dictionary['PressureGradient'] = ('psi/ft', 'psia/ft', 'psig/ft',
+                                      'psi/m', 'psia/m', 'psig/m',
+                                      'bar/m', 'bars/m', 'barsa/m', 'bara/m', 'barg/m',
+                                      'bar/ft', 'bars/ft', 'barsa/ft', 'bara/ft', 'barg/ft')
 
     # Weight
     dictionary['Weight'] = []
     dictionary['Weight_NAMES_REVERSE'] = {
         'gram': ('g',),
         'kilogram': ('kg',),
         'milligram': ('mg',),
+        'microgram': ('ug', 'µg'),
         'metric ton': ('Tonne',),
         'g-mol': ('g-moles',),
         'Kg-mol': ('Kg-moles',),
     }
     dictionary['Weight_UK_NAMES_REVERSE'] = {
         'grain': ('gr',),
         'pennyweight': ('pwt', 'dwt'),
         'dram': ('dr', 'dramch'),
         'ounce': ('oz', 'wt oz', 'weight ounce'),
-        'pound': ('lb', '#', 'libra'),
+        'pound': ('lb', '#', 'libra',),
         'stone': ('st',),
         'quarter': ('qr', 'qrt'),
         # 'hundredweight' : ('cwt',),
         'short hundredweight': ('US hundredweight', 'UScwt', 'swtUS'),
         'long hundredweight': ('UK hundredweight', 'UKcwt', 'cwt', 'swtUK'),
         # 'ton' : ('t',),
         'short ton': ('USton', 'tonUS'),
-        'long ton': ('t', 'UKton', 'ton', 'tonUK'),
+        'long ton': ('t', 'UKton', 'ton', 'tonUK', 'Ton'),
     }
     dictionary['Weight_PLURALwS_UPPER_LOWER_SPACES'] = tuple(dictionary['Weight_NAMES_REVERSE'].keys()) + \
                                                        tuple(dictionary['Weight_UK_NAMES_REVERSE'].keys()) + \
-                                                       ('Tonne', 'ton', 'UKton', 'USton')
+                                                       ('Tonne', 'ton', 'UKton', 'USton', 'lb', 'libra')
     dictionary['Weight_SI'] = ('g', 'g-mol')
 
     # Mass
     dictionary['Mass'] = ['kilogram mass']
     dictionary['Mass_NAMES_REVERSE_UPPER_LOWER'] = {
         'kilogram mass': ('Kgm', 'kilogram mass')
     }
@@ -280,22 +299,25 @@
     dictionary['Density_NAMES_REVERSE_LOWER_UPPER'] = {
         'API': ('degrees',),
         'SgG': ('gas gravity', 'gas specific gravity', 'sgg'),
         'SgW': ('water gravity', 'sgw'),
         'SgO': ('oil gravity', 'sgo'),
     }
     dictionary['Density_NAMES_REVERSE_UPPER'] = {
-        'g/cm3': ('g/cc',),
-        'kg/m3': ('Kg/m3',),
+        'g/cm3': ('g/cc', 'g/cm³',),
+        'kg/m3': ('Kg/m3', 'kg/m³'),
         'lb/ft3': tuple(),
+        'lb/yd3': tuple(),
         'psi/ft': tuple(),
-        'kJ/rm3': ('KJ/rm3',),
+        'kJ/rm3': ('KJ/rm3', 'kJ/rm³'),
+        'kJ/sm3': ('KJ/sm3', 'kJ/sm³'),
+        'kJ/m3': ('KJ/m3', 'kJ/m³'),
         'lb/stb': tuple(),
-        'psia/ft': ('psi/ft',),
-        'bara/m': ('bar/m',),
+        'psia/ft': ('psi/ft', 'psig/ft'),
+        'bara/m': ('bar/m', 'barg/m'),
     }
 
     # Compressibility
     dictionary['Compressibility'] = []
     dictionary['Compressibility_UPPER_NAMES_REVERSE'] = {
         '1/psi': ('1/psia', 'µsip', 'usip', '1/psig'),
         'µsip': ('usip',),
@@ -307,26 +329,34 @@
     dictionary['Rate_NAMES_REVERSE_UPPER_SPACES'] = {
         'standard barrel per day': ('stb/day',),
         'standard cubic foot per day': ('scf/day', 'cf/day', 'scfd'),
         'standard cubic meter per day': ('sm3/day',),
         'barrel per day': ('bbl/day',),
         'cubic meter per day': ('m3/day',),
         'cubic foot per day': ('ft3/day',),
+        'cubic yard per day': ('yd3/day',),
         'reservoir barrel per day': ('rb/day',),
         'reservoir cubic meter per day': ('rm3/day',),
     }
     dictionary['Rate_NAMES_REVERSE_UPPER_SPACES'] = {
         'stb/day': ('stbd',),
         'scf/day': ('scfd', 'cf/day',),
-        'sm3/day': ('sm3d', 'stm3d', 'stm3/day'),
+        'sm3/day': ('sm3d', 'stm3d', 'stm3/day', 'sm³/day'),
         'bbl/day': ('bbld',),
-        'm3/day': ('m3/d',),
+        'm3/day': ('m3/d', 'm³/day'),
         'ft3/day': ('cf/day',),
     }
 
+    # Velocity
+    dictionary['Velocity'] = ['kilometer per hour', 'mile per hour',]
+    dictionary['Velocity_NAMES_REVERSE_UPPER_LOWER'] = {
+        'kilometer per hour': ('kilometers per hour', 'kph', 'KPH', 'km/hr'),
+        'mile per hour': ('miles per hour', 'mph', 'MPH', 'mi/hr'),
+    }
+
     # digital Data
     # dictionary['Data'] = []
     dictionary['dataBYTE'] = []
     dictionary['dataBYTE_NAMES_REVERSE'] = {'byte': ('B', 'Byte', 'BYTE')}
     dictionary['dataBYTE_DATA'] = ('B', 'byte')
     dictionary['dataBIT'] = []
     dictionary['dataBIT_NAMES_REVERSE'] = {'bit': ('b', 'Bit', 'BIT')}
@@ -343,15 +373,15 @@
     # Permeability
     dictionary['Permeability'] = []
     dictionary['Permeability_NAMES_REVERSE'] = {
         'Darcy': ('D',),
         'millidarcy': ('mD',)
     }
     dictionary['Permeability_UPPER_LOWER'] = ('Darcy', 'millidarcy')
-    dictionary['Energy_SI'] = ('D',)
+    dictionary['Permeability_SI'] = ('D',)
 
     # Force
     dictionary['Force'] = []
     dictionary['Force_NAMES_REVERSE_SPACES_RECURSIVE_UPPER'] = {
         'Newton': ('N', 'newton', 'kg*m/s2'),
         'kilogram force': ('kgf', 'kilopondio',),  # 'kilogram'
         'kilopondio': ('kp',),
```

### Comparing `unyts-0.8.3/src/unyts/errors.py` & `unyts-0.8.9/src/unyts/errors.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/gui.py` & `unyts-0.8.9/src/unyts/gui.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Feb 11 10:38:47 2024
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.2.1'
-__release__ = 20240502
+__version__ = '0.3.5'
+__release__ = 20240521
 __all__ = ['start_gui']
 
 import logging
 import tkinter as tk
 from tkinter import ttk
 from stringthings import get_number, is_numeric
+from unyts import __version__ as unyts_version
 from .converter import convert
 from .dictionaries import _all_units
 from .errors import NoConversionFoundError
-from .database import save_memory, load_memory, clean_memory, delete_cache, unyts_parameters_, set_fvf
+from .database import save_memory, load_memory, clean_memory, delete_cache, unyts_parameters_ as up_, set_fvf
 import pathlib, os
+import webbrowser
 
 
 _all_units_str = _all_units()
 
 
 class UnytsApp(tk.Frame):
 
@@ -75,91 +77,130 @@
     def _validate_to_units(self, *args):
         if self.to_unit_val.get() not in _all_units_str and not is_numeric(self.to_unit_val.get()):
             return False
         else:
             return True
 
     def _get_from(self):
-        try:
-            from_value = get_number(self.from_value_val.get())
-            from_unit = self.from_unit_val.get()
-        except ValueError:
-            try:
-                from_value = get_number(self.from_unit_val.get())
-                from_unit = self.from_value_val.get()
-            except ValueError:
-                from_value = self.from_value_val.get()
-                from_unit = self.from_unit_val.get()
-                self.from_value_val.set(f"wrong number format")
-                self.from_unit_val.set(from_unit)
-                return None
+        from_value = self.from_value_val.get().strip()
+        from_unit = self.from_unit_val.get().strip()
+        if len(from_value) == 0 and len(from_unit) > 0 and not is_numeric(from_unit):
+            pass  # is OK
+        elif len(from_unit) == 0 and len(from_value) > 0 and not is_numeric(from_value):
+            from_value, from_unit = from_unit, from_value
+        elif is_numeric(from_value) and not is_numeric(from_unit):
+            from_value = get_number(from_value)
+        elif not is_numeric(from_value) and is_numeric(from_unit):
+            from_value, from_unit = get_number(from_unit), from_value
+        elif not is_numeric(from_value) and not is_numeric(from_unit):
+            self.from_value_val.set(f"wrong number format")
+            from_value, from_unit = None, None
+        self.from_unit_val.set(from_unit)
+        self.from_value_val.set(from_value)
         return from_unit, from_value
 
     def _get_to(self):
-        try:
-            to_value = get_number(self.to_value_val.get())
-            to_unit = self.to_unit_val.get()
-        except ValueError:
-            try:
-                to_value = get_number(self.to_unit_val.get())
-                to_unit = self.to_value_val.get()
-            except ValueError:
-                to_value = self.to_value_val.get()
-                to_unit = self.to_unit_val.get()
-                self.to_value_val.set(f"wrong number format")
-                self.to_unit_val.set(to_unit)
-                return None, None
+        to_value = self.to_value_val.get().strip()
+        to_unit = self.to_unit_val.get().strip()
+        if len(to_value) == 0 and len(to_unit) > 0 and not is_numeric(to_unit):
+            pass  # is OK
+        elif len(to_unit) == 0 and len(to_value) > 0 and not is_numeric(to_value):
+            to_value, to_unit = to_unit, to_value
+        elif is_numeric(to_value) and not is_numeric(to_unit):
+            to_value = get_number(to_value)
+        elif not is_numeric(to_value) and is_numeric(to_unit):
+            to_value, to_unit = get_number(to_unit), to_value
+        elif not is_numeric(to_value) and not is_numeric(to_unit):
+            self.to_value_val.set(f"wrong number format")
+            to_value, to_unit = None, None
+        self.to_unit_val.set(to_unit)
+        self.to_value_val.set(to_value)
         return to_unit, to_value
 
     def _calculate(self, *args):
+        self.button_text.set("looking for conversion...")
         from_unit, from_value = self._get_from()
-        to_unit = self.to_unit_val.get()
-        self.to_value_val.set("")
+        to_unit, to_value = self._get_to()
+        if from_unit is None and from_value is None and to_unit is None and to_value is None:
+            self.from_value_val.set("")
+            self.from_unit_val.set("")
+            self.to_value_val.set("")
+            self.to_unit_val.set("")
+            self.button_text.set("convert")
+            return None
+        if from_value == "" and is_numeric(to_value):
+            return self._rcalculate()
         try:
             to_value = convert(from_value, from_unit, to_unit,
-                               print_conversion_path=False)
+                               print_conversion_path=up_.print_path_)
             self.to_value_val.set(str(to_value))
         except NoConversionFoundError:
+            self.to_value_val.set("")
             self.button_text.set("no conversion found!")
+            return None
+        self.button_text.set("convert")
 
     def _rcalculate(self, *args):
+        self.button_text.set("looking for conversion...")
         from_unit, from_value = self._get_to()
-        to_unit = self.from_unit_val.get()
-        self.from_value_val.set("")
+        to_unit, to_value = self._get_from()
+        if from_unit is None and from_value is None and to_unit is None and to_value is None:
+            self.from_value_val.set("")
+            self.from_unit_val.set("")
+            self.to_value_val.set("")
+            self.to_unit_val.set("")
+            self.button_text.set("convert")
+            return None
+        if from_value == "" and is_numeric(to_value):
+            return self._calculate()
         try:
             to_value = convert(from_value, from_unit, to_unit,
-                               print_conversion_path=False)
+                               print_conversion_path=up_.print_path_)
             self.from_value_val.set(str(to_value))
         except NoConversionFoundError:
+            self.from_value_val.set("")
             self.button_text.set("no conversion found!")
+            return None
+        self.button_text.set("convert")
 
 
 def start_gui():
     def close_gui():
-        logging.info("saving memory...")
-        save_memory()
         logging.info("INFO:shutting down Unyts.")
+        if up_.cache_:
+            logging.info("saving memory...")
+            save_memory()
         root.destroy()
-    if unyts_parameters_.memory_:
+    if up_.memory_:
         load_memory()
     else:
         delete_cache()
+    def open_help():
+        webbrowser.open('https://github.com/ayaranitram/unyts/blob/master/unyts_demo.ipynb')
+    def open_git():
+        webbrowser.open('https://github.com/ayaranitram/unyts')
 
     logging.info("starting Unyts GUI...")
     w, h = 325, 185
     root = tk.Tk(screenName='Unyts')
     root.geometry(f"{w}x{h}")
     root.maxsize(w, h)
     root.minsize(w, h)
     root.resizable(False, False)
     icon_file = 'unyts_icon.ico'
     current_dir = pathlib.Path(__file__).parent.resolve()
     icon_path = os.path.join(current_dir, icon_file)
     root.iconbitmap(icon_path)
 
+    # variables
+    _cache_ = tk.BooleanVar()
+    _cache_.set(up_.cache_)
+    _print_path_ = tk.BooleanVar()
+    _print_path_.set(up_.print_path_)
+
     # setting menu
     root.option_add('*tearOff', False)
     unyts_menu = tk.Menu(root)
     root.config(menu=unyts_menu)
     # File menu
     file_menu = tk.Menu(unyts_menu)
     unyts_menu.add_cascade(label='File', menu=file_menu)
@@ -168,16 +209,23 @@
     file_menu.add_command(label='Clean memory', command=clean_memory)
     file_menu.add_command(label='Delete cache', command=delete_cache)
     file_menu.add_separator()
     file_menu.add_command(label='Exit', command=close_gui)
     # Options menu
     options_menu = tk.Menu(unyts_menu)
     unyts_menu.add_cascade(label='Options', menu=options_menu)
-    options_menu.add_command(label="Set FVF in CMD", command=set_fvf)
-    # options_menu.add_checkbutton(label='Print path', onvalue=True, offvalue=False, variable=unyts_parameters_.print_path_)
-    # options_menu.add_checkbutton(label='Cache', onvalue=True, offvalue=False, variable=unyts_parameters_.cache_)
-    # options_menu.add_checkbutton(label='Reload on next start', onvalue=True, offvalue=False, variable=unyts_parameters_.reload_)
+    options_menu.add_command(label="Set FVF (in CMD)", command=set_fvf)
+    options_menu.add_separator()
+    options_menu.add_checkbutton(label='Show conversion path', variable=_print_path_, command=up_.print_path)
+    options_menu.add_checkbutton(label='Cache', variable=_cache_, command=up_.cache)
+    options_menu.add_checkbutton(label='Reload on next start', variable=up_.reload_, command=up_.reload_next_time)
+    # help menu
+    help_menu = tk.Menu(unyts_menu)
+    unyts_menu.add_cascade(label='Help', menu=help_menu)
+    help_menu.add_command(label='Help', command=open_help)
+    help_menu.add_command(label='GitHub', command=open_git)
+    help_menu.add_command(label=f"Version {unyts_version}")
 
     unyts_gui = UnytsApp()
     unyts_gui.master.title("Unyts converter")
     root.protocol("WM_DELETE_WINDOW", close_gui)
     unyts_gui.mainloop()
```

### Comparing `unyts-0.8.3/src/unyts/helpers/caster.py` & `unyts-0.8.9/src/unyts/helpers/caster.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/helpers/common_classes.py` & `unyts-0.8.9/src/unyts/helpers/common_classes.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/helpers/is_number.py` & `unyts-0.8.9/src/unyts/helpers/is_number.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/helpers/is_unit.py` & `unyts-0.8.9/src/unyts/helpers/is_unit.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/helpers/multi_split.py` & `unyts-0.8.9/src/unyts/helpers/multi_split.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/helpers/unit_string_tools.py` & `unyts-0.8.9/src/unyts/helpers/unit_string_tools.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/network.py` & `unyts-0.8.9/src/unyts/network.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/operations.py` & `unyts-0.8.9/src/unyts/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat Oct 24 14:38:58 2020
 
 @author: Martín Carlos Araya <martinaraya@gmail.com>
 """
 
-__version__ = '0.5.3'
-__release__ = 20230719
+__version__ = '0.5.4'
+__release__ = 20240521
 __all__ = ['unit_product', 'unit_division', 'unit_base_power', 'unit_power', 'unit_addition', 'unit_inverse']
 
 from .dictionaries import dictionary, unitless_names
 from .converter import convertible
 from .helpers.is_number import is_number
 from .helpers.unit_string_tools import reduce_units
 from .helpers.multi_split import multi_split
 
 
+_super_numbers_ = dict(zip('⁰¹³²⁴⁵⁶⁷⁸⁹', '0123456789'))
+
 def unit_split(unit_string: str) -> str:
     us = multi_split(unit_string)
     return us
 
 
 def unit_base_power(unit_string: str) -> tuple:  # tuple[str, int]
     u_bas, u_pow = '', ''
```

### Comparing `unyts-0.8.3/src/unyts/searches.py` & `unyts-0.8.9/src/unyts/searches.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/unit_class.py` & `unyts-0.8.9/src/unyts/unit_class.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/unitary.py` & `unyts-0.8.9/src/unyts/unitary.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/custom.py` & `unyts-0.8.9/src/unyts/units/custom.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/data.py` & `unyts-0.8.9/src/unyts/units/data.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/date.py` & `unyts-0.8.9/src/unyts/units/date.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/define.py` & `unyts-0.8.9/src/unyts/units/define.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/energy.py` & `unyts-0.8.9/src/unyts/units/energy.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/force.py` & `unyts-0.8.9/src/unyts/units/force.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/geometry.py` & `unyts-0.8.9/src/unyts/units/geometry.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/mass.py` & `unyts-0.8.9/src/unyts/units/mass.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/rates.py` & `unyts-0.8.9/src/unyts/units/rates.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/ratios.py` & `unyts-0.8.9/src/unyts/units/ratios.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/temperature.py` & `unyts-0.8.9/src/unyts/units/temperature.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/time.py` & `unyts-0.8.9/src/unyts/units/time.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/units/unitless.py` & `unyts-0.8.9/src/unyts/units/unitless.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts/unyts_icon.ico` & `unyts-0.8.9/src/unyts/unyts_icon.ico`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/src/unyts.egg-info/PKG-INFO` & `unyts-0.8.9/src/unyts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unyts
-Version: 0.8.3
+Version: 0.8.9
 Summary: a unit converter based on graph network and classes to operate with units.
 Author-email: Martin Carlos Araya <martinaraya@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Martín Carlos Araya
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `unyts-0.8.3/src/unyts.egg-info/SOURCES.txt` & `unyts-0.8.9/src/unyts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/tests/test_converter.py` & `unyts-0.8.9/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/tests/test_dictionaries.py` & `unyts-0.8.9/tests/test_dictionaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 known_duplicated_keys = ['PressureGradient', 'Date', 'Impedance', 'Capacitance']
 
 max_check = 25
 
 for key in dictionary:
     if key in ['Impedance', 'Date', 'otherUnits']:
         continue
-    print(key)
+    # print(key)
     if len(dictionary[key]) > max_check:
         to_check = [u for u in dictionary[key] if
                     (u.count('*') <= 1 and u.count('/') == 0) or (u.count('/') <= 1 and u.count('*') == 0)]
     else:
         to_check = dictionary[key]
     for unit in to_check[:max_check]:
+        print(key, unit)
         if key in ['Length', 'Rate'] and (len(unit) <= 2 and unit.endswith('l')) or (
                 '/' in unit and len(unit.split('/')[0]) <= 2 and unit.split('/')[0].endswith('l')):
             continue  # litre is defines as length for SI sufixes (linear multiplier)
         if unit.lower() in ['ounce', 'oz', 'ounces'] and key == 'Weight':
             continue  # 'ounce' can be volume or mass. It is always instantiated as Volume but ounce can be converted to mass
         if key == 'Density' and unit in dictionary['PressureGradient']:
             continue  # pressure gradients have density units
```

### Comparing `unyts-0.8.3/tests/test_operations.py` & `unyts-0.8.9/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/tests/test_uncertain_units.py` & `unyts-0.8.9/tests/test_uncertain_units.py`

 * *Files identical despite different names*

### Comparing `unyts-0.8.3/tests/test_units.py` & `unyts-0.8.9/tests/test_units.py`

 * *Files identical despite different names*

