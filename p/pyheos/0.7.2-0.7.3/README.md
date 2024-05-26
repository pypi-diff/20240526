# Comparing `tmp/pyheos-0.7.2.tar.gz` & `tmp/pyheos-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyheos-0.7.2.tar", last modified: Sat Nov 14 19:51:58 2020, max compression
+gzip compressed data, was "pyheos-0.7.3.tar", last modified: Sun May 26 14:32:56 2024, max compression
```

## Comparing `pyheos-0.7.2.tar` & `pyheos-0.7.3.tar`

### file list

```diff
@@ -1,23 +1,31 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-14 19:51:58.933050 pyheos-0.7.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4431 2020-11-14 19:51:58.933050 pyheos-0.7.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3259 2020-11-14 19:51:17.000000 pyheos-0.7.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-14 19:51:58.933050 pyheos-0.7.2/pyheos/
--rw-rw-r--   0 travis    (2000) travis    (2000)      544 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11738 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/command.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13067 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/connection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8515 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/const.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3015 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/dispatch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1783 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/error.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3854 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/group.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9231 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/heos.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15283 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/player.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3028 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/response.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4106 2020-11-14 19:51:17.000000 pyheos-0.7.2/pyheos/source.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-14 19:51:58.933050 pyheos-0.7.2/pyheos.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4431 2020-11-14 19:51:58.000000 pyheos-0.7.2/pyheos.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      360 2020-11-14 19:51:58.000000 pyheos-0.7.2/pyheos.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-14 19:51:58.000000 pyheos-0.7.2/pyheos.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-14 19:51:58.000000 pyheos-0.7.2/pyheos.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        7 2020-11-14 19:51:58.000000 pyheos-0.7.2/pyheos.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-11-14 19:51:58.933050 pyheos-0.7.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1295 2020-11-14 19:51:17.000000 pyheos-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:32:56.459844 pyheos-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-05-26 14:32:43.000000 pyheos-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-26 14:32:56.459844 pyheos-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-26 14:32:43.000000 pyheos-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:32:56.455844 pyheos-0.7.3/pyheos/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/heos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-26 14:32:43.000000 pyheos-0.7.3/pyheos/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:32:56.459844 pyheos-0.7.3/pyheos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-26 14:32:56.000000 pyheos-0.7.3/pyheos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 14:32:56.459844 pyheos-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-26 14:32:43.000000 pyheos-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:32:56.455844 pyheos-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30212 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_heos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-26 14:32:43.000000 pyheos-0.7.3/tests/test_source.py
```

### Comparing `pyheos-0.7.2/PKG-INFO` & `pyheos-0.7.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 Metadata-Version: 2.1
 Name: pyheos
-Version: 0.7.2
+Version: 0.7.3
 Summary: An async python library for controlling HEOS devices through the HEOS CLI Protocol
 Home-page: https://github.com/andrewsayre/pyheos
 Author: Andrew Sayre
 Author-email: andrew@sayre.net
 License: ASL 2.0
