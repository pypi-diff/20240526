# Comparing `tmp/libbot-3.2.0.tar.gz` & `tmp/libbot-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbot-3.2.0.tar", last modified: Sun May 26 14:34:53 2024, max compression
+gzip compressed data, was "libbot-3.2.1.tar", last modified: Sun May 26 14:51:27 2024, max compression
```

## Comparing `libbot-3.2.0.tar` & `libbot-3.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.772700 libbot-3.2.0/
--rw-rw-rw-   0        0        0    34902 2024-04-22 21:47:22.000000 libbot-3.2.0/LICENSE
--rw-rw-rw-   0        0        0     4501 2024-05-26 14:34:53.770688 libbot-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2509 2024-05-19 12:46:00.000000 libbot-3.2.0/README.md
--rw-rw-rw-   0        0        0     1998 2024-05-19 12:46:23.000000 libbot-3.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.708604 libbot-3.2.0/requirements/
--rw-rw-rw-   0        0        0       16 2024-04-22 21:47:22.000000 libbot-3.2.0/requirements/_.txt
--rw-rw-rw-   0        0        0      205 2024-05-26 13:03:54.000000 libbot-3.2.0/requirements/dev.txt
--rw-rw-rw-   0        0        0       35 2024-05-14 21:19:20.000000 libbot-3.2.0/requirements/pycord.txt
--rw-rw-rw-   0        0        0       43 2024-05-14 21:19:20.000000 libbot-3.2.0/requirements/pyrogram.txt
--rw-rw-rw-   0        0        0       13 2024-05-14 21:19:20.000000 libbot-3.2.0/requirements/speed.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 14:34:53.772700 libbot-3.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.686542 libbot-3.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.711700 libbot-3.2.0/src/libbot/
--rw-rw-rw-   0        0        0      210 2024-05-26 13:40:41.000000 libbot-3.2.0/src/libbot/__init__.py
--rw-rw-rw-   0        0        0     3718 2024-05-26 13:20:39.000000 libbot-3.2.0/src/libbot/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.724768 libbot-3.2.0/src/libbot/errors/
--rw-rw-rw-   0        0        0       54 2024-05-19 11:56:28.000000 libbot-3.2.0/src/libbot/errors/__init__.py
--rw-rw-rw-   0        0        0     1508 2024-05-19 11:55:52.000000 libbot-3.2.0/src/libbot/errors/config.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.726770 libbot-3.2.0/src/libbot/i18n/
--rw-rw-rw-   0        0        0     3880 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.728772 libbot-3.2.0/src/libbot/i18n/classes/
--rw-rw-rw-   0        0        0     3980 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/i18n/classes/bot_locale.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.729775 libbot-3.2.0/src/libbot/i18n/sync/
--rw-rw-rw-   0        0        0     3771 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/i18n/sync/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.691063 libbot-3.2.0/src/libbot/pycord/
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.734215 libbot-3.2.0/src/libbot/pycord/classes/
--rw-rw-rw-   0        0        0       28 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/pycord/classes/__init__.py
--rw-rw-rw-   0        0        0     1985 2024-05-19 13:01:47.000000 libbot-3.2.0/src/libbot/pycord/classes/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.692072 libbot-3.2.0/src/libbot/pyrogram/
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.741734 libbot-3.2.0/src/libbot/pyrogram/classes/
--rw-rw-rw-   0        0        0      102 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/pyrogram/classes/__init__.py
--rw-rw-rw-   0        0        0    15428 2024-05-14 21:19:20.000000 libbot-3.2.0/src/libbot/pyrogram/classes/client.py
--rw-rw-rw-   0        0        0      176 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/pyrogram/classes/command.py
--rw-rw-rw-   0        0        0     1033 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/pyrogram/classes/commandset.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.746736 libbot-3.2.0/src/libbot/sync/
--rw-rw-rw-   0        0        0       84 2024-05-26 13:20:01.000000 libbot-3.2.0/src/libbot/sync/__init__.py
--rw-rw-rw-   0        0        0     3575 2024-05-26 13:20:24.000000 libbot-3.2.0/src/libbot/sync/__main__.py
--rw-rw-rw-   0        0        0     1738 2024-05-26 13:19:52.000000 libbot-3.2.0/src/libbot/sync/_nested.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.764568 libbot-3.2.0/src/libbot.egg-info/
--rw-rw-rw-   0        0        0     4501 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      343 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.762570 libbot-3.2.0/tests/
--rw-rw-rw-   0        0        0     1673 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_bot_locale.py
--rw-rw-rw-   0        0        0     1657 2024-05-26 13:39:02.000000 libbot-3.2.0/tests/test_config_async.py
--rw-rw-rw-   0        0        0     1477 2024-05-26 13:39:05.000000 libbot-3.2.0/tests/test_config_sync.py
--rw-rw-rw-   0        0        0     1893 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_i18n_async.py
--rw-rw-rw-   0        0        0     1758 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_i18n_sync.py
--rw-rw-rw-   0        0        0     1642 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_json_async.py
--rw-rw-rw-   0        0        0     1557 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_json_sync.py
--rw-rw-rw-   0        0        0     1973 2024-05-26 13:27:48.000000 libbot-3.2.0/tests/test_nested_set.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.426476 libbot-3.2.1/
+-rw-rw-rw-   0        0        0    34902 2024-04-22 21:47:22.000000 libbot-3.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4501 2024-05-26 14:51:27.424471 libbot-3.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2509 2024-05-19 12:46:00.000000 libbot-3.2.1/README.md
+-rw-rw-rw-   0        0        0     1998 2024-05-19 12:46:23.000000 libbot-3.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.353475 libbot-3.2.1/requirements/
+-rw-rw-rw-   0        0        0       16 2024-04-22 21:47:22.000000 libbot-3.2.1/requirements/_.txt
+-rw-rw-rw-   0        0        0      205 2024-05-26 13:03:54.000000 libbot-3.2.1/requirements/dev.txt
+-rw-rw-rw-   0        0        0       35 2024-05-14 21:19:20.000000 libbot-3.2.1/requirements/pycord.txt
+-rw-rw-rw-   0        0        0       43 2024-05-14 21:19:20.000000 libbot-3.2.1/requirements/pyrogram.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 21:19:20.000000 libbot-3.2.1/requirements/speed.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:51:27.426476 libbot-3.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.323882 libbot-3.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.356474 libbot-3.2.1/src/libbot/
+-rw-rw-rw-   0        0        0      210 2024-05-26 14:50:31.000000 libbot-3.2.1/src/libbot/__init__.py
+-rw-rw-rw-   0        0        0     3992 2024-05-26 14:41:51.000000 libbot-3.2.1/src/libbot/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.377545 libbot-3.2.1/src/libbot/errors/
+-rw-rw-rw-   0        0        0       54 2024-05-19 11:56:28.000000 libbot-3.2.1/src/libbot/errors/__init__.py
+-rw-rw-rw-   0        0        0     1508 2024-05-19 11:55:52.000000 libbot-3.2.1/src/libbot/errors/config.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.381081 libbot-3.2.1/src/libbot/i18n/
+-rw-rw-rw-   0        0        0     3880 2024-04-22 21:47:22.000000 libbot-3.2.1/src/libbot/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.384081 libbot-3.2.1/src/libbot/i18n/classes/
+-rw-rw-rw-   0        0        0     3980 2024-04-22 21:47:22.000000 libbot-3.2.1/src/libbot/i18n/classes/bot_locale.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.386078 libbot-3.2.1/src/libbot/i18n/sync/
+-rw-rw-rw-   0        0        0     3771 2024-04-22 21:47:22.000000 libbot-3.2.1/src/libbot/i18n/sync/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.329404 libbot-3.2.1/src/libbot/pycord/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.391618 libbot-3.2.1/src/libbot/pycord/classes/
+-rw-rw-rw-   0        0        0       28 2024-04-22 21:47:22.000000 libbot-3.2.1/src/libbot/pycord/classes/__init__.py
+-rw-rw-rw-   0        0        0     1985 2024-05-19 13:01:47.000000 libbot-3.2.1/src/libbot/pycord/classes/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.331414 libbot-3.2.1/src/libbot/pyrogram/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.399650 libbot-3.2.1/src/libbot/pyrogram/classes/
+-rw-rw-rw-   0        0        0      102 2024-04-22 21:47:22.000000 libbot-3.2.1/src/libbot/pyrogram/classes/__init__.py
+-rw-rw-rw-   0        0        0    15428 2024-05-14 21:19:20.000000 libbot-3.2.1/src/libbot/pyrogram/classes/client.py
+-rw-rw-rw-   0        0        0      176 2024-04-22 21:47:22.000000 libbot-3.2.1/src/libbot/pyrogram/classes/command.py
+-rw-rw-rw-   0        0        0     1033 2024-04-22 21:47:22.000000 libbot-3.2.1/src/libbot/pyrogram/classes/commandset.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.404651 libbot-3.2.1/src/libbot/sync/
+-rw-rw-rw-   0        0        0       84 2024-05-26 13:20:01.000000 libbot-3.2.1/src/libbot/sync/__init__.py
+-rw-rw-rw-   0        0        0     3849 2024-05-26 14:41:46.000000 libbot-3.2.1/src/libbot/sync/__main__.py
+-rw-rw-rw-   0        0        0     1738 2024-05-26 13:19:52.000000 libbot-3.2.1/src/libbot/sync/_nested.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.420473 libbot-3.2.1/src/libbot.egg-info/
+-rw-rw-rw-   0        0        0     4501 2024-05-26 14:51:27.000000 libbot-3.2.1/src/libbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2024-05-26 14:51:27.000000 libbot-3.2.1/src/libbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:51:27.000000 libbot-3.2.1/src/libbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      343 2024-05-26 14:51:27.000000 libbot-3.2.1/src/libbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 14:51:27.000000 libbot-3.2.1/src/libbot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 14:51:27.418464 libbot-3.2.1/tests/
+-rw-rw-rw-   0        0        0     1673 2024-04-22 21:47:22.000000 libbot-3.2.1/tests/test_bot_locale.py
+-rw-rw-rw-   0        0        0     1985 2024-05-26 14:49:36.000000 libbot-3.2.1/tests/test_config_async.py
+-rw-rw-rw-   0        0        0     1788 2024-05-26 14:48:52.000000 libbot-3.2.1/tests/test_config_sync.py
+-rw-rw-rw-   0        0        0     1893 2024-04-22 21:47:22.000000 libbot-3.2.1/tests/test_i18n_async.py
+-rw-rw-rw-   0        0        0     1758 2024-04-22 21:47:22.000000 libbot-3.2.1/tests/test_i18n_sync.py
+-rw-rw-rw-   0        0        0     1642 2024-04-22 21:47:22.000000 libbot-3.2.1/tests/test_json_async.py
+-rw-rw-rw-   0        0        0     1557 2024-04-22 21:47:22.000000 libbot-3.2.1/tests/test_json_sync.py
+-rw-rw-rw-   0        0        0     1973 2024-05-26 13:27:48.000000 libbot-3.2.1/tests/test_nested_set.py
```

### Comparing `libbot-3.2.0/LICENSE` & `libbot-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/PKG-INFO` & `libbot-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbot
-Version: 3.2.0
+Version: 3.2.1
 Summary: Universal bot library with functions needed for basic Discord/Telegram bot development.
 Author: Profitroll
 License: GPLv3
 Project-URL: Source, https://git.end-play.xyz/profitroll/LibBotUniversal
 Project-URL: Documentation, https://git.end-play.xyz/profitroll/LibBotUniversal/wiki
 Project-URL: Tracker, https://git.end-play.xyz/profitroll/LibBotUniversal/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `libbot-3.2.0/README.md` & `libbot-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/pyproject.toml` & `libbot-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/src/libbot/__main__.py` & `libbot-3.2.1/src/libbot/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,24 +98,32 @@
     await json_write(
         nested_set(await json_read(config_file), value, *(*path, key)), config_file
     )
     return
 
 
 async def config_delete(
-    key: str, *path: str, config_file: Union[str, Path] = "config.json"
+    key: str,
+    *path: str,
+    missing_ok: bool = False,
+    config_file: Union[str, Path] = "config.json",
 ) -> None:
     """Set config's key by its path
 
     ### Args:
         * key (`str`): Key to delete
         * *path (`str`): Path to the key of the target
+        * missing_ok (`bool`): Do not raise an exception if the key is missing. Defaults to `False`
         * config_file (`Union[str, Path]`, *optional*): Path-like object or path as a string of a location of the config file. Defaults to `"config.json"`
 
     ### Raises:
-        * `KeyError`: Key is not found under path provided
+        * `KeyError`: Key is not found under path provided and `missing_ok` is `False`
     """
     config_data = await json_read(config_file)
 
