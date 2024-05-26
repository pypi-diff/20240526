# Comparing `tmp/abcli-8.227.1.tar.gz` & `tmp/abcli-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abcli-8.227.1.tar", last modified: Sun May 26 03:21:13 2024, max compression
+gzip compressed data, was "abcli-9.2.1.tar", last modified: Sun May 26 04:22:06 2024, max compression
```

## Comparing `abcli-8.227.1.tar` & `abcli-9.2.1.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.857599 abcli-8.227.1/
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:20.000000 abcli-8.227.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     2018 2024-05-26 03:21:13.857028 abcli-8.227.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1117 2024-05-18 22:32:18.000000 abcli-8.227.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.801554 abcli-8.227.1/abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      290 2024-05-26 03:21:08.000000 abcli-8.227.1/abcli/__init__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.806888 abcli-8.227.1/abcli/bash/
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2022-08-19 04:11:13.000000 abcli-8.227.1/abcli/bash/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-04-21 22:44:21.000000 abcli-8.227.1/abcli/bash/colors.py
--rw-r--r--   0 kamangir   (502) staff       (20)      598 2024-02-18 05:10:50.000000 abcli-8.227.1/abcli/bash/help.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2309 2024-04-21 22:45:41.000000 abcli-8.227.1/abcli/bash/list.py
--rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 23:19:04.000000 abcli-8.227.1/abcli/bash/logging.py
--rw-r--r--   0 kamangir   (502) staff       (20)      784 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/elapsed_timer.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5290 2024-04-27 21:10:00.000000 abcli-8.227.1/abcli/env.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.811926 abcli-8.227.1/abcli/file/
--rw-r--r--   0 kamangir   (502) staff       (20)      109 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/file/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      996 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/file/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      570 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/file/classes.py
--rw-r--r--   0 kamangir   (502) staff       (20)     9177 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/file/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6315 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/file/load.py
--rw-r--r--   0 kamangir   (502) staff       (20)     7303 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/file/save.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.814789 abcli-8.227.1/abcli/keywords/
--rw-r--r--   0 kamangir   (502) staff       (20)       84 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/keywords/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      897 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/keywords/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      236 2022-08-20 04:12:52.000000 abcli-8.227.1/abcli/keywords/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1407 2024-04-23 03:10:32.000000 abcli-8.227.1/abcli/keywords/keywords.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1353 2024-04-29 00:44:19.000000 abcli-8.227.1/abcli/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.816068 abcli-8.227.1/abcli/modules/
--rw-r--r--   0 kamangir   (502) staff       (20)       23 2022-08-28 06:57:23.000000 abcli-8.227.1/abcli/modules/__init__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.818271 abcli-8.227.1/abcli/modules/host/
--rw-r--r--   0 kamangir   (502) staff       (20)       90 2022-09-21 00:58:39.000000 abcli-8.227.1/abcli/modules/host/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2523 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/modules/host/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5416 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/modules/host/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2025 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/modules/objects.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.820197 abcli-8.227.1/abcli/options/
--rw-r--r--   0 kamangir   (502) staff       (20)       53 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/options/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1751 2024-05-08 04:06:06.000000 abcli-8.227.1/abcli/options/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2826 2024-05-10 02:13:35.000000 abcli-8.227.1/abcli/options/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.822051 abcli-8.227.1/abcli/path/
--rw-r--r--   0 kamangir   (502) staff       (20)       68 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/path/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/path/consts.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5254 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/path/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.826103 abcli-8.227.1/abcli/plugins/
--rw-r--r--   0 kamangir   (502) staff       (20)       49 2022-08-20 04:12:52.000000 abcli-8.227.1/abcli/plugins/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      916 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/__main__.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.827530 abcli-8.227.1/abcli/plugins/cache/
--rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-8.227.1/abcli/plugins/cache/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1646 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/cache/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4705 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/cache/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      705 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.829225 abcli-8.227.1/abcli/plugins/git/
--rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-20 04:27:12.000000 abcli-8.227.1/abcli/plugins/git/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      696 2024-05-20 04:26:24.000000 abcli-8.227.1/abcli/plugins/git/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1716 2024-05-20 04:27:32.000000 abcli-8.227.1/abcli/plugins/git/version.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.830743 abcli-8.227.1/abcli/plugins/gpu/
--rw-r--r--   0 kamangir   (502) staff       (20)       52 2022-08-20 04:12:52.000000 abcli-8.227.1/abcli/plugins/gpu/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      499 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/gpu/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      590 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/gpu/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.835462 abcli-8.227.1/abcli/plugins/graphics/
--rw-r--r--   0 kamangir   (502) staff       (20)      124 2022-09-25 02:29:01.000000 abcli-8.227.1/abcli/plugins/graphics/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1462 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/graphics/constants.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1740 2024-05-08 02:05:01.000000 abcli-8.227.1/abcli/plugins/graphics/gif.py
--rw-r--r--   0 kamangir   (502) staff       (20)      431 2022-08-14 18:15:57.000000 abcli-8.227.1/abcli/plugins/graphics/image.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/graphics/signature.py
--rw-r--r--   0 kamangir   (502) staff       (20)     6641 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/graphics/text.py
--rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/markdown.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.838212 abcli-8.227.1/abcli/plugins/metadata/
--rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/metadata/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2109 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/metadata/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2231 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/metadata/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.840799 abcli-8.227.1/abcli/plugins/relations/
--rw-r--r--   0 kamangir   (502) staff       (20)       59 2022-08-20 04:12:52.000000 abcli-8.227.1/abcli/plugins/relations/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2102 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/relations/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5157 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/relations/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      680 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/seed.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.843300 abcli-8.227.1/abcli/plugins/storage/
--rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/storage/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2248 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/storage/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     8063 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/storage/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.845700 abcli-8.227.1/abcli/plugins/tags/
--rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-8.227.1/abcli/plugins/tags/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2219 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/tags/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     5991 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/tags/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)      344 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/testing.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1313 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/plugins/video.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.849066 abcli-8.227.1/abcli/string/
--rw-r--r--   0 kamangir   (502) staff       (20)      244 2024-02-18 05:23:47.000000 abcli-8.227.1/abcli/string/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1138 2024-02-18 05:23:40.000000 abcli-8.227.1/abcli/string/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-02-18 05:23:45.000000 abcli-8.227.1/abcli/string/constants.py
--rw-r--r--   0 kamangir   (502) staff       (20)    11283 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/string/functions.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.850619 abcli-8.227.1/abcli/table/
--rw-r--r--   0 kamangir   (502) staff       (20)       45 2022-08-20 04:12:52.000000 abcli-8.227.1/abcli/table/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4541 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/table/classes.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.855829 abcli-8.227.1/abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/tests/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       69 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/tests/test_abcli.py
--rw-r--r--   0 kamangir   (502) staff       (20)      275 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/tests/test_env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      410 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/tests/test_modules_objects.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3194 2024-05-10 02:20:04.000000 abcli-8.227.1/abcli/tests/test_options.py
--rw-r--r--   0 kamangir   (502) staff       (20)      634 2024-05-08 02:13:37.000000 abcli-8.227.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/tests/test_plugins_graphics_signature.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2831 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/tests/test_plugins_metadata.py
--rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/tests/test_plugins_testing.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2199 2024-04-21 00:00:57.000000 abcli-8.227.1/abcli/timer.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 03:21:13.856409 abcli-8.227.1/abcli.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     2018 2024-05-26 03:21:13.000000 abcli-8.227.1/abcli.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     2473 2024-05-26 03:21:13.000000 abcli-8.227.1/abcli.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 03:21:13.000000 abcli-8.227.1/abcli.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-26 03:21:13.000000 abcli-8.227.1/abcli.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-26 03:21:13.000000 abcli-8.227.1/abcli.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 03:28:20.000000 abcli-8.227.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      124 2024-05-20 22:39:16.000000 abcli-8.227.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 03:21:13.857718 abcli-8.227.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      861 2024-05-21 04:09:10.000000 abcli-8.227.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:06.004480 abcli-9.2.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:20.000000 abcli-9.2.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     2016 2024-05-26 04:22:06.004080 abcli-9.2.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1117 2024-05-18 22:32:18.000000 abcli-9.2.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.943759 abcli-9.2.1/abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      288 2024-05-26 04:22:01.000000 abcli-9.2.1/abcli/__init__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.949667 abcli-9.2.1/abcli/bash/
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2022-08-19 04:11:13.000000 abcli-9.2.1/abcli/bash/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-04-21 22:44:21.000000 abcli-9.2.1/abcli/bash/colors.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      598 2024-02-18 05:10:50.000000 abcli-9.2.1/abcli/bash/help.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2309 2024-04-21 22:45:41.000000 abcli-9.2.1/abcli/bash/list.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 23:19:04.000000 abcli-9.2.1/abcli/bash/logging.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      784 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/elapsed_timer.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5290 2024-04-27 21:10:00.000000 abcli-9.2.1/abcli/env.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.953857 abcli-9.2.1/abcli/file/
+-rw-r--r--   0 kamangir   (502) staff       (20)      109 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/file/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      996 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/file/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      570 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/file/classes.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     9177 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/file/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6315 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/file/load.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     7303 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/file/save.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.956937 abcli-9.2.1/abcli/keywords/
+-rw-r--r--   0 kamangir   (502) staff       (20)       84 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/keywords/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      897 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/keywords/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      236 2022-08-20 04:12:52.000000 abcli-9.2.1/abcli/keywords/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1407 2024-04-23 03:10:32.000000 abcli-9.2.1/abcli/keywords/keywords.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1353 2024-04-29 00:44:19.000000 abcli-9.2.1/abcli/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.958503 abcli-9.2.1/abcli/modules/
+-rw-r--r--   0 kamangir   (502) staff       (20)       23 2022-08-28 06:57:23.000000 abcli-9.2.1/abcli/modules/__init__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.961072 abcli-9.2.1/abcli/modules/host/
+-rw-r--r--   0 kamangir   (502) staff       (20)       90 2022-09-21 00:58:39.000000 abcli-9.2.1/abcli/modules/host/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2523 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/modules/host/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5416 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/modules/host/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2025 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/modules/objects.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.963266 abcli-9.2.1/abcli/options/
+-rw-r--r--   0 kamangir   (502) staff       (20)       53 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/options/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1751 2024-05-08 04:06:06.000000 abcli-9.2.1/abcli/options/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2826 2024-05-10 02:13:35.000000 abcli-9.2.1/abcli/options/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.965126 abcli-9.2.1/abcli/path/
+-rw-r--r--   0 kamangir   (502) staff       (20)       68 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/path/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       10 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/path/consts.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5254 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/path/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.969394 abcli-9.2.1/abcli/plugins/
+-rw-r--r--   0 kamangir   (502) staff       (20)       49 2022-08-20 04:12:52.000000 abcli-9.2.1/abcli/plugins/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      916 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/__main__.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.971471 abcli-9.2.1/abcli/plugins/cache/
+-rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.2.1/abcli/plugins/cache/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1646 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/cache/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4705 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/cache/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      524 2024-05-26 04:21:10.000000 abcli-9.2.1/abcli/plugins/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.973649 abcli-9.2.1/abcli/plugins/git/
+-rw-r--r--   0 kamangir   (502) staff       (20)       26 2024-05-20 04:27:12.000000 abcli-9.2.1/abcli/plugins/git/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      696 2024-05-20 04:26:24.000000 abcli-9.2.1/abcli/plugins/git/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1716 2024-05-20 04:27:32.000000 abcli-9.2.1/abcli/plugins/git/version.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.975705 abcli-9.2.1/abcli/plugins/gpu/
+-rw-r--r--   0 kamangir   (502) staff       (20)       52 2022-08-20 04:12:52.000000 abcli-9.2.1/abcli/plugins/gpu/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      499 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/gpu/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      590 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/gpu/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.980935 abcli-9.2.1/abcli/plugins/graphics/
+-rw-r--r--   0 kamangir   (502) staff       (20)      124 2022-09-25 02:29:01.000000 abcli-9.2.1/abcli/plugins/graphics/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1462 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/graphics/constants.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1740 2024-05-08 02:05:01.000000 abcli-9.2.1/abcli/plugins/graphics/gif.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      431 2022-08-14 18:15:57.000000 abcli-9.2.1/abcli/plugins/graphics/image.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3591 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/graphics/signature.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     6641 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/graphics/text.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      953 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/markdown.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.983512 abcli-9.2.1/abcli/plugins/metadata/
+-rw-r--r--   0 kamangir   (502) staff       (20)       58 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/metadata/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2109 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/metadata/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2231 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/metadata/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.985948 abcli-9.2.1/abcli/plugins/relations/
+-rw-r--r--   0 kamangir   (502) staff       (20)       59 2022-08-20 04:12:52.000000 abcli-9.2.1/abcli/plugins/relations/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2102 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/relations/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5157 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/relations/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      680 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/seed.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.988321 abcli-9.2.1/abcli/plugins/storage/
+-rw-r--r--   0 kamangir   (502) staff       (20)       83 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/storage/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2248 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/storage/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     8063 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/storage/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.990670 abcli-9.2.1/abcli/plugins/tags/
+-rw-r--r--   0 kamangir   (502) staff       (20)       55 2022-08-20 04:12:52.000000 abcli-9.2.1/abcli/plugins/tags/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2219 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/tags/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     5991 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/tags/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      344 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/testing.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1313 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/plugins/video.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.993782 abcli-9.2.1/abcli/string/
+-rw-r--r--   0 kamangir   (502) staff       (20)      244 2024-02-18 05:23:47.000000 abcli-9.2.1/abcli/string/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1138 2024-02-18 05:23:40.000000 abcli-9.2.1/abcli/string/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      216 2024-02-18 05:23:45.000000 abcli-9.2.1/abcli/string/constants.py
+-rw-r--r--   0 kamangir   (502) staff       (20)    11283 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/string/functions.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:05.995158 abcli-9.2.1/abcli/table/
+-rw-r--r--   0 kamangir   (502) staff       (20)       45 2022-08-20 04:12:52.000000 abcli-9.2.1/abcli/table/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4541 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/table/classes.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:06.002812 abcli-9.2.1/abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)        0 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/tests/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       69 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/tests/test_abcli.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      275 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/tests/test_env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      410 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/tests/test_modules_objects.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3194 2024-05-10 02:20:04.000000 abcli-9.2.1/abcli/tests/test_options.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      104 2024-05-26 04:20:33.000000 abcli-9.2.1/abcli/tests/test_plugins.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      634 2024-05-08 02:13:37.000000 abcli-9.2.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1037 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/tests/test_plugins_graphics_signature.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2831 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/tests/test_plugins_metadata.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      777 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/tests/test_plugins_testing.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2199 2024-04-21 00:00:57.000000 abcli-9.2.1/abcli/timer.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 04:22:06.003523 abcli-9.2.1/abcli.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     2016 2024-05-26 04:22:05.000000 abcli-9.2.1/abcli.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     2501 2024-05-26 04:22:05.000000 abcli-9.2.1/abcli.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 04:22:05.000000 abcli-9.2.1/abcli.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-26 04:22:05.000000 abcli-9.2.1/abcli.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-26 04:22:05.000000 abcli-9.2.1/abcli.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 03:28:20.000000 abcli-9.2.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      124 2024-05-20 22:39:16.000000 abcli-9.2.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 04:22:06.004591 abcli-9.2.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      861 2024-05-21 04:09:10.000000 abcli-9.2.1/setup.py
```

### Comparing `abcli-8.227.1/PKG-INFO` & `abcli-9.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abcli
-Version: 8.227.1
+Version: 9.2.1
 Summary: 🚀 a language to speak AI.
 Home-page: https://github.com/kamangir/awesome-bash-cli
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `abcli-8.227.1/README.md` & `abcli-9.2.1/README.md`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/bash/help.py` & `abcli-9.2.1/abcli/bash/help.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/bash/list.py` & `abcli-9.2.1/abcli/bash/list.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/bash/logging.py` & `abcli-9.2.1/abcli/bash/logging.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/config.env` & `abcli-9.2.1/abcli/config.env`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/elapsed_timer.py` & `abcli-9.2.1/abcli/elapsed_timer.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/env.py` & `abcli-9.2.1/abcli/env.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/file/__main__.py` & `abcli-9.2.1/abcli/file/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/file/classes.py` & `abcli-9.2.1/abcli/file/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/file/functions.py` & `abcli-9.2.1/abcli/file/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/file/load.py` & `abcli-9.2.1/abcli/file/load.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/file/save.py` & `abcli-9.2.1/abcli/file/save.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/keywords/__main__.py` & `abcli-9.2.1/abcli/keywords/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/keywords/keywords.py` & `abcli-9.2.1/abcli/keywords/keywords.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/logger.py` & `abcli-9.2.1/abcli/logger.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/modules/host/__main__.py` & `abcli-9.2.1/abcli/modules/host/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/modules/host/functions.py` & `abcli-9.2.1/abcli/modules/host/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/modules/objects.py` & `abcli-9.2.1/abcli/modules/objects.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/options/__main__.py` & `abcli-9.2.1/abcli/options/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/options/classes.py` & `abcli-9.2.1/abcli/options/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/path/functions.py` & `abcli-9.2.1/abcli/path/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/__main__.py` & `abcli-9.2.1/abcli/plugins/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/cache/__main__.py` & `abcli-9.2.1/abcli/plugins/cache/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/cache/functions.py` & `abcli-9.2.1/abcli/plugins/cache/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/git/__main__.py` & `abcli-9.2.1/abcli/plugins/git/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/git/version.py` & `abcli-9.2.1/abcli/plugins/git/version.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/gpu/functions.py` & `abcli-9.2.1/abcli/plugins/gpu/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/graphics/constants.py` & `abcli-9.2.1/abcli/plugins/graphics/constants.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/graphics/gif.py` & `abcli-9.2.1/abcli/plugins/graphics/gif.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/graphics/signature.py` & `abcli-9.2.1/abcli/plugins/graphics/signature.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/graphics/text.py` & `abcli-9.2.1/abcli/plugins/graphics/text.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/markdown.py` & `abcli-9.2.1/abcli/plugins/markdown.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/metadata/__main__.py` & `abcli-9.2.1/abcli/plugins/metadata/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/metadata/functions.py` & `abcli-9.2.1/abcli/plugins/metadata/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/relations/__main__.py` & `abcli-9.2.1/abcli/plugins/relations/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/relations/functions.py` & `abcli-9.2.1/abcli/plugins/relations/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/seed.py` & `abcli-9.2.1/abcli/plugins/seed.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/storage/__main__.py` & `abcli-9.2.1/abcli/plugins/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/storage/classes.py` & `abcli-9.2.1/abcli/plugins/storage/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/tags/__main__.py` & `abcli-9.2.1/abcli/plugins/tags/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/tags/functions.py` & `abcli-9.2.1/abcli/plugins/tags/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/plugins/video.py` & `abcli-9.2.1/abcli/plugins/video.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/string/__main__.py` & `abcli-9.2.1/abcli/string/__main__.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/string/functions.py` & `abcli-9.2.1/abcli/string/functions.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/table/classes.py` & `abcli-9.2.1/abcli/table/classes.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/tests/test_options.py` & `abcli-9.2.1/abcli/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py` & `abcli-9.2.1/abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/tests/test_plugins_graphics_signature.py` & `abcli-9.2.1/abcli/tests/test_plugins_graphics_signature.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/tests/test_plugins_metadata.py` & `abcli-9.2.1/abcli/tests/test_plugins_metadata.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/tests/test_plugins_testing.py` & `abcli-9.2.1/abcli/tests/test_plugins_testing.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli/timer.py` & `abcli-9.2.1/abcli/timer.py`

 * *Files identical despite different names*

### Comparing `abcli-8.227.1/abcli.egg-info/PKG-INFO` & `abcli-9.2.1/abcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abcli
-Version: 8.227.1
+Version: 9.2.1
 Summary: 🚀 a language to speak AI.
 Home-page: https://github.com/kamangir/awesome-bash-cli
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `abcli-8.227.1/abcli.egg-info/SOURCES.txt` & `abcli-9.2.1/abcli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,11 +81,12 @@
 abcli/table/__init__.py
 abcli/table/classes.py
 abcli/tests/__init__.py
 abcli/tests/test_abcli.py
 abcli/tests/test_env.py
 abcli/tests/test_modules_objects.py
 abcli/tests/test_options.py
+abcli/tests/test_plugins.py
 abcli/tests/test_plugins_graphics_gif_generate_animated_gif.py
 abcli/tests/test_plugins_graphics_signature.py
 abcli/tests/test_plugins_metadata.py
 abcli/tests/test_plugins_testing.py
```

### Comparing `abcli-8.227.1/setup.py` & `abcli-9.2.1/setup.py`

 * *Files identical despite different names*

