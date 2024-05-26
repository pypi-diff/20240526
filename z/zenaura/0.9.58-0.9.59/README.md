# Comparing `tmp/zenaura-0.9.58.tar.gz` & `tmp/zenaura-0.9.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.58.tar", last modified: Sun May 26 16:41:24 2024, max compression
+gzip compressed data, was "zenaura-0.9.59.tar", last modified: Sun May 26 16:45:01 2024, max compression
```

## Comparing `zenaura-0.9.58.tar` & `zenaura-0.9.59.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.273795 zenaura-0.9.58/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.58/LICENSE
--rw-rw-rw-   0        0        0      607 2024-05-26 16:41:24.273295 zenaura-0.9.58/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 16:41:24.273795 zenaura-0.9.58/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-05-26 16:41:20.000000 zenaura-0.9.58/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.242796 zenaura-0.9.58/tests/
--rw-rw-rw-   0        0        0    33440 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_algorithm.py
--rw-rw-rw-   0        0        0     6591 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_app.py
--rw-rw-rw-   0        0        0     7595 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4161 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1415 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     5301 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_node_properties.py
--rw-rw-rw-   0        0        0     1435 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_observer.py
--rw-rw-rw-   0        0        0     5710 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_rdom_adapter.py
--rw-rw-rw-   0        0        0    15215 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_tags.py
--rw-rw-rw-   0        0        0     3293 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_tasker.py
--rw-rw-rw-   0        0        0     5456 2024-05-26 16:36:07.000000 zenaura-0.9.58/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.235296 zenaura-0.9.58/zenaura/
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.247296 zenaura-0.9.58/zenaura/client/
--rw-rw-rw-   0        0        0      213 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.249795 zenaura-0.9.58/zenaura/client/algorithm/
--rw-rw-rw-   0        0        0       39 2024-05-17 10:24:48.000000 zenaura-0.9.58/zenaura/client/algorithm/__init__.py
--rw-rw-rw-   0        0        0      193 2024-05-18 14:45:35.000000 zenaura-0.9.58/zenaura/client/algorithm/algorithm.py
--rw-rw-rw-   0        0        0      972 2024-05-18 10:35:50.000000 zenaura-0.9.58/zenaura/client/algorithm/operations.py
--rw-rw-rw-   0        0        0     7166 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/algorithm/searcher.py
--rw-rw-rw-   0        0        0     2772 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/algorithm/updater.py
--rw-rw-rw-   0        0        0     8990 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/app.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.251794 zenaura-0.9.58/zenaura/client/compiler/
--rw-rw-rw-   0        0        0       53 2024-05-18 10:37:12.000000 zenaura-0.9.58/zenaura/client/compiler/__init__.py
--rw-rw-rw-   0        0        0     1403 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/compiler/attribute.py
--rw-rw-rw-   0        0        0     3471 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/compiler/compiler.py
--rw-rw-rw-   0        0        0     1132 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/compiler/sanitize.py
--rw-rw-rw-   0        0        0     4093 2024-05-26 14:03:42.000000 zenaura-0.9.58/zenaura/client/component.py
--rw-rw-rw-   0        0        0      744 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/config.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.254296 zenaura-0.9.58/zenaura/client/dom/
--rw-rw-rw-   0        0        0       43 2024-05-13 18:21:23.000000 zenaura-0.9.58/zenaura/client/dom/__init__.py
--rw-rw-rw-   0        0        0      280 2024-05-15 10:34:41.000000 zenaura-0.9.58/zenaura/client/dom/dom.py
--rw-rw-rw-   0        0        0     1803 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/dom/error.py
--rw-rw-rw-   0        0        0     1852 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/dom/mount.py
--rw-rw-rw-   0        0        0     1883 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/dom/render.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.257795 zenaura-0.9.58/zenaura/client/hydrator/
--rw-rw-rw-   0        0        0      235 2024-05-18 13:11:09.000000 zenaura-0.9.58/zenaura/client/hydrator/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/hydrator/compiler_adapter.py
--rw-rw-rw-   0        0        0     1236 2024-05-18 14:37:59.000000 zenaura-0.9.58/zenaura/client/hydrator/hydrator.py
--rw-rw-rw-   0        0        0     1346 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/hydrator/lookup.py
--rw-rw-rw-   0        0        0     6943 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/hydrator/real_dom_adapter.py
--rw-rw-rw-   0        0        0     2264 2024-05-18 16:48:34.000000 zenaura-0.9.58/zenaura/client/hydrator/tasker.py
--rw-rw-rw-   0        0        0     1064 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/hydrator/virtual_dom_adapter.py
--rw-rw-rw-   0        0        0     2631 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/mocks.py
--rw-rw-rw-   0        0        0      896 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/mutator.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.259796 zenaura-0.9.58/zenaura/client/observer/
--rw-rw-rw-   0        0        0       60 2024-05-13 18:21:23.000000 zenaura-0.9.58/zenaura/client/observer/__init__.py
--rw-rw-rw-   0        0        0      396 2024-05-13 18:21:23.000000 zenaura-0.9.58/zenaura/client/observer/observer.py
--rw-rw-rw-   0        0        0     1609 2024-05-13 18:21:23.000000 zenaura-0.9.58/zenaura/client/observer/subject.py
--rw-rw-rw-   0        0        0     2009 2024-05-13 18:06:17.000000 zenaura-0.9.58/zenaura/client/observer.py
--rw-rw-rw-   0        0        0      943 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/page.py
--rw-rw-rw-   0        0        0     2212 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/persistance.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.262295 zenaura-0.9.58/zenaura/client/tags/
--rw-rw-rw-   0        0        0      165 2024-05-26 13:51:25.000000 zenaura-0.9.58/zenaura/client/tags/__init__.py
--rw-rw-rw-   0        0        0      429 2024-05-14 08:37:50.000000 zenaura-0.9.58/zenaura/client/tags/attribute.py
--rw-rw-rw-   0        0        0     4666 2024-05-26 13:54:24.000000 zenaura-0.9.58/zenaura/client/tags/builder.py
--rw-rw-rw-   0        0        0      418 2024-05-14 06:45:47.000000 zenaura-0.9.58/zenaura/client/tags/data.py
--rw-rw-rw-   0        0        0      473 2024-05-14 18:17:26.000000 zenaura-0.9.58/zenaura/client/tags/html.py
--rw-rw-rw-   0        0        0    10231 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/client/tags/node.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.263296 zenaura-0.9.58/zenaura/server/
--rw-rw-rw-   0        0        0       33 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/server/__init__.py
--rw-rw-rw-   0        0        0     1237 2024-05-26 16:36:07.000000 zenaura-0.9.58/zenaura/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:41:24.272796 zenaura-0.9.58/zenaura/zenaura.egg-info/
--rw-rw-rw-   0        0        0      607 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1798 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-26 16:41:24.000000 zenaura-0.9.58/zenaura/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.324932 zenaura-0.9.59/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.59/LICENSE
+-rw-rw-rw-   0        0        0      607 2024-05-26 16:45:01.324432 zenaura-0.9.59/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 16:45:01.324932 zenaura-0.9.59/setup.cfg
+-rw-rw-rw-   0        0        0      776 2024-05-26 16:44:49.000000 zenaura-0.9.59/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.285427 zenaura-0.9.59/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.288928 zenaura-0.9.59/src/zenaura/
+-rw-rw-rw-   0        0        0        0 2024-05-26 16:44:15.000000 zenaura-0.9.59/src/zenaura/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.301932 zenaura-0.9.59/src/zenaura/client/
+-rw-rw-rw-   0        0        0      213 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.304432 zenaura-0.9.59/src/zenaura/client/algorithm/
+-rw-rw-rw-   0        0        0       39 2024-05-17 10:24:48.000000 zenaura-0.9.59/src/zenaura/client/algorithm/__init__.py
+-rw-rw-rw-   0        0        0      193 2024-05-18 14:45:35.000000 zenaura-0.9.59/src/zenaura/client/algorithm/algorithm.py
+-rw-rw-rw-   0        0        0      972 2024-05-18 10:35:50.000000 zenaura-0.9.59/src/zenaura/client/algorithm/operations.py
+-rw-rw-rw-   0        0        0     7166 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/algorithm/searcher.py
+-rw-rw-rw-   0        0        0     2772 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/algorithm/updater.py
+-rw-rw-rw-   0        0        0     8990 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/app.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.306432 zenaura-0.9.59/src/zenaura/client/compiler/
+-rw-rw-rw-   0        0        0       53 2024-05-18 10:37:12.000000 zenaura-0.9.59/src/zenaura/client/compiler/__init__.py
+-rw-rw-rw-   0        0        0     1403 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/compiler/attribute.py
+-rw-rw-rw-   0        0        0     3471 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/compiler/compiler.py
+-rw-rw-rw-   0        0        0     1132 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/compiler/sanitize.py
+-rw-rw-rw-   0        0        0     4093 2024-05-26 14:03:42.000000 zenaura-0.9.59/src/zenaura/client/component.py
+-rw-rw-rw-   0        0        0      744 2024-05-26 13:51:25.000000 zenaura-0.9.59/src/zenaura/client/config.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.308932 zenaura-0.9.59/src/zenaura/client/dom/
+-rw-rw-rw-   0        0        0       43 2024-05-13 18:21:23.000000 zenaura-0.9.59/src/zenaura/client/dom/__init__.py
+-rw-rw-rw-   0        0        0      280 2024-05-15 10:34:41.000000 zenaura-0.9.59/src/zenaura/client/dom/dom.py
+-rw-rw-rw-   0        0        0     1803 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/dom/error.py
+-rw-rw-rw-   0        0        0     1852 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/dom/mount.py
+-rw-rw-rw-   0        0        0     1883 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/dom/render.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.312432 zenaura-0.9.59/src/zenaura/client/hydrator/
+-rw-rw-rw-   0        0        0      235 2024-05-18 13:11:09.000000 zenaura-0.9.59/src/zenaura/client/hydrator/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/hydrator/compiler_adapter.py
+-rw-rw-rw-   0        0        0     1236 2024-05-18 14:37:59.000000 zenaura-0.9.59/src/zenaura/client/hydrator/hydrator.py
+-rw-rw-rw-   0        0        0     1346 2024-05-26 13:51:25.000000 zenaura-0.9.59/src/zenaura/client/hydrator/lookup.py
+-rw-rw-rw-   0        0        0     6943 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/hydrator/real_dom_adapter.py
+-rw-rw-rw-   0        0        0     2264 2024-05-18 16:48:34.000000 zenaura-0.9.59/src/zenaura/client/hydrator/tasker.py
+-rw-rw-rw-   0        0        0     1064 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/hydrator/virtual_dom_adapter.py
+-rw-rw-rw-   0        0        0     2631 2024-05-26 13:51:25.000000 zenaura-0.9.59/src/zenaura/client/mocks.py
+-rw-rw-rw-   0        0        0      896 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/mutator.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.313933 zenaura-0.9.59/src/zenaura/client/observer/
+-rw-rw-rw-   0        0        0       60 2024-05-13 18:21:23.000000 zenaura-0.9.59/src/zenaura/client/observer/__init__.py
+-rw-rw-rw-   0        0        0      396 2024-05-13 18:21:23.000000 zenaura-0.9.59/src/zenaura/client/observer/observer.py
+-rw-rw-rw-   0        0        0     1609 2024-05-13 18:21:23.000000 zenaura-0.9.59/src/zenaura/client/observer/subject.py
+-rw-rw-rw-   0        0        0     2009 2024-05-13 18:06:17.000000 zenaura-0.9.59/src/zenaura/client/observer.py
+-rw-rw-rw-   0        0        0      943 2024-05-26 13:51:25.000000 zenaura-0.9.59/src/zenaura/client/page.py
+-rw-rw-rw-   0        0        0     2212 2024-05-26 13:51:25.000000 zenaura-0.9.59/src/zenaura/client/persistance.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.316432 zenaura-0.9.59/src/zenaura/client/tags/
+-rw-rw-rw-   0        0        0      165 2024-05-26 13:51:25.000000 zenaura-0.9.59/src/zenaura/client/tags/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-14 08:37:50.000000 zenaura-0.9.59/src/zenaura/client/tags/attribute.py
+-rw-rw-rw-   0        0        0     4666 2024-05-26 13:54:24.000000 zenaura-0.9.59/src/zenaura/client/tags/builder.py
+-rw-rw-rw-   0        0        0      418 2024-05-14 06:45:47.000000 zenaura-0.9.59/src/zenaura/client/tags/data.py
+-rw-rw-rw-   0        0        0      473 2024-05-14 18:17:26.000000 zenaura-0.9.59/src/zenaura/client/tags/html.py
+-rw-rw-rw-   0        0        0    10231 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/client/tags/node.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.317933 zenaura-0.9.59/src/zenaura/server/
+-rw-rw-rw-   0        0        0       33 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/server/__init__.py
+-rw-rw-rw-   0        0        0     1237 2024-05-26 16:36:07.000000 zenaura-0.9.59/src/zenaura/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.323433 zenaura-0.9.59/src/zenaura.egg-info/
+-rw-rw-rw-   0        0        0      607 2024-05-26 16:45:01.000000 zenaura-0.9.59/src/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1966 2024-05-26 16:45:01.000000 zenaura-0.9.59/src/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 16:45:01.000000 zenaura-0.9.59/src/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 16:45:01.000000 zenaura-0.9.59/src/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 16:45:01.000000 zenaura-0.9.59/src/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 16:45:01.322932 zenaura-0.9.59/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6591 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 16:36:07.000000 zenaura-0.9.59/tests/test_zenaura_dom.py
```

### Comparing `zenaura-0.9.58/LICENSE` & `zenaura-0.9.59/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/PKG-INFO` & `zenaura-0.9.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.58
+Version: 0.9.59
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.58/setup.py` & `zenaura-0.9.59/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 setup(
     name='zenaura',
-    version='0.9.58',
+    version='0.9.59',
     description="Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.",
     author="Ahmed Rakan",
     author_email="ar.aldhafeeri11@gmail.com",
-     package_dir={"": "zenaura"},
-    packages=find_packages(where='zenaura'),
+     package_dir={"": "src"},
+    packages=find_packages(where='src'),
     install_requires=[
         'bleach'
     ],
     test_suite='tests',
 )
