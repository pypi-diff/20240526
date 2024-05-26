# Comparing `tmp/magyar-4.0.4.tar.gz` & `tmp/magyar-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-4.0.4.tar", last modified: Sat May 25 22:36:15 2024, max compression
+gzip compressed data, was "magyar-4.0.5.tar", last modified: Sun May 26 06:40:03 2024, max compression
```

## Comparing `magyar-4.0.4.tar` & `magyar-4.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-25 22:36:15.573081 magyar-4.0.4/
--rw-r--r--   0 bela      (1000) bela      (1000)     7637 2024-05-25 22:36:15.573081 magyar-4.0.4/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     7218 2024-05-25 21:23:54.000000 magyar-4.0.4/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-25 22:36:15.573081 magyar-4.0.4/magyar.egg-info/
--rw-r--r--   0 bela      (1000) bela      (1000)     7637 2024-05-25 22:36:15.000000 magyar-4.0.4/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-25 22:36:15.000000 magyar-4.0.4/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-25 22:36:15.000000 magyar-4.0.4/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-25 22:36:15.000000 magyar-4.0.4/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)   904428 2024-05-25 22:34:14.000000 magyar-4.0.4/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-25 22:36:15.573081 magyar-4.0.4/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      636 2024-05-25 22:34:14.000000 magyar-4.0.4/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 06:40:03.725217 magyar-4.0.5/
+-rw-r--r--   0 bela      (1000) bela      (1000)     7675 2024-05-26 06:40:03.725217 magyar-4.0.5/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     7259 2024-05-26 06:38:39.000000 magyar-4.0.5/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-26 06:40:03.725217 magyar-4.0.5/magyar.egg-info/
+-rw-r--r--   0 bela      (1000) bela      (1000)     7675 2024-05-26 06:40:03.000000 magyar-4.0.5/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-26 06:40:03.000000 magyar-4.0.5/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-26 06:40:03.000000 magyar-4.0.5/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-26 06:40:03.000000 magyar-4.0.5/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)  2550493 2024-05-26 06:34:28.000000 magyar-4.0.5/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-26 06:40:03.725217 magyar-4.0.5/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      633 2024-05-26 06:37:43.000000 magyar-4.0.5/setup.py
```

### Comparing `magyar-4.0.4/PKG-INFO` & `magyar-4.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 4.0.4
-Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS .. ZIP
+Version: 4.0.5
+Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -190,18 +190,22 @@
 
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_keres.png)
 <BR>
 Azonos szélességi, hosszúsági körön lévő Magyar települések listázása: <BR>
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
 <BR>
 **Postai irányítószámok - ZIP**  <BR><BR>
-magyar.irsz <BR>
-Adatstruktúra :   [('1XXX', 'Budapest'), (2000, 'Szentendre')] <BR><BR>
-magyar.irsz_bp <BR>
-Adatstruktúra:  [(1173, 'Budapest', 'XVII.', '500.', 'utca')]
+magyar.irsz <BR><BR>
+Adatstruktúra : irsz = [ {
+        "iranyitoszam": 2000,
+        "telepules": "Szentendre",
+        "kerulet": NaN,
+        "kozterulet": NaN,
+        "terulet_jellege": NaN
+    },]  <BR><BR>
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.0.4/README.md` & `magyar-4.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -178,18 +178,22 @@
 
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_keres.png)
 <BR>
 Azonos szélességi, hosszúsági körön lévő Magyar települések listázása: <BR>
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
 <BR>
 **Postai irányítószámok - ZIP**  <BR><BR>
-magyar.irsz <BR>
-Adatstruktúra :   [('1XXX', 'Budapest'), (2000, 'Szentendre')] <BR><BR>
-magyar.irsz_bp <BR>
-Adatstruktúra:  [(1173, 'Budapest', 'XVII.', '500.', 'utca')]
+magyar.irsz <BR><BR>
+Adatstruktúra : irsz = [ {
+        "iranyitoszam": 2000,
+        "telepules": "Szentendre",
+        "kerulet": NaN,
+        "kozterulet": NaN,
+        "terulet_jellege": NaN
+    },]  <BR><BR>
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.0.4/magyar.egg-info/PKG-INFO` & `magyar-4.0.5/magyar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 4.0.4
-Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS .. ZIP
+Version: 4.0.5
+Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -190,18 +190,22 @@
 
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_keres.png)
 <BR>
 Azonos szélességi, hosszúsági körön lévő Magyar települések listázása: <BR>
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
 <BR>
 **Postai irányítószámok - ZIP**  <BR><BR>
-magyar.irsz <BR>
-Adatstruktúra :   [('1XXX', 'Budapest'), (2000, 'Szentendre')] <BR><BR>
-magyar.irsz_bp <BR>
-Adatstruktúra:  [(1173, 'Budapest', 'XVII.', '500.', 'utca')]
+magyar.irsz <BR><BR>
+Adatstruktúra : irsz = [ {
+        "iranyitoszam": 2000,
+        "telepules": "Szentendre",
+        "kerulet": NaN,
+        "kozterulet": NaN,
+        "terulet_jellege": NaN
+    },]  <BR><BR>
 ## Szerző
 
 * Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-4.0.4/setup.py` & `magyar-4.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="4.0.4",
+    version="4.0.5",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
-    description="Hungarian lists of names,animals,foods, fruits, rivers ,GPS .. ZIP",
+    description="Hungarian lists of names,animals,foods, fruits, rivers ,GPS,ZIP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

