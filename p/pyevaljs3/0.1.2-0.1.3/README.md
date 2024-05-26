# Comparing `tmp/pyevaljs3-0.1.2.tar.gz` & `tmp/pyevaljs3-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevaljs3-0.1.2.tar", last modified: Sat May 18 11:41:23 2024, max compression
+gzip compressed data, was "pyevaljs3-0.1.3.tar", last modified: Sun May 26 10:22:45 2024, max compression
```

## Comparing `pyevaljs3-0.1.2.tar` & `pyevaljs3-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 11:41:23.752388 pyevaljs3-0.1.2/
--rw-rw-rw-   0        0        0     1093 2023-12-13 10:50:19.000000 pyevaljs3-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3332 2024-05-18 11:41:23.751387 pyevaljs3-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2542 2024-03-04 18:42:48.000000 pyevaljs3-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 11:41:23.730365 pyevaljs3-0.1.2/pyevaljs3/
--rw-rw-rw-   0        0        0     2565 2024-03-04 18:41:30.000000 pyevaljs3-0.1.2/pyevaljs3/__init__.py
--rw-rw-rw-   0        0        0       55 2024-05-18 11:35:06.000000 pyevaljs3-0.1.2/pyevaljs3/__version__.py
--rw-rw-rw-   0        0        0     1860 2024-05-18 11:31:35.000000 pyevaljs3-0.1.2/pyevaljs3/evaljs.py
--rw-rw-rw-   0        0        0       96 2023-12-13 08:02:55.000000 pyevaljs3-0.1.2/pyevaljs3/exception.py
--rw-rw-rw-   0        0        0     4200 2024-03-04 18:58:31.000000 pyevaljs3-0.1.2/pyevaljs3/runtime.py
-drwxrwxrwx   0        0        0        0 2024-05-18 11:41:23.749387 pyevaljs3-0.1.2/pyevaljs3.egg-info/
--rw-rw-rw-   0        0        0     3332 2024-05-18 11:41:23.000000 pyevaljs3-0.1.2/pyevaljs3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-05-18 11:41:23.000000 pyevaljs3-0.1.2/pyevaljs3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 11:41:23.000000 pyevaljs3-0.1.2/pyevaljs3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 11:41:23.000000 pyevaljs3-0.1.2/pyevaljs3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 11:41:23.753388 pyevaljs3-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1193 2024-03-04 17:52:32.000000 pyevaljs3-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 11:41:23.748386 pyevaljs3-0.1.2/tests/
--rw-rw-rw-   0        0        0      792 2024-03-04 18:42:48.000000 pyevaljs3-0.1.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:22:45.515473 pyevaljs3-0.1.3/
+-rw-rw-rw-   0        0        0     1093 2023-12-13 10:50:19.000000 pyevaljs3-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3332 2024-05-26 10:22:45.514473 pyevaljs3-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2542 2024-03-04 18:42:48.000000 pyevaljs3-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 10:22:45.498469 pyevaljs3-0.1.3/pyevaljs3/
+-rw-rw-rw-   0        0        0     2565 2024-03-04 18:41:30.000000 pyevaljs3-0.1.3/pyevaljs3/__init__.py
+-rw-rw-rw-   0        0        0       55 2024-05-26 10:20:50.000000 pyevaljs3-0.1.3/pyevaljs3/__version__.py
+-rw-rw-rw-   0        0        0      329 2024-05-26 10:11:11.000000 pyevaljs3-0.1.3/pyevaljs3/_node_program.py
+-rw-rw-rw-   0        0        0     1860 2024-05-18 11:31:35.000000 pyevaljs3-0.1.3/pyevaljs3/evaljs.py
+-rw-rw-rw-   0        0        0       96 2023-12-13 08:02:55.000000 pyevaljs3-0.1.3/pyevaljs3/exception.py
+-rw-rw-rw-   0        0        0      462 2024-05-26 10:17:44.000000 pyevaljs3-0.1.3/pyevaljs3/runner.py
+-rw-rw-rw-   0        0        0     4095 2024-05-26 10:17:59.000000 pyevaljs3-0.1.3/pyevaljs3/runtime.py
+-rw-rw-rw-   0        0        0       97 2024-05-26 10:20:03.000000 pyevaljs3-0.1.3/pyevaljs3/setting.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:22:45.513473 pyevaljs3-0.1.3/pyevaljs3.egg-info/
+-rw-rw-rw-   0        0        0     3332 2024-05-26 10:22:45.000000 pyevaljs3-0.1.3/pyevaljs3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-05-26 10:22:45.000000 pyevaljs3-0.1.3/pyevaljs3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:22:45.000000 pyevaljs3-0.1.3/pyevaljs3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-26 10:22:45.000000 pyevaljs3-0.1.3/pyevaljs3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:22:45.516474 pyevaljs3-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2024-03-04 17:52:32.000000 pyevaljs3-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:22:45.511472 pyevaljs3-0.1.3/tests/
+-rw-rw-rw-   0        0        0      790 2024-05-26 08:12:35.000000 pyevaljs3-0.1.3/tests/test.py
```

### Comparing `pyevaljs3-0.1.2/LICENSE` & `pyevaljs3-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.2/PKG-INFO` & `pyevaljs3-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyevaljs3
-Version: 0.1.2
+Version: 0.1.3
 Summary: 一个依赖node.js来执行js代码的python库
 Home-page: https://github.com/Smawexi/PyevalJS3
 Author: Samwe
 Author-email: 1281722462@qq.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyevaljs3-0.1.2/README.md` & `pyevaljs3-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.2/pyevaljs3/__init__.py` & `pyevaljs3-0.1.3/pyevaljs3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.2/pyevaljs3/evaljs.py` & `pyevaljs3-0.1.3/pyevaljs3/evaljs.py`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.2/pyevaljs3/runtime.py` & `pyevaljs3-0.1.3/pyevaljs3/runtime.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 import subprocess
 import logging
 import json
 import abc
 import tempfile
 
 from . import exception
+from .setting import IS_WINDOWS, NO_WARNINGS
+from .runner import Runner
 JSException = exception.JSException
 _logger = logging.getLogger("JSEval")
+if not IS_WINDOWS:
+    subprocess.DETACHED_PROCESS = 0
 
 
 def get_node_env():
     node = os.environ.get('NODE_PATH') if os.environ.get('NODE_PATH') else os.environ.get('NODE')
     if not node:
         return "node"
     return node
@@ -31,16 +35,16 @@
 
     @abc.abstractmethod
     def compile(self, source: str = None, suffix: str = None):
         raise NotImplementedError()
 
     def _eval(self, code: str = None, ignore_output=False):
         node = get_node_env()
-        _cmd = [node, "--no-warnings"]
-        _input = f'var __result = (() => {{{code}}})();if (__result !== undefined) {{console.log("JSEval_state: ok");console.log(JSON.stringify(__result));}};'
+        _cmd = [node, NO_WARNINGS]
+        _input = Runner.program('eval', code)
         popen = subprocess.Popen(_cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
                                  universal_newlines=True, creationflags=subprocess.DETACHED_PROCESS)
         try:
             outs, errs = popen.communicate(input=_input)
         except Exception as e:
             _logger.error(e)
             popen.kill()
@@ -78,17 +82,17 @@
 
     @abc.abstractmethod
     def call(self, *args, **kwargs):
         raise NotImplementedError()
 
     def _call(self, func, args):
         node = get_node_env()
-        _source = f'{self._source};var __result = {func}.apply(this, {args});if (__result !== undefined) {{console.log("JSEval_state: ok");console.log(JSON.stringify(__result));}}'
+        _source = Runner.program('call', self._source, func, args)
         _path = self._make_temp_file(_source)
-        _cmd = [node, "--no-warnings", _path]
+        _cmd = [node, NO_WARNINGS, _path]
         popen = subprocess.Popen(_cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
                                  universal_newlines=True, creationflags=subprocess.DETACHED_PROCESS)
         try:
             outs, errs = popen.communicate()
         except Exception as e:
             _logger.error(e)
             popen.kill()
```

### Comparing `pyevaljs3-0.1.2/pyevaljs3.egg-info/PKG-INFO` & `pyevaljs3-0.1.3/pyevaljs3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyevaljs3
-Version: 0.1.2
+Version: 0.1.3
 Summary: 一个依赖node.js来执行js代码的python库
 Home-page: https://github.com/Smawexi/PyevalJS3
 Author: Samwe
 Author-email: 1281722462@qq.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyevaljs3-0.1.2/setup.py` & `pyevaljs3-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.2/tests/test.py` & `pyevaljs3-0.1.3/tests/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-
 import pyevaljs3
 
 payload = {
         "cursor_score": "", "num": 31, "refresh_type": 1, "note_index": 35, "unread_begin_note_id": "",
         "unread_end_note_id": "", "unread_note_count": 0, "category": "homefeed_recommend", "search_key": "",
         "need_num": 6, "image_formats": ["jpg", "webp", "avif"]
     }
```

