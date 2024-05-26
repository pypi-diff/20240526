# Comparing `tmp/Modul-Wrapper-0.2.tar.gz` & `tmp/Modul_Wrapper-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Modul-Wrapper-0.2.tar", last modified: Sun May 26 09:59:54 2024, max compression
+gzip compressed data, was "Modul_Wrapper-0.3.tar", last modified: Sun May 26 10:08:56 2024, max compression
```

## Comparing `Modul-Wrapper-0.2.tar` & `Modul_Wrapper-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 09:59:54.919363 Modul-Wrapper-0.2/
--rw-rw-rw-   0        0        0     1090 2024-05-26 09:13:51.000000 Modul-Wrapper-0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-26 09:59:54.888071 Modul-Wrapper-0.2/Modul-Wrapper/
--rw-rw-rw-   0        0        0       31 2024-05-26 09:13:51.000000 Modul-Wrapper-0.2/Modul-Wrapper/__init__.py
--rw-rw-rw-   0        0        0     1040 2024-05-26 09:43:49.000000 Modul-Wrapper-0.2/Modul-Wrapper/core_modul.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:59:54.903716 Modul-Wrapper-0.2/Modul_Wrapper.egg-info/
--rw-rw-rw-   0        0        0     1447 2024-05-26 09:59:54.000000 Modul-Wrapper-0.2/Modul_Wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-26 09:59:54.000000 Modul-Wrapper-0.2/Modul_Wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 09:59:54.000000 Modul-Wrapper-0.2/Modul_Wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-26 09:59:54.000000 Modul-Wrapper-0.2/Modul_Wrapper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1447 2024-05-26 09:59:54.919363 Modul-Wrapper-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-26 09:33:43.000000 Modul-Wrapper-0.2/README.md
--rw-rw-rw-   0        0        0       86 2024-05-26 09:59:54.919363 Modul-Wrapper-0.2/setup.cfg
--rw-rw-rw-   0        0        0     2595 2024-05-26 09:59:31.000000 Modul-Wrapper-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:08:56.103881 Modul_Wrapper-0.3/
+-rw-rw-rw-   0        0        0     1090 2024-05-26 09:13:51.000000 Modul_Wrapper-0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-26 10:08:56.072608 Modul_Wrapper-0.3/Modul Wrapper/
+-rw-rw-rw-   0        0        0       31 2024-05-26 09:13:51.000000 Modul_Wrapper-0.3/Modul Wrapper/__init__.py
+-rw-rw-rw-   0        0        0     1040 2024-05-26 09:43:49.000000 Modul_Wrapper-0.3/Modul Wrapper/core_modul.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:08:56.103881 Modul_Wrapper-0.3/Modul_Wrapper.egg-info/
+-rw-rw-rw-   0        0        0     1294 2024-05-26 10:08:55.000000 Modul_Wrapper-0.3/Modul_Wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-26 10:08:55.000000 Modul_Wrapper-0.3/Modul_Wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:08:55.000000 Modul_Wrapper-0.3/Modul_Wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 10:08:55.000000 Modul_Wrapper-0.3/Modul_Wrapper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1294 2024-05-26 10:08:56.103881 Modul_Wrapper-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-05-26 09:33:43.000000 Modul_Wrapper-0.3/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-26 10:08:56.119481 Modul_Wrapper-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2442 2024-05-26 10:08:39.000000 Modul_Wrapper-0.3/setup.py
```

### Comparing `Modul-Wrapper-0.2/LICENSE` & `Modul_Wrapper-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Modul-Wrapper-0.2/Modul-Wrapper/core_modul.py` & `Modul_Wrapper-0.3/Modul Wrapper/core_modul.py`

 * *Files identical despite different names*

### Comparing `Modul-Wrapper-0.2/Modul_Wrapper.egg-info/PKG-INFO` & `Modul_Wrapper-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: Modul-Wrapper
-Version: 0.2
-Summary: Modul Wrapper Adalah Modul Untuk Menyimpan Semua Library Yang Akan Digunakan Dalam Bentuk Dictionary Guna Menghindari Crash Karena Penamaan Class atau Function Yang Sama Antar Library.
+Name: Modul_Wrapper
+Version: 0.3
+Summary: Save Your Library To Dictionary
 Home-page: https://github.com/staykimin/Modul-Wrapper
 Author: KIMIN
 Author-email: staykimin@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/staykimin/Modul-Wrapper
 Project-URL: Funding, https://saweria.co/staykimin
 Project-URL: Say Thanks!, https://saweria.co/staykimin
```

### Comparing `Modul-Wrapper-0.2/PKG-INFO` & `Modul_Wrapper-0.3/Modul_Wrapper.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Modul-Wrapper
-Version: 0.2
-Summary: Modul Wrapper Adalah Modul Untuk Menyimpan Semua Library Yang Akan Digunakan Dalam Bentuk Dictionary Guna Menghindari Crash Karena Penamaan Class atau Function Yang Sama Antar Library.
+Version: 0.3
+Summary: Save Your Library To Dictionary
 Home-page: https://github.com/staykimin/Modul-Wrapper
 Author: KIMIN
 Author-email: staykimin@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/staykimin/Modul-Wrapper
 Project-URL: Funding, https://saweria.co/staykimin
 Project-URL: Say Thanks!, https://saweria.co/staykimin
```

### Comparing `Modul-Wrapper-0.2/setup.py` & `Modul_Wrapper-0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
-    name = 'Modul-Wrapper',         # How you named your package folder (MyLib)
-    packages = ['Modul-Wrapper'],   # Chose the same as "name"
-    version = '0.2',      # Start with a small number and increase it with every change you make
+    name = 'Modul_Wrapper',         # How you named your package folder (MyLib)
+    packages = ['Modul Wrapper'],   # Chose the same as "name"
+    version = '0.3',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-    description = 'Modul Wrapper Adalah Modul Untuk Menyimpan Semua Library Yang Akan Digunakan Dalam Bentuk Dictionary Guna Menghindari Crash Karena Penamaan Class atau Function Yang Sama Antar Library.',   # Give a short description about your library
+    description = 'Save Your Library To Dictionary',   # Give a short description about your library
     long_description=long_description,            # Give a long description about your library
     long_description_content_type='text/markdown',
     author = 'KIMIN',                   # Type in your name
     author_email = 'staykimin@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/staykimin/Modul-Wrapper',   # Provide either the link to your github or to your website
     # download_url = 'https://github.com/staykimin/Modul-Wrapper/archive/Modul-Wrapper-0.1.tar.gz',    # I explain this later on
     project_urls={
```

