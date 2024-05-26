# Comparing `tmp/sakee-0.1.6.tar.gz` & `tmp/sakee-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakee-0.1.6.tar", last modified: Sat Oct 21 23:28:29 2023, max compression
+gzip compressed data, was "sakee-0.1.7.tar", last modified: Sun May 26 18:24:55 2024, max compression
```

## Comparing `sakee-0.1.6.tar` & `sakee-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 23:28:29.549717 sakee-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34915 2023-10-21 23:28:18.000000 sakee-0.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2023-10-21 23:28:29.549717 sakee-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2023-10-21 23:28:18.000000 sakee-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-10-21 23:28:18.000000 sakee-0.1.6/inputstreamhelper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 23:28:29.545717 sakee-0.1.6/sakee/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-21 23:28:18.000000 sakee-0.1.6/sakee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2023-10-21 23:28:18.000000 sakee-0.1.6/sakee/addoninfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-10-21 23:28:18.000000 sakee-0.1.6/sakee/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2023-10-21 23:28:18.000000 sakee-0.1.6/sakee/internalplayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2023-10-21 23:28:18.000000 sakee-0.1.6/sakee/pluginhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2023-10-21 23:28:18.000000 sakee-0.1.6/sakee/sakebuiltin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2023-10-21 23:28:18.000000 sakee-0.1.6/sakee/sakejsonrpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2023-10-21 23:28:18.000000 sakee-0.1.6/sakee/stub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 23:28:29.549717 sakee-0.1.6/sakee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2023-10-21 23:28:29.000000 sakee-0.1.6/sakee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-10-21 23:28:29.000000 sakee-0.1.6/sakee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 23:28:29.000000 sakee-0.1.6/sakee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 23:28:29.000000 sakee-0.1.6/sakee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-10-21 23:28:29.000000 sakee-0.1.6/sakee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-21 23:28:29.549717 sakee-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-10-21 23:28:18.000000 sakee-0.1.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27095 2023-10-21 23:28:18.000000 sakee-0.1.6/xbmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2023-10-21 23:28:18.000000 sakee-0.1.6/xbmcaddon.py
--rw-r--r--   0 runner    (1001) docker     (127)    29488 2023-10-21 23:28:18.000000 sakee-0.1.6/xbmcgui.py
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2023-10-21 23:28:18.000000 sakee-0.1.6/xbmcplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2023-10-21 23:28:18.000000 sakee-0.1.6/xbmcvfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:24:55.768744 sakee-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34915 2024-05-26 18:24:45.000000 sakee-0.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-26 18:24:55.768744 sakee-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-26 18:24:45.000000 sakee-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-26 18:24:45.000000 sakee-0.1.7/inputstreamhelper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:24:55.768744 sakee-0.1.7/sakee/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-26 18:24:45.000000 sakee-0.1.7/sakee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-26 18:24:45.000000 sakee-0.1.7/sakee/addoninfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-26 18:24:45.000000 sakee-0.1.7/sakee/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-26 18:24:45.000000 sakee-0.1.7/sakee/internalplayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-26 18:24:45.000000 sakee-0.1.7/sakee/pluginhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-26 18:24:45.000000 sakee-0.1.7/sakee/sakebuiltin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-26 18:24:45.000000 sakee-0.1.7/sakee/sakejsonrpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-26 18:24:45.000000 sakee-0.1.7/sakee/stub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:24:55.768744 sakee-0.1.7/sakee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-26 18:24:55.000000 sakee-0.1.7/sakee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-26 18:24:55.000000 sakee-0.1.7/sakee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:24:55.000000 sakee-0.1.7/sakee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:24:55.000000 sakee-0.1.7/sakee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-26 18:24:55.000000 sakee-0.1.7/sakee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 18:24:55.768744 sakee-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-26 18:24:45.000000 sakee-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:24:55.768744 sakee-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-26 18:24:45.000000 sakee-0.1.7/tests/test_kodistub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-26 18:24:45.000000 sakee-0.1.7/tests/test_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 18:24:45.000000 sakee-0.1.7/tests/test_xbmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-26 18:24:45.000000 sakee-0.1.7/tests/test_xbmc_executebuiltin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-26 18:24:45.000000 sakee-0.1.7/tests/test_xbmc_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-26 18:24:45.000000 sakee-0.1.7/tests/test_xbmcgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-26 18:24:45.000000 sakee-0.1.7/tests/test_xbmcvfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27095 2024-05-26 18:24:45.000000 sakee-0.1.7/xbmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13293 2024-05-26 18:24:45.000000 sakee-0.1.7/xbmcaddon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29904 2024-05-26 18:24:45.000000 sakee-0.1.7/xbmcgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-05-26 18:24:45.000000 sakee-0.1.7/xbmcplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-26 18:24:45.000000 sakee-0.1.7/xbmcvfs.py
```

### Comparing `sakee-0.1.6/LICENSE.md` & `sakee-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sakee-0.1.6/PKG-INFO` & `sakee-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sakee
-Version: 0.1.6
+Version: 0.1.7
 Summary: SAKÉ can help you to debug and develop Kodi Python add-ons
 Home-page: https://github.com/retrospect-addon/kodi.emulator.ascii
 Author: Bas Rieter
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/retrospect-addon/kodi.emulator.ascii/blob/master/README.md
 Project-URL: Source, https://github.com/retrospect-addon/kodi.emulator.ascii/
 Project-URL: Tracker, https://github.com/retrospect-addon/kodi.emulator.ascii/issues
```

### Comparing `sakee-0.1.6/README.md` & `sakee-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sakee-0.1.6/sakee/addoninfo.py` & `sakee-0.1.7/sakee/addoninfo.py`

 * *Files identical despite different names*

### Comparing `sakee-0.1.6/sakee/colors.py` & `sakee-0.1.7/sakee/colors.py`

 * *Files identical despite different names*

### Comparing `sakee-0.1.6/sakee/internalplayer.py` & `sakee-0.1.7/sakee/internalplayer.py`

 * *Files identical despite different names*

### Comparing `sakee-0.1.6/sakee/pluginhandler.py` & `sakee-0.1.7/sakee/pluginhandler.py`

 * *Files identical despite different names*

### Comparing `sakee-0.1.6/sakee/sakebuiltin.py` & `sakee-0.1.7/sakee/sakebuiltin.py`

 * *Files identical despite different names*

### Comparing `sakee-0.1.6/sakee/sakejsonrpc.py` & `sakee-0.1.7/sakee/sakejsonrpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -77,14 +77,57 @@
                 limits=dict(
                     start=0,
                     end=len(addons),
                     total=len(addons)
                 )
             )
 
