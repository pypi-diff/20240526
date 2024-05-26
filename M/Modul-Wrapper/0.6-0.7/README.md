# Comparing `tmp/Modul_Wrapper-0.6.tar.gz` & `tmp/Modul_Wrapper-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Modul_Wrapper-0.6.tar", last modified: Sun May 26 11:47:43 2024, max compression
+gzip compressed data, was "Modul_Wrapper-0.7.tar", last modified: Sun May 26 20:50:53 2024, max compression
```

## Comparing `Modul_Wrapper-0.6.tar` & `Modul_Wrapper-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 11:47:43.824452 Modul_Wrapper-0.6/
--rw-rw-rw-   0        0        0     1090 2024-05-26 09:13:51.000000 Modul_Wrapper-0.6/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-26 11:47:43.793133 Modul_Wrapper-0.6/Modul_Wrapper/
--rw-rw-rw-   0        0        0       28 2024-05-26 10:17:46.000000 Modul_Wrapper-0.6/Modul_Wrapper/__init__.py
--rw-rw-rw-   0        0        0     1031 2024-05-26 10:17:43.000000 Modul_Wrapper-0.6/Modul_Wrapper/core_modul.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:47:43.808757 Modul_Wrapper-0.6/Modul_Wrapper.egg-info/
--rw-rw-rw-   0        0        0     1839 2024-05-26 11:47:43.000000 Modul_Wrapper-0.6/Modul_Wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-26 11:47:43.000000 Modul_Wrapper-0.6/Modul_Wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 11:47:43.000000 Modul_Wrapper-0.6/Modul_Wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-26 11:47:43.000000 Modul_Wrapper-0.6/Modul_Wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1839 2024-05-26 11:47:43.824452 Modul_Wrapper-0.6/PKG-INFO
--rw-rw-rw-   0        0        0      736 2024-05-26 11:39:42.000000 Modul_Wrapper-0.6/README.md
--rw-rw-rw-   0        0        0       86 2024-05-26 11:47:43.824452 Modul_Wrapper-0.6/setup.cfg
--rw-rw-rw-   0        0        0     2465 2024-05-26 11:47:19.000000 Modul_Wrapper-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:50:53.250478 Modul_Wrapper-0.7/
+-rw-rw-rw-   0        0        0     1090 2024-05-26 09:13:51.000000 Modul_Wrapper-0.7/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-26 20:50:53.163478 Modul_Wrapper-0.7/Modul_Wrapper/
+-rw-rw-rw-   0        0        0       28 2024-05-26 10:17:46.000000 Modul_Wrapper-0.7/Modul_Wrapper/__init__.py
+-rw-rw-rw-   0        0        0     1031 2024-05-26 10:17:43.000000 Modul_Wrapper-0.7/Modul_Wrapper/core_modul.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:50:53.248482 Modul_Wrapper-0.7/Modul_Wrapper.egg-info/
+-rw-rw-rw-   0        0        0     1851 2024-05-26 20:50:52.000000 Modul_Wrapper-0.7/Modul_Wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-26 20:50:53.000000 Modul_Wrapper-0.7/Modul_Wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 20:50:52.000000 Modul_Wrapper-0.7/Modul_Wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 20:50:52.000000 Modul_Wrapper-0.7/Modul_Wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1851 2024-05-26 20:50:53.250478 Modul_Wrapper-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2024-05-26 20:48:34.000000 Modul_Wrapper-0.7/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-26 20:50:53.262475 Modul_Wrapper-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2465 2024-05-26 20:48:44.000000 Modul_Wrapper-0.7/setup.py
```

### Comparing `Modul_Wrapper-0.6/LICENSE` & `Modul_Wrapper-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Modul_Wrapper-0.6/Modul_Wrapper/core_modul.py` & `Modul_Wrapper-0.7/Modul_Wrapper/core_modul.py`

 * *Files identical despite different names*

### Comparing `Modul_Wrapper-0.6/Modul_Wrapper.egg-info/PKG-INFO` & `Modul_Wrapper-0.7/Modul_Wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Modul-Wrapper
-Version: 0.6
+Version: 0.7
 Summary: Control Your Library With Dictionary
 Home-page: https://github.com/staykimin/Modul-Wrapper
 Author: KIMIN
 Author-email: staykimin@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/staykimin/Modul-Wrapper
 Project-URL: Funding, https://saweria.co/staykimin