-    nested_delete(config_data, *(*path, key))
+    try:
+        nested_delete(config_data, *(*path, key))
+    except KeyError as exc:
+        if not missing_ok:
+            raise exc from exc
 
     await json_write(config_data, config_file)
```

### Comparing `libbot-3.2.0/src/libbot/errors/config.py` & `libbot-3.2.1/src/libbot/errors/config.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/src/libbot/i18n/__init__.py` & `libbot-3.2.1/src/libbot/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/src/libbot/i18n/classes/bot_locale.py` & `libbot-3.2.1/src/libbot/i18n/classes/bot_locale.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/src/libbot/i18n/sync/__init__.py` & `libbot-3.2.1/src/libbot/i18n/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/src/libbot/pycord/classes/bot.py` & `libbot-3.2.1/src/libbot/pycord/classes/bot.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/src/libbot/pyrogram/classes/client.py` & `libbot-3.2.1/src/libbot/pyrogram/classes/client.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/src/libbot/pyrogram/classes/commandset.py` & `libbot-3.2.1/src/libbot/pyrogram/classes/commandset.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/src/libbot/sync/__main__.py` & `libbot-3.2.1/src/libbot/sync/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -94,24 +94,32 @@
         * `KeyError`: Key is not found under path provided
     """
     json_write(nested_set(json_read(config_file), value, *(*path, key)), config_file)
     return
 
 
 def config_delete(
-    key: str, *path: str, config_file: Union[str, Path] = "config.json"
+    key: str,
+    *path: str,
+    missing_ok: bool = False,
+    config_file: Union[str, Path] = "config.json",
 ) -> None:
     """Set config's key by its path
 
     ### Args:
         * key (`str`): Key to delete
         * *path (`str`): Path to the key of the target