+    # noinspection PyPep8Naming
+    class Favourites:
+        def __init__(self, addon_info):
+            """ Initialise the JSON RPC API Addons Namespace.
+
+            :param obj addon_info:   Information about the current Add-on paths.
+            """
+            self._ADDON_INFO = addon_info
+
+        def GetFavourites(self, **params):
+            favourites = os.path.join(self._ADDON_INFO.kodi_profile_path, "favourites.xml")
+            content = io.open(favourites, "r").read()
+            matches = re.findall(r'name="([^"]+)".*?>([^(]+)\((?:(\d+),)?&quot;([^<]+)&quot;', content)
+
+            result = {
+                "favourites": [],
+                "limits": {
+                    "end": 0,
+                    "start": 0,
+                    "total": 0
+                }
+            }
+            favs = result["favourites"]
+
+            for name, action, window_id, param in matches:
+                if action == "PlayMedia":
+                    action_type = "media"
+                elif action == "ActivateWindow":
+                    action_type = "window"
+                else:
+                    action_type = None
+
+                fav = {
+                    "title": name,
+                    "type": action_type,
+                    "windowparameter": param
+                }
+                favs.append(fav)
+
+            result["limits"]["end"] = len(favs)
+            result["limits"]["total"] = len(favs)
+            return result
+
     class Settings(object):
         """ Allows manipulation of Kodi settings. """
         __SETTINGS = None
 
         def __init__(self, addon_info):
             """ Initialise the JSON RPC API Settings Namespace.
```

### Comparing `sakee-0.1.6/sakee/stub.py` & `sakee-0.1.7/sakee/stub.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,122 +1,125 @@
 # SPDX-License-Identifier: GPL-3.0
 
 import os
 import re
 import sys
 import random
+from typing import Optional, Any
 
 from sakee.colors import Colors
 
 
 class KeyboardStub(object):
     def __init__(self):
         self.__id = random.random()
         self.__queue = []
         self.reset()
 
-    def add_input(self, line):
+    def add_input(self, line: str) -> None:
         self.__queue.append(line)
 
-    def clear_input(self):
+    def clear_input(self) -> None:
         self.__queue = []
 
-    def get_next_input(self):
+    def get_next_input(self) -> Optional[str]:
         if len(self.__queue) == 0:
             return None
 
         return self.__queue.pop(0)
 
-    def reset(self):
+    def reset(self) -> None:
         self.__queue = []
         line = os.environ.get("KODI_STUB_INPUT", None)
         if line:
             self.__queue.append(line)
 
 
 class KodiStub(object):
+    PY2: bool
+    PY3: bool
+
     __keyboard_stub = None
 
-    is_interactive = os.environ.get("KODI_INTERACTIVE", "1") == "1"
-    is_verbose = os.environ.get("KODI_STUB_VERBOSE", "0") == "1"
+    is_interactive: bool = os.environ.get("KODI_INTERACTIVE", "1") == "1"
+    is_verbose: bool = os.environ.get("KODI_STUB_VERBOSE", "0") == "1"
 
     def __init__(self):
         self.PY2 = sys.version_info[0] == 2
         self.PY3 = sys.version_info[0] == 3
 
-    def get_keyboard_stub(self):
+    def get_keyboard_stub(self) -> KeyboardStub:
         if KodiStub.__keyboard_stub is None:
             KodiStub.__keyboard_stub = KeyboardStub()
 
         return KodiStub.__keyboard_stub
 
-    def read_input(self, text, color=None):
+    def read_input(self, text: str, color: Optional[str] = None) -> str:
         """ Reads user's input from the console
 
-        :param str text:    Question for the input
+        :param text:    Question for the input
 
         :return: the read input
-        :rtype: str
 
         """
 
         text = "{} ".format(text)
 
         if color is not None:
             text = "{}{}{}".format(color, text, Colors.EndColor)
 
         # noinspection PyUnresolvedReferences
         return input(text) if self.PY3 else raw_input(text)
 
     @staticmethod
-    def print_heading(text, align_right=False, color=Colors.Yellow):
+    def print_heading(text: str, align_right: bool = False, color: str = Colors.Yellow) -> None:
         """ Aligns text over 120 chars
 
-        :param str text:            The Text to align
-        :param bool align_right:    Align right instead of left?
+        :param text:            The Text to show.
+        :param align_right:     Align right instead of left?
+        :param color:           The color to use.
 
-        :return: the aligned text
-        :rrtype: str
+        :return: The headline text.
 
         """
 
         if text == "":
             heading = "=" * 120
         elif not align_right:
             heading = "= {} {}".format(text, "=" * (120 - 3 - len(text)))
         else:
             heading = "{} {} =".format("=" * (120 - 3 - len(text)), text)
 
         KodiStub.print_line(heading, color=color)
 
     @staticmethod
-    def print_line(line, color=None, verbose=False):
+    def print_line(line: str, color: Optional[str] = None, verbose: bool = False) -> None:
         """ Prints a full line including colors
 
-        :param str line:        The line to print
-        :param str color:       The color to print (use Color)
-        :param bool verbose:    Is the line verbose data?
+        :param line:        The line to print
+        :param color:       The color to print (use Color)
+        :param verbose:     Is the line verbose data?
 
         """
 
         if verbose and not KodiStub.is_verbose:
             return
 
         if color:
             print(color + line + Colors.EndColor)
         else:
             print(line)
 
-    def log_method(self, code_module, name, *args, **kwargs):
+    def log_method(self, code_module: str, name: str, *args: Any, **kwargs: Any) -> None:
         """
 
-        :param str code_module: The module that called this method
-        :param str name:        The method that was callled
-        :param *args:           The arguments that were passed
-        :param **kwargs:        The keyword arguments that where passed
+        :param code_module:  The module that called this method
+        :param name:         The method that was callled
+        :param *args:        The arguments that were passed
+        :param **kwargs:     The keyword arguments that where passed
 
         :return: None
 
         """
 
         KodiStub.print_line("Call to missing: {0}.{1}".format(code_module, name), color=Colors.Blue, verbose=True)
         if not self.is_verbose:
@@ -128,20 +131,19 @@
             print("-> %s.%s(args=%s)" % (code_module, name, args))
         if args and kwargs:
             print("-> %s.%s(args=%s, kwargs=%s)" % (code_module, name, args, kwargs))
         if not args and kwargs:
             print("-> %s.%s(kwargs=%s)" % (code_module, name, kwargs))
 
     @staticmethod
-    def replace_colors(color_tag):
+    def replace_colors(color_tag: str) -> str:
         """ Replace the Kodi color tags with actual tags.
 
-        :param str color_tag: The text that contains color tags
+        :param color_tag: The text that contains color tags
 
-        :rtype: str
         :return: The text with actual ASCII color codes
 
         """
 
         def __color_replacer(color_input):
             color_name = color_input.group(1)
             if color_name == "gold":
@@ -155,18 +157,18 @@
             else:
                 return Colors.EndColor
 
         color_tag = re.sub(r'\[COLOR (\w+)]', __color_replacer, color_tag)
         color_tag = color_tag.replace("[/COLOR]", Colors.EndColor)
         return color_tag
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.__class__.__name__
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str):
         """ Logs any missing methods calls
 
         :param str name:    The name of the attribute
         :return: object
 
         """
```

### Comparing `sakee-0.1.6/sakee.egg-info/PKG-INFO` & `sakee-0.1.7/sakee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sakee
-Version: 0.1.6
+Version: 0.1.7
 Summary: SAKÉ can help you to debug and develop Kodi Python add-ons
 Home-page: https://github.com/retrospect-addon/kodi.emulator.ascii
 Author: Bas Rieter
 License: GPL-3.0
 Project-URL: Documentation, https://github.com/retrospect-addon/kodi.emulator.ascii/blob/master/README.md
 Project-URL: Source, https://github.com/retrospect-addon/kodi.emulator.ascii/
 Project-URL: Tracker, https://github.com/retrospect-addon/kodi.emulator.ascii/issues
```

### Comparing `sakee-0.1.6/setup.py` & `sakee-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup
 
 project_dir = os.path.dirname(os.path.abspath(__file__))
 
 
 setup(
     name='sakee',
-    version="0.1.6",
+    version="0.1.7",
     url='https://github.com/retrospect-addon/kodi.emulator.ascii',
     author='Bas Rieter',
     description='SAKÉ can help you to debug and develop Kodi Python add-ons',
     long_description=io.open(os.path.join(project_dir, 'README.md'), encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     keywords='Kodi, emulator, ascii, xbmc, xbmcgui, xbmcplugin, xbmcaddon',
     license='GPL-3.0',
```

### Comparing `sakee-0.1.6/xbmc.py` & `sakee-0.1.7/xbmc.py`

 * *Files identical despite different names*

### Comparing `sakee-0.1.6/xbmcaddon.py` & `sakee-0.1.7/xbmcaddon.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-License-Identifier: GPL-3.0
-
 import os
 import io
 import re
+from typing import Optional
 
 from sakee import addoninfo
 from sakee.stub import KodiStub
 
 
 # noinspection PyPep8Naming,PyShadowingBuiltins
 class Addon(KodiStub):
@@ -32,136 +32,226 @@
         self.__news = None
         self.__disclaimer = None
         self.__description = None
         self.__load_add_on_xml()
         self.__localization = self.__get_strings()
         self.__settings = self.__get_settings()
 
-    def getSetting(self, id):  # NOSONAR
+    def getSetting(self, id: str) -> Optional[str]:
         """ Returns the value of a setting as a unicode string.
 
