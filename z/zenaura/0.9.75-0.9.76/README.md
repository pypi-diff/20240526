# Comparing `tmp/zenaura-0.9.75.tar.gz` & `tmp/zenaura-0.9.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.75.tar", last modified: Sun May 26 18:50:45 2024, max compression
+gzip compressed data, was "zenaura-0.9.76.tar", last modified: Sun May 26 18:55:11 2024, max compression
```

## Comparing `zenaura-0.9.75.tar` & `zenaura-0.9.76.tar`

### file list

```diff
@@ -1,27 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 18:50:45.074887 zenaura-0.9.75/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.75/LICENSE
--rw-rw-rw-   0        0        0     2028 2024-05-26 18:50:45.074388 zenaura-0.9.75/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.75/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 18:50:45.074887 zenaura-0.9.75/setup.cfg
--rw-rw-rw-   0        0        0      944 2024-05-26 18:50:39.000000 zenaura-0.9.75/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:50:45.046432 zenaura-0.9.75/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 18:50:45.048432 zenaura-0.9.75/src/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:44:14.000000 zenaura-0.9.75/src/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 18:50:45.073386 zenaura-0.9.75/src/zenaura.egg-info/
--rw-rw-rw-   0        0        0     2028 2024-05-26 18:50:45.000000 zenaura-0.9.75/src/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2024-05-26 18:50:45.000000 zenaura-0.9.75/src/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 18:50:45.000000 zenaura-0.9.75/src/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 18:50:45.000000 zenaura-0.9.75/src/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 18:50:45.000000 zenaura-0.9.75/src/zenaura.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 18:50:45.072887 zenaura-0.9.75/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6603 2024-05-26 18:05:15.000000 zenaura-0.9.75/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.75/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:55:11.613195 zenaura-0.9.76/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.76/LICENSE
+-rw-rw-rw-   0        0        0     2028 2024-05-26 18:55:11.613195 zenaura-0.9.76/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.76/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 18:55:11.614092 zenaura-0.9.76/setup.cfg
+-rw-rw-rw-   0        0        0      950 2024-05-26 18:55:07.000000 zenaura-0.9.76/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:55:11.598194 zenaura-0.9.76/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6603 2024-05-26 18:05:15.000000 zenaura-0.9.76/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.76/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:55:11.598694 zenaura-0.9.76/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:44:14.000000 zenaura-0.9.76/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:55:11.611194 zenaura-0.9.76/zenaura/client/
+-rw-rw-rw-   0        0        0      213 2024-05-26 17:44:57.000000 zenaura-0.9.76/zenaura/client/__init__.py
+-rw-rw-rw-   0        0        0     8920 2024-05-26 18:41:50.000000 zenaura-0.9.76/zenaura/client/app.py
+-rw-rw-rw-   0        0        0     4045 2024-05-26 18:38:12.000000 zenaura-0.9.76/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.76/zenaura/client/config.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.76/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      882 2024-05-26 18:38:28.000000 zenaura-0.9.76/zenaura/client/mutator.py
+-rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.76/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      943 2024-05-26 17:44:57.000000 zenaura-0.9.76/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.76/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:55:11.612194 zenaura-0.9.76/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 17:44:57.000000 zenaura-0.9.76/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     1225 2024-05-26 18:40:29.000000 zenaura-0.9.76/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:55:11.612694 zenaura-0.9.76/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     2028 2024-05-26 18:55:11.000000 zenaura-0.9.76/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      752 2024-05-26 18:55:11.000000 zenaura-0.9.76/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:55:11.000000 zenaura-0.9.76/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 18:55:11.000000 zenaura-0.9.76/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 18:55:11.000000 zenaura-0.9.76/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.75/LICENSE` & `zenaura-0.9.76/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/PKG-INFO` & `zenaura-0.9.76/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.75
+Version: 0.9.76
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.75/README.md` & `zenaura-0.9.76/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/setup.py` & `zenaura-0.9.76/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.75',
+    version='0.9.76',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
-    package_dir={"": "src"},
-    packages=["zenaura"],
+    packages=['zenaura', 'zenaura.server', 'zenaura.client'],
     install_requires=[
         'bleach'
     ],
     test_suite='tests',
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

### Comparing `zenaura-0.9.75/src/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.76/zenaura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.75
+Version: 0.9.76
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.75/tests/test_algorithm.py` & `zenaura-0.9.76/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_app.py` & `zenaura-0.9.76/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_compiler.py` & `zenaura-0.9.76/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_component_e2e.py` & `zenaura-0.9.76/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_component_unit.py` & `zenaura-0.9.76/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_node_properties.py` & `zenaura-0.9.76/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_observer.py` & `zenaura-0.9.76/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_rdom_adapter.py` & `zenaura-0.9.76/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_tags.py` & `zenaura-0.9.76/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_tasker.py` & `zenaura-0.9.76/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.75/tests/test_zenaura_dom.py` & `zenaura-0.9.76/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

