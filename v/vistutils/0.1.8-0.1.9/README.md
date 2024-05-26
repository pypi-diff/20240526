# Comparing `tmp/vistutils-0.1.8.tar.gz` & `tmp/vistutils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vistutils-0.1.8.tar", last modified: Fri Feb  2 13:12:04 2024, max compression
+gzip compressed data, was "vistutils-0.1.9.tar", last modified: Mon Feb 12 09:51:01 2024, max compression
```

## Comparing `vistutils-0.1.8.tar` & `vistutils-0.1.9.tar`

### file list

```diff
@@ -1,58 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.652979 vistutils-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-02 13:11:47.000000 vistutils-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-02 13:12:04.652979 vistutils-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-02 13:11:47.000000 vistutils-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-02 13:11:57.000000 vistutils-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-02 13:12:04.652979 vistutils-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.644979 vistutils-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.644979 vistutils-0.1.8/src/vistutils/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/_cat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/_complex_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/_get_project_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/_maybe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/_mono_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/_search_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/_string_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/_weekday.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.648979 vistutils-0.1.8/src/vistutils/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/decorators/_abstract_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/decorators/_dec_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/decorators/_dec_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.648979 vistutils-0.1.8/src/vistutils/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/dispatcher/_abstract_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/dispatcher/_res.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.648979 vistutils-0.1.8/src/vistutils/fields/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/fields/_abstract_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/fields/_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/fields/_custom_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/fields/_field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.648979 vistutils-0.1.8/src/vistutils/metas/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/metas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/metas/_abstract_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/metas/_abstract_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/metas/_base_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/metas/_expanded_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/metas/_type_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.652979 vistutils-0.1.8/src/vistutils/readenv/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/readenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/readenv/_apply_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/readenv/_get_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/readenv/_get_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/readenv/_load_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/readenv/_parse_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/readenv/_read_env_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/readenv/_read_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.652979 vistutils-0.1.8/src/vistutils/waitaminute/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/waitaminute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/waitaminute/_effort_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/waitaminute/_parsing_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-02 13:11:47.000000 vistutils-0.1.8/src/vistutils/waitaminute/_type_msg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 13:12:04.652979 vistutils-0.1.8/src/vistutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-02 13:12:04.000000 vistutils-0.1.8/src/vistutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-02-02 13:12:04.000000 vistutils-0.1.8/src/vistutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 13:12:04.000000 vistutils-0.1.8/src/vistutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-02 13:12:04.000000 vistutils-0.1.8/src/vistutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.203110 vistutils-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-12 09:50:43.000000 vistutils-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-12 09:51:01.203110 vistutils-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-12 09:50:43.000000 vistutils-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-12 09:50:53.000000 vistutils-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-12 09:51:01.207111 vistutils-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.191110 vistutils-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.195110 vistutils-0.1.9/src/vistutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_apply_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_data_array.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.195110 vistutils-0.1.9/src/vistutils/_deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_abstract_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_abstract_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_base_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_cat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_complex_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_custom_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_expanded_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_maybe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_type_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/_weekday.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.199110 vistutils-0.1.9/src/vistutils/_deprecated/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/decorators/_abstract_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/decorators/_dec_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/decorators/_dec_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.199110 vistutils-0.1.9/src/vistutils/_deprecated/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/dispatcher/_abstract_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/dispatcher/_res.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.199110 vistutils-0.1.9/src/vistutils/_deprecated/readenv/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/readenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/readenv/_apply_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/readenv/_get_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/readenv/_get_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/readenv/_load_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/readenv/_parse_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/readenv/_read_env_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_deprecated/readenv/_read_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.199110 vistutils-0.1.9/src/vistutils/_future/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/_field_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/_func_sig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/_meta_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/_overload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/_overload_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/_overload_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.203110 vistutils-0.1.9/src/vistutils/_future/ezdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/ezdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/ezdata/_ez_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/ezdata/_ez_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/ezdata/_ez_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_future/ezdata/_ez_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_get_env_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_get_project_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_load_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_maybe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_mono_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_search_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/_string_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.203110 vistutils-0.1.9/src/vistutils/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/fields/_abstract_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/fields/_class_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/fields/_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.203110 vistutils-0.1.9/src/vistutils/metas/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/metas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/metas/_abstract_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/metas/_abstract_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/metas/_base_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/metas/_type_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.203110 vistutils-0.1.9/src/vistutils/waitaminute/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/waitaminute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/waitaminute/_effort_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/waitaminute/_parsing_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/waitaminute/_type_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-12 09:50:43.000000 vistutils-0.1.9/src/vistutils/waitaminute/_wait_for_it.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:51:01.203110 vistutils-0.1.9/src/vistutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-12 09:51:01.000000 vistutils-0.1.9/src/vistutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-02-12 09:51:01.000000 vistutils-0.1.9/src/vistutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 09:51:01.000000 vistutils-0.1.9/src/vistutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-12 09:51:01.000000 vistutils-0.1.9/src/vistutils.egg-info/top_level.txt
```

### Comparing `vistutils-0.1.8/LICENSE` & `vistutils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/PKG-INFO` & `vistutils-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vistutils
-Version: 0.1.8
+Version: 0.1.9
 Summary: vistutils provides helpful utility functions
 Home-page: https://github.com/AsgerJon/vistutils
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/vistutils
 Project-URL: Bug Tracker, https://github.com/AsgerJon/vistutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vistutils-0.1.8/pyproject.toml` & `vistutils-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools>=68.2']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "vistutils"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name = "Asger Jon Vistisen", email = "asgerjon2@gmail.com" },
 ]
 description = "vistutils provides helpful utility functions"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `vistutils-0.1.8/setup.cfg` & `vistutils-0.1.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vistutils
-version = 0.1.8
+version = 0.1.9
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = Helpful utility functions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AsgerJon/vistutils
 classifiers =
```

