# Comparing `tmp/lanmonitor-3.2.1.tar.gz` & `tmp/lanmonitor-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanmonitor-3.2.1.tar", last modified: Tue Jan 16 17:47:22 2024, max compression
+gzip compressed data, was "lanmonitor-3.2.2.tar", last modified: Sun May 26 17:48:37 2024, max compression
```

## Comparing `lanmonitor-3.2.1.tar` & `lanmonitor-3.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-01-16 17:47:22.190234 lanmonitor-3.2.1/
--rwxrw-r--   0 cjn       (1000) cjn       (1000)     1088 2023-02-14 04:57:32.000000 lanmonitor-3.2.1/LICENSE.txt
--rw-rw-r--   0 cjn       (1000) cjn       (1000)       40 2023-02-27 03:02:26.000000 lanmonitor-3.2.1/MANIFEST.in
--rw-r--r--   0 cjn       (1000) cjn       (1000)    34787 2024-01-16 17:47:22.190234 lanmonitor-3.2.1/PKG-INFO
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)    33421 2024-01-16 17:43:46.000000 lanmonitor-3.2.1/README.md
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)      927 2024-01-16 17:42:38.000000 lanmonitor-3.2.1/pyproject.toml
--rw-rw-r--   0 cjn       (1000) cjn       (1000)       38 2024-01-16 17:47:22.190234 lanmonitor-3.2.1/setup.cfg
-drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-01-16 17:47:22.186234 lanmonitor-3.2.1/src/
-drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-01-16 17:47:22.188234 lanmonitor-3.2.1/src/lanmonitor/
--rwxrw-r--   0 cjn       (1000) cjn       (1000)        0 2023-02-14 04:57:32.000000 lanmonitor-3.2.1/src/lanmonitor/__init__.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     5716 2024-01-05 23:31:20.000000 lanmonitor-3.2.1/src/lanmonitor/apt_upgrade_history_plugin.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     5393 2024-01-05 23:31:30.000000 lanmonitor-3.2.1/src/lanmonitor/dd_wrt_age_plugin.py
-drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-01-16 17:47:22.189234 lanmonitor-3.2.1/src/lanmonitor/deployment_files/
--rw-------   0 cjn       (1000) cjn       (1000)      189 2023-02-17 23:52:03.000000 lanmonitor-3.2.1/src/lanmonitor/deployment_files/creds_SMTP
--rwxrw-r--   0 cjn       (1000) cjn       (1000)     4954 2024-01-05 05:21:33.000000 lanmonitor-3.2.1/src/lanmonitor/deployment_files/lanmonitor.cfg
--rwxrw-r--   0 cjn       (1000) cjn       (1000)      179 2022-12-04 15:48:21.000000 lanmonitor-3.2.1/src/lanmonitor/deployment_files/lanmonitor.service
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     6173 2024-01-05 23:31:40.000000 lanmonitor-3.2.1/src/lanmonitor/freespace_plugin.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     7875 2024-01-05 23:31:55.000000 lanmonitor-3.2.1/src/lanmonitor/fsactivity_plugin.py
--rwxrw-r--   0 cjn       (1000) cjn       (1000)      293 2024-01-05 23:32:05.000000 lanmonitor-3.2.1/src/lanmonitor/globvars.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     4283 2024-01-05 21:25:56.000000 lanmonitor-3.2.1/src/lanmonitor/interface_plugin.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)    12709 2024-01-05 23:32:27.000000 lanmonitor-3.2.1/src/lanmonitor/lanmonfuncs.py
--rwxrw-r--   0 cjn       (1000) cjn       (1000)    17987 2024-01-05 23:31:10.000000 lanmonitor-3.2.1/src/lanmonitor/lanmonitor.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     5280 2024-01-05 23:32:42.000000 lanmonitor-3.2.1/src/lanmonitor/pinghost_plugin.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     3778 2024-01-05 23:32:51.000000 lanmonitor-3.2.1/src/lanmonitor/process_plugin.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     4052 2024-01-05 23:33:00.000000 lanmonitor-3.2.1/src/lanmonitor/selinux_plugin.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     4993 2024-01-05 23:33:08.000000 lanmonitor-3.2.1/src/lanmonitor/service_plugin.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     9986 2024-01-05 23:33:17.000000 lanmonitor-3.2.1/src/lanmonitor/stock_notif.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     4296 2024-01-05 23:33:25.000000 lanmonitor-3.2.1/src/lanmonitor/webpage_plugin.py
--rwxrwxr-x   0 cjn       (1000) cjn       (1000)     6098 2024-01-16 17:41:52.000000 lanmonitor-3.2.1/src/lanmonitor/yum_update_history_plugin.py
-drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-01-16 17:47:22.190234 lanmonitor-3.2.1/src/lanmonitor.egg-info/
--rw-r--r--   0 cjn       (1000) cjn       (1000)    34787 2024-01-16 17:47:22.000000 lanmonitor-3.2.1/src/lanmonitor.egg-info/PKG-INFO
--rw-rw-r--   0 cjn       (1000) cjn       (1000)      959 2024-01-16 17:47:22.000000 lanmonitor-3.2.1/src/lanmonitor.egg-info/SOURCES.txt
--rw-rw-r--   0 cjn       (1000) cjn       (1000)        1 2024-01-16 17:47:22.000000 lanmonitor-3.2.1/src/lanmonitor.egg-info/dependency_links.txt
--rw-rw-r--   0 cjn       (1000) cjn       (1000)       57 2024-01-16 17:47:22.000000 lanmonitor-3.2.1/src/lanmonitor.egg-info/entry_points.txt
--rw-rw-r--   0 cjn       (1000) cjn       (1000)       60 2024-01-16 17:47:22.000000 lanmonitor-3.2.1/src/lanmonitor.egg-info/requires.txt
--rw-rw-r--   0 cjn       (1000) cjn       (1000)       11 2024-01-16 17:47:22.000000 lanmonitor-3.2.1/src/lanmonitor.egg-info/top_level.txt
+drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-05-26 17:48:37.799935 lanmonitor-3.2.2/
+-rwxrw-r--   0 cjn       (1000) cjn       (1000)     1088 2023-02-14 04:57:32.000000 lanmonitor-3.2.2/LICENSE.txt
+-rw-rw-r--   0 cjn       (1000) cjn       (1000)       40 2023-02-27 03:02:26.000000 lanmonitor-3.2.2/MANIFEST.in
+-rw-r--r--   0 cjn       (1000) cjn       (1000)    34789 2024-05-26 17:48:37.799935 lanmonitor-3.2.2/PKG-INFO
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)    33423 2024-05-26 17:31:20.000000 lanmonitor-3.2.2/README.md
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)      927 2024-05-26 17:31:32.000000 lanmonitor-3.2.2/pyproject.toml
+-rw-rw-r--   0 cjn       (1000) cjn       (1000)       38 2024-05-26 17:48:37.799935 lanmonitor-3.2.2/setup.cfg
+drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-05-26 17:48:37.694935 lanmonitor-3.2.2/src/
+drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-05-26 17:48:37.797935 lanmonitor-3.2.2/src/lanmonitor/
+-rwxrw-r--   0 cjn       (1000) cjn       (1000)        0 2023-02-14 04:57:32.000000 lanmonitor-3.2.2/src/lanmonitor/__init__.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     5716 2024-01-05 23:31:20.000000 lanmonitor-3.2.2/src/lanmonitor/apt_upgrade_history_plugin.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     5393 2024-01-05 23:31:30.000000 lanmonitor-3.2.2/src/lanmonitor/dd_wrt_age_plugin.py
+drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-05-26 17:48:37.799935 lanmonitor-3.2.2/src/lanmonitor/deployment_files/
+-rw-------   0 cjn       (1000) cjn       (1000)      189 2023-02-17 23:52:03.000000 lanmonitor-3.2.2/src/lanmonitor/deployment_files/creds_SMTP
+-rwxrw-r--   0 cjn       (1000) cjn       (1000)     4954 2024-01-05 05:21:33.000000 lanmonitor-3.2.2/src/lanmonitor/deployment_files/lanmonitor.cfg
+-rwxrw-r--   0 cjn       (1000) cjn       (1000)      179 2022-12-04 15:48:21.000000 lanmonitor-3.2.2/src/lanmonitor/deployment_files/lanmonitor.service
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     6173 2024-01-05 23:31:40.000000 lanmonitor-3.2.2/src/lanmonitor/freespace_plugin.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     7875 2024-01-05 23:31:55.000000 lanmonitor-3.2.2/src/lanmonitor/fsactivity_plugin.py
+-rwxrw-r--   0 cjn       (1000) cjn       (1000)      293 2024-01-05 23:32:05.000000 lanmonitor-3.2.2/src/lanmonitor/globvars.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     4283 2024-01-05 21:25:56.000000 lanmonitor-3.2.2/src/lanmonitor/interface_plugin.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)    12709 2024-01-05 23:32:27.000000 lanmonitor-3.2.2/src/lanmonitor/lanmonfuncs.py
+-rwxrw-r--   0 cjn       (1000) cjn       (1000)    17987 2024-01-05 23:31:10.000000 lanmonitor-3.2.2/src/lanmonitor/lanmonitor.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     5280 2024-01-05 23:32:42.000000 lanmonitor-3.2.2/src/lanmonitor/pinghost_plugin.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     3778 2024-01-05 23:32:51.000000 lanmonitor-3.2.2/src/lanmonitor/process_plugin.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     4052 2024-01-05 23:33:00.000000 lanmonitor-3.2.2/src/lanmonitor/selinux_plugin.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     4993 2024-01-05 23:33:08.000000 lanmonitor-3.2.2/src/lanmonitor/service_plugin.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     9986 2024-01-05 23:33:17.000000 lanmonitor-3.2.2/src/lanmonitor/stock_notif.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     4296 2024-01-05 23:33:25.000000 lanmonitor-3.2.2/src/lanmonitor/webpage_plugin.py
+-rwxrwxr-x   0 cjn       (1000) cjn       (1000)     6099 2024-05-26 17:25:47.000000 lanmonitor-3.2.2/src/lanmonitor/yum_update_history_plugin.py
+drwxrwxr-x   0 cjn       (1000) cjn       (1000)        0 2024-05-26 17:48:37.799935 lanmonitor-3.2.2/src/lanmonitor.egg-info/
+-rw-r--r--   0 cjn       (1000) cjn       (1000)    34789 2024-05-26 17:48:37.000000 lanmonitor-3.2.2/src/lanmonitor.egg-info/PKG-INFO
+-rw-rw-r--   0 cjn       (1000) cjn       (1000)      959 2024-05-26 17:48:37.000000 lanmonitor-3.2.2/src/lanmonitor.egg-info/SOURCES.txt
+-rw-rw-r--   0 cjn       (1000) cjn       (1000)        1 2024-05-26 17:48:37.000000 lanmonitor-3.2.2/src/lanmonitor.egg-info/dependency_links.txt
+-rw-rw-r--   0 cjn       (1000) cjn       (1000)       57 2024-05-26 17:48:37.000000 lanmonitor-3.2.2/src/lanmonitor.egg-info/entry_points.txt
+-rw-rw-r--   0 cjn       (1000) cjn       (1000)       60 2024-05-26 17:48:37.000000 lanmonitor-3.2.2/src/lanmonitor.egg-info/requires.txt
+-rw-rw-r--   0 cjn       (1000) cjn       (1000)       11 2024-05-26 17:48:37.000000 lanmonitor-3.2.2/src/lanmonitor.egg-info/top_level.txt
```

### Comparing `lanmonitor-3.2.1/LICENSE.txt` & `lanmonitor-3.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/PKG-INFO` & `lanmonitor-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanmonitor
-Version: 3.2.1
+Version: 3.2.2
 Summary: Monitor the state of services, processes, web pages, file system, etc. on your server and LAN
 Author-email: Chris Nelson <github@cjnaz.com>
 License: MIT License
         
         Copyright (c) 2023 Chris Nelson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -429,15 +429,15 @@
 - none
 
 <br/>
 
 ---
 
 ## Version history
