# Comparing `tmp/getmeta-0.6.3.tar.gz` & `tmp/getmeta-2024.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getmeta-0.6.3.tar", last modified: Mon Mar 13 00:15:03 2023, max compression
+gzip compressed data, was "getmeta-2024.5.25.tar", last modified: Sun May 26 01:53:49 2024, max compression
```

## Comparing `getmeta-0.6.3.tar` & `getmeta-2024.5.25.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 00:15:03.453598 getmeta-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-13 00:14:50.000000 getmeta-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-13 00:15:03.453598 getmeta-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-13 00:14:50.000000 getmeta-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 00:15:03.449598 getmeta-0.6.3/getmeta/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-13 00:14:50.000000 getmeta-0.6.3/getmeta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-13 00:14:50.000000 getmeta-0.6.3/getmeta/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-03-13 00:14:50.000000 getmeta-0.6.3/getmeta/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 00:15:03.453598 getmeta-0.6.3/getmeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-13 00:15:03.000000 getmeta-0.6.3/getmeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-13 00:15:03.000000 getmeta-0.6.3/getmeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 00:15:03.000000 getmeta-0.6.3/getmeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-13 00:15:03.000000 getmeta-0.6.3/getmeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 00:15:03.000000 getmeta-0.6.3/getmeta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-13 00:15:03.000000 getmeta-0.6.3/getmeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-13 00:15:03.000000 getmeta-0.6.3/getmeta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 00:15:03.453598 getmeta-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-13 00:14:50.000000 getmeta-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:53:49.498929 getmeta-2024.5.25/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 01:53:41.000000 getmeta-2024.5.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-26 01:53:49.498929 getmeta-2024.5.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-26 01:53:41.000000 getmeta-2024.5.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:53:49.498929 getmeta-2024.5.25/getmeta/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-26 01:53:41.000000 getmeta-2024.5.25/getmeta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-26 01:53:41.000000 getmeta-2024.5.25/getmeta/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-05-26 01:53:41.000000 getmeta-2024.5.25/getmeta/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:53:49.498929 getmeta-2024.5.25/getmeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-26 01:53:49.000000 getmeta-2024.5.25/getmeta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 01:53:49.498929 getmeta-2024.5.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-26 01:53:41.000000 getmeta-2024.5.25/setup.py
```

### Comparing `getmeta-0.6.3/LICENSE` & `getmeta-2024.5.25/LICENSE`

 * *Files identical despite different names*

