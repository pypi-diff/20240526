# Comparing `tmp/zenaura-0.9.84.tar.gz` & `tmp/zenaura-0.9.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.84.tar", last modified: Sun May 26 20:12:15 2024, max compression
+gzip compressed data, was "zenaura-0.9.85.tar", last modified: Sun May 26 20:27:54 2024, max compression
```

## Comparing `zenaura-0.9.84.tar` & `zenaura-0.9.85.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.306970 zenaura-0.9.84/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.84/LICENSE
--rw-rw-rw-   0        0        0     2028 2024-05-26 20:12:15.306469 zenaura-0.9.84/PKG-INFO
--rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.84/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 20:12:15.307469 zenaura-0.9.84/setup.cfg
--rw-rw-rw-   0        0        0     1153 2024-05-26 20:11:47.000000 zenaura-0.9.84/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.262919 zenaura-0.9.84/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6591 2024-05-26 18:57:08.000000 zenaura-0.9.84/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.84/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.263922 zenaura-0.9.84/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.84/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.279442 zenaura-0.9.84/zenaura/client/
--rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.84/zenaura/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.282442 zenaura-0.9.84/zenaura/client/algorithm/
--rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/algorithm/__init__.py
--rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/algorithm/algorithm.py
--rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/algorithm/operations.py
--rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/algorithm/searcher.py
--rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/algorithm/updater.py
--rw-rw-rw-   0        0        0     8990 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/app.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.283945 zenaura-0.9.84/zenaura/client/compiler/
--rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/compiler/__init__.py
--rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/compiler/attribute.py
--rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/compiler/compiler.py
--rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/compiler/sanitize.py
--rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/config.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.294457 zenaura-0.9.84/zenaura/client/dom/
--rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/dom/__init__.py
--rw-rw-rw-   0        0        0      280 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/dom/dom.py
--rw-rw-rw-   0        0        0     1803 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/dom/error.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.295458 zenaura-0.9.84/zenaura/client/dom/lifecycles/
--rw-rw-rw-   0        0        0      437 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/dom/lifecycles/mount.py
--rw-rw-rw-   0        0        0      780 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/dom/lifecycles/render.py
--rw-rw-rw-   0        0        0     1850 2024-05-26 20:11:20.000000 zenaura-0.9.84/zenaura/client/dom/mount.py
--rw-rw-rw-   0        0        0     1883 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/dom/render.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.299456 zenaura-0.9.84/zenaura/client/hydrator/
--rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/hydrator/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/hydrator/compiler_adapter.py
--rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/hydrator/hydrator.py
--rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/hydrator/lookup.py
--rw-rw-rw-   0        0        0     6943 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/hydrator/real_dom_adapter.py
--rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/hydrator/tasker.py
--rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/hydrator/virtual_dom_adapter.py
--rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.84/zenaura/client/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.300956 zenaura-0.9.84/zenaura/client/observer/
--rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/observer/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/observer/observer.py
--rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/observer/subject.py
--rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/observer.py
--rw-rw-rw-   0        0        0      943 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/page.py
--rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.303961 zenaura-0.9.84/zenaura/client/tags/
--rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/tags/__init__.py
--rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/tags/attribute.py
--rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/tags/builder.py
--rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/tags/data.py
--rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/tags/html.py
--rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.84/zenaura/client/tags/node.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.305465 zenaura-0.9.84/zenaura/server/
--rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.84/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0     1173 2024-05-26 19:24:34.000000 zenaura-0.9.84/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:12:15.305970 zenaura-0.9.84/zenaura.egg-info/
--rw-rw-rw-   0        0        0     2028 2024-05-26 20:12:15.000000 zenaura-0.9.84/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1867 2024-05-26 20:12:15.000000 zenaura-0.9.84/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 20:12:15.000000 zenaura-0.9.84/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 20:12:15.000000 zenaura-0.9.84/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 20:12:15.000000 zenaura-0.9.84/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.110753 zenaura-0.9.85/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.85/LICENSE
+-rw-rw-rw-   0        0        0     2028 2024-05-26 20:27:54.110256 zenaura-0.9.85/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.85/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 20:27:54.110753 zenaura-0.9.85/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2024-05-26 20:27:46.000000 zenaura-0.9.85/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.070696 zenaura-0.9.85/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6591 2024-05-26 18:57:08.000000 zenaura-0.9.85/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.85/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.070696 zenaura-0.9.85/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-26 19:08:09.000000 zenaura-0.9.85/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.083720 zenaura-0.9.85/zenaura/client/
+-rw-rw-rw-   0        0        0        0 2024-05-26 18:57:31.000000 zenaura-0.9.85/zenaura/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.087221 zenaura-0.9.85/zenaura/client/algorithm/
+-rw-rw-rw-   0        0        0       39 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/algorithm/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/algorithm/algorithm.py
+-rw-rw-rw-   0        0        0      972 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/algorithm/operations.py
+-rw-rw-rw-   0        0        0     7166 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/algorithm/searcher.py
+-rw-rw-rw-   0        0        0     2772 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/algorithm/updater.py
+-rw-rw-rw-   0        0        0     8990 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/app.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.089220 zenaura-0.9.85/zenaura/client/compiler/
+-rw-rw-rw-   0        0        0       53 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/compiler/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/compiler/attribute.py
+-rw-rw-rw-   0        0        0     3471 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/compiler/compiler.py
+-rw-rw-rw-   0        0        0     1132 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/compiler/sanitize.py
+-rw-rw-rw-   0        0        0     4093 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/config.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.098228 zenaura-0.9.85/zenaura/client/dom/
+-rw-rw-rw-   0        0        0       43 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/dom/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/dom/dom.py
+-rw-rw-rw-   0        0        0     1803 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/dom/error.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.098728 zenaura-0.9.85/zenaura/client/dom/lifecycles/
+-rw-rw-rw-   0        0        0      437 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/dom/lifecycles/mount.py
+-rw-rw-rw-   0        0        0      780 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/dom/lifecycles/render.py
+-rw-rw-rw-   0        0        0     1852 2024-05-26 20:26:11.000000 zenaura-0.9.85/zenaura/client/dom/mount.py
+-rw-rw-rw-   0        0        0     1883 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/dom/render.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.102238 zenaura-0.9.85/zenaura/client/hydrator/
+-rw-rw-rw-   0        0        0      235 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/hydrator/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/hydrator/compiler_adapter.py
+-rw-rw-rw-   0        0        0     1236 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/hydrator/hydrator.py
+-rw-rw-rw-   0        0        0     1346 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/hydrator/lookup.py
+-rw-rw-rw-   0        0        0     6943 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/hydrator/real_dom_adapter.py
+-rw-rw-rw-   0        0        0     2264 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/hydrator/tasker.py
+-rw-rw-rw-   0        0        0     1064 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/hydrator/virtual_dom_adapter.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      896 2024-05-26 18:57:08.000000 zenaura-0.9.85/zenaura/client/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.104246 zenaura-0.9.85/zenaura/client/observer/
+-rw-rw-rw-   0        0        0       60 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/observer/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/observer/observer.py
+-rw-rw-rw-   0        0        0     1609 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/observer/subject.py
+-rw-rw-rw-   0        0        0     2009 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      943 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.107237 zenaura-0.9.85/zenaura/client/tags/
+-rw-rw-rw-   0        0        0      165 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/tags/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/tags/attribute.py
+-rw-rw-rw-   0        0        0     4666 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/tags/builder.py
+-rw-rw-rw-   0        0        0      418 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/tags/data.py
+-rw-rw-rw-   0        0        0      473 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/tags/html.py
+-rw-rw-rw-   0        0        0    10231 2024-05-26 17:44:57.000000 zenaura-0.9.85/zenaura/client/tags/node.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.108739 zenaura-0.9.85/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 19:08:17.000000 zenaura-0.9.85/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     1173 2024-05-26 19:24:34.000000 zenaura-0.9.85/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:27:54.108739 zenaura-0.9.85/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     2028 2024-05-26 20:27:54.000000 zenaura-0.9.85/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1867 2024-05-26 20:27:54.000000 zenaura-0.9.85/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 20:27:54.000000 zenaura-0.9.85/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 20:27:54.000000 zenaura-0.9.85/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 20:27:54.000000 zenaura-0.9.85/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.84/LICENSE` & `zenaura-0.9.85/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/PKG-INFO` & `zenaura-0.9.85/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.84
+Version: 0.9.85
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.84/README.md` & `zenaura-0.9.85/README.md`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/setup.py` & `zenaura-0.9.85/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='zenaura',
-    version='0.9.84',
+    version='0.9.85',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
     packages=['zenaura', 'zenaura.server', 'zenaura.client', 'zenaura.client.algorithm', 'zenaura.client.compiler', 'zenaura.client.hydrator', 'zenaura.client.observer', 'zenaura.client.tags', 'zenaura.client.dom', 'zenaura.client.dom.lifecycles'],
     install_requires=[
         'bleach'
     ],
```

