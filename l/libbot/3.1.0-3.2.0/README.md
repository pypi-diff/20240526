# Comparing `tmp/libbot-3.1.0.tar.gz` & `tmp/libbot-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbot-3.1.0.tar", last modified: Sun May 19 13:03:13 2024, max compression
+gzip compressed data, was "libbot-3.2.0.tar", last modified: Sun May 26 14:34:53 2024, max compression
```

## Comparing `libbot-3.1.0.tar` & `libbot-3.2.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.899559 libbot-3.1.0/
--rw-rw-rw-   0        0        0    34902 2024-04-22 21:47:22.000000 libbot-3.1.0/LICENSE
--rw-rw-rw-   0        0        0     4501 2024-05-19 13:03:13.898557 libbot-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2509 2024-05-19 12:46:00.000000 libbot-3.1.0/README.md
--rw-rw-rw-   0        0        0     1998 2024-05-19 12:46:23.000000 libbot-3.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.854519 libbot-3.1.0/requirements/
--rw-rw-rw-   0        0        0       16 2024-04-22 21:47:22.000000 libbot-3.1.0/requirements/_.txt
--rw-rw-rw-   0        0        0      205 2024-05-19 12:48:35.000000 libbot-3.1.0/requirements/dev.txt
--rw-rw-rw-   0        0        0       35 2024-05-14 21:19:20.000000 libbot-3.1.0/requirements/pycord.txt
--rw-rw-rw-   0        0        0       43 2024-05-14 21:19:20.000000 libbot-3.1.0/requirements/pyrogram.txt
--rw-rw-rw-   0        0        0       13 2024-05-14 21:19:20.000000 libbot-3.1.0/requirements/speed.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 13:03:13.900559 libbot-3.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.837184 libbot-3.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.857792 libbot-3.1.0/src/libbot/
--rw-rw-rw-   0        0        0      151 2024-05-19 11:59:16.000000 libbot-3.1.0/src/libbot/__init__.py
--rw-rw-rw-   0        0        0     2962 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.867004 libbot-3.1.0/src/libbot/errors/
--rw-rw-rw-   0        0        0       54 2024-05-19 11:56:28.000000 libbot-3.1.0/src/libbot/errors/__init__.py
--rw-rw-rw-   0        0        0     1508 2024-05-19 11:55:52.000000 libbot-3.1.0/src/libbot/errors/config.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.869008 libbot-3.1.0/src/libbot/i18n/
--rw-rw-rw-   0        0        0     3880 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.871010 libbot-3.1.0/src/libbot/i18n/classes/
--rw-rw-rw-   0        0        0     3980 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/i18n/classes/bot_locale.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.872007 libbot-3.1.0/src/libbot/i18n/sync/
--rw-rw-rw-   0        0        0     3771 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/i18n/sync/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.841514 libbot-3.1.0/src/libbot/pycord/
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.874003 libbot-3.1.0/src/libbot/pycord/classes/
--rw-rw-rw-   0        0        0       28 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/pycord/classes/__init__.py
--rw-rw-rw-   0        0        0     1985 2024-05-19 13:01:47.000000 libbot-3.1.0/src/libbot/pycord/classes/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.842038 libbot-3.1.0/src/libbot/pyrogram/
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.880529 libbot-3.1.0/src/libbot/pyrogram/classes/
--rw-rw-rw-   0        0        0      102 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/pyrogram/classes/__init__.py
--rw-rw-rw-   0        0        0    15428 2024-05-14 21:19:20.000000 libbot-3.1.0/src/libbot/pyrogram/classes/client.py
--rw-rw-rw-   0        0        0      176 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/pyrogram/classes/command.py
--rw-rw-rw-   0        0        0     1033 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/pyrogram/classes/commandset.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.881533 libbot-3.1.0/src/libbot/sync/
--rw-rw-rw-   0        0        0     3697 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/sync/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.894044 libbot-3.1.0/src/libbot.egg-info/
--rw-rw-rw-   0        0        0     4501 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      343 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.893046 libbot-3.1.0/tests/
--rw-rw-rw-   0        0        0     1673 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_bot_locale.py
--rw-rw-rw-   0        0        0     1289 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_config_async.py
--rw-rw-rw-   0        0        0     1162 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_config_sync.py
--rw-rw-rw-   0        0        0     1893 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_i18n_async.py
--rw-rw-rw-   0        0        0     1758 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_i18n_sync.py
--rw-rw-rw-   0        0        0     1642 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_json_async.py
--rw-rw-rw-   0        0        0     1557 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_json_sync.py
--rw-rw-rw-   0        0        0     1511 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_nested_set.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.772700 libbot-3.2.0/
+-rw-rw-rw-   0        0        0    34902 2024-04-22 21:47:22.000000 libbot-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4501 2024-05-26 14:34:53.770688 libbot-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2509 2024-05-19 12:46:00.000000 libbot-3.2.0/README.md
+-rw-rw-rw-   0        0        0     1998 2024-05-19 12:46:23.000000 libbot-3.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.708604 libbot-3.2.0/requirements/
+-rw-rw-rw-   0        0        0       16 2024-04-22 21:47:22.000000 libbot-3.2.0/requirements/_.txt
+-rw-rw-rw-   0        0        0      205 2024-05-26 13:03:54.000000 libbot-3.2.0/requirements/dev.txt
+-rw-rw-rw-   0        0        0       35 2024-05-14 21:19:20.000000 libbot-3.2.0/requirements/pycord.txt
+-rw-rw-rw-   0        0        0       43 2024-05-14 21:19:20.000000 libbot-3.2.0/requirements/pyrogram.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 21:19:20.000000 libbot-3.2.0/requirements/speed.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:34:53.772700 libbot-3.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.686542 libbot-3.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.711700 libbot-3.2.0/src/libbot/
+-rw-rw-rw-   0        0        0      210 2024-05-26 13:40:41.000000 libbot-3.2.0/src/libbot/__init__.py
+-rw-rw-rw-   0        0        0     3718 2024-05-26 13:20:39.000000 libbot-3.2.0/src/libbot/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.724768 libbot-3.2.0/src/libbot/errors/
+-rw-rw-rw-   0        0        0       54 2024-05-19 11:56:28.000000 libbot-3.2.0/src/libbot/errors/__init__.py
+-rw-rw-rw-   0        0        0     1508 2024-05-19 11:55:52.000000 libbot-3.2.0/src/libbot/errors/config.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.726770 libbot-3.2.0/src/libbot/i18n/
+-rw-rw-rw-   0        0        0     3880 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.728772 libbot-3.2.0/src/libbot/i18n/classes/
+-rw-rw-rw-   0        0        0     3980 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/i18n/classes/bot_locale.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.729775 libbot-3.2.0/src/libbot/i18n/sync/
+-rw-rw-rw-   0        0        0     3771 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/i18n/sync/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.691063 libbot-3.2.0/src/libbot/pycord/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.734215 libbot-3.2.0/src/libbot/pycord/classes/
+-rw-rw-rw-   0        0        0       28 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/pycord/classes/__init__.py
+-rw-rw-rw-   0        0        0     1985 2024-05-19 13:01:47.000000 libbot-3.2.0/src/libbot/pycord/classes/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.692072 libbot-3.2.0/src/libbot/pyrogram/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.741734 libbot-3.2.0/src/libbot/pyrogram/classes/
+-rw-rw-rw-   0        0        0      102 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/pyrogram/classes/__init__.py
+-rw-rw-rw-   0        0        0    15428 2024-05-14 21:19:20.000000 libbot-3.2.0/src/libbot/pyrogram/classes/client.py
+-rw-rw-rw-   0        0        0      176 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/pyrogram/classes/command.py
+-rw-rw-rw-   0        0        0     1033 2024-04-22 21:47:22.000000 libbot-3.2.0/src/libbot/pyrogram/classes/commandset.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.746736 libbot-3.2.0/src/libbot/sync/
+-rw-rw-rw-   0        0        0       84 2024-05-26 13:20:01.000000 libbot-3.2.0/src/libbot/sync/__init__.py
+-rw-rw-rw-   0        0        0     3575 2024-05-26 13:20:24.000000 libbot-3.2.0/src/libbot/sync/__main__.py
+-rw-rw-rw-   0        0        0     1738 2024-05-26 13:19:52.000000 libbot-3.2.0/src/libbot/sync/_nested.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.764568 libbot-3.2.0/src/libbot.egg-info/
+-rw-rw-rw-   0        0        0     4501 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      343 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 14:34:53.000000 libbot-3.2.0/src/libbot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 14:34:53.762570 libbot-3.2.0/tests/
+-rw-rw-rw-   0        0        0     1673 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_bot_locale.py
+-rw-rw-rw-   0        0        0     1657 2024-05-26 13:39:02.000000 libbot-3.2.0/tests/test_config_async.py
+-rw-rw-rw-   0        0        0     1477 2024-05-26 13:39:05.000000 libbot-3.2.0/tests/test_config_sync.py
+-rw-rw-rw-   0        0        0     1893 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_i18n_async.py
+-rw-rw-rw-   0        0        0     1758 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_i18n_sync.py
+-rw-rw-rw-   0        0        0     1642 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_json_async.py
+-rw-rw-rw-   0        0        0     1557 2024-04-22 21:47:22.000000 libbot-3.2.0/tests/test_json_sync.py
+-rw-rw-rw-   0        0        0     1973 2024-05-26 13:27:48.000000 libbot-3.2.0/tests/test_nested_set.py
```

### Comparing `libbot-3.1.0/LICENSE` & `libbot-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/PKG-INFO` & `libbot-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbot
-Version: 3.1.0
+Version: 3.2.0
 Summary: Universal bot library with functions needed for basic Discord/Telegram bot development.
 Author: Profitroll
 License: GPLv3
 Project-URL: Source, https://git.end-play.xyz/profitroll/LibBotUniversal
 Project-URL: Documentation, https://git.end-play.xyz/profitroll/LibBotUniversal/wiki
 Project-URL: Tracker, https://git.end-play.xyz/profitroll/LibBotUniversal/issues
 Classifier: Development Status :: 3 - Alpha