### Comparing `vistutils-0.1.8/src/vistutils/_cat.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_cat.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/_complex_number.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_complex_number.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/_maybe.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_maybe.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/_mono_space.py` & `vistutils-0.1.9/src/vistutils/_mono_space.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/_search_key.py` & `vistutils-0.1.9/src/vistutils/_search_key.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/_string_list.py` & `vistutils-0.1.9/src/vistutils/_string_list.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/decorators/_abstract_decorator.py` & `vistutils-0.1.9/src/vistutils/_deprecated/decorators/_abstract_decorator.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/decorators/_dec_meta.py` & `vistutils-0.1.9/src/vistutils/_deprecated/decorators/_dec_meta.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/dispatcher/_abstract_dispatcher.py` & `vistutils-0.1.9/src/vistutils/_deprecated/dispatcher/_abstract_dispatcher.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/dispatcher/_res.py` & `vistutils-0.1.9/src/vistutils/_deprecated/dispatcher/_res.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/fields/_abstract_field.py` & `vistutils-0.1.9/src/vistutils/fields/_abstract_field.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 automatically by the __set_name__ method. """
 #  MIT Licence
 #  Copyright (c) 2024 Asger Jon Vistisen
 from __future__ import annotations
 
 from abc import abstractmethod
 
+from vistutils.waitaminute import typeMsg
+
 
 class AbstractField:
   """The AbstractField defines an abstract baseclass for descriptor
 classes."""
 
   def __init__(self, *args, **kwargs) -> None:
     self.__field_name__ = None
     self.__field_owner__ = None
 
   def __set_name__(self, owner: type, name: str) -> None:
     self.__field_owner__ = owner
     self.__field_name__ = name
     self.__prepare_owner__(owner)
 
-  @abstractmethod
   def __prepare_owner__(self, owner: type) -> type:
     """This special abstract method must be implemented by subclasses to
 install this field into it."""
 
   def _getFieldOwner(self) -> type:
     """Getter-function for field owner"""
     if self.__field_owner__ is not None:
```

### Comparing `vistutils-0.1.8/src/vistutils/fields/_apply.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_apply.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/fields/_custom_field.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_custom_field.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/fields/_field.py` & `vistutils-0.1.9/src/vistutils/fields/_field.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/metas/_abstract_metaclass.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_abstract_metaclass.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/metas/_abstract_namespace.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_abstract_namespace.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/metas/_base_namespace.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_base_namespace.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/metas/_expanded_class.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_expanded_class.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/readenv/__init__.py` & `vistutils-0.1.9/src/vistutils/_deprecated/readenv/__init__.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/readenv/_apply_env.py` & `vistutils-0.1.9/src/vistutils/_deprecated/readenv/_apply_env.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/readenv/_get_parent.py` & `vistutils-0.1.9/src/vistutils/_deprecated/readenv/_get_parent.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/readenv/_load_env.py` & `vistutils-0.1.9/src/vistutils/_deprecated/readenv/_load_env.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/readenv/_parse_env.py` & `vistutils-0.1.9/src/vistutils/_deprecated/readenv/_parse_env.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/readenv/_read_env_exception.py` & `vistutils-0.1.9/src/vistutils/_deprecated/readenv/_read_env_exception.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/readenv/_read_file.py` & `vistutils-0.1.9/src/vistutils/_deprecated/readenv/_read_file.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/waitaminute/_effort_exception.py` & `vistutils-0.1.9/src/vistutils/waitaminute/_effort_exception.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/waitaminute/_parsing_error.py` & `vistutils-0.1.9/src/vistutils/waitaminute/_parsing_error.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils/waitaminute/_type_msg.py` & `vistutils-0.1.9/src/vistutils/_deprecated/_type_msg.py`

 * *Files identical despite different names*

### Comparing `vistutils-0.1.8/src/vistutils.egg-info/PKG-INFO` & `vistutils-0.1.9/src/vistutils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vistutils
-Version: 0.1.8
+Version: 0.1.9
 Summary: vistutils provides helpful utility functions
 Home-page: https://github.com/AsgerJon/vistutils
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/vistutils
 Project-URL: Bug Tracker, https://github.com/AsgerJon/vistutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vistutils-0.1.8/src/vistutils.egg-info/SOURCES.txt` & `vistutils-0.1.9/src/vistutils.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,72 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/vistutils/__init__.py