-        :param str id:  Id of the setting that the module needs to access.
+        :param id: ID of the setting that the module needs to access.
 
-        :return: The value of a setting as a unicode string.
-        :rtype: str
+        :return: The value of a setting as a unicode string. If the value was not set, None
+        is returned.
 
         """
+
         if id in self.__settings:
             return self.__settings[id]
         else:
-            return ''
+            return ""
 
-    def getSettingBool(self, id):
+    def getSettingBool(self, id: str) -> bool:
         """ Returns the value of a setting as a boolean.
 
-        :param str id:  Id of the setting that the module needs to access.
+        :param id: ID of the setting that the module needs to access.
 
         :return: The value of a setting as a boolean.
-        :rtype: bool
 
         """
+
+        return self.getBool(id)
+
+    def getBool(self, id: str) -> bool:
+        """ Returns the value of a setting as a boolean.
+
+        :param id: ID of the setting that the module needs to access.
+
+        :return: The value of a setting as a boolean.
+
+        """
+
         return self.getSetting(id).lower() == "true"
 
-    def getSettingInt(self, id):
+    def getSettingInt(self, id: str) -> int:
         """ Returns the value of a setting as an integer.
 
-        :param str id:  Id of the setting that the module needs to access.
+        :param str id: ID of the setting that the module needs to access.
 
         :return: The value of a setting as an integer.
         :rtype: int
 
         """
 
+        return self.getInt(id)
+
+    def getInt(self, id: str) -> int:
+        """ Returns the value of a setting as an integer.
+
+        :param id: ID of the setting that the module needs to access.
+
+        :return: The value of a setting as an integer.
+
+        """
+
         return int(self.getSetting(id) or 0)
 
-    def getSettingNumber(self, id):
+    def getSettingNumber(self, id: str) -> float:
         """ Returns the value of a setting as a floating point number.
 
-        :param str id:  Id of the setting that the module needs to access.
+        :param id: ID of the setting that the module needs to access.
+
+        :return: The value of a setting as a floating point number.
+
+        """
+
+        return self.getNumber(id)
+
+    def getNumber(self, id: str) -> float:
+        """ Returns the value of a setting as a floating point number.
+
+        :param id: ID of the setting that the module needs to access.
 
         :return: The value of a setting as a floating point number.
-        :rtype: float
 
         """
 
         return float(self.getSetting(id) or 0.0)
 
-    def getSettingString(self, id):
+    def getSettingString(self, id: str) -> str:
+        """ Returns the value of a setting as a string.
+
+        :param id: ID of the setting that the module needs to access.
+
+        :return: The value of a setting as a string.
+
+        """
+
+        return self.getString(id)
+
+    def getString(self, id: str) -> str:
         """ Returns the value of a setting as a string.
 
-        :param str id:  Id of the setting that the module needs to access.
+        :param id: ID of the setting that the module needs to access.
 
         :return: The value of a setting as a string.
-        :rtype: float
 
         """
 
         return str(self.getSetting(id) or "")
 
-    def setSetting(self, id, value):  # NOSONAR
+    def setSetting(self, id: str, value: str) -> None:
         """ Sets a script setting.
 
-        :param str id:       Id of the setting that the module needs to access.
-        :param str value:    Value of the setting.
+        :param id:       ID of the setting that the module needs to access.
+        :param value:    Value of the setting.
 
         """
 
         self.__settings[id] = value
 
-    def setSettingBool(self, id, value):  # NOSONAR
+    def setSettingBool(self, id: str, value: bool) -> bool:
         """ Sets a script setting.
 
-        :param str id:       Id of the setting that the module needs to access.
-        :param bool value:    Value of the setting.
+        :param id:       ID of the setting that the module needs to access.
+        :param value:    Value of the setting.
+
+        :return: True if the value of the setting was set, false otherwise
+
+        """
+
+        self.setBool(id, value)
+        return True
+
+    def setBool(self, id: str, value: bool) -> None:
+        """ Sets a script setting.
+
+        :param id:       ID of the setting that the module needs to access.
+        :param value:    Value of the setting.
 
         """
 
         self.__settings[id] = "true" if value else "false"
+
+    def setSettingInt(self, id: str, value: int) -> bool:
+        """ Sets a script setting.
+
+        :param id:       ID of the setting that the module needs to access.
+        :param value:    Value of the setting.
+
+        :return: True if the value of the setting was set, false otherwise
+
+        """
+
+        self.setInt(id, value)
         return True
 
-    def setSettingInt(self, id, value):  # NOSONAR
+    def setInt(self, id: str, value: int) -> None:
         """ Sets a script setting.
 
-        :param str id:       Id of the setting that the module needs to access.
-        :param int value:    Value of the setting.
+        :param id:       ID of the setting that the module needs to access.
+        :param value:    Value of the setting.
 
         """
 
         self.__settings[id] = str(value)
+
+    def setSettingNumber(self, id: str, value: float) -> bool:
+        """ Sets a script setting.
+
+        :param str id:       ID of the setting that the module needs to access.
+        :param float value:  Value of the setting.
+
+        :return: True if the value of the setting was set, false otherwise
+
+        """
+
+        self.setNumber(id, value)
         return True
 
-    def setSettingNumber(self, id, value):  # NOSONAR
+    def setNumber(self, id: str, value: float) -> None:
         """ Sets a script setting.
 
-        :param str id:       Id of the setting that the module needs to access.
+        :param str id:       ID of the setting that the module needs to access.
         :param float value:  Value of the setting.
 
         """
 
         self.__settings[id] = str(value)
+
+    def setSettingString(self, id: str, value: str) -> bool:  # NOSONAR
+        """ Sets a script setting.
+
+        :param id:     ID of the setting that the module needs to access.
+        :param value:  Value of the setting.
+
+        :return: True if the value of the setting was set, false otherwise
+
+        """
+
+        self.setString(id, value)
         return True
 
-    def setSettingString(self, id, value):  # NOSONAR
+    def setString(self, id: str, value: str) -> None:  # NOSONAR
         """ Sets a script setting.
 
