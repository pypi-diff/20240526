# Comparing `tmp/slack-machine-0.8.tar.gz` & `tmp/slack-machine-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/slack-machine-0.8.tar", last modified: Sun Oct 15 20:31:05 2017, max compression
+gzip compressed data, was "dist/slack-machine-0.9.tar", last modified: Sun Dec  3 18:28:09 2017, max compression
```

## Comparing `slack-machine-0.8.tar` & `slack-machine-0.9.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/extra/
--rw-r--r--   0 daan       (501) staff       (20)    46959 2017-08-24 19:31:28.000000 slack-machine-0.8/extra/logo.png
--rw-r--r--   0 daan       (501) staff       (20)     1066 2017-08-24 19:33:55.000000 slack-machine-0.8/LICENSE
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/machine/
--rw-r--r--   0 daan       (501) staff       (20)      511 2017-10-15 20:28:02.000000 slack-machine-0.8/machine/__about__.py
--rw-r--r--   0 daan       (501) staff       (20)      325 2017-08-24 21:38:41.000000 slack-machine-0.8/machine/__init__.py
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/machine/bin/
--rw-r--r--   0 daan       (501) staff       (20)        0 2017-08-24 20:34:36.000000 slack-machine-0.8/machine/bin/__init__.py
--rw-r--r--   0 daan       (501) staff       (20)      383 2017-09-15 13:33:09.000000 slack-machine-0.8/machine/bin/run.py
--rw-r--r--   0 daan       (501) staff       (20)     4511 2017-10-13 13:37:05.000000 slack-machine-0.8/machine/core.py
--rw-r--r--   0 daan       (501) staff       (20)     3132 2017-09-15 14:04:23.000000 slack-machine-0.8/machine/dispatch.py
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/machine/plugins/
--rw-r--r--   0 daan       (501) staff       (20)        0 2017-08-14 21:07:30.000000 slack-machine-0.8/machine/plugins/__init__.py
--rw-r--r--   0 daan       (501) staff       (20)    20475 2017-10-15 20:20:25.000000 slack-machine-0.8/machine/plugins/base.py
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/machine/plugins/builtin/
--rw-r--r--   0 daan       (501) staff       (20)        0 2017-08-20 19:18:25.000000 slack-machine-0.8/machine/plugins/builtin/__init__.py
--rw-r--r--   0 daan       (501) staff       (20)      498 2017-10-15 19:05:56.000000 slack-machine-0.8/machine/plugins/builtin/debug.py
--rw-r--r--   0 daan       (501) staff       (20)      735 2017-09-15 11:06:26.000000 slack-machine-0.8/machine/plugins/builtin/general.py
--rw-r--r--   0 daan       (501) staff       (20)     6400 2017-10-15 20:30:02.000000 slack-machine-0.8/machine/plugins/decorators.py
--rw-r--r--   0 daan       (501) staff       (20)      975 2017-09-10 13:08:47.000000 slack-machine-0.8/machine/settings.py
--rw-r--r--   0 daan       (501) staff       (20)     1464 2017-10-13 13:54:45.000000 slack-machine-0.8/machine/singletons.py
--rw-r--r--   0 daan       (501) staff       (20)     3254 2017-09-20 17:24:20.000000 slack-machine-0.8/machine/slack.py
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/machine/storage/
--rw-r--r--   0 daan       (501) staff       (20)     3780 2017-10-13 13:03:29.000000 slack-machine-0.8/machine/storage/__init__.py
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/machine/storage/backends/
--rw-r--r--   0 daan       (501) staff       (20)        0 2017-09-10 12:32:47.000000 slack-machine-0.8/machine/storage/backends/__init__.py
--rw-r--r--   0 daan       (501) staff       (20)     1729 2017-09-13 20:12:12.000000 slack-machine-0.8/machine/storage/backends/base.py
--rw-r--r--   0 daan       (501) staff       (20)     1245 2017-09-10 13:17:59.000000 slack-machine-0.8/machine/storage/backends/memory.py
--rw-r--r--   0 daan       (501) staff       (20)      928 2017-09-15 11:26:46.000000 slack-machine-0.8/machine/storage/backends/redis.py
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/machine/utils/
--rw-r--r--   0 daan       (501) staff       (20)      487 2017-09-15 13:40:09.000000 slack-machine-0.8/machine/utils/__init__.py
--rw-r--r--   0 daan       (501) staff       (20)     2589 2017-08-20 19:03:47.000000 slack-machine-0.8/machine/utils/collections.py
--rw-r--r--   0 daan       (501) staff       (20)      914 2017-10-13 12:29:12.000000 slack-machine-0.8/machine/utils/module_loading.py
--rw-r--r--   0 daan       (501) staff       (20)     1301 2017-08-29 19:03:18.000000 slack-machine-0.8/machine/utils/pool.py
--rw-r--r--   0 daan       (501) staff       (20)      450 2017-09-15 11:35:14.000000 slack-machine-0.8/machine/utils/redis.py
--rw-r--r--   0 daan       (501) staff       (20)      111 2017-08-24 21:57:52.000000 slack-machine-0.8/MANIFEST.in
--rw-r--r--   0 daan       (501) staff       (20)     4802 2017-10-15 20:31:05.000000 slack-machine-0.8/PKG-INFO
--rw-r--r--   0 daan       (501) staff       (20)     3121 2017-10-15 20:26:56.000000 slack-machine-0.8/README.rst
--rw-r--r--   0 daan       (501) staff       (20)       68 2017-10-15 15:13:13.000000 slack-machine-0.8/requirements.txt
--rw-r--r--   0 daan       (501) staff       (20)       72 2017-08-24 20:38:41.000000 slack-machine-0.8/run_dev.py
--rw-r--r--   0 daan       (501) staff       (20)      278 2017-10-15 20:31:05.000000 slack-machine-0.8/setup.cfg
--rw-r--r--   0 daan       (501) staff       (20)     3159 2017-09-12 18:10:52.000000 slack-machine-0.8/setup.py
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/slack_machine.egg-info/
--rw-r--r--   0 daan       (501) staff       (20)        1 2017-10-15 20:31:05.000000 slack-machine-0.8/slack_machine.egg-info/dependency_links.txt
--rw-r--r--   0 daan       (501) staff       (20)       56 2017-10-15 20:31:05.000000 slack-machine-0.8/slack_machine.egg-info/entry_points.txt
--rw-r--r--   0 daan       (501) staff       (20)        1 2017-08-29 20:01:02.000000 slack-machine-0.8/slack_machine.egg-info/not-zip-safe
--rw-r--r--   0 daan       (501) staff       (20)     4802 2017-10-15 20:31:05.000000 slack-machine-0.8/slack_machine.egg-info/PKG-INFO
--rw-r--r--   0 daan       (501) staff       (20)       92 2017-10-15 20:31:05.000000 slack-machine-0.8/slack_machine.egg-info/requires.txt
--rw-r--r--   0 daan       (501) staff       (20)     1373 2017-10-15 20:31:05.000000 slack-machine-0.8/slack_machine.egg-info/SOURCES.txt
--rw-r--r--   0 daan       (501) staff       (20)       14 2017-10-15 20:31:05.000000 slack-machine-0.8/slack_machine.egg-info/top_level.txt
-drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-10-15 20:31:05.000000 slack-machine-0.8/tests/
--rw-r--r--   0 daan       (501) staff       (20)        0 2017-09-01 08:21:06.000000 slack-machine-0.8/tests/__init__.py
--rw-r--r--   0 daan       (501) staff       (20)       75 2017-10-13 13:58:08.000000 slack-machine-0.8/tests/fake_classes.py
--rw-r--r--   0 daan       (501) staff       (20)      473 2017-09-09 19:17:27.000000 slack-machine-0.8/tests/fake_plugins.py
--rw-r--r--   0 daan       (501) staff       (20)       93 2017-09-09 16:33:48.000000 slack-machine-0.8/tests/local_test_settings.py
--rw-r--r--   0 daan       (501) staff       (20)       87 2017-10-13 13:58:47.000000 slack-machine-0.8/tests/singletons.py
--rw-r--r--   0 daan       (501) staff       (20)     2816 2017-10-15 19:56:08.000000 slack-machine-0.8/tests/test_decorators.py
--rw-r--r--   0 daan       (501) staff       (20)     5804 2017-09-15 14:08:39.000000 slack-machine-0.8/tests/test_dispatch.py
--rw-r--r--   0 daan       (501) staff       (20)     1537 2017-09-09 16:47:42.000000 slack-machine-0.8/tests/test_import_settings.py
--rw-r--r--   0 daan       (501) staff       (20)     1484 2017-10-13 12:30:33.000000 slack-machine-0.8/tests/test_import_string.py
--rw-r--r--   0 daan       (501) staff       (20)     1583 2017-09-10 13:01:10.000000 slack-machine-0.8/tests/test_memory_storage.py
--rw-r--r--   0 daan       (501) staff       (20)     2754 2017-10-13 12:37:12.000000 slack-machine-0.8/tests/test_plugin_registration.py
--rw-r--r--   0 daan       (501) staff       (20)     1696 2017-10-13 13:10:43.000000 slack-machine-0.8/tests/test_plugin_storage.py
--rw-r--r--   0 daan       (501) staff       (20)     1260 2017-09-12 19:34:38.000000 slack-machine-0.8/tests/test_redis_storage.py
--rw-r--r--   0 daan       (501) staff       (20)      313 2017-10-13 14:01:19.000000 slack-machine-0.8/tests/test_utils.py
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/extra/
+-rw-r--r--   0 daan       (501) staff       (20)    46959 2017-08-24 19:31:28.000000 slack-machine-0.9/extra/logo.png
+-rw-r--r--   0 daan       (501) staff       (20)     1066 2017-08-24 19:33:55.000000 slack-machine-0.9/LICENSE
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/machine/
+-rw-r--r--   0 daan       (501) staff       (20)      511 2017-12-03 18:26:47.000000 slack-machine-0.9/machine/__about__.py
+-rw-r--r--   0 daan       (501) staff       (20)      325 2017-08-24 21:38:41.000000 slack-machine-0.9/machine/__init__.py
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/machine/bin/
+-rw-r--r--   0 daan       (501) staff       (20)        0 2017-08-24 20:34:36.000000 slack-machine-0.9/machine/bin/__init__.py
+-rw-r--r--   0 daan       (501) staff       (20)      426 2017-12-03 17:23:30.000000 slack-machine-0.9/machine/bin/run.py
+-rw-r--r--   0 daan       (501) staff       (20)     5211 2017-12-03 18:25:34.000000 slack-machine-0.9/machine/core.py
+-rw-r--r--   0 daan       (501) staff       (20)     3132 2017-09-15 14:04:23.000000 slack-machine-0.9/machine/dispatch.py
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/machine/plugins/
+-rw-r--r--   0 daan       (501) staff       (20)        0 2017-08-14 21:07:30.000000 slack-machine-0.9/machine/plugins/__init__.py
+-rw-r--r--   0 daan       (501) staff       (20)    22463 2017-12-03 15:28:16.000000 slack-machine-0.9/machine/plugins/base.py
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/machine/plugins/builtin/
+-rw-r--r--   0 daan       (501) staff       (20)        0 2017-08-20 19:18:25.000000 slack-machine-0.9/machine/plugins/builtin/__init__.py
+-rw-r--r--   0 daan       (501) staff       (20)      498 2017-10-15 19:05:56.000000 slack-machine-0.9/machine/plugins/builtin/debug.py
+-rw-r--r--   0 daan       (501) staff       (20)      735 2017-09-15 11:06:26.000000 slack-machine-0.9/machine/plugins/builtin/general.py
+-rw-r--r--   0 daan       (501) staff       (20)     6400 2017-10-15 20:30:02.000000 slack-machine-0.9/machine/plugins/decorators.py
+-rw-r--r--   0 daan       (501) staff       (20)      975 2017-09-10 13:08:47.000000 slack-machine-0.9/machine/settings.py
+-rw-r--r--   0 daan       (501) staff       (20)     1464 2017-10-13 13:54:45.000000 slack-machine-0.9/machine/singletons.py
+-rw-r--r--   0 daan       (501) staff       (20)     3284 2017-12-03 15:28:16.000000 slack-machine-0.9/machine/slack.py
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/machine/storage/
+-rw-r--r--   0 daan       (501) staff       (20)     3780 2017-10-13 13:03:29.000000 slack-machine-0.9/machine/storage/__init__.py
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/machine/storage/backends/
+-rw-r--r--   0 daan       (501) staff       (20)        0 2017-09-10 12:32:47.000000 slack-machine-0.9/machine/storage/backends/__init__.py
+-rw-r--r--   0 daan       (501) staff       (20)     1729 2017-09-13 20:12:12.000000 slack-machine-0.9/machine/storage/backends/base.py
+-rw-r--r--   0 daan       (501) staff       (20)     1245 2017-09-10 13:17:59.000000 slack-machine-0.9/machine/storage/backends/memory.py
+-rw-r--r--   0 daan       (501) staff       (20)      928 2017-09-15 11:26:46.000000 slack-machine-0.9/machine/storage/backends/redis.py
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/machine/utils/
+-rw-r--r--   0 daan       (501) staff       (20)      487 2017-09-15 13:40:09.000000 slack-machine-0.9/machine/utils/__init__.py
+-rw-r--r--   0 daan       (501) staff       (20)     2589 2017-08-20 19:03:47.000000 slack-machine-0.9/machine/utils/collections.py
+-rw-r--r--   0 daan       (501) staff       (20)      914 2017-10-13 12:29:12.000000 slack-machine-0.9/machine/utils/module_loading.py
+-rw-r--r--   0 daan       (501) staff       (20)     1301 2017-08-29 19:03:18.000000 slack-machine-0.9/machine/utils/pool.py
+-rw-r--r--   0 daan       (501) staff       (20)      450 2017-09-15 11:35:14.000000 slack-machine-0.9/machine/utils/redis.py
+-rw-r--r--   0 daan       (501) staff       (20)      398 2017-12-03 18:25:52.000000 slack-machine-0.9/machine/utils/text.py
+-rw-r--r--   0 daan       (501) staff       (20)      111 2017-08-24 21:57:52.000000 slack-machine-0.9/MANIFEST.in
+-rw-r--r--   0 daan       (501) staff       (20)     4752 2017-12-03 18:28:09.000000 slack-machine-0.9/PKG-INFO
+-rw-r--r--   0 daan       (501) staff       (20)     3121 2017-10-15 20:26:56.000000 slack-machine-0.9/README.rst
+-rw-r--r--   0 daan       (501) staff       (20)       81 2017-12-03 16:30:41.000000 slack-machine-0.9/requirements.txt
+-rw-r--r--   0 daan       (501) staff       (20)       72 2017-08-24 20:38:41.000000 slack-machine-0.9/run_dev.py
+-rw-r--r--   0 daan       (501) staff       (20)      278 2017-12-03 18:28:09.000000 slack-machine-0.9/setup.cfg
+-rw-r--r--   0 daan       (501) staff       (20)     3110 2017-12-03 15:09:59.000000 slack-machine-0.9/setup.py
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/slack_machine.egg-info/
+-rw-r--r--   0 daan       (501) staff       (20)        1 2017-12-03 18:28:09.000000 slack-machine-0.9/slack_machine.egg-info/dependency_links.txt
+-rw-r--r--   0 daan       (501) staff       (20)       56 2017-12-03 18:28:09.000000 slack-machine-0.9/slack_machine.egg-info/entry_points.txt
+-rw-r--r--   0 daan       (501) staff       (20)        1 2017-08-29 20:01:02.000000 slack-machine-0.9/slack_machine.egg-info/not-zip-safe
+-rw-r--r--   0 daan       (501) staff       (20)     4752 2017-12-03 18:28:09.000000 slack-machine-0.9/slack_machine.egg-info/PKG-INFO
+-rw-r--r--   0 daan       (501) staff       (20)      105 2017-12-03 18:28:09.000000 slack-machine-0.9/slack_machine.egg-info/requires.txt
+-rw-r--r--   0 daan       (501) staff       (20)     1395 2017-12-03 18:28:09.000000 slack-machine-0.9/slack_machine.egg-info/SOURCES.txt
+-rw-r--r--   0 daan       (501) staff       (20)       14 2017-12-03 18:28:09.000000 slack-machine-0.9/slack_machine.egg-info/top_level.txt
+drwxr-xr-x   0 daan       (501) staff       (20)        0 2017-12-03 18:28:09.000000 slack-machine-0.9/tests/
+-rw-r--r--   0 daan       (501) staff       (20)        0 2017-09-01 08:21:06.000000 slack-machine-0.9/tests/__init__.py
+-rw-r--r--   0 daan       (501) staff       (20)       75 2017-10-13 13:58:08.000000 slack-machine-0.9/tests/fake_classes.py
+-rw-r--r--   0 daan       (501) staff       (20)      473 2017-09-09 19:17:27.000000 slack-machine-0.9/tests/fake_plugins.py
+-rw-r--r--   0 daan       (501) staff       (20)       93 2017-09-09 16:33:48.000000 slack-machine-0.9/tests/local_test_settings.py
+-rw-r--r--   0 daan       (501) staff       (20)       87 2017-10-13 13:58:47.000000 slack-machine-0.9/tests/singletons.py
+-rw-r--r--   0 daan       (501) staff       (20)     2816 2017-10-15 19:56:08.000000 slack-machine-0.9/tests/test_decorators.py
+-rw-r--r--   0 daan       (501) staff       (20)     5804 2017-09-15 14:08:39.000000 slack-machine-0.9/tests/test_dispatch.py
+-rw-r--r--   0 daan       (501) staff       (20)     1537 2017-09-09 16:47:42.000000 slack-machine-0.9/tests/test_import_settings.py
+-rw-r--r--   0 daan       (501) staff       (20)     1484 2017-10-13 12:30:33.000000 slack-machine-0.9/tests/test_import_string.py
+-rw-r--r--   0 daan       (501) staff       (20)     1583 2017-09-10 13:01:10.000000 slack-machine-0.9/tests/test_memory_storage.py
+-rw-r--r--   0 daan       (501) staff       (20)     2754 2017-10-13 12:37:12.000000 slack-machine-0.9/tests/test_plugin_registration.py
+-rw-r--r--   0 daan       (501) staff       (20)     1696 2017-10-13 13:10:43.000000 slack-machine-0.9/tests/test_plugin_storage.py
+-rw-r--r--   0 daan       (501) staff       (20)     1260 2017-09-12 19:34:38.000000 slack-machine-0.9/tests/test_redis_storage.py
+-rw-r--r--   0 daan       (501) staff       (20)      313 2017-10-13 14:01:19.000000 slack-machine-0.9/tests/test_utils.py
```

### Comparing `slack-machine-0.8/extra/logo.png` & `slack-machine-0.9/extra/logo.png`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/LICENSE` & `slack-machine-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/core.py` & `slack-machine-0.9/machine/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,77 @@
 import sys
 import inspect
 import logging
+
+from clint.textui import puts, indent
 from machine.settings import import_settings
 from machine.singletons import Slack, Scheduler, Storage
 from machine.storage import PluginStorage
 from machine.utils.module_loading import import_string
 from machine.plugins.base import MachineBasePlugin
 from machine.dispatch import EventDispatcher
 from machine.slack import MessagingClient
+from machine.utils.text import show_valid, warn, error, announce
 
 logger = logging.getLogger(__name__)
 
 
 class Machine:
     def __init__(self, settings=None):
-        if settings:
-            self._settings = settings
-            found_local_settings = True
-        else:
-            self._settings, found_local_settings = import_settings()
-        fmt = '[%(asctime)s][%(levelname)s] %(name)s %(filename)s:%(funcName)s:%(lineno)d |' \
-              ' %(message)s'
-        date_fmt = '%Y-%m-%d %H:%M:%S'
-        log_level = self._settings.get('LOGLEVEL', logging.ERROR)
-        logging.basicConfig(
-            level=log_level,
-            format=fmt,
-            datefmt=date_fmt,
-        )
-        if not found_local_settings:
-            logger.warning("No local_settings found! Are you sure this is what you want?")
-        if 'SLACK_API_TOKEN' not in self._settings:
-            logger.error("No SLACK_API_TOKEN found in settings! I need that to work...")
-            sys.exit(1)
-        self._client = Slack()
-        logger.debug("Initializing storage '%s'...", self._settings['STORAGE_BACKEND'])
-        self._storage = Storage.get_instance()
-        logger.debug("Storage initialized!")
-        self._plugin_actions = {
-            'process': {},
-            'listen_to': {},
-            'respond_to': {},
-            'catch_all': {}
-        }
-        self.load_plugins()
-        logger.debug("The following plugin actions were registered: %s", self._plugin_actions)
-        self._dispatcher = EventDispatcher(self._plugin_actions)
+        announce("Initializing Slack Machine:")
+
+        with indent(4):
+            puts("Loading settings...")
+            if settings:
+                self._settings = settings
+                found_local_settings = True
+            else:
+                self._settings, found_local_settings = import_settings()
+            fmt = '[%(asctime)s][%(levelname)s] %(name)s %(filename)s:%(funcName)s:%(lineno)d |' \
+                  ' %(message)s'
+            date_fmt = '%Y-%m-%d %H:%M:%S'
+            log_level = self._settings.get('LOGLEVEL', logging.ERROR)
+            logging.basicConfig(
+                level=log_level,
+                format=fmt,
+                datefmt=date_fmt,
+            )
+            if not found_local_settings:
+                warn("No local_settings found! Are you sure this is what you want?")
+            if 'SLACK_API_TOKEN' not in self._settings:
+                error("No SLACK_API_TOKEN found in settings! I need that to work...")
+                sys.exit(1)
+            self._client = Slack()
+            puts("Initializing storage using backend: {}".format(self._settings['STORAGE_BACKEND']))
+            self._storage = Storage.get_instance()
+            logger.debug("Storage initialized!")
+
+            self._plugin_actions = {
+                'process': {},
+                'listen_to': {},
+                'respond_to': {},
+                'catch_all': {}
+            }
+            puts("Loading plugins...")
+            self.load_plugins()
+            logger.debug("The following plugin actions were registered: %s", self._plugin_actions)
+            self._dispatcher = EventDispatcher(self._plugin_actions)
 
     def load_plugins(self):
-        logger.debug("PLUGINS: %s", self._settings['PLUGINS'])
-        for plugin in self._settings['PLUGINS']:
-            for class_name, cls in import_string(plugin):
-                if MachineBasePlugin in cls.__bases__ and cls is not MachineBasePlugin:
-                    logger.debug("Found a Machine plugin: {}".format(plugin))
-                    storage = PluginStorage(class_name)
-                    instance = cls(self._settings, MessagingClient(),
-                                   storage)
-                    self._register_plugin(class_name, instance)
+        with indent(4):
+            logger.debug("PLUGINS: %s", self._settings['PLUGINS'])
+            for plugin in self._settings['PLUGINS']:
+                for class_name, cls in import_string(plugin):
+                    if MachineBasePlugin in cls.__bases__ and cls is not MachineBasePlugin:
+                        logger.debug("Found a Machine plugin: {}".format(plugin))
+                        storage = PluginStorage(class_name)
+                        instance = cls(self._settings, MessagingClient(),
+                                       storage)
+                        self._register_plugin(class_name, instance)
+                        show_valid(class_name)
 
     def _register_plugin(self, plugin_class, cls_instance):
         if hasattr(cls_instance, 'catch_all'):
             self._plugin_actions['catch_all'][plugin_class] = {
                 'class': cls_instance,
                 'class_name': plugin_class,
                 'function': getattr(cls_instance, 'catch_all')
@@ -92,10 +103,15 @@
                     key = "{}-{}".format(fq_fn_name, regex.pattern)
                     self._plugin_actions[action][key] = event_handler
             if action == 'schedule':
                 Scheduler.get_instance().add_job(fq_fn_name, trigger='cron', args=[cls_instance],
                                                  id=fq_fn_name, replace_existing=True, **config)
 
     def run(self):
-        self._client.rtm_connect()
-        Scheduler.get_instance().start()
-        self._dispatcher.start()
+        announce("\nStarting Slack Machine:")
+        with indent(4):
+            self._client.rtm_connect()
+            show_valid("Connected to Slack")
+            Scheduler.get_instance().start()
+            show_valid("Scheduler started")
+            show_valid("Dispatcher started")
+            self._dispatcher.start()
```