-Description: # pyheos
-        [![Build Status](https://travis-ci.org/andrewsayre/pyheos.svg?branch=master)](https://travis-ci.org/andrewsayre/pyheos)
-        [![Coverage Status](https://coveralls.io/repos/github/andrewsayre/pyheos/badge.svg?branch=master)](https://coveralls.io/github/andrewsayre/pyheos?branch=master)
-        [![image](https://img.shields.io/pypi/v/pyheos.svg)](https://pypi.org/project/pyheos/)
-        [![image](https://img.shields.io/pypi/pyversions/pyheos.svg)](https://pypi.org/project/pyheos/)
-        [![image](https://img.shields.io/pypi/l/pyheos.svg)](https://pypi.org/project/pyheos/)
-        [![image](https://img.shields.io/badge/Reviewed_by-Hound-8E64B0.svg)](https://houndci.com)
-        
-        An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.14 for players with firmware 1.505.140 or newer).
-        
-        ## Installation
-        ```bash
-        pip install pyheos
-        ```
-        or
-        ```bash
-        pip install --use-wheel pyheos
-        ```
-        
-        ## Getting Started
-        
-        The `Heos` class is the implementation providing control to all HEOS compatible devices on the local network through a single network connection.  It is suggested to connect to a device that is hard-wired.
-        
-        #### `pyheos.Heos(host, *, timeout, heart_beat, all_progress_events, dispatcher)`
-        - `host: str`: The IP Address or hostname of a HEOS device on the local network. This parameter is required.
-        - `timeout: float`: Number of seconds to wait during connection and issuing commands. Default is `pyheos.const.DEFAULT_TIMEOUT = 5.0`.  This parameter is required.
-        - `heart_beat: Optional[float]`: Number of seconds since last activity to issue a heart-beat command. Default is `pyheos.const.DEFAULT_HEART_BEAT = 60.0`.  Set this parameter to `None` to disable heart-beat.
-        - `all_progress_events`: Set to `True` to receive signals for each media play-back progression or `False` to only receive a signal when media state transitions to playing or changes.  Default is `True`.  This parameter is required.
-        - `dispatcher: Optional[pyheos.Dispatcher]`: An instance of dispatcher to use for raising signals.  The default is `None` which results in use of the default dispatcher implementation.
-        
-        #### `pyheos.Heos.connect(*, auto_reconnect, reconnect_delay)`
-        
-        Connect to the specified host.  This method is a coroutine.
-        - `auto_reconnect: bool`: Set to `True` to automatically reconnect to the host upon disconnection.  The default is `False`.
-        - `reconnect_delay: float`: The number of seconds to wait before attempting to reconnect upon a connection failure. The default is `DEFAULT_RECONNECT_DELAY = 5.0`
-        
-        #### `pyheos.Heos.disconnect()`
-        
-        Disconnect from the specified host.  This method is a coroutine.
-        
-        #### `pyheos.Heos.get_players(*, refresh)`
-        
-        Retrieve the available players as a `Dict[int, pyheos.Heos.HeosPlayer]` where the key represents the `player_id` and the value the `HeosPlayer` instance.  This method is a coroutine.  This method will populate the `players` property and will begin tracking changes to the players.
-        - `refresh`: Set to `True` to retrieve the latest available players from the CLI. The default is `False` and will return the previous loaded players.
-        
-        ##### Example:
-        ```python
-        import pyheos
-        
-        heos = Heos('172.16.0.1')
-        
-        await heos.connect(auto_reconnect=True)
-        players = await heos.get_players()
-        ...
-        await heos.disconnect()
-        ```
 Keywords: heos
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyheos
+[![CI Status](https://github.com/andrewsayre/pyheos/workflows/CI/badge.svg)](https://github.com/andrewsayre/pyheos/actions)
+[![codecov](https://codecov.io/github/andrewsayre/pyheos/graph/badge.svg?token=PV4P3AN7Z1)](https://codecov.io/github/andrewsayre/pyheos)
+[![image](https://img.shields.io/pypi/v/pyheos.svg)](https://pypi.org/project/pyheos/)
+[![image](https://img.shields.io/pypi/pyversions/pyheos.svg)](https://pypi.org/project/pyheos/)
+[![image](https://img.shields.io/pypi/l/pyheos.svg)](https://pypi.org/project/pyheos/)
+
+An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.14 for players with firmware 1.505.140 or newer).
+
+## Installation
+```bash
+pip install pyheos
+```
+or
+```bash
+pip install --use-wheel pyheos
+```
+
+## Getting Started
+
+The `Heos` class is the implementation providing control to all HEOS compatible devices on the local network through a single network connection.  It is suggested to connect to a device that is hard-wired.
+
+#### `pyheos.Heos(host, *, timeout, heart_beat, all_progress_events, dispatcher)`
+- `host: str`: The IP Address or hostname of a HEOS device on the local network. This parameter is required.
+- `timeout: float`: Number of seconds to wait during connection and issuing commands. Default is `pyheos.const.DEFAULT_TIMEOUT = 5.0`.  This parameter is required.
+- `heart_beat: Optional[float]`: Number of seconds since last activity to issue a heart-beat command. Default is `pyheos.const.DEFAULT_HEART_BEAT = 60.0`.  Set this parameter to `None` to disable heart-beat.
+- `all_progress_events`: Set to `True` to receive signals for each media play-back progression or `False` to only receive a signal when media state transitions to playing or changes.  Default is `True`.  This parameter is required.
+- `dispatcher: Optional[pyheos.Dispatcher]`: An instance of dispatcher to use for raising signals.  The default is `None` which results in use of the default dispatcher implementation.
+
+#### `pyheos.Heos.connect(*, auto_reconnect, reconnect_delay)`
+
+Connect to the specified host.  This method is a coroutine.
+- `auto_reconnect: bool`: Set to `True` to automatically reconnect to the host upon disconnection.  The default is `False`.
+- `reconnect_delay: float`: The number of seconds to wait before attempting to reconnect upon a connection failure. The default is `DEFAULT_RECONNECT_DELAY = 5.0`
+
+#### `pyheos.Heos.disconnect()`
+
+Disconnect from the specified host.  This method is a coroutine.
+
+#### `pyheos.Heos.get_players(*, refresh)`
+
+Retrieve the available players as a `Dict[int, pyheos.Heos.HeosPlayer]` where the key represents the `player_id` and the value the `HeosPlayer` instance.  This method is a coroutine.  This method will populate the `players` property and will begin tracking changes to the players.
+- `refresh`: Set to `True` to retrieve the latest available players from the CLI. The default is `False` and will return the previous loaded players.
+
+##### Example:
+```python
+import pyheos
+
+heos = Heos('172.16.0.1')
+
+await heos.connect(auto_reconnect=True)
+players = await heos.get_players()
+...
+await heos.disconnect()
+```
```

### Comparing `pyheos-0.7.2/README.md` & `pyheos-0.7.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # pyheos
-[![Build Status](https://travis-ci.org/andrewsayre/pyheos.svg?branch=master)](https://travis-ci.org/andrewsayre/pyheos)
-[![Coverage Status](https://coveralls.io/repos/github/andrewsayre/pyheos/badge.svg?branch=master)](https://coveralls.io/github/andrewsayre/pyheos?branch=master)
+[![CI Status](https://github.com/andrewsayre/pyheos/workflows/CI/badge.svg)](https://github.com/andrewsayre/pyheos/actions)
+[![codecov](https://codecov.io/github/andrewsayre/pyheos/graph/badge.svg?token=PV4P3AN7Z1)](https://codecov.io/github/andrewsayre/pyheos)
 [![image](https://img.shields.io/pypi/v/pyheos.svg)](https://pypi.org/project/pyheos/)
 [![image](https://img.shields.io/pypi/pyversions/pyheos.svg)](https://pypi.org/project/pyheos/)
 [![image](https://img.shields.io/pypi/l/pyheos.svg)](https://pypi.org/project/pyheos/)
-[![image](https://img.shields.io/badge/Reviewed_by-Hound-8E64B0.svg)](https://houndci.com)
 
 An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.14 for players with firmware 1.505.140 or newer).
 
 ## Installation
 ```bash
 pip install pyheos
 ```
```

### Comparing `pyheos-0.7.2/pyheos/__init__.py` & `pyheos-0.7.3/pyheos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pyheos - a library for interacting with HEOS devices."""
+
 from . import const
 from .dispatch import Dispatcher
 from .error import CommandError, CommandFailedError, HeosError
 from .group import HeosGroup
 from .heos import Heos
 from .player import HeosNowPlayingMedia, HeosPlayer
 from .source import HeosSource, InputSource
```

### Comparing `pyheos-0.7.2/pyheos/command.py` & `pyheos-0.7.3/pyheos/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define the HEOS command module."""
+
 from typing import Optional, Sequence, Tuple
 
 from . import const
 
 
 class HeosCommands:
     """Define a class that encapsulates well-known commands."""
```

### Comparing `pyheos-0.7.2/pyheos/connection.py` & `pyheos-0.7.3/pyheos/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Define the connection module."""
 
 import asyncio
 from collections import defaultdict
 from datetime import datetime, timedelta
 import json
 import logging
-from typing import Any, DefaultDict, Dict, List, Optional
+from typing import Any, Dict, Optional
 
 from . import const
 from .command import HeosCommands
 from .error import CommandError, HeosError, format_error_message
 from .response import HeosResponse
 
 SEPARATOR = "\r\n"
@@ -31,15 +31,15 @@
 
 
 def _encode_query(items: dict, *, mask=False) -> str:
     """Encode a dict to query string per CLI specifications."""
     pairs = []
     for key in sorted(items.keys()):
         value = _MASK if mask and key in _MASKED_PARAMS else items[key]
-        item = "{}={}".format(key, _quote(value))
+        item = f"{key}={_quote(value)}"
         # Ensure 'url' goes last per CLI spec
         if key == "url":
             pairs.append(item)
         else:
             pairs.insert(0, item)
     return "&".join(pairs)
 
@@ -50,15 +50,15 @@
     def __init__(
         self,
         heos,
         host: str,
         *,
         timeout: float = const.DEFAULT_TIMEOUT,
         heart_beat: Optional[float] = const.DEFAULT_HEART_BEAT,
-        all_progress_events=True
+        all_progress_events=True,
     ):
         """Init a new HeosConnection class."""
         self._heos = heos
         self._all_progress_events = all_progress_events
         self.host = host  # type: str
         self.commands = HeosCommands(self)
         self.timeout = timeout  # type: int
@@ -77,15 +77,15 @@
         self._heart_beat_interval = heart_beat  # type: Optional[float]
         self._heart_beat_task = None  # type: asyncio.Task
 
     async def connect(
         self,
         *,
         auto_reconnect: bool = False,
-        reconnect_delay: float = const.DEFAULT_RECONNECT_DELAY
+        reconnect_delay: float = const.DEFAULT_RECONNECT_DELAY,
     ):
         """Invoke the connect operation."""
         if self._state == const.STATE_CONNECTED:
             return
         # Ensure we don't try to reconnect during initial failures
         self._auto_reconnect = False
         await self._connect()
@@ -183,15 +183,15 @@
                 return
 
     async def _response_handler(self):
         while True:
             # Wait for response
             try:
                 result = await self._reader.readuntil(SEPARATOR_BYTES)
-                self._last_activity = datetime.utcnow()
+                self._last_activity = datetime.now()
                 data = json.loads(result.decode())
                 response = HeosResponse(data)
 
                 # Ignore processing
                 if response.is_under_process:
                     _LOGGER.debug(
                         "Command under process '%s': '%s'", response.command, data
@@ -232,15 +232,15 @@
             ) as error:
                 # Occurs when the connection breaks
                 asyncio.ensure_future(self._handle_connection_error(error))
                 return
 
     async def _heart_beat(self):
         while self._state == const.STATE_CONNECTED:
-            last_activity = datetime.utcnow() - self._last_activity
+            last_activity = datetime.now() - self._last_activity
             threshold = timedelta(seconds=self._heart_beat_interval)
             if last_activity > threshold:
                 try:
                     await self.commands.heart_beat()
                 except CommandError:
                     pass
             await asyncio.sleep(self._heart_beat_interval / 2)
@@ -250,18 +250,16 @@
     ) -> HeosResponse:
         """Execute a command and get it's response."""
         # Build command URI
         sequence = self._sequence
         self._sequence += 1
         params = params or {}
         params["sequence"] = sequence
-        uri = "{}{}?{}".format(const.BASE_URI, command, _encode_query(params))
-        masked_uri = "{}{}?{}".format(
-            const.BASE_URI, command, _encode_query(params, mask=True)
-        )
+        uri = f"{const.BASE_URI}{command}?{_encode_query(params)}"
+        masked_uri = f"{const.BASE_URI}{command}?{_encode_query(params, mask=True)}"
 
         if self._state != const.STATE_CONNECTED:
             _LOGGER.debug(
                 "Command failed '%s': %s", masked_uri, "Not connected to device"
             )
             raise CommandError(command, "Not connected to device")
```

### Comparing `pyheos-0.7.2/pyheos/const.py` & `pyheos-0.7.3/pyheos/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Define consts for the pyheos package."""
 
 __title__ = "pyheos"
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 CLI_PORT = 1255
 DEFAULT_TIMEOUT = 10.0
 DEFAULT_RECONNECT_DELAY = 10.0
 DEFAULT_HEART_BEAT = 10.0
 DEFAULT_STEP = 5
```

### Comparing `pyheos-0.7.2/pyheos/dispatch.py` & `pyheos-0.7.3/pyheos/dispatch.py`

 * *Files identical despite different names*

### Comparing `pyheos-0.7.2/pyheos/error.py` & `pyheos-0.7.3/pyheos/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define the error module for HEOS."""
+
 import asyncio
 
 DEFAULT_ERROR_MESSAGES = {
     asyncio.TimeoutError: "Command timed out",
     ConnectionError: "Connection error",
     BrokenPipeError: "Broken pipe",
     ConnectionAbortedError: "Connection aborted",
@@ -44,15 +45,15 @@
     """Define an error when a HEOS command fails."""
 
     def __init__(self, command: str, text: str, error_id: int):
         """Create a new instance of the error."""
         self._command = command
         self._error_text = text
         self._error_id = error_id
-        super().__init__(command, "{} ({})".format(text, error_id))
+        super().__init__(command, f"{text} ({error_id})")
 
     @property
     def error_text(self) -> str:
         """Get the error text from the response."""
         return self._error_text
 
     @property
```

### Comparing `pyheos-0.7.2/pyheos/group.py` & `pyheos-0.7.3/pyheos/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define the heos group module."""
+
 import asyncio
 from typing import Dict, Sequence
 
 from . import const
 from .player import HeosPlayer
 from .response import HeosResponse
```

### Comparing `pyheos-0.7.2/pyheos/heos.py` & `pyheos-0.7.3/pyheos/heos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define the heos manager module."""
+
 import asyncio
 from typing import Dict, Optional, Sequence
 
 from . import const
 from .connection import HeosConnection
 from .dispatch import Dispatcher
 from .group import HeosGroup, create_group
```

### Comparing `pyheos-0.7.2/pyheos/player.py` & `pyheos-0.7.3/pyheos/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Define the player module."""
+
 import asyncio
 from datetime import datetime
-from typing import Dict, Optional, Sequence
+from typing import Dict, Optional
 
 from . import const
 from .response import HeosResponse
 from .source import HeosSource, InputSource
 
 
 def parse_player_id(data: dict) -> int:
@@ -72,15 +73,15 @@
 
     def event_update_progress(
         self, event: HeosResponse, all_progress_events: bool
     ) -> bool:
         """Update the position/duration from an event."""
         if all_progress_events or self._current_position is None:
             self._current_position = int(event.get_message("cur_pos"))
-            self._current_position_updated = datetime.utcnow()
+            self._current_position_updated = datetime.now()
             self._duration = int(event.get_message("duration"))
             return True
         return False
 
     def clear_progress(self):
         """Clear the current position."""
         self._current_position = None
@@ -182,21 +183,19 @@
         self._shuffle = None  # type: bool
         self._playback_error = None  # type: str
         self._now_playing_media = HeosNowPlayingMedia()
         self._available = True  # type: bool
 
     def __str__(self):
         """Get a user-readable representation of the player."""
-        return "{{{} ({})}}".format(self._name, self._model)
+        return f"{{{self._name} ({self._model})}}"
 
     def __repr__(self):
         """Get a debug representation of the player."""
-        return "{{{} ({}) with id {} at {}}}".format(
-            self.name, self._model, self._player_id, self._ip_address
-        )
+        return f"{{{self.name} ({self._model}) with id {self._player_id} at {self._ip_address}}}"
 
     def from_data(self, data: dict):
         """Update the attributes from the supplied data."""
         self._name = parse_player_name(data)
         self._player_id = parse_player_id(data)
         self._model = data["model"]
         self._version = parse_player_version(data)
@@ -328,15 +327,15 @@
     async def play_quick_select(self, quick_select_id: int):
         """Play the specified quick select."""
         await self._commands.play_quick_select(self._player_id, quick_select_id)
 
     async def add_to_queue(self, source: HeosSource, add_queue_option: int):
         """Add the specified source to the queue."""
         if not source.playable:
-            raise ValueError("Source '{}' is not playable".format(source))
+            raise ValueError(f"Source '{source}' is not playable")
         await self._commands.add_to_queue(
             self._player_id,
             source.source_id,
             source.container_id,
             add_queue_option,
             source.media_id,
         )
```

### Comparing `pyheos-0.7.2/pyheos/response.py` & `pyheos-0.7.3/pyheos/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define the heos response module."""
+
 from typing import Any, Dict, Optional
 from urllib.parse import parse_qsl
 
 from .error import CommandFailedError
 
 
 class HeosResponse:
@@ -16,19 +17,19 @@
         self._message = None  # type: dict
         self._payload = None  # type: dict
         if data:
             self.from_json(data)
 
     def __str__(self):
         """Get a user-readable representation of the response."""
-        return "{}".format(self._raw_data["heos"])
+        return str(self._raw_data["heos"])
 
     def __repr__(self):
         """Get a debug representation of the player."""
-        return "{}".format(self._raw_data)
+        return str(self._raw_data)
 
     def from_json(self, data: dict):
         """Populate the response from json."""
         self._raw_data = data
         heos = data["heos"]
         self._command = heos["command"]
         self._result = heos.get("result") == "success"
```

### Comparing `pyheos-0.7.2/pyheos/source.py` & `pyheos-0.7.3/pyheos/source.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Define the heos source module."""
+
 from typing import Optional, Sequence  # pylint: disable=unused-import
 
 
 class InputSource:
     """Define an input source."""
 
     def __init__(self, player_id: int, name: str, input_name: str):
         """Init the source."""
         self._player_id = player_id  # type: int
         self._name = name  # type: str
         self._input_name = input_name  # type: str
 
     def __str__(self):
         """Get a user-readable representation of the source."""
-        return "<{} ({})>".format(self._name, self._input_name)
+        return f"<{self._name} ({self._input_name})>"
 
     def __repr__(self):
         """Get a debug representation of the source."""
-        return "<{} ({}) on {}>".format(self._name, self._input_name, self._player_id)
+        return f"<{self._name} ({self._input_name}) on {self._player_id}>"
 
     @property
     def name(self) -> str:
         """Get the friendly display name."""
         return self._name
 
     @property
@@ -68,19 +69,19 @@
         self._container = data.get("container") == "yes"
         self._container_id = data.get("cid")
         self._media_id = data.get("mid")
         self._playable = data.get("playable") == "yes"
 
     def __str__(self):
         """Get a user-readable representation of the source."""
-        return "<{} ({})>".format(self._name, self._type)
+        return f"<{self._name} ({self._type})>"
 
     def __repr__(self):
         """Get a debug representation of the source."""
-        return "<{} ({}) {}>".format(self._name, self._type, self._source_id)
+        return f"<{self._name} ({self._type}) {self._source_id}>"
 
     async def browse(self) -> "Sequence[HeosSource]":
         """Browse the contents of the current source."""
         items = await self._commands.browse(self._source_id)
         return [HeosSource(self._commands, item) for item in items]
 
     @property
```

### Comparing `pyheos-0.7.2/pyheos.egg-info/PKG-INFO` & `pyheos-0.7.3/pyheos.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 Metadata-Version: 2.1
 Name: pyheos
-Version: 0.7.2
+Version: 0.7.3
 Summary: An async python library for controlling HEOS devices through the HEOS CLI Protocol
 Home-page: https://github.com/andrewsayre/pyheos
 Author: Andrew Sayre
 Author-email: andrew@sayre.net
 License: ASL 2.0
-Description: # pyheos
-        [![Build Status](https://travis-ci.org/andrewsayre/pyheos.svg?branch=master)](https://travis-ci.org/andrewsayre/pyheos)
-        [![Coverage Status](https://coveralls.io/repos/github/andrewsayre/pyheos/badge.svg?branch=master)](https://coveralls.io/github/andrewsayre/pyheos?branch=master)
-        [![image](https://img.shields.io/pypi/v/pyheos.svg)](https://pypi.org/project/pyheos/)
-        [![image](https://img.shields.io/pypi/pyversions/pyheos.svg)](https://pypi.org/project/pyheos/)
-        [![image](https://img.shields.io/pypi/l/pyheos.svg)](https://pypi.org/project/pyheos/)
-        [![image](https://img.shields.io/badge/Reviewed_by-Hound-8E64B0.svg)](https://houndci.com)
-        
-        An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.14 for players with firmware 1.505.140 or newer).
-        
-        ## Installation
-        ```bash
-        pip install pyheos
-        ```
-        or
-        ```bash
-        pip install --use-wheel pyheos
-        ```
-        
-        ## Getting Started
-        
-        The `Heos` class is the implementation providing control to all HEOS compatible devices on the local network through a single network connection.  It is suggested to connect to a device that is hard-wired.
-        
-        #### `pyheos.Heos(host, *, timeout, heart_beat, all_progress_events, dispatcher)`
-        - `host: str`: The IP Address or hostname of a HEOS device on the local network. This parameter is required.
-        - `timeout: float`: Number of seconds to wait during connection and issuing commands. Default is `pyheos.const.DEFAULT_TIMEOUT = 5.0`.  This parameter is required.
-        - `heart_beat: Optional[float]`: Number of seconds since last activity to issue a heart-beat command. Default is `pyheos.const.DEFAULT_HEART_BEAT = 60.0`.  Set this parameter to `None` to disable heart-beat.
-        - `all_progress_events`: Set to `True` to receive signals for each media play-back progression or `False` to only receive a signal when media state transitions to playing or changes.  Default is `True`.  This parameter is required.
-        - `dispatcher: Optional[pyheos.Dispatcher]`: An instance of dispatcher to use for raising signals.  The default is `None` which results in use of the default dispatcher implementation.
-        
-        #### `pyheos.Heos.connect(*, auto_reconnect, reconnect_delay)`
-        
-        Connect to the specified host.  This method is a coroutine.
-        - `auto_reconnect: bool`: Set to `True` to automatically reconnect to the host upon disconnection.  The default is `False`.
-        - `reconnect_delay: float`: The number of seconds to wait before attempting to reconnect upon a connection failure. The default is `DEFAULT_RECONNECT_DELAY = 5.0`
-        
-        #### `pyheos.Heos.disconnect()`
-        
-        Disconnect from the specified host.  This method is a coroutine.
-        
-        #### `pyheos.Heos.get_players(*, refresh)`
-        
-        Retrieve the available players as a `Dict[int, pyheos.Heos.HeosPlayer]` where the key represents the `player_id` and the value the `HeosPlayer` instance.  This method is a coroutine.  This method will populate the `players` property and will begin tracking changes to the players.
-        - `refresh`: Set to `True` to retrieve the latest available players from the CLI. The default is `False` and will return the previous loaded players.
-        
-        ##### Example:
-        ```python
-        import pyheos
-        
-        heos = Heos('172.16.0.1')
-        
-        await heos.connect(auto_reconnect=True)
-        players = await heos.get_players()
-        ...
-        await heos.disconnect()
-        ```
 Keywords: heos
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyheos
+[![CI Status](https://github.com/andrewsayre/pyheos/workflows/CI/badge.svg)](https://github.com/andrewsayre/pyheos/actions)
+[![codecov](https://codecov.io/github/andrewsayre/pyheos/graph/badge.svg?token=PV4P3AN7Z1)](https://codecov.io/github/andrewsayre/pyheos)
+[![image](https://img.shields.io/pypi/v/pyheos.svg)](https://pypi.org/project/pyheos/)
+[![image](https://img.shields.io/pypi/pyversions/pyheos.svg)](https://pypi.org/project/pyheos/)
+[![image](https://img.shields.io/pypi/l/pyheos.svg)](https://pypi.org/project/pyheos/)
+
+An async python library for controlling HEOS devices through the HEOS CLI Protocol (version 1.14 for players with firmware 1.505.140 or newer).
+
+## Installation
+```bash
+pip install pyheos
+```
+or
+```bash
+pip install --use-wheel pyheos
+```
+
+## Getting Started
+
+The `Heos` class is the implementation providing control to all HEOS compatible devices on the local network through a single network connection.  It is suggested to connect to a device that is hard-wired.
+
+#### `pyheos.Heos(host, *, timeout, heart_beat, all_progress_events, dispatcher)`
+- `host: str`: The IP Address or hostname of a HEOS device on the local network. This parameter is required.
+- `timeout: float`: Number of seconds to wait during connection and issuing commands. Default is `pyheos.const.DEFAULT_TIMEOUT = 5.0`.  This parameter is required.
+- `heart_beat: Optional[float]`: Number of seconds since last activity to issue a heart-beat command. Default is `pyheos.const.DEFAULT_HEART_BEAT = 60.0`.  Set this parameter to `None` to disable heart-beat.
+- `all_progress_events`: Set to `True` to receive signals for each media play-back progression or `False` to only receive a signal when media state transitions to playing or changes.  Default is `True`.  This parameter is required.
+- `dispatcher: Optional[pyheos.Dispatcher]`: An instance of dispatcher to use for raising signals.  The default is `None` which results in use of the default dispatcher implementation.
+
+#### `pyheos.Heos.connect(*, auto_reconnect, reconnect_delay)`
+
+Connect to the specified host.  This method is a coroutine.
+- `auto_reconnect: bool`: Set to `True` to automatically reconnect to the host upon disconnection.  The default is `False`.
+- `reconnect_delay: float`: The number of seconds to wait before attempting to reconnect upon a connection failure. The default is `DEFAULT_RECONNECT_DELAY = 5.0`
+
+#### `pyheos.Heos.disconnect()`
+
+Disconnect from the specified host.  This method is a coroutine.
+
+#### `pyheos.Heos.get_players(*, refresh)`
+
+Retrieve the available players as a `Dict[int, pyheos.Heos.HeosPlayer]` where the key represents the `player_id` and the value the `HeosPlayer` instance.  This method is a coroutine.  This method will populate the `players` property and will begin tracking changes to the players.
+- `refresh`: Set to `True` to retrieve the latest available players from the CLI. The default is `False` and will return the previous loaded players.
+
+##### Example:
+```python
+import pyheos
+
+heos = Heos('172.16.0.1')
+
+await heos.connect(auto_reconnect=True)
+players = await heos.get_players()
+...
+await heos.disconnect()
+```
```

### Comparing `pyheos-0.7.2/setup.py` & `pyheos-0.7.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     long_description_content_type="text/markdown",
     url="https://github.com/andrewsayre/pyheos",
     author="Andrew Sayre",
     author_email="andrew@sayre.net",
     license="ASL 2.0",
     packages=find_packages(exclude=("tests", "tests.*")),
     install_requires=[],
-    tests_require=["tox>=3.5.0,<4.0.0"],
+    tests_require=[],
     platforms=["any"],
     keywords="heos",
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries",
         "Topic :: Home Automation",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

