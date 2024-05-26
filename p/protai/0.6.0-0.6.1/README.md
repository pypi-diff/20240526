# Comparing `tmp/protai-0.6.0.tar.gz` & `tmp/protai-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protai-0.6.0.tar", last modified: Sat May 25 22:44:57 2024, max compression
+gzip compressed data, was "protai-0.6.1.tar", last modified: Sun May 26 00:07:09 2024, max compression
```

## Comparing `protai-0.6.0.tar` & `protai-0.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 22:44:57.083592 protai-0.6.0/
--rw-rw-rw-   0        0        0     1107 2024-05-23 18:18:24.000000 protai-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     3293 2024-05-25 22:44:57.082593 protai-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2619 2024-05-23 23:24:58.000000 protai-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 22:44:57.060663 protai-0.6.0/protai/
--rw-rw-rw-   0        0        0        5 2024-05-25 22:42:27.000000 protai-0.6.0/protai/VERSION
--rw-rw-rw-   0        0        0       69 2024-05-23 18:18:24.000000 protai-0.6.0/protai/__init__.py
--rw-rw-rw-   0        0        0     4919 2024-05-25 22:43:02.000000 protai-0.6.0/protai/auth.py
--rw-rw-rw-   0        0        0     3253 2024-05-25 22:42:56.000000 protai-0.6.0/protai/protai.py
-drwxrwxrwx   0        0        0        0 2024-05-25 22:44:57.080450 protai-0.6.0/protai.egg-info/
--rw-rw-rw-   0        0        0     3293 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 22:44:57.083592 protai-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     4178 2024-05-23 18:18:24.000000 protai-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 00:07:09.648522 protai-0.6.1/
+-rw-rw-rw-   0        0        0     1107 2024-05-23 18:18:24.000000 protai-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     4512 2024-05-26 00:07:09.648522 protai-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3838 2024-05-26 00:01:50.000000 protai-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 00:07:09.620880 protai-0.6.1/protai/
+-rw-rw-rw-   0        0        0        5 2024-05-26 00:06:20.000000 protai-0.6.1/protai/VERSION
+-rw-rw-rw-   0        0        0       69 2024-05-23 18:18:24.000000 protai-0.6.1/protai/__init__.py
+-rw-rw-rw-   0        0        0     4919 2024-05-25 22:43:02.000000 protai-0.6.1/protai/auth.py
+-rw-rw-rw-   0        0        0     3253 2024-05-25 22:42:56.000000 protai-0.6.1/protai/protai.py
+drwxrwxrwx   0        0        0        0 2024-05-26 00:07:09.646382 protai-0.6.1/protai.egg-info/
+-rw-rw-rw-   0        0        0     4512 2024-05-26 00:07:09.000000 protai-0.6.1/protai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-26 00:07:09.000000 protai-0.6.1/protai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 00:07:09.000000 protai-0.6.1/protai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-26 00:07:09.000000 protai-0.6.1/protai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-05-26 00:07:09.000000 protai-0.6.1/protai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 00:07:09.000000 protai-0.6.1/protai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 00:07:09.649522 protai-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     4178 2024-05-23 18:18:24.000000 protai-0.6.1/setup.py
```

### Comparing `protai-0.6.0/LICENSE` & `protai-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `protai-0.6.0/protai/auth.py` & `protai-0.6.1/protai/auth.py`

 * *Files identical despite different names*

### Comparing `protai-0.6.0/protai/protai.py` & `protai-0.6.1/protai/protai.py`

 * *Files identical despite different names*

### Comparing `protai-0.6.0/setup.py` & `protai-0.6.1/setup.py`

 * *Files identical despite different names*