### Comparing `slack-machine-0.8/machine/dispatch.py` & `slack-machine-0.9/machine/dispatch.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/plugins/base.py` & `slack-machine-0.9/machine/plugins/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
         .. _basic Slack formatting: https://api.slack.com/docs/message-formatting
 
         :param channel: id or name of channel to send message to. Can be public or private (group)
             channel, or DM channel.
         :param text: message text
         :param thread_ts: optional timestamp of thread, to send a message in that thread
+        :returns: None
         """
         self._client.send(channel, text, thread_ts)
 
     def say_scheduled(self, when, channel, text):
         """Schedule a message to a channel
 
         This is the scheduled version of
@@ -86,14 +87,15 @@
         It behaves the same, but will send the message at the scheduled time.
 
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param channel: id or name of channel to send message to. Can be public or private (group)
             channel, or DM channel.
         :param text: message text
+        :returns: None
         """
         self._client.send_scheduled(when, channel, text)
 
     def say_webapi(self, channel, text, attachments=None, thread_ts=None, ephemeral_user=None):
         """Send a message to a channel using the WebAPI
 
         Send a message to a channel using the WebAPI. Allows for rich formatting using
@@ -107,69 +109,80 @@
         :param channel: id or name of channel to send message to. Can be public or private (group)
             channel, or DM channel.
         :param text: message text
         :param attachments: optional attachments (see `attachments`_)
         :param thread_ts: optional timestamp of thread, to send a message in that thread
         :param ephemeral_user: optional user name or id if the message needs to visible
             to a specific user only
