# Comparing `tmp/centerline-1.1.0.tar.gz` & `tmp/centerline-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centerline-1.1.0.tar", last modified: Sat Feb 10 20:25:32 2024, max compression
+gzip compressed data, was "centerline-1.1.1.tar", last modified: Sun May 26 11:58:38 2024, max compression
```

## Comparing `centerline-1.1.0.tar` & `centerline-1.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.030321 centerline-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-10 20:25:07.000000 centerline-1.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-02-10 20:25:07.000000 centerline-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-10 20:25:07.000000 centerline-1.1.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-02-10 20:25:07.000000 centerline-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-10 20:25:07.000000 centerline-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-10 20:25:07.000000 centerline-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-02-10 20:25:32.030321 centerline-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-10 20:25:07.000000 centerline-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.022320 centerline-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.022320 centerline-1.1.0/docs/chapters/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/chapters/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/chapters/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/chapters/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/chapters/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/chapters/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.022320 centerline-1.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   119343 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/images/example.png
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.022320 centerline-1.1.0/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-10 20:25:07.000000 centerline-1.1.0/docs/modules/centerline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-10 20:25:07.000000 centerline-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-10 20:25:32.034320 centerline-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-10 20:25:07.000000 centerline-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.018320 centerline-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.026321 centerline-1.1.0/src/centerline/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-10 20:25:07.000000 centerline-1.1.0/src/centerline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-02-10 20:25:07.000000 centerline-1.1.0/src/centerline/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-10 20:25:07.000000 centerline-1.1.0/src/centerline/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-02-10 20:25:07.000000 centerline-1.1.0/src/centerline/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.030321 centerline-1.1.0/src/centerline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-02-10 20:25:32.000000 centerline-1.1.0/src/centerline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-10 20:25:32.000000 centerline-1.1.0/src/centerline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 20:25:32.000000 centerline-1.1.0/src/centerline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-10 20:25:32.000000 centerline-1.1.0/src/centerline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 20:25:31.000000 centerline-1.1.0/src/centerline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-10 20:25:32.000000 centerline-1.1.0/src/centerline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-10 20:25:32.000000 centerline-1.1.0/src/centerline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.026321 centerline-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.018320 centerline-1.1.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.030321 centerline-1.1.0/tests/data/geojson/
--rw-r--r--   0 runner    (1001) docker     (127)    37808 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/data/geojson/linestrings.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/data/geojson/points.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/data/geojson/polygons.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 20:25:32.030321 centerline-1.1.0/tests/data/shp/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/data/shp/polygons.cpg
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/data/shp/polygons.dbf
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/data/shp/polygons.prj
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/data/shp/polygons.qpj
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/data/shp/polygons.shp
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/data/shp/polygons.shx
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-02-10 20:25:07.000000 centerline-1.1.0/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-02-10 20:25:07.000000 centerline-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.030748 centerline-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-26 11:58:23.000000 centerline-1.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-26 11:58:23.000000 centerline-1.1.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-26 11:58:23.000000 centerline-1.1.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-26 11:58:23.000000 centerline-1.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-26 11:58:23.000000 centerline-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-26 11:58:23.000000 centerline-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-26 11:58:38.030748 centerline-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-26 11:58:23.000000 centerline-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.018748 centerline-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.022748 centerline-1.1.1/docs/chapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/chapters/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/chapters/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/chapters/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/chapters/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/chapters/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.022748 centerline-1.1.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   119343 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/images/example.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.022748 centerline-1.1.1/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-26 11:58:23.000000 centerline-1.1.1/docs/modules/centerline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-26 11:58:23.000000 centerline-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-26 11:58:38.030748 centerline-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-26 11:58:23.000000 centerline-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.018748 centerline-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.022748 centerline-1.1.1/src/centerline/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-26 11:58:23.000000 centerline-1.1.1/src/centerline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-26 11:58:23.000000 centerline-1.1.1/src/centerline/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-26 11:58:23.000000 centerline-1.1.1/src/centerline/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-26 11:58:23.000000 centerline-1.1.1/src/centerline/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.026748 centerline-1.1.1/src/centerline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-26 11:58:38.000000 centerline-1.1.1/src/centerline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-26 11:58:38.000000 centerline-1.1.1/src/centerline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:58:38.000000 centerline-1.1.1/src/centerline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-26 11:58:38.000000 centerline-1.1.1/src/centerline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:58:37.000000 centerline-1.1.1/src/centerline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-26 11:58:38.000000 centerline-1.1.1/src/centerline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 11:58:38.000000 centerline-1.1.1/src/centerline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.026748 centerline-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.018748 centerline-1.1.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.026748 centerline-1.1.1/tests/data/geojson/
+-rw-r--r--   0 runner    (1001) docker     (127)    37808 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/data/geojson/linestrings.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/data/geojson/points.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/data/geojson/polygons.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:58:38.026748 centerline-1.1.1/tests/data/shp/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/data/shp/polygons.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/data/shp/polygons.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/data/shp/polygons.prj
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/data/shp/polygons.qpj
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/data/shp/polygons.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/data/shp/polygons.shx
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-26 11:58:23.000000 centerline-1.1.1/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-26 11:58:23.000000 centerline-1.1.1/tox.ini
```

### Comparing `centerline-1.1.0/.readthedocs.yml` & `centerline-1.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/CHANGELOG.rst` & `centerline-1.1.1/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 
 The format is based on `Keep a Changelog <http://keepachangelog.com/>`_ and this project adheres to `Semantic Versioning <http://semver.org/>`_.
 
 Changes for the upcoming release can be found in the `changelog.d` directory in this repository. Do **NOT** add changelog entries here! This changelog is managed by `towncrier <https://github.com/hawkowl/towncrier>`_ and is compiled at release time.
 
 .. towncrier release notes start
 
