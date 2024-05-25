# Comparing `tmp/magyar-4.0.1.tar.gz` & `tmp/magyar-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-4.0.1.tar", last modified: Sat May 25 18:52:21 2024, max compression
+gzip compressed data, was "magyar-4.0.3.tar", last modified: Sat May 25 21:26:20 2024, max compression
```

## Comparing `magyar-4.0.1.tar` & `magyar-4.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-25 18:52:21.699541 magyar-4.0.1/
--rw-r--r--   0 bela      (1000) bela      (1000)     7113 2024-05-25 18:52:21.699541 magyar-4.0.1/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     6699 2024-05-25 18:50:31.000000 magyar-4.0.1/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-25 18:52:21.698541 magyar-4.0.1/magyar.egg-info/
--rw-r--r--   0 bela      (1000) bela      (1000)     7113 2024-05-25 18:52:21.000000 magyar-4.0.1/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-25 18:52:21.000000 magyar-4.0.1/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-25 18:52:21.000000 magyar-4.0.1/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-25 18:52:21.000000 magyar-4.0.1/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)   349737 2024-05-25 17:42:38.000000 magyar-4.0.1/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-25 18:52:21.699541 magyar-4.0.1/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      631 2024-05-25 18:40:50.000000 magyar-4.0.1/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-25 21:26:20.032410 magyar-4.0.3/
+-rw-r--r--   0 bela      (1000) bela      (1000)     7633 2024-05-25 21:26:20.032410 magyar-4.0.3/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     7218 2024-05-25 21:23:54.000000 magyar-4.0.3/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2024-05-25 21:26:20.032410 magyar-4.0.3/magyar.egg-info/
+-rw-r--r--   0 bela      (1000) bela      (1000)     7633 2024-05-25 21:26:19.000000 magyar-4.0.3/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2024-05-25 21:26:19.000000 magyar-4.0.3/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2024-05-25 21:26:19.000000 magyar-4.0.3/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2024-05-25 21:26:19.000000 magyar-4.0.3/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)   904430 2024-05-25 21:08:31.000000 magyar-4.0.3/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2024-05-25 21:26:20.032410 magyar-4.0.3/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      632 2024-05-25 21:24:48.000000 magyar-4.0.3/setup.py
```

### Comparing `magyar-4.0.1/PKG-INFO` & `magyar-4.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 4.0.1
-Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS..
+Version: 4.0.3
+Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -180,21 +180,29 @@
         magyar.fel_kerekit(szam)
         magyar.le_kerekit(szam)
 
 
 Tizedes számot kerekít egész számra fel vagy le.  </br>
  </br>
 ![Kerekítés](https://raw.githubusercontent.com/kobanya/nevek/master/kerekites.png)
-
+**GPS koordináták :** <BR>
+Adatformátum:  [('Aba', 'Fejér', 47.0292178, 18.5216608) <BR> <BR>
 Magyarosrági települések GPS koordinátáinak keresése:
 
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_keres.png)
-
-
+<BR>
+Azonos szélességi, hosszúsági körön lévő Magyar települések listázása: <BR>
+![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
+<BR>
+**Postai irányítószámok - ZIP**  <BR><BR>
+magyar.irsz <BR>
+Adatstruktúra :   [('1XXX', 'Budapest'), (2000, 'Szentendre')] <BR><BR>
+magyar.irsz_bp <BR>
+Adatstruktúra:  [(1173, 'Budapest', 'XVII.', '500.', 'utca')]
 ## Szerző
 
-* Név: Nagy BÉLa és Szabados Levente
+* Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
 Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-4.0.1/README.md` & `magyar-4.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -168,21 +168,29 @@
         magyar.fel_kerekit(szam)
         magyar.le_kerekit(szam)
 
 
 Tizedes számot kerekít egész számra fel vagy le.  </br>
  </br>
 ![Kerekítés](https://raw.githubusercontent.com/kobanya/nevek/master/kerekites.png)
-
+**GPS koordináták :** <BR>
+Adatformátum:  [('Aba', 'Fejér', 47.0292178, 18.5216608) <BR> <BR>
 Magyarosrági települések GPS koordinátáinak keresése:
 
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_keres.png)
-
-
+<BR>
+Azonos szélességi, hosszúsági körön lévő Magyar települések listázása: <BR>
+![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
+<BR>
+**Postai irányítószámok - ZIP**  <BR><BR>
+magyar.irsz <BR>
+Adatstruktúra :   [('1XXX', 'Budapest'), (2000, 'Szentendre')] <BR><BR>
+magyar.irsz_bp <BR>
+Adatstruktúra:  [(1173, 'Budapest', 'XVII.', '500.', 'utca')]
 ## Szerző
 
-* Név: Nagy BÉLa és Szabados Levente
+* Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
 Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-4.0.1/magyar.egg-info/PKG-INFO` & `magyar-4.0.3/magyar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 4.0.1
-Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS..
+Version: 4.0.3
+Summary: Hungarian lists of names,animals,foods, fruits, rivers ,GPS ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -180,21 +180,29 @@
         magyar.fel_kerekit(szam)
         magyar.le_kerekit(szam)
 
 
 Tizedes számot kerekít egész számra fel vagy le.  </br>
  </br>
 ![Kerekítés](https://raw.githubusercontent.com/kobanya/nevek/master/kerekites.png)
-
+**GPS koordináták :** <BR>
+Adatformátum:  [('Aba', 'Fejér', 47.0292178, 18.5216608) <BR> <BR>
 Magyarosrági települések GPS koordinátáinak keresése:
 
 ![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_keres.png)
-
-
+<BR>
+Azonos szélességi, hosszúsági körön lévő Magyar települések listázása: <BR>
+![GPS Keresés](https://raw.githubusercontent.com/kobanya/nevek/master/GPS_azonos.png)
+<BR>
+**Postai irányítószámok - ZIP**  <BR><BR>
+magyar.irsz <BR>
+Adatstruktúra :   [('1XXX', 'Budapest'), (2000, 'Szentendre')] <BR><BR>
+magyar.irsz_bp <BR>
+Adatstruktúra:  [(1173, 'Budapest', 'XVII.', '500.', 'utca')]
 ## Szerző
 
-* Név: Nagy BÉLa és Szabados Levente
+* Név: Nagy BÉLA és Szabados Levente (GPS coordináták)
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
 Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-4.0.1/setup.py` & `magyar-4.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="4.0.1",
+    version="4.0.3",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
-    description="Hungarian lists of names,animals,foods, fruits, rivers ,GPS..",
+    description="Hungarian lists of names,animals,foods, fruits, rivers ,GPS ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

