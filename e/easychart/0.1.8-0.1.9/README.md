# Comparing `tmp/easychart-0.1.8.tar.gz` & `tmp/easychart-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easychart-0.1.8.tar", last modified: Sat Oct 31 16:31:38 2020, max compression
+gzip compressed data, was "dist/easychart-0.1.9.tar", last modified: Sat Nov  7 19:41:49 2020, max compression
```

## Comparing `easychart-0.1.8.tar` & `easychart-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-10-31 16:31:38.000000 easychart-0.1.8/
--rw-r--r--   0 dschenck   (501) staff       (20)      118 2020-08-24 21:41:46.000000 easychart-0.1.8/MANIFEST.in
--rw-r--r--   0 dschenck   (501) staff       (20)      632 2020-10-31 16:31:38.000000 easychart-0.1.8/PKG-INFO
--rw-r--r--   0 dschenck   (501) staff       (20)      142 2020-08-09 12:48:36.000000 easychart-0.1.8/README.md
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-10-31 16:31:38.000000 easychart-0.1.8/easychart/
--rw-r--r--   0 dschenck   (501) staff       (20)     2766 2020-10-31 16:19:28.000000 easychart-0.1.8/easychart/__init__.py
--rw-r--r--   0 dschenck   (501) staff       (20)      820 2020-10-29 12:01:07.000000 easychart-0.1.8/easychart/config.json
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-10-31 16:31:38.000000 easychart-0.1.8/easychart/datasets/
--rw-r--r--   0 dschenck   (501) staff       (20)     6148 2020-08-15 17:36:44.000000 easychart-0.1.8/easychart/datasets/.DS_Store
--rw-r--r--   0 dschenck   (501) staff       (20)  1676975 2020-08-16 09:10:43.000000 easychart-0.1.8/easychart/datasets/S&P500.csv
--rw-r--r--   0 dschenck   (501) staff       (20)     1347 2020-08-21 21:36:09.000000 easychart-0.1.8/easychart/datasets/__init__.py
--rwxr-xr-x   0 dschenck   (501) staff       (20)  3192560 2019-09-20 15:24:26.000000 easychart-0.1.8/easychart/datasets/diamonds.csv
--rw-r--r--   0 dschenck   (501) staff       (20)    18596 2020-08-15 20:47:27.000000 easychart-0.1.8/easychart/datasets/electricity.csv
--rw-r--r--   0 dschenck   (501) staff       (20)  3502257 2020-08-13 22:32:02.000000 easychart-0.1.8/easychart/datasets/olympics.csv
--rw-r--r--   0 dschenck   (501) staff       (20)      413 2020-08-21 21:35:35.000000 easychart-0.1.8/easychart/datasets/populations.csv
--rw-r--r--   0 dschenck   (501) staff       (20)   513998 2020-07-19 17:15:21.000000 easychart-0.1.8/easychart/datasets/stocks.csv
--rw-r--r--   0 dschenck   (501) staff       (20)    13092 2020-08-15 16:37:11.000000 easychart-0.1.8/easychart/datasets/unemployment.csv
--rw-r--r--   0 dschenck   (501) staff       (20)     1152 2020-08-23 10:43:00.000000 easychart-0.1.8/easychart/encoders.py
--rw-r--r--   0 dschenck   (501) staff       (20)      442 2020-10-29 11:13:58.000000 easychart-0.1.8/easychart/internals.py
--rw-r--r--   0 dschenck   (501) staff       (20)     1040 2020-08-23 11:52:17.000000 easychart-0.1.8/easychart/ipynb.py
--rw-r--r--   0 dschenck   (501) staff       (20)    13321 2020-10-31 16:30:27.000000 easychart-0.1.8/easychart/models.py
--rw-r--r--   0 dschenck   (501) staff       (20)     1249 2020-08-23 11:29:38.000000 easychart-0.1.8/easychart/template.html
--rw-r--r--   0 dschenck   (501) staff       (20)     2773 2020-08-23 11:53:51.000000 easychart-0.1.8/easychart/templating.py
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-10-31 16:31:38.000000 easychart-0.1.8/easychart/themes/
--rw-r--r--   0 dschenck   (501) staff       (20)     6148 2020-08-23 11:08:09.000000 easychart-0.1.8/easychart/themes/.DS_Store
--rwxr-xr-x   0 dschenck   (501) staff       (20)     1764 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/538.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)     1460 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/alone.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)     2113 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/bloom.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)     1431 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/db.json
--rw-r--r--   0 dschenck   (501) staff       (20)     3004 2020-09-10 20:23:50.000000 easychart-0.1.8/easychart/themes/easychart.json
--rw-r--r--   0 dschenck   (501) staff       (20)     1908 2020-08-23 11:04:51.000000 easychart-0.1.8/easychart/themes/economist.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)      789 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/elementary.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)      885 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/ffx.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)      819 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/flat.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)     1311 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/flatdark.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)     1800 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/ft.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)     1317 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/ggplot2.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)      742 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/google.json
--rw-r--r--   0 dschenck   (501) staff       (20)       36 2020-08-23 11:16:15.000000 easychart-0.1.8/easychart/themes/highcharts.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)      931 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/monokai.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)      364 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/null.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)     1338 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/smpl.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)     1440 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/superheroes.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)      456 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/tufte.json
--rwxr-xr-x   0 dschenck   (501) staff       (20)      487 2020-04-16 08:44:22.000000 easychart-0.1.8/easychart/themes/tufte2.json
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-10-31 16:31:38.000000 easychart-0.1.8/easychart.egg-info/
--rw-r--r--   0 dschenck   (501) staff       (20)      632 2020-10-31 16:31:37.000000 easychart-0.1.8/easychart.egg-info/PKG-INFO
--rw-r--r--   0 dschenck   (501) staff       (20)     1304 2020-10-31 16:31:38.000000 easychart-0.1.8/easychart.egg-info/SOURCES.txt
--rw-r--r--   0 dschenck   (501) staff       (20)        1 2020-10-31 16:31:37.000000 easychart-0.1.8/easychart.egg-info/dependency_links.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       22 2020-10-31 16:31:37.000000 easychart-0.1.8/easychart.egg-info/requires.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       16 2020-10-31 16:31:37.000000 easychart-0.1.8/easychart.egg-info/top_level.txt
--rw-r--r--   0 dschenck   (501) staff       (20)       38 2020-10-31 16:31:38.000000 easychart-0.1.8/setup.cfg
--rw-r--r--   0 dschenck   (501) staff       (20)      716 2020-10-31 09:43:52.000000 easychart-0.1.8/setup.py
-drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-10-31 16:31:38.000000 easychart-0.1.8/tests/
--rw-r--r--   0 dschenck   (501) staff       (20)        0 2020-10-29 11:24:51.000000 easychart-0.1.8/tests/__init__.py
--rw-r--r--   0 dschenck   (501) staff       (20)      290 2020-10-29 11:25:30.000000 easychart-0.1.8/tests/internals.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-11-07 19:41:49.000000 easychart-0.1.9/
+-rw-r--r--   0 dschenck   (501) staff       (20)      118 2020-08-24 21:41:46.000000 easychart-0.1.9/MANIFEST.in
+-rw-r--r--   0 dschenck   (501) staff       (20)      632 2020-11-07 19:41:49.000000 easychart-0.1.9/PKG-INFO
+-rw-r--r--   0 dschenck   (501) staff       (20)      142 2020-08-09 12:48:36.000000 easychart-0.1.9/README.md
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-11-07 19:41:48.000000 easychart-0.1.9/easychart/
+-rw-r--r--   0 dschenck   (501) staff       (20)     2777 2020-11-07 19:12:55.000000 easychart-0.1.9/easychart/__init__.py
+-rw-r--r--   0 dschenck   (501) staff       (20)       21 2020-11-07 19:34:28.000000 easychart-0.1.9/easychart/__meta__.py
+-rw-r--r--   0 dschenck   (501) staff       (20)      820 2020-10-29 12:01:07.000000 easychart-0.1.9/easychart/config.json
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-11-07 19:41:49.000000 easychart-0.1.9/easychart/datasets/
+-rw-r--r--   0 dschenck   (501) staff       (20)     6148 2020-08-15 17:36:44.000000 easychart-0.1.9/easychart/datasets/.DS_Store
+-rw-r--r--   0 dschenck   (501) staff       (20)  1676975 2020-08-16 09:10:43.000000 easychart-0.1.9/easychart/datasets/S&P500.csv
+-rw-r--r--   0 dschenck   (501) staff       (20)     1347 2020-08-21 21:36:09.000000 easychart-0.1.9/easychart/datasets/__init__.py
+-rwxr-xr-x   0 dschenck   (501) staff       (20)  3192560 2019-09-20 15:24:26.000000 easychart-0.1.9/easychart/datasets/diamonds.csv
+-rw-r--r--   0 dschenck   (501) staff       (20)    18596 2020-08-15 20:47:27.000000 easychart-0.1.9/easychart/datasets/electricity.csv
+-rw-r--r--   0 dschenck   (501) staff       (20)  3502257 2020-08-13 22:32:02.000000 easychart-0.1.9/easychart/datasets/olympics.csv
+-rw-r--r--   0 dschenck   (501) staff       (20)      413 2020-08-21 21:35:35.000000 easychart-0.1.9/easychart/datasets/populations.csv
+-rw-r--r--   0 dschenck   (501) staff       (20)   513998 2020-07-19 17:15:21.000000 easychart-0.1.9/easychart/datasets/stocks.csv
+-rw-r--r--   0 dschenck   (501) staff       (20)    13092 2020-08-15 16:37:11.000000 easychart-0.1.9/easychart/datasets/unemployment.csv
+-rw-r--r--   0 dschenck   (501) staff       (20)     1808 2020-11-07 18:12:42.000000 easychart-0.1.9/easychart/encoders.py
+-rw-r--r--   0 dschenck   (501) staff       (20)      442 2020-10-29 11:13:58.000000 easychart-0.1.9/easychart/internals.py
+-rw-r--r--   0 dschenck   (501) staff       (20)     1040 2020-08-23 11:52:17.000000 easychart-0.1.9/easychart/ipynb.py
+-rw-r--r--   0 dschenck   (501) staff       (20)    14388 2020-11-07 19:32:59.000000 easychart-0.1.9/easychart/models.py
+-rw-r--r--   0 dschenck   (501) staff       (20)     1249 2020-08-23 11:29:38.000000 easychart-0.1.9/easychart/template.html
+-rw-r--r--   0 dschenck   (501) staff       (20)     2824 2020-11-07 18:33:30.000000 easychart-0.1.9/easychart/templating.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-11-07 19:41:49.000000 easychart-0.1.9/easychart/themes/
+-rw-r--r--   0 dschenck   (501) staff       (20)     6148 2020-08-23 11:08:09.000000 easychart-0.1.9/easychart/themes/.DS_Store
+-rwxr-xr-x   0 dschenck   (501) staff       (20)     1764 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/538.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)     1460 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/alone.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)     2113 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/bloom.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)     1431 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/db.json
+-rw-r--r--   0 dschenck   (501) staff       (20)     3004 2020-09-10 20:23:50.000000 easychart-0.1.9/easychart/themes/easychart.json
+-rw-r--r--   0 dschenck   (501) staff       (20)     1908 2020-08-23 11:04:51.000000 easychart-0.1.9/easychart/themes/economist.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)      789 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/elementary.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)      885 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/ffx.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)      819 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/flat.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)     1311 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/flatdark.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)     1800 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/ft.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)     1317 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/ggplot2.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)      742 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/google.json
+-rw-r--r--   0 dschenck   (501) staff       (20)       36 2020-08-23 11:16:15.000000 easychart-0.1.9/easychart/themes/highcharts.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)      931 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/monokai.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)      364 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/null.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)     1338 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/smpl.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)     1440 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/superheroes.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)      456 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/tufte.json
+-rwxr-xr-x   0 dschenck   (501) staff       (20)      487 2020-04-16 08:44:22.000000 easychart-0.1.9/easychart/themes/tufte2.json
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-11-07 19:41:49.000000 easychart-0.1.9/easychart.egg-info/
+-rw-r--r--   0 dschenck   (501) staff       (20)      632 2020-11-07 19:41:48.000000 easychart-0.1.9/easychart.egg-info/PKG-INFO
+-rw-r--r--   0 dschenck   (501) staff       (20)     1326 2020-11-07 19:41:48.000000 easychart-0.1.9/easychart.egg-info/SOURCES.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)        1 2020-11-07 19:41:48.000000 easychart-0.1.9/easychart.egg-info/dependency_links.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       33 2020-11-07 19:41:48.000000 easychart-0.1.9/easychart.egg-info/requires.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       16 2020-11-07 19:41:48.000000 easychart-0.1.9/easychart.egg-info/top_level.txt
+-rw-r--r--   0 dschenck   (501) staff       (20)       38 2020-11-07 19:41:49.000000 easychart-0.1.9/setup.cfg
+-rw-r--r--   0 dschenck   (501) staff       (20)      729 2020-11-07 19:41:45.000000 easychart-0.1.9/setup.py
+drwxr-xr-x   0 dschenck   (501) staff       (20)        0 2020-11-07 19:41:49.000000 easychart-0.1.9/tests/
+-rw-r--r--   0 dschenck   (501) staff       (20)        0 2020-10-29 11:24:51.000000 easychart-0.1.9/tests/__init__.py
+-rw-r--r--   0 dschenck   (501) staff       (20)      290 2020-10-29 11:25:30.000000 easychart-0.1.9/tests/internals.py
```

### Comparing `easychart-0.1.8/PKG-INFO` & `easychart-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easychart
-Version: 0.1.8
+Version: 0.1.9
 Summary: Highcharts meets python
 Home-page: https://easychart.readthedocs.io/en/latest/
 Author: david.schenck@outlook.com
 Author-email: david.schenck@outlook.com
 License: UNKNOWN
 Description: # easychart
         highcharts meets python
