# Comparing `tmp/abcli-9.26.1.tar.gz` & `tmp/abcli-9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abcli-9.26.1.tar", last modified: Sun May 26 17:45:03 2024, max compression
+gzip compressed data, was "abcli-9.3.1.tar", last modified: Sun May 26 04:24:36 2024, max compression
```

## Comparing `abcli-9.26.1.tar` & `abcli-9.3.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.748484 abcli-9.26.1/
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 17:16:07.000000 abcli-9.26.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     2017 2024-05-26 17:45:03.747908 abcli-9.26.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1117 2024-05-26 17:16:07.000000 abcli-9.26.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.707503 abcli-9.26.1/abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      321 2024-05-26 17:44:58.000000 abcli-9.26.1/abcli/__init__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.710089 abcli-9.26.1/abcli/bash/
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2022-08-19 04:11:13.000000 abcli-9.26.1/abcli/bash/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/bash/colors.py
--rw-r--r--   0 kamangir   (502) staff       (20)      598 2024-02-18 05:10:50.000000 abcli-9.26.1/abcli/bash/help.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2309 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/bash/list.py
--rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/bash/logging.py
--rw-r--r--   0 kamangir   (502) staff       (20)      784 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/elapsed_timer.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5370 2024-05-26 17:40:13.000000 abcli-9.26.1/abcli/env.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.712094 abcli-9.26.1/abcli/file/
--rw-r--r--   0 kamangir   (502) staff       (20)      109 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/file/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      996 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/file/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      570 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/file/classes.py
--rw-r--r--   0 kamangir   (502) staff       (20)     9177 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/file/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6315 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/file/load.py
--rw-r--r--   0 kamangir   (502) staff       (20)     7303 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/file/save.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.714120 abcli-9.26.1/abcli/keywords/
--rw-r--r--   0 kamangir   (502) staff       (20)       84 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/keywords/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      897 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/keywords/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      236 2022-08-20 04:12:52.000000 abcli-9.26.1/abcli/keywords/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1407 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/keywords/keywords.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1353 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.715230 abcli-9.26.1/abcli/modules/
--rw-r--r--   0 kamangir   (502) staff       (20)       23 2022-08-28 06:57:23.000000 abcli-9.26.1/abcli/modules/__init__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.716711 abcli-9.26.1/abcli/modules/host/
--rw-r--r--   0 kamangir   (502) staff       (20)       90 2022-09-21 00:58:39.000000 abcli-9.26.1/abcli/modules/host/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2523 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/modules/host/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5416 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/modules/host/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2025 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/modules/objects.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.718098 abcli-9.26.1/abcli/options/
--rw-r--r--   0 kamangir   (502) staff       (20)       53 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/options/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1751 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/options/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2826 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/options/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.719438 abcli-9.26.1/abcli/path/
--rw-r--r--   0 kamangir   (502) staff       (20)       68 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/path/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/path/consts.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5254 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/path/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.724291 abcli-9.26.1/abcli/plugins/
--rw-r--r--   0 kamangir   (502) staff       (20)       49 2024-05-26 17:16:10.000000 abcli-9.26.1/abcli/plugins/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1651 2024-05-26 17:16:10.000000 abcli-9.26.1/abcli/plugins/__main__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.725760 abcli-9.26.1/abcli/plugins/cache/
--rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.26.1/abcli/plugins/cache/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1646 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/cache/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4705 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/cache/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1265 2024-05-26 17:16:10.000000 abcli-9.26.1/abcli/plugins/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.727269 abcli-9.26.1/abcli/plugins/git/
--rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/git/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      696 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/git/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1716 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/git/version.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.728703 abcli-9.26.1/abcli/plugins/gpu/
--rw-r--r--   0 kamangir   (502) staff       (20)       52 2022-08-20 04:12:52.000000 abcli-9.26.1/abcli/plugins/gpu/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      499 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/gpu/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      590 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/gpu/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.731957 abcli-9.26.1/abcli/plugins/graphics/
--rw-r--r--   0 kamangir   (502) staff       (20)      124 2022-09-25 02:29:01.000000 abcli-9.26.1/abcli/plugins/graphics/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1462 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/graphics/constants.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1740 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/graphics/gif.py
--rw-r--r--   0 kamangir   (502) staff       (20)      431 2022-08-14 18:15:57.000000 abcli-9.26.1/abcli/plugins/graphics/image.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/graphics/signature.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6641 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/graphics/text.py
--rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/markdown.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.733427 abcli-9.26.1/abcli/plugins/metadata/
--rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/metadata/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2109 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/metadata/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2231 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/metadata/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.734421 abcli-9.26.1/abcli/plugins/relations/
--rw-r--r--   0 kamangir   (502) staff       (20)       59 2022-08-20 04:12:52.000000 abcli-9.26.1/abcli/plugins/relations/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2102 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/relations/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5157 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/relations/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      705 2024-05-26 17:16:10.000000 abcli-9.26.1/abcli/plugins/seed.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.735401 abcli-9.26.1/abcli/plugins/storage/
--rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/storage/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2248 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/storage/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     8063 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/storage/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.737042 abcli-9.26.1/abcli/plugins/tags/
--rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.26.1/abcli/plugins/tags/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2219 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/tags/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5991 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/tags/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      344 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/testing.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1313 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/plugins/video.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.740003 abcli-9.26.1/abcli/string/
--rw-r--r--   0 kamangir   (502) staff       (20)      244 2024-02-18 05:23:47.000000 abcli-9.26.1/abcli/string/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1138 2024-02-18 05:23:40.000000 abcli-9.26.1/abcli/string/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-02-18 05:23:45.000000 abcli-9.26.1/abcli/string/constants.py
--rw-r--r--   0 kamangir   (502) staff       (20)    11283 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/string/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.741249 abcli-9.26.1/abcli/table/
--rw-r--r--   0 kamangir   (502) staff       (20)       45 2022-08-20 04:12:52.000000 abcli-9.26.1/abcli/table/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4541 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/table/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.746644 abcli-9.26.1/abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/tests/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       69 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/tests/test_abcli.py
--rw-r--r--   0 kamangir   (502) staff       (20)      275 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/tests/test_env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      410 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/tests/test_modules_objects.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3194 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/tests/test_options.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1400 2024-05-26 17:16:10.000000 abcli-9.26.1/abcli/tests/test_plugins.py
--rw-r--r--   0 kamangir   (502) staff       (20)      634 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/tests/test_plugins_graphics_signature.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2831 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/tests/test_plugins_metadata.py
--rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/tests/test_plugins_testing.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2199 2024-05-26 17:16:07.000000 abcli-9.26.1/abcli/timer.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 17:45:03.747219 abcli-9.26.1/abcli.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     2017 2024-05-26 17:45:03.000000 abcli-9.26.1/abcli.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     2501 2024-05-26 17:45:03.000000 abcli-9.26.1/abcli.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 17:45:03.000000 abcli-9.26.1/abcli.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-26 17:45:03.000000 abcli-9.26.1/abcli.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-26 17:45:03.000000 abcli-9.26.1/abcli.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 17:16:07.000000 abcli-9.26.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      124 2024-05-26 17:16:07.000000 abcli-9.26.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 17:45:03.748602 abcli-9.26.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      863 2024-05-26 17:16:10.000000 abcli-9.26.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.962942 abcli-9.3.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:20.000000 abcli-9.3.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     2016 2024-05-26 04:24:36.962567 abcli-9.3.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1117 2024-05-18 22:32:18.000000 abcli-9.3.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.929032 abcli-9.3.1/abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      288 2024-05-26 04:24:32.000000 abcli-9.3.1/abcli/__init__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.932563 abcli-9.3.1/abcli/bash/
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2022-08-19 04:11:13.000000 abcli-9.3.1/abcli/bash/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-04-21 22:44:21.000000 abcli-9.3.1/abcli/bash/colors.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      598 2024-02-18 05:10:50.000000 abcli-9.3.1/abcli/bash/help.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2309 2024-04-21 22:45:41.000000 abcli-9.3.1/abcli/bash/list.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 23:19:04.000000 abcli-9.3.1/abcli/bash/logging.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      784 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/elapsed_timer.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5290 2024-04-27 21:10:00.000000 abcli-9.3.1/abcli/env.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.934874 abcli-9.3.1/abcli/file/
+-rw-r--r--   0 kamangir   (502) staff       (20)      109 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/file/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      996 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/file/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      570 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/file/classes.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     9177 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/file/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6315 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/file/load.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     7303 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/file/save.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.936590 abcli-9.3.1/abcli/keywords/
+-rw-r--r--   0 kamangir   (502) staff       (20)       84 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/keywords/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      897 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/keywords/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      236 2022-08-20 04:12:52.000000 abcli-9.3.1/abcli/keywords/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1407 2024-04-23 03:10:32.000000 abcli-9.3.1/abcli/keywords/keywords.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1353 2024-04-29 00:44:19.000000 abcli-9.3.1/abcli/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.937533 abcli-9.3.1/abcli/modules/
+-rw-r--r--   0 kamangir   (502) staff       (20)       23 2022-08-28 06:57:23.000000 abcli-9.3.1/abcli/modules/__init__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.939650 abcli-9.3.1/abcli/modules/host/
+-rw-r--r--   0 kamangir   (502) staff       (20)       90 2022-09-21 00:58:39.000000 abcli-9.3.1/abcli/modules/host/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2523 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/modules/host/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5416 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/modules/host/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2025 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/modules/objects.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.941039 abcli-9.3.1/abcli/options/
+-rw-r--r--   0 kamangir   (502) staff       (20)       53 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/options/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1751 2024-05-08 04:06:06.000000 abcli-9.3.1/abcli/options/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2826 2024-05-10 02:13:35.000000 abcli-9.3.1/abcli/options/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.942063 abcli-9.3.1/abcli/path/
+-rw-r--r--   0 kamangir   (502) staff       (20)       68 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/path/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/path/consts.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5254 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/path/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.944230 abcli-9.3.1/abcli/plugins/
+-rw-r--r--   0 kamangir   (502) staff       (20)       49 2022-08-20 04:12:52.000000 abcli-9.3.1/abcli/plugins/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      916 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/__main__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.945838 abcli-9.3.1/abcli/plugins/cache/
+-rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.3.1/abcli/plugins/cache/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1646 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/cache/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4705 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/cache/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      524 2024-05-26 04:21:10.000000 abcli-9.3.1/abcli/plugins/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.947083 abcli-9.3.1/abcli/plugins/git/
+-rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-20 04:27:12.000000 abcli-9.3.1/abcli/plugins/git/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      696 2024-05-20 04:26:24.000000 abcli-9.3.1/abcli/plugins/git/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1716 2024-05-20 04:27:32.000000 abcli-9.3.1/abcli/plugins/git/version.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.948165 abcli-9.3.1/abcli/plugins/gpu/
+-rw-r--r--   0 kamangir   (502) staff       (20)       52 2022-08-20 04:12:52.000000 abcli-9.3.1/abcli/plugins/gpu/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      499 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/gpu/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      590 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/gpu/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.951174 abcli-9.3.1/abcli/plugins/graphics/
+-rw-r--r--   0 kamangir   (502) staff       (20)      124 2022-09-25 02:29:01.000000 abcli-9.3.1/abcli/plugins/graphics/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1462 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/graphics/constants.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1740 2024-05-08 02:05:01.000000 abcli-9.3.1/abcli/plugins/graphics/gif.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      431 2022-08-14 18:15:57.000000 abcli-9.3.1/abcli/plugins/graphics/image.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/graphics/signature.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6641 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/graphics/text.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/markdown.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.952268 abcli-9.3.1/abcli/plugins/metadata/
+-rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/metadata/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2109 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/metadata/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2231 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/metadata/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.953094 abcli-9.3.1/abcli/plugins/relations/
+-rw-r--r--   0 kamangir   (502) staff       (20)       59 2022-08-20 04:12:52.000000 abcli-9.3.1/abcli/plugins/relations/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2102 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/relations/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5157 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/relations/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      680 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/seed.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.954448 abcli-9.3.1/abcli/plugins/storage/
+-rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/storage/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2248 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/storage/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     8063 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/storage/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.955523 abcli-9.3.1/abcli/plugins/tags/
+-rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.3.1/abcli/plugins/tags/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2219 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/tags/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5991 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/tags/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      344 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/testing.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1313 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/plugins/video.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.957271 abcli-9.3.1/abcli/string/
+-rw-r--r--   0 kamangir   (502) staff       (20)      244 2024-02-18 05:23:47.000000 abcli-9.3.1/abcli/string/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1138 2024-02-18 05:23:40.000000 abcli-9.3.1/abcli/string/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-02-18 05:23:45.000000 abcli-9.3.1/abcli/string/constants.py
+-rw-r--r--   0 kamangir   (502) staff       (20)    11283 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/string/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.958167 abcli-9.3.1/abcli/table/
+-rw-r--r--   0 kamangir   (502) staff       (20)       45 2022-08-20 04:12:52.000000 abcli-9.3.1/abcli/table/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4541 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/table/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.961621 abcli-9.3.1/abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/tests/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       69 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/tests/test_abcli.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      275 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/tests/test_env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      410 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/tests/test_modules_objects.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3194 2024-05-10 02:20:04.000000 abcli-9.3.1/abcli/tests/test_options.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      104 2024-05-26 04:20:33.000000 abcli-9.3.1/abcli/tests/test_plugins.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      634 2024-05-08 02:13:37.000000 abcli-9.3.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/tests/test_plugins_graphics_signature.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2831 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/tests/test_plugins_metadata.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/tests/test_plugins_testing.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2199 2024-04-21 00:00:57.000000 abcli-9.3.1/abcli/timer.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:24:36.962021 abcli-9.3.1/abcli.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     2016 2024-05-26 04:24:36.000000 abcli-9.3.1/abcli.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     2501 2024-05-26 04:24:36.000000 abcli-9.3.1/abcli.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 04:24:36.000000 abcli-9.3.1/abcli.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-26 04:24:36.000000 abcli-9.3.1/abcli.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-26 04:24:36.000000 abcli-9.3.1/abcli.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 03:28:20.000000 abcli-9.3.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      124 2024-05-20 22:39:16.000000 abcli-9.3.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 04:24:36.963018 abcli-9.3.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      861 2024-05-21 04:09:10.000000 abcli-9.3.1/setup.py
```

### Comparing `abcli-9.26.1/PKG-INFO` & `abcli-9.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abcli
-Version: 9.26.1
+Version: 9.3.1
 Summary: 🚀 a language to speak AI.
 Home-page: https://github.com/kamangir/awesome-bash-cli
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `abcli-9.26.1/README.md` & `abcli-9.3.1/README.md`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/bash/help.py` & `abcli-9.3.1/abcli/bash/help.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/bash/list.py` & `abcli-9.3.1/abcli/bash/list.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/bash/logging.py` & `abcli-9.3.1/abcli/bash/logging.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/config.env` & `abcli-9.3.1/abcli/config.env`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/elapsed_timer.py` & `abcli-9.3.1/abcli/elapsed_timer.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/env.py` & `abcli-9.3.1/abcli/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,14 @@
     load_dotenv(env_filename)
 
 
 load_env(__name__)
 load_config(__name__)
 
 
-abcli_is_github_workflow = os.getenv("GITHUB_ACTIONS", "")
-
 abcli_aws_ec2_default_image_name = os.getenv("abcli_aws_ec2_default_image_name", "")
 abcli_aws_ec2_default_instance_type = os.getenv(
     "abcli_aws_ec2_default_instance_type", ""
 )
 abcli_aws_ec2_default_template = os.getenv("abcli_aws_ec2_default_template", "")
 abcli_aws_ec2_image_id_abcli = os.getenv("abcli_aws_ec2_image_id_abcli", "")
 abcli_aws_ec2_image_id_abcli_g4dn = os.getenv("abcli_aws_ec2_image_id_abcli_g4dn", "")
@@ -120,15 +118,15 @@
 abcli_log_filename = os.getenv("abcli_log_filename", "")
 
 abcli_publish_prefix = os.getenv("abcli_publish_prefix", "")
 
 abcli_papertrail_dest_host = os.getenv("abcli_papertrail_dest_host", "")
 abcli_papertrail_dest_port = os.getenv("abcli_papertrail_dest_port", "")
 
-abcli_plugins_must_have = os.getenv("abcli_plugins_must_have", "")
+abcli_plugins = os.getenv("abcli_plugins", "")
 
 abcli_session_auto_upload = os.getenv("abcli_session_auto_upload", "")
 abcli_session_imager_diff = os.getenv("abcli_session_imager_diff", "")
 abcli_session_imager_enabled = os.getenv("abcli_session_imager_enabled", "")
 abcli_session_imager_period = os.getenv("abcli_session_imager_period", "")
 abcli_session_imager = os.getenv("abcli_session_imager", "")
 abcli_session_messenger_period = os.getenv("abcli_session_messenger_period", "")
```