+        :returns: Dictionary deserialized from `chat.postMessage`_ request, or `chat.postEphemeral`_
+            if `ephemeral_user` is True.
+
+        .. _chat.postMessage: https://api.slack.com/methods/chat.postMessage
+        .. _chat.postEphemeral: https://api.slack.com/methods/chat.postEphemeral
         """
-        self._client.send_webapi(channel, text, attachments, thread_ts, ephemeral_user)
+        return self._client.send_webapi(channel, text, attachments, thread_ts, ephemeral_user)
 
     def say_webapi_scheduled(self, when, channel, text, attachments, ephemeral_user):
         """Schedule a message to a channel and send it using the WebAPI
 
         This is the scheduled version of
         :py:meth:`~machine.plugins.base.MachineBasePlugin.say_webapi`.
         It behaves the same, but will send the message at the scheduled time.
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param text: message text
         :param attachments: optional attachments (see `attachments`_)
         :param ephemeral_user: optional user name or id if the message needs to visible
             to a specific user only
+        :returns: None
         """
         self._client.send_webapi_scheduled(when, channel, text, attachments, ephemeral_user)
 
     def react(self, channel, ts, emoji):
         """React to a message in a channel
 
         Add a reaction to a message in a channel. What message to react to, is determined by the
         combination of the channel and the timestamp of the message.
 
         :param channel: id or name of channel to send message to. Can be public or private (group)
             channel, or DM channel.
         :param ts: timestamp of the message to react to
         :param emoji: what emoji to react with (should be a string, like 'angel', 'thumbsup', etc.)
