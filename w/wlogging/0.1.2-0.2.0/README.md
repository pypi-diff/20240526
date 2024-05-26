# Comparing `tmp/wlogging-0.1.2.tar.gz` & `tmp/wlogging-0.2.0.tar.gz`

## Comparing `wlogging-0.1.2.tar` & `wlogging-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 wlogging-0.1.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 wlogging-0.1.2/src/wlogging/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 wlogging-0.1.2/src/wlogging/formatters.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 wlogging-0.1.2/src/wlogging/loggers.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 wlogging-0.1.2/.gitignore
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 wlogging-0.1.2/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 wlogging-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 wlogging-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 wlogging-0.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 wlogging-0.2.0/src/wlogging/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 wlogging-0.2.0/src/wlogging/formatters.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 wlogging-0.2.0/src/wlogging/loggers.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 wlogging-0.2.0/.gitignore
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 wlogging-0.2.0/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 wlogging-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 wlogging-0.2.0/PKG-INFO
```

### Comparing `wlogging-0.1.2/.github/workflows/publish-to-pypi.yml` & `wlogging-0.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `wlogging-0.1.2/src/wlogging/__init__.py` & `wlogging-0.2.0/src/wlogging/__init__.py`

 * *Files identical despite different names*

### Comparing `wlogging-0.1.2/src/wlogging/formatters.py` & `wlogging-0.2.0/src/wlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `wlogging-0.1.2/src/wlogging/loggers.py` & `wlogging-0.2.0/src/wlogging/loggers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 """
 """
 
 
 #[
 from __future__ import annotations
 
-import types
+from types import (MethodType, )
+import functools as _ft
 
 import logging
 from . import formatters as _formatters
 #]
 
 
-__all__ = [
+__all__ = (
     "get_colored_logger",
-]
+    "get_colored_two_liner",
+)
 
 
 def get_colored_logger(
     name: str | None = None,
-    propagate: bool = True,
     level: int = logging.WARNING,
     format: str = "%(asctime)s | %(levelname)s | %(name)s | %(message)s",
+    propagate: bool = True,
     remove_existing_handlers: bool = True,
 ) -> logging.Logger:
     """
     """
     logger = logging.getLogger(name, )
-    logger.clear_handlers = types.MethodType(_clear_handlers, logger, )
+    logger.clear_handlers = MethodType(_clear_handlers, logger, )
     logger.propagate = propagate
     if remove_existing_handlers:
         logger.clear_handlers()
     handler = logging.StreamHandler()
     formatter = _formatters.ColoredFormatter(format, )
     handler.set_formatter(formatter, )
     logger.addHandler(handler, )
     logger.setLevel(level, )
     logger._decorated = True
     return logger
 
 
+get_colored_two_liner = _ft.partial(
+    get_colored_logger,
+    format="%(asctime)s | %(levelname)s | %(name)s:\n••• %(message)s",
+)
+
+
 def _clear_handlers(logger: Logger, ) -> None:
     for handler in logger.handlers:
         logger.remove_handler(handler, )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wlogging-0.1.2/pyproject.toml` & `wlogging-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["hatchling"]
     build-backend = "hatchling.build"
 
 [project]
     name = "wlogging"
-    version = "0.1.2"
+    version = "0.2.0"
     authors = [
       { name="Jaromir Benes", email="jaromir.benes@gmail.com" },
     ]
     description = "Pythonic wrapper for the standard logging module"
     readme = "README.md"
     requires-python = ">=3.11"
     classifiers = [
```

### Comparing `wlogging-0.1.2/PKG-INFO` & `wlogging-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: wlogging
-Version: 0.1.2
+Version: 0.2.0
 Summary: Pythonic wrapper for the standard logging module
 Project-URL: Homepage, https://github.com/iris-solutions-team/wlogging
 Project-URL: Bug Tracker, https://github.com/iris-solutions-team/wlogging/issues
 Author-email: Jaromir Benes <jaromir.benes@gmail.com>
 Keywords: logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

