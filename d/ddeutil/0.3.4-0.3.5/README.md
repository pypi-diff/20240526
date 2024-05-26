# Comparing `tmp/ddeutil-0.3.4.tar.gz` & `tmp/ddeutil-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil-0.3.4.tar", last modified: Mon May 13 04:02:15 2024, max compression
+gzip compressed data, was "ddeutil-0.3.5.tar", last modified: Sun May 26 07:08:30 2024, max compression
```

## Comparing `ddeutil-0.3.4.tar` & `ddeutil-0.3.5.tar`

### file list

```diff
@@ -1,36 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:02:15.099546 ddeutil-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-13 04:02:08.000000 ddeutil-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 04:02:15.099546 ddeutil-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-13 04:02:08.000000 ddeutil-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-13 04:02:08.000000 ddeutil-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 04:02:15.099546 ddeutil-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:02:15.091546 ddeutil-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:02:15.091546 ddeutil-0.3.4/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:02:15.095546 ddeutil-0.3.4/src/ddeutil/core/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__about__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:02:15.095546 ddeutil-0.3.4/src/ddeutil/core/__base/
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__base/__types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__base/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__base/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__base/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__base/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__base/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__base/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__base/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:02:15.095546 ddeutil-0.3.4/src/ddeutil/core/base/
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/dtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-13 04:02:08.000000 ddeutil-0.3.4/src/ddeutil/core/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:02:15.099546 ddeutil-0.3.4/src/ddeutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-13 04:02:15.000000 ddeutil-0.3.4/src/ddeutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 04:02:15.000000 ddeutil-0.3.4/src/ddeutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 04:02:15.000000 ddeutil-0.3.4/src/ddeutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 04:02:15.000000 ddeutil-0.3.4/src/ddeutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 04:02:15.000000 ddeutil-0.3.4/src/ddeutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:02:15.099546 ddeutil-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-13 04:02:08.000000 ddeutil-0.3.4/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 04:02:08.000000 ddeutil-0.3.4/tests/test_dtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-13 04:02:08.000000 ddeutil-0.3.4/tests/test_randomly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:08:30.453540 ddeutil-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-26 07:08:24.000000 ddeutil-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-26 07:08:30.449540 ddeutil-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-26 07:08:24.000000 ddeutil-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-26 07:08:24.000000 ddeutil-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:08:30.453540 ddeutil-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:08:30.445540 ddeutil-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:08:30.445540 ddeutil-0.3.5/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:08:30.449540 ddeutil-0.3.5/src/ddeutil/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__about__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:08:30.449540 ddeutil-0.3.5/src/ddeutil/core/__base/
+-rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__base/__types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__base/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__base/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__base/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__base/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__base/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__base/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__base/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/dtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-26 07:08:24.000000 ddeutil-0.3.5/src/ddeutil/core/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:08:30.449540 ddeutil-0.3.5/src/ddeutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-26 07:08:30.000000 ddeutil-0.3.5/src/ddeutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-26 07:08:30.000000 ddeutil-0.3.5/src/ddeutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:08:30.000000 ddeutil-0.3.5/src/ddeutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 07:08:30.000000 ddeutil-0.3.5/src/ddeutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-26 07:08:30.000000 ddeutil-0.3.5/src/ddeutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:08:30.449540 ddeutil-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_dtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_randomly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-26 07:08:24.000000 ddeutil-0.3.5/tests/test_split.py
```

### Comparing `ddeutil-0.3.4/LICENSE` & `ddeutil-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.4/PKG-INFO` & `ddeutil-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil
-Version: 0.3.4
+Version: 0.3.5
 Summary: Data Developer & Engineer Core Utility Objects
 Author-email: korawica <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil/
 Keywords: data,utility
 Classifier: Topic :: Utilities