```

### Comparing `zenaura-0.9.58/tests/test_algorithm.py` & `zenaura-0.9.59/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_app.py` & `zenaura-0.9.59/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_compiler.py` & `zenaura-0.9.59/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_component_e2e.py` & `zenaura-0.9.59/tests/test_component_e2e.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_component_unit.py` & `zenaura-0.9.59/tests/test_component_unit.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_node_properties.py` & `zenaura-0.9.59/tests/test_node_properties.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_observer.py` & `zenaura-0.9.59/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_rdom_adapter.py` & `zenaura-0.9.59/tests/test_rdom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_tags.py` & `zenaura-0.9.59/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_tasker.py` & `zenaura-0.9.59/tests/test_tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/tests/test_zenaura_dom.py` & `zenaura-0.9.59/tests/test_zenaura_dom.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/algorithm/operations.py` & `zenaura-0.9.59/src/zenaura/client/algorithm/operations.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/algorithm/searcher.py` & `zenaura-0.9.59/src/zenaura/client/algorithm/searcher.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/algorithm/updater.py` & `zenaura-0.9.59/src/zenaura/client/algorithm/updater.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/app.py` & `zenaura-0.9.59/src/zenaura/client/app.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/compiler/attribute.py` & `zenaura-0.9.59/src/zenaura/client/compiler/attribute.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/compiler/compiler.py` & `zenaura-0.9.59/src/zenaura/client/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/compiler/sanitize.py` & `zenaura-0.9.59/src/zenaura/client/compiler/sanitize.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/component.py` & `zenaura-0.9.59/src/zenaura/client/component.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/config.py` & `zenaura-0.9.59/src/zenaura/client/config.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/dom/error.py` & `zenaura-0.9.59/src/zenaura/client/dom/error.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/dom/mount.py` & `zenaura-0.9.59/src/zenaura/client/dom/mount.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/dom/render.py` & `zenaura-0.9.59/src/zenaura/client/dom/render.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/hydrator/compiler_adapter.py` & `zenaura-0.9.59/src/zenaura/client/hydrator/compiler_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/hydrator/hydrator.py` & `zenaura-0.9.59/src/zenaura/client/hydrator/hydrator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/hydrator/lookup.py` & `zenaura-0.9.59/src/zenaura/client/hydrator/lookup.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/hydrator/real_dom_adapter.py` & `zenaura-0.9.59/src/zenaura/client/hydrator/real_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/hydrator/tasker.py` & `zenaura-0.9.59/src/zenaura/client/hydrator/tasker.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/hydrator/virtual_dom_adapter.py` & `zenaura-0.9.59/src/zenaura/client/hydrator/virtual_dom_adapter.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/mocks.py` & `zenaura-0.9.59/src/zenaura/client/mocks.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/mutator.py` & `zenaura-0.9.59/src/zenaura/client/mutator.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/observer/subject.py` & `zenaura-0.9.59/src/zenaura/client/observer/subject.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/observer.py` & `zenaura-0.9.59/src/zenaura/client/observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/page.py` & `zenaura-0.9.59/src/zenaura/client/page.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/persistance.py` & `zenaura-0.9.59/src/zenaura/client/persistance.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/tags/builder.py` & `zenaura-0.9.59/src/zenaura/client/tags/builder.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/client/tags/node.py` & `zenaura-0.9.59/src/zenaura/client/tags/node.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/server/server.py` & `zenaura-0.9.59/src/zenaura/server/server.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.58/zenaura/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.59/src/zenaura.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.58
+Version: 0.9.59
 Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 License-File: LICENSE
 Requires-Dist: bleach