-- 3.2.1 240116 - yum_update_history_plugin command match bug fix.
+- 3.2.2 240526 - yum_update_history_plugin command match bug fixes.
 - 3.2 240105 - Adjusted for cjnfuncs V2.1. fsactivity plugin supports missing file. yum_update_history_plugin now requires full command match.
 - 3.1 230320 - Plugins now distinguish between ssh access issues and real failures when checking on remote hosts.  
 Added cfg param ssh_timeout, fixed cmd_check command fail retry bug, added pinghost_plugin_timeout.
   cmd_check returns RTN_PASS, RTN_FAIL, RTN_WARNING (for remote ssh access issues)
 - 3.0.2 230226 - Converted to package format, updated to cjnfuncs 2.0.
 - V2.0  221130 - Changed to check_interval per item.  Added `freespace` and `apt_upgrade_history` plugins.  Removed --once switch, replaced with --service switch.  Removed config RecheckInterval, replaced with ServiceLoopTime.  - Added `--print-log` switch.  Tuned up debug logging for plugin development.  Fixed summaries disable bug.
 - V1.5  221120 - Added apt_upgrade_history plugin, Added `--print-log` switch, Fixed summaries disable bug.
```

### Comparing `lanmonitor-3.2.1/README.md` & `lanmonitor-3.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
 - none
 
 <br/>
 
 ---
 
 ## Version history
