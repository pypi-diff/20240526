# Comparing `tmp/zenaura-0.9.65.tar.gz` & `tmp/zenaura-0.9.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.65.tar", last modified: Sun May 26 17:19:48 2024, max compression
+gzip compressed data, was "zenaura-0.9.66.tar", last modified: Sun May 26 17:31:16 2024, max compression
```

## Comparing `zenaura-0.9.65.tar` & `zenaura-0.9.66.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.430693 zenaura-0.9.65/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.65/LICENSE
--rw-rw-rw-   0        0        0     1804 2024-05-26 17:19:48.430194 zenaura-0.9.65/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.65/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 17:19:48.430693 zenaura-0.9.65/setup.cfg
--rw-rw-rw-   0        0        0      802 2024-05-26 17:19:41.000000 zenaura-0.9.65/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.404566 zenaura-0.9.65/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.404566 zenaura-0.9.65/src/zenaura/
-drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.421543 zenaura-0.9.65/src/zenaura/client/
--rw-rw-rw-   0        0        0      213 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/__init__.py
--rw-rw-rw-   0        0        0     8990 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/app.py
--rw-rw-rw-   0        0        0     4093 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/config.py
--rw-rw-rw-   0        0        0     2631 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0      896 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/mutator.py
--rw-rw-rw-   0        0        0     2009 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/observer.py
--rw-rw-rw-   0        0        0      943 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/page.py
--rw-rw-rw-   0        0        0     2212 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.422342 zenaura-0.9.65/src/zenaura/server/
--rw-rw-rw-   0        0        0       33 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0     1237 2024-05-26 17:13:43.000000 zenaura-0.9.65/src/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.429694 zenaura-0.9.65/src/zenaura.egg-info/
--rw-rw-rw-   0        0        0     1804 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      796 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 17:19:48.000000 zenaura-0.9.65/src/zenaura.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 17:19:48.429192 zenaura-0.9.65/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6603 2024-05-26 17:16:47.000000 zenaura-0.9.65/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 17:13:43.000000 zenaura-0.9.65/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:31:16.419290 zenaura-0.9.66/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.66/LICENSE
+-rw-rw-rw-   0        0        0     1804 2024-05-26 17:31:16.418286 zenaura-0.9.66/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.66/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 17:31:16.419290 zenaura-0.9.66/setup.cfg
+-rw-rw-rw-   0        0        0      802 2024-05-26 17:31:06.000000 zenaura-0.9.66/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:31:16.392786 zenaura-0.9.66/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 17:31:16.392786 zenaura-0.9.66/src/zenaura/
+drwxrwxrwx   0        0        0        0 2024-05-26 17:31:16.410286 zenaura-0.9.66/src/zenaura/client/
+-rw-rw-rw-   0        0        0      213 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/client/__init__.py
+-rw-rw-rw-   0        0        0     8990 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/client/app.py
+-rw-rw-rw-   0        0        0     4093 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/client/config.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      896 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/client/mutator.py
+-rw-rw-rw-   0        0        0     2009 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      943 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:31:16.410787 zenaura-0.9.66/src/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     1237 2024-05-26 17:13:43.000000 zenaura-0.9.66/src/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:31:16.417287 zenaura-0.9.66/src/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     1804 2024-05-26 17:31:16.000000 zenaura-0.9.66/src/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      796 2024-05-26 17:31:16.000000 zenaura-0.9.66/src/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 17:31:16.000000 zenaura-0.9.66/src/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 17:31:16.000000 zenaura-0.9.66/src/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 17:31:16.000000 zenaura-0.9.66/src/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 17:31:16.416787 zenaura-0.9.66/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6603 2024-05-26 17:16:47.000000 zenaura-0.9.66/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:13:43.000000 zenaura-0.9.66/tests/test_zenaura_dom.py
```

### Comparing `zenaura-0.9.65/LICENSE` & `zenaura-0.9.66/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/PKG-INFO` & `zenaura-0.9.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.65
+Version: 0.9.66
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.65/README.md` & `zenaura-0.9.66/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/setup.py` & `zenaura-0.9.66/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.65',
+    version='0.9.66',
     description="Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
      packages=find_namespace_packages(where='src', include=['zenaura.client', 'zenaura.server']),
     package_dir={'': 'src'},
     install_requires=[
         'bleach'
```

### Comparing `zenaura-0.9.65/src/zenaura/client/app.py` & `zenaura-0.9.66/src/zenaura/client/app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/src/zenaura/client/component.py` & `zenaura-0.9.66/src/zenaura/client/component.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/src/zenaura/client/config.py` & `zenaura-0.9.66/src/zenaura/client/config.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/src/zenaura/client/mocks.py` & `zenaura-0.9.66/src/zenaura/client/mocks.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/src/zenaura/client/mutator.py` & `zenaura-0.9.66/src/zenaura/client/mutator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/src/zenaura/client/observer.py` & `zenaura-0.9.66/src/zenaura/client/observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/src/zenaura/client/page.py` & `zenaura-0.9.66/src/zenaura/client/page.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/src/zenaura/client/persistance.py` & `zenaura-0.9.66/src/zenaura/client/persistance.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/src/zenaura/server/server.py` & `zenaura-0.9.66/src/zenaura/server/server.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/src/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.66/src/zenaura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.65
+Version: 0.9.66
 Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.65/src/zenaura.egg-info/SOURCES.txt` & `zenaura-0.9.66/src/zenaura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_algorithm.py` & `zenaura-0.9.66/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_app.py` & `zenaura-0.9.66/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_compiler.py` & `zenaura-0.9.66/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_component_e2e.py` & `zenaura-0.9.66/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_component_unit.py` & `zenaura-0.9.66/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_node_properties.py` & `zenaura-0.9.66/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_observer.py` & `zenaura-0.9.66/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_rdom_adapter.py` & `zenaura-0.9.66/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_tags.py` & `zenaura-0.9.66/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_tasker.py` & `zenaura-0.9.66/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.65/tests/test_zenaura_dom.py` & `zenaura-0.9.66/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

