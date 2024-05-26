# Comparing `tmp/kbve-1.0.8.tar.gz` & `tmp/kbve-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbve-1.0.8.tar", max compression
+gzip compressed data, was "kbve-1.0.9.tar", max compression
```

## Comparing `kbve-1.0.8.tar` & `kbve-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0       35 2024-05-16 22:58:29.163511 kbve-1.0.8/README.md
--rw-r--r--   0        0        0      161 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/OAI_CONFIG_LIST.json
--rw-r--r--   0        0        0       12 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/__init__.py
--rw-r--r--   0        0        0        9 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/__init__.py
--rw-r--r--   0        0        0     4075 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/api_connector.py
--rw-r--r--   0        0        0      283 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/__init__.py
--rw-r--r--   0        0        0     1998 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/coindesk_client.py
--rw-r--r--   0        0        0     1985 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/novnc_client.py
--rw-r--r--   0        0        0     1166 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/poetry_db_client.py
--rw-r--r--   0        0        0      982 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/runelite_client.py
--rw-r--r--   0        0        0     1336 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/screen_client.py
--rw-r--r--   0        0        0     2967 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/websocket_echo_client.py
--rw-r--r--   0        0        0      234 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/__init__.py
--rw-r--r--   0        0        0     2315 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/broadcast_utils.py
--rw-r--r--   0        0        0     1088 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/cors_utils.py
--rw-r--r--   0        0        0     2350 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/image_utils.py
--rw-r--r--   0        0        0      823 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/kr_decorator.py
--rw-r--r--   0        0        0     3048 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/rss_utils.py
--rw-r--r--   0        0        0     1517 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/theme_core.py
--rw-r--r--   0        0        0      940 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/atlas_autogen.py
--rw-r--r--   0        0        0      616 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/bigman.py
--rw-r--r--   0        0        0        0 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/__init__.py
--rw-r--r--   0        0        0     1480 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/doom.py
--rw-r--r--   0        0        0     1167 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/enter_the_matrix.py
--rw-r--r--   0        0        0     4640 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/memetris.py
--rw-r--r--   0        0        0     2012 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/pacman.py
--rw-r--r--   0        0        0     1379 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/snake.py
--rw-r--r--   0        0        0     2215 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/tetris.py
--rw-r--r--   0        0        0      473 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/hello.py
--rw-r--r--   0        0        0       11 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/__init__.py
--rw-r--r--   0        0        0      523 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/coindesk.py
--rw-r--r--   0        0        0      190 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/poem.py
--rw-r--r--   0        0        0     1434 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/rsps.py
--rw-r--r--   0        0        0      335 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/rss.py
--rw-r--r--   0        0        0    15477 2024-05-16 22:58:29.923512 kbve-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     8809 1970-01-01 00:00:00.000000 kbve-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-05-21 01:48:18.906626 kbve-1.0.9/README.md
+-rw-r--r--   0        0        0      161 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/OAI_CONFIG_LIST.json
+-rw-r--r--   0        0        0       12 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/__init__.py
+-rw-r--r--   0        0        0        9 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/__init__.py
+-rw-r--r--   0        0        0     4075 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/api_connector.py
+-rw-r--r--   0        0        0      323 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/clients/__init__.py
+-rw-r--r--   0        0        0     5438 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/clients/chrome_client.py
+-rw-r--r--   0        0        0     1998 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/clients/coindesk_client.py
+-rw-r--r--   0        0        0     3117 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/clients/novnc_client.py
+-rw-r--r--   0        0        0     1166 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/clients/poetry_db_client.py
+-rw-r--r--   0        0        0     4174 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/clients/runelite_client.py
+-rw-r--r--   0        0        0     4372 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/clients/screen_client.py
+-rw-r--r--   0        0        0     2967 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/clients/websocket_echo_client.py
+-rw-r--r--   0        0        0      234 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/utils/__init__.py
+-rw-r--r--   0        0        0     2315 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/utils/broadcast_utils.py
+-rw-r--r--   0        0        0     1088 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/utils/cors_utils.py
+-rw-r--r--   0        0        0     2350 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/utils/image_utils.py
+-rw-r--r--   0        0        0      823 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/utils/kr_decorator.py
+-rw-r--r--   0        0        0     3048 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/utils/rss_utils.py
+-rw-r--r--   0        0        0     1517 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/api/utils/theme_core.py
+-rw-r--r--   0        0        0      940 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/atlas_autogen.py
+-rw-r--r--   0        0        0      616 2024-05-21 01:48:18.910626 kbve-1.0.9/kbve_atlas/bigman.py
+-rw-r--r--   0        0        0        0 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/games/__init__.py
+-rw-r--r--   0        0        0     1480 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/games/doom.py
+-rw-r--r--   0        0        0     1167 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/games/enter_the_matrix.py
+-rw-r--r--   0        0        0     4640 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/games/memetris.py
+-rw-r--r--   0        0        0     2012 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/games/pacman.py
+-rw-r--r--   0        0        0     1379 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/games/snake.py
+-rw-r--r--   0        0        0     2215 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/games/tetris.py
+-rw-r--r--   0        0        0      473 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/hello.py
+-rw-r--r--   0        0        0       11 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/models/__init__.py
+-rw-r--r--   0        0        0      523 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/models/coindesk.py
+-rw-r--r--   0        0        0      190 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/models/poem.py
+-rw-r--r--   0        0        0     1434 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/models/rsps.py
+-rw-r--r--   0        0        0      335 2024-05-21 01:48:18.914626 kbve-1.0.9/kbve_atlas/models/rss.py
+-rw-r--r--   0        0        0    21683 2024-05-21 01:48:19.770629 kbve-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    12480 1970-01-01 00:00:00.000000 kbve-1.0.9/PKG-INFO
```

### Comparing `kbve-1.0.8/kbve_atlas/api/api_connector.py` & `kbve-1.0.9/kbve_atlas/api/api_connector.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/api/clients/coindesk_client.py` & `kbve-1.0.9/kbve_atlas/api/clients/coindesk_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/api/clients/poetry_db_client.py` & `kbve-1.0.9/kbve_atlas/api/clients/poetry_db_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/api/clients/websocket_echo_client.py` & `kbve-1.0.9/kbve_atlas/api/clients/websocket_echo_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/api/utils/broadcast_utils.py` & `kbve-1.0.9/kbve_atlas/api/utils/broadcast_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/api/utils/cors_utils.py` & `kbve-1.0.9/kbve_atlas/api/utils/cors_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/api/utils/image_utils.py` & `kbve-1.0.9/kbve_atlas/api/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/api/utils/kr_decorator.py` & `kbve-1.0.9/kbve_atlas/api/utils/kr_decorator.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/api/utils/rss_utils.py` & `kbve-1.0.9/kbve_atlas/api/utils/rss_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/api/utils/theme_core.py` & `kbve-1.0.9/kbve_atlas/api/utils/theme_core.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/atlas_autogen.py` & `kbve-1.0.9/kbve_atlas/atlas_autogen.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/bigman.py` & `kbve-1.0.9/kbve_atlas/bigman.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/games/doom.py` & `kbve-1.0.9/kbve_atlas/games/doom.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/games/enter_the_matrix.py` & `kbve-1.0.9/kbve_atlas/games/enter_the_matrix.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/games/memetris.py` & `kbve-1.0.9/kbve_atlas/games/memetris.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/games/pacman.py` & `kbve-1.0.9/kbve_atlas/games/pacman.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/games/snake.py` & `kbve-1.0.9/kbve_atlas/games/snake.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/games/tetris.py` & `kbve-1.0.9/kbve_atlas/games/tetris.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/models/coindesk.py` & `kbve-1.0.9/kbve_atlas/models/coindesk.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/kbve_atlas/models/rsps.py` & `kbve-1.0.9/kbve_atlas/models/rsps.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.8/pyproject.toml` & `kbve-1.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -31,28 +31,28 @@
   stubPath = "typings"
   typingsPath = "typings"
   analyzeTypeshed = false
   autoSearchPaths = true
 
 [tool.poetry]
 name = "kbve"