+        :returns: Dictionary deserialized from `reactions.add`_ request.
+
+        .. _reactions.add: https://api.slack.com/methods/reactions.add
         """
-        self._client.react(channel, ts, emoji)
+        return self._client.react(channel, ts, emoji)
 
     def send_dm(self, user, text):
         """Send a Direct Message
 
         Send a Direct Message to a user by opening a DM channel and sending a message to it.
         Only `basic Slack formatting`_ allowed. For richer formatting using attachments, use
         :py:meth:`~machine.plugins.base.MachineBasePlugin.send_dm_webapi`
 
         .. _basic Slack formatting: https://api.slack.com/docs/message-formatting
 
         :param user: id or name of the user to send direct message to
         :param text: message text
+        :returns: None
         """
         self._client.send_dm(user, text)
 
     def send_dm_scheduled(self, when, user, text):
         """Schedule a Direct Message
 
         This is the scheduled version of
         :py:meth:`~machine.plugins.base.MachineBasePlugin.send_dm`. It behaves the same, but will
         send the DM at the scheduled time.
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param user: id or name of the user to send direct message to
         :param text: message text
+        :returns: None
         """
         self._client.send_dm_scheduled(when, user, text)
 
     def send_dm_webapi(self, user, text, attachments=None):
         """Send a Direct Message through the WebAPI
 
         Send a Direct Message to a user by opening a DM channel and sending a message to it via