```

### Comparing `zenaura-0.9.58/zenaura/zenaura.egg-info/SOURCES.txt` & `zenaura-0.9.59/src/zenaura.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 LICENSE
 setup.py
+src/zenaura/__init__.py
+src/zenaura.egg-info/PKG-INFO
+src/zenaura.egg-info/SOURCES.txt
+src/zenaura.egg-info/dependency_links.txt
+src/zenaura.egg-info/requires.txt
+src/zenaura.egg-info/top_level.txt
+src/zenaura/client/__init__.py
+src/zenaura/client/app.py
+src/zenaura/client/component.py
+src/zenaura/client/config.py
+src/zenaura/client/mocks.py
+src/zenaura/client/mutator.py
+src/zenaura/client/observer.py
+src/zenaura/client/page.py
+src/zenaura/client/persistance.py
+src/zenaura/client/algorithm/__init__.py
+src/zenaura/client/algorithm/algorithm.py
+src/zenaura/client/algorithm/operations.py
+src/zenaura/client/algorithm/searcher.py
+src/zenaura/client/algorithm/updater.py
+src/zenaura/client/compiler/__init__.py
+src/zenaura/client/compiler/attribute.py
+src/zenaura/client/compiler/compiler.py
+src/zenaura/client/compiler/sanitize.py
+src/zenaura/client/dom/__init__.py
+src/zenaura/client/dom/dom.py
+src/zenaura/client/dom/error.py
+src/zenaura/client/dom/mount.py
+src/zenaura/client/dom/render.py
+src/zenaura/client/hydrator/__init__.py
+src/zenaura/client/hydrator/compiler_adapter.py
+src/zenaura/client/hydrator/hydrator.py
+src/zenaura/client/hydrator/lookup.py
+src/zenaura/client/hydrator/real_dom_adapter.py
+src/zenaura/client/hydrator/tasker.py
+src/zenaura/client/hydrator/virtual_dom_adapter.py
+src/zenaura/client/observer/__init__.py
+src/zenaura/client/observer/observer.py
+src/zenaura/client/observer/subject.py
+src/zenaura/client/tags/__init__.py
+src/zenaura/client/tags/attribute.py
+src/zenaura/client/tags/builder.py
+src/zenaura/client/tags/data.py
+src/zenaura/client/tags/html.py
+src/zenaura/client/tags/node.py
+src/zenaura/server/__init__.py
+src/zenaura/server/server.py
 tests/test_algorithm.py
 tests/test_app.py
 tests/test_compiler.py
 tests/test_component_e2e.py
 tests/test_component_unit.py
 tests/test_node_properties.py
 tests/test_observer.py
 tests/test_rdom_adapter.py
 tests/test_tags.py
 tests/test_tasker.py
