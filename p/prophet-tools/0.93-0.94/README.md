# Comparing `tmp/prophet_tools-0.93.tar.gz` & `tmp/prophet_tools-0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophet_tools-0.93.tar", last modified: Wed Apr 24 22:15:48 2024, max compression
+gzip compressed data, was "prophet_tools-0.94.tar", last modified: Sun May 26 18:51:55 2024, max compression
```

## Comparing `prophet_tools-0.93.tar` & `prophet_tools-0.94.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 22:15:48.499544 prophet_tools-0.93/
--rw-rw-rw-   0        0        0      138 2024-04-24 22:15:48.499544 prophet_tools-0.93/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-09-29 07:18:11.000000 prophet_tools-0.93/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 22:15:48.495546 prophet_tools-0.93/prophet_tools/
--rw-rw-rw-   0        0        0        0 2024-04-23 19:32:58.000000 prophet_tools-0.93/prophet_tools/__init__.py
--rw-rw-rw-   0        0        0      149 2024-04-23 19:32:58.000000 prophet_tools-0.93/prophet_tools/auto_import.py
--rw-rw-rw-   0        0        0     1811 2024-04-23 19:32:58.000000 prophet_tools-0.93/prophet_tools/file_convertors.py
--rw-rw-rw-   0        0        0      268 2024-04-23 19:32:58.000000 prophet_tools-0.93/prophet_tools/how_to_import.py
--rw-rw-rw-   0        0        0     7501 2024-04-24 22:15:14.000000 prophet_tools-0.93/prophet_tools/my_functions.py
--rw-rw-rw-   0        0        0      463 2024-04-23 19:32:58.000000 prophet_tools-0.93/prophet_tools/parsing.py
--rw-rw-rw-   0        0        0     1287 2024-04-23 19:45:43.000000 prophet_tools-0.93/prophet_tools/terminal.py
--rw-rw-rw-   0        0        0     4164 2024-04-23 19:32:58.000000 prophet_tools-0.93/prophet_tools/всё_подряд.py
-drwxrwxrwx   0        0        0        0 2024-04-24 22:15:48.499544 prophet_tools-0.93/prophet_tools.egg-info/
--rw-rw-rw-   0        0        0      138 2024-04-24 22:15:48.000000 prophet_tools-0.93/prophet_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2024-04-24 22:15:48.000000 prophet_tools-0.93/prophet_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 22:15:48.000000 prophet_tools-0.93/prophet_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 19:48:57.000000 prophet_tools-0.93/prophet_tools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-04-24 22:15:48.000000 prophet_tools-0.93/prophet_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 22:15:48.500543 prophet_tools-0.93/setup.cfg
--rw-rw-rw-   0        0        0      241 2024-04-24 22:15:33.000000 prophet_tools-0.93/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:51:55.429113 prophet_tools-0.94/
+-rw-rw-rw-   0        0        0      138 2024-05-26 18:51:55.429113 prophet_tools-0.94/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-12-24 23:12:27.000000 prophet_tools-0.94/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 18:51:55.424698 prophet_tools-0.94/prophet_tools/
+-rw-rw-rw-   0        0        0        0 2024-02-12 01:43:39.000000 prophet_tools-0.94/prophet_tools/__init__.py
+-rw-rw-rw-   0        0        0      149 2023-12-24 23:12:27.000000 prophet_tools-0.94/prophet_tools/auto_import.py
+-rw-rw-rw-   0        0        0     1811 2024-03-16 17:13:15.000000 prophet_tools-0.94/prophet_tools/file_convertors.py
+-rw-rw-rw-   0        0        0      268 2024-02-12 01:41:06.000000 prophet_tools-0.94/prophet_tools/how_to_import.py
+-rw-rw-rw-   0        0        0     7558 2024-05-26 18:50:56.000000 prophet_tools-0.94/prophet_tools/my_functions.py
+-rw-rw-rw-   0        0        0      463 2024-02-12 01:56:50.000000 prophet_tools-0.94/prophet_tools/parsing.py
+-rw-rw-rw-   0        0        0     1287 2024-05-26 18:50:17.000000 prophet_tools-0.94/prophet_tools/terminal.py
+-rw-rw-rw-   0        0        0     4164 2023-12-29 20:12:13.000000 prophet_tools-0.94/prophet_tools/всё_подряд.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:51:55.428112 prophet_tools-0.94/prophet_tools.egg-info/
+-rw-rw-rw-   0        0        0      138 2024-05-26 18:51:55.000000 prophet_tools-0.94/prophet_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-05-26 18:51:55.000000 prophet_tools-0.94/prophet_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:51:55.000000 prophet_tools-0.94/prophet_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-12 01:48:06.000000 prophet_tools-0.94/prophet_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-05-26 18:51:55.000000 prophet_tools-0.94/prophet_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 18:51:55.430112 prophet_tools-0.94/setup.cfg
+-rw-rw-rw-   0        0        0      241 2024-05-26 18:51:49.000000 prophet_tools-0.94/setup.py
```

### Comparing `prophet_tools-0.93/prophet_tools/file_convertors.py` & `prophet_tools-0.94/prophet_tools/file_convertors.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.93/prophet_tools/my_functions.py` & `prophet_tools-0.94/prophet_tools/my_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,16 @@
             what = what.lower()
         if type(what) is list:
             what = what.copy()
             for i in range(len(what)):
                 what.insert(i, what.pop(i).lower())
         return what
 
+    if what == '' or where == '':
+        return False
     if ignore_case:
         what = clear_case(what)
         where = clear_case(where)
     if type(what) is type(where) is str:
         return what in where or where in what
     elif type(what) is str:
         for place in where:
```

### Comparing `prophet_tools-0.93/prophet_tools/terminal.py` & `prophet_tools-0.94/prophet_tools/terminal.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.93/prophet_tools/всё_подряд.py` & `prophet_tools-0.94/prophet_tools/всё_подряд.py`

 * *Files identical despite different names*