```

### Comparing `easychart-0.1.8/easychart/__init__.py` & `easychart-0.1.9/easychart/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from easychart.models import Chart, Plot, Grid
+from easychart.__meta__ import * 
 
 import easychart.ipynb
 import easychart.datasets as datasets
 
-__version__ = "0.1.8"
-
-def new(*, type=None, datetime=False, zoom="x", tooltip=None, title=None, subtitle=None, 
+def new(type=None, *, datetime=False, zoom="x", tooltip=None, title=None, subtitle=None, 
         xtitle=None, ytitle=None, xformat=None, yformat=None, ymin=None, ymax=None,
         legend=None, categories=None):
     """
     Creates a new chart with some preset defaults
 
     Parameters
     ------------------
```

### Comparing `easychart-0.1.8/easychart/config.json` & `easychart-0.1.9/easychart/config.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/datasets/.DS_Store` & `easychart-0.1.9/easychart/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/datasets/S&P500.csv` & `easychart-0.1.9/easychart/datasets/S&P500.csv`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/datasets/__init__.py` & `easychart-0.1.9/easychart/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/datasets/diamonds.csv` & `easychart-0.1.9/easychart/datasets/diamonds.csv`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/datasets/electricity.csv` & `easychart-0.1.9/easychart/datasets/electricity.csv`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/datasets/olympics.csv` & `easychart-0.1.9/easychart/datasets/olympics.csv`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/datasets/stocks.csv` & `easychart-0.1.9/easychart/datasets/stocks.csv`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/datasets/unemployment.csv` & `easychart-0.1.9/easychart/datasets/unemployment.csv`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/encoders.py` & `easychart-0.1.9/easychart/encoders.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,55 @@
 import json
+import collections
 import numpy as np
 import pandas as pd
 import datetime
 import easychart
 import easytree
 
+def default(value):
+    """
+    JSON default encoder function for non-standard objects
+
+    Example
+    -------------------------
+    >>> json.dumps([pd.Timestamp(2020,4,20)], default=default)
+    [2020-04-20]
+    """
+    if isinstance(value, (easychart.Chart, easytree.Tree)):
+        return value.serialize()
+    if isinstance(value, (pd.Timestamp, datetime.datetime)):
+        if value == value.replace(hour=0, minute=0, second=0): 
+            return value.strftime("%Y-%m-%d")
+        return value.strftime("%Y-%m-%d %H:%M:%S.%f")
+    if isinstance(value, datetime.date):
+        return value.strftime("%Y-%m-%d")
+    if isinstance(value, np.datetime64):
+        return pd.Timestamp(value.astype(int))
+    if isinstance(value, np.ndarray):
+        return value.tolist()
+    if isinstance(value, (np.int64, np.int32, np.int16, np.int8, np.int_)):
+        return int(value)
+    if isinstance(value, (np.double, np.float64, np.float_)):
+        return float(value)
+    if isinstance(value, (pd.DataFrame, pd.Series, pd.Index)): 
+        return value.values.tolist()
+    if isinstance(value, (collections.abc.KeysView, collections.abc.ValuesView, collections.abc.ItemsView)): 
+        return list(value)
+    raise TypeError(f"Object of type '{type(value).__name__}' is not JSON serializable")
+
 class Encoder(json.JSONEncoder):
+    """
+    JSON default encoder class
+
+    Note
+    -------------------------
+    simplejson recommends passing a default function rather than
+    a default encoding class
+
+    Example
+    -------------------------
+    >>> json.dumps([pd.Timestamp(2020,4,20)], cls=Encoder)
+    [2020-04-20]
+    """
     def default(self, value):
-        if isinstance(value, (easychart.Chart, easytree.Tree)):
-            return self.default(value.serialize())
-        if isinstance(value, (pd.Timestamp, datetime.datetime)):
-            if value == value.replace(hour=0, minute=0, second=0): 
-                return value.strftime("%Y-%m-%d")
-            return value.strftime("%Y-%m-%d %H:%M:%S.%f")
-        if isinstance(value, datetime.date):
-            return value.strftime("%Y-%m-%d")
-        if isinstance(value, np.datetime64):
-            return self.default(pd.Timestamp(value.astype(int)))
-        if isinstance(value, np.ndarray):
-            return value.tolist()
-        if isinstance(value, (np.int64, np.int32, np.int16, np.int8, np.int_)):
-            return int(value)
-        if isinstance(value, (np.double, np.float64, np.float_)):
-            return float(value)
-        if isinstance(value, (pd.DataFrame, pd.Series, pd.Index)): 
-            return value.values.tolist()
-        return super().default(value)
+        return default(value)
```

### Comparing `easychart-0.1.8/easychart/ipynb.py` & `easychart-0.1.9/easychart/ipynb.py`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/models.py` & `easychart-0.1.9/easychart/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 import easytree
 import pandas as pd
 import numpy as np
 import datetime
-import json
+import simplejson
 import re
 
 import easychart.encoders as encoders
 import easychart.internals as internals
 
 class SeriesCollection(easytree.Tree): 
     """
     Series collection
     """
     def append(self, data=None, **kwargs):
         if "legend" in kwargs:
             kwargs["showInLegend"] = kwargs.pop("legend")
-        if "marker" in kwargs and isinstance(kwargs["marker"], bool): 
-            kwargs["marker"] = {"enabled": kwargs["marker"]}
+        if "marker" in kwargs: 
+            if isinstance(kwargs["marker"], bool): 
+                kwargs["marker"] = {"enabled": kwargs["marker"]}
+            elif kwargs["marker"] is None: 
+                kwargs["marker"] = {"enabled": False}
         if "width" in kwargs: 
             kwargs["lineWidth"] = kwargs.pop("width")
         if "dash" in kwargs: 
             kwargs["dashStyle"] = kwargs.pop("dash")
         if "dashstyle" in kwargs: 
             kwargs["dashStyle"] = kwargs.pop("dashstyle")
         if "linestyle" in kwargs: 
             kwargs["dashStyle"] = kwargs.pop("linestyle")
+        if "active" in kwargs: 
+            kwargs["visible"] = kwargs.pop("active")
+        if "enabled" in kwargs: 
+            kwargs["visible"] = kwargs.pop("enabled")
         if isinstance(data, (zip, range)):
             data = list(data)
         if isinstance(data, (list, tuple)):
             if "index" in kwargs:
                 index = kwargs.pop("index")
                 if all([isinstance(d, datetime.date) for d in index]):
                     data = [internals.flatten(internals.timestamp(d), v) for (d, v) in zip(index, data)]
@@ -78,14 +85,32 @@
 
     def __setattr__(self, name, value):
         if hasattr(self.__class__, f"set_{name}"): 
             getattr(self, f"set_{name}")(value)
             return 
         return super().__setattr__(name, value)
 
+    def set_type(self, value):
+        """
+        Shortcut for self.chart.type = value
+        """
+        self.chart.type = value
+
+    def set_height(self, value):
+        """
+        Shortcut for self.chart.height = value
+        """
+        self.chart.height = value
+
+    def set_width(self, value):
+        """
+        Shortcut for self.chart.width = value
+        """
+        self.chart.width = value
+
     def set_title(self, value):
         """
         Shortcut for self.title.text = value
         """ 
         if isinstance(value, str):
             self.title.text = value
             return 
@@ -175,14 +200,26 @@
         Set the xAxis as a datetime axis
         """
         if isinstance(value, bool) and value == True:
             self.xAxis.type = "datetime"
             return
         raise ValueError("Unexpected value for xAxis.type")
 
+    def set_marker(self, value):
+        """
+        Set the default marker
+        """
+        if isinstance(value, bool): 
+            self.plotOptions.series.marker.enabled = value
+            return
+        if value is None: 
+            self.plotOptions.series.marker.enabled = False
+            return
+        self.plotOptions.series.marker = value
+
     def append(self, data=None, **kwargs):
         """
         Shortcut for :code:`chart.series.append(data, **kwargs)`
         """
         return self.series.append(data, **kwargs)
 
     def plot(self, data=None, **kwargs):
@@ -279,15 +316,15 @@
         return Plot(self, width, height, theme)
         
     def save(self, filename, indent=0):
         """
         Serializes and saves the chart configuration to a JSON file
         """
         with open(filename, "w") as file: 
-            json.dump(self.serialize(), file, cls=encoders.Encoder, indent=indent)
+            simplejson.dump(self.serialize(), file, default=encoders.default, indent=indent)
         return
 
 class Plot: 
     """
     Chart container
     """
     def __init__(self, chart, width="100%", height="400px", theme=None):
```

### Comparing `easychart-0.1.8/easychart/template.html` & `easychart-0.1.9/easychart/template.html`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/templating.py` & `easychart-0.1.9/easychart/templating.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import json
 import html
+import simplejson
 import easychart
 import easychart.encoders
 import warnings
 
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 
 #create the environment 
@@ -56,11 +57,11 @@
 
     #get the template and render
     template = environment.get_template("template.html")
 
     return template.render(
             scripts=config["scripts"], 
             stylesheets=config["stylesheets"],
-            theme=json.dumps(grid.theme), 
-            plots=json.dumps([plot.serialize() for plot in grid.plots], 
-                              cls=easychart.encoders.Encoder))
+            theme=simplejson.dumps(grid.theme), 
+            plots=simplejson.dumps([plot.serialize() for plot in grid.plots], 
+                              default=easychart.encoders.default, ignore_nan=True))
```

### Comparing `easychart-0.1.8/easychart/themes/.DS_Store` & `easychart-0.1.9/easychart/themes/.DS_Store`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/538.json` & `easychart-0.1.9/easychart/themes/538.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/alone.json` & `easychart-0.1.9/easychart/themes/alone.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/bloom.json` & `easychart-0.1.9/easychart/themes/bloom.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/db.json` & `easychart-0.1.9/easychart/themes/db.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/easychart.json` & `easychart-0.1.9/easychart/themes/easychart.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/economist.json` & `easychart-0.1.9/easychart/themes/economist.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/elementary.json` & `easychart-0.1.9/easychart/themes/elementary.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/ffx.json` & `easychart-0.1.9/easychart/themes/ffx.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/flat.json` & `easychart-0.1.9/easychart/themes/flat.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/flatdark.json` & `easychart-0.1.9/easychart/themes/flatdark.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/ft.json` & `easychart-0.1.9/easychart/themes/ft.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/ggplot2.json` & `easychart-0.1.9/easychart/themes/ggplot2.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/google.json` & `easychart-0.1.9/easychart/themes/google.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/monokai.json` & `easychart-0.1.9/easychart/themes/monokai.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/smpl.json` & `easychart-0.1.9/easychart/themes/smpl.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart/themes/superheroes.json` & `easychart-0.1.9/easychart/themes/superheroes.json`

 * *Files identical despite different names*

### Comparing `easychart-0.1.8/easychart.egg-info/PKG-INFO` & `easychart-0.1.9/easychart.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easychart
-Version: 0.1.8
+Version: 0.1.9
 Summary: Highcharts meets python
 Home-page: https://easychart.readthedocs.io/en/latest/
 Author: david.schenck@outlook.com
 Author-email: david.schenck@outlook.com
 License: UNKNOWN
 Description: # easychart
         highcharts meets python
```

### Comparing `easychart-0.1.8/easychart.egg-info/SOURCES.txt` & `easychart-0.1.9/easychart.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 setup.py
 easychart/__init__.py
+easychart/__meta__.py
 easychart/config.json
 easychart/encoders.py
 easychart/internals.py
 easychart/ipynb.py
 easychart/models.py
 easychart/template.html
 easychart/templating.py
```

### Comparing `easychart-0.1.8/setup.py` & `easychart-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="easychart",
-    version="0.1.8",
+    version="0.1.9",
     author="david.schenck@outlook.com",
     author_email="david.schenck@outlook.com",
     description="Highcharts meets python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://easychart.readthedocs.io/en/latest/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=["pandas","numpy","easytree"],
+    install_requires=["pandas","numpy","easytree","simplejson"],
     include_package_data=True
 )
```

