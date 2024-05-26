# Comparing `tmp/magyar-4.0.5.tar.gz` & `tmp/magyar-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-4.0.5.tar", last modified: Sun May 26 06:40:03 2024, max compression
+gzip compressed data, was "magyar-4.0.6.tar", last modified: Sun May 26 07:11:36 2024, max compression
```

## Comparing `magyar-4.0.5.tar` & `magyar-4.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 06:40:03.725217 magyar-4.0.5/
--rw-r--r--   0 bela      (1000) bela      (1000)     7675 2024-05-26 06:40:03.725217 magyar-4.0.5/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     7259 2024-05-26 06:38:39.000000 magyar-4.0.5/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 06:40:03.725217 magyar-4.0.5/magyar.egg-info/
--rw-r--r--   0 bela      (1000) bela      (1000)     7675 2024-05-26 06:40:03.000000 magyar-4.0.5/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-26 06:40:03.000000 magyar-4.0.5/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-26 06:40:03.000000 magyar-4.0.5/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-26 06:40:03.000000 magyar-4.0.5/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)  2550493 2024-05-26 06:34:28.000000 magyar-4.0.5/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-26 06:40:03.725217 magyar-4.0.5/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      633 2024-05-26 06:37:43.000000 magyar-4.0.5/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 07:11:36.789558 magyar-4.0.6/
+-rw-r--r--   0 bela      (1000) bela      (1000)     7682 2024-05-26 07:11:36.789558 magyar-4.0.6/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     7266 2024-05-26 07:10:34.000000 magyar-4.0.6/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 07:11:36.789558 magyar-4.0.6/magyar.egg-info/
+-rw-r--r--   0 bela      (1000) bela      (1000)     7682 2024-05-26 07:11:36.000000 magyar-4.0.6/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-26 07:11:36.000000 magyar-4.0.6/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-26 07:11:36.000000 magyar-4.0.6/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-26 07:11:36.000000 magyar-4.0.6/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)  2560466 2024-05-26 06:56:18.000000 magyar-4.0.6/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-26 07:11:36.789558 magyar-4.0.6/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      633 2024-05-26 07:10:34.000000 magyar-4.0.6/setup.py
```

### Comparing `magyar-4.0.5/PKG-INFO` & `magyar-4.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 4.0.5
+Version: 4.0.6
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -188,23 +188,23 @@
 Adatformátum:  [('Aba', 'Fejér', 47.0292178, 18.5216608) <BR> <BR>
 Magyarosrági települések GPS koordinátáinak keresése:
 
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_keres.png)
 <BR>
 Azonos szélességi, hosszúsági körön lévő Magyar települések listázása: <BR>
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
-<BR>
+<BR><BR>
 **Postai irányítószámok - ZIP**  <BR><BR>
 magyar.irsz <BR><BR>
 Adatstruktúra : irsz = [ {
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },]  <BR><BR>
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.0.5/README.md` & `magyar-4.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -176,23 +176,23 @@
 Adatformátum:  [('Aba', 'Fejér', 47.0292178, 18.5216608) <BR> <BR>
 Magyarosrági települések GPS koordinátáinak keresése:
 
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_keres.png)
 <BR>
 Azonos szélességi, hosszúsági körön lévő Magyar települések listázása: <BR>
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
-<BR>
+<BR><BR>
 **Postai irányítószámok - ZIP**  <BR><BR>
 magyar.irsz <BR><BR>
 Adatstruktúra : irsz = [ {
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },]  <BR><BR>
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.0.5/magyar.egg-info/PKG-INFO` & `magyar-4.0.6/magyar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 4.0.5
+Version: 4.0.6
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -188,23 +188,23 @@
 Adatformátum:  [('Aba', 'Fejér', 47.0292178, 18.5216608) <BR> <BR>
 Magyarosrági települések GPS koordinátáinak keresése:
 
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_keres.png)
 <BR>
 Azonos szélességi, hosszúsági körön lévő Magyar települések listázása: <BR>
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
-<BR>
+<BR><BR>
 **Postai irányítószámok - ZIP**  <BR><BR>
 magyar.irsz <BR><BR>
 Adatstruktúra : irsz = [ {
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },]  <BR><BR>
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.0.5/magyar.py` & `magyar-4.0.6/magyar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23270 +1,23270 @@
 # Magyar nevek listái
 
 irsz = [
     {
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2009,
         "telepules": "Pilisszentlászló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2011,
         "telepules": "Budakalász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2013,
         "telepules": "Pomáz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2014,
         "telepules": "Csobánka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2015,
         "telepules": "Szigetmonostor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2016,
         "telepules": "Leányfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2017,
         "telepules": "Pócsmegyer",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2021,
         "telepules": "Tahitótfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2022,
         "telepules": "Tahitótfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2023,
         "telepules": "Dunabogdány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2024,
         "telepules": "Kisoroszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2025,
         "telepules": "Visegrád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2026,
         "telepules": "Visegrád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2027,
         "telepules": "Dömös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2028,
         "telepules": "Pilismarót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2030,
         "telepules": "Érd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2038,
         "telepules": "Sóskút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2039,
         "telepules": "Pusztazámor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2040,
         "telepules": "Budaörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2045,
         "telepules": "Törökbálint",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2049,
         "telepules": "Diósd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2051,
         "telepules": "Biatorbágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2053,
         "telepules": "Herceghalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2060,
         "telepules": "Bicske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2063,
         "telepules": "Óbarok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2064,
         "telepules": "Csabdi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2065,
         "telepules": "Mány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2066,
         "telepules": "Szár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2066,
         "telepules": "Újbarok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2067,
         "telepules": "Szárliget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2071,
         "telepules": "Páty",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2072,
         "telepules": "Zsámbék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2073,
         "telepules": "Tök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2074,
         "telepules": "Perbál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2080,
         "telepules": "Pilisjászfalu ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2081,
         "telepules": "Piliscsaba ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2083,
         "telepules": "Solymár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2084,
         "telepules": "Pilisszentiván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2085,
         "telepules": "Pilisvörösvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2086,
         "telepules": "Tinnye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2089,
         "telepules": "Telki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2090,
         "telepules": "Remeteszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2091,
         "telepules": "Etyek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2092,
         "telepules": "Budakeszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2093,
         "telepules": "Budajenő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2094,
         "telepules": "Nagykovácsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2095,
         "telepules": "Pilisszántó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2096,
         "telepules": "Üröm",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2097,
         "telepules": "Pilisborosjenő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2098,
         "telepules": "Pilisszentkereszt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2099,
         "telepules": "Pilisszentkereszt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2100,
         "telepules": "Gödöllő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2111,
         "telepules": "Szada",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2112,
         "telepules": "Veresegyház",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2113,
         "telepules": "Erdőkertes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2114,
         "telepules": "Valkó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2115,
         "telepules": "Vácszentlászló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2116,
         "telepules": "Zsámbok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2117,
         "telepules": "Isaszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2118,
         "telepules": "Dány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2119,
         "telepules": "Pécel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2120,
         "telepules": "Dunakeszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2131,
         "telepules": "Göd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2132,
         "telepules": "Göd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2133,
         "telepules": "Sződliget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2134,
         "telepules": "Sződ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2135,
         "telepules": "Csörög",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2141,
         "telepules": "Csömör",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2142,
         "telepules": "Nagytarcsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2143,
         "telepules": "Kistarcsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2144,
         "telepules": "Kerepes ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2145,
         "telepules": "Kerepes ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2146,
         "telepules": "Mogyoród",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2151,
         "telepules": "Fót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2161,
         "telepules": "Csomád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2162,
         "telepules": "Őrbottyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2163,
         "telepules": "Vácrátót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2164,
         "telepules": "Váchartyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2165,
         "telepules": "Kisnémedi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2166,
         "telepules": "Püspökszilágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2167,
         "telepules": "Vácduka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2170,
         "telepules": "Aszód",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2173,
         "telepules": "Kartal",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2174,
         "telepules": "Verseg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2175,
         "telepules": "Kálló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2176,
         "telepules": "Erdőkürt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2177,
         "telepules": "Erdőtarcsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2181,
         "telepules": "Iklad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2182,
         "telepules": "Domony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2183,
         "telepules": "Galgamácsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2184,
         "telepules": "Vácegres",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2185,
         "telepules": "Váckisújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2191,
         "telepules": "Bag",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2192,
         "telepules": "Hévízgyörk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2193,
         "telepules": "Galgahévíz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2194,
         "telepules": "Tura",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2200,
         "telepules": "Monor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2209,
         "telepules": "Péteri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2211,
         "telepules": "Vasad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2212,
         "telepules": "Csévharaszt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2213,
         "telepules": "Monorierdő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2214,
         "telepules": "Pánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2215,
         "telepules": "Káva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2216,
         "telepules": "Bénye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2217,
         "telepules": "Gomba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2220,
         "telepules": "Vecsés",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2225,
         "telepules": "Üllő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2230,
         "telepules": "Gyömrő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2233,
         "telepules": "Ecser",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2234,
         "telepules": "Maglód",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2235,
         "telepules": "Mende",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2241,
         "telepules": "Sülysáp  ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2243,
         "telepules": "Kóka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2244,
         "telepules": "Úri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2251,
         "telepules": "Tápiószecső",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2252,
         "telepules": "Tóalmás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2253,
         "telepules": "Tápióság",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2254,
         "telepules": "Szentmártonkáta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2255,
         "telepules": "Szentlőrinckáta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2300,
         "telepules": "Ráckeve",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2309,
         "telepules": "Lórév",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2310,
         "telepules": "Szigetszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2314,
         "telepules": "Halásztelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2315,
         "telepules": "Szigethalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2316,
         "telepules": "Tököl",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2317,
         "telepules": "Szigetcsép",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2318,
         "telepules": "Szigetszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2319,
         "telepules": "Szigetújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2321,
         "telepules": "Szigetbecse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2322,
         "telepules": "Makád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2330,
         "telepules": "Dunaharaszti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2335,
         "telepules": "Taksony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2336,
         "telepules": "Dunavarsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2337,
         "telepules": "Délegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2338,
         "telepules": "Áporka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2339,
         "telepules": "Majosháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2340,
         "telepules": "Kiskunlacháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2344,
         "telepules": "Dömsöd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2345,
         "telepules": "Apaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2347,
         "telepules": "Bugyi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2351,
         "telepules": "Alsónémedi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2360,
         "telepules": "Gyál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2363,
         "telepules": "Felsőpakony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2364,
         "telepules": "Ócsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2365,
         "telepules": "Inárcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2366,
         "telepules": "Kakucs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2367,
         "telepules": "Újhartyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2370,
         "telepules": "Dabas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2371,
         "telepules": "Dabas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2373,
         "telepules": "Dabas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2375,
         "telepules": "Tatárszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2376,
         "telepules": "Hernád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2377,
         "telepules": "Örkény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2378,
         "telepules": "Pusztavacs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2381,
         "telepules": "Táborfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2400,
         "telepules": "Dunaújváros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2407,
         "telepules": "Dunaújváros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2421,
         "telepules": "Nagyvenyim",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2422,
         "telepules": "Mezőfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2423,
         "telepules": "Daruszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2424,
         "telepules": "Előszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2425,
         "telepules": "Nagykarácsony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2426,
         "telepules": "Baracs ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2427,
         "telepules": "Baracs ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2428,
         "telepules": "Kisapostag",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2431,
         "telepules": "Perkáta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2432,
         "telepules": "Szabadegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2433,
         "telepules": "Sárosd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2434,
         "telepules": "Hantos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2435,
         "telepules": "Nagylók",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2440,
         "telepules": "Százhalombatta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2451,
         "telepules": "Ercsi ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2453,
         "telepules": "Ercsi ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2454,
         "telepules": "Iváncsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2455,
         "telepules": "Beloiannisz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2456,
         "telepules": "Besnyő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2457,
         "telepules": "Adony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2458,
         "telepules": "Kulcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2459,
         "telepules": "Rácalmás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2461,
         "telepules": "Tárnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2462,
         "telepules": "Martonvásár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2463,
         "telepules": "Tordas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2464,
         "telepules": "Gyúró",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2465,
         "telepules": "Ráckeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2471,
         "telepules": "Baracska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2472,
         "telepules": "Kajászó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2473,
         "telepules": "Vál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2475,
         "telepules": "Kápolnásnyék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2476,
         "telepules": "Pázmánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2477,
         "telepules": "Vereb",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2481,
         "telepules": "Velence ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2483,
         "telepules": "Gárdony ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2484,
         "telepules": "Gárdony ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2485,
         "telepules": "Gárdony ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2490,
         "telepules": "Pusztaszabolcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2500,
         "telepules": "Esztergom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2508,
         "telepules": "Esztergom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2509,
         "telepules": "Esztergom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2510,
         "telepules": "Dorog",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2517,
         "telepules": "Kesztölc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2518,
         "telepules": "Leányvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2519,
         "telepules": "Piliscsév",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2521,
         "telepules": "Csolnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2522,
         "telepules": "Dág",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2523,
         "telepules": "Sárisáp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2524,
         "telepules": "Nagysáp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2525,
         "telepules": "Bajna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2526,
         "telepules": "Epöl",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2527,
         "telepules": "Máriahalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2528,
         "telepules": "Úny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2529,
         "telepules": "Annavölgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2531,
         "telepules": "Tokod ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2532,
         "telepules": "Tokodaltáró",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2533,
         "telepules": "Bajót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2534,
         "telepules": "Tát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2535,
         "telepules": "Mogyorósbánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2536,
         "telepules": "Nyergesújfalu ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2541,
         "telepules": "Lábatlan ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2543,
         "telepules": "Süttő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2544,
         "telepules": "Neszmély",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2545,
         "telepules": "Dunaalmás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2600,
         "telepules": "Vác",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2610,
         "telepules": "Nőtincs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2610,
         "telepules": "Ősagárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2611,
         "telepules": "Felsőpetény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2612,
         "telepules": "Kosd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2613,
         "telepules": "Rád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2614,
         "telepules": "Penc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2615,
         "telepules": "Csővár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2616,
         "telepules": "Keszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2617,
         "telepules": "Alsópetény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2618,
         "telepules": "Nézsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2619,
         "telepules": "Legénd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2621,
         "telepules": "Verőce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2623,
         "telepules": "Kismaros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2624,
         "telepules": "Szokolya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2625,
         "telepules": "Kóspallag",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2626,
         "telepules": "Nagymaros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2627,
         "telepules": "Zebegény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2628,
         "telepules": "Szob",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2629,
         "telepules": "Márianosztra",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2631,
         "telepules": "Ipolydamásd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2632,
         "telepules": "Letkés",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2633,
         "telepules": "Ipolytölgyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2634,
         "telepules": "Nagybörzsöny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2635,
         "telepules": "Vámosmikola",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2636,
         "telepules": "Tésa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2637,
         "telepules": "Perőcsény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2638,
         "telepules": "Kemence",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2639,
         "telepules": "Bernecebaráti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2640,
         "telepules": "Szendehely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2641,
         "telepules": "Berkenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2642,
         "telepules": "Nógrád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2643,
         "telepules": "Diósjenő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2644,
         "telepules": "Borsosberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2645,
         "telepules": "Nagyoroszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2646,
         "telepules": "Drégelypalánk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2647,
         "telepules": "Hont",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2648,
         "telepules": "Patak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2649,
         "telepules": "Dejtár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2651,
         "telepules": "Rétság",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2652,
         "telepules": "Tereske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2653,
         "telepules": "Bánk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2654,
         "telepules": "Romhány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2655,
         "telepules": "Kétbodony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2655,
         "telepules": "Kisecset",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2655,
         "telepules": "Szente",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2656,
         "telepules": "Szátok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2657,
         "telepules": "Tolmács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2658,
         "telepules": "Horpács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2658,
         "telepules": "Pusztaberki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2659,
         "telepules": "Érsekvadkert",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2660,
         "telepules": "Balassagyarmat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2660,
         "telepules": "Ipolyszög",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2668,
         "telepules": "Patvarc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2669,
         "telepules": "Ipolyvece",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2671,
         "telepules": "Őrhalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2672,
         "telepules": "Hugyag",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2673,
         "telepules": "Csitár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2674,
         "telepules": "Iliny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2675,
         "telepules": "Nógrádmarcal",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2676,
         "telepules": "Cserhátsurány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2677,
         "telepules": "Herencsény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2678,
         "telepules": "Csesztve",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2681,
         "telepules": "Galgagyörk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2682,
         "telepules": "Püspökhatvan",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2683,
         "telepules": "Acsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2685,
         "telepules": "Nógrádsáp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2686,
         "telepules": "Galgaguta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2687,
         "telepules": "Bercel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2688,
         "telepules": "Vanyarc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2691,
         "telepules": "Nógrádkövesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2692,
         "telepules": "Szécsénke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2693,
         "telepules": "Becske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2694,
         "telepules": "Magyarnándor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2694,
         "telepules": "Cserháthaláp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2694,
         "telepules": "Debercsény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2696,
         "telepules": "Terény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2697,
         "telepules": "Szanda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2698,
         "telepules": "Mohora",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2699,
         "telepules": "Szügy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2700,
         "telepules": "Cegléd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2711,
         "telepules": "Tápiószentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2712,
         "telepules": "Nyársapát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2713,
         "telepules": "Csemő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2721,
         "telepules": "Pilis",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2723,
         "telepules": "Nyáregyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2724,
         "telepules": "Újlengyel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2730,
         "telepules": "Albertirsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2735,
         "telepules": "Dánszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2736,
         "telepules": "Mikebuda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2737,
         "telepules": "Ceglédbercel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2738,
         "telepules": "Cegléd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2740,
         "telepules": "Abony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2745,
         "telepules": "Kőröstetétlen",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2746,
         "telepules": "Jászkarajenő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2747,
         "telepules": "Törtel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2750,
         "telepules": "Nagykőrös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2755,
         "telepules": "Kocsér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2760,
         "telepules": "Nagykáta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2764,
         "telepules": "Tápióbicske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2765,
         "telepules": "Farmos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2766,
         "telepules": "Tápiószele",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2767,
         "telepules": "Tápiógyörgye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2768,
         "telepules": "Újszilvás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2769,
         "telepules": "Tápiószőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2800,
         "telepules": "Tatabánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2821,
         "telepules": "Gyermely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2822,
         "telepules": "Szomor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2823,
         "telepules": "Vértessomló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2824,
         "telepules": "Várgesztes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2831,
         "telepules": "Tarján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2832,
         "telepules": "Héreg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2833,
         "telepules": "Vértestolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2834,
         "telepules": "Tardos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2835,
         "telepules": "Tata",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2836,
         "telepules": "Baj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2837,
         "telepules": "Vértesszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2840,
         "telepules": "Oroszlány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2851,
         "telepules": "Környe",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2852,
         "telepules": "Kecskéd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2853,
         "telepules": "Kömlőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2854,
         "telepules": "Dad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2855,
         "telepules": "Bokod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2856,
         "telepules": "Szákszend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2858,
         "telepules": "Császár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2859,
         "telepules": "Vérteskethely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2861,
         "telepules": "Bakonysárkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2862,
         "telepules": "Aka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2870,
         "telepules": "Kisbér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2879,
         "telepules": "Kisbér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2881,
         "telepules": "Ászár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2882,
         "telepules": "Kerékteleki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2883,
         "telepules": "Bársonyos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2884,
         "telepules": "Bakonyszombathely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2885,
         "telepules": "Bakonybánk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2886,
         "telepules": "Réde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2887,
         "telepules": "Ácsteszér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2888,
         "telepules": "Csatka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2889,
         "telepules": "Súr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2890,
         "telepules": "Tata",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2896,
         "telepules": "Szomód",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2897,
         "telepules": "Dunaszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2898,
         "telepules": "Kocs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2899,
         "telepules": "Naszály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2900,
         "telepules": "Komárom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2903,
         "telepules": "Komárom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2911,
         "telepules": "Mocsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2921,
         "telepules": "Komárom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2931,
         "telepules": "Almásfüzitő ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2941,
         "telepules": "Ács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2942,
         "telepules": "Nagyigmánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2943,
         "telepules": "Bábolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2943,
         "telepules": "Tárkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2944,
         "telepules": "Bana",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2945,
         "telepules": "Tárkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2946,
         "telepules": "Csép",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2947,
         "telepules": "Ete",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2948,
         "telepules": "Kisigmánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 2949,
         "telepules": "Csém",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3000,
         "telepules": "Hatvan",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3009,
         "telepules": "Kerekharaszt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3011,
         "telepules": "Heréd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3012,
         "telepules": "Nagykökényes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3013,
         "telepules": "Ecséd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3014,
         "telepules": "Hort",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3015,
         "telepules": "Csány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3016,
         "telepules": "Boldog",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3021,
         "telepules": "Lőrinci ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3022,
         "telepules": "Lőrinci ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3023,
         "telepules": "Petőfibánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3024,
         "telepules": "Lőrinci ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3031,
         "telepules": "Zagyvaszántó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3032,
         "telepules": "Apc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3033,
         "telepules": "Rózsaszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3034,
         "telepules": "Szűcsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3035,
         "telepules": "Gyöngyöspata",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3036,
         "telepules": "Gyöngyöstarján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3041,
         "telepules": "Héhalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3042,
         "telepules": "Palotás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3043,
         "telepules": "Egyházasdengeleg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3044,
         "telepules": "Szirák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3045,
         "telepules": "Bér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3046,
         "telepules": "Kisbágyon",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3047,
         "telepules": "Buják",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3051,
         "telepules": "Szarvasgede",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3052,
         "telepules": "Csécse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3053,
         "telepules": "Ecseg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3053,
         "telepules": "Kozárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3060,
         "telepules": "Pásztó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3063,
         "telepules": "Jobbágyi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3064,
         "telepules": "Szurdokpüspöki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3065,
         "telepules": "Pásztó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3066,
         "telepules": "Cserhátszentiván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3066,
         "telepules": "Bokor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3066,
         "telepules": "Kutasó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3067,
         "telepules": "Felsőtold",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3067,
         "telepules": "Garáb",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3068,
         "telepules": "Mátraszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3069,
         "telepules": "Alsótold",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3070,
         "telepules": "Bátonyterenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3073,
         "telepules": "Tar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3074,
         "telepules": "Sámsonháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3075,
         "telepules": "Nagybárkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3075,
         "telepules": "Kisbárkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3075,
         "telepules": "Márkháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3077,
         "telepules": "Mátraverebély",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3078,
         "telepules": "Bátonyterenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3082,
         "telepules": "Pásztó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3100,
         "telepules": "Salgótarján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3102,
         "telepules": "Salgótarján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3104,
         "telepules": "Salgótarján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3109,
         "telepules": "Salgótarján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3121,
         "telepules": "Somoskőújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3123,
         "telepules": "Cered",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3124,
         "telepules": "Zabar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3125,
         "telepules": "Szilaspogony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3126,
         "telepules": "Bárna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3127,
         "telepules": "Kazár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3128,
         "telepules": "Vizslás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3129,
         "telepules": "Lucfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3129,
         "telepules": "Nagykeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3131,
         "telepules": "Sóshartyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3132,
         "telepules": "Nógrádmegyer",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3133,
         "telepules": "Magyargéc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3134,
         "telepules": "Piliny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3135,
         "telepules": "Szécsényfelfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3136,
         "telepules": "Etes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3137,
         "telepules": "Karancsberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3138,
         "telepules": "Ipolytarnóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3141,
         "telepules": "Salgótarján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3142,
         "telepules": "Mátraszele",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3143,
         "telepules": "Mátranovák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3144,
         "telepules": "Mátranovák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3145,
         "telepules": "Mátraterenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3146,
         "telepules": "Mátraterenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3147,
         "telepules": "Kazár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3151,
         "telepules": "Rákóczibánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3152,
         "telepules": "Nemti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3153,
         "telepules": "Dorogháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3154,
         "telepules": "Szuha",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3155,
         "telepules": "Mátramindszent",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3161,
         "telepules": "Kishartyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3162,
         "telepules": "Ságújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3163,
         "telepules": "Karancsság",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3163,
         "telepules": "Szalmatercs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3165,
         "telepules": "Endrefalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3170,
         "telepules": "Szécsény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3175,
         "telepules": "Nagylóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3176,
         "telepules": "Hollókő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3177,
         "telepules": "Rimóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3178,
         "telepules": "Varsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3179,
         "telepules": "Nógrádsipek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3181,
         "telepules": "Karancsalja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3182,
         "telepules": "Karancslapujtő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3183,
         "telepules": "Karancskeszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3184,
         "telepules": "Mihálygerge",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3185,
         "telepules": "Egyházasgerge",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3186,
         "telepules": "Litke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3187,
         "telepules": "Nógrádszakál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3188,
         "telepules": "Ludányhalászi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3200,
         "telepules": "Gyöngyös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3211,
         "telepules": "Gyöngyösoroszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3212,
         "telepules": "Gyöngyöshalász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3213,
         "telepules": "Atkár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3214,
         "telepules": "Nagyréde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3221,
         "telepules": "Gyöngyös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3231,
         "telepules": "Gyöngyössolymos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3232,
         "telepules": "Gyöngyös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3233,
         "telepules": "Gyöngyös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3234,
         "telepules": "Mátraszentimre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3235,
         "telepules": "Mátraszentimre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3240,
         "telepules": "Parád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3242,
         "telepules": "Parádsasvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3243,
         "telepules": "Bodony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3245,
         "telepules": "Recsk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3246,
         "telepules": "Mátraderecske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3247,
         "telepules": "Mátraballa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3248,
         "telepules": "Ivád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3250,
         "telepules": "Pétervására",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3252,
         "telepules": "Erdőkövesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3253,
         "telepules": "Istenmezeje",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3254,
         "telepules": "Váraszó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3255,
         "telepules": "Fedémes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3256,
         "telepules": "Kisfüzes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3257,
         "telepules": "Bükkszenterzsébet",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3258,
         "telepules": "Tarnalelesz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3259,
         "telepules": "Szentdomonkos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3261,
         "telepules": "Abasár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3261,
         "telepules": "Pálosvörösmart",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3262,
         "telepules": "Markaz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3263,
         "telepules": "Domoszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3264,
         "telepules": "Kisnána",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3265,
         "telepules": "Vécs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3271,
         "telepules": "Visonta ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3272,
         "telepules": "Visonta ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3273,
         "telepules": "Halmajugra",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3274,
         "telepules": "Ludas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3275,
         "telepules": "Detk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3281,
         "telepules": "Karácsond",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3282,
         "telepules": "Nagyfüged",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3283,
         "telepules": "Tarnazsadány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3284,
         "telepules": "Tarnaméra",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3291,
         "telepules": "Vámosgyörk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3292,
         "telepules": "Adács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3293,
         "telepules": "Visznek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3294,
         "telepules": "Tarnaörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3295,
         "telepules": "Erk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3296,
         "telepules": "Zaránk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3300,
         "telepules": "Eger",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3321,
         "telepules": "Egerbakta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3322,
         "telepules": "Hevesaranyos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3323,
         "telepules": "Szarvaskő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3324,
         "telepules": "Felsőtárkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3325,
         "telepules": "Noszvaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3326,
         "telepules": "Ostoros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3327,
         "telepules": "Novaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3328,
         "telepules": "Egerszólát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3331,
         "telepules": "Tarnaszentmária",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3332,
         "telepules": "Sirok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3333,
         "telepules": "Terpes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3334,
         "telepules": "Szajla",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3335,
         "telepules": "Bükkszék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3336,
         "telepules": "Bátor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3337,
         "telepules": "Egerbocs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3341,
         "telepules": "Egercsehi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3341,
         "telepules": "Szúcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3343,
         "telepules": "Bekölce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3344,
         "telepules": "Mikófalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3345,
         "telepules": "Mónosbél",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3346,
         "telepules": "Bélapátfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3346,
         "telepules": "Bükkszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3347,
         "telepules": "Balaton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3348,
         "telepules": "Szilvásvárad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3349,
         "telepules": "Nagyvisnyó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3350,
         "telepules": "Kál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3351,
         "telepules": "Verpelét",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3352,
         "telepules": "Feldebrő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3353,
         "telepules": "Aldebrő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3354,
         "telepules": "Tófalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3355,
         "telepules": "Kápolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3356,
         "telepules": "Kompolt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3357,
         "telepules": "Nagyút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3358,
         "telepules": "Erdőtelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3359,
         "telepules": "Tenk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3360,
         "telepules": "Heves",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3368,
         "telepules": "Boconád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3369,
         "telepules": "Tarnabod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3371,
         "telepules": "Átány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3372,
         "telepules": "Kömlő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3373,
         "telepules": "Besenyőtelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3374,
         "telepules": "Dormánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3375,
         "telepules": "Mezőtárkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3377,
         "telepules": "Szihalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3378,
         "telepules": "Mezőszemere",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3379,
         "telepules": "Egerfarmos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3381,
         "telepules": "Pély",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3382,
         "telepules": "Tarnaszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3383,
         "telepules": "Hevesvezekény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3384,
         "telepules": "Kisköre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3385,
         "telepules": "Tiszanána",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3386,
         "telepules": "Sarud",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3387,
         "telepules": "Újlőrincfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3388,
         "telepules": "Poroszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3390,
         "telepules": "Füzesabony ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3394,
         "telepules": "Egerszalók",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3395,
         "telepules": "Demjén",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3396,
         "telepules": "Kerecsend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3397,
         "telepules": "Maklár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3398,
         "telepules": "Nagytálya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3399,
         "telepules": "Andornaktálya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3400,
         "telepules": "Mezőkövesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3411,
         "telepules": "Szomolya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3412,
         "telepules": "Bogács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3413,
         "telepules": "Cserépfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3414,
         "telepules": "Bükkzsérc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3416,
         "telepules": "Tard",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3417,
         "telepules": "Cserépváralja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3418,
         "telepules": "Szentistván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3421,
         "telepules": "Mezőnyárád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3422,
         "telepules": "Bükkábrány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3423,
         "telepules": "Tibolddaróc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3424,
         "telepules": "Kács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3425,
         "telepules": "Sály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3426,
         "telepules": "Borsodgeszt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3431,
         "telepules": "Vatta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3432,
         "telepules": "Emőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3433,
         "telepules": "Nyékládháza ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3434,
         "telepules": "Mályi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3441,
         "telepules": "Mezőkeresztes ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3442,
         "telepules": "Csincse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3443,
         "telepules": "Mezőnagymihály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3444,
         "telepules": "Gelej",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3450,
         "telepules": "Mezőcsát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3458,
         "telepules": "Tiszakeszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3459,
         "telepules": "Igrici",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3461,
         "telepules": "Egerlövő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3462,
         "telepules": "Borsodivánka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3463,
         "telepules": "Négyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3464,
         "telepules": "Tiszavalk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3465,
         "telepules": "Tiszabábolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3466,
         "telepules": "Tiszadorogma",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3467,
         "telepules": "Ároktő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3500,
         "telepules": "Miskolc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3551,
         "telepules": "Ónod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3552,
         "telepules": "Muhi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3553,
         "telepules": "Kistokaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3554,
         "telepules": "Bükkaranyos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3555,
         "telepules": "Harsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3556,
         "telepules": "Kisgyőr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3557,
         "telepules": "Bükkszentkereszt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3559,
         "telepules": "Répáshuta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3561,
         "telepules": "Felsőzsolca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3562,
         "telepules": "Onga",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3563,
         "telepules": "Hernádkak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3564,
         "telepules": "Hernádnémeti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3565,
         "telepules": "Tiszalúc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3571,
         "telepules": "Alsózsolca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3572,
         "telepules": "Sajólád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3573,
         "telepules": "Sajópetri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3574,
         "telepules": "Bőcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3575,
         "telepules": "Berzék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3576,
         "telepules": "Sajóhídvég",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3577,
         "telepules": "Köröm",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3578,
         "telepules": "Girincs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3578,
         "telepules": "Kiscsécs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3579,
         "telepules": "Kesznyéten",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3580,
         "telepules": "Tiszaújváros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3586,
         "telepules": "Sajóörös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3587,
         "telepules": "Tiszapalkonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3588,
         "telepules": "Hejőkürt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3589,
         "telepules": "Tiszatarján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3591,
         "telepules": "Oszlár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3592,
         "telepules": "Nemesbikk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3593,
         "telepules": "Hejőbába",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3594,
         "telepules": "Hejőpapi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3595,
         "telepules": "Hejőszalonta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3596,
         "telepules": "Szakáld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3597,
         "telepules": "Hejőkeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3598,
         "telepules": "Nagycsécs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3599,
         "telepules": "Sajószöged",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3600,
         "telepules": "Ózd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3604,
         "telepules": "Ózd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3608,
         "telepules": "Farkaslyuk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3621,
         "telepules": "Ózd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3622,
         "telepules": "Uppony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3623,
         "telepules": "Borsodszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3625,
         "telepules": "Ózd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3626,
         "telepules": "Hangony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3627,
         "telepules": "Domaháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3627,
         "telepules": "Kissikátor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3630,
         "telepules": "Putnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3635,
         "telepules": "Dubicsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3636,
         "telepules": "Vadna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3636,
         "telepules": "Sajógalgóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3641,
         "telepules": "Nagybarca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3642,
         "telepules": "Bánhorváti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3643,
         "telepules": "Dédestapolcsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3644,
         "telepules": "Tardona",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3645,
         "telepules": "Mályinka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3646,
         "telepules": "Nekézseny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3647,
         "telepules": "Csokvaomány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3648,
         "telepules": "Csernely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3648,
         "telepules": "Bükkmogyorósd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3648,
         "telepules": "Lénárddaróc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3651,
         "telepules": "Ózd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3652,
         "telepules": "Sajónémeti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3653,
         "telepules": "Sajópüspöki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3654,
         "telepules": "Bánréve",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3655,
         "telepules": "Hét",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3656,
         "telepules": "Sajóvelezd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3656,
         "telepules": "Sajómercse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3657,
         "telepules": "Királd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3658,
         "telepules": "Borsodbóta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3659,
         "telepules": "Sáta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3661,
         "telepules": "Ózd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3662,
         "telepules": "Ózd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3663,
         "telepules": "Arló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3664,
         "telepules": "Járdánháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3671,
         "telepules": "Borsodnádasd ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3672,
         "telepules": "Borsodnádasd ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3700,
         "telepules": "Kazincbarcika",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3704,
         "telepules": "Berente",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3711,
         "telepules": "Szirmabesenyő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3712,
         "telepules": "Sajóvámos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3712,
         "telepules": "Sajósenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3713,
         "telepules": "Arnót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3714,
         "telepules": "Sajópálfala",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3715,
         "telepules": "Gesztely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3716,
         "telepules": "Újcsanálos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3716,
         "telepules": "Sóstófalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3717,
         "telepules": "Alsódobsza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3718,
         "telepules": "Megyaszó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3720,
         "telepules": "Sajókaza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3720,
         "telepules": "Sajóivánka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3721,
         "telepules": "Felsőnyárád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3721,
         "telepules": "Dövény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3721,
         "telepules": "Jákfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3722,
         "telepules": "Felsőkelecsény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3723,
         "telepules": "Zubogy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3724,
         "telepules": "Ragály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3724,
         "telepules": "Trizs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3725,
         "telepules": "Imola",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3726,
         "telepules": "Zádorfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3726,
         "telepules": "Alsószuha",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3726,
         "telepules": "Szuhafő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3728,
         "telepules": "Kelemér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3728,
         "telepules": "Gömörszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3729,
         "telepules": "Serényfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3731,
         "telepules": "Szuhakálló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3732,
         "telepules": "Kurityán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3733,
         "telepules": "Rudabánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3734,
         "telepules": "Szuhogy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3735,
         "telepules": "Felsőtelekes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3735,
         "telepules": "Alsótelekes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3735,
         "telepules": "Kánó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3741,
         "telepules": "Izsófalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3742,
         "telepules": "Rudolftelep",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3743,
         "telepules": "Ormosbánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3744,
         "telepules": "Múcsony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3751,
         "telepules": "Szendrőlád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3752,
         "telepules": "Szendrő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3752,
         "telepules": "Galvács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3753,
         "telepules": "Abod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3754,
         "telepules": "Szalonna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3754,
         "telepules": "Meszes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3755,
         "telepules": "Martonyi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3756,
         "telepules": "Perkupa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3756,
         "telepules": "Varbóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3757,
         "telepules": "Szőlősardó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3757,
         "telepules": "Égerszög",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3757,
         "telepules": "Teresztenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3758,
         "telepules": "Jósvafő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3759,
         "telepules": "Aggtelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3761,
         "telepules": "Szin",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3761,
         "telepules": "Szinpetri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3761,
         "telepules": "Tornakápolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3762,
         "telepules": "Szögliget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3763,
         "telepules": "Bódvaszilas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3764,
         "telepules": "Bódvarákó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3765,
         "telepules": "Komjáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3765,
         "telepules": "Tornabarakony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3765,
         "telepules": "Tornaszentandrás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3767,
         "telepules": "Tornanádaska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3768,
         "telepules": "Hidvégardó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3768,
         "telepules": "Becskeháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3768,
         "telepules": "Bódvalenke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3769,
         "telepules": "Tornaszentjakab",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3770,
         "telepules": "Sajószentpéter",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3773,
         "telepules": "Sajókápolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3773,
         "telepules": "Sajólászlófalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3775,
         "telepules": "Kondó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3776,
         "telepules": "Radostyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3777,
         "telepules": "Parasznya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3778,
         "telepules": "Varbó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3779,
         "telepules": "Alacska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3780,
         "telepules": "Edelény ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3780,
         "telepules": "Balajt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3780,
         "telepules": "Damak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3780,
         "telepules": "Ládbesenyő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3783,
         "telepules": "Edelény ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3786,
         "telepules": "Lak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3786,
         "telepules": "Hegymeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3786,
         "telepules": "Irota",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3786,
         "telepules": "Szakácsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3787,
         "telepules": "Tomor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3791,
         "telepules": "Sajókeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3792,
         "telepules": "Sajóbábony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3793,
         "telepules": "Sajóecseg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3794,
         "telepules": "Boldva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3794,
         "telepules": "Ziliz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3795,
         "telepules": "Hangács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3795,
         "telepules": "Nyomár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3796,
         "telepules": "Borsodszirák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3800,
         "telepules": "Szikszó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3809,
         "telepules": "Selyeb",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3809,
         "telepules": "Abaújszolnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3809,
         "telepules": "Nyésta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3811,
         "telepules": "Alsóvadász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3812,
         "telepules": "Homrogd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3812,
         "telepules": "Monaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3813,
         "telepules": "Kupa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3814,
         "telepules": "Felsővadász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3815,
         "telepules": "Gadna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3815,
         "telepules": "Abaújlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3816,
         "telepules": "Gagyvendégi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3817,
         "telepules": "Gagybátor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3821,
         "telepules": "Krasznokvajda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3821,
         "telepules": "Büttös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3821,
         "telepules": "Kány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3821,
         "telepules": "Keresztéte",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3821,
         "telepules": "Pamlény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3821,
         "telepules": "Perecse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3821,
         "telepules": "Szászfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3825,
         "telepules": "Rakaca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3825,
         "telepules": "Debréte",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3825,
         "telepules": "Viszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3826,
         "telepules": "Rakacaszend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3831,
         "telepules": "Kázsmárk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3832,
         "telepules": "Léh",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3833,
         "telepules": "Rásonysápberencs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3834,
         "telepules": "Detek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3834,
         "telepules": "Beret",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3836,
         "telepules": "Baktakék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3837,
         "telepules": "Felsőgagy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3837,
         "telepules": "Alsógagy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3837,
         "telepules": "Csenyéte",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3837,
         "telepules": "Gagyapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3841,
         "telepules": "Aszaló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3842,
         "telepules": "Halmaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3843,
         "telepules": "Kiskinizs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3844,
         "telepules": "Nagykinizs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3844,
         "telepules": "Szentistvánbaksa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3846,
         "telepules": "Hernádkércs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3847,
         "telepules": "Felsődobsza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3848,
         "telepules": "Csobád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3849,
         "telepules": "Forró",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3851,
         "telepules": "Ináncs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3852,
         "telepules": "Hernádszentandrás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3853,
         "telepules": "Pere",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3853,
         "telepules": "Hernádbűd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3854,
         "telepules": "Gibárt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3855,
         "telepules": "Fancsal",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3860,
         "telepules": "Encs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3863,
         "telepules": "Szalaszend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3864,
         "telepules": "Fulókércs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3865,
         "telepules": "Fáj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3866,
         "telepules": "Szemere",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3866,
         "telepules": "Litka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3871,
         "telepules": "Méra",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3872,
         "telepules": "Novajidrány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3873,
         "telepules": "Garadna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3874,
         "telepules": "Hernádvécse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3874,
         "telepules": "Hernádpetri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3874,
         "telepules": "Pusztaradvány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3875,
         "telepules": "Hernádszurdok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3876,
         "telepules": "Hidasnémeti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3877,
         "telepules": "Tornyosnémeti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3881,
         "telepules": "Abaújszántó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3881,
         "telepules": "Baskó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3881,
         "telepules": "Sima",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3882,
         "telepules": "Abaújkér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3882,
         "telepules": "Abaújalpár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3884,
         "telepules": "Boldogkőújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3885,
         "telepules": "Boldogkőváralja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3885,
         "telepules": "Arka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3886,
         "telepules": "Korlát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3887,
         "telepules": "Hernádcéce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3888,
         "telepules": "Vizsoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3891,
         "telepules": "Vilmány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3892,
         "telepules": "Hejce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3893,
         "telepules": "Fony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3893,
         "telepules": "Mogyoróska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3893,
         "telepules": "Regéc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3894,
         "telepules": "Göncruszka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3895,
         "telepules": "Gönc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3896,
         "telepules": "Telkibánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3897,
         "telepules": "Zsujta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3898,
         "telepules": "Abaújvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3898,
         "telepules": "Pányok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3899,
         "telepules": "Kéked",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3900,
         "telepules": "Szerencs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3902,
         "telepules": "Szerencs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3903,
         "telepules": "Bekecs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3904,
         "telepules": "Legyesbénye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3905,
         "telepules": "Monok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3906,
         "telepules": "Golop",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3907,
         "telepules": "Tállya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3908,
         "telepules": "Rátka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3909,
         "telepules": "Mád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3910,
         "telepules": "Tokaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3915,
         "telepules": "Tarcal",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3916,
         "telepules": "Bodrogkeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3917,
         "telepules": "Bodrogkisfalud",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3918,
         "telepules": "Szegi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3918,
         "telepules": "Szegilong",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3921,
         "telepules": "Taktaszada",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3922,
         "telepules": "Taktaharkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3923,
         "telepules": "Gesztely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3924,
         "telepules": "Taktakenéz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3925,
         "telepules": "Prügy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3926,
         "telepules": "Taktabáj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3927,
         "telepules": "Csobaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3928,
         "telepules": "Tiszatardos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3929,
         "telepules": "Tiszaladány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3931,
         "telepules": "Mezőzombor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3932,
         "telepules": "Erdőbénye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3933,
         "telepules": "Olaszliszka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3934,
         "telepules": "Tolcsva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3935,
         "telepules": "Erdőhorváti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3936,
         "telepules": "Háromhuta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3937,
         "telepules": "Komlóska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3941,
         "telepules": "Vámosújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3942,
         "telepules": "Sárazsadány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3943,
         "telepules": "Bodrogolaszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3944,
         "telepules": "Sátoraljaújhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3945,
         "telepules": "Sátoraljaújhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3950,
         "telepules": "Sárospatak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3954,
         "telepules": "Györgytarló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3955,
         "telepules": "Kenézlő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3956,
         "telepules": "Viss",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3957,
         "telepules": "Zalkod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3958,
         "telepules": "Hercegkút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3959,
         "telepules": "Makkoshotyka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3961,
         "telepules": "Vajdácska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3962,
         "telepules": "Karos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3963,
         "telepules": "Karcsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3964,
         "telepules": "Pácin",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3965,
         "telepules": "Nagyrozvágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3965,
         "telepules": "Kisrozvágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3967,
         "telepules": "Lácacséke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3971,
         "telepules": "Tiszakarád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3972,
         "telepules": "Tiszacsermely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3973,
         "telepules": "Cigánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3974,
         "telepules": "Ricse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3974,
         "telepules": "Semjén",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3976,
         "telepules": "Révleányvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3977,
         "telepules": "Zemplénagárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3978,
         "telepules": "Dámóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3980,
         "telepules": "Sátoraljaújhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3985,
         "telepules": "Alsóberecki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3985,
         "telepules": "Felsőberecki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3987,
         "telepules": "Bodroghalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3988,
         "telepules": "Sátoraljaújhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3989,
         "telepules": "Mikóháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3989,
         "telepules": "Alsóregmec",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3989,
         "telepules": "Felsőregmec",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3991,
         "telepules": "Vilyvitány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3992,
         "telepules": "Kovácsvágás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3992,
         "telepules": "Vágáshuta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3993,
         "telepules": "Füzérradvány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3994,
         "telepules": "Pálháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3994,
         "telepules": "Bózsva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3994,
         "telepules": "Filkeháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3994,
         "telepules": "Füzérkajata",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3994,
         "telepules": "Kishuta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3994,
         "telepules": "Nagyhuta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3995,
         "telepules": "Pusztafalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3996,
         "telepules": "Füzér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3997,
         "telepules": "Füzérkomlós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3998,
         "telepules": "Nyíri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 3999,
         "telepules": "Hollóháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4000,
         "telepules": "Debrecen",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4060,
         "telepules": "Balmazújváros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4064,
         "telepules": "Nagyhegyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4065,
         "telepules": "Újszentmargita",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4066,
         "telepules": "Tiszacsege",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4067,
         "telepules": "Egyek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4069,
         "telepules": "Egyek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4071,
         "telepules": "Hortobágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4074,
         "telepules": "Hajdúböszörmény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4075,
         "telepules": "Görbeháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4080,
         "telepules": "Hajdúnánás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4085,
         "telepules": "Hajdúnánás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4086,
         "telepules": "Hajdúböszörmény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4087,
         "telepules": "Hajdúdorog",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4090,
         "telepules": "Polgár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4095,
         "telepules": "Folyás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4096,
         "telepules": "Újtikos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4097,
         "telepules": "Tiszagyulaháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4100,
         "telepules": "Berettyóújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4110,
         "telepules": "Biharkeresztes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4114,
         "telepules": "Bojt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4115,
         "telepules": "Ártánd ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4116,
         "telepules": "Berekböszörmény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4117,
         "telepules": "Told ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4118,
         "telepules": "Mezőpeterd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4119,
         "telepules": "Váncsod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4121,
         "telepules": "Szentpéterszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4122,
         "telepules": "Gáborján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4123,
         "telepules": "Hencida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4124,
         "telepules": "Esztár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4125,
         "telepules": "Pocsaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4126,
         "telepules": "Kismarja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4127,
         "telepules": "Nagykereki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4128,
         "telepules": "Bedő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4130,
         "telepules": "Derecske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4132,
         "telepules": "Tépe",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4133,
         "telepules": "Konyár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4134,
         "telepules": "Mezősas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4135,
         "telepules": "Körösszegapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4136,
         "telepules": "Körösszakál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4137,
         "telepules": "Magyarhomorog",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4138,
         "telepules": "Komádi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4141,
         "telepules": "Furta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4142,
         "telepules": "Zsáka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4143,
         "telepules": "Vekerd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4144,
         "telepules": "Darvas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4145,
         "telepules": "Csökmő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4146,
         "telepules": "Újiráz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4150,
         "telepules": "Püspökladány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4161,
         "telepules": "Báránd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4162,
         "telepules": "Szerep",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4163,
         "telepules": "Szerep",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4164,
         "telepules": "Bakonszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4171,
         "telepules": "Sárrétudvari",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4172,
         "telepules": "Biharnagybajom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4173,
         "telepules": "Nagyrábé",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4174,
         "telepules": "Bihartorda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4175,
         "telepules": "Bihardancsháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4176,
         "telepules": "Sáp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4177,
         "telepules": "Földes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4181,
         "telepules": "Nádudvar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4183,
         "telepules": "Kaba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4184,
         "telepules": "Tetétlen",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4200,
         "telepules": "Hajdúszoboszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4211,
         "telepules": "Ebes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4212,
         "telepules": "Hajdúszovát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4220,
         "telepules": "Hajdúböszörmény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4224,
         "telepules": "Hajdúböszörmény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4231,
         "telepules": "Bököny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4232,
         "telepules": "Geszteréd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4233,
         "telepules": "Balkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4234,
         "telepules": "Szakoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4235,
         "telepules": "Biri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4241,
         "telepules": "Bocskaikert",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4242,
         "telepules": "Hajdúhadház",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4243,
         "telepules": "Téglás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4244,
         "telepules": "Újfehértó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4245,
         "telepules": "Érpatak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4246,
         "telepules": "Nyíregyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4251,
         "telepules": "Hajdúsámson",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4252,
         "telepules": "Nyíradony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4253,
         "telepules": "Nyíradony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4254,
         "telepules": "Nyíradony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4262,
         "telepules": "Nyíracsád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4263,
         "telepules": "Nyírmártonfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4264,
         "telepules": "Nyírábrány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4266,
         "telepules": "Fülöp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4267,
         "telepules": "Penészlek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4271,
         "telepules": "Mikepércs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4272,
         "telepules": "Sáránd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4273,
         "telepules": "Hajdúbagos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4274,
         "telepules": "Hosszúpályi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4275,
         "telepules": "Monostorpályi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4281,
         "telepules": "Létavértes ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4283,
         "telepules": "Létavértes ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4284,
         "telepules": "Kokad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4285,
         "telepules": "Álmosd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4286,
         "telepules": "Bagamér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4287,
         "telepules": "Vámospércs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4288,
         "telepules": "Újléta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4300,
         "telepules": "Nyírbátor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4311,
         "telepules": "Nyírgyulaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4320,
         "telepules": "Nagykálló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4324,
         "telepules": "Kállósemjén",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4325,
         "telepules": "Kisléta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4326,
         "telepules": "Máriapócs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4327,
         "telepules": "Pócspetri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4331,
         "telepules": "Nyírcsászári",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4332,
         "telepules": "Nyírderzs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4333,
         "telepules": "Nyírkáta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4334,
         "telepules": "Hodász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4335,
         "telepules": "Kántorjánosi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4336,
         "telepules": "Őr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4337,
         "telepules": "Jármi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4338,
         "telepules": "Papos ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4341,
         "telepules": "Nyírvasvári",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4342,
         "telepules": "Terem",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4343,
         "telepules": "Bátorliget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4351,
         "telepules": "Vállaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4352,
         "telepules": "Mérk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4353,
         "telepules": "Tiborszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4354,
         "telepules": "Fábiánháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4355,
         "telepules": "Nagyecsed",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4356,
         "telepules": "Nyírcsaholy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4361,
         "telepules": "Nyírbogát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4362,
         "telepules": "Nyírgelse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4363,
         "telepules": "Nyírmihálydi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4371,
         "telepules": "Nyírlugos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4372,
         "telepules": "Nyírbéltek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4373,
         "telepules": "Ömböly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4374,
         "telepules": "Encsencs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4375,
         "telepules": "Piricse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4376,
         "telepules": "Nyírpilis",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4400,
         "telepules": "Nyíregyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4405,
         "telepules": "Nyíregyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4431,
         "telepules": "Nyíregyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4432,
         "telepules": "Nyíregyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4433,
         "telepules": "Nyíregyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4434,
         "telepules": "Kálmánháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4440,
         "telepules": "Tiszavasvári",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4441,
         "telepules": "Szorgalmatos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4445,
         "telepules": "Nagycserkesz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4446,
         "telepules": "Tiszaeszlár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4447,
         "telepules": "Tiszalök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4450,
         "telepules": "Tiszalök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4455,
         "telepules": "Tiszadada",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4456,
         "telepules": "Tiszadob",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4461,
         "telepules": "Nyírtelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4463,
         "telepules": "Tiszanagyfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4464,
         "telepules": "Tiszaeszlár    ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4465,
         "telepules": "Rakamaz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4466,
         "telepules": "Timár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4467,
         "telepules": "Szabolcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4468,
         "telepules": "Balsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4471,
         "telepules": "Gávavencsellő   ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4472,
         "telepules": "Gávavencsellő   ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4474,
         "telepules": "Tiszabercel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4475,
         "telepules": "Paszab",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4481,
         "telepules": "Nyíregyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4482,
         "telepules": "Kótaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4483,
         "telepules": "Buj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4484,
         "telepules": "Ibrány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4485,
         "telepules": "Nagyhalász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4486,
         "telepules": "Tiszatelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4487,
         "telepules": "Tiszatelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4488,
         "telepules": "Beszterec",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4491,
         "telepules": "Újdombrád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4492,
         "telepules": "Dombrád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4493,
         "telepules": "Tiszakanyár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4494,
         "telepules": "Kékcse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4495,
         "telepules": "Döge",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4496,
         "telepules": "Szabolcsveresmart",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4501,
         "telepules": "Kemecse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4502,
         "telepules": "Vasmegyer",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4503,
         "telepules": "Tiszarád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4511,
         "telepules": "Nyírbogdány ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4515,
         "telepules": "Kék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4516,
         "telepules": "Demecser",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4517,
         "telepules": "Gégény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4521,
         "telepules": "Berkesz ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4522,
         "telepules": "Nyírtass",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4523,
         "telepules": "Pátroha",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4524,
         "telepules": "Ajak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4525,
         "telepules": "Rétközberencs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4531,
         "telepules": "Nyírpazony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4532,
         "telepules": "Nyírtura",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4533,
         "telepules": "Sényő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4534,
         "telepules": "Székely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4535,
         "telepules": "Nyíribrony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4536,
         "telepules": "Ramocsaháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4537,
         "telepules": "Nyírkércs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4541,
         "telepules": "Nyírjákó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4542,
         "telepules": "Petneháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4543,
         "telepules": "Laskod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4544,
         "telepules": "Nyírkarász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4545,
         "telepules": "Gyulaháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4546,
         "telepules": "Anarcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4547,
         "telepules": "Szabolcsbáka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4551,
         "telepules": "Nyíregyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4552,
         "telepules": "Napkor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4553,
         "telepules": "Apagy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4554,
         "telepules": "Nyírtét",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4555,
         "telepules": "Levelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4556,
         "telepules": "Magy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4557,
         "telepules": "Besenyőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4558,
         "telepules": "Ófehértó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4561,
         "telepules": "Baktalórántháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4562,
         "telepules": "Vaja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4563,
         "telepules": "Rohod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4564,
         "telepules": "Nyírmada",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4565,
         "telepules": "Pusztadobos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4566,
         "telepules": "Ilk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4567,
         "telepules": "Gemzse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4600,
         "telepules": "Kisvárda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4611,
         "telepules": "Jéke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4621,
         "telepules": "Fényeslitke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4622,
         "telepules": "Komoró",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4623,
         "telepules": "Tuzsér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4624,
         "telepules": "Tiszabezdéd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4625,
         "telepules": "Záhony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4625,
         "telepules": "Győröcske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4627,
         "telepules": "Zsurk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4628,
         "telepules": "Tiszaszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4631,
         "telepules": "Pap",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4632,
         "telepules": "Nyírlövő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4633,
         "telepules": "Lövőpetri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4634,
         "telepules": "Aranyosapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4635,
         "telepules": "Újkenéz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4641,
         "telepules": "Mezőladány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4642,
         "telepules": "Tornyospálca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4643,
         "telepules": "Benk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4644,
         "telepules": "Mándok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4645,
         "telepules": "Tiszamogyorós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4646,
         "telepules": "Eperjeske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4700,
         "telepules": "Mátészalka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4721,
         "telepules": "Szamoskér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4722,
         "telepules": "Nyírmeggyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4731,
         "telepules": "Tunyogmatolcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4732,
         "telepules": "Cégénydányád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4733,
         "telepules": "Gyügye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4734,
         "telepules": "Szamosújlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4735,
         "telepules": "Szamossályi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4735,
         "telepules": "Hermánszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4737,
         "telepules": "Kisnamény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4737,
         "telepules": "Darnó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4741,
         "telepules": "Jánkmajtis",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4742,
         "telepules": "Csegöld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4743,
         "telepules": "Csengersima",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4745,
         "telepules": "Szamosbecs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4746,
         "telepules": "Szamostatárfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4751,
         "telepules": "Kocsord",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4752,
         "telepules": "Győrtelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4754,
         "telepules": "Géberjén",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4754,
         "telepules": "Fülpösdaróc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4755,
         "telepules": "Ököritófülpös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4756,
         "telepules": "Rápolt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4761,
         "telepules": "Porcsalma",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4762,
         "telepules": "Tyukod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4763,
         "telepules": "Ura",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4764,
         "telepules": "Csengerújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4765,
         "telepules": "Csenger",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4765,
         "telepules": "Komlódtótfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4766,
         "telepules": "Pátyod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4767,
         "telepules": "Szamosangyalos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4800,
         "telepules": "Vásárosnamény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4803,
         "telepules": "Vásárosnamény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4804,
         "telepules": "Vásárosnamény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4811,
         "telepules": "Kisvarsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4812,
         "telepules": "Nagyvarsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4813,
         "telepules": "Gyüre ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4821,
         "telepules": "Ópályi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4822,
         "telepules": "Nyírparasznya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4823,
         "telepules": "Nagydobos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4824,
         "telepules": "Szamosszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4826,
         "telepules": "Olcsva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4831,
         "telepules": "Tiszaszalka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4832,
         "telepules": "Tiszavid",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4833,
         "telepules": "Tiszaadony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4834,
         "telepules": "Tiszakerecseny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4835,
         "telepules": "Mátyus",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4836,
         "telepules": "Lónya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4841,
         "telepules": "Jánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4842,
         "telepules": "Gulács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4843,
         "telepules": "Hetefejércse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4844,
         "telepules": "Csaroda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4845,
         "telepules": "Tákos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4900,
         "telepules": "Fehérgyarmat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4911,
         "telepules": "Nábrád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4912,
         "telepules": "Kérsemjén",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4913,
         "telepules": "Panyola",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4914,
         "telepules": "Olcsvaapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4921,
         "telepules": "Kisar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4921,
         "telepules": "Tivadar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4922,
         "telepules": "Nagyar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4931,
         "telepules": "Tarpa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4932,
         "telepules": "Márokpapi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4933,
         "telepules": "Beregsurány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4934,
         "telepules": "Beregdaróc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4935,
         "telepules": "Gelénes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4936,
         "telepules": "Vámosatya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4937,
         "telepules": "Barabás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4941,
         "telepules": "Penyige",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4942,
         "telepules": "Mánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4942,
         "telepules": "Nemesborzova",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4943,
         "telepules": "Kömörő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4944,
         "telepules": "Túristvándi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4945,
         "telepules": "Szatmárcseke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4946,
         "telepules": "Tiszakóród",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4947,
         "telepules": "Tiszacsécse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4948,
         "telepules": "Milota",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4951,
         "telepules": "Tiszabecs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4952,
         "telepules": "Uszka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4953,
         "telepules": "Magosliget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4954,
         "telepules": "Sonkád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4955,
         "telepules": "Botpalád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4956,
         "telepules": "Kispalád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4961,
         "telepules": "Zsarolyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4962,
         "telepules": "Nagyszekeres",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4963,
         "telepules": "Kisszekeres",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4964,
         "telepules": "Fülesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4965,
         "telepules": "Kölcse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4966,
         "telepules": "Vámosoroszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4967,
         "telepules": "Csaholc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4968,
         "telepules": "Túrricse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4969,
         "telepules": "Tisztaberek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4971,
         "telepules": "Rozsály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4972,
         "telepules": "Gacsály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4973,
         "telepules": "Császló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4974,
         "telepules": "Zajta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4975,
         "telepules": "Méhtelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4976,
         "telepules": "Garbolc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4977,
         "telepules": "Nagyhódos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 4977,
         "telepules": "Kishódos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5000,
         "telepules": "Szolnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5008,
         "telepules": "Szolnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5051,
         "telepules": "Zagyvarékas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5052,
         "telepules": "Újszász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5053,
         "telepules": "Szászberek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5054,
         "telepules": "Jászalsószentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5055,
         "telepules": "Jászladány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5061,
         "telepules": "Tiszasüly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5062,
         "telepules": "Kőtelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5063,
         "telepules": "Hunyadfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5064,
         "telepules": "Csataszög",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5065,
         "telepules": "Nagykörű",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5071,
         "telepules": "Besenyszög",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5081,
         "telepules": "Szajol",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5082,
         "telepules": "Tiszatenyő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5083,
         "telepules": "Kengyel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5084,
         "telepules": "Rákócziújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5085,
         "telepules": "Rákóczifalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5091,
         "telepules": "Tószeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5092,
         "telepules": "Tiszavárkony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5093,
         "telepules": "Vezseny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5094,
         "telepules": "Tiszajenő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5095,
         "telepules": "Tiszavárkony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5100,
         "telepules": "Jászberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5111,
         "telepules": "Jászfelsőszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5121,
         "telepules": "Jászjákóhalma",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5122,
         "telepules": "Jászdózsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5123,
         "telepules": "Jászárokszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5124,
         "telepules": "Jászágó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5125,
         "telepules": "Pusztamonostor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5126,
         "telepules": "Jászfényszaru",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5130,
         "telepules": "Jászapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5135,
         "telepules": "Jászivány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5136,
         "telepules": "Jászszentandrás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5137,
         "telepules": "Jászkisér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5141,
         "telepules": "Jásztelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5142,
         "telepules": "Alattyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5143,
         "telepules": "Jánoshida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5144,
         "telepules": "Jászboldogháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5152,
         "telepules": "Jászberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5200,
         "telepules": "Törökszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5211,
         "telepules": "Tiszapüspöki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5212,
         "telepules": "Törökszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5213,
         "telepules": "Fegyvernek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5222,
         "telepules": "Örményes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5231,
         "telepules": "Fegyvernek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5232,
         "telepules": "Tiszabő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5233,
         "telepules": "Tiszagyenda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5234,
         "telepules": "Tiszaroff",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5235,
         "telepules": "Tiszabura",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5241,
         "telepules": "Abádszalók",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5243,
         "telepules": "Tiszaderzs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5244,
         "telepules": "Tiszaszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5300,
         "telepules": "Karcag",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5309,
         "telepules": "Berekfürdő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5310,
         "telepules": "Kisújszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5321,
         "telepules": "Kunmadaras",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5322,
         "telepules": "Tiszaszentimre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5323,
         "telepules": "Tiszaszentimre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5324,
         "telepules": "Tomajmonostora",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5331,
         "telepules": "Kenderes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5340,
         "telepules": "Kunhegyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5349,
         "telepules": "Kenderes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5350,
         "telepules": "Tiszafüred",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5358,
         "telepules": "Tiszafüred",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5359,
         "telepules": "Tiszafüred",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5361,
         "telepules": "Tiszaigar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5362,
         "telepules": "Tiszaörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5363,
         "telepules": "Nagyiván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5400,
         "telepules": "Mezőtúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5411,
         "telepules": "Kétpó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5412,
         "telepules": "Kuncsorba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5420,
         "telepules": "Túrkeve",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5430,
         "telepules": "Tiszaföldvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5435,
         "telepules": "Martfű",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5440,
         "telepules": "Kunszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5449,
         "telepules": "Kunszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5451,
         "telepules": "Öcsöd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5452,
         "telepules": "Mesterszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5453,
         "telepules": "Mezőhék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5461,
         "telepules": "Tiszaföldvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5462,
         "telepules": "Cibakháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5463,
         "telepules": "Nagyrév",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5464,
         "telepules": "Tiszainoka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5465,
         "telepules": "Cserkeszőlő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5471,
         "telepules": "Tiszakürt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5474,
         "telepules": "Tiszasas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5475,
         "telepules": "Csépa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5476,
         "telepules": "Szelevény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5500,
         "telepules": "Gyomaendrőd    ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5502,
         "telepules": "Gyomaendrőd    ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5510,
         "telepules": "Dévaványa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5515,
         "telepules": "Ecsegfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5516,
         "telepules": "Körösladány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5520,
         "telepules": "Szeghalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5525,
         "telepules": "Füzesgyarmat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5526,
         "telepules": "Kertészsziget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5527,
         "telepules": "Bucsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5530,
         "telepules": "Vésztő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5534,
         "telepules": "Okány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5536,
         "telepules": "Körösújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5537,
         "telepules": "Zsadány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5538,
         "telepules": "Biharugra",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5539,
         "telepules": "Körösnagyharsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5540,
         "telepules": "Szarvas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5551,
         "telepules": "Csabacsűd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5552,
         "telepules": "Kardos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5553,
         "telepules": "Kondoros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5555,
         "telepules": "Hunya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5556,
         "telepules": "Örménykút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5561,
         "telepules": "Békésszentandrás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5600,
         "telepules": "Békéscsaba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5609,
         "telepules": "Csabaszabadi ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5621,
         "telepules": "Csárdaszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5622,
         "telepules": "Köröstarcsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5623,
         "telepules": "Békéscsaba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5624,
         "telepules": "Doboz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5630,
         "telepules": "Békés",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5641,
         "telepules": "Tarhos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5643,
         "telepules": "Bélmegyer",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5650,
         "telepules": "Mezőberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5661,
         "telepules": "Újkígyós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5662,
         "telepules": "Csanádapáca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5663,
         "telepules": "Medgyesbodzás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5664,
         "telepules": "Medgyesbodzás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5665,
         "telepules": "Pusztaottlaka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5666,
         "telepules": "Medgyesegyháza  ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5667,
         "telepules": "Magyarbánhegyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5668,
         "telepules": "Nagybánhegyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5671,
         "telepules": "Békéscsaba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5672,
         "telepules": "Murony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5673,
         "telepules": "Kamut",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5674,
         "telepules": "Kétsoprony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5675,
         "telepules": "Telekgerendás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5700,
         "telepules": "Gyula",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5711,
         "telepules": "Gyula",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5712,
         "telepules": "Szabadkígyós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5720,
         "telepules": "Sarkad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5725,
         "telepules": "Kötegyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5726,
         "telepules": "Méhkerék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5727,
         "telepules": "Újszalonta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5731,
         "telepules": "Sarkadkeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5732,
         "telepules": "Mezőgyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5734,
         "telepules": "Geszt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5741,
         "telepules": "Kétegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5742,
         "telepules": "Elek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5743,
         "telepules": "Lőkösháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5744,
         "telepules": "Kevermes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5745,
         "telepules": "Dombiratos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5746,
         "telepules": "Kunágota",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5747,
         "telepules": "Almáskamarás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5751,
         "telepules": "Nagykamarás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5752,
         "telepules": "Medgyesegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5800,
         "telepules": "Mezőkovácsháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5811,
         "telepules": "Végegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5820,
         "telepules": "Mezőhegyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5830,
         "telepules": "Battonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5836,
         "telepules": "Dombegyház",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5837,
         "telepules": "Kisdombegyház",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5838,
         "telepules": "Magyardombegyház",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5900,
         "telepules": "Orosháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5903,
         "telepules": "Orosháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5904,
         "telepules": "Orosháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5905,
         "telepules": "Orosháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5919,
         "telepules": "Pusztaföldvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5920,
         "telepules": "Csorvás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5925,
         "telepules": "Gerendás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5931,
         "telepules": "Nagyszénás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5932,
         "telepules": "Gádoros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5940,
         "telepules": "Tótkomlós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5945,
         "telepules": "Kardoskút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5946,
         "telepules": "Békéssámson",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 5948,
         "telepules": "Kaszaper",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6000,
         "telepules": "Kecskemét",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6008,
         "telepules": "Kecskemét",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6031,
         "telepules": "Szentkirály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6032,
         "telepules": "Nyárlőrinc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6033,
         "telepules": "Városföld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6034,
         "telepules": "Helvécia",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6035,
         "telepules": "Ballószög",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6041,
         "telepules": "Kerekegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6042,
         "telepules": "Fülöpháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6043,
         "telepules": "Kunbaracs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6044,
         "telepules": "Kecskemét",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6045,
         "telepules": "Ladánybene",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6050,
         "telepules": "Lajosmizse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6055,
         "telepules": "Felsőlajos ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6060,
         "telepules": "Tiszakécske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6062,
         "telepules": "Tiszakécske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6064,
         "telepules": "Tiszaug",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6065,
         "telepules": "Lakitelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6066,
         "telepules": "Tiszaalpár ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6067,
         "telepules": "Tiszaalpár ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6070,
         "telepules": "Izsák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6075,
         "telepules": "Páhi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6076,
         "telepules": "Ágasegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6077,
         "telepules": "Orgovány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6078,
         "telepules": "Jakabszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6080,
         "telepules": "Szabadszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6085,
         "telepules": "Fülöpszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6086,
         "telepules": "Szalkszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6087,
         "telepules": "Dunavecse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6088,
         "telepules": "Apostag",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6090,
         "telepules": "Kunszentmiklós ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6096,
         "telepules": "Kunpeszér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6097,
         "telepules": "Kunadacs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6098,
         "telepules": "Tass",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6100,
         "telepules": "Kiskunfélegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6111,
         "telepules": "Gátér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6112,
         "telepules": "Pálmonostora",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6113,
         "telepules": "Petőfiszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6114,
         "telepules": "Bugac",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6114,
         "telepules": "Bugacpusztaháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6115,
         "telepules": "Kunszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6116,
         "telepules": "Fülöpjakab ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6120,
         "telepules": "Kiskunmajsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6131,
         "telepules": "Szank",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6132,
         "telepules": "Móricgát ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6133,
         "telepules": "Jászszentlászló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6134,
         "telepules": "Kömpöc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6135,
         "telepules": "Csólyospálos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6136,
         "telepules": "Harkakötöny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6200,
         "telepules": "Kiskőrös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6211,
         "telepules": "Kaskantyú",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6221,
         "telepules": "Akasztó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6222,
         "telepules": "Csengőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6223,
         "telepules": "Soltszentimre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6224,
         "telepules": "Tabdi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6230,
         "telepules": "Soltvadkert",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6235,
         "telepules": "Bócsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6236,
         "telepules": "Tázlár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6237,
         "telepules": "Kecel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6238,
         "telepules": "Imrehegy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6239,
         "telepules": "Császártöltés",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6300,
         "telepules": "Kalocsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6311,
         "telepules": "Öregcsertő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6320,
         "telepules": "Solt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6321,
         "telepules": "Újsolt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6323,
         "telepules": "Dunaegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6325,
         "telepules": "Dunatetétlen",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6326,
         "telepules": "Harta ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6327,
         "telepules": "Harta ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6328,
         "telepules": "Dunapataj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6331,
         "telepules": "Foktő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6332,
         "telepules": "Uszód",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6333,
         "telepules": "Dunaszentbenedek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6334,
         "telepules": "Géderlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6335,
         "telepules": "Ordas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6336,
         "telepules": "Szakmár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6337,
         "telepules": "Újtelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6341,
         "telepules": "Homokmégy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6342,
         "telepules": "Drágszél",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6343,
         "telepules": "Miske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6344,
         "telepules": "Hajós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6345,
         "telepules": "Nemesnádudvar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6346,
         "telepules": "Sükösd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6347,
         "telepules": "Érsekcsanád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6348,
         "telepules": "Érsekhalma",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6351,
         "telepules": "Bátya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6352,
         "telepules": "Fajsz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6353,
         "telepules": "Dusnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6400,
         "telepules": "Kiskunhalas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6411,
         "telepules": "Zsana",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6412,
         "telepules": "Balotaszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6413,
         "telepules": "Kunfehértó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6414,
         "telepules": "Pirtó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6421,
         "telepules": "Kisszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6422,
         "telepules": "Tompa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6423,
         "telepules": "Kelebia",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6424,
         "telepules": "Csikéria",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6425,
         "telepules": "Bácsszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6430,
         "telepules": "Bácsalmás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6435,
         "telepules": "Kunbaja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6440,
         "telepules": "Jánoshalma",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6444,
         "telepules": "Kéleshalom ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6445,
         "telepules": "Borota",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6446,
         "telepules": "Rém",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6447,
         "telepules": "Felsőszentiván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6448,
         "telepules": "Csávoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6449,
         "telepules": "Mélykút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6451,
         "telepules": "Tataháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6452,
         "telepules": "Mátételke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6453,
         "telepules": "Bácsbokod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6454,
         "telepules": "Bácsborsód",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6455,
         "telepules": "Katymár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6456,
         "telepules": "Madaras",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6500,
         "telepules": "Baja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6503,
         "telepules": "Baja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6511,
         "telepules": "Bácsszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6512,
         "telepules": "Szeremle",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6513,
         "telepules": "Dunafalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6521,
         "telepules": "Vaskút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6522,
         "telepules": "Gara",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6523,
         "telepules": "Csátalja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6524,
         "telepules": "Dávod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6525,
         "telepules": "Hercegszántó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6527,
         "telepules": "Nagybaracska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6528,
         "telepules": "Bátmonostor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6600,
         "telepules": "Szentes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6612,
         "telepules": "Nagytőke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6621,
         "telepules": "Derekegyház",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6622,
         "telepules": "Nagymágocs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6623,
         "telepules": "Árpádhalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6624,
         "telepules": "Eperjes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6625,
         "telepules": "Fábiánsebestyén",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6630,
         "telepules": "Mindszent",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6635,
         "telepules": "Szegvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6636,
         "telepules": "Mártély",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6640,
         "telepules": "Csongrád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6645,
         "telepules": "Felgyő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6646,
         "telepules": "Tömörkény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6647,
         "telepules": "Csanytelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6648,
         "telepules": "Csongrád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6700,
         "telepules": "Szeged",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6750,
         "telepules": "Algyő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6754,
         "telepules": "Újszentiván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6755,
         "telepules": "Kübekháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6756,
         "telepules": "Tiszasziget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6758,
         "telepules": "Röszke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6760,
         "telepules": "Kistelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6762,
         "telepules": "Sándorfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6763,
         "telepules": "Szatymaz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6764,
         "telepules": "Balástya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6765,
         "telepules": "Csengele",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6766,
         "telepules": "Dóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6767,
         "telepules": "Ópusztaszer",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6768,
         "telepules": "Baks",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6769,
         "telepules": "Pusztaszer",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6772,
         "telepules": "Deszk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6773,
         "telepules": "Klárafalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6774,
         "telepules": "Ferencszállás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6775,
         "telepules": "Kiszombor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6781,
         "telepules": "Domaszék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6782,
         "telepules": "Mórahalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6783,
         "telepules": "Ásotthalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6784,
         "telepules": "Öttömös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6785,
         "telepules": "Pusztamérges",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6786,
         "telepules": "Ruzsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6787,
         "telepules": "Zákányszék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6792,
         "telepules": "Zsombó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6793,
         "telepules": "Forráskút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6794,
         "telepules": "Üllés",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6795,
         "telepules": "Bordány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6800,
         "telepules": "Hódmezővásárhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6805,
         "telepules": "Hódmezővásárhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6806,
         "telepules": "Hódmezővásárhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6821,
         "telepules": "Székkutas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6900,
         "telepules": "Makó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6903,
         "telepules": "Makó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6911,
         "telepules": "Királyhegyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6912,
         "telepules": "Kövegy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6913,
         "telepules": "Csanádpalota",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6914,
         "telepules": "Pitvaros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6915,
         "telepules": "Csanádalberti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6916,
         "telepules": "Ambrózfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6917,
         "telepules": "Nagyér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6921,
         "telepules": "Maroslele",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6922,
         "telepules": "Földeák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6923,
         "telepules": "Óföldeák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6931,
         "telepules": "Apátfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6932,
         "telepules": "Magyarcsanád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 6933,
         "telepules": "Nagylak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7000,
         "telepules": "Sárbogárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7003,
         "telepules": "Sárbogárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7011,
         "telepules": "Alap",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7012,
         "telepules": "Alsószentiván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7013,
         "telepules": "Cece",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7014,
         "telepules": "Sáregres",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7015,
         "telepules": "Igar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7016,
         "telepules": "Igar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7017,
         "telepules": "Mezőszilas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7018,
         "telepules": "Sárbogárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7019,
         "telepules": "Sárbogárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7020,
         "telepules": "Dunaföldvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7025,
         "telepules": "Bölcske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7026,
         "telepules": "Madocsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7027,
         "telepules": "Paks",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7030,
         "telepules": "Paks",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7038,
         "telepules": "Pusztahencse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7039,
         "telepules": "Németkér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7041,
         "telepules": "Vajta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7042,
         "telepules": "Pálfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7043,
         "telepules": "Bikács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7044,
         "telepules": "Nagydorog",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7045,
         "telepules": "Györköny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7047,
         "telepules": "Sárszentlőrinc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7051,
         "telepules": "Kajdacs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7052,
         "telepules": "Kölesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7054,
         "telepules": "Tengelic",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7056,
         "telepules": "Szedres",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7057,
         "telepules": "Medina",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7061,
         "telepules": "Belecska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7062,
         "telepules": "Keszőhidegkút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7063,
         "telepules": "Szárazd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7064,
         "telepules": "Gyönk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7065,
         "telepules": "Miszla",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7066,
         "telepules": "Udvari",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7067,
         "telepules": "Varsád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7068,
         "telepules": "Kistormás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7071,
         "telepules": "Szakadát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7072,
         "telepules": "Diósberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7081,
         "telepules": "Simontornya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7082,
         "telepules": "Kisszékely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7083,
         "telepules": "Tolnanémedi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7084,
         "telepules": "Pincehely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7085,
         "telepules": "Nagyszékely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7086,
         "telepules": "Ozora",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7087,
         "telepules": "Fürged",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7090,
         "telepules": "Tamási",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7091,
         "telepules": "Pári",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7092,
         "telepules": "Nagykónyi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7093,
         "telepules": "Értény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7094,
         "telepules": "Koppányszántó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7095,
         "telepules": "Iregszemcse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7095,
         "telepules": "Újireg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7097,
         "telepules": "Nagyszokoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7098,
         "telepules": "Magyarkeszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7099,
         "telepules": "Felsőnyék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7100,
         "telepules": "Szekszárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7121,
         "telepules": "Szálka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7122,
         "telepules": "Kakasd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7130,
         "telepules": "Tolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7131,
         "telepules": "Tolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7132,
         "telepules": "Bogyiszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7133,
         "telepules": "Fadd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7134,
         "telepules": "Gerjen",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7135,
         "telepules": "Dunaszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7136,
         "telepules": "Fácánkert",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7140,
         "telepules": "Bátaszék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7142,
         "telepules": "Pörböly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7143,
         "telepules": "Őcsény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7144,
         "telepules": "Decs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7145,
         "telepules": "Sárpilis",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7146,
         "telepules": "Várdomb",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7147,
         "telepules": "Alsónána",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7148,
         "telepules": "Alsónyék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7149,
         "telepules": "Báta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7150,
         "telepules": "Bonyhád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7158,
         "telepules": "Bonyhádvarasd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7159,
         "telepules": "Kisdorog",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7161,
         "telepules": "Cikó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7162,
         "telepules": "Grábóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7163,
         "telepules": "Mőcsény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7164,
         "telepules": "Bátaapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7165,
         "telepules": "Mórágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7171,
         "telepules": "Sióagárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7172,
         "telepules": "Harc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7173,
         "telepules": "Zomba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7174,
         "telepules": "Kéty",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7175,
         "telepules": "Felsőnána",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7176,
         "telepules": "Murga",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7181,
         "telepules": "Tevel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7182,
         "telepules": "Závod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7183,
         "telepules": "Kisvejke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7184,
         "telepules": "Lengyel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7185,
         "telepules": "Mucsfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7186,
         "telepules": "Aparhant",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7186,
         "telepules": "Nagyvejke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7187,
         "telepules": "Bonyhád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7188,
         "telepules": "Szárász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7191,
         "telepules": "Hőgyész",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7192,
         "telepules": "Szakály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7193,
         "telepules": "Regöly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7194,
         "telepules": "Kalaznó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7195,
         "telepules": "Mucsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7200,
         "telepules": "Dombóvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7211,
         "telepules": "Dalmand",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7212,
         "telepules": "Kocsola",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7213,
         "telepules": "Szakcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7214,
         "telepules": "Lápafő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7214,
         "telepules": "Várong",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7215,
         "telepules": "Nak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7224,
         "telepules": "Dúzs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7225,
         "telepules": "Csibrák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7226,
         "telepules": "Kurd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7227,
         "telepules": "Gyulaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7228,
         "telepules": "Döbrököz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7251,
         "telepules": "Kapospula",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7252,
         "telepules": "Attala",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7253,
         "telepules": "Csoma",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7253,
         "telepules": "Szabadi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7255,
         "telepules": "Nagyberki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7256,
         "telepules": "Kercseliget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7257,
         "telepules": "Mosdós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7258,
         "telepules": "Baté",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7258,
         "telepules": "Kaposkeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7261,
         "telepules": "Taszár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7261,
         "telepules": "Kaposhomok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7271,
         "telepules": "Fonó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7272,
         "telepules": "Gölle",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7273,
         "telepules": "Büssü",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7274,
         "telepules": "Kazsok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7275,
         "telepules": "Igal",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7276,
         "telepules": "Somogyszil",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7276,
         "telepules": "Gadács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7279,
         "telepules": "Kisgyalán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7281,
         "telepules": "Bonnya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7282,
         "telepules": "Kisbárapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7282,
         "telepules": "Fiad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7283,
         "telepules": "Somogyacsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7284,
         "telepules": "Somogydöröcske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7285,
         "telepules": "Törökkoppány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7285,
         "telepules": "Kára",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7285,
         "telepules": "Szorosad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7300,
         "telepules": "Komló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7304,
         "telepules": "Mánfa ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7305,
         "telepules": "Mecsekpölöske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7331,
         "telepules": "Liget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7332,
         "telepules": "Magyaregregy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7333,
         "telepules": "Kárász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7333,
         "telepules": "Vékény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7334,
         "telepules": "Szalatnak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7334,
         "telepules": "Köblény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7341,
         "telepules": "Csikóstőttős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7342,
         "telepules": "Mágocs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7343,
         "telepules": "Nagyhajmás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7344,
         "telepules": "Mekényes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7345,
         "telepules": "Alsómocsolád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7346,
         "telepules": "Bikal",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7347,
         "telepules": "Egyházaskozár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7348,
         "telepules": "Hegyhátmaróc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7348,
         "telepules": "Tófű",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7349,
         "telepules": "Szászvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7351,
         "telepules": "Máza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7352,
         "telepules": "Györe",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7353,
         "telepules": "Izmény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7354,
         "telepules": "Váralja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7355,
         "telepules": "Nagymányok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7356,
         "telepules": "Kismányok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7357,
         "telepules": "Jágónak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7361,
         "telepules": "Kaposszekcső",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7362,
         "telepules": "Vásárosdombó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7362,
         "telepules": "Gerényes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7362,
         "telepules": "Tarrós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7370,
         "telepules": "Sásd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7370,
         "telepules": "Felsőegerszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7370,
         "telepules": "Meződ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7370,
         "telepules": "Oroszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7370,
         "telepules": "Palé",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7370,
         "telepules": "Varga",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7370,
         "telepules": "Vázsnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7381,
         "telepules": "Kisvaszar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7381,
         "telepules": "Ág",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7381,
         "telepules": "Tékes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7383,
         "telepules": "Tormás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7383,
         "telepules": "Baranyaszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7383,
         "telepules": "Szágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7384,
         "telepules": "Baranyajenő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7385,
         "telepules": "Gödre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7386,
         "telepules": "Gödre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7391,
         "telepules": "Mindszentgodisa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7391,
         "telepules": "Kisbeszterce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7391,
         "telepules": "Kishajmás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7393,
         "telepules": "Bakóca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7394,
         "telepules": "Magyarhertelend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7394,
         "telepules": "Bodolyabér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7396,
         "telepules": "Magyarszék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7400,
         "telepules": "Kaposvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7400,
         "telepules": "Zselickislak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7431,
         "telepules": "Juta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7432,
         "telepules": "Hetes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7432,
         "telepules": "Csombárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7434,
         "telepules": "Mezőcsokonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7435,
         "telepules": "Somogysárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7436,
         "telepules": "Újvárfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7439,
         "telepules": "Bodrog",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7441,
         "telepules": "Magyaregres",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7442,
         "telepules": "Várda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7443,
         "telepules": "Somogyjád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7443,
         "telepules": "Alsóbogát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7443,
         "telepules": "Edde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7444,
         "telepules": "Osztopán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7452,
         "telepules": "Somogyaszaló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7451,
         "telepules": "Kaposvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7453,
         "telepules": "Mernye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7454,
         "telepules": "Somodor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7455,
         "telepules": "Somogygeszti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7456,
         "telepules": "Felsőmocsolád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7457,
         "telepules": "Ecseny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7458,
         "telepules": "Polány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7461,
         "telepules": "Orci",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7463,
         "telepules": "Magyaratád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7463,
         "telepules": "Patalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7464,
         "telepules": "Ráksi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7465,
         "telepules": "Szentgáloskér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7471,
         "telepules": "Zimány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7472,
         "telepules": "Szentbalázs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7472,
         "telepules": "Cserénfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7473,
         "telepules": "Gálosfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7473,
         "telepules": "Hajmás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7473,
         "telepules": "Kaposgyarmat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7474,
         "telepules": "Simonfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7474,
         "telepules": "Zselicszentpál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7475,
         "telepules": "Bőszénfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7476,
         "telepules": "Kaposszerdahely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7477,
         "telepules": "Szenna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7477,
         "telepules": "Patca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7477,
         "telepules": "Szilvásszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7477,
         "telepules": "Zselickisfalud",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7478,
         "telepules": "Bárdudvarnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7479,
         "telepules": "Sántos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7500,
         "telepules": "Nagyatád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7511,
         "telepules": "Ötvöskónyi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7512,
         "telepules": "Mike",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7513,
         "telepules": "Rinyaszentkirály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7514,
         "telepules": "Tarany",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7515,
         "telepules": "Somogyudvarhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7516,
         "telepules": "Berzence",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7517,
         "telepules": "Bolhás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7521,
         "telepules": "Kaposmérő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7522,
         "telepules": "Kaposújlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7523,
         "telepules": "Kaposfő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7523,
         "telepules": "Kisasszond",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7524,
         "telepules": "Kiskorpád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7525,
         "telepules": "Jákó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7526,
         "telepules": "Csököly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7527,
         "telepules": "Gige",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7527,
         "telepules": "Rinyakovácsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7530,
         "telepules": "Kadarkút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7530,
         "telepules": "Kőkút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7532,
         "telepules": "Hencse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7533,
         "telepules": "Hedrehely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7533,
         "telepules": "Visnye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7535,
         "telepules": "Lad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7536,
         "telepules": "Patosfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7537,
         "telepules": "Homokszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7538,
         "telepules": "Kálmáncsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7539,
         "telepules": "Szulok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7541,
         "telepules": "Kutas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7542,
         "telepules": "Kisbajom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7543,
         "telepules": "Beleg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7544,
         "telepules": "Szabás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7545,
         "telepules": "Nagykorpád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7551,
         "telepules": "Lábod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7552,
         "telepules": "Rinyabesenyő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7553,
         "telepules": "Görgeteg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7555,
         "telepules": "Csokonyavisonta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7556,
         "telepules": "Rinyaújlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7557,
         "telepules": "Barcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7561,
         "telepules": "Nagybajom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7561,
         "telepules": "Pálmajor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7562,
         "telepules": "Segesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7563,
         "telepules": "Somogyszob",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7564,
         "telepules": "Kaszó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7570,
         "telepules": "Barcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7582,
         "telepules": "Komlósd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7582,
         "telepules": "Péterhida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7584,
         "telepules": "Babócsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7584,
         "telepules": "Rinyaújnép",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7584,
         "telepules": "Somogyaracs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7585,
         "telepules": "Háromfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7585,
         "telepules": "Bakháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7586,
         "telepules": "Bolhó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7587,
         "telepules": "Heresznye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7588,
         "telepules": "Vízvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7589,
         "telepules": "Bélavár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7600,
         "telepules": "Pécs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7639,
         "telepules": "Kökény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7661,
         "telepules": "Erzsébet",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7661,
         "telepules": "Kátoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7661,
         "telepules": "Kékesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7661,
         "telepules": "Szellő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7663,
         "telepules": "Máriakéménd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7664,
         "telepules": "Berkesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7664,
         "telepules": "Pereked",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7664,
         "telepules": "Szilágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7666,
         "telepules": "Pogány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7668,
         "telepules": "Keszü",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7668,
         "telepules": "Gyód",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7671,
         "telepules": "Bicsérd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7671,
         "telepules": "Aranyosgadány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7671,
         "telepules": "Zók",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7672,
         "telepules": "Boda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7673,
         "telepules": "Kővágószőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7673,
         "telepules": "Cserkút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7675,
         "telepules": "Bakonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7675,
         "telepules": "Kővágótöttös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7677,
         "telepules": "Orfű ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7678,
         "telepules": "Abaliget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7678,
         "telepules": "Husztót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7678,
         "telepules": "Kovácsszénája",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7681,
         "telepules": "Hetvehely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7681,
         "telepules": "Okorvölgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7681,
         "telepules": "Szentkatalin",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7682,
         "telepules": "Bükkösd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7683,
         "telepules": "Helesfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7683,
         "telepules": "Cserdi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7683,
         "telepules": "Dinnyeberki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7694,
         "telepules": "Hosszúhetény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7695,
         "telepules": "Mecseknádasd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7695,
         "telepules": "Óbánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7695,
         "telepules": "Ófalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7696,
         "telepules": "Hidas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7700,
         "telepules": "Mohács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7711,
         "telepules": "Bár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7712,
         "telepules": "Dunaszekcső",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7714,
         "telepules": "Mohács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7715,
         "telepules": "Mohács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7716,
         "telepules": "Homorúd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7717,
         "telepules": "Kölked",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7718,
         "telepules": "Udvar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7720,
         "telepules": "Pécsvárad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7720,
         "telepules": "Apátvarasd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7720,
         "telepules": "Lovászhetény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7720,
         "telepules": "Martonfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7720,
         "telepules": "Zengővárkony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7723,
         "telepules": "Erdősmecske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7724,
         "telepules": "Feked",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7725,
         "telepules": "Szebény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7726,
         "telepules": "Véménd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7727,
         "telepules": "Palotabozsok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7728,
         "telepules": "Somberek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7728,
         "telepules": "Görcsönydoboka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7731,
         "telepules": "Nagypall",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7732,
         "telepules": "Fazekasboda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7733,
         "telepules": "Geresdlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7733,
         "telepules": "Maráza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7735,
         "telepules": "Himesháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7735,
         "telepules": "Erdősmárok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7735,
         "telepules": "Szűr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7737,
         "telepules": "Székelyszabar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7741,
         "telepules": "Nagykozár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7742,
         "telepules": "Bogád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7743,
         "telepules": "Romonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7744,
         "telepules": "Ellend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7745,
         "telepules": "Olasz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7745,
         "telepules": "Hásságy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7747,
         "telepules": "Belvárdgyula",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7747,
         "telepules": "Birján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7751,
         "telepules": "Szederkény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7751,
         "telepules": "Monyoród",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7752,
         "telepules": "Versend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7753,
         "telepules": "Szajk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7754,
         "telepules": "Bóly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7755,
         "telepules": "Töttös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7756,
         "telepules": "Borjád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7756,
         "telepules": "Kisbudmér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7756,
         "telepules": "Nagybudmér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7756,
         "telepules": "Pócsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7757,
         "telepules": "Babarc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7757,
         "telepules": "Liptód",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7759,
         "telepules": "Lánycsók",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7759,
         "telepules": "Kisnyárád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7761,
         "telepules": "Kozármisleny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7761,
         "telepules": "Lothárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7761,
         "telepules": "Magyarsarlós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7762,
         "telepules": "Pécsudvard",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7763,
         "telepules": "Egerág",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7763,
         "telepules": "Áta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7763,
         "telepules": "Kisherend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7763,
         "telepules": "Szemely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7763,
         "telepules": "Szőkéd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7766,
         "telepules": "Újpetre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7766,
         "telepules": "Kiskassa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7766,
         "telepules": "Peterd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7766,
         "telepules": "Pécsdevecser",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7768,
         "telepules": "Vokány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7768,
         "telepules": "Kistótfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7771,
         "telepules": "Palkonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7772,
         "telepules": "Villánykövesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7772,
         "telepules": "Ivánbattyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7773,
         "telepules": "Villány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7773,
         "telepules": "Kisjakabfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7774,
         "telepules": "Márok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7775,
         "telepules": "Magyarbóly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7775,
         "telepules": "Illocska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7775,
         "telepules": "Kislippó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7775,
         "telepules": "Lapáncsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7781,
         "telepules": "Lippó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7781,
         "telepules": "Ivándárda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7781,
         "telepules": "Sárok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7782,
         "telepules": "Bezedek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7783,
         "telepules": "Majs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7784,
         "telepules": "Nagynyárád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7785,
         "telepules": "Sátorhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7800,
         "telepules": "Siklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7800,
         "telepules": "Kisharsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7800,
         "telepules": "Nagytótfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7811,
         "telepules": "Szalánta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7811,
         "telepules": "Bisse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7811,
         "telepules": "Bosta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7811,
         "telepules": "Csarnóta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7811,
         "telepules": "Szilvás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7811,
         "telepules": "Túrony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7812,
         "telepules": "Garé",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7813,
         "telepules": "Szava",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7814,
         "telepules": "Ócsárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7814,
         "telepules": "Babarcszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7814,
         "telepules": "Kisdér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7814,
         "telepules": "Siklósbodony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7815,
         "telepules": "Harkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7817,
         "telepules": "Diósviszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7817,
         "telepules": "Márfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7817,
         "telepules": "Rádfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7822,
         "telepules": "Nagyharsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7823,
         "telepules": "Siklósnagyfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7823,
         "telepules": "Kistapolca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7824,
         "telepules": "Egyházasharaszti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7825,
         "telepules": "Old",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7826,
         "telepules": "Alsószentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7827,
         "telepules": "Beremend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7827,
         "telepules": "Kásád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7831,
         "telepules": "Pellérd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7833,
         "telepules": "Görcsöny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7833,
         "telepules": "Regenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7833,
         "telepules": "Szőke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7834,
         "telepules": "Baksa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7834,
         "telepules": "Tengeri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7834,
         "telepules": "Téseny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7836,
         "telepules": "Bogádmindszent",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7836,
         "telepules": "Ózdfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7837,
         "telepules": "Hegyszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7838,
         "telepules": "Vajszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7838,
         "telepules": "Besence",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7838,
         "telepules": "Hirics",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7838,
         "telepules": "Lúzsok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7838,
         "telepules": "Nagycsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7838,
         "telepules": "Páprád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7838,
         "telepules": "Piskó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7838,
         "telepules": "Vejti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7839,
         "telepules": "Zaláta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7839,
         "telepules": "Kemse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7841,
         "telepules": "Sámod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7841,
         "telepules": "Adorjás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7841,
         "telepules": "Baranyahídvég",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7841,
         "telepules": "Kisszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7841,
         "telepules": "Kórós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7843,
         "telepules": "Kémes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7843,
         "telepules": "Cún",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7843,
         "telepules": "Drávapiski",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7843,
         "telepules": "Szaporca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7843,
         "telepules": "Tésenfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7846,
         "telepules": "Drávacsepely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7847,
         "telepules": "Kovácshida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7847,
         "telepules": "Drávaszerdahely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7847,
         "telepules": "Ipacsfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7849,
         "telepules": "Drávacsehi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7850,
         "telepules": "Drávapalkonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7851,
         "telepules": "Drávaszabolcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7853,
         "telepules": "Gordisa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7854,
         "telepules": "Matty",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7900,
         "telepules": "Szigetvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7900,
         "telepules": "Botykapeterd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7900,
         "telepules": "Csertő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7912,
         "telepules": "Nagypeterd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7912,
         "telepules": "Nyugotszenterzsébet",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7912,
         "telepules": "Nagyváty",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7913,
         "telepules": "Szentdénes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7914,
         "telepules": "Rózsafa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7914,
         "telepules": "Bánfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7914,
         "telepules": "Katádfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7915,
         "telepules": "Dencsháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7915,
         "telepules": "Szentegát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7918,
         "telepules": "Lakócsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7918,
         "telepules": "Szentborbás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7918,
         "telepules": "Tótújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7921,
         "telepules": "Somogyhatvan",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7922,
         "telepules": "Somogyapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7923,
         "telepules": "Basal",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7923,
         "telepules": "Patapoklosi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7924,
         "telepules": "Somogyviszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7925,
         "telepules": "Somogyhárságy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7925,
         "telepules": "Magyarlukafa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7926,
         "telepules": "Vásárosbéc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7932,
         "telepules": "Mozsgó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7932,
         "telepules": "Almáskeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7932,
         "telepules": "Szulimán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7934,
         "telepules": "Almamellék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7935,
         "telepules": "Ibafa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7935,
         "telepules": "Csebény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7935,
         "telepules": "Horváthertelend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7936,
         "telepules": "Szentlászló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7937,
         "telepules": "Boldogasszonyfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7940,
         "telepules": "Szentlőrinc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7940,
         "telepules": "Csonkamindszent",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7940,
         "telepules": "Kacsóta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7951,
         "telepules": "Szabadszentkirály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7951,
         "telepules": "Gerde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7951,
         "telepules": "Pécsbagota",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7951,
         "telepules": "Velény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7953,
         "telepules": "Királyegyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7954,
         "telepules": "Magyarmecske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7954,
         "telepules": "Gilvánfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7954,
         "telepules": "Gyöngyfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7954,
         "telepules": "Kisasszonyfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7954,
         "telepules": "Magyartelek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7957,
         "telepules": "Okorág ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7958,
         "telepules": "Kákics ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7960,
         "telepules": "Sellye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7960,
         "telepules": "Drávaiványi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7960,
         "telepules": "Drávasztára",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7960,
         "telepules": "Marócsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7960,
         "telepules": "Sósvertike",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7960,
         "telepules": "Sumony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7964,
         "telepules": "Csányoszró",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7966,
         "telepules": "Bogdása",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7967,
         "telepules": "Drávafok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7967,
         "telepules": "Drávakeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7967,
         "telepules": "Markóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7968,
         "telepules": "Felsőszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7971,
         "telepules": "Hobol",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7972,
         "telepules": "Gyöngyösmellék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7973,
         "telepules": "Teklafalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7973,
         "telepules": "Bürüs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7973,
         "telepules": "Endrőc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7973,
         "telepules": "Várad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7975,
         "telepules": "Kétújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7976,
         "telepules": "Zádor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7976,
         "telepules": "Szörény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7977,
         "telepules": "Kastélyosdombó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7977,
         "telepules": "Drávagárdony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7977,
         "telepules": "Potony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7979,
         "telepules": "Drávatamási",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7980,
         "telepules": "Pettend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7981,
         "telepules": "Nemeske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7981,
         "telepules": "Kistamási",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7981,
         "telepules": "Merenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7981,
         "telepules": "Molvány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7981,
         "telepules": "Tótszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7985,
         "telepules": "Nagydobsza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7985,
         "telepules": "Kisdobsza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7987,
         "telepules": "Istvándi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 7988,
         "telepules": "Darány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8000,
         "telepules": "Székesfehérvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8019,
         "telepules": "Székesfehérvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8041,
         "telepules": "Csór",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8042,
         "telepules": "Moha",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8043,
         "telepules": "Iszkaszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8044,
         "telepules": "Kincsesbánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8045,
         "telepules": "Isztimér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8046,
         "telepules": "Bakonykúti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8051,
         "telepules": "Sárkeresztes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8052,
         "telepules": "Fehérvárcsurgó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8053,
         "telepules": "Bodajk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8054,
         "telepules": "Balinka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8055,
         "telepules": "Balinka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8056,
         "telepules": "Bakonycsernye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8060,
         "telepules": "Mór",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8065,
         "telepules": "Nagyveleg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8066,
         "telepules": "Pusztavám",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8071,
         "telepules": "Magyaralmás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8072,
         "telepules": "Söréd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8073,
         "telepules": "Csákberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8074,
         "telepules": "Csókakő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8080,
         "telepules": "Bodmér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8081,
         "telepules": "Zámoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8082,
         "telepules": "Gánt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8083,
         "telepules": "Csákvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8085,
         "telepules": "Vértesboglár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8086,
         "telepules": "Felcsút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8087,
         "telepules": "Alcsútdoboz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8088,
         "telepules": "Tabajd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8089,
         "telepules": "Vértesacsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8092,
         "telepules": "Pátka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8093,
         "telepules": "Lovasberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8095,
         "telepules": "Pákozd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8096,
         "telepules": "Sukoró",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8097,
         "telepules": "Nadap",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8100,
         "telepules": "Várpalota",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8105,
         "telepules": "Pétfürdő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8109,
         "telepules": "Tés",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8111,
         "telepules": "Seregélyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8112,
         "telepules": "Zichyújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8121,
         "telepules": "Tác",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8122,
         "telepules": "Csősz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8123,
         "telepules": "Soponya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8124,
         "telepules": "Káloz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8125,
         "telepules": "Sárkeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8126,
         "telepules": "Sárszentágota",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8127,
         "telepules": "Aba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8130,
         "telepules": "Enying",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8131,
         "telepules": "Enying",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8132,
         "telepules": "Lepsény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8133,
         "telepules": "Mezőszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8134,
         "telepules": "Mátyásdomb",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8135,
         "telepules": "Dég",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8136,
         "telepules": "Lajoskomárom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8137,
         "telepules": "Mezőkomárom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8138,
         "telepules": "Szabadhídvég",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8139,
         "telepules": "Szabadhídvég",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8142,
         "telepules": "Úrhida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8143,
         "telepules": "Sárszentmihály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8144,
         "telepules": "Sárkeszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8145,
         "telepules": "Nádasdladány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8146,
         "telepules": "Jenő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8151,
         "telepules": "Szabadbattyán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8152,
         "telepules": "Kőszárhegy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8154,
         "telepules": "Polgárdi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8156,
         "telepules": "Kisláng",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8157,
         "telepules": "Füle",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8161,
         "telepules": "Ősi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8162,
         "telepules": "Küngös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8163,
         "telepules": "Csajág",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8164,
         "telepules": "Balatonfőkajár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8171,
         "telepules": "Balatonvilágos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8172,
         "telepules": "Balatonakarattya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8174,
         "telepules": "Balatonkenese",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8175,
         "telepules": "Balatonfűzfő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8181,
         "telepules": "Berhida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8182,
         "telepules": "Berhida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8183,
         "telepules": "Papkeszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8184,
         "telepules": "Balatonfűzfő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8191,
         "telepules": "Öskü",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8192,
         "telepules": "Hajmáskér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8193,
         "telepules": "Sóly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8194,
         "telepules": "Vilonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8195,
         "telepules": "Királyszentistván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8196,
         "telepules": "Litér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8200,
         "telepules": "Veszprém",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8220,
         "telepules": "Balatonalmádi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8225,
         "telepules": "Szentkirályszabadja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8226,
         "telepules": "Alsóörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8227,
         "telepules": "Felsőörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8228,
         "telepules": "Lovas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8229,
         "telepules": "Csopak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8229,
         "telepules": "Paloznak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8230,
         "telepules": "Balatonfüred",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8233,
         "telepules": "Balatonszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8237,
         "telepules": "Tihany",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8241,
         "telepules": "Aszófő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8242,
         "telepules": "Balatonudvari",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8242,
         "telepules": "Örvényes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8243,
         "telepules": "Balatonakali",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8244,
         "telepules": "Dörgicse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8245,
         "telepules": "Pécsely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8245,
         "telepules": "Vászoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8246,
         "telepules": "Tótvázsony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8247,
         "telepules": "Hidegkút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8248,
         "telepules": "Nemesvámos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8248,
         "telepules": "Veszprémfajsz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8251,
         "telepules": "Zánka ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8252,
         "telepules": "Balatonszepezd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8253,
         "telepules": "Révfülöp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8254,
         "telepules": "Kővágóörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8254,
         "telepules": "Kékkút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8255,
         "telepules": "Balatonrendes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8255,
         "telepules": "Kővágóörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8256,
         "telepules": "Ábrahámhegy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8256,
         "telepules": "Salföld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8257,
         "telepules": "Badacsonytomaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8258,
         "telepules": "Badacsonytomaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8261,
         "telepules": "Badacsonytomaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8263,
         "telepules": "Badacsonytördemic",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8264,
         "telepules": "Szigliget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8265,
         "telepules": "Hegymagas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8271,
         "telepules": "Mencshely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8272,
         "telepules": "Szentantalfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8272,
         "telepules": "Balatoncsicsó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8272,
         "telepules": "Óbudavár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8272,
         "telepules": "Szentjakabfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8272,
         "telepules": "Tagyon",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8273,
         "telepules": "Monoszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8274,
         "telepules": "Köveskál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8275,
         "telepules": "Balatonhenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8281,
         "telepules": "Szentbékkálla",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8282,
         "telepules": "Mindszentkálla",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8283,
         "telepules": "Káptalantóti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8284,
         "telepules": "Nemesgulács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8284,
         "telepules": "Kisapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8286,
         "telepules": "Gyulakeszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8291,
         "telepules": "Nagyvázsony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8291,
         "telepules": "Barnag",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8291,
         "telepules": "Pula",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8291,
         "telepules": "Vöröstó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8292,
         "telepules": "Öcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8294,
         "telepules": "Kapolcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8294,
         "telepules": "Vigántpetend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8295,
         "telepules": "Taliándörögd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8296,
         "telepules": "Monostorapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8296,
         "telepules": "Hegyesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8297,
         "telepules": "Tapolca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8300,
         "telepules": "Tapolca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8300,
         "telepules": "Raposka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8308,
         "telepules": "Zalahaláp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8308,
         "telepules": "Sáska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8311,
         "telepules": "Nemesvita",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8312,
         "telepules": "Balatonederics",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8313,
         "telepules": "Balatongyörök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8314,
         "telepules": "Vonyarcvashegy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8315,
         "telepules": "Gyenesdiás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8316,
         "telepules": "Várvölgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8316,
         "telepules": "Vállus",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8317,
         "telepules": "Lesencefalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8318,
         "telepules": "Lesencetomaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8319,
         "telepules": "Lesenceistvánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8321,
         "telepules": "Uzsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8330,
         "telepules": "Sümeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8341,
         "telepules": "Mihályfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8341,
         "telepules": "Kisvásárhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8341,
         "telepules": "Szalapa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8342,
         "telepules": "Óhíd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8344,
         "telepules": "Zalaerdőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8344,
         "telepules": "Hetyefő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8345,
         "telepules": "Dabronc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8346,
         "telepules": "Gógánfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8347,
         "telepules": "Ukk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8348,
         "telepules": "Rigács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8348,
         "telepules": "Megyer",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8348,
         "telepules": "Zalameggyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8349,
         "telepules": "Zalagyömörő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8351,
         "telepules": "Sümegprága",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8352,
         "telepules": "Bazsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8353,
         "telepules": "Zalaszántó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8353,
         "telepules": "Vindornyalak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8354,
         "telepules": "Karmacs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8354,
         "telepules": "Vindornyafok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8354,
         "telepules": "Zalaköveskút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8355,
         "telepules": "Vindornyaszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8356,
         "telepules": "Kisgörbő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8356,
         "telepules": "Nagygörbő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8357,
         "telepules": "Sümegcsehi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8357,
         "telepules": "Döbröce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8360,
         "telepules": "Keszthely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8371,
         "telepules": "Nemesbük",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8372,
         "telepules": "Cserszegtomaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8373,
         "telepules": "Rezi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8380,
         "telepules": "Hévíz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8391,
         "telepules": "Sármellék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8392,
         "telepules": "Zalavár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8393,
         "telepules": "Szentgyörgyvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8394,
         "telepules": "Alsópáhok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8395,
         "telepules": "Felsőpáhok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8400,
         "telepules": "Ajka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8409,
         "telepules": "Úrkút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8411,
         "telepules": "Veszprém",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8412,
         "telepules": "Veszprém",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8413,
         "telepules": "Eplény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8414,
         "telepules": "Olaszfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8415,
         "telepules": "Nagyesztergár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8416,
         "telepules": "Dudar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8417,
         "telepules": "Csetény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8418,
         "telepules": "Bakonyoszlop",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8419,
         "telepules": "Csesznek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8420,
         "telepules": "Zirc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8422,
         "telepules": "Bakonynána",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8423,
         "telepules": "Szápár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8424,
         "telepules": "Jásd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8425,
         "telepules": "Lókút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8426,
         "telepules": "Pénzesgyőr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8427,
         "telepules": "Bakonybél",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8428,
         "telepules": "Borzavár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8429,
         "telepules": "Porva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8430,
         "telepules": "Bakonyszentkirály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8431,
         "telepules": "Bakonyszentlászló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8432,
         "telepules": "Fenyőfő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8433,
         "telepules": "Bakonygyirót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8434,
         "telepules": "Románd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8435,
         "telepules": "Gic",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8438,
         "telepules": "Veszprémvarsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8439,
         "telepules": "Sikátor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8440,
         "telepules": "Herend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8441,
         "telepules": "Márkó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8442,
         "telepules": "Hárskút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8443,
         "telepules": "Bánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8444,
         "telepules": "Szentgál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8445,
         "telepules": "Városlőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8445,
         "telepules": "Csehbánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8446,
         "telepules": "Kislőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8447,
         "telepules": "Ajka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8448,
         "telepules": "Ajka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8449,
         "telepules": "Magyarpolány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8451,
         "telepules": "Ajka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8452,
         "telepules": "Halimba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8452,
         "telepules": "Szőc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8454,
         "telepules": "Nyirád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8455,
         "telepules": "Pusztamiske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8456,
         "telepules": "Noszlop",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8457,
         "telepules": "Bakonypölöske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8458,
         "telepules": "Oroszi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8460,
         "telepules": "Devecser",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8468,
         "telepules": "Kolontár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8469,
         "telepules": "Kamond",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8471,
         "telepules": "Káptalanfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8471,
         "telepules": "Bodorfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8471,
         "telepules": "Nemeshany",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8473,
         "telepules": "Gyepükaján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8474,
         "telepules": "Csabrendek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8475,
         "telepules": "Veszprémgalsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8475,
         "telepules": "Hosztót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8475,
         "telepules": "Szentimrefalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8476,
         "telepules": "Zalaszegvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8477,
         "telepules": "Tüskevár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8477,
         "telepules": "Apácatorna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8477,
         "telepules": "Kisberzseny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8478,
         "telepules": "Somlójenő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8479,
         "telepules": "Borszörcsök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8481,
         "telepules": "Somlóvásárhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8482,
         "telepules": "Doba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8483,
         "telepules": "Somlószőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8483,
         "telepules": "Kisszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8484,
         "telepules": "Nagyalásony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8484,
         "telepules": "Somlóvecse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8484,
         "telepules": "Vid",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8485,
         "telepules": "Dabrony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8491,
         "telepules": "Karakószörcsök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8492,
         "telepules": "Kerta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8493,
         "telepules": "Iszkáz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8494,
         "telepules": "Kiscsősz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8495,
         "telepules": "Csögle",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8496,
         "telepules": "Nagypirit",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8496,
         "telepules": "Kispirit",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8497,
         "telepules": "Adorjánháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8497,
         "telepules": "Egeralja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8500,
         "telepules": "Pápa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8511,
         "telepules": "Pápa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8512,
         "telepules": "Nyárád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8513,
         "telepules": "Mihályháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8514,
         "telepules": "Mezőlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8515,
         "telepules": "Békás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8516,
         "telepules": "Kemeneshőgyész",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8517,
         "telepules": "Magyargencs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8518,
         "telepules": "Kemenesszentpéter",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8521,
         "telepules": "Nagyacsád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8522,
         "telepules": "Nemesgörzsöny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8523,
         "telepules": "Egyházaskesző",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8523,
         "telepules": "Várkesző",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8531,
         "telepules": "Marcaltő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8532,
         "telepules": "Marcaltő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8533,
         "telepules": "Malomsok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8541,
         "telepules": "Takácsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8542,
         "telepules": "Vaszar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8543,
         "telepules": "Gecse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8551,
         "telepules": "Nagygyimót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8552,
         "telepules": "Vanyola",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8553,
         "telepules": "Lovászpatona",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8554,
         "telepules": "Nagydém",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8555,
         "telepules": "Bakonytamási",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8556,
         "telepules": "Pápateszér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8557,
         "telepules": "Bakonyszentiván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8557,
         "telepules": "Bakonyság",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8558,
         "telepules": "Csót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8561,
         "telepules": "Adásztevel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8562,
         "telepules": "Nagytevel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8563,
         "telepules": "Homokbödöge",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8564,
         "telepules": "Ugod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8565,
         "telepules": "Béb",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8571,
         "telepules": "Bakonykoppány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8572,
         "telepules": "Bakonyszücs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8581,
         "telepules": "Bakonyjákó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8581,
         "telepules": "Németbánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8582,
         "telepules": "Farkasgyepű",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8591,
         "telepules": "Pápa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8591,
         "telepules": "Nóráp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8592,
         "telepules": "Dáka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8593,
         "telepules": "Pápadereske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8594,
         "telepules": "Pápasalamon",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8595,
         "telepules": "Kup",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8596,
         "telepules": "Pápakovácsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8597,
         "telepules": "Ganna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8597,
         "telepules": "Döbrönte",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8598,
         "telepules": "Pápa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8600,
         "telepules": "Siófok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8612,
         "telepules": "Nyim",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8613,
         "telepules": "Balatonendréd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8614,
         "telepules": "Bálványos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8617,
         "telepules": "Kőröshegy ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8618,
         "telepules": "Kereki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8619,
         "telepules": "Pusztaszemes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8621,
         "telepules": "Zamárdi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8622,
         "telepules": "Szántód",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8623,
         "telepules": "Balatonföldvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8624,
         "telepules": "Balatonszárszó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8625,
         "telepules": "Szólád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8626,
         "telepules": "Teleki",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8627,
         "telepules": "Kötcse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8628,
         "telepules": "Nagycsepely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8630,
         "telepules": "Balatonboglár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8635,
         "telepules": "Ordacsehi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8636,
         "telepules": "Balatonszemes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8637,
         "telepules": "Balatonőszöd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8638,
         "telepules": "Balatonlelle",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8640,
         "telepules": "Fonyód",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8646,
         "telepules": "Balatonfenyves",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8647,
         "telepules": "Balatonmáriafürdő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8648,
         "telepules": "Balatonkeresztúr ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8649,
         "telepules": "Balatonberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8651,
         "telepules": "Balatonszabadi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8652,
         "telepules": "Siójut",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8653,
         "telepules": "Ádánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8654,
         "telepules": "Ságvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8655,
         "telepules": "Som",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8656,
         "telepules": "Nagyberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8658,
         "telepules": "Bábonymegyer",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8660,
         "telepules": "Tab",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8660,
         "telepules": "Lulla",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8660,
         "telepules": "Sérsekszőlős",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8660,
         "telepules": "Torvaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8660,
         "telepules": "Zala",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8666,
         "telepules": "Bedegkér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8666,
         "telepules": "Somogyegres",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8667,
         "telepules": "Kánya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8668,
         "telepules": "Tengőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8669,
         "telepules": "Miklósi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8671,
         "telepules": "Kapoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8672,
         "telepules": "Zics",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8673,
         "telepules": "Somogymeggyes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8674,
         "telepules": "Nágocs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8675,
         "telepules": "Andocs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8676,
         "telepules": "Karád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8681,
         "telepules": "Látrány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8681,
         "telepules": "Visz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8683,
         "telepules": "Somogytúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8684,
         "telepules": "Somogybabod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8685,
         "telepules": "Gamás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8691,
         "telepules": "Balatonboglár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8692,
         "telepules": "Szőlősgyörök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8692,
         "telepules": "Gyugy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8693,
         "telepules": "Lengyeltóti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8693,
         "telepules": "Kisberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8694,
         "telepules": "Hács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8695,
         "telepules": "Buzsák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8696,
         "telepules": "Táska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8697,
         "telepules": "Öreglak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8698,
         "telepules": "Somogyvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8698,
         "telepules": "Pamuk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8699,
         "telepules": "Somogyvámos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8700,
         "telepules": "Marcali",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8700,
         "telepules": "Csömend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8705,
         "telepules": "Somogyszentpál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8706,
         "telepules": "Nikla",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8707,
         "telepules": "Pusztakovácsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8707,
         "telepules": "Libickozma",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8708,
         "telepules": "Somogyfajsz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8709,
         "telepules": "Marcali",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8710,
         "telepules": "Balatonszentgyörgy ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8711,
         "telepules": "Vörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8712,
         "telepules": "Balatonújlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8713,
         "telepules": "Kéthely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8714,
         "telepules": "Marcali",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8714,
         "telepules": "Kelevíz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8715,
         "telepules": "Gadány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8716,
         "telepules": "Mesztegnyő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8716,
         "telepules": "Hosszúvíz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8717,
         "telepules": "Szenyér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8717,
         "telepules": "Nemeskisfalud",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8718,
         "telepules": "Tapsony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8719,
         "telepules": "Böhönye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8721,
         "telepules": "Vése",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8722,
         "telepules": "Nemesdéd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8723,
         "telepules": "Varászló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8724,
         "telepules": "Inke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8725,
         "telepules": "Iharosberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8726,
         "telepules": "Iharos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8726,
         "telepules": "Somogycsicsó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8728,
         "telepules": "Pogányszentpéter",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8731,
         "telepules": "Hollád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8731,
         "telepules": "Tikos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8732,
         "telepules": "Sávoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8732,
         "telepules": "Főnyed",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8732,
         "telepules": "Szegerdő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8733,
         "telepules": "Somogysámson",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8734,
         "telepules": "Somogyzsitfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8735,
         "telepules": "Csákány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8736,
         "telepules": "Szőkedencs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8737,
         "telepules": "Somogysimonyi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8738,
         "telepules": "Nemesvid",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8739,
         "telepules": "Nagyszakácsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8741,
         "telepules": "Zalaapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8741,
         "telepules": "Bókaháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8742,
         "telepules": "Esztergályhorváti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8743,
         "telepules": "Zalaszabar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8744,
         "telepules": "Orosztony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8745,
         "telepules": "Kerecseny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8746,
         "telepules": "Nagyrada",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8747,
         "telepules": "Garabonc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8747,
         "telepules": "Zalamerenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8749,
         "telepules": "Zalakaros",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8751,
         "telepules": "Zalakomár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8752,
         "telepules": "Zalakomár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8753,
         "telepules": "Balatonmagyaród",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8754,
         "telepules": "Galambok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8756,
         "telepules": "Nagyrécse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8756,
         "telepules": "Csapi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8756,
         "telepules": "Kisrécse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8756,
         "telepules": "Zalasárszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8761,
         "telepules": "Pacsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8761,
         "telepules": "Zalaigrice",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8762,
         "telepules": "Szentpéterúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8762,
         "telepules": "Gétye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8764,
         "telepules": "Dióskál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8764,
         "telepules": "Zalaszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8765,
         "telepules": "Egeraracsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8767,
         "telepules": "Felsőrajk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8767,
         "telepules": "Alsórajk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8767,
         "telepules": "Pötréte",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8771,
         "telepules": "Hahót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8772,
         "telepules": "Zalaszentbalázs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8772,
         "telepules": "Börzönce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8773,
         "telepules": "Pölöskefő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8773,
         "telepules": "Kacorlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8774,
         "telepules": "Gelse",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8774,
         "telepules": "Gelsesziget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8774,
         "telepules": "Kilimán",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8776,
         "telepules": "Magyarszerdahely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8776,
         "telepules": "Bocska",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8776,
         "telepules": "Magyarszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8777,
         "telepules": "Hosszúvölgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8777,
         "telepules": "Fűzvölgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8777,
         "telepules": "Homokkomárom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8778,
         "telepules": "Újudvar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8782,
         "telepules": "Zalacsány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8782,
         "telepules": "Ligetfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8782,
         "telepules": "Tilaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8784,
         "telepules": "Kehidakustány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8785,
         "telepules": "Zalaszentgrót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8785,
         "telepules": "Kallósd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8788,
         "telepules": "Zalaszentlászló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8788,
         "telepules": "Sénye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8789,
         "telepules": "Zalaszentgrót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8790,
         "telepules": "Zalaszentgrót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8792,
         "telepules": "Zalavég",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8793,
         "telepules": "Tekenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8795,
         "telepules": "Zalaszentgrót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8796,
         "telepules": "Türje",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8797,
         "telepules": "Batyk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8798,
         "telepules": "Zalabér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8799,
         "telepules": "Pakod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8799,
         "telepules": "Dötk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8800,
         "telepules": "Nagykanizsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8808,
         "telepules": "Nagykanizsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8809,
         "telepules": "Nagykanizsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8821,
         "telepules": "Nagybakónak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8822,
         "telepules": "Zalaújlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8824,
         "telepules": "Sand",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8825,
         "telepules": "Miháld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8825,
         "telepules": "Pat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8827,
         "telepules": "Zalaszentjakab",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8831,
         "telepules": "Nagykanizsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8832,
         "telepules": "Liszó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8834,
         "telepules": "Murakeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8835,
         "telepules": "Fityeház",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8840,
         "telepules": "Csurgó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8840,
         "telepules": "Csurgónagymarton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8849,
         "telepules": "Szenta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8851,
         "telepules": "Gyékényes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8852,
         "telepules": "Zákány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8853,
         "telepules": "Zákányfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8854,
         "telepules": "Őrtilos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8855,
         "telepules": "Belezna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8856,
         "telepules": "Surd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8857,
         "telepules": "Nemespátró",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8858,
         "telepules": "Porrog",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8858,
         "telepules": "Porrogszentkirály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8858,
         "telepules": "Porrogszentpál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8858,
         "telepules": "Somogybükkösd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8861,
         "telepules": "Szepetnek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8862,
         "telepules": "Semjénháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8863,
         "telepules": "Molnári",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8864,
         "telepules": "Tótszerdahely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8865,
         "telepules": "Tótszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8866,
         "telepules": "Becsehely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8866,
         "telepules": "Petrivente",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8868,
         "telepules": "Letenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8868,
         "telepules": "Kistolmács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8868,
         "telepules": "Murarátka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8868,
         "telepules": "Zajk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8872,
         "telepules": "Muraszemenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8872,
         "telepules": "Szentmargitfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8873,
         "telepules": "Csörnyeföld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8874,
         "telepules": "Dobri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8874,
         "telepules": "Kerkaszentkirály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8876,
         "telepules": "Tormafölde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8877,
         "telepules": "Tornyiszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8878,
         "telepules": "Lovászi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8879,
         "telepules": "Szécsisziget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8879,
         "telepules": "Kerkateskánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8881,
         "telepules": "Sormás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8882,
         "telepules": "Eszteregnye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8883,
         "telepules": "Rigyác",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8885,
         "telepules": "Borsfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8885,
         "telepules": "Valkonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8886,
         "telepules": "Oltárc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8887,
         "telepules": "Bázakerettye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8887,
         "telepules": "Lasztonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8888,
         "telepules": "Lispeszentadorján",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8888,
         "telepules": "Kiscsehi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8888,
         "telepules": "Maróc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8891,
         "telepules": "Bánokszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8891,
         "telepules": "Várfölde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8893,
         "telepules": "Szentliszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8893,
         "telepules": "Bucsuta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8895,
         "telepules": "Pusztamagyaród",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8896,
         "telepules": "Pusztaszentlászló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8897,
         "telepules": "Söjtör",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8900,
         "telepules": "Zalaegerszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8904,
         "telepules": "Zalaegerszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8911,
         "telepules": "Nagykutas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8911,
         "telepules": "Kiskutas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8912,
         "telepules": "Kispáli",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8912,
         "telepules": "Nagypáli",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8913,
         "telepules": "Egervár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8913,
         "telepules": "Gősfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8913,
         "telepules": "Lakhegy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8914,
         "telepules": "Vasboldogasszony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8915,
         "telepules": "Nemesrádó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8917,
         "telepules": "Milejszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8918,
         "telepules": "Csonkahegyhát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8918,
         "telepules": "Németfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8919,
         "telepules": "Kustánszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8921,
         "telepules": "Zalaszentiván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8921,
         "telepules": "Alibánfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8921,
         "telepules": "Pethőhenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8921,
         "telepules": "Zalaszentlőrinc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8923,
         "telepules": "Nemesapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8924,
         "telepules": "Alsónemesapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8925,
         "telepules": "Búcsúszentlászló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8925,
         "telepules": "Nemessándorháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8925,
         "telepules": "Nemesszentandrás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8926,
         "telepules": "Kisbucsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8928,
         "telepules": "Nemeshetés",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8929,
         "telepules": "Pölöske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8931,
         "telepules": "Kemendollár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8931,
         "telepules": "Vöckönd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8932,
         "telepules": "Pókaszepetk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8932,
         "telepules": "Gyűrűs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8932,
         "telepules": "Zalaistvánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8934,
         "telepules": "Bezeréd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8935,
         "telepules": "Nagykapornak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8935,
         "telepules": "Almásháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8935,
         "telepules": "Misefa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8935,
         "telepules": "Orbányosfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8935,
         "telepules": "Padár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8936,
         "telepules": "Zalaszentmihály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8943,
         "telepules": "Bocfölde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8943,
         "telepules": "Csatár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8944,
         "telepules": "Sárhida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8945,
         "telepules": "Bak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8946,
         "telepules": "Tófej",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8946,
         "telepules": "Baktüttös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8946,
         "telepules": "Pusztaederics",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8947,
         "telepules": "Zalatárnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8947,
         "telepules": "Szentkozmadombja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8948,
         "telepules": "Nova",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8948,
         "telepules": "Barlahida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8949,
         "telepules": "Mikekarácsonyfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8951,
         "telepules": "Gutorfölde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8951,
         "telepules": "Csertalakos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8953,
         "telepules": "Szentpéterfölde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8954,
         "telepules": "Ortaháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8956,
         "telepules": "Páka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8956,
         "telepules": "Kányavár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8956,
         "telepules": "Pördefölde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8957,
         "telepules": "Csömödér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8957,
         "telepules": "Hernyék",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8957,
         "telepules": "Kissziget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8957,
         "telepules": "Zebecke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8958,
         "telepules": "Iklódbördőce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8960,
         "telepules": "Lenti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8960,
         "telepules": "Gosztola",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8966,
         "telepules": "Lenti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8969,
         "telepules": "Gáborjánháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8969,
         "telepules": "Bödeháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8969,
         "telepules": "Szijártóháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8969,
         "telepules": "Zalaszombatfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8971,
         "telepules": "Zalabaksa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8971,
         "telepules": "Kerkabarabás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8973,
         "telepules": "Csesztreg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8973,
         "telepules": "Alsószenterzsébet",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8973,
         "telepules": "Felsőszenterzsébet",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8973,
         "telepules": "Kerkafalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8973,
         "telepules": "Kerkakutas",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8973,
         "telepules": "Magyarföld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8973,
         "telepules": "Ramocsa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8975,
         "telepules": "Szentgyörgyvölgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8976,
         "telepules": "Nemesnép",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8976,
         "telepules": "Márokföld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8977,
         "telepules": "Resznek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8977,
         "telepules": "Baglad",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8977,
         "telepules": "Lendvajakabfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8978,
         "telepules": "Rédics",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8978,
         "telepules": "Belsősárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8978,
         "telepules": "Külsősárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8978,
         "telepules": "Lendvadedes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8981,
         "telepules": "Gellénháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8981,
         "telepules": "Lickóvadamos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8983,
         "telepules": "Nagylengyel",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8983,
         "telepules": "Babosdöbréte",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8983,
         "telepules": "Ormándlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8984,
         "telepules": "Petrikeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8984,
         "telepules": "Gombosszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8984,
         "telepules": "Iborfia",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8985,
         "telepules": "Becsvölgye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8986,
         "telepules": "Pórszombat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8986,
         "telepules": "Pusztaapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8986,
         "telepules": "Szilvágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8988,
         "telepules": "Kálócfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8988,
         "telepules": "Kozmadombja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8989,
         "telepules": "Dobronhegy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8990,
         "telepules": "Pálfiszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8991,
         "telepules": "Teskánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8991,
         "telepules": "Böde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8991,
         "telepules": "Hottó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8992,
         "telepules": "Bagod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8992,
         "telepules": "Boncodfölde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8992,
         "telepules": "Hagyárosbörönd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8992,
         "telepules": "Zalaboldogfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8994,
         "telepules": "Zalaszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8994,
         "telepules": "Kávás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8995,
         "telepules": "Salomvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8995,
         "telepules": "Keménfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8996,
         "telepules": "Zalacséb",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8997,
         "telepules": "Zalaháshágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8998,
         "telepules": "Vaspör",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8998,
         "telepules": "Ozmánbük",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8999,
         "telepules": "Zalalövő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 8999,
         "telepules": "Csöde",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9000,
         "telepules": "Győr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9061,
         "telepules": "Vámosszabadi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9062,
         "telepules": "Kisbajcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9062,
         "telepules": "Vének",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9063,
         "telepules": "Nagybajcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9064,
         "telepules": "Vámosszabadi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9071,
         "telepules": "Gönyű",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9072,
         "telepules": "Nagyszentjános",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9073,
         "telepules": "Bőny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9074,
         "telepules": "Rétalap",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9081,
         "telepules": "Győrújbarát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9082,
         "telepules": "Nyúl",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9083,
         "telepules": "Écs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9084,
         "telepules": "Győrság",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9085,
         "telepules": "Pázmándfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9086,
         "telepules": "Töltéstava",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9088,
         "telepules": "Bakonypéterd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9089,
         "telepules": "Lázi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9090,
         "telepules": "Pannonhalma",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9091,
         "telepules": "Ravazd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9092,
         "telepules": "Tarjánpuszta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9093,
         "telepules": "Győrasszonyfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9094,
         "telepules": "Tápszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9095,
         "telepules": "Táp",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9096,
         "telepules": "Nyalka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9097,
         "telepules": "Mezőörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9098,
         "telepules": "Mezőörs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9099,
         "telepules": "Pér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9100,
         "telepules": "Tét",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9111,
         "telepules": "Tényő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9112,
         "telepules": "Sokorópátka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9113,
         "telepules": "Koroncó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9121,
         "telepules": "Győrszemere",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9122,
         "telepules": "Felpéc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9123,
         "telepules": "Kajárpéc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9124,
         "telepules": "Gyömöre",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9125,
         "telepules": "Szerecseny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9126,
         "telepules": "Gyarmat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9127,
         "telepules": "Csikvánd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9131,
         "telepules": "Mórichida",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9132,
         "telepules": "Árpás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9133,
         "telepules": "Kisbabot",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9133,
         "telepules": "Rábaszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9134,
         "telepules": "Bodonhely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9135,
         "telepules": "Rábaszentmihály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9136,
         "telepules": "Rábacsécsény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9136,
         "telepules": "Mérges",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9141,
         "telepules": "Ikrény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9142,
         "telepules": "Rábapatona",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9143,
         "telepules": "Enese",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9144,
         "telepules": "Kóny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9145,
         "telepules": "Bágyogszovát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9146,
         "telepules": "Rábapordány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9147,
         "telepules": "Dör",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9151,
         "telepules": "Abda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9152,
         "telepules": "Börcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9153,
         "telepules": "Öttevény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9154,
         "telepules": "Mosonszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9155,
         "telepules": "Lébény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9161,
         "telepules": "Győrsövényház",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9162,
         "telepules": "Bezi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9163,
         "telepules": "Fehértó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9164,
         "telepules": "Markotabödöge",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9165,
         "telepules": "Rábcakapi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9165,
         "telepules": "Cakóháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9165,
         "telepules": "Tárnokréti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9167,
         "telepules": "Bősárkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9167,
         "telepules": "Jánossomorja    ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9168,
         "telepules": "Acsalag",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9168,
         "telepules": "Csorna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9169,
         "telepules": "Barbacs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9169,
         "telepules": "Maglóca",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9171,
         "telepules": "Győrújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9172,
         "telepules": "Győrzámoly",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9173,
         "telepules": "Győrladamér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9174,
         "telepules": "Dunaszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9175,
         "telepules": "Dunaszentpál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9176,
         "telepules": "Mecsér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9177,
         "telepules": "Ásványráró",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9178,
         "telepules": "Hédervár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9181,
         "telepules": "Kimle",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9182,
         "telepules": "Károlyháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9183,
         "telepules": "Mosonszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9183,
         "telepules": "Mosonszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9184,
         "telepules": "Kunsziget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9200,
         "telepules": "Mosonmagyaróvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9211,
         "telepules": "Feketeerdő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9221,
         "telepules": "Levél",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9222,
         "telepules": "Hegyeshalom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9223,
         "telepules": "Bezenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9224,
         "telepules": "Rajka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9225,
         "telepules": "Dunakiliti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9226,
         "telepules": "Dunasziget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9228,
         "telepules": "Halászi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9231,
         "telepules": "Máriakálnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9232,
         "telepules": "Darnózseli",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9233,
         "telepules": "Lipót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9234,
         "telepules": "Kisbodak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9235,
         "telepules": "Püski",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9235,
         "telepules": "Dunaremete",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9241,
         "telepules": "Jánossomorja    ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9241,
         "telepules": "Jánossomorja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9242,
         "telepules": "Jánossomorja    ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9243,
         "telepules": "Várbalog",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9244,
         "telepules": "Újrónafő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9245,
         "telepules": "Mosonszolnok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9246,
         "telepules": "Mosonudvar",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9300,
         "telepules": "Csorna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9311,
         "telepules": "Pásztori",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9312,
         "telepules": "Szilsárkány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9313,
         "telepules": "Rábacsanak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9314,
         "telepules": "Egyed",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9315,
         "telepules": "Sobor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9316,
         "telepules": "Rábaszentandrás",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9317,
         "telepules": "Szany",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9321,
         "telepules": "Farád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9322,
         "telepules": "Rábatamási",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9323,
         "telepules": "Jobaháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9324,
         "telepules": "Bogyoszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9324,
         "telepules": "Potyond",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9325,
         "telepules": "Sopronnémeti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9326,
         "telepules": "Szil",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9327,
         "telepules": "Vág",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9327,
         "telepules": "Rábasebes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9330,
         "telepules": "Kapuvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9339,
         "telepules": "Kapuvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9341,
         "telepules": "Kisfalud",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9342,
         "telepules": "Mihályi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9343,
         "telepules": "Beled",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9343,
         "telepules": "Edve",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9343,
         "telepules": "Vásárosfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9344,
         "telepules": "Rábakecöl",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9345,
         "telepules": "Páli",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9346,
         "telepules": "Magyarkeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9346,
         "telepules": "Vadosfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9346,
         "telepules": "Zsebeháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9351,
         "telepules": "Babót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9352,
         "telepules": "Veszkény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9353,
         "telepules": "Szárföld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9354,
         "telepules": "Osli",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9361,
         "telepules": "Hövej",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9362,
         "telepules": "Himod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9363,
         "telepules": "Gyóró",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9364,
         "telepules": "Cirák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9365,
         "telepules": "Dénesfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9371,
         "telepules": "Vitnyéd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9372,
         "telepules": "Csapod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9373,
         "telepules": "Pusztacsalád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9374,
         "telepules": "Iván",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9375,
         "telepules": "Répceszemere",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9375,
         "telepules": "Csáfordjánosfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9375,
         "telepules": "Csér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9400,
         "telepules": "Sopron",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9407,
         "telepules": "Sopron",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9408,
         "telepules": "Sopron",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9421,
         "telepules": "Fertőrákos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9422,
         "telepules": "Harka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9423,
         "telepules": "Ágfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9431,
         "telepules": "Fertőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9433,
         "telepules": "Fertőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9434,
         "telepules": "Sarród",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9435,
         "telepules": "Sarród",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9436,
         "telepules": "Fertőszéplak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9437,
         "telepules": "Hegykő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9438,
         "telepules": "Sarród",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9441,
         "telepules": "Agyagosszergény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9442,
         "telepules": "Fertőendréd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9443,
         "telepules": "Petőháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9444,
         "telepules": "Fertőszentmiklós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9451,
         "telepules": "Röjtökmuzsaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9451,
         "telepules": "Ebergőc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9461,
         "telepules": "Lövő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9462,
         "telepules": "Völcsej",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9463,
         "telepules": "Sopronhorpács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9464,
         "telepules": "Und",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9471,
         "telepules": "Nemeskér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9472,
         "telepules": "Újkér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9473,
         "telepules": "Egyházasfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9474,
         "telepules": "Szakony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9474,
         "telepules": "Gyalóka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9475,
         "telepules": "Répcevis",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9476,
         "telepules": "Zsira",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9481,
         "telepules": "Pinnye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9482,
         "telepules": "Nagylózs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9483,
         "telepules": "Sopronkövesd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9484,
         "telepules": "Pereszteg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9485,
         "telepules": "Nagycenk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9491,
         "telepules": "Hidegség",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9492,
         "telepules": "Fertőhomok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9493,
         "telepules": "Fertőboz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9494,
         "telepules": "Sopron",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9495,
         "telepules": "Kópháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9500,
         "telepules": "Celldömölk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9511,
         "telepules": "Kemenesmihályfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9512,
         "telepules": "Ostffyasszonyfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9513,
         "telepules": "Csönge",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9514,
         "telepules": "Kenyeri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9515,
         "telepules": "Pápoc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9516,
         "telepules": "Vönöck",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9517,
         "telepules": "Kemenessömjén",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9521,
         "telepules": "Kemenesszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9522,
         "telepules": "Kemenesmagasi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9523,
         "telepules": "Szergény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9531,
         "telepules": "Mersevát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9532,
         "telepules": "Külsővat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9533,
         "telepules": "Nemesszalók",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9534,
         "telepules": "Marcalgergelyi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9534,
         "telepules": "Vinár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9541,
         "telepules": "Celldömölk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9542,
         "telepules": "Boba",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9542,
         "telepules": "Nemeskocs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9544,
         "telepules": "Kemenespálfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9545,
         "telepules": "Jánosháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9547,
         "telepules": "Karakó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9548,
         "telepules": "Nemeskeresztúr",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9549,
         "telepules": "Keléd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9551,
         "telepules": "Mesteri",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9552,
         "telepules": "Vásárosmiske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9553,
         "telepules": "Köcsk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9553,
         "telepules": "Kemeneskápolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9554,
         "telepules": "Egyházashetye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9554,
         "telepules": "Borgáta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9555,
         "telepules": "Kissomlyó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9556,
         "telepules": "Duka",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9561,
         "telepules": "Nagysimonyi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9561,
         "telepules": "Tokorcs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9600,
         "telepules": "Sárvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9608,
         "telepules": "Sárvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9609,
         "telepules": "Sárvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9611,
         "telepules": "Csénye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9612,
         "telepules": "Bögöt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9612,
         "telepules": "Porpác",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9621,
         "telepules": "Ölbő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9622,
         "telepules": "Szeleste",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9623,
         "telepules": "Répceszentgyörgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9624,
         "telepules": "Chernelházadamonya",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9625,
         "telepules": "Bő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9625,
         "telepules": "Gór",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9631,
         "telepules": "Hegyfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9632,
         "telepules": "Sajtoskál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9633,
         "telepules": "Simaság",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9634,
         "telepules": "Lócs",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9634,
         "telepules": "Iklanberény",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9635,
         "telepules": "Zsédeny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9636,
         "telepules": "Pósfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9641,
         "telepules": "Rábapaty",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9643,
         "telepules": "Jákfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9651,
         "telepules": "Uraiújfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9652,
         "telepules": "Nick",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9653,
         "telepules": "Répcelak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9654,
         "telepules": "Csánig",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9661,
         "telepules": "Vasegerszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9662,
         "telepules": "Tompaládony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9662,
         "telepules": "Mesterháza",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9663,
         "telepules": "Nemesládony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9664,
         "telepules": "Nagygeresd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9665,
         "telepules": "Vámoscsalád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9671,
         "telepules": "Sitke",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9672,
         "telepules": "Gérce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9673,
         "telepules": "Káld",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9674,
         "telepules": "Vashosszúfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9675,
         "telepules": "Bögöte",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9676,
         "telepules": "Hosszúpereszteg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9681,
         "telepules": "Sótony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9682,
         "telepules": "Nyőgér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9683,
         "telepules": "Bejcgyertyános",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9684,
         "telepules": "Egervölgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9685,
         "telepules": "Szemenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9700,
         "telepules": "Szombathely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9707,
         "telepules": "Szombathely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9721,
         "telepules": "Gencsapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9722,
         "telepules": "Perenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9723,
         "telepules": "Gyöngyösfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9724,
         "telepules": "Lukácsháza ",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9725,
         "telepules": "Kőszegszerdahely",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9725,
         "telepules": "Cák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9725,
         "telepules": "Kőszegdoroszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9726,
         "telepules": "Velem",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9727,
         "telepules": "Bozsok",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9730,
         "telepules": "Kőszeg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9733,
         "telepules": "Horvátzsidány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9733,
         "telepules": "Kiszsidány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9733,
         "telepules": "Ólmod",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9734,
         "telepules": "Peresznye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9735,
         "telepules": "Csepreg",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9736,
         "telepules": "Tormásliget",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9737,
         "telepules": "Bük",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9738,
         "telepules": "Tömörd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9739,
         "telepules": "Nemescsó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9739,
         "telepules": "Kőszegpaty",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9739,
         "telepules": "Pusztacsó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9740,
         "telepules": "Bük",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9741,
         "telepules": "Vassurány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9742,
         "telepules": "Salköveskút",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9743,
         "telepules": "Söpte",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9744,
         "telepules": "Vasasszonyfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9745,
         "telepules": "Meszlen",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9746,
         "telepules": "Acsád",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9747,
         "telepules": "Vasszilvágy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9748,
         "telepules": "Vát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9749,
         "telepules": "Nemesbőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9751,
         "telepules": "Vép",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9752,
         "telepules": "Bozzai",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9752,
         "telepules": "Kenéz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9754,
         "telepules": "Pecöl",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9754,
         "telepules": "Megyehíd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9756,
         "telepules": "Ikervár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9757,
         "telepules": "Meggyeskovácsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9761,
         "telepules": "Táplánszentkereszt",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9762,
         "telepules": "Tanakajd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9763,
         "telepules": "Vasszécseny",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9764,
         "telepules": "Csempeszkopács",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9764,
         "telepules": "Meggyeskovácsi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9766,
         "telepules": "Rum",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9766,
         "telepules": "Rábatöttös",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9766,
         "telepules": "Zsennye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9771,
         "telepules": "Balogunyom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9772,
         "telepules": "Kisunyom",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9773,
         "telepules": "Sorokpolány",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9774,
         "telepules": "Sorkifalud",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9774,
         "telepules": "Gyanógeregye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9774,
         "telepules": "Sorkikápolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9775,
         "telepules": "Nemeskolta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9776,
         "telepules": "Püspökmolnári",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9777,
         "telepules": "Rábahídvég",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9781,
         "telepules": "Egyházashollós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9782,
         "telepules": "Nemesrempehollós",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9783,
         "telepules": "Egyházasrádóc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9784,
         "telepules": "Rádóckölked",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9784,
         "telepules": "Harasztifalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9784,
         "telepules": "Nagykölked",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9789,
         "telepules": "Sé",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9791,
         "telepules": "Torony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9791,
         "telepules": "Dozmat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9792,
         "telepules": "Bucsu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9793,
         "telepules": "Narda",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9794,
         "telepules": "Felsőcsatár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9795,
         "telepules": "Vaskeresztes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9796,
         "telepules": "Pornóapáti",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9796,
         "telepules": "Horvátlövő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9797,
         "telepules": "Nárai",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9798,
         "telepules": "Ják",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9799,
         "telepules": "Szentpéterfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9800,
         "telepules": "Vasvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9811,
         "telepules": "Andrásfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9812,
         "telepules": "Telekes",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9813,
         "telepules": "Gersekarát",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9813,
         "telepules": "Sárfimizdó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9814,
         "telepules": "Halastó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9821,
         "telepules": "Győrvár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9821,
         "telepules": "Hegyhátszentpéter",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9823,
         "telepules": "Pácsony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9824,
         "telepules": "Olaszfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9825,
         "telepules": "Oszkó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9826,
         "telepules": "Petőmihályfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9831,
         "telepules": "Bérbaltavár",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9832,
         "telepules": "Nagytilaj",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9833,
         "telepules": "Csehi",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9834,
         "telepules": "Csehimindszent",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9835,
         "telepules": "Mikosszéplak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9836,
         "telepules": "Csipkerek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9841,
         "telepules": "Kám",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9842,
         "telepules": "Alsóújlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9900,
         "telepules": "Körmend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9909,
         "telepules": "Körmend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9909,
         "telepules": "Magyarnádalja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9912,
         "telepules": "Molnaszecsőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9912,
         "telepules": "Magyarszecsőd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9913,
         "telepules": "Szarvaskend",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9913,
         "telepules": "Döröske",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9913,
         "telepules": "Nagymizdó",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9914,
         "telepules": "Döbörhegy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9915,
         "telepules": "Nádasd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9915,
         "telepules": "Hegyháthodász",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9915,
         "telepules": "Hegyhátsál",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9915,
         "telepules": "Katafa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9917,
         "telepules": "Halogy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9917,
         "telepules": "Daraboshegy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9918,
         "telepules": "Felsőmarác",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9919,
         "telepules": "Csákánydoroszló",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9921,
         "telepules": "Vasalja",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9922,
         "telepules": "Pinkamindszent",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9923,
         "telepules": "Kemestaródfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9931,
         "telepules": "Ivánc",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9931,
         "telepules": "Hegyhátszentmárton",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9932,
         "telepules": "Viszák",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9933,
         "telepules": "Őrimagyarósd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9934,
         "telepules": "Hegyhátszentjakab",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9934,
         "telepules": "Felsőjánosfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9934,
         "telepules": "Szaknyér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9935,
         "telepules": "Szőce",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9936,
         "telepules": "Kisrákos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9937,
         "telepules": "Pankasz",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9938,
         "telepules": "Nagyrákos",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9938,
         "telepules": "Szatta",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9941,
         "telepules": "Őriszentpéter",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9941,
         "telepules": "Ispánk",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9942,
         "telepules": "Szalafő",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9943,
         "telepules": "Kondorfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9944,
         "telepules": "Bajánsenye",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9944,
         "telepules": "Kerkáskápolna",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9945,
         "telepules": "Kercaszomor",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9946,
         "telepules": "Magyarszombatfa",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9946,
         "telepules": "Velemér",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9951,
         "telepules": "Rátót",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9952,
         "telepules": "Gasztony",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9953,
         "telepules": "Vasszentmihály",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9953,
         "telepules": "Nemesmedves",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9954,
         "telepules": "Rönök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9955,
         "telepules": "Szentgotthárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9961,
         "telepules": "Rábagyarmat",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9962,
         "telepules": "Csörötnek",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9962,
         "telepules": "Magyarlak",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9970,
         "telepules": "Szentgotthárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9981,
         "telepules": "Szentgotthárd",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9982,
         "telepules": "Apátistvánfalva",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9982,
         "telepules": "Kétvölgy",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9982,
         "telepules": "Orfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9983,
         "telepules": "Alsószölnök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9983,
         "telepules": "Szakonyfalu",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 9985,
         "telepules": "Felsőszölnök",
-        "kerulet": NaN,
-        "kozterulet": NaN,
-        "terulet_jellege": NaN
+        "kerulet": null,
+        "kozterulet": null,
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 1173,
         "telepules": "Budapest",
         "kerulet": "XVII.",
         "kozterulet": "501.",
         "terulet_jellege": "utca"
@@ -31810,15 +31810,15 @@
         "terulet_jellege": "utca"
     },
     {
         "iranyitoszam": 1185,
         "telepules": "Budapest",
         "kerulet": "XVIII.",
         "kozterulet": "BUD Nemzetközi Repülőtér",
-        "terulet_jellege": NaN
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 1033,
         "telepules": "Budapest",
         "kerulet": "III.",
         "kozterulet": "Bud Spencer",
         "terulet_jellege": "park"
@@ -53363,15 +53363,15 @@
         "terulet_jellege": "körút"
     },
     {
         "iranyitoszam": 1163,
         "telepules": "Budapest",
         "kerulet": "XVI.",
         "kozterulet": "Kertvárosi Olimpikonok Parkja",
-        "terulet_jellege": NaN
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 1174,
         "telepules": "Budapest",
         "kerulet": "XVII.",
         "kozterulet": "Kerülő ",
         "terulet_jellege": "utca"
@@ -66474,22 +66474,22 @@
         "terulet_jellege": "sétány"
     },
     {
         "iranyitoszam": 1066,
         "telepules": "Budapest",
         "kerulet": "VI.",
         "kozterulet": "Oktogon",
-        "terulet_jellege": NaN
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 1067,
         "telepules": "Budapest",
         "kerulet": "VI.",
         "kozterulet": "Oktogon",
-        "terulet_jellege": NaN
+        "terulet_jellege": null
     },
     {
         "iranyitoszam": 1106,
         "telepules": "Budapest",
         "kerulet": "X.",
         "kozterulet": "Olaj ",
         "terulet_jellege": "utca"
```

### Comparing `magyar-4.0.5/setup.py` & `magyar-4.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="4.0.5",
+    version="4.0.6",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

