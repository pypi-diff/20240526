# Comparing `tmp/zenaura-0.9.77.tar.gz` & `tmp/zenaura-0.9.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.77.tar", last modified: Sun May 26 18:57:47 2024, max compression
+gzip compressed data, was "zenaura-0.9.78.tar", last modified: Sun May 26 19:02:37 2024, max compression
```

## Comparing `zenaura-0.9.77.tar` & `zenaura-0.9.78.tar`

### file list

```diff
@@ -1,39 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 18:57:47.000456 zenaura-0.9.77/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.77/LICENSE
--rw-rw-rw-   0        0        0     2028 2024-05-26 18:57:46.999956 zenaura-0.9.77/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.77/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 18:57:47.000956 zenaura-0.9.77/setup.cfg
--rw-rw-rw-   0        0        0      950 2024-05-26 18:57:15.000000 zenaura-0.9.77/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:57:46.985456 zenaura-0.9.77/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6591 2024-05-26 18:57:08.000000 zenaura-0.9.77/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.77/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:57:46.985957 zenaura-0.9.77/zenaura/
--rw-rw-rw-   0        0        0      229 2024-05-26 18:57:08.000000 zenaura-0.9.77/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:57:46.997956 zenaura-0.9.77/zenaura/client/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.77/zenaura/client/__init__.py
--rw-rw-rw-   0        0        0     8990 2024-05-26 18:57:08.000000 zenaura-0.9.77/zenaura/client/app.py
--rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.77/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.77/zenaura/client/config.py
--rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.77/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.77/zenaura/client/mutator.py
--rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.77/zenaura/client/observer.py
--rw-rw-rw-   0        0        0      943 2024-05-26 17:44:57.000000 zenaura-0.9.77/zenaura/client/page.py
--rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.77/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:57:46.998457 zenaura-0.9.77/zenaura/server/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:57:25.000000 zenaura-0.9.77/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0     1237 2024-05-26 18:57:08.000000 zenaura-0.9.77/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:57:46.999456 zenaura-0.9.77/zenaura.egg-info/
--rw-rw-rw-   0        0        0     2028 2024-05-26 18:57:46.000000 zenaura-0.9.77/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      752 2024-05-26 18:57:46.000000 zenaura-0.9.77/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 18:57:46.000000 zenaura-0.9.77/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 18:57:46.000000 zenaura-0.9.77/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 18:57:46.000000 zenaura-0.9.77/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.114938 zenaura-0.9.78/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.78/LICENSE
+-rw-rw-rw-   0        0        0     2028 2024-05-26 19:02:37.113938 zenaura-0.9.78/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.78/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 19:02:37.114938 zenaura-0.9.78/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2024-05-26 19:02:32.000000 zenaura-0.9.78/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.086938 zenaura-0.9.78/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6591 2024-05-26 18:57:08.000000 zenaura-0.9.78/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.78/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.087437 zenaura-0.9.78/zenaura/
+-rw-rw-rw-   0        0        0      229 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.099937 zenaura-0.9.78/zenaura/client/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.78/zenaura/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.102438 zenaura-0.9.78/zenaura/client/algorithm/
+-rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/algorithm/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/algorithm/algorithm.py
+-rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/algorithm/operations.py
+-rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/algorithm/searcher.py
+-rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/algorithm/updater.py
+-rw-rw-rw-   0        0        0     8990 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/app.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.104437 zenaura-0.9.78/zenaura/client/compiler/
+-rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/compiler/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/compiler/attribute.py
+-rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/compiler/compiler.py
+-rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/compiler/sanitize.py
+-rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/config.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.107437 zenaura-0.9.78/zenaura/client/hydrator/
+-rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/hydrator/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/hydrator/compiler_adapter.py
+-rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/hydrator/hydrator.py
+-rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/hydrator/lookup.py
+-rw-rw-rw-   0        0        0     6943 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/hydrator/real_dom_adapter.py
+-rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/hydrator/tasker.py
+-rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/hydrator/virtual_dom_adapter.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/client/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.108937 zenaura-0.9.78/zenaura/client/observer/
+-rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/observer/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/observer/observer.py
+-rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/observer/subject.py
+-rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      943 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.111937 zenaura-0.9.78/zenaura/client/tags/
+-rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/tags/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/tags/attribute.py
+-rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/tags/builder.py
+-rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/tags/data.py
+-rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/tags/html.py
+-rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.78/zenaura/client/tags/node.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.112437 zenaura-0.9.78/zenaura/server/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:57:25.000000 zenaura-0.9.78/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     1237 2024-05-26 18:57:08.000000 zenaura-0.9.78/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-26 19:02:37.113437 zenaura-0.9.78/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     2028 2024-05-26 19:02:37.000000 zenaura-0.9.78/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1646 2024-05-26 19:02:37.000000 zenaura-0.9.78/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 19:02:37.000000 zenaura-0.9.78/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 19:02:37.000000 zenaura-0.9.78/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 19:02:37.000000 zenaura-0.9.78/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.77/LICENSE` & `zenaura-0.9.78/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/PKG-INFO` & `zenaura-0.9.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.77
+Version: 0.9.78
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.77/README.md` & `zenaura-0.9.78/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/setup.py` & `zenaura-0.9.78/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.77',
+    version='0.9.78',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
-    packages=['zenaura', 'zenaura.server', 'zenaura.client'],
+    packages=['zenaura', 'zenaura.server', 'zenaura.client', 'zenaura.client.algorithm', 'zenaura.client.compiler', 'zenaura.client.hydrator', 'zenaura.client.observer', 'zenaura.client.tags'],
     install_requires=[
         'bleach'
     ],
     test_suite='tests',
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

