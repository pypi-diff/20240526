# Comparing `tmp/os_toolkit-0.1.0.tar.gz` & `tmp/os_toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os_toolkit-0.1.0.tar", last modified: Mon Apr 29 03:12:12 2024, max compression
+gzip compressed data, was "os_toolkit-0.1.1.tar", last modified: Sun May 26 04:02:25 2024, max compression
```

## Comparing `os_toolkit-0.1.0.tar` & `os_toolkit-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 03:12:12.027511 os_toolkit-0.1.0/
--rw-rw-rw-   0        0        0      219 2024-04-29 03:12:12.026459 os_toolkit-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 03:12:12.013493 os_toolkit-0.1.0/os_tool/
--rw-rw-rw-   0        0        0       53 2024-04-18 01:36:51.000000 os_toolkit-0.1.0/os_tool/__init__.py
--rw-rw-rw-   0        0        0     7559 2024-04-27 05:13:42.000000 os_toolkit-0.1.0/os_tool/os_01.py
--rw-rw-rw-   0        0        0     2960 2024-04-12 04:46:37.000000 os_toolkit-0.1.0/os_tool/os_test.py
--rw-rw-rw-   0        0        0       12 2024-04-12 04:45:25.000000 os_toolkit-0.1.0/os_tool/test01.py
-drwxrwxrwx   0        0        0        0 2024-04-29 03:12:12.025462 os_toolkit-0.1.0/os_toolkit.egg-info/
--rw-rw-rw-   0        0        0      219 2024-04-29 03:12:11.000000 os_toolkit-0.1.0/os_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-29 03:12:11.000000 os_toolkit-0.1.0/os_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 03:12:11.000000 os_toolkit-0.1.0/os_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-29 03:12:11.000000 os_toolkit-0.1.0/os_toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 03:12:12.027511 os_toolkit-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      285 2024-04-29 03:11:48.000000 os_toolkit-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:02:25.676674 os_toolkit-0.1.1/
+-rw-rw-rw-   0        0        0      167 2024-05-26 04:02:25.673682 os_toolkit-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 04:02:25.643958 os_toolkit-0.1.1/os_toolkit/
+-rw-rw-rw-   0        0        0      106 2024-05-25 03:19:21.000000 os_toolkit-0.1.1/os_toolkit/__init__.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:07.000000 os_toolkit-0.1.1/os_toolkit/cant_use_ost.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:00.000000 os_toolkit-0.1.1/os_toolkit/fix_bug_ost.py
+-rw-rw-rw-   0        0        0     5595 2024-05-22 04:27:01.000000 os_toolkit-0.1.1/os_toolkit/sandbox1_ost.py
+-rw-rw-rw-   0        0        0     7559 2024-04-27 05:13:42.000000 os_toolkit-0.1.1/os_toolkit/utils_ost.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:02:25.672684 os_toolkit-0.1.1/os_toolkit.egg-info/
+-rw-rw-rw-   0        0        0      167 2024-05-26 04:02:25.000000 os_toolkit-0.1.1/os_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-26 04:02:25.000000 os_toolkit-0.1.1/os_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 04:02:25.000000 os_toolkit-0.1.1/os_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-26 04:02:25.000000 os_toolkit-0.1.1/os_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 04:02:25.000000 os_toolkit-0.1.1/os_toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 04:02:25.676674 os_toolkit-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      350 2024-05-26 04:01:53.000000 os_toolkit-0.1.1/setup.py
```

### Comparing `os_toolkit-0.1.0/os_tool/os_01.py` & `os_toolkit-0.1.1/os_toolkit/utils_ost.py`

 * *Files identical despite different names*