```

### Comparing `ddeutil-0.3.4/README.md` & `ddeutil-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.4/pyproject.toml` & `ddeutil-0.3.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT"}
 authors = [{ name = "korawica", email = "korawich.anu@gmail.com" }]
 keywords = ['data', 'utility']
 classifiers = [
     "Topic :: Utilities",
     "Natural Language :: English",
-    # "Development Status :: 3 - Alpha",
     "Development Status :: 4 - Beta",
-    # "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -48,15 +46,24 @@
 changelog = "CHANGELOG.md"
 
 [tool.coverage.run]
 branch = true
 relative_files = true
 concurrency = ["thread", "multiprocessing"]
 source = ["ddeutil", "tests"]
-omit = ["perf_*.py"]
+omit = [
+    "perf_*.py",
+    "core/__init__.py",
+]
+
+[tool.coverage.report]
+exclude_lines = [
+    "raise NotImplementedError",
+    "no cove",
+]
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 console_output_style = "count"
 addopts = [
     "--strict-config",
     "--strict-markers",
@@ -81,27 +88,29 @@
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [tool.black]
 line-length = 80
 target-version = ['py39']
 exclude = """
-/(
-    \\.git
-    | \\.__pycache__
-    | \\.idea
-    | \\.ruff_cache
-    | \\.mypy_cache
-    | \\.pytest_cache
-    | \\.venv
-    | _build
-    | buck-out
-    | build
-    | dist
-)/
+(
+    /(
+        \\.git
+        | \\.eggs
+        | \\.__pycache__
+        | \\.idea
+        | \\.ruff_cache
+        | \\.mypy_cache
+        | \\.pytest_cache
+        | \\.venv
+        | build
+        | dist
+        | venv
+    )/
+)
 """
 
 [tool.ruff]
 line-length = 80
 exclude = [
     ".git",
     ".mypy_cache",
@@ -118,14 +127,15 @@
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
+    "E203",  # whitespace before punctuation
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `ddeutil-0.3.4/src/ddeutil/core/__base/__init__.py` & `ddeutil-0.3.5/src/ddeutil/core/__base/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import importlib
 import operator
 import sys
 import typing
 from collections.abc import Callable, Collection
+from functools import partial
 from math import ceil
 
 from .cache import (
     clear_cache,
     memoize,
     memoized_property,
 )
@@ -56,15 +57,15 @@
 )
 
 T = typing.TypeVar("T")
 
 concat: typing.Callable[[typing.Any], str] = "".join
 
 
-def operate(x):
+def operate(x):  # no cove
     return getattr(operator, x)
 
 
 def is_generic(t: type):
     """Return True if type in the generic alias type."""
     return hasattr(t, "__origin__")
 
@@ -163,14 +164,19 @@
     except AttributeError as err:
         raise ImportError(
             f'Module "{module_path}" does not define a "{class_name}" '
             f"attribute/class"
         ) from err
 
 
+def lazy(module: str):
+    """Lazy use import_string function that warpped with partial function."""
+    return partial(import_string, module)
+
+
 def round_up(number: float, decimals):
     """
     Examples:
         >>> round_up(1.00406, 2)
         1.01
         >>> round_up(1.00001, 1)
         1.1
```

### Comparing `ddeutil-0.3.4/src/ddeutil/core/__base/cache.py` & `ddeutil-0.3.5/src/ddeutil/core/__base/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             return self.cache[key]
 
         value: Any = self.function(*args, **kwargs)
         self.cache[key] = value
         return value
 
 
-def memoized_property(func_get):
+def memoized_property(func_get):  # no cove
     """Return a property attribute for new-style classes that only calls its
     getter on the first access. The result is stored and on subsequent
     accesses is returned, preventing the need to call the getter anymore.
 
     :usage:
         >>> class C(object):
         ...     load_name_count = 0
@@ -70,15 +70,15 @@
         if not hasattr(self, attr_name):
             setattr(self, attr_name, func_get(self))
         return getattr(self, attr_name)
 
     return property(func_get_memoized)
 
 
-def clear_cache(attrs: tuple):
+def clear_cache(attrs: tuple):  # no cove
     """Clear or delete attribute value of the class that implement cache.
     :usage:
         >>> class C(object):
         ...     load_name_count = 0
         ...     @memoized_property
         ...     def name(self) -> str:
         ...         "name's docstring"
```

### Comparing `ddeutil-0.3.4/src/ddeutil/core/__base/checker.py` & `ddeutil-0.3.5/src/ddeutil/core/__base/checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "0",
     "0.0",
     "x",
 )
 
 
 def is_int(value: Any) -> bool:
-    """Check value that is integer.
+    """Check value that be integer.
 
     Examples:
         >>> is_int('')
         False
         >>> is_int('0.0')
         False
         >>> is_int('-3'), int('-3')
```

### Comparing `ddeutil-0.3.4/src/ddeutil/core/__base/convert.py` & `ddeutil-0.3.5/src/ddeutil/core/__base/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,19 @@
                 f"can not convert string value {value!r} to int or float"
             ) from err
 
 
 def must_list(value: Optional[Union[str, list[Any]]] = None) -> list[Any]:
     """Return the list value that was converted from string or list value.
 
+    :param value: A value that will validate and force to list value.
+    :type value: str | list[Any] | None
+
+    :rtype: list[Any]
+
     Examples:
         >>> must_list('[1, 2, 3]')
         [1, 2, 3]
         >>> must_list(None)
         []
     """
     if value:
```

### Comparing `ddeutil-0.3.4/src/ddeutil/core/__base/hash.py` & `ddeutil-0.3.5/src/ddeutil/core/__base/hash.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,33 +104,33 @@
     """
     return hmac.compare_digest(
         pw_hash, hashlib.pbkdf2_hmac("sha256", password.encode(), salt, 100000)
     )
 
 
 def tokenize(*args, **kwargs):
-    """Deterministic token (modified from dask.base)
+    """Deterministic token (modified from dask.base).
 
     Examples:
         >>> tokenize([1, 2, '3'])
         '9d71491b50023b06fc76928e6eddb952'
         >>> tokenize('Hello') == tokenize('Hello')
         True
     """
     if kwargs:
         args += (kwargs,)
     try:
         rs = hashlib.md5(str(args).encode())
-    except ValueError:
+    except ValueError:  # no cove
         # FIPS systems: https://github.com/fsspec/filesystem_spec/issues/380
         rs = hashlib.md5(str(args).encode(), usedforsecurity=False)
     return rs.hexdigest()
 
 
-def freeze(value: Any) -> Any:
+def freeze(value: Any) -> Any:  # no cove
     """Freeze a value to immutable object.
     Examples:
         >>> freeze({'foo': 'bar'})
         frozenset({('foo', 'bar')})
         >>> freeze('foo')
         'foo'
         >>> freeze(('foo', 'bar'))
@@ -141,15 +141,15 @@
     elif isinstance(value, list):
         return tuple(freeze(value) for value in value)
     elif isinstance(value, set):
         return frozenset(freeze(value) for value in value)
     return value
 
 
-def freeze_args(func):
+def freeze_args(func):  # no cove
     """Transform mutable dictionary into immutable useful to be compatible with
     cache.
 
     Examples:
         >>> from functools import lru_cache
         ... @lru_cache(maxsize=None)
         ... def call_name(value: dict):
@@ -181,12 +181,12 @@
             for k, v in kwargs.items()
         }
         return func(*args, **kwargs)
 
     return wrapped
 
 
