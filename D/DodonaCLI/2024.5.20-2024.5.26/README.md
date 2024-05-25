# Comparing `tmp/dodonacli-2024.5.20.tar.gz` & `tmp/dodonacli-2024.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodonacli-2024.5.20.tar", last modified: Mon May 20 14:27:35 2024, max compression
+gzip compressed data, was "dodonacli-2024.5.26.tar", last modified: Sat May 25 22:38:04 2024, max compression
```

## Comparing `dodonacli-2024.5.20.tar` & `dodonacli-2024.5.26.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.644019 dodonacli-2024.5.20/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.644019 dodonacli-2024.5.20/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/.github/workflows/publish_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/DodonaCLI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 14:27:35.000000 dodonacli-2024.5.20/DodonaCLI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.644019 dodonacli-2024.5.20/dodonacli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/dodonacli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/cli_next.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/commands/up.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/dodonacli/source/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/get_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/interactive_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/pretty_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/set_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/submission_data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli/source/syntax_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1637 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/dodonacli_completion_script.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/man-page/
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/man-page/dodonacli.1
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/man-page/dodonacli.1.gz
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-20 14:27:29.000000 dodonacli-2024.5.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:27:35.648019 dodonacli-2024.5.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:04.497926 dodonacli-2024.5.26/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:04.489926 dodonacli-2024.5.26/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:04.489926 dodonacli-2024.5.26/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/.github/workflows/publish_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:04.497926 dodonacli-2024.5.26/DodonaCLI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-25 22:38:04.000000 dodonacli-2024.5.26/DodonaCLI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-25 22:38:04.000000 dodonacli-2024.5.26/DodonaCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 22:38:04.000000 dodonacli-2024.5.26/DodonaCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-25 22:38:04.000000 dodonacli-2024.5.26/DodonaCLI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 22:38:04.000000 dodonacli-2024.5.26/DodonaCLI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 22:38:04.000000 dodonacli-2024.5.26/DodonaCLI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-25 22:38:04.497926 dodonacli-2024.5.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:04.493926 dodonacli-2024.5.26/dodonacli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:04.493926 dodonacli-2024.5.26/dodonacli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/cli_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12690 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/commands/up.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      945 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:04.493926 dodonacli-2024.5.26/dodonacli/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13042 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/source/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/source/interactive_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/source/pretty_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13904 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/source/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/source/pretty_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/source/set_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/source/submission_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli/source/syntax_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1637 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/dodonacli_completion_script.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 22:38:04.493926 dodonacli-2024.5.26/man-page/
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/man-page/dodonacli.1
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/man-page/dodonacli.1.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-25 22:38:00.000000 dodonacli-2024.5.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 22:38:04.497926 dodonacli-2024.5.26/setup.cfg
```

### Comparing `dodonacli-2024.5.20/.github/workflows/publish.yml` & `dodonacli-2024.5.26/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/.github/workflows/publish_test.yml` & `dodonacli-2024.5.26/.github/workflows/publish_test.yml`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/DodonaCLI.egg-info/PKG-INFO` & `dodonacli-2024.5.26/DodonaCLI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.5.20
+Version: 2024.5.26
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dodonacli-2024.5.20/DodonaCLI.egg-info/SOURCES.txt` & `dodonacli-2024.5.26/DodonaCLI.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,12 +26,13 @@
 dodonacli/commands/tutorial.py
 dodonacli/commands/up.py
 dodonacli/source/__init__.py
 dodonacli/source/get_data.py
 dodonacli/source/interactive_tutorial.py
 dodonacli/source/pretty_console.py
 dodonacli/source/pretty_print.py
+dodonacli/source/pretty_printer.py
 dodonacli/source/set_data.py
 dodonacli/source/submission_data_handler.py
 dodonacli/source/syntax_checker.py
 man-page/dodonacli.1
 man-page/dodonacli.1.gz
```