### Comparing `zenaura-0.9.84/tests/test_algorithm.py` & `zenaura-0.9.85/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_app.py` & `zenaura-0.9.85/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_compiler.py` & `zenaura-0.9.85/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_component_e2e.py` & `zenaura-0.9.85/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_component_unit.py` & `zenaura-0.9.85/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_node_properties.py` & `zenaura-0.9.85/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_observer.py` & `zenaura-0.9.85/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_rdom_adapter.py` & `zenaura-0.9.85/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_tags.py` & `zenaura-0.9.85/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_tasker.py` & `zenaura-0.9.85/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/tests/test_zenaura_dom.py` & `zenaura-0.9.85/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/algorithm/operations.py` & `zenaura-0.9.85/zenaura/client/algorithm/operations.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/algorithm/searcher.py` & `zenaura-0.9.85/zenaura/client/algorithm/searcher.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/algorithm/updater.py` & `zenaura-0.9.85/zenaura/client/algorithm/updater.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/app.py` & `zenaura-0.9.85/zenaura/client/app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/compiler/attribute.py` & `zenaura-0.9.85/zenaura/client/compiler/attribute.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/compiler/compiler.py` & `zenaura-0.9.85/zenaura/client/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/compiler/sanitize.py` & `zenaura-0.9.85/zenaura/client/compiler/sanitize.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/component.py` & `zenaura-0.9.85/zenaura/client/component.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/config.py` & `zenaura-0.9.85/zenaura/client/config.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/dom/error.py` & `zenaura-0.9.85/zenaura/client/dom/error.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/dom/lifecycles/render.py` & `zenaura-0.9.85/zenaura/client/dom/lifecycles/render.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/dom/mount.py` & `zenaura-0.9.85/zenaura/client/dom/mount.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,24 +29,25 @@
             - comp: An instance of the Component class.
 
             Returns:
             None
         """
 
         try :
-            
-            # clean up perviously mounted components :
-            self.zen_dom_table.clear()
+            compiled_html = self.hyd_comp_compile_page(page)
 
             # wait for DOMContent to be loaded 
             await rdom_hyd.hyd_rdom_wait_for_dom_content_loaded()
-            compiled_html = self.hyd_comp_compile_page(page)
 
             self.hyd_rdom_attach_to_root(compiled_html)
             # trigger attached for page components
+            
+            # clean up perviously mounted components :
+            self.zen_dom_table.clear()
+
             for comp in page.children:
                 # trigger attached for page components
                 self.attached(comp)
                 # update state in vdom
                 self.hyd_vdom_update(comp)
 
         except Exception as e:
```

### Comparing `zenaura-0.9.84/zenaura/client/dom/render.py` & `zenaura-0.9.85/zenaura/client/dom/render.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/hydrator/compiler_adapter.py` & `zenaura-0.9.85/zenaura/client/hydrator/compiler_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/hydrator/hydrator.py` & `zenaura-0.9.85/zenaura/client/hydrator/hydrator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/hydrator/lookup.py` & `zenaura-0.9.85/zenaura/client/hydrator/lookup.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/hydrator/real_dom_adapter.py` & `zenaura-0.9.85/zenaura/client/hydrator/real_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/hydrator/tasker.py` & `zenaura-0.9.85/zenaura/client/hydrator/tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/hydrator/virtual_dom_adapter.py` & `zenaura-0.9.85/zenaura/client/hydrator/virtual_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/mocks.py` & `zenaura-0.9.85/zenaura/client/mocks.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/mutator.py` & `zenaura-0.9.85/zenaura/client/mutator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/observer/subject.py` & `zenaura-0.9.85/zenaura/client/observer/subject.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/observer.py` & `zenaura-0.9.85/zenaura/client/observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/page.py` & `zenaura-0.9.85/zenaura/client/page.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/persistance.py` & `zenaura-0.9.85/zenaura/client/persistance.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/tags/builder.py` & `zenaura-0.9.85/zenaura/client/tags/builder.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/client/tags/node.py` & `zenaura-0.9.85/zenaura/client/tags/node.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura/server/server.py` & `zenaura-0.9.85/zenaura/server/server.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.84/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.85/zenaura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.84
+Version: 0.9.85
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.84/zenaura.egg-info/SOURCES.txt` & `zenaura-0.9.85/zenaura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