-        :param str id:       Id of the setting that the module needs to access.
-        :param str value:  Value of the setting.
+        :param id:     ID of the setting that the module needs to access.
+        :param value:  Value of the setting.
 
         """
 
         self.__settings[id] = value
-        return True
 
-    def getAddonInfo(self, id):  # NOSONAR
+    def getAddonInfo(self, id: str) -> str:
         """ Returns the value of an addon property as a string.
 
-        :param str id:  Id of the property that the module needs to access.
+        :param id:  Id of the property that the module needs to access.
 
         :return: Returns the value of an addon property as a string.
-        :rtype: str
 
         Possible options are: author, changelog, description, disclaimer, fanart, icon, id,
                               name, path, profile, stars, summary, type, version
         """
         id = id.lower()
         # missing: starts - type
 
@@ -170,45 +260,45 @@
         elif id == "changelog":
             return self.__news
         elif id == "description":
             return self.__description
         elif id == "disclaimer":
             return self.__disclaimer
         elif id == "fanart":
-            return self.__fanart
+            return str(self.__fanart)
         elif id == "icon":
             return self.__icon
         elif id == "id":
             return self.__add_on_id
         elif id == "name":
             return self.__name
         elif id == "path":
             return self.__add_on_path
         elif id == "profile":
-            return self.__add_on_profile_path
+            return str(self.__add_on_profile_path)
         elif id == "summary":
             return self.__summary
         elif id == "version":
             return self.__version
 
         raise ValueError("Cannot find info '%s'" % (id,))
 
-    def getLocalizedString(self, id):  # NOSONAR
+    def getLocalizedString(self, id: int) -> str:
         """ Returns an addon's localized 'unicode string'.
 
         :param int id:      Id# for string you want to localize.
 
         :return: Localized 'unicode string'
         :rtype: str
 
         """
 
         return self.__localization.get(id, "Translated {}".format(id))
 
-    def openSettings(self):  # NOSONAR
+    def openSettings(self) -> None:
         self.print_heading("Add-on settings")
         for setting, value in self.__settings.items():
             self.print_line("{}:{}".format(setting, value), verbose=True)
 
     def __repr__(self):
         return repr(self.__settings)
```

### Comparing `sakee-0.1.6/xbmcgui.py` & `sakee-0.1.7/xbmcgui.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # SPDX-License-Identifier: GPL-3.0
+from typing import List, Optional, Union
+
 
 from sakee.colors import Colors
 from sakee.stub import KodiStub
 
 NOTIFICATION_INFO = "info"
 NOTIFICATION_WARNING = "warning"
 NOTIFICATION_ERROR = "error"
@@ -14,29 +16,253 @@
 INPUT_IPADDRESS = 4
 INPUT_PASSWORD = 5
 
 PASSWORD_VERIFY = 1
 ALPHANUM_HIDE_INPUT = 2
 
 
+# noinspection PyPep8Naming
+class ListItem(KodiStub):
+
+    # noinspection PyUnusedLocal
+    def __init__(self, label="", label2="", path="", offscreen=False):
+        """ ListItem class. Creates a new ListItem.
+
+        label          : [opt] string or unicode -
+        label2         : [opt] string or unicode - label2 text.
+        iconImage      : [opt] string - icon filename.
+        thumbnailImage : [opt] string - thumbnail filename.
+        path           : [opt] string or unicode -
+
+        :param str label:           Label1 text.
+        :param str label2:          Label2 text.
+        :param str path:            Listitem's path.
+        :param bool offscreen:      Is an offscreen item?
+
+        *Note, You can use the above as keywords for arguments and skip certain optional arguments.
+           Once you use a keyword, all following arguments require the keyword.
+
+        """
+
+        super(ListItem, self).__init__()
+
+        self.__info = dict()
+        self.__art = dict()
+        self.__type = None
+
+        self.__label = label
+        self.__info["*label1"] = label
+        self.__label2 = label2
+        self.__info["*label2"] = label2
+
+        self.__path = path
+        self.__subtitles = []
+
+        # store properties
+        self.__properties = {"path": path}
+
+    def setIconImage(self, icon):  # NOSONAR
+        raise DeprecationWarning("No more setIconImage: http://kodi.wiki/view/Jarvis_API_changes")
+
+    def setThumbnailImage(self, thumbnail):  # NOSONAR
+        raise DeprecationWarning("No more setThumbnailImage: http://kodi.wiki/view/Jarvis_API_changes")
+
+    # noinspection PyShadowingBuiltins
+    def setInfo(self, type, infoLabels):  # NOSONAR
+        """ Sets the listitem's infoLabels.
+
+        :param str type:                    Type of
+        :param dict[str,str] infoLabels:    Pairs of { label: value }
+
+        ============  ======================================
+        Command name  Description
+        ============  ======================================
+        video         Video information
+        music         Music information
+        pictures      Pictures informanion
+        game          Game information
+        ============  ======================================
+
+        See http://kodi.wiki/view/InfoLabels
+
+        """
+
+        self.__type = type
+        self.__info.update(infoLabels)
+        self.print_line("Updating infolabels with {}".format(infoLabels), verbose=True)
+
+    def setContentLookup(self, enable):
+        """ Enable or disable content lookup for item.
+
+        :param bool enable: bool to enable content lookup
+
+        If disabled, HEAD requests to e.g determine mime type will not be sent.
+
+        """
+        pass
+
+    def setArt(self, values):  # NOSONAR
+        """ Sets the listitem's art
+
+        :param dict[str,str] values:    Pairs of { label: value }.
+
+        ==========  ======================================
+        Label       Type
+        ==========  ======================================
+        thumb       image filename
+        poster      image filename
+        banner      image filename
+        fanart      image filename
+        clearart    image filename
+        clearlogo   image filename
+        landscape   image filename
+        icon        image filename
+        ==========  ======================================
+
+        """
+
+        self.__art.update(values)
+        self.print_line("Updating artwork with {}".format(values), verbose=True)
+
+    def setLabel(self, label):  # NOSONAR
+        """ Sets the listitem's label.
+
+        :param str label:   text string.
+
+        """
+
+        self.__label = label
+        self.__art["label1"] = label
+        self.print_line("Setting label1='{}'".format(label), verbose=True)
+
+    def getLabel(self):
+        """ Returns the listitem label.
+
+        :return: label2
+        :rtype: str
+
+        """
+
+        return self.__label
+
+    def setLabel2(self, label):  # NOSONAR
+        """ Sets the listitem's label.
+
+        :param str label:   text string.
+
+        """
+
+        self.__label2 = label
+        self.__art["label2"] = label
+        self.print_line("Setting label2='{}'".format(label), verbose=True)
+
+    def getLabel2(self):
+        """ Returns the listitem label.
+
+        :return: label2
+        :rtype: str
+
+        """
+
+        return self.__label2
+
+    def setSubtitles(self, subtitleFiles):  # NOSONAR
+        """ Sets subtitles for this listitem.
+
+        :param list[str] subtitleFiles: list with path to subtitle files
+
+        """
+
+        self.__subtitles = subtitleFiles
+        for sub in subtitleFiles:
+            self.print_line("Adding subtitles: {}".format(sub), verbose=True)
+
+    def setProperty(self, key, value):  # NOSONAR
+        """ Sets a listitem property, similar to an infolabel.
+
+        :param str key:         Property name.
+        :param str value:       Value of property.
+
+        NOTE: Key is NOT case sensitive.
+
+        """
+
+        self.__properties[key.lower()] = value
+        self.print_line("Adding property: {}: {}".format(key, value), verbose=True)
+
+    def getProperty(self, key):  # NOSONAR
+        """ Returns a listitem property as a string, similar to an infolabel.
+
+        :param str key: property name.
+
+        :return:
+
+        NOTE: Key is NOT case sensitive.
+
+        """
+
+        return self.__properties.get(key.lower(), None)
+
+    def getPath(self):  # NOSONAR
+        """ Returns the path of this listitem.
+
+        :return: The path of this listitem.
+        :rtype: str
+        """
+
+        return self.__path or self.getProperty("path") or ""
+
+    def setPath(self, path):  # NOSONAR
+        """ Sets the listitem's path.
+
+        :param str path:    Activated when item is clicked.
+
+        """
+
+        self.__path = path
+        self.setProperty("path", path)
+
+    def __str__(self):
+        if KodiStub.is_verbose:
+            value = "%s [%s]\n" % (self.__label, self.__type or "")
+            value = "%sInfoLabels\n" % (value,)
+            keys = sorted(self.__info.keys())
+            for key in keys:
+                value = "%s    - %s: %s\n" % (value, key, self.__info[key])
+            value = "%sProperties\n" % (value,)
+            keys = sorted(self.__properties.keys())
+            for key in keys:
+                value = "%s    - %s: %s\n" % (value, key, self.__properties[key])
+
+            return value
+        else:
+            return self.__label
+
+    def __unicode__(self):
+        return self.__str__()
+
+    def __repr__(self):
+        return self.__str__()
+
+
+# noinspection PyPep8Naming,PyShadowingBuiltins
 class Dialog(KodiStub):
     def __init__(self):
         super(Dialog, self).__init__()
 
-    def ok(self, heading, message):  # NOSONAR
+    def ok(self, heading: str, message: str) -> bool:
         """ OK dialog
 
         The functions permit the call of a dialog of information, a confirmation
         of the user by press from OK required.
 
