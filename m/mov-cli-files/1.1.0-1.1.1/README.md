# Comparing `tmp/mov_cli_files-1.1.0.tar.gz` & `tmp/mov_cli_files-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli_files-1.1.0.tar", last modified: Fri Apr 26 01:21:43 2024, max compression
+gzip compressed data, was "mov_cli_files-1.1.1.tar", last modified: Sun May 26 14:34:22 2024, max compression
```

## Comparing `mov_cli_files-1.1.0.tar` & `mov_cli_files-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/LICENSE
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2921 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)      544 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/README.md
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/mov_cli_files/
--rw-r--r--   0 ananas    (1000) ananas    (1000)      296 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/mov_cli_files/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)      987 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/mov_cli_files/paths.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     3011 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/mov_cli_files/scraper.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/mov_cli_files.egg-info/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2921 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)      290 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/SOURCES.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/dependency_links.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)       96 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/requires.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)       14 2024-04-26 01:21:43.000000 mov_cli_files-1.1.0/mov_cli_files.egg-info/top_level.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1349 2024-04-26 01:21:34.000000 mov_cli_files-1.1.0/pyproject.toml
--rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-04-26 01:21:43.863646 mov_cli_files-1.1.0/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-26 14:34:22.772119 mov_cli_files-1.1.1/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1064 2024-05-26 14:20:38.000000 mov_cli_files-1.1.1/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3410 2024-05-26 14:34:22.768786 mov_cli_files-1.1.1/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1114 2024-05-26 14:20:38.000000 mov_cli_files-1.1.1/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-26 14:34:22.768786 mov_cli_files-1.1.1/mov_cli_files/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      296 2024-05-26 14:32:02.000000 mov_cli_files-1.1.1/mov_cli_files/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      987 2024-05-26 14:20:38.000000 mov_cli_files-1.1.1/mov_cli_files/paths.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3012 2024-05-26 14:21:05.000000 mov_cli_files-1.1.1/mov_cli_files/scraper.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-26 14:34:22.768786 mov_cli_files-1.1.1/mov_cli_files.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     3410 2024-05-26 14:34:22.000000 mov_cli_files-1.1.1/mov_cli_files.egg-info/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      290 2024-05-26 14:34:22.000000 mov_cli_files-1.1.1/mov_cli_files.egg-info/SOURCES.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-05-26 14:34:22.000000 mov_cli_files-1.1.1/mov_cli_files.egg-info/dependency_links.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       42 2024-05-26 14:34:22.000000 mov_cli_files-1.1.1/mov_cli_files.egg-info/requires.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       14 2024-05-26 14:34:22.000000 mov_cli_files-1.1.1/mov_cli_files.egg-info/top_level.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1286 2024-05-26 14:20:38.000000 mov_cli_files-1.1.1/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-26 14:34:22.772119 mov_cli_files-1.1.1/setup.cfg
```

### Comparing `mov_cli_files-1.1.0/LICENSE` & `mov_cli_files-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli_files-1.1.0/PKG-INFO` & `mov_cli_files-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mov-cli-files
-Version: 1.1.0
+Version: 1.1.1
 Summary:  A mov-cli v4 plugin for watching files on your device.
-Author-email: Ananas <ananas@r3tr0ananas.lol>
+Author-email: Ananas <ananas@r3tr0ananas.pro>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -36,32 +36,29 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.3.0
 Requires-Dist: thefuzz
