# Comparing `tmp/zenaura-0.9.63.tar.gz` & `tmp/zenaura-0.9.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.63.tar", last modified: Sun May 26 17:06:15 2024, max compression
+gzip compressed data, was "zenaura-0.9.65.tar", last modified: Sun May 26 17:19:48 2024, max compression
```

## Comparing `zenaura-0.9.63.tar` & `zenaura-0.9.65.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 17:06:15.075318 zenaura-0.9.63/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.63/LICENSE
--rw-rw-rw-   0        0        0      607 2024-05-26 17:06:15.074818 zenaura-0.9.63/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.63/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 17:06:15.075819 zenaura-0.9.63/setup.cfg
--rw-rw-rw-   0        0        0      822 2024-05-26 17:05:53.000000 zenaura-0.9.63/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:06:15.064815 zenaura-0.9.63/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6591 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 16:54:28.000000 zenaura-0.9.63/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:06:15.065314 zenaura-0.9.63/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-26 17:05:47.000000 zenaura-0.9.63/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:06:15.074319 zenaura-0.9.63/zenaura.egg-info/
--rw-rw-rw-   0        0        0      607 2024-05-26 17:06:15.000000 zenaura-0.9.63/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-05-26 17:06:15.000000 zenaura-0.9.63/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 17:06:15.000000 zenaura-0.9.63/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 17:06:15.000000 zenaura-0.9.63/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 17:06:15.000000 zenaura-0.9.63/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.430693 zenaura-0.9.65/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.65/LICENSE
+-rw-rw-rw-   0        0        0     1804 2024-05-26 17:19:48.430194 zenaura-0.9.65/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.65/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 17:19:48.430693 zenaura-0.9.65/setup.cfg
+-rw-rw-rw-   0        0        0      802 2024-05-26 17:19:41.000000 zenaura-0.9.65/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.404566 zenaura-0.9.65/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.404566 zenaura-0.9.65/src/zenaura/
+drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.421543 zenaura-0.9.65/src/zenaura/client/
+-rw-rw-rw-   0        0        0      213 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/__init__.py
+-rw-rw-rw-   0        0        0     8990 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/app.py
+-rw-rw-rw-   0        0        0     4093 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/config.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      896 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/mutator.py
+-rw-rw-rw-   0        0        0     2009 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      943 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.422342 zenaura-0.9.65/src/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     1237 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.429694 zenaura-0.9.65/src/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     1804 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      796 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.429192 zenaura-0.9.65/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6603 2024-05-26 17:16:47.000000 zenaura-0.9.65/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_zenaura_dom.py
```

### Comparing `zenaura-0.9.63/LICENSE` & `zenaura-0.9.65/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/README.md` & `zenaura-0.9.65/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/setup.py` & `zenaura-0.9.65/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.63',
-    description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
+    version='0.9.65',
+    description="Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
-    packages=['zenaura'],
+     packages=find_namespace_packages(where='src', include=['zenaura.client', 'zenaura.server']),
+    package_dir={'': 'src'},
     install_requires=[
         'bleach'
     ],
     test_suite='tests',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
 )
```

### Comparing `zenaura-0.9.63/tests/test_algorithm.py` & `zenaura-0.9.65/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/tests/test_app.py` & `zenaura-0.9.65/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 import unittest
 from unittest.mock import MagicMock, patch
-from zenaura import Page
+from zenaura.client.page import Page
 
 
 
 sys.modules["pyscript"] = MagicMock()
 
 class TestApp(unittest.TestCase):
```

### Comparing `zenaura-0.9.63/tests/test_compiler.py` & `zenaura-0.9.65/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/tests/test_component_e2e.py` & `zenaura-0.9.65/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/tests/test_component_unit.py` & `zenaura-0.9.65/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/tests/test_node_properties.py` & `zenaura-0.9.65/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/tests/test_observer.py` & `zenaura-0.9.65/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/tests/test_rdom_adapter.py` & `zenaura-0.9.65/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/tests/test_tags.py` & `zenaura-0.9.65/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/tests/test_tasker.py` & `zenaura-0.9.65/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.63/tests/test_zenaura_dom.py` & `zenaura-0.9.65/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

