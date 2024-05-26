# Comparing `tmp/zenaura-0.9.53.tar.gz` & `tmp/zenaura-0.9.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.53.tar", last modified: Sun May 26 15:47:48 2024, max compression
+gzip compressed data, was "zenaura-0.9.54.tar", last modified: Sun May 26 15:50:36 2024, max compression
```

## Comparing `zenaura-0.9.53.tar` & `zenaura-0.9.54.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:47:48.234795 zenaura-0.9.53/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.53/LICENSE
--rw-rw-rw-   0        0        0     1804 2024-05-26 15:47:48.234295 zenaura-0.9.53/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-18 13:42:46.000000 zenaura-0.9.53/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 15:47:48.234795 zenaura-0.9.53/setup.cfg
--rw-rw-rw-   0        0        0      690 2024-05-26 15:47:29.000000 zenaura-0.9.53/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:47:48.224295 zenaura-0.9.53/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 13:51:25.000000 zenaura-0.9.53/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6591 2024-05-26 14:35:19.000000 zenaura-0.9.53/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 14:03:42.000000 zenaura-0.9.53/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 14:03:42.000000 zenaura-0.9.53/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 13:51:25.000000 zenaura-0.9.53/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 14:03:42.000000 zenaura-0.9.53/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.53/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 14:03:42.000000 zenaura-0.9.53/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 13:56:00.000000 zenaura-0.9.53/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-18 19:29:37.000000 zenaura-0.9.53/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 14:03:42.000000 zenaura-0.9.53/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:47:48.225795 zenaura-0.9.53/zenaura/
--rw-rw-rw-   0        0        0      373 2024-05-26 15:47:13.000000 zenaura-0.9.53/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:47:48.233295 zenaura-0.9.53/zenaura.egg-info/
--rw-rw-rw-   0        0        0     1804 2024-05-26 15:47:48.000000 zenaura-0.9.53/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-05-26 15:47:48.000000 zenaura-0.9.53/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:47:48.000000 zenaura-0.9.53/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 15:47:48.000000 zenaura-0.9.53/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 15:47:48.000000 zenaura-0.9.53/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 15:50:36.389177 zenaura-0.9.54/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.54/LICENSE
+-rw-rw-rw-   0        0        0     1804 2024-05-26 15:50:36.389177 zenaura-0.9.54/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-18 13:42:46.000000 zenaura-0.9.54/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:50:36.389177 zenaura-0.9.54/setup.cfg
+-rw-rw-rw-   0        0        0      690 2024-05-26 15:50:32.000000 zenaura-0.9.54/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:50:36.381161 zenaura-0.9.54/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 13:51:25.000000 zenaura-0.9.54/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6591 2024-05-26 14:35:19.000000 zenaura-0.9.54/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 14:03:42.000000 zenaura-0.9.54/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 14:03:42.000000 zenaura-0.9.54/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 13:51:25.000000 zenaura-0.9.54/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 14:03:42.000000 zenaura-0.9.54/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.54/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 14:03:42.000000 zenaura-0.9.54/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 13:56:00.000000 zenaura-0.9.54/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-18 19:29:37.000000 zenaura-0.9.54/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 14:03:42.000000 zenaura-0.9.54/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:50:36.381661 zenaura-0.9.54/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-26 15:50:23.000000 zenaura-0.9.54/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:50:36.388172 zenaura-0.9.54/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     1804 2024-05-26 15:50:36.000000 zenaura-0.9.54/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-05-26 15:50:36.000000 zenaura-0.9.54/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:50:36.000000 zenaura-0.9.54/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 15:50:36.000000 zenaura-0.9.54/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 15:50:36.000000 zenaura-0.9.54/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.53/LICENSE` & `zenaura-0.9.54/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/PKG-INFO` & `zenaura-0.9.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.53
+Version: 0.9.54
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.53/README.md` & `zenaura-0.9.54/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/setup.py` & `zenaura-0.9.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.53',
+    version='0.9.54',
     description="Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura'],
     install_requires=[
         'bleach'
     ],
```

### Comparing `zenaura-0.9.53/tests/test_algorithm.py` & `zenaura-0.9.54/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_app.py` & `zenaura-0.9.54/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_compiler.py` & `zenaura-0.9.54/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_component_e2e.py` & `zenaura-0.9.54/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_component_unit.py` & `zenaura-0.9.54/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_node_properties.py` & `zenaura-0.9.54/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_observer.py` & `zenaura-0.9.54/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_rdom_adapter.py` & `zenaura-0.9.54/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_tags.py` & `zenaura-0.9.54/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_tasker.py` & `zenaura-0.9.54/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/tests/test_zenaura_dom.py` & `zenaura-0.9.54/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.53/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.54/zenaura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.53
+Version: 0.9.54
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