-src/vistutils/_cat.py
-src/vistutils/_complex_number.py
+src/vistutils/_apply_env.py
+src/vistutils/_data_array.py
+src/vistutils/_get_env_files.py
 src/vistutils/_get_project_root.py
+src/vistutils/_load_env.py
 src/vistutils/_maybe.py
 src/vistutils/_mono_space.py
 src/vistutils/_search_key.py
 src/vistutils/_string_list.py
-src/vistutils/_weekday.py
 src/vistutils.egg-info/PKG-INFO
 src/vistutils.egg-info/SOURCES.txt
 src/vistutils.egg-info/dependency_links.txt
 src/vistutils.egg-info/top_level.txt
-src/vistutils/decorators/__init__.py
-src/vistutils/decorators/_abstract_decorator.py
-src/vistutils/decorators/_dec_meta.py
-src/vistutils/decorators/_dec_space.py
-src/vistutils/dispatcher/__init__.py
-src/vistutils/dispatcher/_abstract_dispatcher.py
-src/vistutils/dispatcher/_res.py
+src/vistutils/_deprecated/__init__.py
+src/vistutils/_deprecated/_abstract_metaclass.py
+src/vistutils/_deprecated/_abstract_namespace.py
+src/vistutils/_deprecated/_apply.py
+src/vistutils/_deprecated/_base_namespace.py
+src/vistutils/_deprecated/_cat.py
+src/vistutils/_deprecated/_complex_number.py
+src/vistutils/_deprecated/_custom_field.py
+src/vistutils/_deprecated/_data_type.py
+src/vistutils/_deprecated/_expanded_class.py
+src/vistutils/_deprecated/_maybe.py
+src/vistutils/_deprecated/_type_msg.py
+src/vistutils/_deprecated/_weekday.py
+src/vistutils/_deprecated/decorators/__init__.py
+src/vistutils/_deprecated/decorators/_abstract_decorator.py
+src/vistutils/_deprecated/decorators/_dec_meta.py
+src/vistutils/_deprecated/decorators/_dec_space.py
+src/vistutils/_deprecated/dispatcher/__init__.py
+src/vistutils/_deprecated/dispatcher/_abstract_dispatcher.py
+src/vistutils/_deprecated/dispatcher/_res.py
+src/vistutils/_deprecated/readenv/__init__.py
+src/vistutils/_deprecated/readenv/_apply_env.py
+src/vistutils/_deprecated/readenv/_get_parent.py
+src/vistutils/_deprecated/readenv/_get_root.py
+src/vistutils/_deprecated/readenv/_load_env.py
+src/vistutils/_deprecated/readenv/_parse_env.py
+src/vistutils/_deprecated/readenv/_read_env_exception.py
+src/vistutils/_deprecated/readenv/_read_file.py
+src/vistutils/_future/__init__.py
+src/vistutils/_future/_field_namespace.py
+src/vistutils/_future/_func_sig.py
+src/vistutils/_future/_meta_field.py
+src/vistutils/_future/_overload.py
+src/vistutils/_future/_overload_metaclass.py
+src/vistutils/_future/_overload_namespace.py
+src/vistutils/_future/ezdata/__init__.py
+src/vistutils/_future/ezdata/_ez_data.py
+src/vistutils/_future/ezdata/_ez_field.py
+src/vistutils/_future/ezdata/_ez_meta.py
+src/vistutils/_future/ezdata/_ez_space.py
 src/vistutils/fields/__init__.py
 src/vistutils/fields/_abstract_field.py
-src/vistutils/fields/_apply.py
-src/vistutils/fields/_custom_field.py
+src/vistutils/fields/_class_field.py
 src/vistutils/fields/_field.py
 src/vistutils/metas/__init__.py
 src/vistutils/metas/_abstract_metaclass.py
 src/vistutils/metas/_abstract_namespace.py
 src/vistutils/metas/_base_namespace.py
-src/vistutils/metas/_expanded_class.py
 src/vistutils/metas/_type_names.py
-src/vistutils/readenv/__init__.py
-src/vistutils/readenv/_apply_env.py
-src/vistutils/readenv/_get_parent.py
-src/vistutils/readenv/_get_root.py
-src/vistutils/readenv/_load_env.py
-src/vistutils/readenv/_parse_env.py
-src/vistutils/readenv/_read_env_exception.py
-src/vistutils/readenv/_read_file.py
 src/vistutils/waitaminute/__init__.py
 src/vistutils/waitaminute/_effort_exception.py
 src/vistutils/waitaminute/_parsing_error.py
-src/vistutils/waitaminute/_type_msg.py
+src/vistutils/waitaminute/_type_msg.py
+src/vistutils/waitaminute/_wait_for_it.py
```

