# Comparing `tmp/scocli-1.2.tar.gz` & `tmp/scocli-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scocli-1.2.tar", last modified: Tue May 21 00:15:36 2024, max compression
+gzip compressed data, was "scocli-1.3.1.tar", last modified: Sun May 26 17:45:33 2024, max compression
```

## Comparing `scocli-1.2.tar` & `scocli-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-21 00:15:36.142665 scocli-1.2/
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      187 2024-05-21 00:15:36.142665 scocli-1.2/PKG-INFO
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      468 2024-04-10 14:37:41.000000 scocli-1.2/README.md
-drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-21 00:15:36.142665 scocli-1.2/sco/
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        0 2024-04-10 14:37:41.000000 scocli-1.2/sco/__init__.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     5095 2024-05-21 00:07:37.000000 scocli-1.2/sco/addResource.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     4334 2024-05-21 00:07:37.000000 scocli-1.2/sco/build.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     1131 2024-05-21 00:07:37.000000 scocli-1.2/sco/bundle.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     4537 2024-05-21 00:07:37.000000 scocli-1.2/sco/checkManifest.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     2270 2024-05-21 00:07:37.000000 scocli-1.2/sco/organizeManifest.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     2284 2024-05-21 00:07:37.000000 scocli-1.2/sco/removeResource.py
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     1047 2024-05-21 00:07:37.000000 scocli-1.2/sco/seeManifest.py
-drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-21 00:15:36.142665 scocli-1.2/scocli.egg-info/
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      187 2024-05-21 00:15:36.000000 scocli-1.2/scocli.egg-info/PKG-INFO
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      286 2024-05-21 00:15:36.000000 scocli-1.2/scocli.egg-info/SOURCES.txt
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        1 2024-05-21 00:15:36.000000 scocli-1.2/scocli.egg-info/dependency_links.txt
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        4 2024-05-21 00:15:36.000000 scocli-1.2/scocli.egg-info/top_level.txt
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)       38 2024-05-21 00:15:36.142665 scocli-1.2/setup.cfg
--rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      467 2024-05-21 00:07:37.000000 scocli-1.2/setup.py
+drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-26 17:45:33.356734 scocli-1.3.1/
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      189 2024-05-26 17:45:33.356734 scocli-1.3.1/PKG-INFO
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      468 2024-04-10 14:37:41.000000 scocli-1.3.1/README.md
+drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-26 17:45:33.356734 scocli-1.3.1/sco/
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        0 2024-04-10 14:37:41.000000 scocli-1.3.1/sco/__init__.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     5095 2024-05-26 17:34:59.000000 scocli-1.3.1/sco/addResource.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     4334 2024-05-26 17:34:59.000000 scocli-1.3.1/sco/build.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     1131 2024-05-26 17:34:59.000000 scocli-1.3.1/sco/bundle.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     4537 2024-05-26 17:34:59.000000 scocli-1.3.1/sco/checkManifest.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     2270 2024-05-26 17:34:59.000000 scocli-1.3.1/sco/organizeManifest.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     2284 2024-05-26 17:34:59.000000 scocli-1.3.1/sco/removeResource.py
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)     1712 2024-05-26 17:40:30.000000 scocli-1.3.1/sco/seeManifest.py
+drwxrwxr-x   0 vasapg    (1000) vasapg    (1000)        0 2024-05-26 17:45:33.356734 scocli-1.3.1/scocli.egg-info/
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      189 2024-05-26 17:45:33.000000 scocli-1.3.1/scocli.egg-info/PKG-INFO
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      286 2024-05-26 17:45:33.000000 scocli-1.3.1/scocli.egg-info/SOURCES.txt
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        1 2024-05-26 17:45:33.000000 scocli-1.3.1/scocli.egg-info/dependency_links.txt
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)        4 2024-05-26 17:45:33.000000 scocli-1.3.1/scocli.egg-info/top_level.txt
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)       38 2024-05-26 17:45:33.356734 scocli-1.3.1/setup.cfg
+-rw-rw-r--   0 vasapg    (1000) vasapg    (1000)      469 2024-05-26 17:43:44.000000 scocli-1.3.1/setup.py
```

### Comparing `scocli-1.2/sco/addResource.py` & `scocli-1.3.1/sco/addResource.py`

 * *Files identical despite different names*

### Comparing `scocli-1.2/sco/build.py` & `scocli-1.3.1/sco/build.py`

 * *Files identical despite different names*

### Comparing `scocli-1.2/sco/bundle.py` & `scocli-1.3.1/sco/bundle.py`

 * *Files identical despite different names*

### Comparing `scocli-1.2/sco/checkManifest.py` & `scocli-1.3.1/sco/checkManifest.py`

 * *Files identical despite different names*

### Comparing `scocli-1.2/sco/organizeManifest.py` & `scocli-1.3.1/sco/organizeManifest.py`

 * *Files identical despite different names*

### Comparing `scocli-1.2/sco/removeResource.py` & `scocli-1.3.1/sco/removeResource.py`

 * *Files identical despite different names*

