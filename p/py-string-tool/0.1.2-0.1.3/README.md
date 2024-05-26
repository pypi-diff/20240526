# Comparing `tmp/py_string_tool-0.1.2.tar.gz` & `tmp/py_string_tool-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_string_tool-0.1.2.tar", last modified: Mon Apr 29 05:06:51 2024, max compression
+gzip compressed data, was "py_string_tool-0.1.3.tar", last modified: Sun May 26 04:00:22 2024, max compression
```

## Comparing `py_string_tool-0.1.2.tar` & `py_string_tool-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 05:06:51.057710 py_string_tool-0.1.2/
--rw-rw-rw-   0        0        0      195 2024-04-29 05:06:51.057710 py_string_tool-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 05:06:51.044945 py_string_tool-0.1.2/py_string_tool/
--rw-rw-rw-   0        0        0       63 2024-04-29 05:06:20.000000 py_string_tool-0.1.2/py_string_tool/__init__.py
--rw-rw-rw-   0        0        0      480 2024-04-29 04:18:10.000000 py_string_tool-0.1.2/py_string_tool/blackslash_replace.py
--rw-rw-rw-   0        0        0     6401 2024-04-29 04:20:41.000000 py_string_tool-0.1.2/py_string_tool/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:06:51.055715 py_string_tool-0.1.2/py_string_tool.egg-info/
--rw-rw-rw-   0        0        0      195 2024-04-29 05:06:50.000000 py_string_tool-0.1.2/py_string_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-04-29 05:06:50.000000 py_string_tool-0.1.2/py_string_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 05:06:50.000000 py_string_tool-0.1.2/py_string_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-29 05:06:50.000000 py_string_tool-0.1.2/py_string_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-29 05:06:50.000000 py_string_tool-0.1.2/py_string_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 05:06:51.057710 py_string_tool-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      302 2024-04-29 05:06:24.000000 py_string_tool-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:00:22.379923 py_string_tool-0.1.3/
+-rw-rw-rw-   0        0        0      143 2024-05-26 04:00:22.378926 py_string_tool-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 04:00:22.358981 py_string_tool-0.1.3/py_string_tool/
+-rw-rw-rw-   0        0        0       67 2024-05-25 03:19:03.000000 py_string_tool-0.1.3/py_string_tool/__init__.py
+-rw-rw-rw-   0        0        0      480 2024-04-29 04:18:10.000000 py_string_tool-0.1.3/py_string_tool/blackslash_replace.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:07.000000 py_string_tool-0.1.3/py_string_tool/cant_use_pst.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:00.000000 py_string_tool-0.1.3/py_string_tool/fix_bug_pst.py
+-rw-rw-rw-   0        0        0    17963 2024-05-25 04:30:48.000000 py_string_tool-0.1.3/py_string_tool/utils_pst.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:00:22.377931 py_string_tool-0.1.3/py_string_tool.egg-info/
+-rw-rw-rw-   0        0        0      143 2024-05-26 04:00:22.000000 py_string_tool-0.1.3/py_string_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-05-26 04:00:22.000000 py_string_tool-0.1.3/py_string_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 04:00:22.000000 py_string_tool-0.1.3/py_string_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-26 04:00:22.000000 py_string_tool-0.1.3/py_string_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-26 04:00:22.000000 py_string_tool-0.1.3/py_string_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 04:00:22.379923 py_string_tool-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      334 2024-05-26 03:59:47.000000 py_string_tool-0.1.3/setup.py
```