-def random_str(num_length: int = 8) -> str:
+def random_str(num_length: int = 8) -> str:  # no cov
     """Random string from uppercase ASCII and number 0-9"""
     return "".join(
         random.choices(string.ascii_uppercase + string.digits, k=num_length)
     )
```

### Comparing `ddeutil-0.3.4/src/ddeutil/core/__base/merge.py` & `ddeutil-0.3.5/src/ddeutil/core/__base/merge.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.4/src/ddeutil/core/__base/sorting.py` & `ddeutil-0.3.5/src/ddeutil/core/__base/sorting.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     elif isinstance(value, list):
         return sorted(ordered(x) for x in value)
     return value
 
 
 def sort_priority(
     values: Union[list[T], set[T], tuple[T, ...]],
+    *,
     priority: list[T],
     reverse: bool = False,
     mode: Optional[str] = None,
 ) -> list[T]:
     """Sorts an iterable according to a list of priority items.
 
     Examples:
```

### Comparing `ddeutil-0.3.4/src/ddeutil/core/__base/splitter.py` & `ddeutil-0.3.5/src/ddeutil/core/__base/splitter.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.4/src/ddeutil/core/__init__.py` & `ddeutil-0.3.5/src/ddeutil/core/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,23 +12,25 @@
     hash_all,
     hash_pwd,
     hash_str,
     import_string,
     is_generic,
     is_int,
     isinstance_check,
+    lazy,
     memoize,
     memoized_property,
     merge_dict,
     merge_dict_value,
     merge_dict_values,
     merge_list,
     merge_values,
     must_bool,
     must_list,
+    must_rsplit,
     must_split,
     onlyone,
     operate,
     ordered,
     random_str,
     remove_pad,
     round_up,
```

### Comparing `ddeutil-0.3.4/src/ddeutil/core/decorator.py` & `ddeutil-0.3.5/src/ddeutil/core/decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 import contextlib
 import copy
 import functools
 import inspect
+import logging
+import time
 import warnings
+from collections.abc import Generator
 from functools import wraps
-from time import (
-    sleep,
-    time,
-)
 from typing import TYPE_CHECKING, Any, Callable, TypeVar
 
 if TYPE_CHECKING:
     import sys
 
     if sys.version_info >= (3, 10):
         from typing import ParamSpec
@@ -26,15 +25,15 @@
 
 STR_TYPES = (bytes, str)
 
 
 def deepcopy(func: Callable[P, T]) -> Callable[P, T]:
     """Deep copy method
 