+1.1.1 (2024-05-26)
+-------------------
+
+Bugfixes
+^^^^^^^^
+
+- Adding `predicate` as a named parameter in `str_tree.query` (`#47 <https://github.com/fitodic/centerline/pull/47>`_)
+
+
 1.1.0 (2024-02-10)
 -------------------
 
 Features
 ^^^^^^^^
 
 - Convert the centerline within check to use Shapely STRTrees (`#44 <https://github.com/fitodic/centerline/pull/44>`_)
```

### Comparing `centerline-1.1.0/CONTRIBUTING.rst` & `centerline-1.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/LICENSE` & `centerline-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/PKG-INFO` & `centerline-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centerline
-Version: 1.1.0
+Version: 1.1.1
 Summary: Calculate the centerline of a polygon
 Home-page: https://github.com/fitodic/centerline
 Download-URL: https://pypi.org/project/centerline/
 Author: Filip Todic
 Author-email: todic.filip@gmail.com
 License: MIT License
 Keywords: polygon,centerline,Voronoi
```

### Comparing `centerline-1.1.0/README.rst` & `centerline-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/docs/Makefile` & `centerline-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/docs/chapters/faq.rst` & `centerline-1.1.1/docs/chapters/faq.rst`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/docs/chapters/installation.rst` & `centerline-1.1.1/docs/chapters/installation.rst`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/docs/chapters/usage.rst` & `centerline-1.1.1/docs/chapters/usage.rst`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/docs/conf.py` & `centerline-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/docs/images/example.png` & `centerline-1.1.1/docs/images/example.png`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/docs/index.rst` & `centerline-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/docs/make.bat` & `centerline-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/docs/modules/centerline.rst` & `centerline-1.1.1/docs/modules/centerline.rst`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/pyproject.toml` & `centerline-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/setup.cfg` & `centerline-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/src/centerline/converters.py` & `centerline-1.1.1/src/centerline/converters.py`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/src/centerline/exceptions.py` & `centerline-1.1.1/src/centerline/exceptions.py`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/src/centerline/geometry.py` & `centerline-1.1.1/src/centerline/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,17 @@
                 ending_point = self._create_point_with_restored_coordinates(
                     x=vertices[ridge[1]][0], y=vertices[ridge[1]][1]
                 )
                 linestring = LineString((starting_point, ending_point))
                 linestrings.append(linestring)
 
         str_tree = STRtree(linestrings)
-        linestrings_indexes = str_tree.query(self._input_geometry, "contains")
+        linestrings_indexes = str_tree.query(
+            self._input_geometry, predicate="contains"
+        )
         contained_linestrings = [linestrings[i] for i in linestrings_indexes]
         if len(contained_linestrings) < 2:
             raise exceptions.TooFewRidgesError
 
         return unary_union(contained_linestrings)
 
     def _get_voronoi_vertices_and_ridges(self):
```

### Comparing `centerline-1.1.0/src/centerline.egg-info/PKG-INFO` & `centerline-1.1.1/src/centerline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centerline
-Version: 1.1.0
+Version: 1.1.1
 Summary: Calculate the centerline of a polygon
 Home-page: https://github.com/fitodic/centerline
 Download-URL: https://pypi.org/project/centerline/
 Author: Filip Todic
 Author-email: todic.filip@gmail.com
 License: MIT License
 Keywords: polygon,centerline,Voronoi
```

### Comparing `centerline-1.1.0/src/centerline.egg-info/SOURCES.txt` & `centerline-1.1.1/src/centerline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/tests/conftest.py` & `centerline-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/tests/data/geojson/linestrings.geojson` & `centerline-1.1.1/tests/data/geojson/linestrings.geojson`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/tests/data/geojson/points.geojson` & `centerline-1.1.1/tests/data/geojson/points.geojson`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/tests/data/geojson/polygons.geojson` & `centerline-1.1.1/tests/data/geojson/polygons.geojson`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/tests/data/shp/polygons.shp` & `centerline-1.1.1/tests/data/shp/polygons.shp`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/tests/test_geometry.py` & `centerline-1.1.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/tests/test_scripts.py` & `centerline-1.1.1/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `centerline-1.1.0/tox.ini` & `centerline-1.1.1/tox.ini`

 * *Files identical despite different names*