-- 3.2.1 240116 - yum_update_history_plugin command match bug fix.
+- 3.2.2 240526 - yum_update_history_plugin command match bug fixes.
 - 3.2 240105 - Adjusted for cjnfuncs V2.1. fsactivity plugin supports missing file. yum_update_history_plugin now requires full command match.
 - 3.1 230320 - Plugins now distinguish between ssh access issues and real failures when checking on remote hosts.  
 Added cfg param ssh_timeout, fixed cmd_check command fail retry bug, added pinghost_plugin_timeout.
   cmd_check returns RTN_PASS, RTN_FAIL, RTN_WARNING (for remote ssh access issues)
 - 3.0.2 230226 - Converted to package format, updated to cjnfuncs 2.0.
 - V2.0  221130 - Changed to check_interval per item.  Added `freespace` and `apt_upgrade_history` plugins.  Removed --once switch, replaced with --service switch.  Removed config RecheckInterval, replaced with ServiceLoopTime.  - Added `--print-log` switch.  Tuned up debug logging for plugin development.  Fixed summaries disable bug.
 - V1.5  221120 - Added apt_upgrade_history plugin, Added `--print-log` switch, Fixed summaries disable bug.
```

### Comparing `lanmonitor-3.2.1/pyproject.toml` & `lanmonitor-3.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"] #, "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lanmonitor"
-version = "3.2.1"
+version = "3.2.2"
 description = "Monitor the state of services, processes, web pages, file system, etc. on your server and LAN"
 readme = "README.md"
 requires-python = ">=3.6"       # Centos 7 uses 3.6.8
 authors = [ {name = "Chris Nelson", email = "github@cjnaz.com"} ]
 license = {file = "LICENSE.txt"}
 dependencies = [
     'cjnfuncs >= 2.1',
```

### Comparing `lanmonitor-3.2.1/src/lanmonitor/apt_upgrade_history_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/apt_upgrade_history_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/dd_wrt_age_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/dd_wrt_age_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/deployment_files/lanmonitor.cfg` & `lanmonitor-3.2.2/src/lanmonitor/deployment_files/lanmonitor.cfg`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/freespace_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/freespace_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/fsactivity_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/fsactivity_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/interface_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/interface_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/lanmonfuncs.py` & `lanmonitor-3.2.2/src/lanmonitor/lanmonfuncs.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/lanmonitor.py` & `lanmonitor-3.2.2/src/lanmonitor/lanmonitor.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/pinghost_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/pinghost_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/process_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/process_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/selinux_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/selinux_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/service_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/service_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/stock_notif.py` & `lanmonitor-3.2.2/src/lanmonitor/stock_notif.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/webpage_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/webpage_plugin.py`

 * *Files identical despite different names*

### Comparing `lanmonitor-3.2.1/src/lanmonitor/yum_update_history_plugin.py` & `lanmonitor-3.2.2/src/lanmonitor/yum_update_history_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from lanmonitor.lanmonfuncs import RTN_PASS, RTN_WARNING, RTN_FAIL, RTN_CRITICAL, cmd_check
 from cjnfuncs.core import logging
 from cjnfuncs.timevalue import timevalue, retime
 
 
 
 # Configs / Constants
-YUMLINEFORMAT=re.compile(r"[ \d]+ \| ([\w -]+) \| ([\d :-]+) ")
+YUMLINEFORMAT=re.compile(r"[ \d]+ \| ([\w -=]+) \| ([\d :-]+) ")
 #    154 | update --skip-broken     | 2021-03-18 22:31 | Update         |    5 ss
 
 
 class monitor:
 
     def __init__ (self):
         pass
```

### Comparing `lanmonitor-3.2.1/src/lanmonitor.egg-info/PKG-INFO` & `lanmonitor-3.2.2/src/lanmonitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanmonitor
-Version: 3.2.1
+Version: 3.2.2
 Summary: Monitor the state of services, processes, web pages, file system, etc. on your server and LAN
 Author-email: Chris Nelson <github@cjnaz.com>
 License: MIT License
         
         Copyright (c) 2023 Chris Nelson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -429,15 +429,15 @@
 - none
 
 <br/>
 
 ---
 
 ## Version history
-- 3.2.1 240116 - yum_update_history_plugin command match bug fix.
+- 3.2.2 240526 - yum_update_history_plugin command match bug fixes.
 - 3.2 240105 - Adjusted for cjnfuncs V2.1. fsactivity plugin supports missing file. yum_update_history_plugin now requires full command match.
 - 3.1 230320 - Plugins now distinguish between ssh access issues and real failures when checking on remote hosts.  
 Added cfg param ssh_timeout, fixed cmd_check command fail retry bug, added pinghost_plugin_timeout.
   cmd_check returns RTN_PASS, RTN_FAIL, RTN_WARNING (for remote ssh access issues)
 - 3.0.2 230226 - Converted to package format, updated to cjnfuncs 2.0.
 - V2.0  221130 - Changed to check_interval per item.  Added `freespace` and `apt_upgrade_history` plugins.  Removed --once switch, replaced with --service switch.  Removed config RecheckInterval, replaced with ServiceLoopTime.  - Added `--print-log` switch.  Tuned up debug logging for plugin development.  Fixed summaries disable bug.
 - V1.5  221120 - Added apt_upgrade_history plugin, Added `--print-log` switch, Fixed summaries disable bug.
```

### Comparing `lanmonitor-3.2.1/src/lanmonitor.egg-info/SOURCES.txt` & `lanmonitor-3.2.2/src/lanmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

