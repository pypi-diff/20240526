# Comparing `tmp/pymail2-0.1.0.tar.gz` & `tmp/pymail2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymail2-0.1.0.tar", last modified: Sun May 26 05:24:37 2024, max compression
+gzip compressed data, was "pymail2-0.1.1.tar", last modified: Sun May 26 11:26:32 2024, max compression
```

## Comparing `pymail2-0.1.0.tar` & `pymail2-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:24:37.751550 pymail2-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-26 05:24:30.000000 pymail2-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-26 05:24:37.751550 pymail2-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 05:24:30.000000 pymail2-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:24:37.751550 pymail2-0.1.0/pymail2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-26 05:24:37.000000 pymail2-0.1.0/pymail2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-26 05:24:37.000000 pymail2-0.1.0/pymail2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 05:24:37.000000 pymail2-0.1.0/pymail2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 05:24:37.000000 pymail2-0.1.0/pymail2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 05:24:37.751550 pymail2-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-26 05:24:30.000000 pymail2-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:26:32.573321 pymail2-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-26 11:26:23.000000 pymail2-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-26 11:26:32.573321 pymail2-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-26 11:26:23.000000 pymail2-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:26:32.573321 pymail2-0.1.1/pymail2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-26 11:26:32.000000 pymail2-0.1.1/pymail2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-26 11:26:32.000000 pymail2-0.1.1/pymail2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:26:32.000000 pymail2-0.1.1/pymail2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:26:32.000000 pymail2-0.1.1/pymail2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-26 11:26:23.000000 pymail2-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-26 11:26:32.573321 pymail2-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-26 11:26:23.000000 pymail2-0.1.1/setup.py
```

### Comparing `pymail2-0.1.0/LICENSE` & `pymail2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymail2-0.1.0/PKG-INFO` & `pymail2-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymail2
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is most easiest way to send email using smtp
 Home-page: https://github.com/oakdatamechanic/pymail
 Author: Avinash Negi
 Author-email: avinash.negi2194@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pymail2-0.1.0/pymail2.egg-info/PKG-INFO` & `pymail2-0.1.1/pymail2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymail2
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is most easiest way to send email using smtp
 Home-page: https://github.com/oakdatamechanic/pymail
 Author: Avinash Negi
 Author-email: avinash.negi2194@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