-    EExamples:
+    Examples:
         >>> @deepcopy
         ... def foo(a, b, c=None):
         ...     c = c or {}
         ...     a[1] = 3
         ...     b[2] = 4
         ...     c[3] = 5
         ...     return a, b, c
@@ -100,17 +99,17 @@
         ...     time.sleep(2)
         ...     return
         >>> will_sleep()
         Execution time: 2.003119945526123 seconds
     """
 
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
-        start_time = time()
+        start_time = time.monotonic()
         result = func(*args, **kwargs)
-        execution_time = time() - start_time
+        execution_time = time.monotonic() - start_time
         print(f"Execution time: {execution_time} seconds")
         return result
 
     return wrapper
 
 
 def timing(name: str) -> Callable[[Callable[P, T]], Callable[P, T]]:
@@ -124,60 +123,64 @@
         >>> will_sleep()
         Sleep ....................................................... 2.01s
     """
 
     def timing_internal(func: Callable[P, T]) -> Callable[P, T]:
         @wraps(func)
         def wrap(*args: P.args, **kw: P.kwargs) -> T:
-            ts = time()
+            ts = time.monotonic()
             result = func(*args, **kw)
             padded_name: str = f"{name} ".ljust(60, ".")
-            padded_time: str = f" {(time() - ts):0.2f}".rjust(6, ".")
+            padded_time: str = f" {(time.monotonic() - ts):0.2f}".rjust(6, ".")
             print(f"{padded_name}{padded_time}s", flush=True)
             return result
 
         return wrap
 
     return timing_internal
 
 
 @contextlib.contextmanager
-def timer_perf(title: str):
+def timer_perf(title: str) -> Generator[None, None, None]:
     """
     Examples:
         >>> import time
         >>> with timer_perf('Sleep'):
         ...     time.sleep(2)
         Sleep ....................................................... 2.00s
     """
