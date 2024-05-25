# Comparing `tmp/eva-shell-0.2.8.tar.gz` & `tmp/eva-shell-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva-shell-0.2.8.tar", last modified: Wed Jan 24 23:02:18 2024, max compression
+gzip compressed data, was "eva-shell-0.2.9.tar", last modified: Fri Jan 26 00:22:31 2024, max compression
```

## Comparing `eva-shell-0.2.8.tar` & `eva-shell-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-01-24 23:02:18.739751 eva-shell-0.2.8/
--rw-r--r--   0 divisor   (1000) root         (0)    10644 2023-11-19 23:00:18.000000 eva-shell-0.2.8/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      458 2024-01-24 23:02:18.735751 eva-shell-0.2.8/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       19 2022-03-19 02:57:04.000000 eva-shell-0.2.8/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-01-24 23:02:18.735751 eva-shell-0.2.8/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       73 2022-03-19 02:57:04.000000 eva-shell-0.2.8/bin/eva
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-01-24 23:02:18.735751 eva-shell-0.2.8/eva4_shell/
--rw-r--r--   0 divisor   (1000) root         (0)       74 2024-01-24 23:02:03.000000 eva-shell-0.2.8/eva4_shell/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    54325 2024-01-24 23:02:03.000000 eva-shell-0.2.8/eva4_shell/ap.py
--rw-r--r--   0 divisor   (1000) root         (0)     7078 2024-01-24 23:02:03.000000 eva-shell-0.2.8/eva4_shell/charts.py
--rw-r--r--   0 divisor   (1000) root         (0)    60095 2024-01-24 23:02:03.000000 eva-shell-0.2.8/eva4_shell/cli.py
--rw-r--r--   0 divisor   (1000) root         (0)     2686 2024-01-24 23:02:03.000000 eva-shell-0.2.8/eva4_shell/client.py
--rw-r--r--   0 divisor   (1000) root         (0)     5107 2024-01-24 23:02:03.000000 eva-shell-0.2.8/eva4_shell/compl.py
--rw-r--r--   0 divisor   (1000) root         (0)      653 2024-01-24 23:02:03.000000 eva-shell-0.2.8/eva4_shell/sharedobj.py
--rw-r--r--   0 divisor   (1000) root         (0)     1696 2024-01-24 23:02:03.000000 eva-shell-0.2.8/eva4_shell/shell.py
--rw-r--r--   0 divisor   (1000) root         (0)    15867 2024-01-24 23:02:03.000000 eva-shell-0.2.8/eva4_shell/tools.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-01-24 23:02:18.735751 eva-shell-0.2.8/eva_shell.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      458 2024-01-24 23:02:18.000000 eva-shell-0.2.8/eva_shell.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      382 2024-01-24 23:02:18.000000 eva-shell-0.2.8/eva_shell.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2024-01-24 23:02:18.000000 eva-shell-0.2.8/eva_shell.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)      166 2024-01-24 23:02:18.000000 eva-shell-0.2.8/eva_shell.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       11 2024-01-24 23:02:18.000000 eva-shell-0.2.8/eva_shell.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2024-01-24 23:02:18.739751 eva-shell-0.2.8/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)     1187 2024-01-24 23:02:03.000000 eva-shell-0.2.8/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-01-26 00:22:31.470346 eva-shell-0.2.9/
+-rw-r--r--   0 divisor   (1000) root         (0)    10644 2023-11-19 23:00:18.000000 eva-shell-0.2.9/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      458 2024-01-26 00:22:31.466346 eva-shell-0.2.9/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       19 2022-03-19 02:57:04.000000 eva-shell-0.2.9/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-01-26 00:22:31.466346 eva-shell-0.2.9/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       73 2022-03-19 02:57:04.000000 eva-shell-0.2.9/bin/eva
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-01-26 00:22:31.466346 eva-shell-0.2.9/eva4_shell/
+-rw-r--r--   0 divisor   (1000) root         (0)       74 2024-01-26 00:21:55.000000 eva-shell-0.2.9/eva4_shell/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    54325 2024-01-26 00:21:55.000000 eva-shell-0.2.9/eva4_shell/ap.py
+-rw-r--r--   0 divisor   (1000) root         (0)     7078 2024-01-26 00:21:55.000000 eva-shell-0.2.9/eva4_shell/charts.py
+-rw-r--r--   0 divisor   (1000) root         (0)    60095 2024-01-26 00:21:55.000000 eva-shell-0.2.9/eva4_shell/cli.py
+-rw-r--r--   0 divisor   (1000) root         (0)     2686 2024-01-26 00:21:55.000000 eva-shell-0.2.9/eva4_shell/client.py
+-rw-r--r--   0 divisor   (1000) root         (0)     5107 2024-01-26 00:21:55.000000 eva-shell-0.2.9/eva4_shell/compl.py
+-rw-r--r--   0 divisor   (1000) root         (0)      653 2024-01-26 00:21:55.000000 eva-shell-0.2.9/eva4_shell/sharedobj.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1696 2024-01-26 00:21:55.000000 eva-shell-0.2.9/eva4_shell/shell.py
+-rw-r--r--   0 divisor   (1000) root         (0)    16173 2024-01-26 00:21:55.000000 eva-shell-0.2.9/eva4_shell/tools.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-01-26 00:22:31.466346 eva-shell-0.2.9/eva_shell.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      458 2024-01-26 00:22:31.000000 eva-shell-0.2.9/eva_shell.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      382 2024-01-26 00:22:31.000000 eva-shell-0.2.9/eva_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2024-01-26 00:22:31.000000 eva-shell-0.2.9/eva_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)      166 2024-01-26 00:22:31.000000 eva-shell-0.2.9/eva_shell.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       11 2024-01-26 00:22:31.000000 eva-shell-0.2.9/eva_shell.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2024-01-26 00:22:31.470346 eva-shell-0.2.9/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)     1187 2024-01-26 00:21:55.000000 eva-shell-0.2.9/setup.py
```

### Comparing `eva-shell-0.2.8/LICENSE` & `eva-shell-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eva-shell-0.2.8/eva4_shell/ap.py` & `eva-shell-0.2.9/eva4_shell/ap.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.2.8/eva4_shell/charts.py` & `eva-shell-0.2.9/eva4_shell/charts.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.2.8/eva4_shell/cli.py` & `eva-shell-0.2.9/eva4_shell/cli.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.2.8/eva4_shell/client.py` & `eva-shell-0.2.9/eva4_shell/client.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.2.8/eva4_shell/compl.py` & `eva-shell-0.2.9/eva4_shell/compl.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.2.8/eva4_shell/sharedobj.py` & `eva-shell-0.2.9/eva4_shell/sharedobj.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.2.8/eva4_shell/shell.py` & `eva-shell-0.2.9/eva4_shell/shell.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.2.8/eva4_shell/tools.py` & `eva-shell-0.2.9/eva4_shell/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,19 +236,29 @@
         print(out)
     if err is not None:
         print('--- ERR ---')
         print(colored(err, color='red'))
     print()
 
 
+def convert_bytes(data):
+    if isinstance(data, bytes):
+        return list(data)
+    if isinstance(data, list):
+        return [convert_bytes(item) for item in data]
+    if isinstance(data, dict):
+        return {key: convert_bytes(value) for key, value in data.items()}
+    return data
+
+
 def print_result(data, need_header=True, name_value=False, cols=None):
     if current_command.json:
         from pygments import highlight, lexers, formatters
         import json
-        j = json.dumps(data, indent=4, sort_keys=True)
+        j = json.dumps(convert_bytes(data), indent=4, sort_keys=True)
         if can_colorize():
             j = highlight(j, lexers.JsonLexer(), formatters.TerminalFormatter())
         print(j)
         return
     elif data:
         if name_value:
             if name_value is True:
```

### Comparing `eva-shell-0.2.8/setup.py` & `eva-shell-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='eva-shell',
```