-        :param str heading:      dialog heading.
-        :param str message:      dialog message.
+        :param heading:      dialog heading.
+        :param message:      dialog message.
 
         :return: Returns True if 'Ok' was pressed, else False.
-        :rtype: bool
 
         Example::
 
             dialog = xbmcgui.Dialog()
             ok = dialog.ok('Kodi', 'There was an error.')
 
         """
@@ -46,47 +272,51 @@
         if KodiStub.is_interactive:
             self.read_input("{}. OK?".format(message), color=Colors.Yellow)
         else:
             KodiStub.print_line("{}. OK?".format(message), Colors.Yellow)
         return True
 
     # noinspection PyUnusedLocal
-    def textviewer(self, heading, text, usemono=False):
-        """ The text viewer dialog can be used to display descriptions, help texts or other larger texts.
-
-        :param str heading:     Dialog heading.
-        :param str text:        Dialog text.
-        :param bool usemono:    Use a monospace font.
+    def textviewer(self, heading: str, text: str, usemono: bool = False) -> None:
+        """ The text viewer dialog can be used to display descriptions,
+        help texts or other larger texts.
+
+        :param heading:     Dialog heading.
+        :param text:        Dialog text.
+        :param usemono:     Use a monospace font.
 
         """
 
         text = self.replace_colors(text)
         text = text.replace("\\n", "\n")
         self.print_heading(heading)
         self.print_line(text)
         self.print_line("=" * 120, color=Colors.Yellow)
 
         if KodiStub.is_interactive:
             self.read_input("OK?", color=Colors.Yellow)
         else:
             KodiStub.print_line("OK?", Colors.Yellow)
-        return True
+        return
 
     # noinspection PyPep8Naming,PyUnusedLocal
-    def multiselect(self, heading, options, autoclose=0, preselect=None, useDetails=False):  # NOSONAR
+    def multiselect(self, heading: str,
+                    options: Union[List[str], List[ListItem]],
+                    autoclose: int = 0,
+                    preselect: Optional[List[int]] = None,
+                    useDetails: bool = False) -> Optional[List[int]]:
         """ Show a multi-select dialog.
 
-        :param str heading:                     Dialog heading.
-        :param list[string|ListItem] options:   Options to choose from.
-        :param int autoclose:                   Milliseconds to autoclose dialog. (default=do not autoclose)
-        :param list[int]|None preselect:        Indexes of items to preselect in list (default: do not preselect any item)
-        :param bool useDetails:                 Use detailed list instead of a compact list. (default=false)
+        :param heading:          Dialog heading.
+        :param options:          Options to choose from.
+        :param autoclose:        Milliseconds to autoclose dialog. (default=do not autoclose)
+        :param preselect:        Indexes of items to preselect in list (default: do not preselect any item)
+        :param useDetails:       Use detailed list instead of a compact list. (default=false)
 
         :return: Returns the selected items as a list of indices, or None if cancelled.
-        :rtype: list[int]
 
         """
 
         self.print_heading(heading)
 
         selections = []
         for i in range(0, len(options)):
@@ -96,25 +326,27 @@
         selections = self.read_input("What items to select (%s)? " % (",".join(selections)),
                                      color=Colors.Yellow).lower()
         if not selections:
             return None
         return list(map(lambda index_value: int(index_value), selections.split(",")))
 
     # noinspection PyPep8Naming,PyUnusedLocal
-    def select(self, heading, options, autoclose=0, preselect=None, useDetails=False):  # NOSONAR
+    def select(self, heading: str,
+               options: Union[List[str], List[ListItem]],
+               autoclose: int = 0, preselect: int = -1,
+               useDetails: bool = False) -> Optional[int]:
         """ Show a select dialog.
 
-        :param str heading:                     Dialog heading.
-        :param list[string|ListItem] options:   Options to choose from.
-        :param int autoclose:                   Milliseconds to autoclose dialog. (default=do not autoclose)
-        :param int|None preselect:              Indexes of items to preselect in list (default: do not preselect any item)
-        :param bool useDetails:                 Use detailed list instead of a compact list. (default=false)
+        :param heading:         Dialog heading.
+        :param options:         Options to choose from.
+        :param autoclose:       Milliseconds to autoclose dialog. (default=do not autoclose)
+        :param preselect:       Indexes of items to preselect in list (default: do not preselect any item)
+        :param useDetails:      Use detailed list instead of a compact list. (default=false)
 
         :return: Returns the selected items as a list of indices, or None if cancelled.
-        :rtype: int
 
         """
         self.print_heading(heading)
 
         selections = []
         for i in range(0, len(options)):
             self.print_line("{} ) {}".format(i, options[i]))
@@ -122,26 +354,26 @@
         self.print_line("=" * 120, color=Colors.Yellow)
         selections = self.read_input("What item to select (%s)? " % (",".join(selections)), color=Colors.Yellow).lower()
         if not selections:
             return None
         return list(map(lambda index_value: int(index_value), selections.split(",")))[0]
 
     # noinspection PyUnusedLocal
-    def yesno(self, heading, message, nolabel='', yeslabel='', customlabel=None, autoclose=0):
+    def yesno(self, heading: str, message: str, nolabel: str = "", yeslabel: str = "",
+              customlabel: Optional[str] = None, autoclose: int = 0) -> bool:
         """ The Yes / No dialog can be used to inform the user about questions and get the answer.
 
-        :param str heading:             Dialog heading.
-        :param str message:             Message to display.
-        :param str nolabel:             Label to put on the no button.
-        :param str yeslabel:            Label to put on the yes button.
-        :param str|None customlabel:    Label to put on the custom button.
-        :param autoclose:               Milliseconds to autoclose dialog. (default=do not autoclose)
+        :param heading:             Dialog heading.
+        :param message:             Message to display.
+        :param nolabel:             Label to put on the no button.
+        :param yeslabel:            Label to put on the yes button.
+        :param customlabel:         Label to put on the custom button.
+        :param autoclose:           Milliseconds to autoclose dialog. (default=do not autoclose)
 
         :return: Returns True if 'Yes' was pressed, else False.
-        :rtype: bool
 
         """
 
         if not nolabel:
             nolabel = "No"
 
         if not yeslabel:
