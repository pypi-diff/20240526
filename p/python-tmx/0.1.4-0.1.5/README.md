# Comparing `tmp/python-tmx-0.1.4.tar.gz` & `tmp/python_tmx-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-tmx-0.1.4.tar", last modified: Thu Feb  1 15:25:46 2024, max compression
+gzip compressed data, was "python_tmx-0.1.5.tar", last modified: Sun May 26 14:50:15 2024, max compression
```

## Comparing `python-tmx-0.1.4.tar` & `python_tmx-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-01 15:25:46.348178 python-tmx-0.1.4/
--rw-rw-rw-   0        0        0     1089 2024-02-01 15:02:43.000000 python-tmx-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2054 2024-02-01 15:25:46.348178 python-tmx-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1492 2024-02-01 15:02:43.000000 python-tmx-0.1.4/README.md
--rw-rw-rw-   0        0        0      636 2024-02-01 15:25:28.000000 python-tmx-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-01 15:25:46.348178 python-tmx-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-01 15:25:46.331028 python-tmx-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-02-01 15:25:46.348178 python-tmx-0.1.4/src/python_tmx.egg-info/
--rw-rw-rw-   0        0        0     2054 2024-02-01 15:25:46.000000 python-tmx-0.1.4/src/python_tmx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-02-01 15:25:46.000000 python-tmx-0.1.4/src/python_tmx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-01 15:25:46.000000 python-tmx-0.1.4/src/python_tmx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-02-01 15:25:46.000000 python-tmx-0.1.4/src/python_tmx.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-01 15:25:46.348178 python-tmx-0.1.4/src/tmx/
--rw-rw-rw-   0        0        0     7672 2024-02-01 15:02:43.000000 python-tmx-0.1.4/src/tmx/__init__.py
--rw-rw-rw-   0        0        0     4150 2024-02-01 15:02:43.000000 python-tmx-0.1.4/src/tmx/inline.py
--rw-rw-rw-   0        0        0    15200 2024-02-01 15:13:07.000000 python-tmx-0.1.4/src/tmx/structural.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:50:15.338709 python_tmx-0.1.5/
+-rw-rw-rw-   0        0        0     1089 2024-05-26 14:46:13.000000 python_tmx-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2455 2024-05-26 14:50:15.337706 python_tmx-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1492 2024-05-26 14:46:13.000000 python_tmx-0.1.5/README.md
+-rw-rw-rw-   0        0        0     1012 2024-05-26 14:46:40.000000 python_tmx-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:50:15.338709 python_tmx-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 14:50:15.293235 python_tmx-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:50:15.336192 python_tmx-0.1.5/src/python_tmx.egg-info/
+-rw-rw-rw-   0        0        0     2455 2024-05-26 14:50:15.000000 python_tmx-0.1.5/src/python_tmx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-26 14:50:15.000000 python_tmx-0.1.5/src/python_tmx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:50:15.000000 python_tmx-0.1.5/src/python_tmx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-26 14:50:15.000000 python_tmx-0.1.5/src/python_tmx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-26 14:50:15.000000 python_tmx-0.1.5/src/python_tmx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 14:50:15.335184 python_tmx-0.1.5/src/tmx/
+-rw-rw-rw-   0        0        0     7672 2024-05-26 14:46:13.000000 python_tmx-0.1.5/src/tmx/__init__.py
+-rw-rw-rw-   0        0        0     4150 2024-05-26 14:46:13.000000 python_tmx-0.1.5/src/tmx/inline.py
+-rw-rw-rw-   0        0        0    15209 2024-05-26 14:46:22.000000 python_tmx-0.1.5/src/tmx/structural.py
```

### Comparing `python-tmx-0.1.4/LICENSE` & `python_tmx-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-tmx-0.1.4/PKG-INFO` & `python_tmx-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 Metadata-Version: 2.1
 Name: python-tmx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library for manipulating, creating and editing tmx files
 Author-email: Enzo Agosta <agosta.enzowork@gmail.com>
+License: MIT
 Project-URL: Homepage, https://github.com/ChonkyYoshi/python-tmx
 Project-URL: Issues, https://github.com/ChonkyYoshi/python-tmx/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 
 # Python-tmx
 A python library based on lxml to help create, edit, and export tmx files quickly.
 
 # Installation
 Install the latest version of the library using Pypi, note that lxml is required.
 ```python
```

### Comparing `python-tmx-0.1.4/README.md` & `python_tmx-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `python-tmx-0.1.4/src/python_tmx.egg-info/PKG-INFO` & `python_tmx-0.1.5/src/python_tmx.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 Metadata-Version: 2.1
 Name: python-tmx
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library for manipulating, creating and editing tmx files
 Author-email: Enzo Agosta <agosta.enzowork@gmail.com>
+License: MIT
 Project-URL: Homepage, https://github.com/ChonkyYoshi/python-tmx
 Project-URL: Issues, https://github.com/ChonkyYoshi/python-tmx/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lxml
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
 
 # Python-tmx
 A python library based on lxml to help create, edit, and export tmx files quickly.
 
 # Installation
 Install the latest version of the library using Pypi, note that lxml is required.
 ```python
```

### Comparing `python-tmx-0.1.4/src/tmx/__init__.py` & `python_tmx-0.1.5/src/tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `python-tmx-0.1.4/src/tmx/inline.py` & `python_tmx-0.1.5/src/tmx/inline.py`

 * *Files identical despite different names*

### Comparing `python-tmx-0.1.4/src/tmx/structural.py` & `python_tmx-0.1.5/src/tmx/structural.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """structural tags definitions"""
+
 from dataclasses import dataclass, field
 from lxml.etree import Element, _Element, ElementTree, _ElementTree
 from typing import Literal
 from .inline import run
 from datetime import datetime
 from re import match
 from pathlib import Path
@@ -173,15 +174,15 @@
                     tmx_attrib["o-encoding"] = str(value)
                 elif attribute in ["creationdate", "changedate", "lastusagedate"]:
                     if isinstance(value, datetime):
                         if value.utcoffset() is not None:
                             value = value - value.utcoffset()
                         tmx_attrib[attribute] = value.strftime("%Y%m%dT%H%M%SZ")
                     else:
-                        if not match(r"\d{8}T\d{6}"):
+                        if not match(r"\d{8}T\d{6}", value):
                             raise ValueError(f"{attribute} format is not correct.")
                         tmx_attrib[attribute] = value
                 elif attribute == "otmf":
                     tmx_attrib["o-tmf"] = str(value)
                 else:
                     tmx_attrib[attribute] = value
         return tmx_attrib
```