-    ts = time()
-    yield
-    te = time()
-    padded_name: str = f"{title} ".ljust(60, ".")
-    padded_time: str = f" {(te - ts):0.2f}".rjust(6, ".")
-    print(f"{padded_name}{padded_time}s", flush=True)
+    ts = time.monotonic()
+    try:
+        yield
+    finally:
+        te = time.monotonic()
+        padded_name: str = f"{title} ".ljust(60, ".")
+        padded_time: str = f" {(te - ts):0.2f}".rjust(6, ".")
+        logging.debug(f"{padded_name}{padded_time}s")
 
 
-def debug(func: Callable[P, T]) -> Callable[P, T]:
+def debug(func: Callable[P, T]) -> Callable[P, T]:  # no cove
     """
     Examples:
         >>> @debug
         ... def add_numbers(x, y):
         ...     return x + y
         >>> add_numbers(7, y=5, )
         Calling add_numbers with args: (7,) kwargs: {'y': 5}
         add_numbers returned: 12
         12
     """
 
     @wraps(func)
     def wrapper(*args: P.args, **kwargs: P.kwargs):
-        print(f"Calling {func.__name__} with args: {args} kwargs: {kwargs}")
+        logging.debug(
+            f"Calling {func.__name__} with args: {args} kwargs: {kwargs}"
+        )
         result = func(*args, **kwargs)
-        print(f"{func.__name__} returned: {result}")
+        logging.debug(f"{func.__name__} returned: {result}")
         return result
 
     return wrapper
 
 
 def validate_input(
     *validations: tuple[Callable[[Any], bool]],
@@ -210,15 +213,15 @@
 
     return decorator
 
 
 def retry(
     max_attempts: int,
     delay: int = 1,
-) -> Callable[[Callable[P, T]], Callable[P, T]]:
+) -> Callable[[Callable[P, T]], Callable[P, T]]:  # no cove
     """Retry decorator with sequencial.
     Examples:
         >>> @retry(max_attempts=3, delay=2)
         ... def fetch_data(url):
         ...     print("Fetching the data ...")
         ...     raise TimeoutError("Server is not responding.")
         >>> fetch_data("https://example.com/data")
@@ -236,17 +239,17 @@
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
             _attempts: int = 0
             while _attempts < max_attempts:
                 try:
                     return func(*args, **kwargs)
                 except Exception as e:
                     _attempts += 1
-                    print(f"Attempt {_attempts} failed: {e}")
-                    sleep(delay)
-            print(
+                    logging.info(f"Attempt {_attempts} failed: {e}")
+                    time.sleep(delay)
+            logging.debug(
                 f"Function `{func.__name__}` failed after "
                 f"{max_attempts} attempts"
             )
 
         return wrapper
 
     return decorator
```

### Comparing `ddeutil-0.3.4/src/ddeutil/core/dtutils.py` & `ddeutil-0.3.5/src/ddeutil/core/dtutils.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.4/src/ddeutil/core/threader.py` & `ddeutil-0.3.5/src/ddeutil/core/threader.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.4/src/ddeutil.egg-info/PKG-INFO` & `ddeutil-0.3.5/src/ddeutil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil
-Version: 0.3.4
+Version: 0.3.5
 Summary: Data Developer & Engineer Core Utility Objects
 Author-email: korawica <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil/
 Keywords: data,utility
 Classifier: Topic :: Utilities
```

### Comparing `ddeutil-0.3.4/src/ddeutil.egg-info/SOURCES.txt` & `ddeutil-0.3.5/src/ddeutil.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,11 +16,18 @@
 src/ddeutil/core/__base/cache.py
 src/ddeutil/core/__base/checker.py
 src/ddeutil/core/__base/convert.py
 src/ddeutil/core/__base/hash.py
 src/ddeutil/core/__base/merge.py
 src/ddeutil/core/__base/sorting.py
 src/ddeutil/core/__base/splitter.py
-src/ddeutil/core/base/__init__.py
+tests/test_base.py
+tests/test_cache.py
+tests/test_checker.py
+tests/test_convert.py
 tests/test_decorator.py
 tests/test_dtutils.py
-tests/test_randomly.py
+tests/test_hash.py
+tests/test_merge.py
+tests/test_randomly.py
+tests/test_sorting.py
+tests/test_split.py
```