+        * missing_ok (`bool`): Do not raise an exception if the key is missing. Defaults to `False`
         * config_file (`Union[str, Path]`, *optional*): Path-like object or path as a string of a location of the config file. Defaults to `"config.json"`
 
     ### Raises:
-        * `KeyError`: Key is not found under path provided
+        * `KeyError`: Key is not found under path provided and `missing_ok` is `False`
     """
     config_data = json_read(config_file)
 
-    nested_delete(config_data, *(*path, key))
+    try:
+        nested_delete(config_data, *(*path, key))
+    except KeyError as exc:
+        if not missing_ok:
+            raise exc from exc
 
     json_write(config_data, config_file)
```

### Comparing `libbot-3.2.0/src/libbot/sync/_nested.py` & `libbot-3.2.1/src/libbot/sync/_nested.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/src/libbot.egg-info/PKG-INFO` & `libbot-3.2.1/src/libbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbot
-Version: 3.2.0
+Version: 3.2.1
 Summary: Universal bot library with functions needed for basic Discord/Telegram bot development.
 Author: Profitroll
 License: GPLv3
 Project-URL: Source, https://git.end-play.xyz/profitroll/LibBotUniversal
 Project-URL: Documentation, https://git.end-play.xyz/profitroll/LibBotUniversal/wiki
 Project-URL: Tracker, https://git.end-play.xyz/profitroll/LibBotUniversal/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `libbot-3.2.0/src/libbot.egg-info/SOURCES.txt` & `libbot-3.2.1/src/libbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/tests/test_bot_locale.py` & `libbot-3.2.1/tests/test_bot_locale.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/tests/test_config_async.py` & `libbot-3.2.1/tests/test_config_async.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Any, List
 
 import pytest
 
-from libbot import config_delete, config_get, config_set, sync
+from libbot import config_delete, config_get, config_set
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "args, expected",
     [
         (["locale"], "en"),
@@ -54,7 +54,21 @@
     [
         ("bot_token", ["bot"]),
     ],
 )
 async def test_config_delete(key: str, path: List[str], location_config: Path):
     await config_delete(key, *path, config_file=location_config)
     assert key not in (await config_get(*path, config_file=location_config))
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize(
+    "key, path",
+    [
+        ("bot_lol", ["bot"]),
+    ],
+)
+async def test_config_delete_missing(key: str, path: List[str], location_config: Path):
+    assert (
+        await config_delete(key, *path, missing_ok=True, config_file=location_config)
+        is None
+    )
```

### Comparing `libbot-3.2.0/tests/test_config_sync.py` & `libbot-3.2.1/tests/test_config_sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,7 +47,20 @@
     [
         ("bot_token", ["bot"]),
     ],
 )
 def test_config_delete(key: str, path: List[str], location_config: Path):
     sync.config_delete(key, *path, config_file=location_config)
     assert key not in sync.config_get(*path, config_file=location_config)
+
+
+@pytest.mark.parametrize(
+    "key, path",
+    [
+        ("bot_lol", ["bot"]),
+    ],
+)
+async def test_config_delete_missing(key: str, path: List[str], location_config: Path):
+    assert (
+        sync.config_delete(key, *path, missing_ok=True, config_file=location_config)
+        is None
+    )
```

### Comparing `libbot-3.2.0/tests/test_i18n_async.py` & `libbot-3.2.1/tests/test_i18n_async.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/tests/test_i18n_sync.py` & `libbot-3.2.1/tests/test_i18n_sync.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/tests/test_json_async.py` & `libbot-3.2.1/tests/test_json_async.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/tests/test_json_sync.py` & `libbot-3.2.1/tests/test_json_sync.py`

 * *Files identical despite different names*

### Comparing `libbot-3.2.0/tests/test_nested_set.py` & `libbot-3.2.1/tests/test_nested_set.py`

 * *Files identical despite different names*

