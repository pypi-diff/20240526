# Comparing `tmp/magyar-4.0.7.tar.gz` & `tmp/magyar-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-4.0.7.tar", last modified: Sun May 26 08:40:41 2024, max compression
+gzip compressed data, was "magyar-4.1.0.tar", last modified: Sun May 26 09:08:19 2024, max compression
```

## Comparing `magyar-4.0.7.tar` & `magyar-4.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 08:40:41.178046 magyar-4.0.7/
--rw-r--r--   0 bela      (1000) bela      (1000)     7682 2024-05-26 08:40:41.178046 magyar-4.0.7/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     7266 2024-05-26 07:10:34.000000 magyar-4.0.7/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 08:40:41.178046 magyar-4.0.7/magyar.egg-info/
--rw-r--r--   0 bela      (1000) bela      (1000)     7682 2024-05-26 08:40:41.000000 magyar-4.0.7/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-26 08:40:41.000000 magyar-4.0.7/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-26 08:40:41.000000 magyar-4.0.7/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-26 08:40:41.000000 magyar-4.0.7/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)  2560465 2024-05-26 08:35:43.000000 magyar-4.0.7/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-26 08:40:41.178046 magyar-4.0.7/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      633 2024-05-26 08:07:26.000000 magyar-4.0.7/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 09:08:19.420143 magyar-4.1.0/
+-rw-r--r--   0 bela      (1000) bela      (1000)     7763 2024-05-26 09:08:19.420143 magyar-4.1.0/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     7347 2024-05-26 09:02:28.000000 magyar-4.1.0/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 09:08:19.419143 magyar-4.1.0/magyar.egg-info/
+-rw-r--r--   0 bela      (1000) bela      (1000)     7763 2024-05-26 09:08:19.000000 magyar-4.1.0/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-26 09:08:19.000000 magyar-4.1.0/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-26 09:08:19.000000 magyar-4.1.0/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-26 09:08:19.000000 magyar-4.1.0/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)  2560465 2024-05-26 08:35:43.000000 magyar-4.1.0/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-26 09:08:19.420143 magyar-4.1.0/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      633 2024-05-26 08:59:27.000000 magyar-4.1.0/setup.py
```

### Comparing `magyar-4.0.7/PKG-INFO` & `magyar-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 4.0.7
+Version: 4.1.0
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -194,18 +194,19 @@
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
 <BR><BR>
 **Postai irányítószámok - ZIP**  <BR><BR>
 magyar.irsz <BR><BR>
 Adatstruktúra : irsz = [ {
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
-        "kerulet": null,
-        "kozterulet": null,
-        "terulet_jellege": null
+        "kerulet": None,
+        "kozterulet": None,
+        "terulet_jellege": None
     },]  <BR><BR>
+![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/irsz.png)
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.0.7/README.md` & `magyar-4.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -182,18 +182,19 @@
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
 <BR><BR>
 **Postai irányítószámok - ZIP**  <BR><BR>
 magyar.irsz <BR><BR>
 Adatstruktúra : irsz = [ {
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
-        "kerulet": null,
-        "kozterulet": null,
-        "terulet_jellege": null
+        "kerulet": None,
+        "kozterulet": None,
+        "terulet_jellege": None
     },]  <BR><BR>
+![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/irsz.png)
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.0.7/magyar.egg-info/PKG-INFO` & `magyar-4.1.0/magyar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 4.0.7
+Version: 4.1.0
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -194,18 +194,19 @@
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
 <BR><BR>
 **Postai irányítószámok - ZIP**  <BR><BR>
 magyar.irsz <BR><BR>
 Adatstruktúra : irsz = [ {
         "iranyitoszam": 2000,
         "telepules": "Szentendre",
-        "kerulet": null,
-        "kozterulet": null,
-        "terulet_jellege": null
+        "kerulet": None,
+        "kozterulet": None,
+        "terulet_jellege": None
     },]  <BR><BR>
+![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/irsz.png)
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.0.7/magyar.py` & `magyar-4.1.0/magyar.py`

 * *Files identical despite different names*

### Comparing `magyar-4.0.7/setup.py` & `magyar-4.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="4.0.7",
+    version="4.1.0",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