@@ -177,40 +190,45 @@
         `attachments`_.
 
         .. _attachments: https://api.slack.com/docs/message-attachments
 
         :param user: id or name of the user to send direct message to
         :param text: message text
         :param attachments: optional attachments (see `attachments`_)
+        :returns: Dictionary deserialized from `chat.postMessage`_ request.
+
+        .. _chat.postMessage: https://api.slack.com/methods/chat.postMessage
         """
-        self._client.send_dm_webapi(user, text, attachments)
+        return self._client.send_dm_webapi(user, text, attachments)
 
     def send_dm_webapi_scheduled(self, when, user, text, attachments=None):
         """Schedule a Direct Message and send it using the WebAPI
 
         This is the scheduled version of
         :py:meth:`~machine.plugins.base.MachineBasePlugin.send_dm_webapi`. It behaves the same, but
         will send the DM at the scheduled time.
 
         .. _attachments: https://api.slack.com/docs/message-attachments
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param text: message text
         :param attachments: optional attachments (see `attachments`_)
+        :returns: None
         """
         self._client.send_dm_webapi_scheduled(when, user, text, attachments)
 
     def emit(self, event, **kwargs):
         """Emit an event
 
         Emit an event that plugins can listen for. You can include arbitrary data as keyword
         arguments.
 
         :param event: name of the event
         :param kwargs: any data you want to emit with the event
