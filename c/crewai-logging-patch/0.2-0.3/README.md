# Comparing `tmp/crewai_logging_patch-0.2.tar.gz` & `tmp/crewai_logging_patch-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crewai_logging_patch-0.2.tar", last modified: Sun May 26 03:32:29 2024, max compression
+gzip compressed data, was "crewai_logging_patch-0.3.tar", last modified: Sun May 26 03:47:37 2024, max compression
```

## Comparing `crewai_logging_patch-0.2.tar` & `crewai_logging_patch-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:32:29.550813 crewai_logging_patch-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-26 03:32:19.000000 crewai_logging_patch-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-26 03:32:29.550813 crewai_logging_patch-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-26 03:32:19.000000 crewai_logging_patch-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:32:29.550813 crewai_logging_patch-0.2/crewai_logging_patch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-26 03:32:29.000000 crewai_logging_patch-0.2/crewai_logging_patch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-26 03:32:29.000000 crewai_logging_patch-0.2/crewai_logging_patch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 03:32:29.000000 crewai_logging_patch-0.2/crewai_logging_patch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 03:32:29.000000 crewai_logging_patch-0.2/crewai_logging_patch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:32:29.550813 crewai_logging_patch-0.2/logger_patch/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-26 03:32:19.000000 crewai_logging_patch-0.2/logger_patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-26 03:32:19.000000 crewai_logging_patch-0.2/logger_patch/logger_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 03:32:29.550813 crewai_logging_patch-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-26 03:32:19.000000 crewai_logging_patch-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:32:29.550813 crewai_logging_patch-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 03:32:19.000000 crewai_logging_patch-0.2/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:47:37.172533 crewai_logging_patch-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-26 03:47:33.000000 crewai_logging_patch-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-26 03:47:37.172533 crewai_logging_patch-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-26 03:47:33.000000 crewai_logging_patch-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:47:37.172533 crewai_logging_patch-0.3/crewai_logging_patch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-26 03:47:37.000000 crewai_logging_patch-0.3/crewai_logging_patch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-26 03:47:37.000000 crewai_logging_patch-0.3/crewai_logging_patch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 03:47:37.000000 crewai_logging_patch-0.3/crewai_logging_patch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 03:47:37.000000 crewai_logging_patch-0.3/crewai_logging_patch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:47:37.172533 crewai_logging_patch-0.3/logger_patch/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-26 03:47:33.000000 crewai_logging_patch-0.3/logger_patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-26 03:47:33.000000 crewai_logging_patch-0.3/logger_patch/logger_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 03:47:37.172533 crewai_logging_patch-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-26 03:47:33.000000 crewai_logging_patch-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 03:47:37.172533 crewai_logging_patch-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 03:47:33.000000 crewai_logging_patch-0.3/tests/tests.py
```

### Comparing `crewai_logging_patch-0.2/LICENSE` & `crewai_logging_patch-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crewai_logging_patch-0.2/PKG-INFO` & `crewai_logging_patch-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crewai_logging_patch
-Version: 0.2
+Version: 0.3
 Home-page: https://github.com/theCyberTech/CrewAI_Logger_Patch
 Author: theCyberTech
 Author-email: the_t3ch@pm.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crewai_logging_patch-0.2/README.md` & `crewai_logging_patch-0.3/README.md`

 * *Files identical despite different names*

### Comparing `crewai_logging_patch-0.2/crewai_logging_patch.egg-info/PKG-INFO` & `crewai_logging_patch-0.3/crewai_logging_patch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crewai_logging_patch
-Version: 0.2
+Version: 0.3
 Home-page: https://github.com/theCyberTech/CrewAI_Logger_Patch
 Author: theCyberTech
 Author-email: the_t3ch@pm.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crewai_logging_patch-0.2/logger_patch/logger_patch.py` & `crewai_logging_patch-0.3/logger_patch/logger_patch.py`

 * *Files identical despite different names*