-version = "1.0.8"
+version = "1.0.9"
 description = "ATLAS"
 authors = [ ]
 license = "Proprietary"
 readme = "README.md"
 
   [[tool.poetry.packages]]
   include = "kbve_atlas"
 
   [tool.poetry.dependencies]
   python = ">=3.10,<3.13"
 
     [tool.poetry.dependencies.aiohttp]
-    version = "3.9.4 "
+    version = "3.9.5 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.aiosignal]
     version = "1.3.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
@@ -83,43 +83,63 @@
     optional = false
 
     [tool.poetry.dependencies.beautifulsoup4]
     version = "4.12.3 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.behave]
+    version = "1.2.6 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.broadcaster]
     version = "0.2.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
     extras = [ "redis" ]
 
     [tool.poetry.dependencies.certifi]
     version = "2024.2.2 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.cffi]
     version = "1.16.0 "
-    markers = 'os_name == "nt" and implementation_name != "pypy" and python_version >= "3.10" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13" and (os_name == "nt" or platform_python_implementation != "PyPy") and (implementation_name != "pypy" or platform_python_implementation != "PyPy")'
+    optional = false
+
+    [tool.poetry.dependencies.chardet]
+    version = "5.2.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.charset-normalizer]
     version = "3.3.2 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.click]
     version = "8.1.7 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.colorama]
     version = "0.4.6 "
