# Comparing `tmp/wikipathway2genes-0.0.3.tar.gz` & `tmp/wikipathway2genes-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikipathway2genes-0.0.3.tar", last modified: Sun May 26 18:08:48 2024, max compression
+gzip compressed data, was "wikipathway2genes-0.0.4.tar", last modified: Sun May 26 18:14:00 2024, max compression
```

## Comparing `wikipathway2genes-0.0.3.tar` & `wikipathway2genes-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:08:48.437424 wikipathway2genes-0.0.3/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      188 2024-05-26 18:08:48.437424 wikipathway2genes-0.0.3/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      380 2024-05-26 18:06:14.000000 wikipathway2genes-0.0.3/README.md
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-26 18:08:48.437424 wikipathway2genes-0.0.3/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      483 2024-05-26 18:08:17.000000 wikipathway2genes-0.0.3/setup.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:08:48.437424 wikipathway2genes-0.0.3/wikipathway2genes.egg-info/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      188 2024-05-26 18:08:48.000000 wikipathway2genes-0.0.3/wikipathway2genes.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      308 2024-05-26 18:08:48.000000 wikipathway2genes-0.0.3/wikipathway2genes.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-26 18:08:48.000000 wikipathway2genes-0.0.3/wikipathway2genes.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       61 2024-05-26 18:08:48.000000 wikipathway2genes-0.0.3/wikipathway2genes.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       24 2024-05-26 18:08:48.000000 wikipathway2genes-0.0.3/wikipathway2genes.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        9 2024-05-26 18:08:48.000000 wikipathway2genes-0.0.3/wikipathway2genes.egg-info/top_level.txt
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:08:48.437424 wikipathway2genes-0.0.3/wp2genes/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 wikipathway2genes-0.0.3/wp2genes/__init__.py
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1088 2024-05-26 17:26:59.000000 wikipathway2genes-0.0.3/wp2genes/wp2genes.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:14:00.357199 wikipathway2genes-0.0.4/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      609 2024-05-26 18:14:00.357199 wikipathway2genes-0.0.4/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      380 2024-05-26 18:12:34.000000 wikipathway2genes-0.0.4/README.md
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-26 18:14:00.357199 wikipathway2genes-0.0.4/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      581 2024-05-26 18:13:41.000000 wikipathway2genes-0.0.4/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:14:00.357199 wikipathway2genes-0.0.4/wikipathway2genes.egg-info/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      609 2024-05-26 18:14:00.000000 wikipathway2genes-0.0.4/wikipathway2genes.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      308 2024-05-26 18:14:00.000000 wikipathway2genes-0.0.4/wikipathway2genes.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-26 18:14:00.000000 wikipathway2genes-0.0.4/wikipathway2genes.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       61 2024-05-26 18:14:00.000000 wikipathway2genes-0.0.4/wikipathway2genes.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       24 2024-05-26 18:14:00.000000 wikipathway2genes-0.0.4/wikipathway2genes.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        9 2024-05-26 18:14:00.000000 wikipathway2genes-0.0.4/wikipathway2genes.egg-info/top_level.txt
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:14:00.357199 wikipathway2genes-0.0.4/wp2genes/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 wikipathway2genes-0.0.4/wp2genes/__init__.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1088 2024-05-26 17:26:59.000000 wikipathway2genes-0.0.4/wp2genes/wp2genes.py
```

### Comparing `wikipathway2genes-0.0.3/wp2genes/wp2genes.py` & `wikipathway2genes-0.0.4/wp2genes/wp2genes.py`

 * *Files identical despite different names*

