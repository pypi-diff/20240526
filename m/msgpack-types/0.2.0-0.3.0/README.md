# Comparing `tmp/msgpack-types-0.2.0.tar.gz` & `tmp/msgpack_types-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgpack-types-0.2.0.tar", last modified: Sat Jul 24 23:28:49 2021, max compression
+gzip compressed data, was "msgpack_types-0.3.0.tar", max compression
```

## Comparing `msgpack-types-0.2.0.tar` & `msgpack_types-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11357 2020-12-12 03:11:33.658845 msgpack-types-0.2.0/LICENSE
--rw-r--r--   0        0        0      475 2021-02-27 16:38:56.724599 msgpack-types-0.2.0/README.md
--rw-r--r--   0        0        0     2466 2020-12-12 03:06:22.337405 msgpack-types-0.2.0/msgpack-stubs/__init__.pyi
--rw-r--r--   0        0        0       56 2020-12-12 00:34:47.075356 msgpack-types-0.2.0/msgpack-stubs/_version.pyi
--rw-r--r--   0        0        0      460 2020-12-12 00:37:54.216491 msgpack-types-0.2.0/msgpack-stubs/exceptions.pyi
--rw-r--r--   0        0        0      849 2021-07-24 23:28:20.077870 msgpack-types-0.2.0/msgpack-stubs/ext.pyi
--rw-r--r--   0        0        0     2760 2020-12-12 03:06:46.020461 msgpack-types-0.2.0/msgpack-stubs/fallback.pyi
--rw-r--r--   0        0        0      640 2021-07-24 23:28:25.096899 msgpack-types-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 msgpack-types-0.2.0/setup.py
--rw-r--r--   0        0        0     1018 1970-01-01 00:00:00.000000 msgpack-types-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-26 01:52:42.988371 msgpack_types-0.3.0/LICENSE
+-rw-r--r--   0        0        0      475 2024-05-26 01:52:42.988438 msgpack_types-0.3.0/README.md
+-rw-r--r--   0        0        0     2464 2024-05-26 01:52:42.988529 msgpack_types-0.3.0/msgpack-stubs/__init__.pyi
+-rw-r--r--   0        0        0       56 2024-05-26 01:52:42.988579 msgpack_types-0.3.0/msgpack-stubs/_version.pyi
+-rw-r--r--   0        0        0      460 2024-05-26 01:52:42.988633 msgpack_types-0.3.0/msgpack-stubs/exceptions.pyi
+-rw-r--r--   0        0        0      849 2024-05-26 01:52:42.988684 msgpack_types-0.3.0/msgpack-stubs/ext.pyi
+-rw-r--r--   0        0        0     2755 2024-05-26 01:54:30.660804 msgpack_types-0.3.0/msgpack-stubs/fallback.pyi
+-rw-r--r--   0        0        0      640 2024-05-26 01:54:35.392925 msgpack_types-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 msgpack_types-0.3.0/PKG-INFO
```

### Comparing `msgpack-types-0.2.0/LICENSE` & `msgpack_types-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msgpack-types-0.2.0/msgpack-stubs/__init__.pyi` & `msgpack_types-0.3.0/msgpack-stubs/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     read_size: int = ...,
     use_list: bool = ...,
     raw: bool = ...,
     timestamp: int = ...,
     strict_map_key: bool = ...,
     object_hook: Optional[Callable[[Dict[Any, Any]], Any]] = ...,
     object_pairs_hook: Optional[Callable[[List[Tuple[Any, Any]]], Any]] = ...,
-    list_hook: Optional[[Callable[[List[Any]], Any]]] = ...,
+    list_hook: Optional[Callable[[List[Any]], Any]] = ...,
     unicode_errors: Optional[str] = ...,
     max_buffer_size: int = ...,
     ext_hook: Callable[[int, bytes], Any] = ...,
     max_str_len: int = ...,
     max_bin_len: int = ...,
     max_array_len: int = ...,
     max_map_len: int = ...,
```

### Comparing `msgpack-types-0.2.0/msgpack-stubs/ext.pyi` & `msgpack_types-0.3.0/msgpack-stubs/ext.pyi`

 * *Files identical despite different names*

### Comparing `msgpack-types-0.2.0/msgpack-stubs/fallback.pyi` & `msgpack_types-0.3.0/msgpack-stubs/fallback.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     read_size: int = ...,
     use_list: bool = ...,
     raw: bool = ...,
     timestamp: int = ...,
     strict_map_key: bool = ...,
     object_hook: Optional[Callable[[Dict[Any, Any]], Any]] = ...,
     object_pairs_hook: Optional[Callable[[List[Tuple[Any, Any]]], Any]] = ...,
-    list_hook: Optional[[Callable[[List[Any]], Any]]] = ...,
+    list_hook: Optional[Callable[[List[Any]], Any]] = ...,
     unicode_errors: Optional[str] = ...,
     max_buffer_size: int = ...,
     ext_hook: Callable[[int, bytes], Any] = ...,
     max_str_len: int = ...,
     max_bin_len: int = ...,
     max_array_len: int = ...,
     max_map_len: int = ...,
@@ -34,15 +34,15 @@
         read_size: int = ...,
         use_list: bool = ...,
         raw: bool = ...,
         timestamp: int = ...,
         strict_map_key: bool = ...,
         object_hook: Optional[Callable[[Dict[Any, Any]], Any]] = ...,
         object_pairs_hook: Optional[Callable[[List[Tuple[Any, Any]]], Any]] = ...,
-        list_hook: Optional[[Callable[[List[Any]], Any]]] = ...,
+        list_hook: Optional[Callable[[List[Any]], Any]] = ...,
         unicode_errors: Optional[str] = ...,
         max_buffer_size: int = ...,
         ext_hook: Callable[[int, bytes], Any] = ...,
         max_str_len: int = ...,
         max_bin_len: int = ...,
         max_array_len: int = ...,
         max_map_len: int = ...,
@@ -74,8 +74,7 @@
     def pack_map_pairs(self, pairs: Any) -> bytes: ...
     def pack_array_header(self, n: int) -> bytes: ...
     def pack_map_header(self, n: int) -> bytes: ...
     def pack_ext_type(self, typecode: int, data: bytes) -> None: ...
     def bytes(self) -> bytes: ...
     def reset(self) -> None: ...
     def getbuffer(self) -> memoryview: ...
-
```

### Comparing `msgpack-types-0.2.0/pyproject.toml` & `msgpack_types-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msgpack-types"
-version = "0.2.0"
+version = "0.3.0"
 description = "Type stubs for msgpack"
 repository = "https://github.com/sbdchd/msgpack-types"
 readme = "README.md"
 authors = ["Steve Dignam <steve@dignam.xyz>"]
 license = "Apache-2.0"
 keywords = ["msgpack", "types", "mypy", "stubs"]
 packages = [
```

### Comparing `msgpack-types-0.2.0/PKG-INFO` & `msgpack_types-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: msgpack-types
-Version: 0.2.0
+Version: 0.3.0
 Summary: Type stubs for msgpack
 Home-page: https://github.com/sbdchd/msgpack-types
 License: Apache-2.0
 Keywords: msgpack,types,mypy,stubs
 Author: Steve Dignam
 Author-email: steve@dignam.xyz
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/sbdchd/msgpack-types
 Description-Content-Type: text/markdown
 
 # msgpack-types [![PyPI](https://img.shields.io/pypi/v/msgpack-types.svg)](https://pypi.org/project/msgpack-types/)
 
 > Type stubs for [msgpack](https://github.com/msgpack/msgpack-python)
```