+        :returns: None
         """
         e = signal(event)
         e.send(self, **kwargs)
 
 
 class Message:
     """A message that was received by the bot
@@ -270,25 +288,27 @@
         Only `basic Slack formatting`_ allowed. For richer formatting using attachments, use
         :py:meth:`~machine.plugins.base.Message.say_webapi`
 
         .. _basic Slack formatting: https://api.slack.com/docs/message-formatting
 
         :param text: message text
         :param thread_ts: optional timestamp of thread, to send a message in that thread
+        :returns: None
         """
         self._client.send(self.channel.id, text, thread_ts)
 
     def say_scheduled(self, when, text):
         """Schedule a message
 
         This is the scheduled version of :py:meth:`~machine.plugins.base.Message.say`.
         It behaves the same, but will send the message at the scheduled time.
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param text: message text
+        :returns: None
         """
         self._client.send_scheduled(when, self.channel.id, text)
 
     def say_webapi(self, text, attachments=None, thread_ts=None, ephemeral=False):
         """Send a new message using the WebAPI to the channel the original message was received in
 
         Send a new message to the channel the original message was received in, using the WebAPI.
@@ -300,48 +320,63 @@
         .. _attachments: https://api.slack.com/docs/message-attachments
 
         :param text: message text
         :param attachments: optional attachments (see `attachments`_)
         :param thread_ts: optional timestamp of thread, to send a message in that thread
         :param ephemeral: ``True/False`` wether to send the message as an ephemeral message, only
             visible to the sender of the original message
+        :returns: Dictionary deserialized from `chat.postMessage`_ request, or `chat.postEphemeral`_
+            if `ephemeral` is True.
+
+        .. _chat.postMessage: https://api.slack.com/methods/chat.postMessage
+        .. _chat.postEphemeral: https://api.slack.com/methods/chat.postEphemeral
         """
         if ephemeral:
             ephemeral_user = self.sender.id
         else:
             ephemeral_user = None
-        self._client.send_webapi(self.channel.id, text, attachments, thread_ts, ephemeral_user)
+
+        return self._client.send_webapi(
+            self.channel.id,
+            text,
+            attachments,
+            thread_ts,
+            ephemeral_user,
+        )
 
     def say_webapi_scheduled(self, when, text, attachments=None, ephemeral=False):
         """Schedule a message and send it using the WebAPI
 
         This is the scheduled version of :py:meth:`~machine.plugins.base.Message.say_webapi`.
         It behaves the same, but will send the DM at the scheduled time.
 
         .. _attachments: https://api.slack.com/docs/message-attachments
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param text: message text
         :param attachments: optional attachments (see `attachments`_)
         :param ephemeral: ``True/False`` wether to send the message as an ephemeral message, only
             visible to the sender of the original message
+        :returns: None
         """
         if ephemeral:
             ephemeral_user = self.sender.id
         else:
             ephemeral_user = None
+
         self._client.send_webapi_scheduled(when, self.channel.id, text, attachments, ephemeral_user)
 
     def reply(self, text, in_thread=False):
         """Reply to the sender of the original message
 
         Reply to the sender of the original message with a new message, mentioning that user.
 
         :param text: message text
         :param in_thread: ``True/False`` wether to reply to the original message in-thread
+        :returns: None
         """
         if in_thread:
             self.say(text, thread_ts=self.thread_ts)
         else:
             text = self._create_reply(text)
             self.say(text)
 
@@ -349,14 +384,15 @@
         """Schedule a reply
 
         This is the scheduled version of :py:meth:`~machine.plugins.base.Message.reply`.
         It behaves the same, but will send the reply at the scheduled time.
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param text: message text
+        :returns: None
         """
         self.say_scheduled(when, self._create_reply(text))
 
     def reply_webapi(self, text, attachments=None, in_thread=False, ephemeral=False):
         """Reply to the sender of the original message using the WebAPI
 
         Reply to the sender of the original message with a new message, mentioning that user. Uses
