# Comparing `tmp/setux-0.6.3.0.tar.gz` & `tmp/setux-0.6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/setux-0.6.3.0.tar", last modified: Mon Aug 31 09:28:40 2020, max compression
+gzip compressed data, was "dist/setux-0.6.3.1.tar", last modified: Mon Aug 31 13:37:36 2020, max compression
```

## Comparing `setux-0.6.3.0.tar` & `setux-0.6.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:28:40.000000 setux-0.6.3.0/
--rw-rw-r--   0 louis     (4444) louis     (4444)     1483 2020-08-31 09:28:40.000000 setux-0.6.3.0/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      415 2020-08-28 09:09:07.000000 setux-0.6.3.0/README.rst
--rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-31 09:28:40.000000 setux-0.6.3.0/setup.cfg
--rw-rw-r--   0 louis     (4444) louis     (4444)     1598 2020-08-31 09:27:50.000000 setux-0.6.3.0/setup.py
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:28:40.000000 setux-0.6.3.0/setux/
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:28:40.000000 setux-0.6.3.0/setux/main/
--rw-rw-r--   0 louis     (4444) louis     (4444)       83 2020-08-31 09:27:50.000000 setux-0.6.3.0/setux/main/__init__.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1302 2020-08-28 09:09:07.000000 setux-0.6.3.0/setux/main/main.py
--rw-r--r--   0 louis     (4444) louis     (4444)      379 2020-08-28 09:08:57.000000 setux-0.6.3.0/setux/main/usage.py
-drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 09:28:40.000000 setux-0.6.3.0/setux.egg-info/
--rw-rw-r--   0 louis     (4444) louis     (4444)     1483 2020-08-31 09:28:40.000000 setux-0.6.3.0/setux.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (4444) louis     (4444)      267 2020-08-31 09:28:40.000000 setux-0.6.3.0/setux.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)        1 2020-08-31 09:28:40.000000 setux-0.6.3.0/setux.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)       48 2020-08-31 09:28:40.000000 setux-0.6.3.0/setux.egg-info/entry_points.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)      141 2020-08-31 09:28:40.000000 setux-0.6.3.0/setux.egg-info/requires.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)        6 2020-08-31 09:28:40.000000 setux-0.6.3.0/setux.egg-info/top_level.txt
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:37:36.000000 setux-0.6.3.1/
+-rw-rw-r--   0 louis     (4444) louis     (4444)     1483 2020-08-31 13:37:36.000000 setux-0.6.3.1/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      415 2020-08-28 09:09:07.000000 setux-0.6.3.1/README.rst
+-rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-31 13:37:36.000000 setux-0.6.3.1/setup.cfg
+-rw-r--r--   0 louis     (4444) louis     (4444)     1598 2020-08-31 13:30:19.000000 setux-0.6.3.1/setup.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:37:36.000000 setux-0.6.3.1/setux/
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:37:36.000000 setux-0.6.3.1/setux/main/
+-rw-r--r--   0 louis     (4444) louis     (4444)       83 2020-08-31 13:30:19.000000 setux-0.6.3.1/setux/main/__init__.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     1302 2020-08-28 09:09:07.000000 setux-0.6.3.1/setux/main/main.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      379 2020-08-28 09:08:57.000000 setux-0.6.3.1/setux/main/usage.py
+drwxrwxr-x   0 louis     (4444) louis     (4444)        0 2020-08-31 13:37:36.000000 setux-0.6.3.1/setux.egg-info/
+-rw-rw-r--   0 louis     (4444) louis     (4444)     1483 2020-08-31 13:37:36.000000 setux-0.6.3.1/setux.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (4444) louis     (4444)      267 2020-08-31 13:37:36.000000 setux-0.6.3.1/setux.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)        1 2020-08-31 13:37:36.000000 setux-0.6.3.1/setux.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)       48 2020-08-31 13:37:36.000000 setux-0.6.3.1/setux.egg-info/entry_points.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)      141 2020-08-31 13:37:36.000000 setux-0.6.3.1/setux.egg-info/requires.txt
+-rw-rw-r--   0 louis     (4444) louis     (4444)        6 2020-08-31 13:37:36.000000 setux-0.6.3.1/setux.egg-info/top_level.txt
```

### Comparing `setux-0.6.3.0/PKG-INFO` & `setux-0.6.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: setux
-Version: 0.6.3.0
+Version: 0.6.3.1
 Summary: System deployment
 Home-page: https://framagit.org/louis-riviere-xyz/setux
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ########
          setux
```

### Comparing `setux-0.6.3.0/setup.py` & `setux-0.6.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'Topic :: Utilities',
     ],
     python_requires='>3.6',
     install_requires = [
         'setux_core>=0.4.0',
         'setux_distros>=0.4.1',
         'setux_targets>=0.4.0',
-        'setux_managers>=0.5.0',
+        'setux_managers>=0.5.1',
         'setux_modules>=0.3.4',
         'setux_logger>=0.2.0',
         'setux_repl>=0.4.2',
     ],
     packages = find_namespace_packages(
         include=['setux.*']
     ),
```

### Comparing `setux-0.6.3.0/setux/main/main.py` & `setux-0.6.3.1/setux/main/main.py`

 * *Files identical despite different names*

### Comparing `setux-0.6.3.0/setux.egg-info/PKG-INFO` & `setux-0.6.3.1/setux.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: setux
-Version: 0.6.3.0
+Version: 0.6.3.1
 Summary: System deployment
 Home-page: https://framagit.org/louis-riviere-xyz/setux
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ########
          setux
```