### Comparing `abcli-9.26.1/abcli/file/__main__.py` & `abcli-9.3.1/abcli/file/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/file/classes.py` & `abcli-9.3.1/abcli/file/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/file/functions.py` & `abcli-9.3.1/abcli/file/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/file/load.py` & `abcli-9.3.1/abcli/file/load.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/file/save.py` & `abcli-9.3.1/abcli/file/save.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/keywords/__main__.py` & `abcli-9.3.1/abcli/keywords/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/keywords/keywords.py` & `abcli-9.3.1/abcli/keywords/keywords.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/logger.py` & `abcli-9.3.1/abcli/logger.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/modules/host/__main__.py` & `abcli-9.3.1/abcli/modules/host/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/modules/host/functions.py` & `abcli-9.3.1/abcli/modules/host/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/modules/objects.py` & `abcli-9.3.1/abcli/modules/objects.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/options/__main__.py` & `abcli-9.3.1/abcli/options/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/options/classes.py` & `abcli-9.3.1/abcli/options/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/path/functions.py` & `abcli-9.3.1/abcli/path/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/__main__.py` & `abcli-9.3.1/abcli/plugins/cache/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,85 @@
 import argparse
-from abcli import VERSION
-from abcli.plugins import NAME
-from abcli.plugins.functions import get_module_name, get_plugin_name, list_of_external
+from . import *
 from abcli.logger import logger
 
 
 parser = argparse.ArgumentParser(NAME)
 parser.add_argument(
     "task",
     type=str,
-    default="",
-    help="get_module_name|get_plugin_name|list_of_external",
-)
-parser.add_argument(
-    "--delim",
-    type=str,
-    default=", ",
+    default="read",
+    help="clone,create,read,search,write",
 )
 parser.add_argument(
-    "--log",
-    default=1,
+    "--all",
+    default=0,
     type=int,
-    help="0|1",
 )
 parser.add_argument(
-    "--repo_names",
+    "--dataframe",
     default=0,
     type=int,
-    help="0|1",
 )
 parser.add_argument(
-    "--repo_name",
-    default="",
+    "--destination",
     type=str,
+    default="",
 )
 parser.add_argument(
-    "--plugin_name",
-    default="",
+    "--keyword",
     type=str,
 )
 parser.add_argument(
-    "--from_plugin_name",
+    "--like",
     default=0,
     type=int,
-    help="0|1",
+)
+parser.add_argument(
+    "--source",
+    type=str,
+    default="",
+)
+parser.add_argument(
+    "--unique",
+    default=1,
+    type=int,
+    help="cache.read('unique')",
+)
+parser.add_argument(
+    "--value",
+    type=str,
+    default="unknown",
 )
 args = parser.parse_args()
 