@@ -22,18 +22,18 @@
 License-File: LICENSE
 Requires-Dist: aiofiles>=23.0.0
 Provides-Extra: dev
 Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: build==1.2.1; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: mypy==1.10.0; extra == "dev"
-Requires-Dist: pylint==3.2.1; extra == "dev"
+Requires-Dist: pylint==3.2.2; extra == "dev"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
-Requires-Dist: pytest==8.2.0; extra == "dev"
+Requires-Dist: pytest==8.2.1; extra == "dev"
 Requires-Dist: tox==4.15.0; extra == "dev"
 Requires-Dist: types-aiofiles==23.2.0.20240403; extra == "dev"
 Requires-Dist: types-ujson==5.10.0.20240515; extra == "dev"
 Provides-Extra: pycord
 Requires-Dist: apscheduler~=3.10.4; extra == "pycord"
 Requires-Dist: py-cord~=2.5.0; extra == "pycord"
 Provides-Extra: pyrogram
```

### Comparing `libbot-3.1.0/README.md` & `libbot-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/pyproject.toml` & `libbot-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/src/libbot/__main__.py` & `libbot-3.2.0/src/libbot/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 import aiofiles
 
 try:
     from ujson import dumps, loads
 except ImportError:
     from json import dumps, loads
 
-from libbot.sync import nested_set
+from .sync._nested import nested_delete, nested_set
 
 
 async def json_read(path: Union[str, Path]) -> Any:
     """Read contents of a JSON file
 
     ### Args:
         * path (`Union[str, Path]`): Path-like object or path as a string
 
     ### Returns:
         * `Any`: File contents
     """
     async with aiofiles.open(str(path), mode="r", encoding="utf-8") as f:
         data = await f.read()
