# Comparing `tmp/fdk_asgi-0.5.0.tar.gz` & `tmp/fdk_asgi-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdk_asgi-0.5.0.tar", max compression
+gzip compressed data, was "fdk_asgi-0.6.0.tar", max compression
```

## Comparing `fdk_asgi-0.5.0.tar` & `fdk_asgi-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-01-14 21:23:24.869231 fdk_asgi-0.5.0/LICENSE
--rw-r--r--   0        0        0     7648 2024-01-14 21:23:24.869231 fdk_asgi-0.5.0/README.md
--rw-r--r--   0        0        0     2395 2024-01-14 21:23:24.869231 fdk_asgi-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-14 21:23:24.873231 fdk_asgi-0.5.0/src/fdk_asgi/__init__.py
--rw-r--r--   0        0        0     5300 2024-01-14 21:23:24.873231 fdk_asgi-0.5.0/src/fdk_asgi/app.py
--rw-r--r--   0        0        0     5955 2024-01-14 21:23:24.873231 fdk_asgi-0.5.0/src/fdk_asgi/cli.py
--rw-r--r--   0        0        0      880 2024-01-14 21:23:24.873231 fdk_asgi-0.5.0/src/fdk_asgi/exceptions.py
--rw-r--r--   0        0        0     4394 2024-01-14 21:23:24.873231 fdk_asgi-0.5.0/src/fdk_asgi/testing.py
--rw-r--r--   0        0        0      691 2024-01-14 21:23:24.873231 fdk_asgi-0.5.0/src/fdk_asgi/types.py
--rw-r--r--   0        0        0     2227 2024-01-14 21:23:24.873231 fdk_asgi-0.5.0/src/fdk_asgi/utils.py
--rw-r--r--   0        0        0     8437 1970-01-01 00:00:00.000000 fdk_asgi-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-26 20:19:20.202531 fdk_asgi-0.6.0/LICENSE
+-rw-r--r--   0        0        0     7648 2024-05-26 20:19:20.202531 fdk_asgi-0.6.0/README.md
+-rw-r--r--   0        0        0     2562 2024-05-26 20:19:20.202531 fdk_asgi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-26 20:19:20.202531 fdk_asgi-0.6.0/src/fdk_asgi/__init__.py
+-rw-r--r--   0        0        0     5300 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/app.py
+-rw-r--r--   0        0        0     5955 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/cli.py
+-rw-r--r--   0        0        0      880 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/exceptions.py
+-rw-r--r--   0        0        0      621 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/types.py
+-rw-r--r--   0        0        0     2227 2024-05-26 20:19:20.206531 fdk_asgi-0.6.0/src/fdk_asgi/utils.py
+-rw-r--r--   0        0        0     8478 1970-01-01 00:00:00.000000 fdk_asgi-0.6.0/PKG-INFO
```

### Comparing `fdk_asgi-0.5.0/LICENSE` & `fdk_asgi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.5.0/README.md` & `fdk_asgi-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.5.0/pyproject.toml` & `fdk_asgi-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+[project]
+name = "fdk-asgi"
+requires-python = ">=3.8"
+
 [tool.poetry]
 name = "fdk-asgi"
-version = "0.5.0"
+version = "0.6.0"
 description = "An alternative FDK to easily run any ASGI application on OCI Functions behind an API Gateway."
 authors = ["Björn Reetz <git@bjoern-reetz.de>"]
 readme = "README.md"
 packages = [{include = "fdk_asgi", from = "src"}]
 
 [tool.poetry.scripts]
 fdk-asgi-serve = 'fdk_asgi.cli:app'
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 asgiref = "^3.7.2"
 httptools = "^0.6.0"
 typer = { version = "^0.9.0", optional = true }
 uvicorn = { version = "^0.25", optional = true }
+strenum = "^0.4.15"
 
 [tool.poetry.extras]
 cli = ["typer", "uvicorn"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 httpx = "^0.26"
@@ -28,18 +33,23 @@
 trio = "^0.23.2"
 hypothesis = "^6.92.2"
 pytest-cov = "^4.1.0"
 setuptools = "^69.0.3"  # required by pybadges
 pybadges = "^3.0.1"
 typer = "*"
 uvicorn = "*"
+mypy = "^1.10.0"
 
 [tool.coverage.run]
 source = ["src", "tests"]
 
+[tool.mypy]
+files = "src"
+strict = true
+
 [tool.pytest.ini_options]
 addopts = [
     "--cov",
     "--cov-report=term:skip-covered",
     "--import-mode=importlib",
     "--strict-config",
     "--strict-markers",
@@ -94,15 +104,16 @@
     "RUF",
 ]
 
 [tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
 
 [tool.ruff.per-file-ignores]
-"**/test_*.py" = ["S101"]
+"tests/**/test_*.py" = ["S101"]
+"tests/utils.py" = ["S101"]
 "src/fdk_asgi/testing.py" = ["S101"]
 "src/fdk_asgi/cli.py" = ["FBT", "ERA001"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 version_scheme = "pep440"
```

### Comparing `fdk_asgi-0.5.0/src/fdk_asgi/app.py` & `fdk_asgi-0.6.0/src/fdk_asgi/app.py`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.5.0/src/fdk_asgi/cli.py` & `fdk_asgi-0.6.0/src/fdk_asgi/cli.py`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.5.0/src/fdk_asgi/exceptions.py` & `fdk_asgi-0.6.0/src/fdk_asgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.5.0/src/fdk_asgi/types.py` & `fdk_asgi-0.6.0/src/fdk_asgi/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import typing
-from enum import Enum
+
+from strenum import StrEnum
 
 Scope = typing.MutableMapping[str, typing.Any]
 Message = typing.MutableMapping[str, typing.Any]
 
 Receive = typing.Callable[[], typing.Awaitable[Message]]
 Send = typing.Callable[[Message], typing.Awaitable[None]]
 
 ASGIApp = typing.Callable[[Scope, Receive, Send], typing.Awaitable[None]]
 
 
-class StrEnum(str, Enum):
-    def __str__(self):
-        return self.value
-
-
 class HTTPProtocolType(StrEnum):
     auto = "auto"
     h11 = "h11"
     httptools = "httptools"
 
 
 class LifespanType(StrEnum):
```

### Comparing `fdk_asgi-0.5.0/src/fdk_asgi/utils.py` & `fdk_asgi-0.6.0/src/fdk_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.5.0/PKG-INFO` & `fdk_asgi-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: fdk-asgi
-Version: 0.5.0
+Version: 0.6.0
 Summary: An alternative FDK to easily run any ASGI application on OCI Functions behind an API Gateway.
 Author: Björn Reetz
 Author-email: git@bjoern-reetz.de
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: cli
 Requires-Dist: asgiref (>=3.7.2,<4.0.0)
 Requires-Dist: httptools (>=0.6.0,<0.7.0)
+Requires-Dist: strenum (>=0.4.15,<0.5.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0) ; extra == "cli"
 Requires-Dist: uvicorn (>=0.25,<0.26) ; extra == "cli"
 Description-Content-Type: text/markdown
 
 # fdk-asgi
 
 [![pipeline status](https://github.com/bjoern-reetz/fdk-asgi/actions/workflows/publish.yml/badge.svg?main)](https://github.com/bjoern-reetz/fdk-asgi/actions/workflows/publish.yml)
```