-    markers = 'python_version >= "3.10" and python_version < "3.13" and (sys_platform == "win32" or platform_system == "Windows")'
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.cryptography]
+    version = "42.0.7 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.cssselect]
+    version = "1.2.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.diskcache]
     version = "5.6.3 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
@@ -130,40 +150,50 @@
 
     [tool.poetry.dependencies.docker]
     version = "7.0.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.exceptiongroup]
-    version = "1.2.0 "
-    markers = 'python_version >= "3.10" and python_version < "3.11"'
+    version = "1.2.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.execnet]
+    version = "2.1.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.fastapi]
-    version = "0.110.1 "
+    version = "0.110.3 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.fasteners]
+    version = "0.19 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.filelock]
-    version = "3.13.4 "
+    version = "3.14.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.flaml]
     version = "2.1.2 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.frozenlist]
     version = "1.4.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.fsspec]
-    version = "2024.3.1 "
+    version = "2024.5.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.h11]
     version = "0.14.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
@@ -180,15 +210,15 @@
 
     [tool.poetry.dependencies.httpx]
     version = "0.27.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.huggingface-hub]
-    version = "0.22.2 "
+    version = "0.23.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.humancursor]
     version = "1.1.5 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
@@ -199,34 +229,54 @@
     optional = false
 
     [tool.poetry.dependencies.importlib-metadata]
     version = "7.1.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.iniconfig]
+    version = "2.0.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.jinja2]
-    version = "3.1.3 "
+    version = "3.1.4 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.jwcrypto]
+    version = "1.5.6 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.litellm]
-    version = "1.35.4 "
+    version = "1.37.16 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.lxml]
-    version = "5.2.1 "
+    version = "5.2.2 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.markdown-it-py]
+    version = "3.0.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.markupsafe]
     version = "2.1.5 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.mdurl]
+    version = "0.1.2 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.mouseinfo]
     version = "0.1.3 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.multidict]
     version = "6.0.5 "
@@ -235,15 +285,15 @@
 
     [tool.poetry.dependencies.numpy]
     version = "1.26.4 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.openai]
-    version = "1.17.1 "
+    version = "1.30.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.opencv-python]
     version = "4.9.0.80 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
@@ -254,55 +304,105 @@
     optional = false
 
     [tool.poetry.dependencies.packaging]
     version = "24.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.parameterized]
+    version = "0.9.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.parse-type]
+    version = "0.6.2 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.parse]
+    version = "1.20.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pdbp]
+    version = "1.5.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.pillow]
     version = "10.3.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.pip]
+    version = "24.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.platformdirs]
+    version = "4.2.2 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pluggy]
+    version = "1.5.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.py]
+    version = "1.11.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.pyautogen]
-    version = "0.2.23 "
+    version = "0.2.27 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
     extras = [ "lmm", "redis" ]
 
     [tool.poetry.dependencies.pyautogui]
     version = "0.9.54 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.pycparser]
     version = "2.22 "