+
     return loads(data)
 
 
 async def json_write(data: Any, path: Union[str, Path]) -> None:
     """Write contents to a JSON file
 
     ### Args:
@@ -69,27 +70,52 @@
     This can be easily done with the following code:
     ```python
     import libbot
     salary = await libbot.config_get("salary", "users", "Pete")
     ```
     """
     this_key = await json_read(config_file)
+
     for dict_key in path:
         this_key = this_key[dict_key]
+
     return this_key[key]
 
 
 async def config_set(
     key: str, value: Any, *path: str, config_file: Union[str, Path] = "config.json"
 ) -> None:
     """Set config's key by its path to the value
 
     ### Args:
         * key (`str`): Key that leads to the value
         * value (`Any`): Any JSON serializable data
         * *path (`str`): Path to the key of the target
         * config_file (`Union[str, Path]`, *optional*): Path-like object or path as a string of a location of the config file. Defaults to `"config.json"`
+
+    ### Raises:
+        * `KeyError`: Key is not found under path provided
     """
     await json_write(
         nested_set(await json_read(config_file), value, *(*path, key)), config_file
     )
     return
+
+
+async def config_delete(
+    key: str, *path: str, config_file: Union[str, Path] = "config.json"
+) -> None:
+    """Set config's key by its path
+
+    ### Args:
+        * key (`str`): Key to delete
+        * *path (`str`): Path to the key of the target
+        * config_file (`Union[str, Path]`, *optional*): Path-like object or path as a string of a location of the config file. Defaults to `"config.json"`
+
+    ### Raises:
+        * `KeyError`: Key is not found under path provided
+    """
+    config_data = await json_read(config_file)
+
+    nested_delete(config_data, *(*path, key))
+
+    await json_write(config_data, config_file)
```

### Comparing `libbot-3.1.0/src/libbot/errors/config.py` & `libbot-3.2.0/src/libbot/errors/config.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/src/libbot/i18n/__init__.py` & `libbot-3.2.0/src/libbot/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/src/libbot/i18n/classes/bot_locale.py` & `libbot-3.2.0/src/libbot/i18n/classes/bot_locale.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/src/libbot/i18n/sync/__init__.py` & `libbot-3.2.0/src/libbot/i18n/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/src/libbot/pycord/classes/bot.py` & `libbot-3.2.0/src/libbot/pycord/classes/bot.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/src/libbot/pyrogram/classes/client.py` & `libbot-3.2.0/src/libbot/pyrogram/classes/client.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/src/libbot/pyrogram/classes/commandset.py` & `libbot-3.2.0/src/libbot/pyrogram/classes/commandset.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/src/libbot.egg-info/PKG-INFO` & `libbot-3.2.0/src/libbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libbot
-Version: 3.1.0
+Version: 3.2.0
 Summary: Universal bot library with functions needed for basic Discord/Telegram bot development.
 Author: Profitroll
 License: GPLv3
 Project-URL: Source, https://git.end-play.xyz/profitroll/LibBotUniversal
 Project-URL: Documentation, https://git.end-play.xyz/profitroll/LibBotUniversal/wiki
 Project-URL: Tracker, https://git.end-play.xyz/profitroll/LibBotUniversal/issues
 Classifier: Development Status :: 3 - Alpha