@@ -368,93 +404,108 @@
         .. _attachments: https://api.slack.com/docs/message-attachments
 
         :param text: message text
         :param attachments: optional attachments (see `attachments`_)
         :param in_thread: ``True/False`` wether to reply to the original message in-thread
         :param ephemeral: ``True/False`` wether to send the message as an ephemeral message, only
             visible to the sender of the original message
+        :returns: Dictionary deserialized from `chat.postMessage`_ request, or `chat.postEphemeral`_
+            if `ephemeral` is True.
+
+        .. _chat.postMessage: https://api.slack.com/methods/chat.postMessage
+        .. _chat.postEphemeral: https://api.slack.com/methods/chat.postEphemeral
         """
         if in_thread and not ephemeral:
-            self.say_webapi(text, attachments=attachments, thread_ts=self.thread_ts)
+            return self.say_webapi(text, attachments=attachments, thread_ts=self.thread_ts)
         else:
             text = self._create_reply(text)
-            self.say_webapi(text, attachments=attachments, ephemeral=ephemeral)
+            return self.say_webapi(text, attachments=attachments, ephemeral=ephemeral)
 
     def reply_webapi_scheduled(self, when, text, attachments=None, ephemeral=False):
         """Schedule a reply and send it using the WebAPI
 
         This is the scheduled version of :py:meth:`~machine.plugins.base.Message.reply_webapi`.
         It behaves the same, but will send the reply at the scheduled time.
 
         .. _attachments: https://api.slack.com/docs/message-attachments
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param attachments: optional attachments (see `attachments`_)
         :param ephemeral: ``True/False`` wether to send the message as an ephemeral message, only
             visible to the sender of the original message
+        :returns: None
         """
         self.say_webapi_scheduled(when, self._create_reply(text), attachments, ephemeral)
 
     def reply_dm(self, text):
         """Reply to the sender of the original message with a DM
 
         Reply in a Direct Message to the sender of the original message by opening a DM channel and
         sending a message to it.
 
         :param text: message text
+        :returns: None
         """
         self._client.send_dm(self.sender.id, text)
 
     def reply_dm_scheduled(self, when, text):
         """Schedule a DM reply
 
         This is the scheduled version of :py:meth:`~machine.plugins.base.Message.reply_dm`. It
         behaves the same, but will send the DM at the scheduled time.
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param text: message text
+        :returns: None
         """
         self._client.send_dm_scheduled(when, self.sender.id, text)
 
     def reply_dm_webapi(self, text, attachments=None):
         """Reply to the sender of the original message with a DM using the WebAPI
 
         Reply in a Direct Message to the sender of the original message by opening a DM channel and
         sending a message to it via the WebAPI. Allows for rich formatting using
         `attachments`_.
 
         .. _attachments: https://api.slack.com/docs/message-attachments
 
         :param text: message text
         :param attachments: optional attachments (see `attachments`_)
+        :returns: Dictionary deserialized from `chat.postMessage`_ request.
+
+        .. _chat.postMessage: https://api.slack.com/methods/chat.postMessage
         """
-        self._client.send_dm_webapi(self.sender.id, text, attachments)
+        return self._client.send_dm_webapi(self.sender.id, text, attachments)
 
     def reply_dm_webapi_scheduled(self, when, text, attachments=None):
         """Schedule a DM reply and send it using the WebAPI
 
         This is the scheduled version of :py:meth:`~machine.plugins.base.Message.reply_dm_webapi`.
         It behaves the same, but will send the DM at the scheduled time.
 
         .. _attachments: https://api.slack.com/docs/message-attachments
 
         :param when: when you want the message to be sent, as :py:class:`datetime.datetime` instance
         :param text: message text
         :param attachments: optional attachments (see `attachments`_)
+        :returns: None
         """
         self._client.send_dm_webapi_scheduled(when, self.sender.id, text, attachments)
 
     def react(self, emoji):
         """React to the original message
 
         Add a reaction to the original message
 
         :param emoji: what emoji to react with (should be a string, like 'angel', 'thumbsup', etc.)