### Comparing `dodonacli-2024.5.20/LICENSE` & `dodonacli-2024.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/PKG-INFO` & `dodonacli-2024.5.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DodonaCLI
-Version: 2024.5.20
+Version: 2024.5.26
 Summary: A CLI tool for Dodona
 Author-email: Bram Windey <windey.bram@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Bram Windey
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dodonacli-2024.5.20/README.md` & `dodonacli-2024.5.26/README.md`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli/commands/cli_next.py` & `dodonacli-2024.5.26/dodonacli/commands/cli_next.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,28 +165,28 @@
     prefixes = make_visual_representation(previous_id, previous_id_index, next_id, id_list)
     pretty_print.print_series_data(series_data_json, settings, prefixes=prefixes)
 
     return config
 
 
 def get_next_course(config, settings, connection, headers, reverse, unsolved):
-    from dodonacli.source import get_data, pretty_print
+    from dodonacli.source import get_data, pretty_print, pretty_printer
 
     # Get all registred courses
     course_data_json = get_data.courses_data(connection, headers)
 
     id_list = [course['id'] for course in course_data_json]
     previous_id = config['course_id']
     previous_id_index = id_list.index(int(previous_id))
 
     # Find the next course (loop back to front if it was the last)
     # If courses get more data that indicates if it's completely solved,
     # then this will get the same logic found in get_next_exercise()
     if unsolved:
-        pretty_print.custom_print(
+        pretty_printer.custom_print(
             "Unsolved flag not supported yet for series and courses.",
             {'new_lines_above': settings['new_lines_above']}
         )
 
     next_id = id_list[(previous_id_index + 1 - (2 * reverse)) % len(id_list)]
 
     # Store new course
```

### Comparing `dodonacli-2024.5.20/dodonacli/commands/display.py` & `dodonacli-2024.5.26/dodonacli/commands/display.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli/commands/info.py` & `dodonacli-2024.5.26/dodonacli/commands/info.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,155 +6,150 @@
 def info():
     pass
 
 
 @click.command(help='Display the current version of DodonaCLI. The versioning system '
                     'uses a YYYY.M.D format.')
 def version():
-    from dodonacli.source import pretty_console
+    from dodonacli.source import get_data, pretty_printer
 
-    pretty_console.console.print("DodonaCLI " + get_dodonacli_version())
+    pretty_printer.custom_print("DodonaCLI " + get_dodonacli_version(), get_data.get_settings(), pretty=True)
 
 
 @click.command(help='Checks if there is a new update available for DodonaCLI.')
 def check_update():
     from packaging.version import parse
     from pkg_info import get_pkg_info
-    from dodonacli.source import get_data, pretty_console
+    from dodonacli.source import get_data, pretty_printer
 
     settings = get_data.get_settings()
     dodonacli_version = get_dodonacli_version()
 
     pkg = get_pkg_info('DodonaCLI')
 
     if parse(pkg.version) > parse(dodonacli_version):
-        pretty_console.console.print(
-            '\n' * settings['new_lines_above']
-            + f"There is a new version available: {pkg.version}\n"
-              f"You can update your old version ({dodonacli_version}) with\n"
-              "  'pip install --upgrade DodonaCLI'"
-            + '\n' * settings['new_lines_below']
-        )
+        text = f"There is a new version available: {pkg.version}\n" \
+               f"You can update your old version ({dodonacli_version}) with\n" \
+               f"  'pip install --upgrade DodonaCLI'"
     else:
-        print(
-            '\n' * settings['new_lines_above']
-            + "Your DodonaCLI is up-to-date."
-            + '\n' * settings['new_lines_below']
-        )
+        text = "Your DodonaCLI is up-to-date."
+
+    pretty_printer.custom_print(text, settings, pretty=True)
 
 
 @click.command(help='Tab completion, very handy for fast use')
 def completion():
-    from dodonacli.source import get_data, pretty_console
+    from dodonacli.source import get_data, pretty_printer
 
     settings = get_data.get_settings()
 