@@ -22,18 +22,18 @@
 License-File: LICENSE
 Requires-Dist: aiofiles>=23.0.0
 Provides-Extra: dev
 Requires-Dist: black==24.4.2; extra == "dev"
 Requires-Dist: build==1.2.1; extra == "dev"
 Requires-Dist: isort==5.13.2; extra == "dev"
 Requires-Dist: mypy==1.10.0; extra == "dev"
-Requires-Dist: pylint==3.2.1; extra == "dev"
+Requires-Dist: pylint==3.2.2; extra == "dev"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "dev"
 Requires-Dist: pytest-cov==5.0.0; extra == "dev"
-Requires-Dist: pytest==8.2.0; extra == "dev"
+Requires-Dist: pytest==8.2.1; extra == "dev"
 Requires-Dist: tox==4.15.0; extra == "dev"
 Requires-Dist: types-aiofiles==23.2.0.20240403; extra == "dev"
 Requires-Dist: types-ujson==5.10.0.20240515; extra == "dev"
 Provides-Extra: pycord
 Requires-Dist: apscheduler~=3.10.4; extra == "pycord"
 Requires-Dist: py-cord~=2.5.0; extra == "pycord"
 Provides-Extra: pyrogram
```

### Comparing `libbot-3.1.0/src/libbot.egg-info/SOURCES.txt` & `libbot-3.2.0/src/libbot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 src/libbot/pycord/classes/__init__.py
 src/libbot/pycord/classes/bot.py
 src/libbot/pyrogram/classes/__init__.py
 src/libbot/pyrogram/classes/client.py
 src/libbot/pyrogram/classes/command.py
 src/libbot/pyrogram/classes/commandset.py
 src/libbot/sync/__init__.py
+src/libbot/sync/__main__.py
+src/libbot/sync/_nested.py
 tests/test_bot_locale.py
 tests/test_config_async.py
 tests/test_config_sync.py
 tests/test_i18n_async.py
 tests/test_i18n_sync.py
 tests/test_json_async.py
 tests/test_json_sync.py