@@ -153,22 +385,23 @@
             answer = self.read_input(question, Colors.Yellow)
             return yeslabel.lower().startswith(answer.lower())
         else:
             KodiStub.print_line(question, Colors.Yellow)
             return True
 
     # noinspection PyUnusedLocal
-    def notification(self, heading, message, icon=NOTIFICATION_INFO, time=5000, sound=True):
+    def notification(self, heading: str, message: str, icon: str = NOTIFICATION_INFO,
+                     time: int = 5000, sound: bool = True) -> False:
         """ Show a Notification alert.
 
-        :param str heading:             Dialog heading.
-        :param str message:             Message to display.
-        :param str icon:                Icon to use. (default=xbmcgui.NOTIFICATION_INFO)
-        :param int time:                Time in milliseconds.
-        :param str sound:               Play notification sound. (default=True)
+        :param heading:             Dialog heading.
+        :param message:             Message to display.
+        :param icon:                Icon to use. (default=xbmcgui.NOTIFICATION_INFO)
+        :param time:                Time in milliseconds.
+        :param sound:               Play notification sound. (default=True)
 
         ============================  ============
         Icon                          Description
         ============================  ============
         xbmcgui.NOTIFICATION_INFO     Info icon
         xbmcgui.NOTIFICATION_WARNING  Warning icon
         xbmcgui.NOTIFICATION_ERROR    Error icon
@@ -183,22 +416,23 @@
             color = Colors.White
 
         self.print_heading(heading, align_right=True, color=color)
         self.print_line(message, color=color)
         self.print_line("=" * 120, color)
 
     # noinspection PyUnusedLocal
-    def input(self, heading, defaultt='', type=INPUT_ALPHANUM, option=0, autoclose=0):
+    def input(self, heading: str, defaultt: str = "", type: int = INPUT_ALPHANUM,
+              option: int = 0, autoclose: int = 0):
         """ Show an input dialog.
 
-        :param str heading:             Dialog heading.
-        :param str defaultt:            Default value
-        :param int type:                The type of keyboard dialog.
-        :param str option:              Option for the dialog.
-        :param int autoclose:           Milliseconds to autoclose dialog. (default=do not autoclose)
+        :param heading:             Dialog heading.
+        :param defaultt:            Default value
+        :param type:                The type of keyboard dialog.
+        :param option:              Option for the dialog.
+        :param autoclose:           Milliseconds to autoclose dialog. (default=do not autoclose)
 
         ========================  =========================================
         Type                      Description
         ========================  =========================================
         xbmcgui.INPUT_ALPHANUM    Standard keyboard
         xbmcgui.INPUT_NUMERIC     Format: #
         xbmcgui.INPUT_DATE        Format: DD/MM/YYYY
@@ -222,68 +456,70 @@
             keyboard = self.get_keyboard_stub()
             value = keyboard.get_next_input()
             return value if value is not None else defaultt
 
         KodiStub.print_heading(heading)
         try:
             answer = self.read_input("Please provide keyboard input [{}]?".format(defaultt), color=Colors.Yellow)
-            return answer if answer != '' else defaultt
+            return answer if answer != "" else defaultt
         except EOFError:
-            return ''
+            return ""
 
     # noinspection PyUnusedLocal
-    def numeric(self, type, heading, defaultt=None, bHiddenInput=None):
+    def numeric(self, type: int, heading: str, defaultt: str = "", bHiddenInput: bool = False):
         """ Show an numeric input dialog.
 
-        :param int type:                The type of numeric dialog.
-        :param str heading:             Dialog heading (will be ignored for type 4).
-        :param str defaultt:            Default value.
-        :param bool bHiddenInput:       Mask input (available for type 0).
+        :param type:                The type of numeric dialog.
+        :param heading:             Dialog heading (will be ignored for type 4).
+        :param defaultt:            Default value.
+        :param bHiddenInput:        Mask input (available for type 0).
 
         =====  ========================  ========================================================
         Param  Type                      Description
         =====  ========================  ========================================================
         0      ShowAndGetNumber          Default format: #
         1      ShowAndGetDate            Default format: DD/MM/YYYY
         2      ShowAndGetTime            Default format: HH:MM
         3      ShowAndGetIPAddress       Default format: #.#.#.#
         4      ShowAndVerifyNewPassword  Default format: *
         =====  ========================  ========================================================
 
         :return: Returns the entered data as a string. Returns the default value if dialog was canceled.
-        :rtype: str
 
         """
+
         if not self.is_interactive:
             keyboard = self.get_keyboard_stub()
             value = keyboard.get_next_input()
             return value if value is not None else defaultt
 
         KodiStub.print_heading(heading)
         try:
             answer = self.read_input("Please provide keyboard input [{}]?".format(defaultt), color=Colors.Yellow)
-            return answer if answer != '' else defaultt
+            return answer if answer != "" else defaultt
         except EOFError:
-            return ''
+            return ""
 
     # noinspection PyUnusedLocal
-    def browse(self, type, heading, shares, mask='', useThumbs=False, treatAsFolder=False, defaultt='', enableMultiple=False):
+    def browse(self, type: int, heading: str, shares: str, mask: str = "", useThumbs: bool = False,
+               treatAsFolder: bool = False, defaultt: str = "",
+               enableMultiple: bool = False) -> Union[str, List[str]]:
         """ Browser dialog.
 
         The function offer the possibility to select a file by the user of the add-on.
         It allows all the options that are possible in Kodi itself and offers all support file types.
 
-        :param int type:                The type of browse dialog.
-        :param str heading:             Dialog heading.
-        :param str shares:              From sources.xml
-        :param str mask:                '|' separated file mask. (i.e. '.jpg|.png')
-        :param bool useThumbs:          Auto switch to Thumb view if files exist.
-        :param bool treatAsFolder:      Playlists and archives act as folders.
-        :param str defaultt:            Default path or file.
-        :param bool enableMultiple:     Multiple file selection is enabled.
+        :param type:                The type of browse dialog.
+        :param heading:             Dialog heading.
+        :param shares:              From sources.xml
+        :param mask:                '|' separated file mask. (i.e. '.jpg|.png')
+        :param useThumbs:           Auto switch to Thumb view if files exist.
+        :param treatAsFolder:       Playlists and archives act as folders.
+        :param defaultt:            Default path or file.
+        :param enableMultiple:      Multiple file selection is enabled.
 
         ========================  =========================================
         Type                      Description
         ========================  =========================================
         0                         ShowAndGetDirectory
         1                         ShowAndGetFile
         2                         ShowAndGetImage
@@ -305,36 +541,37 @@
 
         :return: If enableMultiple is False (default): returns filename and/or path as a string to the location of the highlighted item, if user pressed 'Ok' or
                  a masked item was selected. Returns the default value if dialog was canceled.
                  If enableMultiple is True: returns tuple of marked filenames as a string if user pressed 'Ok' or a masked item was selected. Returns empty
                  tuple if dialog was canceled.
                  If type is 0 or 3 the enableMultiple parameter is ignored.
 
-        :rtype: str|tuple[str]
-
         """
