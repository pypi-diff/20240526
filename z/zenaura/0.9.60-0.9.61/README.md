# Comparing `tmp/zenaura-0.9.60.tar.gz` & `tmp/zenaura-0.9.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.60.tar", last modified: Sun May 26 16:57:02 2024, max compression
+gzip compressed data, was "zenaura-0.9.61.tar", last modified: Sun May 26 17:02:38 2024, max compression
```

## Comparing `zenaura-0.9.60.tar` & `zenaura-0.9.61.tar`

### file list

```diff
@@ -1,73 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.854655 zenaura-0.9.60/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.60/LICENSE
--rw-rw-rw-   0        0        0      607 2024-05-26 16:57:02.854155 zenaura-0.9.60/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 16:57:02.854655 zenaura-0.9.60/setup.cfg
--rw-rw-rw-   0        0        0      785 2024-05-26 16:56:23.000000 zenaura-0.9.60/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.823655 zenaura-0.9.60/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6591 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 16:54:28.000000 zenaura-0.9.60/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.817149 zenaura-0.9.60/zenaura/
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.828155 zenaura-0.9.60/zenaura/client/
--rw-rw-rw-   0        0        0      213 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.830655 zenaura-0.9.60/zenaura/client/algorithm/
--rw-rw-rw-   0        0        0       39 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/algorithm/__init__.py
--rw-rw-rw-   0        0        0      193 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/algorithm/algorithm.py
--rw-rw-rw-   0        0        0      972 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/algorithm/operations.py
--rw-rw-rw-   0        0        0     7166 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/algorithm/searcher.py
--rw-rw-rw-   0        0        0     2772 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/algorithm/updater.py
--rw-rw-rw-   0        0        0     8990 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/app.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.832656 zenaura-0.9.60/zenaura/client/compiler/
--rw-rw-rw-   0        0        0       53 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/compiler/__init__.py
--rw-rw-rw-   0        0        0     1403 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/compiler/attribute.py
--rw-rw-rw-   0        0        0     3471 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/compiler/compiler.py
--rw-rw-rw-   0        0        0     1132 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/compiler/sanitize.py
--rw-rw-rw-   0        0        0     4093 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/config.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.835155 zenaura-0.9.60/zenaura/client/dom/
--rw-rw-rw-   0        0        0       43 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/dom/__init__.py
--rw-rw-rw-   0        0        0      280 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/dom/dom.py
--rw-rw-rw-   0        0        0     1803 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/dom/error.py
--rw-rw-rw-   0        0        0     1852 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/dom/mount.py
--rw-rw-rw-   0        0        0     1883 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/dom/render.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.838655 zenaura-0.9.60/zenaura/client/hydrator/
--rw-rw-rw-   0        0        0      235 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/hydrator/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/hydrator/compiler_adapter.py
--rw-rw-rw-   0        0        0     1236 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/hydrator/hydrator.py
--rw-rw-rw-   0        0        0     1346 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/hydrator/lookup.py
--rw-rw-rw-   0        0        0     6943 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/hydrator/real_dom_adapter.py
--rw-rw-rw-   0        0        0     2264 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/hydrator/tasker.py
--rw-rw-rw-   0        0        0     1064 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/hydrator/virtual_dom_adapter.py
--rw-rw-rw-   0        0        0     2631 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0      896 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.840156 zenaura-0.9.60/zenaura/client/observer/
--rw-rw-rw-   0        0        0       60 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/observer/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/observer/observer.py
--rw-rw-rw-   0        0        0     1609 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/observer/subject.py
--rw-rw-rw-   0        0        0     2009 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/observer.py
--rw-rw-rw-   0        0        0      943 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/page.py
--rw-rw-rw-   0        0        0     2212 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.842655 zenaura-0.9.60/zenaura/client/tags/
--rw-rw-rw-   0        0        0      165 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/tags/__init__.py
--rw-rw-rw-   0        0        0      429 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/tags/attribute.py
--rw-rw-rw-   0        0        0     4666 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/tags/builder.py
--rw-rw-rw-   0        0        0      418 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/tags/data.py
--rw-rw-rw-   0        0        0      473 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/tags/html.py
--rw-rw-rw-   0        0        0    10231 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/client/tags/node.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.843655 zenaura-0.9.60/zenaura/server/
--rw-rw-rw-   0        0        0       33 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0     1237 2024-05-26 16:54:28.000000 zenaura-0.9.60/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:57:02.853655 zenaura-0.9.60/zenaura/zenaura.egg-info/
--rw-rw-rw-   0        0        0      607 2024-05-26 16:57:02.000000 zenaura-0.9.60/zenaura/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1798 2024-05-26 16:57:02.000000 zenaura-0.9.60/zenaura/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 16:57:02.000000 zenaura-0.9.60/zenaura/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 16:57:02.000000 zenaura-0.9.60/zenaura/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-26 16:57:02.000000 zenaura-0.9.60/zenaura/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 17:02:38.511882 zenaura-0.9.61/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.61/LICENSE
+-rw-rw-rw-   0        0        0      607 2024-05-26 17:02:38.511383 zenaura-0.9.61/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.61/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 17:02:38.511882 zenaura-0.9.61/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-05-26 17:00:41.000000 zenaura-0.9.61/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:02:38.501373 zenaura-0.9.61/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6591 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 16:54:28.000000 zenaura-0.9.61/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:02:38.502373 zenaura-0.9.61/zenaura/
+-rw-rw-rw-   0        0        0      229 2024-05-26 16:54:28.000000 zenaura-0.9.61/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:02:38.510881 zenaura-0.9.61/zenaura.egg-info/
+-rw-rw-rw-   0        0        0      607 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 17:02:38.000000 zenaura-0.9.61/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.60/LICENSE` & `zenaura-0.9.61/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/PKG-INFO` & `zenaura-0.9.61/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.60
+Version: 0.9.61
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.60/setup.py` & `zenaura-0.9.61/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name='zenaura',
-    version='0.9.60',
+    version='0.9.61',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
-    package_dir={"": "zenaura"},
-    packages=find_packages(where='zenaura'),
+    packages=['zenaura'],
     install_requires=[
         'bleach'
     ],
     test_suite='tests',
 )
```

### Comparing `zenaura-0.9.60/tests/test_algorithm.py` & `zenaura-0.9.61/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_app.py` & `zenaura-0.9.61/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_compiler.py` & `zenaura-0.9.61/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_component_e2e.py` & `zenaura-0.9.61/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_component_unit.py` & `zenaura-0.9.61/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_node_properties.py` & `zenaura-0.9.61/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_observer.py` & `zenaura-0.9.61/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_rdom_adapter.py` & `zenaura-0.9.61/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_tags.py` & `zenaura-0.9.61/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_tasker.py` & `zenaura-0.9.61/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/tests/test_zenaura_dom.py` & `zenaura-0.9.61/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.60/zenaura/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.61/zenaura.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.60
+Version: 0.9.61
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 License-File: LICENSE
 Requires-Dist: bleach
```