-delim = " " if args.delim == "space" else args.delim
-
 success = False
-if args.task == "get_module_name":
-    success = True
-    print(get_module_name(args.repo_name))
-elif args.task == "get_plugin_name":
+if args.task == "clone":
+    success = clone(args.source, args.destination)
+elif args.task == "create":
+    success = create()
+elif args.task == "read":
+    output = read(
+        args.keyword,
+        all=args.all,
+        like=args.like,
+        dataframe=args.dataframe,
+        unique=args.unique,
+    )
+
+    print(
+        ("None" if output.empty else output.drop(columns=["log_id"]))
+        if args.dataframe
+        else output
+    )
     success = True
-    print(get_plugin_name(args.repo_name))
-elif args.task == "list_of_external":
-    output = list_of_external(args.repo_names == 1)
-    if args.log:
-        logger.info(
-            "{:,} external {}(s): {}".format(
-                len(output),
-                "repo" if args.repo_names else "plugin",
-                delim.join(output),
-            )
-        )
-    else:
-        print(delim.join(output))
+elif args.task == "search":
+    for keyword, value in search(args.keyword).items():
+        print(f"{keyword}: {value}")
     success = True
+elif args.task == "write":
+    success = write(args.keyword, args.value)
 else:
     logger.error(f"-{NAME}: {args.task}: command not found.")
 
 if not success:
     logger.error(f"-{NAME}: {args.task}: failed.")