+        :returns: Dictionary deserialized from `reactions.add`_ request.
+
+        .. _reactions.add: https://api.slack.com/methods/reactions.add
         """
-        self._client.react(self.channel.id, self._msg_event['ts'], emoji)
+        return self._client.react(self.channel.id, self._msg_event['ts'], emoji)
 
     def _create_reply(self, text):
         chan = self._msg_event['channel']
         if chan.startswith('C') or chan.startswith('G'):
             return "{}: {}".format(self.at_sender, text)
         else:
             return text
```

### Comparing `slack-machine-0.8/machine/plugins/builtin/general.py` & `slack-machine-0.9/machine/plugins/builtin/general.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/plugins/decorators.py` & `slack-machine-0.9/machine/plugins/decorators.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/settings.py` & `slack-machine-0.9/machine/settings.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/singletons.py` & `slack-machine-0.9/machine/singletons.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/slack.py` & `slack-machine-0.9/machine/slack.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,81 +16,90 @@
 
     def send(self, channel, text, thread_ts=None):
         Slack.get_instance().rtm_send_message(channel, text, thread_ts)
 
     def send_scheduled(self, when, channel, text):
         args = [self, channel, text]
         kwargs = {'thread_ts': None}
+
         Scheduler.get_instance().add_job(MessagingClient.send, trigger='date', args=args,
                                          kwargs=kwargs, run_date=when)
 
     def send_webapi(self, channel, text, attachments=None, thread_ts=None, ephemeral_user=None):
         method = 'chat.postMessage'
+
         # This is the only way to conditionally add thread_ts
         kwargs = {
             'channel': channel,
             'text': text,
             'attachments': attachments,
             'as_user': True
         }
+
         if ephemeral_user:
             method = 'chat.postEphemeral'
             kwargs['user'] = ephemeral_user
         else:
             if thread_ts:
                 kwargs['thread_ts'] = thread_ts
-        Slack.get_instance().api_call(
+
+        return Slack.get_instance().api_call(
             method,
             **kwargs
         )
 
     def send_webapi_scheduled(self, when, channel, text, attachments=None, ephemeral_user=None):
         args = [self, channel, text]
         kwargs = {
             'attachments': attachments,
             'thread_ts': None,
             'ephemeral_user': ephemeral_user
         }
+
         Scheduler.get_instance().add_job(MessagingClient.send_webapi, trigger='date', args=args,
                                          kwargs=kwargs, run_date=when)
 
     def react(self, channel, ts, emoji):
-        Slack.get_instance().api_call(
+        return Slack.get_instance().api_call(
             'reactions.add',
             name=emoji,
             channel=channel,
             timestamp=ts
         )
 
     def open_im(self, user):
         response = Slack.get_instance().api_call(
             'im.open',
             user=user
         )
+
         return response['channel']['id']
 
     def send_dm(self, user, text):
         u = self.users.find(user)
         dm_channel = self.open_im(u.id)
+
         self.send(dm_channel, text)
 
     def send_dm_scheduled(self, when, user, text):
         args = [self, user, text]
         Scheduler.get_instance().add_job(MessagingClient.send_dm, trigger='date', args=args,
                                          run_date=when)
 
     def send_dm_webapi(self, user, text, attachments=None):
         u = self.users.find(user)
         dm_channel = self.open_im(u.id)
-        Slack.get_instance().api_call(
+
+        return Slack.get_instance().api_call(
             'chat.postMessage',
             channel=dm_channel,
             text=text,
             attachments=attachments,
             as_user=True
         )
 
     def send_dm_webapi_scheduled(self, when, user, text, attachments=None):
         args = [self, user, text]
         kwargs = {'attachments': attachments}
+
         Scheduler.get_instance().add_job(MessagingClient.send_dm_webapi, trigger='data', args=args,
                                          kwargs=kwargs)
```

### Comparing `slack-machine-0.8/machine/storage/__init__.py` & `slack-machine-0.9/machine/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/storage/backends/base.py` & `slack-machine-0.9/machine/storage/backends/base.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/storage/backends/memory.py` & `slack-machine-0.9/machine/storage/backends/memory.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/storage/backends/redis.py` & `slack-machine-0.9/machine/storage/backends/redis.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/utils/collections.py` & `slack-machine-0.9/machine/utils/collections.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/utils/module_loading.py` & `slack-machine-0.9/machine/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/machine/utils/pool.py` & `slack-machine-0.9/machine/utils/pool.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/PKG-INFO` & `slack-machine-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: slack-machine
-Version: 0.8
+Version: 0.9
 Summary: A sexy, simple, yet powerful and extendable Slack bot
 Home-page: https://github.com/DandyDev/slack-machine
 Author: Daan Debie
 Author-email: debie.daan@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: Slack Machine
@@ -102,15 +102,14 @@
 Keywords: slack bot framework ai
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
 Classifier: Topic :: Office/Business
```

### Comparing `slack-machine-0.8/README.rst` & `slack-machine-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/setup.py` & `slack-machine-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Communications :: Chat",
         "Topic :: Internet",
         "Topic :: Office/Business"
```

### Comparing `slack-machine-0.8/slack_machine.egg-info/PKG-INFO` & `slack-machine-0.9/slack_machine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: slack-machine
-Version: 0.8
+Version: 0.9
 Summary: A sexy, simple, yet powerful and extendable Slack bot
 Home-page: https://github.com/DandyDev/slack-machine
 Author: Daan Debie
 Author-email: debie.daan@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: Slack Machine
@@ -102,15 +102,14 @@
 Keywords: slack bot framework ai
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Internet
 Classifier: Topic :: Office/Business
```

### Comparing `slack-machine-0.8/slack_machine.egg-info/SOURCES.txt` & `slack-machine-0.9/slack_machine.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 machine/storage/backends/memory.py
 machine/storage/backends/redis.py
 machine/utils/__init__.py
 machine/utils/collections.py
 machine/utils/module_loading.py
 machine/utils/pool.py
 machine/utils/redis.py
+machine/utils/text.py
 slack_machine.egg-info/PKG-INFO
 slack_machine.egg-info/SOURCES.txt
 slack_machine.egg-info/dependency_links.txt
 slack_machine.egg-info/entry_points.txt
 slack_machine.egg-info/not-zip-safe
 slack_machine.egg-info/requires.txt
 slack_machine.egg-info/top_level.txt
```

### Comparing `slack-machine-0.8/tests/test_decorators.py` & `slack-machine-0.9/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/tests/test_dispatch.py` & `slack-machine-0.9/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/tests/test_import_settings.py` & `slack-machine-0.9/tests/test_import_settings.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/tests/test_import_string.py` & `slack-machine-0.9/tests/test_import_string.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/tests/test_memory_storage.py` & `slack-machine-0.9/tests/test_memory_storage.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/tests/test_plugin_registration.py` & `slack-machine-0.9/tests/test_plugin_registration.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/tests/test_plugin_storage.py` & `slack-machine-0.9/tests/test_plugin_storage.py`

 * *Files identical despite different names*

### Comparing `slack-machine-0.8/tests/test_redis_storage.py` & `slack-machine-0.9/tests/test_redis_storage.py`

 * *Files identical despite different names*