@@ -31,23 +31,23 @@
 ## Example
 
 Tanpa Menggunakan Deklarasi Khusus
 ```python
 from Modul_Wrapper import Wrap
 
 modul = Wrap(modul_path="modul.json")
-datetime = modul['datetime'].datetime.now().strftime("%H:%M")
+datetime = modul.modul['datetime'].datetime.now().strftime("%H:%M")
 print(datetime)
 ```
 
 Menggunakan Deklarasi Khusus
 ```python
 from Modul_Wrapper import Wrap
 
 modul = Wrap(modul_path="modul.json")
-datetime = modul['modul_jam'].datetime.now().strftime("%H:%M")
+datetime = modul.modul['modul_jam'].datetime.now().strftime("%H:%M")
 print(datetime)
 ```
 
 ## Konfigurasi Modul
 
 Download Format Konfigurasi Modul Di : https://github.com/staykimin/Modul-Wrapper
```

### Comparing `Modul_Wrapper-0.6/PKG-INFO` & `Modul_Wrapper-0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Modul_Wrapper
-Version: 0.6
+Version: 0.7
 Summary: Control Your Library With Dictionary
 Home-page: https://github.com/staykimin/Modul-Wrapper
 Author: KIMIN
 Author-email: staykimin@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/staykimin/Modul-Wrapper
 Project-URL: Funding, https://saweria.co/staykimin
@@ -31,23 +31,23 @@
 ## Example
 
 Tanpa Menggunakan Deklarasi Khusus
 ```python
 from Modul_Wrapper import Wrap
 
 modul = Wrap(modul_path="modul.json")
-datetime = modul['datetime'].datetime.now().strftime("%H:%M")
+datetime = modul.modul['datetime'].datetime.now().strftime("%H:%M")
 print(datetime)
 ```
 
 Menggunakan Deklarasi Khusus
 ```python
 from Modul_Wrapper import Wrap
 
 modul = Wrap(modul_path="modul.json")
-datetime = modul['modul_jam'].datetime.now().strftime("%H:%M")
+datetime = modul.modul['modul_jam'].datetime.now().strftime("%H:%M")
 print(datetime)
 ```
 
 ## Konfigurasi Modul
 
 Download Format Konfigurasi Modul Di : https://github.com/staykimin/Modul-Wrapper
```

### Comparing `Modul_Wrapper-0.6/README.md` & `Modul_Wrapper-0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 ## Example
 
 Tanpa Menggunakan Deklarasi Khusus
 ```python
 from Modul_Wrapper import Wrap
 
 modul = Wrap(modul_path="modul.json")
-datetime = modul['datetime'].datetime.now().strftime("%H:%M")
+datetime = modul.modul['datetime'].datetime.now().strftime("%H:%M")
 print(datetime)
 ```
 
 Menggunakan Deklarasi Khusus
 ```python
 from Modul_Wrapper import Wrap
 
 modul = Wrap(modul_path="modul.json")
-datetime = modul['modul_jam'].datetime.now().strftime("%H:%M")
+datetime = modul.modul['modul_jam'].datetime.now().strftime("%H:%M")
 print(datetime)
 ```
 
 ## Konfigurasi Modul
 
 Download Format Konfigurasi Modul Di : https://github.com/staykimin/Modul-Wrapper
```

### Comparing `Modul_Wrapper-0.6/setup.py` & `Modul_Wrapper-0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'Modul_Wrapper',         # How you named your package folder (MyLib)
     packages = ['Modul_Wrapper'],   # Chose the same as "name"
-    version = '0.6',      # Start with a small number and increase it with every change you make
+    version = '0.7',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Control Your Library With Dictionary',   # Give a short description about your library
     long_description=long_description,            # Give a long description about your library
     long_description_content_type='text/markdown',
     author = 'KIMIN',                   # Type in your name
     author_email = 'staykimin@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/staykimin/Modul-Wrapper',   # Provide either the link to your github or to your website
```