### Comparing `zenaura-0.9.77/tests/test_algorithm.py` & `zenaura-0.9.78/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_app.py` & `zenaura-0.9.78/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_compiler.py` & `zenaura-0.9.78/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_component_e2e.py` & `zenaura-0.9.78/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_component_unit.py` & `zenaura-0.9.78/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_node_properties.py` & `zenaura-0.9.78/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_observer.py` & `zenaura-0.9.78/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_rdom_adapter.py` & `zenaura-0.9.78/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_tags.py` & `zenaura-0.9.78/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_tasker.py` & `zenaura-0.9.78/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/tests/test_zenaura_dom.py` & `zenaura-0.9.78/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura/client/app.py` & `zenaura-0.9.78/zenaura/client/app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura/client/component.py` & `zenaura-0.9.78/zenaura/client/component.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura/client/config.py` & `zenaura-0.9.78/zenaura/client/config.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura/client/mocks.py` & `zenaura-0.9.78/zenaura/client/mocks.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura/client/mutator.py` & `zenaura-0.9.78/zenaura/client/mutator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura/client/observer.py` & `zenaura-0.9.78/zenaura/client/observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura/client/page.py` & `zenaura-0.9.78/zenaura/client/page.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura/client/persistance.py` & `zenaura-0.9.78/zenaura/client/persistance.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura/server/server.py` & `zenaura-0.9.78/zenaura/server/server.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.77/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.78/zenaura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.77
+Version: 0.9.78
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.77/zenaura.egg-info/SOURCES.txt` & `zenaura-0.9.78/zenaura.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -23,9 +23,34 @@
 zenaura/client/component.py
 zenaura/client/config.py
 zenaura/client/mocks.py
 zenaura/client/mutator.py
 zenaura/client/observer.py
 zenaura/client/page.py
 zenaura/client/persistance.py
+zenaura/client/algorithm/__init__.py
+zenaura/client/algorithm/algorithm.py
+zenaura/client/algorithm/operations.py
+zenaura/client/algorithm/searcher.py
+zenaura/client/algorithm/updater.py
+zenaura/client/compiler/__init__.py
+zenaura/client/compiler/attribute.py
+zenaura/client/compiler/compiler.py
+zenaura/client/compiler/sanitize.py
+zenaura/client/hydrator/__init__.py
+zenaura/client/hydrator/compiler_adapter.py
+zenaura/client/hydrator/hydrator.py
+zenaura/client/hydrator/lookup.py
+zenaura/client/hydrator/real_dom_adapter.py
+zenaura/client/hydrator/tasker.py
+zenaura/client/hydrator/virtual_dom_adapter.py
+zenaura/client/observer/__init__.py
+zenaura/client/observer/observer.py
+zenaura/client/observer/subject.py
+zenaura/client/tags/__init__.py
+zenaura/client/tags/attribute.py
+zenaura/client/tags/builder.py
+zenaura/client/tags/data.py
+zenaura/client/tags/html.py
+zenaura/client/tags/node.py
 zenaura/server/__init__.py
 zenaura/server/server.py
```

