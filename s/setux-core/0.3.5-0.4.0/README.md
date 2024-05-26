# Comparing `tmp/setux_core-0.3.5.tar.gz` & `tmp/setux_core-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/setux_core-0.3.5.tar", last modified: Mon Aug 24 12:00:24 2020, max compression
+gzip compressed data, was "dist/setux_core-0.4.0.tar", last modified: Sun Aug 30 18:37:14 2020, max compression
```

## Comparing `setux_core-0.3.5.tar` & `setux_core-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-24 12:00:24.000000 setux_core-0.3.5/
--rw-r--r--   0 louis     (4444) louis     (4444)     1011 2020-08-24 12:00:24.000000 setux_core-0.3.5/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      135 2020-08-09 08:10:25.000000 setux_core-0.3.5/README.rst
--rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-24 12:00:24.000000 setux_core-0.3.5/setup.cfg
--rw-r--r--   0 louis     (4444) louis     (4444)     1273 2020-08-24 11:59:38.000000 setux_core-0.3.5/setup.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-24 12:00:24.000000 setux_core-0.3.5/setux/
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-24 12:00:24.000000 setux_core-0.3.5/setux/core/
--rw-r--r--   0 louis     (4444) louis     (4444)       78 2020-08-24 11:59:38.000000 setux_core-0.3.5/setux/core/__init__.py
--rw-r--r--   0 louis     (4444) louis     (4444)     2513 2020-08-23 10:05:16.000000 setux_core-0.3.5/setux/core/distro.py
--rw-r--r--   0 louis     (4444) louis     (4444)      734 2020-08-10 08:44:12.000000 setux_core-0.3.5/setux/core/errors.py
--rw-r--r--   0 louis     (4444) louis     (4444)     2207 2020-08-09 08:10:25.000000 setux_core-0.3.5/setux/core/manage.py
--rw-r--r--   0 louis     (4444) louis     (4444)     1553 2020-08-24 11:59:38.000000 setux_core-0.3.5/setux/core/module.py
--rw-r--r--   0 louis     (4444) louis     (4444)     2226 2020-08-23 10:05:16.000000 setux_core-0.3.5/setux/core/package.py
--rw-r--r--   0 louis     (4444) louis     (4444)     2356 2020-08-24 11:59:38.000000 setux_core-0.3.5/setux/core/plugins.py
--rw-r--r--   0 louis     (4444) louis     (4444)     2138 2020-08-09 08:10:25.000000 setux_core-0.3.5/setux/core/service.py
--rw-r--r--   0 louis     (4444) louis     (4444)     7636 2020-08-24 08:34:42.000000 setux_core-0.3.5/setux/core/target.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-24 12:00:24.000000 setux_core-0.3.5/setux_core.egg-info/
--rw-rw-r--   0 louis     (4444) louis     (4444)     1011 2020-08-24 12:00:24.000000 setux_core-0.3.5/setux_core.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (4444) louis     (4444)      392 2020-08-24 12:00:24.000000 setux_core-0.3.5/setux_core.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)        1 2020-08-24 12:00:24.000000 setux_core-0.3.5/setux_core.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)       15 2020-08-24 12:00:24.000000 setux_core-0.3.5/setux_core.egg-info/requires.txt
--rw-rw-r--   0 louis     (4444) louis     (4444)        6 2020-08-24 12:00:24.000000 setux_core-0.3.5/setux_core.egg-info/top_level.txt
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 18:37:14.000000 setux_core-0.4.0/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1011 2020-08-30 18:37:14.000000 setux_core-0.4.0/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      135 2020-08-25 09:43:18.000000 setux_core-0.4.0/README.rst
+-rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-30 18:37:14.000000 setux_core-0.4.0/setup.cfg
+-rw-r--r--   0 louis     (4444) louis     (4444)     1273 2020-08-30 17:32:34.000000 setux_core-0.4.0/setup.py
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 18:37:14.000000 setux_core-0.4.0/setux/
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 18:37:14.000000 setux_core-0.4.0/setux/core/
+-rw-r--r--   0 louis     (4444) louis     (4444)       78 2020-08-30 17:32:54.000000 setux_core-0.4.0/setux/core/__init__.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     2513 2020-08-30 17:32:34.000000 setux_core-0.4.0/setux/core/distro.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      734 2020-08-25 09:43:18.000000 setux_core-0.4.0/setux/core/errors.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     2207 2020-08-25 09:43:18.000000 setux_core-0.4.0/setux/core/manage.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     2235 2020-08-30 17:32:54.000000 setux_core-0.4.0/setux/core/module.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     2226 2020-08-30 17:32:34.000000 setux_core-0.4.0/setux/core/package.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     2356 2020-08-30 17:32:34.000000 setux_core-0.4.0/setux/core/plugins.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     2138 2020-08-25 09:43:18.000000 setux_core-0.4.0/setux/core/service.py
+-rw-r--r--   0 louis     (4444) louis     (4444)     7636 2020-08-30 17:32:34.000000 setux_core-0.4.0/setux/core/target.py
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 18:37:14.000000 setux_core-0.4.0/setux_core.egg-info/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1011 2020-08-30 18:37:13.000000 setux_core-0.4.0/setux_core.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      392 2020-08-30 18:37:13.000000 setux_core-0.4.0/setux_core.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)        1 2020-08-30 18:37:13.000000 setux_core-0.4.0/setux_core.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)       15 2020-08-30 18:37:13.000000 setux_core-0.4.0/setux_core.egg-info/requires.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)        6 2020-08-30 18:37:13.000000 setux_core-0.4.0/setux_core.egg-info/top_level.txt
```

### Comparing `setux_core-0.3.5/PKG-INFO` & `setux_core-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: setux_core
-Version: 0.3.5
+Version: 0.4.0
 Summary: System deployment
 Home-page: https://github.com/louis-riviere-xyz/setux_core
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ########
          setux
```

### Comparing `setux_core-0.3.5/setup.py` & `setux_core-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `setux_core-0.3.5/setux/core/distro.py` & `setux_core-0.4.0/setux/core/distro.py`

 * *Files identical despite different names*

### Comparing `setux_core-0.3.5/setux/core/errors.py` & `setux_core-0.4.0/setux/core/errors.py`

 * *Files identical despite different names*

### Comparing `setux_core-0.3.5/setux/core/manage.py` & `setux_core-0.4.0/setux/core/manage.py`

 * *Files identical despite different names*

### Comparing `setux_core-0.3.5/setux/core/package.py` & `setux_core-0.4.0/setux/core/package.py`

 * *Files identical despite different names*

### Comparing `setux_core-0.3.5/setux/core/plugins.py` & `setux_core-0.4.0/setux/core/plugins.py`

 * *Files identical despite different names*

### Comparing `setux_core-0.3.5/setux/core/service.py` & `setux_core-0.4.0/setux/core/service.py`

 * *Files identical despite different names*

### Comparing `setux_core-0.3.5/setux/core/target.py` & `setux_core-0.4.0/setux/core/target.py`

 * *Files identical despite different names*

### Comparing `setux_core-0.3.5/setux_core.egg-info/PKG-INFO` & `setux_core-0.4.0/setux_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: setux-core
-Version: 0.3.5
+Version: 0.4.0
 Summary: System deployment
 Home-page: https://github.com/louis-riviere-xyz/setux_core
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ########
          setux
```

