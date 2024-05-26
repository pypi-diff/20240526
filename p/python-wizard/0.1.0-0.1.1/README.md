# Comparing `tmp/python_wizard-0.1.0.tar.gz` & `tmp/python_wizard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_wizard-0.1.0.tar", last modified: Mon Apr 29 06:24:34 2024, max compression
+gzip compressed data, was "python_wizard-0.1.1.tar", last modified: Sun May 26 03:52:36 2024, max compression
```

## Comparing `python_wizard-0.1.0.tar` & `python_wizard-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 06:24:34.357468 python_wizard-0.1.0/
--rw-rw-rw-   0        0        0      252 2024-04-29 06:24:34.357468 python_wizard-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 06:24:34.343505 python_wizard-0.1.0/python_wizard/
--rw-rw-rw-   0        0        0       62 2024-04-29 06:22:01.000000 python_wizard-0.1.0/python_wizard/__init__.py
--rw-rw-rw-   0        0        0     2907 2024-03-23 03:53:52.000000 python_wizard-0.1.0/python_wizard/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:24:34.355473 python_wizard-0.1.0/python_wizard.egg-info/
--rw-rw-rw-   0        0        0      252 2024-04-29 06:24:34.000000 python_wizard-0.1.0/python_wizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-04-29 06:24:34.000000 python_wizard-0.1.0/python_wizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:24:34.000000 python_wizard-0.1.0/python_wizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 06:24:34.000000 python_wizard-0.1.0/python_wizard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 06:24:34.357468 python_wizard-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      335 2024-04-29 06:18:48.000000 python_wizard-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:52:36.368550 python_wizard-0.1.1/
+-rw-rw-rw-   0        0        0      200 2024-05-26 03:52:36.367553 python_wizard-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 03:52:36.332136 python_wizard-0.1.1/python_wizard/
+-rw-rw-rw-   0        0        0      104 2024-05-25 03:02:40.000000 python_wizard-0.1.1/python_wizard/__init__.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:07.000000 python_wizard-0.1.1/python_wizard/cant_use_pw.py
+-rw-rw-rw-   0        0        0      262 2024-05-26 03:20:00.000000 python_wizard-0.1.1/python_wizard/fix_bug_pw.py
+-rw-rw-rw-   0        0        0      838 2024-05-12 03:29:43.000000 python_wizard-0.1.1/python_wizard/sandbox1_pw.py
+-rw-rw-rw-   0        0        0     3225 2024-05-22 03:40:47.000000 python_wizard-0.1.1/python_wizard/utils_pw.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:52:36.365559 python_wizard-0.1.1/python_wizard.egg-info/
+-rw-rw-rw-   0        0        0      200 2024-05-26 03:52:36.000000 python_wizard-0.1.1/python_wizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-26 03:52:36.000000 python_wizard-0.1.1/python_wizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 03:52:36.000000 python_wizard-0.1.1/python_wizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 03:52:36.000000 python_wizard-0.1.1/python_wizard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 03:52:36.368550 python_wizard-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      335 2024-05-22 03:45:36.000000 python_wizard-0.1.1/setup.py
```

### Comparing `python_wizard-0.1.0/python_wizard/utils.py` & `python_wizard-0.1.1/python_wizard/utils_pw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # v02 => import print_time
 
+def filter_dict(myDict,select_key):
+    # should be in my lib
+    ans = {key: value for key, value in myDict.items() if key in select_key}
+    return ans
+
+def reorder_dict(input_dict, new_order):
+    from collections import OrderedDict
+    return OrderedDict((key, input_dict[key]) for key in new_order)
+
+
+
 def is_convertible_to_num(s):
     if isinstance(s,(int,float)):
         return True
     try:
         int(s)
         return True
     except ValueError:
```