-tests/test_zenaura_dom.py
-zenaura/client/__init__.py
-zenaura/client/app.py
-zenaura/client/component.py
-zenaura/client/config.py
-zenaura/client/mocks.py
-zenaura/client/mutator.py
-zenaura/client/observer.py
-zenaura/client/page.py
-zenaura/client/persistance.py
-zenaura/client/algorithm/__init__.py
-zenaura/client/algorithm/algorithm.py
-zenaura/client/algorithm/operations.py
-zenaura/client/algorithm/searcher.py
-zenaura/client/algorithm/updater.py
-zenaura/client/compiler/__init__.py
-zenaura/client/compiler/attribute.py
-zenaura/client/compiler/compiler.py
-zenaura/client/compiler/sanitize.py
-zenaura/client/dom/__init__.py
-zenaura/client/dom/dom.py
-zenaura/client/dom/error.py
-zenaura/client/dom/mount.py
-zenaura/client/dom/render.py
-zenaura/client/hydrator/__init__.py
-zenaura/client/hydrator/compiler_adapter.py
-zenaura/client/hydrator/hydrator.py
-zenaura/client/hydrator/lookup.py
-zenaura/client/hydrator/real_dom_adapter.py
-zenaura/client/hydrator/tasker.py
-zenaura/client/hydrator/virtual_dom_adapter.py
-zenaura/client/observer/__init__.py
-zenaura/client/observer/observer.py
-zenaura/client/observer/subject.py
-zenaura/client/tags/__init__.py
-zenaura/client/tags/attribute.py
-zenaura/client/tags/builder.py
-zenaura/client/tags/data.py
-zenaura/client/tags/html.py
-zenaura/client/tags/node.py
-zenaura/server/__init__.py
-zenaura/server/server.py
-zenaura/zenaura.egg-info/PKG-INFO
-zenaura/zenaura.egg-info/SOURCES.txt
-zenaura/zenaura.egg-info/dependency_links.txt
-zenaura/zenaura.egg-info/requires.txt
-zenaura/zenaura.egg-info/top_level.txt
+tests/test_zenaura_dom.py
```