+
         if enableMultiple:
             return self.browseMultiple(type, heading, shares, mask, useThumbs, treatAsFolder, defaultt)
         else:
             return self.browseSingle(type, heading, shares, mask, useThumbs, treatAsFolder, defaultt)
 
     # noinspection PyUnusedLocal
-    def browseMultiple(self, type, heading, shares, mask='', useThumbs=False, treatAsFolder=False, defaultt=''):
+    def browseMultiple(self, type: int, heading: str, shares: str, mask: str = "",
+                       useThumbs: bool = False, treatAsFolder: bool = False,
+                       defaultt: str = "") -> List[str]:
         """ Browser dialog.
 
         The function offer the possibility to select a file by the user of the add-on.
         It allows all the options that are possible in Kodi itself and offers all support file types.
 
-        :param int type:                The type of browse dialog.
-        :param str heading:             Dialog heading.
-        :param str shares:              From sources.xml
-        :param str mask:                '|' separated file mask. (i.e. '.jpg|.png')
-        :param bool useThumbs:          Auto switch to Thumb view if files exist.
-        :param bool treatAsFolder:      Playlists and archives act as folders.
-        :param str defaultt:            Default path or file.
+        :param type:                The type of browse dialog.
+        :param heading:             Dialog heading.
+        :param shares:              From sources.xml
+        :param mask:                '|' separated file mask. (i.e. '.jpg|.png')
+        :param useThumbs:           Auto switch to Thumb view if files exist.
+        :param treatAsFolder:       Playlists and archives act as folders.
+        :param defaultt:            Default path or file.
 
         ========================  =========================================
         Type                      Description
         ========================  =========================================
         0                         ShowAndGetDirectory
         1                         ShowAndGetFile
         2                         ShowAndGetImage
@@ -353,43 +590,44 @@
         "local"                      list local drives
         ""                           list local drives and network shares
         ===========================  ============================================================================
 
         :return: Returns tuple of marked filenames as a string if user pressed 'Ok' or a masked item was selected.
                  Returns empty tuple if dialog was canceled.
 
-        :rtype: tuple[str]
-
         """
+
         if not self.is_interactive:
             keyboard = self.get_keyboard_stub()
             value = keyboard.get_next_input()
-            return (value,) if value is not None else (defaultt,)
+            return [value] if value is not None else [defaultt]
 
         KodiStub.print_heading(heading)
         try:
             answer = self.read_input("Please enter the path to a file [{}]?".format(defaultt), color=Colors.Yellow)
-            return (answer,) if answer != '' else (defaultt,)
+            return [answer] if answer != "" else [defaultt]
         except EOFError:
-            return ()
+            return []
 
     # noinspection PyUnusedLocal
-    def browseSingle(self, type, heading, shares, mask='', useThumbs=False, treatAsFolder=False, defaultt=''):
+    def browseSingle(self, type: int, heading: str, shares: str, mask: str = "",
+                     useThumbs: bool = False, treatAsFolder: bool = False,
+                     defaultt: str = "") -> str:
         """ Browser dialog.
 
         The function offer the possibility to select a file by the user of the add-on.
         It allows all the options that are possible in Kodi itself and offers all support file types.
 
-        :param int type:                The type of browse dialog.
-        :param str heading:             Dialog heading.
-        :param str shares:              From sources.xml
-        :param str mask:                '|' separated file mask. (i.e. '.jpg|.png')
-        :param bool useThumbs:          Auto switch to Thumb view if files exist.
-        :param bool treatAsFolder:      Playlists and archives act as folders.
-        :param str defaultt:            Default path or file.
+        :param type:                The type of browse dialog.
+        :param heading:             Dialog heading.
+        :param shares:              From sources.xml
+        :param mask:                '|' separated file mask. (i.e. '.jpg|.png')
+        :param useThumbs:           Auto switch to Thumb view if files exist.
+        :param treatAsFolder:       Playlists and archives act as folders.
+        :param defaultt:            Default path or file.
 
         ========================  =========================================
         Type                      Description
         ========================  =========================================
         0                         ShowAndGetDirectory
         1                         ShowAndGetFile
         2                         ShowAndGetImage
@@ -408,344 +646,119 @@
         "local"                      list local drives
         ""                           list local drives and network shares
         ===========================  ============================================================================
 
         :return: Returns filename and/or path as a string to the location of the highlighted item, if user pressed 'Ok' or a masked item was selected.
                  Returns the default value if dialog was canceled.
 
-        :rtype: str
-
         """
+
         if not self.is_interactive:
             keyboard = self.get_keyboard_stub()
             value = keyboard.get_next_input()
             return value if value is not None else defaultt
 
         KodiStub.print_heading(heading)
         try:
             answer = self.read_input("Please enter the path to a file [{}]?".format(defaultt), color=Colors.Yellow)
-            return answer if answer != '' else defaultt
+            return answer if answer != "" else defaultt
         except EOFError:
