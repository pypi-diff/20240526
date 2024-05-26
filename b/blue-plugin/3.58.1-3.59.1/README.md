# Comparing `tmp/blue_plugin-3.58.1.tar.gz` & `tmp/blue_plugin-3.59.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_plugin-3.58.1.tar", last modified: Sun May 26 17:22:10 2024, max compression
+gzip compressed data, was "blue_plugin-3.59.1.tar", last modified: Sun May 26 20:34:37 2024, max compression
```

## Comparing `blue_plugin-3.58.1.tar` & `blue_plugin-3.59.1.tar`

### file list

```diff
@@ -1,23 +1,37 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:22:10.515352 blue_plugin-3.58.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-3.58.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:48:46.000000 blue_plugin-3.58.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     1599 2024-05-26 17:22:10.514985 blue_plugin-3.58.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      758 2024-05-21 03:10:18.000000 blue_plugin-3.58.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:22:10.511270 blue_plugin-3.58.1/blue_plugin/
--rw-r--r--   0 kamangir   (502) staff       (20)      155 2024-05-26 17:22:04.000000 blue_plugin-3.58.1/blue_plugin/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-21 00:08:25.000000 blue_plugin-3.58.1/blue_plugin/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-3.58.1/blue_plugin/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-3.58.1/blue_plugin/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-3.58.1/blue_plugin/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-3.58.1/blue_plugin/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-3.58.1/blue_plugin/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:22:10.514392 blue_plugin-3.58.1/blue_plugin.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     1599 2024-05-26 17:22:10.000000 blue_plugin-3.58.1/blue_plugin.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      401 2024-05-26 17:22:10.000000 blue_plugin-3.58.1/blue_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 17:22:10.000000 blue_plugin-3.58.1/blue_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-26 17:22:10.000000 blue_plugin-3.58.1/blue_plugin.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-26 17:22:10.000000 blue_plugin-3.58.1/blue_plugin.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 03:07:32.000000 blue_plugin-3.58.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-20 22:39:24.000000 blue_plugin-3.58.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 17:22:10.515424 blue_plugin-3.58.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      295 2024-05-26 17:21:12.000000 blue_plugin-3.58.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:34:37.669951 blue_plugin-3.59.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-09-09 01:44:55.000000 blue_plugin-3.59.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:48:46.000000 blue_plugin-3.59.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     1599 2024-05-26 20:34:37.669379 blue_plugin-3.59.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      758 2024-05-21 03:10:18.000000 blue_plugin-3.59.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:34:37.657677 blue_plugin-3.59.1/blue_plugin/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:34:37.664969 blue_plugin-3.59.1/blue_plugin/.abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      184 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/abcli.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      152 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       61 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/aka.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      816 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/blue_plugin.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      440 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/leaf.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:34:37.665655 blue_plugin-3.59.1/blue_plugin/.abcli/node/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1173 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/node/leaf.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      478 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/node.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      376 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/session.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:34:37.667714 blue_plugin-3.59.1/blue_plugin/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      205 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/tests/thing.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      306 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/tests/thing_with_args.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      148 2024-05-26 17:21:12.000000 blue_plugin-3.59.1/blue_plugin/.abcli/tests/version.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      155 2024-05-26 20:34:31.000000 blue_plugin-3.59.1/blue_plugin/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-21 00:08:25.000000 blue_plugin-3.59.1/blue_plugin/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       25 2024-04-19 01:49:55.000000 blue_plugin-3.59.1/blue_plugin/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      235 2024-04-27 21:22:01.000000 blue_plugin-3.59.1/blue_plugin/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-02-25 23:41:15.000000 blue_plugin-3.59.1/blue_plugin/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       92 2024-03-24 00:16:06.000000 blue_plugin-3.59.1/blue_plugin/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-08-20 02:33:38.000000 blue_plugin-3.59.1/blue_plugin/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 20:34:37.668455 blue_plugin-3.59.1/blue_plugin.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1599 2024-05-26 20:34:37.000000 blue_plugin-3.59.1/blue_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      749 2024-05-26 20:34:37.000000 blue_plugin-3.59.1/blue_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 20:34:37.000000 blue_plugin-3.59.1/blue_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-26 20:34:37.000000 blue_plugin-3.59.1/blue_plugin.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       12 2024-05-26 20:34:37.000000 blue_plugin-3.59.1/blue_plugin.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 03:07:32.000000 blue_plugin-3.59.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      131 2024-05-20 22:39:24.000000 blue_plugin-3.59.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 20:34:37.670080 blue_plugin-3.59.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      379 2024-05-26 20:32:55.000000 blue_plugin-3.59.1/setup.py
```

### Comparing `blue_plugin-3.58.1/LICENSE` & `blue_plugin-3.59.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blue_plugin-3.58.1/PKG-INFO` & `blue_plugin-3.59.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_plugin
-Version: 3.58.1
+Version: 3.59.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `blue_plugin-3.58.1/README.md` & `blue_plugin-3.59.1/README.md`

 * *Files identical despite different names*

### Comparing `blue_plugin-3.58.1/blue_plugin.egg-info/PKG-INFO` & `blue_plugin-3.59.1/blue_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_plugin
-Version: 3.58.1
+Version: 3.59.1
 Summary: 🌀 a git template for an awesome-bash-cli plugin.
 Home-page: https://github.com/kamangir/blue-plugin
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