```

### Comparing `abcli-9.26.1/abcli/plugins/cache/__main__.py` & `abcli-9.3.1/abcli/plugins/metadata/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,101 @@
 import argparse
-from . import *
+from abcli.plugins.metadata import get, NAME, post, MetadataSourceType
 from abcli.logger import logger
 
 
 parser = argparse.ArgumentParser(NAME)
 parser.add_argument(
     "task",
     type=str,
-    default="read",
-    help="clone,create,read,search,write",
+    default="",
+    help="get|post",
 )
 parser.add_argument(
-    "--all",
-    default=0,
-    type=int,
+    "--default",
+    type=str,
+    default="",
 )
 parser.add_argument(
-    "--dataframe",
-    default=0,
+    "--delim",
+    type=str,
+    default="",
+)
+parser.add_argument(
+    "--dict_keys",
     type=int,
+    default=0,
+    help="0|1",
 )
 parser.add_argument(
-    "--destination",
-    type=str,
-    default="",
+    "--dict_values",
+    type=int,
+    default=0,
+    help="0|1",
 )
 parser.add_argument(
-    "--keyword",
+    "--filename",
     type=str,
+    default="metadata.yaml",
 )
 parser.add_argument(
-    "--like",
-    default=0,
+    "--is_base64_encoded",
     type=int,
+    default=0,
+    help="0|1",
+)
+parser.add_argument(
+    "--key",
+    type=str,
 )
 parser.add_argument(
     "--source",
     type=str,
-    default="",
 )
 parser.add_argument(
-    "--unique",
-    default=1,
-    type=int,
-    help="cache.read('unique')",
+    "--source_type",
+    type=str,
+    default=MetadataSourceType.FILENAME.name.lower(),
+    help="|".join([source_type.name.lower() for source_type in MetadataSourceType]),
 )
 parser.add_argument(
     "--value",
     type=str,
-    default="unknown",
+)
+parser.add_argument(
+    "--verbose",
+    type=int,
+    default="0",
+    help="0|1",
 )
 args = parser.parse_args()
 