+Requires-Dist: mov-cli>=4.3.14
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-files 
   <sub>A mov-cli v4 plugin for watching files on your device.</sub>
   
   ![grafik](https://github.com/mov-cli/mov-cli-files/assets/132799819/5f25ac19-de39-4b26-8121-c0f58f167c6b)
 
 </div>
 
-
 ## Installation 🛠️
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-files
 ```
@@ -72,9 +69,27 @@
 ```toml
 [mov-cli.plugins]
 files = "mov-cli-files"
 ```
 
 ## Usage 🖱️
 ```sh
-mov-cli -s files PATH
+mov-cli -s files {query}
+```
+
+### Example 🌟
+Let's say I want to play an mp4 file in my Videos folder named "osaka_america_ya.mp4", this is the command you can use:
+```sh
+mov-cli -s files america ya
+```
+
+### Search in literal path 🔎
+If you would like to quickly search in a path that is not scanned by the plugin use the ``path`` scraper option like so:
+```sh
+mov-cli -s files osaka oh my gah -- --path ./Downloads
+```
+
+### Give me EVERYTHING ✴️
+If you would like to search for everything use the star chatacter (``*``) instead of entering a query like so:
+```sh
+mov-cli -s files "*"
 ```
```

### Comparing `mov_cli_files-1.1.0/mov_cli_files/paths.py` & `mov_cli_files-1.1.1/mov_cli_files/paths.py`

 * *Files identical despite different names*

### Comparing `mov_cli_files-1.1.0/mov_cli_files/scraper.py` & `mov_cli_files-1.1.1/mov_cli_files/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 create_datetime = datetime.fromtimestamp(st_ctime)
 
                 year = create_datetime.strftime("%Y")
 
                 yield Metadata(
                     id = str(path), 
                     title = path.stem, 
-                    type = MetadataType.MOVIE, 
+                    type = MetadataType.SINGLE, 
                     year = year
                 )
 
     def scrape(self, metadata: Metadata, _: EpisodeSelector) -> Single:
         return Single(
             url = metadata.id, 
             title = metadata.title,
```

### Comparing `mov_cli_files-1.1.0/mov_cli_files.egg-info/PKG-INFO` & `mov_cli_files-1.1.1/mov_cli_files.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mov-cli-files
-Version: 1.1.0
+Version: 1.1.1
 Summary:  A mov-cli v4 plugin for watching files on your device.
-Author-email: Ananas <ananas@r3tr0ananas.lol>
+Author-email: Ananas <ananas@r3tr0ananas.pro>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -36,32 +36,29 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.3.0
 Requires-Dist: thefuzz
+Requires-Dist: mov-cli>=4.3.14
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-files 
   <sub>A mov-cli v4 plugin for watching files on your device.</sub>
   
   ![grafik](https://github.com/mov-cli/mov-cli-files/assets/132799819/5f25ac19-de39-4b26-8121-c0f58f167c6b)
 
 </div>
 
-
 ## Installation 🛠️
 Here's how to install and add the plugin to mov-cli.
 
 1. Install the pip package.
 ```sh
 pip install mov-cli-files
 ```
@@ -72,9 +69,27 @@
 ```toml
 [mov-cli.plugins]
 files = "mov-cli-files"
 ```
 
 ## Usage 🖱️
 ```sh
-mov-cli -s files PATH
+mov-cli -s files {query}
+```
+
+### Example 🌟
+Let's say I want to play an mp4 file in my Videos folder named "osaka_america_ya.mp4", this is the command you can use:
+```sh
+mov-cli -s files america ya
+```
+
+### Search in literal path 🔎
+If you would like to quickly search in a path that is not scanned by the plugin use the ``path`` scraper option like so:
+```sh
+mov-cli -s files osaka oh my gah -- --path ./Downloads
+```
+
+### Give me EVERYTHING ✴️
+If you would like to search for everything use the star chatacter (``*``) instead of entering a query like so:
+```sh
+mov-cli -s files "*"
 ```
```

### Comparing `mov_cli_files-1.1.0/pyproject.toml` & `mov_cli_files-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "mov-cli-files"
 description = " A mov-cli v4 plugin for watching files on your device."
 authors = [
-    {name = "Ananas", email = "ananas@r3tr0ananas.lol"}
+    {name = "Ananas", email = "ananas@r3tr0ananas.pro"}
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = [
     "amazing mov-cli plugin"
 ]
@@ -18,19 +18,16 @@
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 	'Programming Language :: Python :: 3.11',
     "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-    "requests",
-    "importlib-metadata; python_version<'3.8'",
-
-    "mov-cli>=4.3.0",
-    "thefuzz"
+    "thefuzz",
+    "mov-cli>=4.3.14"
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "ruff",
@@ -45,8 +42,8 @@
 version = { attr = "mov_cli_files.__version__" }
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-include = ["mov_cli_files*"]
+include = ["mov_cli_files*"]
```

