# Comparing `tmp/zenaura-0.9.50.tar.gz` & `tmp/zenaura-0.9.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.50.tar", last modified: Sun May 26 14:19:22 2024, max compression
+gzip compressed data, was "zenaura-0.9.51.tar", last modified: Sun May 26 15:24:47 2024, max compression
```

## Comparing `zenaura-0.9.50.tar` & `zenaura-0.9.51.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:19:22.559901 zenaura-0.9.50/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.50/LICENSE
--rw-rw-rw-   0        0        0     1781 2024-05-26 14:19:22.559401 zenaura-0.9.50/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-18 13:42:46.000000 zenaura-0.9.50/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 14:19:22.559901 zenaura-0.9.50/setup.cfg
--rw-rw-rw-   0        0        0      709 2024-05-26 14:19:14.000000 zenaura-0.9.50/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:19:22.551898 zenaura-0.9.50/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 13:51:25.000000 zenaura-0.9.50/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6603 2024-05-26 14:05:43.000000 zenaura-0.9.50/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 14:03:42.000000 zenaura-0.9.50/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 14:03:42.000000 zenaura-0.9.50/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 13:51:25.000000 zenaura-0.9.50/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 14:03:42.000000 zenaura-0.9.50/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.50/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 14:03:42.000000 zenaura-0.9.50/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 13:56:00.000000 zenaura-0.9.50/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-18 19:29:37.000000 zenaura-0.9.50/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 14:03:42.000000 zenaura-0.9.50/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:19:22.552398 zenaura-0.9.50/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-11 11:31:00.000000 zenaura-0.9.50/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:19:22.558901 zenaura-0.9.50/zenaura.egg-info/
--rw-rw-rw-   0        0        0     1781 2024-05-26 14:19:22.000000 zenaura-0.9.50/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-05-26 14:19:22.000000 zenaura-0.9.50/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:19:22.000000 zenaura-0.9.50/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 14:19:22.000000 zenaura-0.9.50/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 15:24:47.521991 zenaura-0.9.51/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.51/LICENSE
+-rw-rw-rw-   0        0        0     1804 2024-05-26 15:24:47.521492 zenaura-0.9.51/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-18 13:42:46.000000 zenaura-0.9.51/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:24:47.521991 zenaura-0.9.51/setup.cfg
+-rw-rw-rw-   0        0        0      690 2024-05-26 15:18:58.000000 zenaura-0.9.51/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:24:47.509491 zenaura-0.9.51/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 13:51:25.000000 zenaura-0.9.51/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6591 2024-05-26 14:35:19.000000 zenaura-0.9.51/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 14:03:42.000000 zenaura-0.9.51/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 14:03:42.000000 zenaura-0.9.51/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 13:51:25.000000 zenaura-0.9.51/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 14:03:42.000000 zenaura-0.9.51/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.51/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 14:03:42.000000 zenaura-0.9.51/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 13:56:00.000000 zenaura-0.9.51/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-18 19:29:37.000000 zenaura-0.9.51/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 14:03:42.000000 zenaura-0.9.51/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:24:47.510491 zenaura-0.9.51/zenaura/
+-rw-rw-rw-   0        0        0      373 2024-05-26 15:23:29.000000 zenaura-0.9.51/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:24:47.520992 zenaura-0.9.51/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     1804 2024-05-26 15:24:47.000000 zenaura-0.9.51/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-05-26 15:24:47.000000 zenaura-0.9.51/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:24:47.000000 zenaura-0.9.51/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 15:24:47.000000 zenaura-0.9.51/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 15:24:47.000000 zenaura-0.9.51/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.50/LICENSE` & `zenaura-0.9.51/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/PKG-INFO` & `zenaura-0.9.51/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.50
+Version: 0.9.51
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: bleach
 
 # Zenaura 
 
 <img title="a title" alt="Alt text" src="./assets/logo.png" width="300" height="300" />
 
 Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
```

### Comparing `zenaura-0.9.50/README.md` & `zenaura-0.9.51/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/setup.py` & `zenaura-0.9.51/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.50',
+    version='0.9.51',
     description="Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura'],
     install_requires=[
-        # Add any dependencies here
+        'bleach'
     ],
     test_suite='tests',
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

### Comparing `zenaura-0.9.50/tests/test_algorithm.py` & `zenaura-0.9.51/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/tests/test_app.py` & `zenaura-0.9.51/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import unittest
 from unittest.mock import MagicMock, patch
-from zenaura.client.page import Page
+from zenaura import Page
 
 
 
 sys.modules["pyscript"] = MagicMock()
 
 class TestApp(unittest.TestCase):
```

### Comparing `zenaura-0.9.50/tests/test_compiler.py` & `zenaura-0.9.51/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/tests/test_component_e2e.py` & `zenaura-0.9.51/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/tests/test_component_unit.py` & `zenaura-0.9.51/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/tests/test_node_properties.py` & `zenaura-0.9.51/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/tests/test_observer.py` & `zenaura-0.9.51/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/tests/test_rdom_adapter.py` & `zenaura-0.9.51/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/tests/test_tags.py` & `zenaura-0.9.51/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/tests/test_tasker.py` & `zenaura-0.9.51/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/tests/test_zenaura_dom.py` & `zenaura-0.9.51/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.50/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.51/zenaura.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.50
+Version: 0.9.51
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: bleach
 
 # Zenaura 
 
 <img title="a title" alt="Alt text" src="./assets/logo.png" width="300" height="300" />
 
 Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
```