+delim = " " if args.delim == "space" else args.delim
+
 success = False
-if args.task == "clone":
-    success = clone(args.source, args.destination)
-elif args.task == "create":
-    success = create()
-elif args.task == "read":
-    output = read(
-        args.keyword,
-        all=args.all,
-        like=args.like,
-        dataframe=args.dataframe,
-        unique=args.unique,
+if args.task == "get":
+    success = True
+    output = get(
+        key=args.key,
+        default=args.default,
+        source=args.source,
+        source_type=MetadataSourceType[args.source_type.upper()],
+        dict_keys=args.dict_keys,
+        dict_values=args.dict_values,
+        filename=args.filename,
     )
-
-    print(
-        ("None" if output.empty else output.drop(columns=["log_id"]))
-        if args.dataframe
-        else output
+    print(delim.join(output) if isinstance(output, list) else output)
+elif args.task == "post":
+    success = post(
+        key=args.key,
+        value=args.value,
+        filename=args.filename,
+        source=args.source,
+        source_type=MetadataSourceType[args.source_type.upper()],
+        is_base64_encoded=args.is_base64_encoded,
+        verbose=args.verbose == 1,
     )
-    success = True
-elif args.task == "search":
-    for keyword, value in search(args.keyword).items():
-        print(f"{keyword}: {value}")
-    success = True
-elif args.task == "write":
-    success = write(args.keyword, args.value)
 else:
     logger.error(f"-{NAME}: {args.task}: command not found.")
 
 if not success:
     logger.error(f"-{NAME}: {args.task}: failed.")
```

### Comparing `abcli-9.26.1/abcli/plugins/cache/functions.py` & `abcli-9.3.1/abcli/plugins/cache/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/git/__main__.py` & `abcli-9.3.1/abcli/plugins/git/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/git/version.py` & `abcli-9.3.1/abcli/plugins/git/version.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/gpu/functions.py` & `abcli-9.3.1/abcli/plugins/gpu/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/graphics/constants.py` & `abcli-9.3.1/abcli/plugins/graphics/constants.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/graphics/gif.py` & `abcli-9.3.1/abcli/plugins/graphics/gif.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/graphics/signature.py` & `abcli-9.3.1/abcli/plugins/graphics/signature.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/graphics/text.py` & `abcli-9.3.1/abcli/plugins/graphics/text.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/markdown.py` & `abcli-9.3.1/abcli/plugins/markdown.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/metadata/__main__.py` & `abcli-9.3.1/abcli/plugins/relations/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,98 @@
 import argparse
-from abcli.plugins.metadata import get, NAME, post, MetadataSourceType
+from . import *
 from abcli.logger import logger
 
 
 parser = argparse.ArgumentParser(NAME)
 parser.add_argument(
     "task",
     type=str,
-    default="",
-    help="get|post",
+    default="get",
+    help="clone|create|get|list|search|set",
 )
 parser.add_argument(
-    "--default",
-    type=str,
-    default="",
+    "--count",
+    type=int,
+    default=-1,
 )
 parser.add_argument(
     "--delim",
     type=str,
-    default="",
+    default=", ",
 )
 parser.add_argument(
-    "--dict_keys",
-    type=int,
-    default=0,
-    help="0|1",
-)
-parser.add_argument(
-    "--dict_values",
-    type=int,
-    default=0,
-    help="0|1",
+    "--filename",
+    type=str,
 )
 parser.add_argument(
-    "--filename",
+    "--item_name",
+    default="object",
     type=str,
-    default="metadata.yaml",
 )
 parser.add_argument(
-    "--is_base64_encoded",
+    "--log",
+    default=1,
     type=int,
-    default=0,
     help="0|1",
 )
 parser.add_argument(
-    "--key",
-    type=str,
-)
-parser.add_argument(
-    "--source",
+    "--object_1",
     type=str,
 )
 parser.add_argument(
-    "--source_type",
+    "--object_2",
     type=str,
-    default=MetadataSourceType.FILENAME.name.lower(),
-    help="|".join([source_type.name.lower() for source_type in MetadataSourceType]),
 )
 parser.add_argument(
-    "--value",
+    "--relation",
+    default="",
     type=str,
 )
 parser.add_argument(
-    "--verbose",
+    "--return_list",
     type=int,
-    default="0",
-    help="0|1",
+    default=0,
 )
 args = parser.parse_args()
 
 delim = " " if args.delim == "space" else args.delim
 
 success = False
-if args.task == "get":
+if args.task == "clone":
+    success = clone(args.object_1, args.object_2)
+elif args.task == "create":
+    success = create()
+elif args.task == "get":
+    relation = get(args.object_1, args.object_2)
+    if args.log:
+        logger.info(
+            f"{args.object_1} -{f'{relation}->' if relation else 'X-'} {args.object_2}"
+        )
+    else:
+        print(relation)
     success = True
-    output = get(
-        key=args.key,
-        default=args.default,
-        source=args.source,
-        source_type=MetadataSourceType[args.source_type.upper()],
-        dict_keys=args.dict_keys,
-        dict_values=args.dict_values,
-        filename=args.filename,
-    )
-    print(delim.join(output) if isinstance(output, list) else output)
-elif args.task == "post":
-    success = post(
-        key=args.key,
-        value=args.value,
-        filename=args.filename,
-        source=args.source,
-        source_type=MetadataSourceType[args.source_type.upper()],
-        is_base64_encoded=args.is_base64_encoded,
-        verbose=args.verbose == 1,
-    )
+elif args.task == "list":
+    for thing in sorted(
+        ["{} : {}".format(this, that) for this, that in inverse_of.items() if this]
+    ):
+        print(thing)
+    success = True
+elif args.task == "search":
+    output = search(args.object_1, args.relation, args.count)
+
+    if args.relation:
+        if args.log:
+            logger.info(f"{len(output):,} {args.item_name}(s): {delim.join(output)}")
+        else:
+            print(delim.join(output))
+    else:
+        print(output)
+
+    success = file.save_json(args.filename, output) if args.filename else True
+elif args.task == "set":
+    success = set_(args.object_1, args.object_2, args.relation)
 else:
     logger.error(f"-{NAME}: {args.task}: command not found.")
 
 if not success:
     logger.error(f"-{NAME}: {args.task}: failed.")
```

### Comparing `abcli-9.26.1/abcli/plugins/metadata/functions.py` & `abcli-9.3.1/abcli/plugins/metadata/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/relations/functions.py` & `abcli-9.3.1/abcli/plugins/relations/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/seed.py` & `abcli-9.3.1/abcli/plugins/seed.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from abcli import NAME
 from abcli import env
 from abcli.logger import logger
 
 
-NAME = f"{NAME}.plugins.seed"
+NAME = "abcli.plugins.seed"
 
 
 def log(
     object_name: str = ".",
     target: str = "open_object",
 ):
     object_name = env.abcli_object_name if object_name == "." else object_name
```

### Comparing `abcli-9.26.1/abcli/plugins/storage/__main__.py` & `abcli-9.3.1/abcli/plugins/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/storage/classes.py` & `abcli-9.3.1/abcli/plugins/storage/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/tags/__main__.py` & `abcli-9.3.1/abcli/plugins/tags/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/tags/functions.py` & `abcli-9.3.1/abcli/plugins/tags/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/plugins/video.py` & `abcli-9.3.1/abcli/plugins/video.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/string/__main__.py` & `abcli-9.3.1/abcli/string/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/string/functions.py` & `abcli-9.3.1/abcli/string/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/table/classes.py` & `abcli-9.3.1/abcli/table/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/tests/test_options.py` & `abcli-9.3.1/abcli/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py` & `abcli-9.3.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/tests/test_plugins_graphics_signature.py` & `abcli-9.3.1/abcli/tests/test_plugins_graphics_signature.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/tests/test_plugins_metadata.py` & `abcli-9.3.1/abcli/tests/test_plugins_metadata.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/tests/test_plugins_testing.py` & `abcli-9.3.1/abcli/tests/test_plugins_testing.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli/timer.py` & `abcli-9.3.1/abcli/timer.py`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/abcli.egg-info/PKG-INFO` & `abcli-9.3.1/abcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abcli
-Version: 9.26.1
+Version: 9.3.1
 Summary: 🚀 a language to speak AI.
 Home-page: https://github.com/kamangir/awesome-bash-cli
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `abcli-9.26.1/abcli.egg-info/SOURCES.txt` & `abcli-9.3.1/abcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abcli-9.26.1/setup.py` & `abcli-9.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from abcli import NAME, VERSION, DESCRIPTION, REPO_NAME
+from abcli import NAME, VERSION, DESCRIPTION
 from blueness.pypi import setup
 
 setup(
     filename=__file__,
-    repo_name=REPO_NAME,
+    repo_name="awesome-bash-cli",
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     packages=[
         NAME,
         f"{NAME}.bash",
         f"{NAME}.file",
```

