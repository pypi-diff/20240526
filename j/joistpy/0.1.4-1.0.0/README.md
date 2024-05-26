# Comparing `tmp/joistpy-0.1.4.tar.gz` & `tmp/joistpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joistpy-0.1.4.tar", last modified: Tue May 21 17:44:51 2024, max compression
+gzip compressed data, was "joistpy-1.0.0.tar", max compression
```

## Comparing `joistpy-0.1.4.tar` & `joistpy-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 17:44:51.550673 joistpy-0.1.4/
--rw-rw-rw-   0        0        0    35149 2024-05-21 15:08:39.000000 joistpy-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      475 2024-05-21 17:44:51.544502 joistpy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1403 2024-05-21 16:23:40.000000 joistpy-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 17:44:51.493038 joistpy-0.1.4/joistpy/
--rw-rw-rw-   0        0        0       24 2024-05-21 04:34:52.000000 joistpy-0.1.4/joistpy/__init__.py
--rw-rw-rw-   0        0        0     4996 2024-05-21 17:42:38.000000 joistpy-0.1.4/joistpy/joistpy.py
-drwxrwxrwx   0        0        0        0 2024-05-21 17:44:51.540193 joistpy-0.1.4/joistpy/property files/
--rw-rw-rw-   0        0        0    24559 2024-05-21 14:09:30.000000 joistpy-0.1.4/joistpy/property files/K_L_360.csv
--rw-rw-rw-   0        0        0    24416 2024-05-21 14:09:48.000000 joistpy-0.1.4/joistpy/property files/K_Total.csv
--rw-rw-rw-   0        0        0      602 2024-05-21 14:10:04.000000 joistpy-0.1.4/joistpy/property files/K_weight.csv
-drwxrwxrwx   0        0        0        0 2024-05-21 17:44:51.542881 joistpy-0.1.4/joistpy.egg-info/
--rw-rw-rw-   0        0        0      475 2024-05-21 17:44:51.000000 joistpy-0.1.4/joistpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2024-05-21 17:44:51.000000 joistpy-0.1.4/joistpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 17:44:51.000000 joistpy-0.1.4/joistpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-21 17:44:51.000000 joistpy-0.1.4/joistpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 17:44:51.551682 joistpy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      802 2024-05-21 17:44:36.000000 joistpy-0.1.4/setup.py
+-rw-r--r--   0        0        0       99 2024-05-26 04:42:25.628000 joistpy-1.0.0/joistpy/__init__.py
+-rw-r--r--   0        0        0    11236 2024-05-26 04:37:45.064211 joistpy-1.0.0/joistpy/joistpy.py
+-rw-r--r--   0        0        0    24559 2024-05-21 14:09:30.500655 joistpy-1.0.0/joistpy/property files/K_L_360.csv
+-rw-r--r--   0        0        0    24416 2024-05-21 14:09:48.663660 joistpy-1.0.0/joistpy/property files/K_Total.csv
+-rw-r--r--   0        0        0      602 2024-05-21 14:10:04.118254 joistpy-1.0.0/joistpy/property files/K_weight.csv
+-rw-r--r--   0        0        0     1092 2024-05-26 04:17:22.849982 joistpy-1.0.0/LICENSE
+-rw-r--r--   0        0        0      475 2024-05-26 01:27:35.420825 joistpy-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1404 2024-05-26 04:57:24.863872 joistpy-1.0.0/README.md
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 joistpy-1.0.0/PKG-INFO
```

### Comparing `joistpy-0.1.4/joistpy/property files/K_L_360.csv` & `joistpy-1.0.0/joistpy/property files/K_L_360.csv`

 * *Files identical despite different names*

### Comparing `joistpy-0.1.4/joistpy/property files/K_Total.csv` & `joistpy-1.0.0/joistpy/property files/K_Total.csv`

 * *Files identical despite different names*

### Comparing `joistpy-0.1.4/joistpy/property files/K_weight.csv` & `joistpy-1.0.0/joistpy/property files/K_weight.csv`

 * *Files identical despite different names*