-    markers = 'os_name == "nt" and implementation_name != "pypy" and python_version >= "3.10" and python_version < "3.13"'
+    markers = 'python_version >= "3.10" and python_version < "3.13" and (os_name == "nt" or platform_python_implementation != "PyPy") and (implementation_name != "pypy" or platform_python_implementation != "PyPy")'
     optional = false
 
     [tool.poetry.dependencies.pydantic-core]
-    version = "2.18.1 "
+    version = "2.18.2 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.pydantic]
-    version = "2.7.0 "
+    version = "2.7.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.pygetwindow]
     version = "0.0.9 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.pygments]
+    version = "2.18.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.pymsgbox]
     version = "1.0.9 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.pynose]
+    version = "1.5.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.pyobjc-core]
     version = "10.2 "
     markers = 'python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"'
     optional = false
 
     [tool.poetry.dependencies.pyobjc-framework-cocoa]
     version = "10.2 "
@@ -310,19 +410,29 @@
     optional = false
 
     [tool.poetry.dependencies.pyobjc-framework-quartz]
     version = "10.2 "
     markers = 'python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"'
     optional = false
 
+    [tool.poetry.dependencies.pyotp]
+    version = "2.9.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.pyperclip]
     version = "1.8.2 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.pyreadline3]
+    version = "3.4.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13" and platform_system == "Windows"'
+    optional = false
+
     [tool.poetry.dependencies.pyrect]
     version = "0.2.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.pyscreeze]
     version = "0.1.30 "
@@ -330,14 +440,44 @@
     optional = false
 
     [tool.poetry.dependencies.pysocks]
     version = "1.7.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.pytest-html]
+    version = "2.0.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pytest-metadata]
+    version = "3.1.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pytest-ordering]
+    version = "0.6 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pytest-rerunfailures]
+    version = "14.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pytest-xdist]
+    version = "3.6.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.pytest]
+    version = "8.2.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.python-dotenv]
     version = "1.0.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.python3-xlib]
     version = "0.15 "
@@ -345,51 +485,86 @@
     optional = false
 
     [tool.poetry.dependencies.pytweening]
     version = "1.2.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.pyvirtualdisplay]
+    version = "3.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.pywin32]
     version = "306 "
     markers = 'python_version >= "3.10" and python_version < "3.13" and sys_platform == "win32"'
     optional = false
 
     [tool.poetry.dependencies.pyyaml]
     version = "6.0.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.redis]
-    version = "5.0.3 "
+    version = "5.0.4 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.regex]
-    version = "2023.12.25 "
+    version = "2024.5.15 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.replicate]
-    version = "0.25.1 "
+    version = "0.26.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.requests]
     version = "2.31.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.rich]
+    version = "13.7.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.rubicon-objc]
-    version = "0.4.8 "
+    version = "0.4.9 "
     markers = 'python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"'
     optional = false
 
+    [tool.poetry.dependencies.sbvirtualdisplay]
+    version = "1.3.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.selenium]
-    version = "4.19.0 "
+    version = "4.21.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.seleniumbase]
+    version = "4.27.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.setuptools]
+    version = "69.5.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.simplejson]
+    version = "3.19.2 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.six]
+    version = "1.16.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.sniffio]
     version = "1.3.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
@@ -405,41 +580,51 @@
     optional = false
 
     [tool.poetry.dependencies.starlette]
     version = "0.37.2 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.tabcompleter]
+    version = "1.3.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.termcolor]
     version = "2.4.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.tiktoken]
-    version = "0.6.0 "
+    version = "0.7.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.tokenizers]
-    version = "0.15.2 "
+    version = "0.19.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.tomli]
+    version = "2.0.1 "
+    markers = 'python_version >= "3.10" and python_version < "3.11"'
+    optional = false
+
     [tool.poetry.dependencies.tqdm]
-    version = "4.66.2 "
+    version = "4.66.4 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.trio-websocket]
     version = "0.11.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.trio]