-    pretty_console.console.print(
-        '\n' * settings['new_lines_above']
-        + "There are 2 ways of doing tab-completion: \n"
-          "   - using Click's default tab-completion for bash/zsh/fish\n"
-          "   - using DodonaCLI's custom script for bash only\n"
-          "\nThe reason there is a custom script, is because the default completion lacks "
-          "a bit here and there.\n"
-          "The default option is easier to use, and doesn't need a redownload after an update.\n\n"
-          "To install the default completion:\n"
-          "   Follow this short tutorial:\n"
-          "       https://click.palletsprojects.com/en/8.1.x/shell-completion/#enabling-completion\n"
-          "   Replace every occurence of 'foo-bar' with 'dodona'\n"
-          "   Do notice that you can choose how you name the file, and where you put it.\n\n"
-          "To install the custom script for bash:\n"
-          "   Go to DodonaCLI's GitHub: https://www.github.com/BWindey/DodonaCLI\n"
-          "   And download 'dodonacli_completion_script.sh' (at top-level of project structure)\n"
-          "   Now add 'source <PATH TO SCRIPT>' to your '.bashrc',\n"
-          "   where you fill in the path to the downloaded script."
-          "\n\n"
-          "For both ways you'll have to either [u yellow]restart your terminal[/], "
-          "or re-'source' your .bashrc/.fishrc/...\n"
-          "Happy tabbing!"
-        + '\n' * settings['new_lines_below']
+    pretty_printer.custom_print(
+        "There are 2 ways of doing tab-completion: \n"
+        "   - using Click's default tab-completion for bash/zsh/fish\n"
+        "   - using DodonaCLI's custom script for bash only\n"
+        "\nThe reason there is a custom script, is because the default completion lacks "
+        "a bit here and there.\n"
+        "The default option is easier to use, and doesn't need a redownload after an update.\n\n"
+        "To install the default completion:\n"
+        "   Follow this short tutorial:\n"
+        "       https://click.palletsprojects.com/en/8.1.x/shell-completion/#enabling-completion\n"
+        "   Replace every occurence of 'foo-bar' with 'dodona'\n"
+        "   Do notice that you can choose how you name the file, and where you put it.\n\n"
+        "To install the custom script for bash:\n"
+        "   Go to DodonaCLI's GitHub: https://www.github.com/BWindey/DodonaCLI\n"
+        "   And download 'dodonacli_completion_script.sh' (at top-level of project structure)\n"
+        "   Now add 'source <PATH TO SCRIPT>' to your '.bashrc',\n"
+        "   where you fill in the path to the downloaded script."
+        "\n\n"
+        "For both ways you'll have to either [u yellow]restart your terminal[/], "
+        "or re-'source' your .bashrc/.fishrc/...\n"
+        "Happy tabbing!",
+        settings, pretty=True
     )
 
 
 @click.command(help="Link to the GitHub page of DodonaCLI. "
                     "Can be handy for the README page, manpages, Issues (bug reports) and pull requests.")
 def github():
-    from dodonacli.source import get_data, pretty_console
+    from dodonacli.source import get_data, pretty_printer
 
     settings = get_data.get_settings()
 
-    pretty_console.console.print(
-        '\n' * settings['new_lines_above']
-        + "https://www.github.com/BWindey/DodonaCLI"
-        + '\n' * settings['new_lines_below']
+    pretty_printer.custom_print(
+        "https://www.github.com/BWindey/DodonaCLI",
+        settings, pretty=True
     )
 
 
 @click.command(help='Changelog for the latest version.')
 def changelog():
     from rich.markdown import Markdown
     from dodonacli.source import get_data, pretty_console
 
     settings = get_data.get_settings()
 
     changelog_raw = (
-            '\n' * settings['new_lines_above']
-            + "\t- Added man-page sub-command to completion-script, oopsie,"
-              "forgot that previously\n"
-              "\t- Added a settings.json file at the same location as config.json. "
-              "This settings file may be edited directly by the user, the config one NOT.\n"
-              "\t- All the implemented settings, followed by their default setting:\n"
-              "\t\t- 'amount_feedback_context': 3\n"
-              "\t\t- 'amount_feedback_tab': -1\n"
-              "\t\t- 'amount_feedback_testcase': 3\n"
-              "\t\t- 'amount_feedback_test': 3\n"
-              "\t\t- 'amount_sub_exercise': 10\n"
-              "\t\t- 'amount_sub_global': -1\n"
-              "\t\t- 'new_lines_above': 1\n"
-              "\t\t- 'new_lines_below': 1\n"
-              "\t\t- 'paste_force_warning': True\n"
-              "\t\t- 'display_series_after_select': False\n"
-              "\t\t- 'display_exercises_after_select': False\n"
-              "\t\t- 'display_exercise_after_select': False\n\n"
-              "\t\t* For feedback-settings, the order is tab->context->testcase->test. The number "
-              "tells you how many of them will be shown in your terminal.\n"
-              "\t\t* The new-lines ones describe how many empty lines should be printed around "
-              "each complete message DodonaCLI prints to your terminal. This has always be 1-1, "
-              "but is now customisable.\n"
-              "\t\t* The display ... after select does exactly what you think it does!\n"
-              "\t\t* An integer set to -1 means that there is no upper bound but that "
-              "of the amount of data the Dodona API gives.\n\n"
-              "\t- Drastically improved the 'display --force' when only a course is selected\n"
-              "\n"
-              "\tAs always, you can use the '--help' flag after every command and sub-command to learn more.\n"
-              "\tHappy coding!"
-            + '\n' * settings['new_lines_below']
+        "\t- Added some forgotten settings-driven prints, I think every print now takes the "
+        "new-lines into account.\n"
+        "\t- Moved some imports around, speeding up some subcommands that don't connect to Dodona.\n"
+        "\nThis was a small quick update, so here is the changelog for the previous update:\n\n"
+        "\t- Added man-page sub-command to completion-script, oopsie,"
+        "forgot that previously\n"
+        "\t- Added a settings.json file at the same location as config.json. "
+        "This settings file may be edited directly by the user, the config one NOT.\n"
+        "\t- All the implemented settings, followed by their default setting:\n"
+        "\t\t- 'amount_feedback_context': 3\n"
+        "\t\t- 'amount_feedback_tab': -1\n"
+        "\t\t- 'amount_feedback_testcase': 3\n"
+        "\t\t- 'amount_feedback_test': 3\n"
+        "\t\t- 'amount_sub_exercise': 10\n"
+        "\t\t- 'amount_sub_global': -1\n"
+        "\t\t- 'new_lines_above': 1\n"
+        "\t\t- 'new_lines_below': 1\n"
+        "\t\t- 'paste_force_warning': True\n"
+        "\t\t- 'display_series_after_select': False\n"
+        "\t\t- 'display_exercises_after_select': False\n"
+        "\t\t- 'display_exercise_after_select': False\n\n"
+        "\t\t* For feedback-settings, the order is tab->context->testcase->test. The number "
+        "tells you how many of them will be shown in your terminal.\n"
+        "\t\t* The new-lines ones describe how many empty lines should be printed around "
+        "each complete message DodonaCLI prints to your terminal. This has always be 1-1, "
+        "but is now customisable.\n"
+        "\t\t* The display ... after select does exactly what you think it does!\n"
+        "\t\t* An integer set to -1 means that there is no upper bound but that "
+        "of the amount of data the Dodona API gives.\n\n"
+        "\t- Drastically improved the 'display --force' when only a course is selected\n"
+        "\n"
+        "\tAs always, you can use the '--help' flag after every command and sub-command to learn more.\n"
+        "\tHappy coding!"
     )
     md = Markdown(changelog_raw)
+    print('\n' * settings['new_lines_above'], end='')
     pretty_console.console.print(md)
+    print('\n' * settings['new_lines_below'], end='')
 
 
 @click.command(help='Man-pages for DodonaCLI, very professional')
 def man_page():
-    from dodonacli.source import get_data, pretty_console
+    from dodonacli.source import get_data, pretty_printer
 
     settings = get_data.get_settings()
 
-    pretty_console.console.print(
-        "\n" * settings['new_lines_above'] +
+    pretty_printer.custom_print(
         "To install a man-page for DodonaCLI, you can download it from GitHub:\n"
         "  https://www.github.com/BWindey/DodonaCLI\n"
         "The man-page files are located under the 'man-page' directory.\n"
         "Download the .gz version (gzip-compressed), "
         "the other one is not useful unless you want to see how man-pages are written.\n\n"
         "Now run the command 'manpath' in your terminal, this should print a list of "
         "paths, seperated by a ':'\n"
         "Now move the downloaded file to one of those paths.\n"
         "I personally put it onder '~/.local/share/man/man1/'\n"
-        "[u yellow]Note[/] that te manual-entry is for 'dodonacli', not 'dodona'"
-        "\n" * settings['new_lines_below']
+        "[yellow]Note:[/] the manual-entry is for 'dodonacli', not 'dodona'",
+        settings, pretty=True
     )
 
 
 def get_dodonacli_version():
     from importlib import metadata
     return metadata.version(__package__.split('.')[0])
```

### Comparing `dodonacli-2024.5.20/dodonacli/commands/post.py` & `dodonacli-2024.5.26/dodonacli/commands/post.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli/commands/select.py` & `dodonacli-2024.5.26/dodonacli/commands/select.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                    "\n\nUsage: dodona select --hidden <TOKEN> <SERIES_ID>")
 @click.option("--other", "-other",
               help="Select a course that you're not registered for. Only works with "
                    "an id, not a name.",
               is_flag=True, default=False)
 @click.argument('thing')
 def select(thing, hidden, other):
-    from dodonacli.source import set_data, get_data, pretty_print
+    from dodonacli.source import set_data, get_data, pretty_print, pretty_printer
 
     # Read configs in
     config = get_data.get_configs()
     settings = get_data.get_settings()
 
     # Start up the connection to Dodona
     connection = http.client.HTTPSConnection("dodona.be")
@@ -80,15 +80,15 @@
             json_data = get_data.exercise_data(connection, headers, config['course_id'], config['exercise_id'])
             pretty_print.print_exercise(json_data, config['TOKEN'], {'new_lines_below': settings['new_lines_below']})
         else:
             config = select_exercise(connection, headers, thing, config, settings)
 
     else:
         # You can't select more when everything is already selected
-        pretty_print.custom_print(
+        pretty_printer.custom_print(
             "There is already an exercise selected.\n"
             "Please remove selection with 'dodona up' before selecting a new exercise.",
             settings
         )
         return
 
     # Save selections in config file
```

### Comparing `dodonacli-2024.5.20/dodonacli/commands/settings.py` & `dodonacli-2024.5.26/dodonacli/commands/settings.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli/commands/submission.py` & `dodonacli-2024.5.26/dodonacli/commands/submission.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli/commands/up.py` & `dodonacli-2024.5.26/dodonacli/commands/up.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli/main.py` & `dodonacli-2024.5.26/dodonacli/main.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli/source/get_data.py` & `dodonacli-2024.5.26/dodonacli/source/get_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,19 @@
     try:
         connection.request(connection_type, link, headers=headers)
 
     except socket.gaierror:
         print("Something went wrong trying to connect to Dodona. This is probably an internet connection problem.")
         exit(2)
 
+    except Exception as e:
+        print("Something went wrong trying to connect to Dodona, can you report this error on Github please?")
+        print(e)
+        connection.close()
+
     return connection
 
 
 def handle_connection_response(connection: http.client.HTTPSConnection) -> bytes:
     """
     Handle response from Dodona connection
     Terminates program if there was a problem with the connection
```

### Comparing `dodonacli-2024.5.20/dodonacli/source/interactive_tutorial.py` & `dodonacli-2024.5.26/dodonacli/source/interactive_tutorial.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli/source/pretty_print.py` & `dodonacli-2024.5.26/dodonacli/source/pretty_print.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,8 @@
-import http.client
-import json
-import markdownify
-import re
-
-from bs4 import BeautifulSoup
-from rich.markdown import Markdown
-from rich.padding import Padding
-
-from . import get_data, pretty_console, submission_data_handler
-
-
-def custom_print(text: str, settings: dict, pretty: bool = False):
-    """
-    Prints out the text with the amount of newlines specified in settings
-    :param text: text to print
-    :param settings: dict with settings
-    :param pretty: whether to use the pretty_console print, or the standard Python print
-    """
-    if pretty:
-        printer = pretty_console.console.print
-    else:
-        printer = print
-
-    printer(
-        '\n' * settings.get('new_lines_above', 0)
-        + text
-        + '\n' * settings.get('new_lines_below', 0)
-    )
+from .pretty_printer import custom_print
 
 
 def print_courses_data(json_data: dict, settings: dict, title: str = "Your courses:", prefixes: dict = None):
     """
     Print out the courses in json_data in a neat way
     :param json_data: json object with data about Dodona courses
     :param settings: dict with settings
@@ -86,14 +58,20 @@
     # Find the maximum length of all but the last element in all tuples to align them in the terminal
     max_series_id_length = max(len(e[0]) for e in display_data)
     max_series_name_length = max(len(e[1]) for e in display_data)
 
     # Print out all the series in display_data while also handling the Markdown inside the series-description
     result = "[u bright_blue]All series:[/]\n"
     if force:
+        import markdownify
+        import re
+        from rich.markdown import Markdown
+        from rich.padding import Padding
+        from dodonacli.source import pretty_console
+
         pretty_console.console.print('\n' * settings['new_lines_above'] + result, end='')
 
         for i, series in enumerate(display_data):
             description = series[2].strip('\n')
             description = re.sub(r'{: *target="_blank"}', '', description).strip()
             md_description = Markdown(markdownify.markdownify(description))
 
@@ -201,14 +179,21 @@
         custom_print(
             f"You can find the exercise description at \n{json_data['description_url']}",
             settings,
             pretty=True
         )
 
     else:
+        import http.client
+        import markdownify
+        from bs4 import BeautifulSoup
+        from rich.markdown import Markdown
+        from rich.padding import Padding
+        from dodonacli.source import get_data, pretty_console
+
         custom_print(
             "Expected programming language: " + json_data['programming_language']['name'] + '\n',
             {'new_lines_above': settings['new_lines_above']},
             pretty=True
         )
 
         # Make sandbox.dodona connection for exercise description:
@@ -246,47 +231,53 @@
 def print_result(json_results: dict, url: str, settings: dict):
     """
     Print out the results of a submission in a neat way
     :param json_results: json object with data about a submission
     :param url: link to the submission
     :param settings: dict with settings
     """
+    from dodonacli.source import submission_data_handler
+
     if json_results['accepted']:
         # Everything passed, well done!
         result = "[bold bright_green]All tests passed![/] You can continue to next exercise.\n"
     else:
         result = submission_data_handler.submission_data_handler(json_results, settings).strip() + '\n'
 
     result += url
     custom_print(result, settings, pretty=True)
 
 
-def print_status(config: dict):
+def print_status(config: dict, settings: dict):
     """
     Print out the current selection of course, exercise-series and exercise.
     :param config: Dictionary with the configs
+    :param settings: Dictionary with the settings
     """
     course_string = config['course_name']
     if config['course_id'] is not None:
         course_string += f" ({config['course_id']})"
 
-    pretty_console.console.print(
-        f"\n[u bright_blue]Status:[/]\n"
+    custom_print(
+        f"[u bright_blue]Status:[/]\n"
         f"\t{'Course: '.ljust(10)}{course_string}\n"
         f"\t{'Series: '.ljust(10)}{config['serie_name']}\n"
-        f"\t{'Exercise: '.ljust(10)}{config['exercise_name']}\n"
+        f"\t{'Exercise: '.ljust(10)}{config['exercise_name']}",
+        settings, pretty=True
     )
 
 
 def print_exercise_submissions(json_data: dict, settings: dict):
     """
     Print out a list of the (up to) 10 most recent submissions as found in json_data
     :param json_data: Dictionary with submission data
     :param settings: Dictionary with settings
     """
+    from dodonacli.source import pretty_console
+
     pretty_console.console.print(
         "\n[u bright_blue]Most recent submissions:[/]"
     )
 
     amount_shown = min(settings['amount_sub_exercise'], len(json_data))
     if amount_shown == -1:
         amount_shown = len(json_data)
@@ -305,26 +296,31 @@
             f"\t{accepted_emoji}  [link={submission['url'].rstrip('.json')}]#{len(json_data) - i: <2}[/link]"
             f"\t{status}\t"
         )
     # Newline for clarity
     print()
 
 
-def print_all_submissions(connection: http.client.HTTPSConnection, headers: dict, json_data: dict, settings: dict):
+def print_all_submissions(connection, headers: dict, json_data: dict, settings: dict):
     """
     Print out a list of the latest 30 submissions for the user, userwide (not tied to an exercise).
     Makes extra requests to Dodona to get the name of the exercises of the submissions
     :param connection: Connection to Dodona
     :param headers: Headers to send with the connection
     :param json_data: Dictionary with submission info
     :param settings: Dictionary with settings
     :return:
     """
+    from dodonacli.source import pretty_console
+    import json
+
+    print('\n' * settings['new_lines_above'], end='')
+
     pretty_console.console.print(
-        "\n[u bright_blue]Most recent submissions:[/]"
+        "[u bright_blue]Most recent submissions:[/]"
     )
 
     amount_shown = min(settings['amount_sub_global'], len(json_data))
     if amount_shown == -1:
         amount_shown = len(json_data)
 
     for i, submission in enumerate(json_data[:amount_shown]):
@@ -351,9 +347,8 @@
         pretty_console.console.print(
             f"\t{accepted_emoji}  [link={submission['url'].rstrip('.json')}]#{len(json_data) - i: <2}[/link]"
             f"\t{status: <25}"
             f"\t{exercise_name}"
         )
 
     connection.close()
-    # Newline for clarity
-    print()
+    print('\n' * settings['new_lines_below'], end='')
```

### Comparing `dodonacli-2024.5.20/dodonacli/source/set_data.py` & `dodonacli-2024.5.26/dodonacli/source/set_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import random
 import rich.status
 import time
 
 from datetime import datetime
 
-from . import pretty_print, pretty_console, get_data
+from . import pretty_print, get_data, pretty_printer
 
 
 def dump_config(config: dict):
     """
     Save the config to it's file again.
     :param config: Dictionary containing the configs
     """
@@ -62,23 +62,23 @@
     json_payload = json.dumps(payload)
 
     # Connect to Dodona and post the solution
     connection.request("POST", "/submissions.json", json_payload, headers=headers)
     res = connection.getresponse()
     status = res.status
     if status == 422:
-        pretty_print.custom_print(
+        pretty_printer.custom_print(
             "[i]Patience, young padawan.\n"
             "A cooldown, Dodona servers have, to prevent DDOS attacks, hmm, yes.[/]",
             settings, pretty=True
         )
         return
 
     elif status != 200:
-        pretty_print.custom_print(
+        pretty_printer.custom_print(
             "Error connection to Dodona: " + str(res.status) + '\n'
             + "Reason: " + res.reason,
             settings, pretty=True
         )
         return
 
     # Read out the result
@@ -170,12 +170,12 @@
     """
     name = name.replace(' ', '-')
     file_name = f"{name}_{submission_id}{extension}"
 
     with open(file_name, "w") as code_file:
         code_file.write(content)
 
-    pretty_print.custom_print(
+    pretty_printer.custom_print(
         f"Code from your submission for {name} is now saved in:\n"
         f"\t{name}_{submission_id}{extension}",
         settings, pretty=True
     )
```

### Comparing `dodonacli-2024.5.20/dodonacli/source/submission_data_handler.py` & `dodonacli-2024.5.26/dodonacli/source/submission_data_handler.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli/source/syntax_checker.py` & `dodonacli-2024.5.26/dodonacli/source/syntax_checker.py`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/dodonacli_completion_script.sh` & `dodonacli-2024.5.26/dodonacli_completion_script.sh`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/man-page/dodonacli.1` & `dodonacli-2024.5.26/man-page/dodonacli.1`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/man-page/dodonacli.1.gz` & `dodonacli-2024.5.26/man-page/dodonacli.1.gz`

 * *Files identical despite different names*

### Comparing `dodonacli-2024.5.20/pyproject.toml` & `dodonacli-2024.5.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DodonaCLI"
-version = '2024.5.20'
+version = '2024.5.26'
 authors = [
     { name = "Bram Windey", email = "windey.bram@gmail.com" },
 ]
 description = "A CLI tool for Dodona"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
```

