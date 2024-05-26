# Comparing `tmp/mov_cli_test-1.1.5.tar.gz` & `tmp/mov_cli_test-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli_test-1.1.5.tar", last modified: Sat May 11 19:41:16 2024, max compression
+gzip compressed data, was "mov_cli_test-1.1.6.tar", last modified: Sun May 26 17:20:10 2024, max compression
```

## Comparing `mov_cli_test-1.1.5.tar` & `mov_cli_test-1.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-11 19:41:16.897625 mov_cli_test-1.1.5/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1062 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/LICENSE
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2962 2024-05-11 19:41:16.897625 mov_cli_test-1.1.5/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)      532 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/README.md
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-11 19:41:16.894291 mov_cli_test-1.1.5/mov_cli_test/
--rw-r--r--   0 ananas    (1000) ananas    (1000)      350 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/mov_cli_test/__init__.py
--rw-r--r--   0 ananas    (1000) ananas    (1000)     4735 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/mov_cli_test/scraper.py
-drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-11 19:41:16.894291 mov_cli_test-1.1.5/mov_cli_test.egg-info/
--rw-r--r--   0 ananas    (1000) ananas    (1000)     2962 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/PKG-INFO
--rw-r--r--   0 ananas    (1000) ananas    (1000)      260 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/SOURCES.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/dependency_links.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)      117 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/requires.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)       13 2024-05-11 19:41:16.000000 mov_cli_test-1.1.5/mov_cli_test.egg-info/top_level.txt
--rw-r--r--   0 ananas    (1000) ananas    (1000)     1398 2024-05-11 19:41:05.000000 mov_cli_test-1.1.5/pyproject.toml
--rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-11 19:41:16.897625 mov_cli_test-1.1.5/setup.cfg
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-26 17:20:10.090094 mov_cli_test-1.1.6/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1062 2024-05-26 17:19:09.000000 mov_cli_test-1.1.6/LICENSE
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2816 2024-05-26 17:20:10.090094 mov_cli_test-1.1.6/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      532 2024-05-26 17:19:09.000000 mov_cli_test-1.1.6/README.md
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-26 17:20:10.086761 mov_cli_test-1.1.6/mov_cli_test/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      350 2024-05-26 17:19:24.000000 mov_cli_test-1.1.6/mov_cli_test/__init__.py
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     4735 2024-05-26 17:19:09.000000 mov_cli_test-1.1.6/mov_cli_test/scraper.py
+drwxr-xr-x   0 ananas    (1000) ananas    (1000)        0 2024-05-26 17:20:10.086761 mov_cli_test-1.1.6/mov_cli_test.egg-info/
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     2816 2024-05-26 17:20:10.000000 mov_cli_test-1.1.6/mov_cli_test.egg-info/PKG-INFO
+-rw-r--r--   0 ananas    (1000) ananas    (1000)      260 2024-05-26 17:20:10.000000 mov_cli_test-1.1.6/mov_cli_test.egg-info/SOURCES.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)        1 2024-05-26 17:20:10.000000 mov_cli_test-1.1.6/mov_cli_test.egg-info/dependency_links.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       28 2024-05-26 17:20:10.000000 mov_cli_test-1.1.6/mov_cli_test.egg-info/requires.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       13 2024-05-26 17:20:10.000000 mov_cli_test-1.1.6/mov_cli_test.egg-info/top_level.txt
+-rw-r--r--   0 ananas    (1000) ananas    (1000)     1286 2024-05-26 17:19:09.000000 mov_cli_test-1.1.6/pyproject.toml
+-rw-r--r--   0 ananas    (1000) ananas    (1000)       38 2024-05-26 17:20:10.090094 mov_cli_test-1.1.6/setup.cfg
```

### Comparing `mov_cli_test-1.1.5/LICENSE` & `mov_cli_test-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli_test-1.1.5/PKG-INFO` & `mov_cli_test-1.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-test
-Version: 1.1.5
+Version: 1.1.6
 Summary: A mov-cli plugin that let's you test mov-cli's capabilities by watching free films and animations in the creative commons.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 Goldy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,19 +35,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.2
 Requires-Dist: pytubefix
-Requires-Dist: devgoldyutils>=2.5.8
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-test
```

### Comparing `mov_cli_test-1.1.5/README.md` & `mov_cli_test-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mov_cli_test-1.1.5/mov_cli_test/scraper.py` & `mov_cli_test-1.1.6/mov_cli_test/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli_test-1.1.5/mov_cli_test.egg-info/PKG-INFO` & `mov_cli_test-1.1.6/mov_cli_test.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli-test
-Version: 1.1.5
+Version: 1.1.6
 Summary: A mov-cli plugin that let's you test mov-cli's capabilities by watching free films and animations in the creative commons.
 Author-email: Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 Goldy
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,19 +35,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.2
 Requires-Dist: pytubefix
-Requires-Dist: devgoldyutils>=2.5.8
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: build; extra == "dev"
 
 <div align="center">
 
   # mov-cli-test
```

### Comparing `mov_cli_test-1.1.5/pyproject.toml` & `mov_cli_test-1.1.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,15 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
 	'Programming Language :: Python :: 3.11'
 ]
 dependencies = [
-    "requests",
-    "importlib-metadata; python_version<'3.8'",
-
-    "mov-cli>=4.2",
-    "pytubefix",
-    "devgoldyutils>=2.5.8"
+    "pytubefix"
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "ruff",
@@ -45,8 +40,8 @@
 version = { attr = "mov_cli_test.__version__" }
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
-include = ["mov_cli_test*"]
+include = ["mov_cli_test*"]
```