-    version = "0.25.0 "
+    version = "0.25.1 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.typing-extensions]
     version = "4.11.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
@@ -467,26 +652,36 @@
     optional = false
 
     [tool.poetry.dependencies.websockets]
     version = "12.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
+    [tool.poetry.dependencies.websockify]
+    version = "0.11.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
+    [tool.poetry.dependencies.wheel]
+    version = "0.43.0 "
+    markers = 'python_version >= "3.10" and python_version < "3.13"'
+    optional = false
+
     [tool.poetry.dependencies.wsproto]
     version = "1.2.0 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.yarl]
     version = "1.9.4 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
     [tool.poetry.dependencies.zipp]
-    version = "3.18.1 "
+    version = "3.18.2 "
     markers = 'python_version >= "3.10" and python_version < "3.13"'
     optional = false
 
 [tool.poetry.group.dev]
 dependencies = { }
 
 [build-system]
```

### Comparing `kbve-1.0.8/PKG-INFO` & `kbve-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,143 @@
 Metadata-Version: 2.1
 Name: kbve
-Version: 1.0.8
+Version: 1.0.9
 Summary: ATLAS
 License: Proprietary
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (==3.9.4) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: aiohttp (==3.9.5) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: aiosignal (==1.3.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: annotated-types (==0.6.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: anyio (==4.3.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: async-timeout (==4.0.3) ; python_version >= "3.10" and python_full_version < "3.11.3"
 Requires-Dist: asyncio-redis (==0.16.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: attrs (==23.2.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: beautifulsoup4 (==4.12.3) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: behave (==1.2.6) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: broadcaster[redis] (==0.2.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: certifi (==2024.2.2) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: cffi (==1.16.0) ; os_name == "nt" and implementation_name != "pypy" and python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: cffi (==1.16.0) ; python_version >= "3.10" and python_version < "3.13" and (os_name == "nt" or platform_python_implementation != "PyPy") and (implementation_name != "pypy" or platform_python_implementation != "PyPy")
+Requires-Dist: chardet (==5.2.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: charset-normalizer (==3.3.2) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: click (==8.1.7) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: colorama (==0.4.6) ; python_version >= "3.10" and python_version < "3.13" and (sys_platform == "win32" or platform_system == "Windows")
+Requires-Dist: colorama (==0.4.6) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: cryptography (==42.0.7) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: cssselect (==1.2.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: diskcache (==5.6.3) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: distro (==1.9.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: docker (==7.0.0) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: exceptiongroup (==1.2.0) ; python_version >= "3.10" and python_version < "3.11"
-Requires-Dist: fastapi (==0.110.1) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: filelock (==3.13.4) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: exceptiongroup (==1.2.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: execnet (==2.1.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: fastapi (==0.110.3) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: fasteners (==0.19) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: filelock (==3.14.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: flaml (==2.1.2) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: frozenlist (==1.4.1) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: fsspec (==2024.3.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: fsspec (==2024.5.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: h11 (==0.14.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: httpcore (==1.0.5) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: httptools (==0.6.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: httpx (==0.27.0) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: huggingface-hub (==0.22.2) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: huggingface-hub (==0.23.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: humancursor (==1.1.5) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: idna (==3.7) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: importlib-metadata (==7.1.0) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: jinja2 (==3.1.3) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: litellm (==1.35.4) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: lxml (==5.2.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: iniconfig (==2.0.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: jinja2 (==3.1.4) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: jwcrypto (==1.5.6) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: litellm (==1.37.16) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: lxml (==5.2.2) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: markdown-it-py (==3.0.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: markupsafe (==2.1.5) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: mdurl (==0.1.2) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: mouseinfo (==0.1.3) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: multidict (==6.0.5) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: numpy (==1.26.4) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: openai (==1.17.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: openai (==1.30.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: opencv-python (==4.9.0.80) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: outcome (==1.3.0.post0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: packaging (==24.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: parameterized (==0.9.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: parse (==1.20.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: parse-type (==0.6.2) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pdbp (==1.5.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pillow (==10.3.0) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: pyautogen[lmm,redis] (==0.2.23) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pip (==24.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: platformdirs (==4.2.2) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pluggy (==1.5.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: py (==1.11.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pyautogen[lmm,redis] (==0.2.27) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pyautogui (==0.9.54) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: pycparser (==2.22) ; os_name == "nt" and implementation_name != "pypy" and python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: pydantic (==2.7.0) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: pydantic-core (==2.18.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pycparser (==2.22) ; python_version >= "3.10" and python_version < "3.13" and (os_name == "nt" or platform_python_implementation != "PyPy") and (implementation_name != "pypy" or platform_python_implementation != "PyPy")
+Requires-Dist: pydantic (==2.7.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pydantic-core (==2.18.2) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pygetwindow (==0.0.9) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pygments (==2.18.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pymsgbox (==1.0.9) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pynose (==1.5.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pyobjc-core (==10.2) ; python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"
 Requires-Dist: pyobjc-framework-cocoa (==10.2) ; python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"
 Requires-Dist: pyobjc-framework-quartz (==10.2) ; python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"
+Requires-Dist: pyotp (==2.9.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pyperclip (==1.8.2) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pyreadline3 (==3.4.1) ; python_version >= "3.10" and python_version < "3.13" and platform_system == "Windows"
 Requires-Dist: pyrect (==0.2.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pyscreeze (==0.1.30) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pysocks (==1.7.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pytest (==8.2.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pytest-html (==2.0.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pytest-metadata (==3.1.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pytest-ordering (==0.6) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pytest-rerunfailures (==14.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pytest-xdist (==3.6.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: python-dotenv (==1.0.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: python3-xlib (==0.15) ; platform_system == "Linux" and python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pytweening (==1.2.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: pyvirtualdisplay (==3.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: pywin32 (==306) ; python_version >= "3.10" and python_version < "3.13" and sys_platform == "win32"
 Requires-Dist: pyyaml (==6.0.1) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: redis (==5.0.3) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: regex (==2023.12.25) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: replicate (==0.25.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: redis (==5.0.4) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: regex (==2024.5.15) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: replicate (==0.26.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: requests (==2.31.0) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: rubicon-objc (==0.4.8) ; python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"
-Requires-Dist: selenium (==4.19.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: rich (==13.7.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: rubicon-objc (==0.4.9) ; python_version >= "3.10" and python_version < "3.13" and platform_system == "Darwin"
+Requires-Dist: sbvirtualdisplay (==1.3.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: selenium (==4.21.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: seleniumbase (==4.27.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: setuptools (==69.5.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: simplejson (==3.19.2) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: six (==1.16.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: sniffio (==1.3.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: sortedcontainers (==2.4.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: soupsieve (==2.5) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: starlette (==0.37.2) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: tabcompleter (==1.3.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: termcolor (==2.4.0) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: tiktoken (==0.6.0) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: tokenizers (==0.15.2) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: tqdm (==4.66.2) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: trio (==0.25.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: tiktoken (==0.7.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: tokenizers (==0.19.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: tomli (==2.0.1) ; python_version >= "3.10" and python_version < "3.11"
+Requires-Dist: tqdm (==4.66.4) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: trio (==0.25.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: trio-websocket (==0.11.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: typing-extensions (==4.11.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: urllib3[socks] (==2.2.1) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: uvicorn[standard] (==0.29.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: uvloop (==0.19.0) ; (sys_platform != "win32" and sys_platform != "cygwin") and platform_python_implementation != "PyPy" and python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: watchfiles (==0.21.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: websockets (==12.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: websockify (==0.11.0) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: wheel (==0.43.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: wsproto (==1.2.0) ; python_version >= "3.10" and python_version < "3.13"
 Requires-Dist: yarl (==1.9.4) ; python_version >= "3.10" and python_version < "3.13"
-Requires-Dist: zipp (==3.18.1) ; python_version >= "3.10" and python_version < "3.13"
+Requires-Dist: zipp (==3.18.2) ; python_version >= "3.10" and python_version < "3.13"
 Description-Content-Type: text/markdown
 
 # atlas
 
 Project description here.
```

