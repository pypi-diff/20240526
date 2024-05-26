# Comparing `tmp/pyarcamsolo-0.0.5.tar.gz` & `tmp/pyarcamsolo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarcamsolo-0.0.5.tar", last modified: Fri Mar  8 20:18:46 2024, max compression
+gzip compressed data, was "pyarcamsolo-0.0.6.tar", last modified: Sun May 26 18:19:46 2024, max compression
```

## Comparing `pyarcamsolo-0.0.5.tar` & `pyarcamsolo-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:18:46.114252 pyarcamsolo-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-08 20:18:18.000000 pyarcamsolo-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-08 20:18:46.114252 pyarcamsolo-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-08 20:18:18.000000 pyarcamsolo-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:18:46.110252 pyarcamsolo-0.0.5/pyarcamsolo/
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-03-08 20:18:18.000000 pyarcamsolo-0.0.5/pyarcamsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-08 20:18:18.000000 pyarcamsolo-0.0.5/pyarcamsolo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-08 20:18:18.000000 pyarcamsolo-0.0.5/pyarcamsolo/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-03-08 20:18:18.000000 pyarcamsolo-0.0.5/pyarcamsolo/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-08 20:18:18.000000 pyarcamsolo-0.0.5/pyarcamsolo/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 20:18:46.114252 pyarcamsolo-0.0.5/pyarcamsolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-03-08 20:18:46.000000 pyarcamsolo-0.0.5/pyarcamsolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-08 20:18:46.000000 pyarcamsolo-0.0.5/pyarcamsolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 20:18:46.000000 pyarcamsolo-0.0.5/pyarcamsolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-08 20:18:46.000000 pyarcamsolo-0.0.5/pyarcamsolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-08 20:18:46.000000 pyarcamsolo-0.0.5/pyarcamsolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-08 20:18:46.000000 pyarcamsolo-0.0.5/pyarcamsolo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-08 20:18:18.000000 pyarcamsolo-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 20:18:46.118252 pyarcamsolo-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-08 20:18:18.000000 pyarcamsolo-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/pyarcamsolo/
+-rw-r--r--   0 runner    (1001) docker     (127)    22522 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyarcamsolo/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 18:19:46.000000 pyarcamsolo-0.0.6/pyarcamsolo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 18:19:46.767363 pyarcamsolo-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-26 18:19:18.000000 pyarcamsolo-0.0.6/setup.py
```

### Comparing `pyarcamsolo-0.0.5/LICENSE` & `pyarcamsolo-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.0.5/PKG-INFO` & `pyarcamsolo-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.0.5
+Version: 0.0.6
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.0.5/README.md` & `pyarcamsolo-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.0.5/pyarcamsolo/__init__.py` & `pyarcamsolo-0.0.6/pyarcamsolo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,25 +97,29 @@
         )
 
     def set_zone_callback(
         self, zone: int, callback_id: uuid.UUID = None, callback: Callable[..., None] | None = None
     ) -> uuid.UUID | None:
         """Configure a zone callback."""
         if zone in self.zones:
+            self._zone_callbacks.setdefault(zone, {})
             if callback:
                 callback_id = uuid.uuid4()
-                self._zone_callbacks.setdefault(zone, {})
                 self._zone_callbacks[zone][callback_id] = callback
                 return callback_id
             elif callback_id:
-                self._zone_callbacks[zone].pop(callback_id)
-                return None
+                if callback_id in self._zone_callbacks[zone]:
+                    self._zone_callbacks[zone].pop(callback_id)
+                    return None
+                raise ValueError("Callback does not exist.")
             else:
-                self._zone_callbacks.pop(zone)
-                return None
+                if zone in self._zone_callbacks:
+                    self._zone_callbacks.pop(zone)
+                    return None
+                raise ValueError("Zone does not exist.")
 
     def _clear_zone_callbacks(self):
         """Clear any configured zone callbacks."""
         self._zone_callbacks = {}
 
     def _call_zone_callbacks(self, zone: int):
         """Call a configured callback."""
```

### Comparing `pyarcamsolo-0.0.5/pyarcamsolo/commands.py` & `pyarcamsolo-0.0.6/pyarcamsolo/commands.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.0.5/pyarcamsolo/parser.py` & `pyarcamsolo-0.0.6/pyarcamsolo/parser.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.0.5/pyarcamsolo/util.py` & `pyarcamsolo-0.0.6/pyarcamsolo/util.py`

 * *Files identical despite different names*

### Comparing `pyarcamsolo-0.0.5/pyarcamsolo.egg-info/PKG-INFO` & `pyarcamsolo-0.0.6/pyarcamsolo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarcamsolo
-Version: 0.0.5
+Version: 0.0.6
 Summary: Asyncio Python library for controlling Arcam Solo Hi-Fi devices via RS232 ser2net bridge.
 Home-page: http://github.com/pantherale0/pyarcamsolo
 Author: pantherale0
 License: MIT
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
```

### Comparing `pyarcamsolo-0.0.5/setup.py` & `pyarcamsolo-0.0.6/setup.py`

 * *Files identical despite different names*

