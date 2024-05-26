# Comparing `tmp/regolith-json-template-1.2.0.tar.gz` & `tmp/regolith_json_template-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regolith-json-template-1.2.0.tar", last modified: Sun Jul  9 19:14:15 2023, max compression
+gzip compressed data, was "regolith_json_template-1.3.0.tar", last modified: Sun May 26 08:56:27 2024, max compression
```

## Comparing `regolith-json-template-1.2.0.tar` & `regolith_json_template-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 19:14:15.822356 regolith-json-template-1.2.0/
--rw-rw-rw-   0        0        0     1083 2023-02-24 19:44:45.000000 regolith-json-template-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2150 2023-07-09 19:14:15.823349 regolith-json-template-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      556 2023-03-19 19:01:06.000000 regolith-json-template-1.2.0/README.rst
--rw-rw-rw-   0        0        0       90 2022-09-28 21:38:25.000000 regolith-json-template-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      764 2023-07-09 19:14:15.824351 regolith-json-template-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-09-28 23:50:58.000000 regolith-json-template-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:14:15.803604 regolith-json-template-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 19:14:15.814352 regolith-json-template-1.2.0/src/regolith_json_template/
--rw-rw-rw-   0        0        0     9295 2023-07-09 19:11:03.000000 regolith-json-template-1.2.0/src/regolith_json_template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 19:14:15.821354 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/
--rw-rw-rw-   0        0        0     2150 2023-07-09 19:14:15.000000 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-09 19:14:15.000000 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 19:14:15.000000 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-07-09 19:14:15.000000 regolith-json-template-1.2.0/src/regolith_json_template.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 08:56:27.772802 regolith_json_template-1.3.0/
+-rw-rw-rw-   0        0        0     1083 2023-02-24 19:44:46.000000 regolith_json_template-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2150 2024-05-26 08:56:27.772802 regolith_json_template-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-03-19 19:01:08.000000 regolith_json_template-1.3.0/README.rst
+-rw-rw-rw-   0        0        0       90 2022-09-28 21:38:26.000000 regolith_json_template-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      764 2024-05-26 08:56:27.774743 regolith_json_template-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-09-28 23:51:00.000000 regolith_json_template-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:56:27.758041 regolith_json_template-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 08:56:27.766359 regolith_json_template-1.3.0/src/regolith_json_template/
+-rw-rw-rw-   0        0        0     9839 2024-05-26 08:55:19.000000 regolith_json_template-1.3.0/src/regolith_json_template/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:56:27.771801 regolith_json_template-1.3.0/src/regolith_json_template.egg-info/
+-rw-rw-rw-   0        0        0     2150 2024-05-26 08:56:27.000000 regolith_json_template-1.3.0/src/regolith_json_template.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-05-26 08:56:27.000000 regolith_json_template-1.3.0/src/regolith_json_template.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 08:56:27.000000 regolith_json_template-1.3.0/src/regolith_json_template.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-26 08:56:27.000000 regolith_json_template-1.3.0/src/regolith_json_template.egg-info/top_level.txt
```

### Comparing `regolith-json-template-1.2.0/LICENSE` & `regolith_json_template-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regolith-json-template-1.2.0/PKG-INFO` & `regolith_json_template-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regolith-json-template
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python package for easier reuseability of the JSON Template Regolith filter for Minecraft Bedrock Edition
 Author: Nusiq
 License: MIT
 Project-URL: Source, https://github.com/Nusiq/regolith-json-template/tree/master
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `regolith-json-template-1.2.0/README.rst` & `regolith_json_template-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `regolith-json-template-1.2.0/setup.cfg` & `regolith_json_template-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `regolith-json-template-1.2.0/src/regolith_json_template/__init__.py` & `regolith_json_template-1.3.0/src/regolith_json_template/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from copy import deepcopy, copy
 import uuid
 import math
 import random
 from typing import Any, NamedTuple
 
-VERSION = (1, 2, 0)
+VERSION = (1, 3, 0)
 __version__ = '.'.join([str(x) for x in VERSION])
 
 EVAL_STRING_OPEN = '`'
 EVAL_STRING_CLOSE = '`'
 LIST_UNPACK_KEY = '__unpack__'
 LIST_UNPACK_OPTIONAL_VALUE = '__value__'
 
@@ -133,18 +133,28 @@
                         # one, because the next item always is based on the
                         # old_data_k_value so it can't be evaluated when it needs
                         # to be a source for other items.
                         if i == last_item_index:
                             data[evaluated_key] = old_data_k_value
                         else:  # copy the rest
                             data[evaluated_key] = deepcopy(old_data_k_value)
-                        data[evaluated_key] = eval_json(
+                        evaluated_value = eval_json(
                             data[evaluated_key], child_scope)
+                        # Ellipsis (...) is used as no value indicator.
+                        if evaluated_value != ...:
+                            data[evaluated_key] = evaluated_value
+                        elif evaluated_key in data:
+                            del data[evaluated_key]
                 else:
-                    data[k] = eval_json(data[k], scope)
+                    evaluated_value = eval_json(data[k], scope)
+                    # Ellipsis (...) is used as no value indicator.
+                    if evaluated_value != ...:
+                        data[k] = evaluated_value
+                    elif k in data:
+                        del data[k]
     elif isinstance(data, list):
         join_strings: JsonTemplateJoinStr | None = None
         new_data = []
         for i, item in enumerate(data):
             eval_item = eval_json(item, scope, True)
             if isinstance(eval_item, _Unpack):
                 if (
```

### Comparing `regolith-json-template-1.2.0/src/regolith_json_template.egg-info/PKG-INFO` & `regolith_json_template-1.3.0/src/regolith_json_template.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regolith-json-template
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python package for easier reuseability of the JSON Template Regolith filter for Minecraft Bedrock Edition
 Author: Nusiq
 License: MIT
 Project-URL: Source, https://github.com/Nusiq/regolith-json-template/tree/master
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

