# Comparing `tmp/zenaura-0.9.61.tar.gz` & `tmp/zenaura-0.9.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.61.tar", last modified: Sun May 26 17:02:38 2024, max compression
+gzip compressed data, was "zenaura-0.9.62.tar", last modified: Sun May 26 17:04:54 2024, max compression
```

## Comparing `zenaura-0.9.61.tar` & `zenaura-0.9.62.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 17:02:38.511882 zenaura-0.9.61/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.61/LICENSE
--rw-rw-rw-   0        0        0      607 2024-05-26 17:02:38.511383 zenaura-0.9.61/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.61/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 17:02:38.511882 zenaura-0.9.61/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-05-26 17:00:41.000000 zenaura-0.9.61/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:02:38.501373 zenaura-0.9.61/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6591 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:02:38.502373 zenaura-0.9.61/zenaura/
--rw-rw-rw-   0        0        0      229 2024-05-26 16:54:28.000000 zenaura-0.9.61/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:02:38.510881 zenaura-0.9.61/zenaura.egg-info/
--rw-rw-rw-   0        0        0      607 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 17:04:54.561017 zenaura-0.9.62/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.62/LICENSE
+-rw-rw-rw-   0        0        0      607 2024-05-26 17:04:54.560517 zenaura-0.9.62/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.62/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 17:04:54.561516 zenaura-0.9.62/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-05-26 17:04:49.000000 zenaura-0.9.62/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:04:54.551517 zenaura-0.9.62/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6591 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 16:54:28.000000 zenaura-0.9.62/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:04:54.552517 zenaura-0.9.62/zenaura/
+-rw-rw-rw-   0        0        0      243 2024-05-26 17:04:45.000000 zenaura-0.9.62/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:04:54.560017 zenaura-0.9.62/zenaura.egg-info/
+-rw-rw-rw-   0        0        0      607 2024-05-26 17:04:54.000000 zenaura-0.9.62/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-05-26 17:04:54.000000 zenaura-0.9.62/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 17:04:54.000000 zenaura-0.9.62/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 17:04:54.000000 zenaura-0.9.62/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 17:04:54.000000 zenaura-0.9.62/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.61/LICENSE` & `zenaura-0.9.62/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/PKG-INFO` & `zenaura-0.9.62/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.61
+Version: 0.9.62
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.61/README.md` & `zenaura-0.9.62/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/setup.py` & `zenaura-0.9.62/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.61',
+    version='0.9.62',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura'],
     install_requires=[
         'bleach'
     ],
```

### Comparing `zenaura-0.9.61/tests/test_algorithm.py` & `zenaura-0.9.62/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_app.py` & `zenaura-0.9.62/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_compiler.py` & `zenaura-0.9.62/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_component_e2e.py` & `zenaura-0.9.62/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_component_unit.py` & `zenaura-0.9.62/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_node_properties.py` & `zenaura-0.9.62/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_observer.py` & `zenaura-0.9.62/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_rdom_adapter.py` & `zenaura-0.9.62/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_tags.py` & `zenaura-0.9.62/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_tasker.py` & `zenaura-0.9.62/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/tests/test_zenaura_dom.py` & `zenaura-0.9.62/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.61/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.62/zenaura.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.61
+Version: 0.9.62
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 License-File: LICENSE
 Requires-Dist: bleach
```