-            return ''
-
-
-# noinspection PyPep8Naming
-class ListItem(KodiStub):
-
-    # noinspection PyUnusedLocal
-    def __init__(self, label="", label2="", path="", offscreen=False):
-        """ ListItem class. Creates a new ListItem.
-
-        label          : [opt] string or unicode -
-        label2         : [opt] string or unicode - label2 text.
-        iconImage      : [opt] string - icon filename.
-        thumbnailImage : [opt] string - thumbnail filename.
-        path           : [opt] string or unicode -
-
-        :param str label:           Label1 text.
-        :param str label2:          Label2 text.
-        :param str path:            Listitem's path.
-        :param bool offscreen:      Is an offscreen item?
-
-        *Note, You can use the above as keywords for arguments and skip certain optional arguments.
-           Once you use a keyword, all following arguments require the keyword.
-
-        """
-
-        super(ListItem, self).__init__()
-
-        self.__info = dict()
-        self.__art = dict()
-        self.__type = None
-
-        self.__label = label
-        self.__info["*label1"] = label
-        self.__label2 = label2
-        self.__info["*label2"] = label2
-
-        self.__path = path
-        self.__subtitles = []
-
-        # store properties
-        self.__properties = {"path": path}
-
-    def setIconImage(self, icon):  # NOSONAR
-        raise DeprecationWarning("No more setIconImage: http://kodi.wiki/view/Jarvis_API_changes")
-
-    def setThumbnailImage(self, thumbnail):  # NOSONAR
-        raise DeprecationWarning("No more setThumbnailImage: http://kodi.wiki/view/Jarvis_API_changes")
-
-    # noinspection PyShadowingBuiltins
-    def setInfo(self, type, infoLabels):  # NOSONAR
-        """ Sets the listitem's infoLabels.
-
-        :param str type:                    Type of
-        :param dict[str,str] infoLabels:    Pairs of { label: value }
-
-        ============  ======================================
-        Command name  Description
-        ============  ======================================
-        video         Video information
-        music         Music information
-        pictures      Pictures informanion
-        game          Game information
-        ============  ======================================
-
-        See http://kodi.wiki/view/InfoLabels
-
-        """
-
-        self.__type = type
-        self.__info.update(infoLabels)
-        self.print_line("Updating infolabels with {}".format(infoLabels), verbose=True)
-
-    def setContentLookup(self, enable):
-        """ Enable or disable content lookup for item.
-
-        :param bool enable: bool to enable content lookup
-
-        If disabled, HEAD requests to e.g determine mime type will not be sent.
-
-        """
-        pass
-
-    def setArt(self, values):  # NOSONAR
-        """ Sets the listitem's art
-
-        :param dict[str,str] values:    Pairs of { label: value }.
-
-        ==========  ======================================
-        Label       Type
-        ==========  ======================================
-        thumb       image filename
-        poster      image filename
-        banner      image filename
-        fanart      image filename
-        clearart    image filename
-        clearlogo   image filename
-        landscape   image filename
-        icon        image filename
-        ==========  ======================================
-
-        """
-
-        self.__art.update(values)
-        self.print_line("Updating artwork with {}".format(values), verbose=True)
-
-    def setLabel(self, label):  # NOSONAR
-        """ Sets the listitem's label.
-
-        :param str label:   text string.
-
-        """
-
-        self.__label = label
-        self.__art["label1"] = label
-        self.print_line("Setting label1='{}'".format(label), verbose=True)
-
-    def getLabel(self):
-        """ Returns the listitem label.
-
-        :return: label2
-        :rtype: str
-
-        """
-
-        return self.__label
-
-    def setLabel2(self, label):  # NOSONAR
-        """ Sets the listitem's label.
-
-        :param str label:   text string.
-
-        """
-
-        self.__label2 = label
-        self.__art["label2"] = label
-        self.print_line("Setting label2='{}'".format(label), verbose=True)
-
-    def getLabel2(self):
-        """ Returns the listitem label.
-
-        :return: label2
-        :rtype: str
-
-        """
-
-        return self.__label2
-
-    def setSubtitles(self, subtitleFiles):  # NOSONAR
-        """ Sets subtitles for this listitem.
-
-        :param list[str] subtitleFiles: list with path to subtitle files
-
-        """
-
-        self.__subtitles = subtitleFiles
-        for sub in subtitleFiles:
-            self.print_line("Adding subtitles: {}".format(sub), verbose=True)
-
-    def setProperty(self, key, value):  # NOSONAR
-        """ Sets a listitem property, similar to an infolabel.
-
-        :param str key:         Property name.
-        :param str value:       Value of property.
-
-        NOTE: Key is NOT case sensitive.
-
-        """
-
-        self.__properties[key.lower()] = value
-        self.print_line("Adding property: {}: {}".format(key, value), verbose=True)
-
-    def getProperty(self, key):  # NOSONAR
-        """ Returns a listitem property as a string, similar to an infolabel.
-
-        :param str key: property name.
-
-        :return:
-
-        NOTE: Key is NOT case sensitive.
-
-        """
-
-        return self.__properties.get(key.lower(), None)
-
-    def getPath(self):  # NOSONAR
-        """ Returns the path of this listitem.
-
-        :return: The path of this listitem.
-        :rtype: str
-        """
-
-        return self.__path or self.getProperty("path") or ""
-
-    def setPath(self, path):  # NOSONAR
-        """ Sets the listitem's path.
-
-        :param str path:    Activated when item is clicked.
-
-        """
-
-        self.__path = path
-        self.setProperty("path", path)
-
-    def __str__(self):
-        if KodiStub.is_verbose:
-            value = "%s [%s]\n" % (self.__label, self.__type or "")
-            value = "%sInfoLabels\n" % (value,)
-            keys = sorted(self.__info.keys())
-            for key in keys:
-                value = "%s    - %s: %s\n" % (value, key, self.__info[key])
-            value = "%sProperties\n" % (value,)
-            keys = sorted(self.__properties.keys())
-            for key in keys:
-                value = "%s    - %s: %s\n" % (value, key, self.__properties[key])
-
-            return value
-        else:
-            return self.__label
-
-    def __unicode__(self):
-        return self.__str__()
-
-    def __repr__(self):
-        return self.__str__()
+            return ""
 
 
 class DialogProgress(KodiStub):
     def __init__(self):
         """ Kodi's progress dialog class (Duh!) """
 
         self.__message = None
 
         super(DialogProgress, self).__init__()
 
-    def create(self, heading, message=""):
+    def create(self, heading: str, message: str = "") -> None:
         """
         Create and show a progress dialog.
 
-        :param str heading:       dialog heading.
-        :param str|None message:  line #1 multi-line text.
+        :param heading:   dialog heading.
+        :param message:   line f text to show.
 
         It is preferred to only use line1 as it is actually a multi-line text.
         In this case line2 and line3 must be omitted.
 
         Use update() to update lines and progressbar.
 
         """
 
         self.__message = message
         self.print_heading(heading)
         self.print_line(message)
 
-    def update(self, percent, message=""):
+    def update(self, percent: int, message: str = "") -> None:
         """ Updates the progress dialog.
 
-        :param int percent:         Percent complete. (0:100)
-        :param str|None message:    Message to show.
+        :param percent:    Percent complete. (0:100)
+        :param message:    Message to show.
 
         """
 
         self.print_line(
             "{}{}%{}: {}".format(
                 Colors.Yellow, percent, Colors.EndColor, message or self.__message))
 
-    def close(self):
+    def close(self) -> None:
         """ Close the progress dialog. """
         self.print_line("=" * 120, color=Colors.Yellow)
 
-    def iscanceled(self):
+    def iscanceled(self) -> bool:
         """ Checks progress is canceled. """
         return False
 
 
 # noinspection PyArgumentList
 class DialogProgressBG(KodiStub):
     def __init__(self):
         self.__message = None
         super(DialogProgressBG, self).__init__()
 
-    def create(self, heading, message=""):
+    def create(self, heading: str, message: str = "") -> None:
         """
         Create and show a progress background dialog.
 
-        :param str heading:       dialog heading.
-        :param str|None message:  line #1 multi-line text.
+        :param heading:   dialog heading.
+        :param message:   line f text to show.
 
         It is preferred to only use line1 as it is actually a multi-line text.
         In this case line2 and line3 must be omitted.
 
         Use update() to update lines and progressbar.
 
         """
 
         self.__message = message
         self.print_heading(heading, align_right=True)
         self.print_line(message)
 
-    def update(self, percent, heading="", message=""):
+    def update(self, percent: int, heading: str = "", message: str = "") -> None:
         """ Updates the progress dialog.
 
-        :param int percent:         Percent complete. (0:100)
-        :param str|None heading:    Dialog heading.
-        :param str|None message:    Message to show.
+        :param percent:    Percent complete. (0:100)
+        :param heading:    Dialog heading.
+        :param message:    Message to show.
 
         """
 
         if heading:
             self.print_line(
                 "{}{}%: {}{} - {}".format(
                     Colors.Yellow, percent, heading, Colors.EndColor, message or self.__message))
         else:
             self.print_line(
                 "{}{}%{}: {}".format(
                     Colors.Yellow, percent, Colors.EndColor, message or self.__message))
 
-    def close(self):
+    def close(self) -> None:
         """ Close the progress dialog. """
         self.print_line("=" * 120, color=Colors.Yellow)
 
     # noinspection PyPep8Naming
-    def isFinished(self):
-        """ Checks progress is canceled. """
+    def isFinished(self) -> bool:
+        """ Checks progress is finished. """
         return False
```

### Comparing `sakee-0.1.6/xbmcplugin.py` & `sakee-0.1.7/xbmcplugin.py`

 * *Files identical despite different names*

### Comparing `sakee-0.1.6/xbmcvfs.py` & `sakee-0.1.7/xbmcvfs.py`

 * *Files identical despite different names*

