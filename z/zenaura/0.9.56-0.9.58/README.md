# Comparing `tmp/zenaura-0.9.56.tar.gz` & `tmp/zenaura-0.9.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.56.tar", last modified: Sun May 26 16:15:00 2024, max compression
+gzip compressed data, was "zenaura-0.9.58.tar", last modified: Sun May 26 16:41:24 2024, max compression
```

## Comparing `zenaura-0.9.56.tar` & `zenaura-0.9.58.tar`

### file list

```diff
@@ -1,26 +1,73 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 16:15:00.824068 zenaura-0.9.56/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.56/LICENSE
--rw-rw-rw-   0        0        0     1804 2024-05-26 16:15:00.823568 zenaura-0.9.56/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-18 13:42:46.000000 zenaura-0.9.56/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 16:15:00.824068 zenaura-0.9.56/setup.cfg
--rw-rw-rw-   0        0        0      690 2024-05-26 16:14:56.000000 zenaura-0.9.56/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:15:00.815065 zenaura-0.9.56/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 13:51:25.000000 zenaura-0.9.56/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6591 2024-05-26 14:35:19.000000 zenaura-0.9.56/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 14:03:42.000000 zenaura-0.9.56/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 14:03:42.000000 zenaura-0.9.56/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 13:51:25.000000 zenaura-0.9.56/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 14:03:42.000000 zenaura-0.9.56/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.56/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 14:03:42.000000 zenaura-0.9.56/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 13:56:00.000000 zenaura-0.9.56/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-18 19:29:37.000000 zenaura-0.9.56/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 14:03:42.000000 zenaura-0.9.56/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:15:00.816065 zenaura-0.9.56/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-26 16:09:11.000000 zenaura-0.9.56/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:15:00.823069 zenaura-0.9.56/zenaura.egg-info/
--rw-rw-rw-   0        0        0     1804 2024-05-26 16:15:00.000000 zenaura-0.9.56/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-05-26 16:15:00.000000 zenaura-0.9.56/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 16:15:00.000000 zenaura-0.9.56/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 16:15:00.000000 zenaura-0.9.56/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 16:15:00.000000 zenaura-0.9.56/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.273795 zenaura-0.9.58/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.58/LICENSE
+-rw-rw-rw-   0        0        0      607 2024-05-26 16:41:24.273295 zenaura-0.9.58/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 16:41:24.273795 zenaura-0.9.58/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-05-26 16:41:20.000000 zenaura-0.9.58/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.242796 zenaura-0.9.58/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6591 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.235296 zenaura-0.9.58/zenaura/
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.247296 zenaura-0.9.58/zenaura/client/
+-rw-rw-rw-   0        0        0      213 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.249795 zenaura-0.9.58/zenaura/client/algorithm/
+-rw-rw-rw-   0        0        0       39 2024-05-17 10:24:48.000000 zenaura-0.9.58/zenaura/client/algorithm/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-05-18 14:45:35.000000 zenaura-0.9.58/zenaura/client/algorithm/algorithm.py
+-rw-rw-rw-   0        0        0      972 2024-05-18 10:35:50.000000 zenaura-0.9.58/zenaura/client/algorithm/operations.py
+-rw-rw-rw-   0        0        0     7166 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/algorithm/searcher.py
+-rw-rw-rw-   0        0        0     2772 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/algorithm/updater.py
+-rw-rw-rw-   0        0        0     8990 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/app.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.251794 zenaura-0.9.58/zenaura/client/compiler/
+-rw-rw-rw-   0        0        0       53 2024-05-18 10:37:12.000000 zenaura-0.9.58/zenaura/client/compiler/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/compiler/attribute.py
+-rw-rw-rw-   0        0        0     3471 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/compiler/compiler.py
+-rw-rw-rw-   0        0        0     1132 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/compiler/sanitize.py
+-rw-rw-rw-   0        0        0     4093 2024-05-26 14:03:42.000000 zenaura-0.9.58/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/config.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.254296 zenaura-0.9.58/zenaura/client/dom/
+-rw-rw-rw-   0        0        0       43 2024-05-13 18:21:23.000000 zenaura-0.9.58/zenaura/client/dom/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-05-15 10:34:41.000000 zenaura-0.9.58/zenaura/client/dom/dom.py
+-rw-rw-rw-   0        0        0     1803 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/dom/error.py
+-rw-rw-rw-   0        0        0     1852 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/dom/mount.py
+-rw-rw-rw-   0        0        0     1883 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/dom/render.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.257795 zenaura-0.9.58/zenaura/client/hydrator/
+-rw-rw-rw-   0        0        0      235 2024-05-18 13:11:09.000000 zenaura-0.9.58/zenaura/client/hydrator/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/hydrator/compiler_adapter.py
+-rw-rw-rw-   0        0        0     1236 2024-05-18 14:37:59.000000 zenaura-0.9.58/zenaura/client/hydrator/hydrator.py
+-rw-rw-rw-   0        0        0     1346 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/hydrator/lookup.py
+-rw-rw-rw-   0        0        0     6943 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/hydrator/real_dom_adapter.py
+-rw-rw-rw-   0        0        0     2264 2024-05-18 16:48:34.000000 zenaura-0.9.58/zenaura/client/hydrator/tasker.py
+-rw-rw-rw-   0        0        0     1064 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/hydrator/virtual_dom_adapter.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      896 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.259796 zenaura-0.9.58/zenaura/client/observer/
+-rw-rw-rw-   0        0        0       60 2024-05-13 18:21:23.000000 zenaura-0.9.58/zenaura/client/observer/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-13 18:21:23.000000 zenaura-0.9.58/zenaura/client/observer/observer.py
+-rw-rw-rw-   0        0        0     1609 2024-05-13 18:21:23.000000 zenaura-0.9.58/zenaura/client/observer/subject.py
+-rw-rw-rw-   0        0        0     2009 2024-05-13 18:06:17.000000 zenaura-0.9.58/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      943 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.262295 zenaura-0.9.58/zenaura/client/tags/
+-rw-rw-rw-   0        0        0      165 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/tags/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-14 08:37:50.000000 zenaura-0.9.58/zenaura/client/tags/attribute.py
+-rw-rw-rw-   0        0        0     4666 2024-05-26 13:54:24.000000 zenaura-0.9.58/zenaura/client/tags/builder.py
+-rw-rw-rw-   0        0        0      418 2024-05-14 06:45:47.000000 zenaura-0.9.58/zenaura/client/tags/data.py
+-rw-rw-rw-   0        0        0      473 2024-05-14 18:17:26.000000 zenaura-0.9.58/zenaura/client/tags/html.py
+-rw-rw-rw-   0        0        0    10231 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/tags/node.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.263296 zenaura-0.9.58/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     1237 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.272796 zenaura-0.9.58/zenaura/zenaura.egg-info/
+-rw-rw-rw-   0        0        0      607 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1798 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.56/LICENSE` & `zenaura-0.9.58/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_algorithm.py` & `zenaura-0.9.58/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_app.py` & `zenaura-0.9.58/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_compiler.py` & `zenaura-0.9.58/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_component_e2e.py` & `zenaura-0.9.58/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_component_unit.py` & `zenaura-0.9.58/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_node_properties.py` & `zenaura-0.9.58/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_observer.py` & `zenaura-0.9.58/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_rdom_adapter.py` & `zenaura-0.9.58/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_tags.py` & `zenaura-0.9.58/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_tasker.py` & `zenaura-0.9.58/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.56/tests/test_zenaura_dom.py` & `zenaura-0.9.58/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