```

### Comparing `libbot-3.1.0/tests/test_bot_locale.py` & `libbot-3.2.0/tests/test_bot_locale.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/tests/test_config_async.py` & `libbot-3.2.0/tests/test_config_async.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Any, List
 
 import pytest
 
-from libbot import config_get, config_set
+from libbot import config_delete, config_get, config_set, sync
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
     "args, expected",
     [
         (["locale"], "en"),
@@ -42,7 +42,19 @@
         ("locale", [], "en"),
         ("bot_token", ["bot"], "sample_token"),
     ],
 )
 async def test_config_set(key: str, path: List[str], value: Any, location_config: Path):
     await config_set(key, value, *path, config_file=location_config)
     assert await config_get(key, *path, config_file=location_config) == value
+
+
+@pytest.mark.asyncio
+@pytest.mark.parametrize(
+    "key, path",
+    [
+        ("bot_token", ["bot"]),
+    ],
+)
+async def test_config_delete(key: str, path: List[str], location_config: Path):
+    await config_delete(key, *path, config_file=location_config)
+    assert key not in (await config_get(*path, config_file=location_config))
```

### Comparing `libbot-3.1.0/tests/test_config_sync.py` & `libbot-3.2.0/tests/test_config_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,7 +36,18 @@
         ("locale", [], "en"),
         ("bot_token", ["bot"], "sample_token"),
     ],
 )
 def test_config_set(key: str, path: List[str], value: Any, location_config: Path):
     sync.config_set(key, value, *path, config_file=location_config)
     assert sync.config_get(key, *path, config_file=location_config) == value
+
+
+@pytest.mark.parametrize(
+    "key, path",
+    [
+        ("bot_token", ["bot"]),
+    ],
+)
+def test_config_delete(key: str, path: List[str], location_config: Path):
+    sync.config_delete(key, *path, config_file=location_config)
+    assert key not in sync.config_get(*path, config_file=location_config)
```

### Comparing `libbot-3.1.0/tests/test_i18n_async.py` & `libbot-3.2.0/tests/test_i18n_async.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/tests/test_i18n_sync.py` & `libbot-3.2.0/tests/test_i18n_sync.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/tests/test_json_async.py` & `libbot-3.2.0/tests/test_json_async.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/tests/test_json_sync.py` & `libbot-3.2.0/tests/test_json_sync.py`

 * *Files identical despite different names*

### Comparing `libbot-3.1.0/tests/test_nested_set.py` & `libbot-3.2.0/tests/test_nested_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, List
 
 import pytest
 
-from libbot import sync
+from libbot.sync._nested import nested_delete, nested_set
 
 
 @pytest.mark.parametrize(
     "target, value, path, create_missing, expected",
     [
         ({"foo": "bar"}, "rab", ["foo"], True, {"foo": "rab"}),
         ({"foo": "bar"}, {"123": 456}, ["foo"], True, {"foo": {"123": 456}}),
@@ -29,17 +29,15 @@
 def test_nested_set_valid(
     target: Dict[str, Any],
     value: Any,
     path: List[str],
     create_missing: bool,
     expected: Any,
 ):
-    assert (
-        sync.nested_set(target, value, *path, create_missing=create_missing)
-    ) == expected
+    assert (nested_set(target, value, *path, create_missing=create_missing)) == expected
 
 
 @pytest.mark.parametrize(
     "target, value, path, create_missing, expected",
     [
         (
             {"foo": {"bar": {}}},
@@ -55,9 +53,29 @@
     value: Any,
     path: List[str],
     create_missing: bool,
     expected: Any,
 ):
     with pytest.raises(expected):
         assert (
-            sync.nested_set(target, value, *path, create_missing=create_missing)
+            nested_set(target, value, *path, create_missing=create_missing)
         ) == expected
+
+
+@pytest.mark.parametrize(
+    "target, path, expected",
+    [
+        ({"foo": "bar"}, ["foo"], {}),
+        ({"foo": "bar", "bar": "foo"}, ["bar"], {"foo": "bar"}),
+        (
+            {"foo": {"bar": {}}},
+            ["foo", "bar"],
+            {"foo": {}},
+        ),
+    ],
+)
+def test_nested_delete(
+    target: Dict[str, Any],
+    path: List[str],
+    expected: Any,
+):
+    assert (nested_delete(target, *path)) == expected
```

