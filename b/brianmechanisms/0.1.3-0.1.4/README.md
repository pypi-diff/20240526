# Comparing `tmp/brianmechanisms-0.1.3.tar.gz` & `tmp/brianmechanisms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brianmechanisms-0.1.3.tar", last modified: Sat May 25 20:59:31 2024, max compression
+gzip compressed data, was "brianmechanisms-0.1.4.tar", last modified: Sun May 26 09:41:19 2024, max compression
```

## Comparing `brianmechanisms-0.1.3.tar` & `brianmechanisms-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/src/brianmechanisms/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/appproximateStraightLineMechanisms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/locii.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/straightLineMechanisms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:41:19.343919 brianmechanisms-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/src/brianmechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/appproximateStraightLineMechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/locii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 09:41:09.000000 brianmechanisms-0.1.4/src/brianmechanisms/straightLineMechanisms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:41:19.347919 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 09:41:19.000000 brianmechanisms-0.1.4/src/brianmechanisms.egg-info/top_level.txt
```

### Comparing `brianmechanisms-0.1.3/LICENSE` & `brianmechanisms-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.3/src/brianmechanisms/appproximateStraightLineMechanisms.py` & `brianmechanisms-0.1.4/src/brianmechanisms/appproximateStraightLineMechanisms.py`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.3/src/brianmechanisms/locii.py` & `brianmechanisms-0.1.4/src/brianmechanisms/locii.py`

 * *Files identical despite different names*

