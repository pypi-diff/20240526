# Comparing `tmp/permacache-3.7.0.tar.gz` & `tmp/permacache-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permacache-3.7.0.tar", last modified: Thu Jun  1 19:55:31 2023, max compression
+gzip compressed data, was "permacache-3.7.1.tar", last modified: Sun May 26 03:41:51 2024, max compression
```

## Comparing `permacache-3.7.0.tar` & `permacache-3.7.1.tar`

### file list

```diff
@@ -1,22 +1,34 @@
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-01 19:55:31.802679 permacache-3.7.0/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3051 2023-06-01 19:55:31.802679 permacache-3.7.0/PKG-INFO
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     2105 2021-12-16 05:53:32.000000 permacache-3.7.0/README.md
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-01 19:55:31.802679 permacache-3.7.0/permacache/
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      247 2023-06-01 19:53:46.000000 permacache-3.7.0/permacache/__init__.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3381 2023-06-01 19:53:46.000000 permacache-3.7.0/permacache/cache.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      871 2023-06-01 19:53:46.000000 permacache-3.7.0/permacache/cache_miss_error.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     1183 2022-01-29 00:35:40.000000 permacache-3.7.0/permacache/dict_function.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3875 2022-04-08 03:07:04.000000 permacache-3.7.0/permacache/hash.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)     3988 2022-12-06 23:50:14.000000 permacache-3.7.0/permacache/locked_shelf.py
--rw-r--r--   0 kavi      (1000) kavi      (1000)     1065 2021-03-14 06:24:57.000000 permacache-3.7.0/permacache/main.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      584 2022-09-20 00:37:01.000000 permacache-3.7.0/permacache/swap_unpickler.py
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      853 2022-01-29 00:38:11.000000 permacache-3.7.0/permacache/utils.py
-drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2023-06-01 19:55:31.802679 permacache-3.7.0/permacache.egg-info/
--rw-r--r--   0 kavi      (1000) kavi      (1000)     3051 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/PKG-INFO
--rw-r--r--   0 kavi      (1000) kavi      (1000)      450 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/SOURCES.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)        1 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/dependency_links.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       53 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/entry_points.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       32 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/requires.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       11 2023-06-01 19:55:31.000000 permacache-3.7.0/permacache.egg-info/top_level.txt
--rw-r--r--   0 kavi      (1000) kavi      (1000)       79 2023-06-01 19:55:31.802679 permacache-3.7.0/setup.cfg
--rw-rw-r--   0 kavi      (1000) kavi      (1000)      838 2023-06-01 19:53:46.000000 permacache-3.7.0/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2024-05-26 03:41:51.549026 permacache-3.7.1/
+-rw-r--r--   0 kavi      (1000) kavi      (1000)    34502 2021-03-14 04:43:47.000000 permacache-3.7.1/LICENSE
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3536 2024-05-26 03:41:51.549026 permacache-3.7.1/PKG-INFO
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2960 2024-05-26 03:40:38.000000 permacache-3.7.1/README.md
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2024-05-26 03:41:51.545026 permacache-3.7.1/permacache/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      247 2024-05-22 23:20:34.000000 permacache-3.7.1/permacache/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     5165 2024-05-26 03:40:38.000000 permacache-3.7.1/permacache/cache.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      956 2024-05-23 00:50:24.000000 permacache-3.7.1/permacache/cache_miss_error.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1234 2024-05-23 00:50:24.000000 permacache-3.7.1/permacache/dict_function.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3767 2024-05-23 00:50:24.000000 permacache-3.7.1/permacache/hash.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     4015 2024-05-23 00:50:24.000000 permacache-3.7.1/permacache/locked_shelf.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1065 2024-05-22 23:20:34.000000 permacache-3.7.1/permacache/main.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3945 2024-05-26 03:40:38.000000 permacache-3.7.1/permacache/out_file_cache.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      617 2024-05-23 00:50:24.000000 permacache-3.7.1/permacache/swap_unpickler.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      853 2022-01-29 00:38:11.000000 permacache-3.7.1/permacache/utils.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2024-05-26 03:41:51.545026 permacache-3.7.1/permacache.egg-info/
+-rw-r--r--   0 kavi      (1000) kavi      (1000)     3536 2024-05-26 03:41:51.000000 permacache-3.7.1/permacache.egg-info/PKG-INFO
+-rw-r--r--   0 kavi      (1000) kavi      (1000)      726 2024-05-26 03:41:51.000000 permacache-3.7.1/permacache.egg-info/SOURCES.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)        1 2024-05-26 03:41:51.000000 permacache-3.7.1/permacache.egg-info/dependency_links.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       52 2024-05-26 03:41:51.000000 permacache-3.7.1/permacache.egg-info/entry_points.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       32 2024-05-26 03:41:51.000000 permacache-3.7.1/permacache.egg-info/requires.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       17 2024-05-26 03:41:51.000000 permacache-3.7.1/permacache.egg-info/top_level.txt
+-rw-r--r--   0 kavi      (1000) kavi      (1000)       79 2024-05-26 03:41:51.549026 permacache-3.7.1/setup.cfg
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      939 2024-05-26 03:41:40.000000 permacache-3.7.1/setup.py
+drwxrwxr-x   0 kavi      (1000) kavi      (1000)        0 2024-05-26 03:41:51.549026 permacache-3.7.1/tests/
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)        0 2024-05-23 00:50:24.000000 permacache-3.7.1/tests/__init__.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     3032 2024-05-26 03:16:13.000000 permacache-3.7.1/tests/dict_function_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1316 2024-05-23 01:03:19.000000 permacache-3.7.1/tests/locked_shelf_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1249 2024-05-23 18:24:57.000000 permacache-3.7.1/tests/parallel_access_locked_shelf_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2722 2024-05-23 18:24:57.000000 permacache-3.7.1/tests/stringify_test.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     1142 2024-05-23 21:48:09.000000 permacache-3.7.1/tests/test_cache.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)      758 2024-05-23 01:03:19.000000 permacache-3.7.1/tests/test_export.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     6749 2024-05-26 03:40:38.000000 permacache-3.7.1/tests/test_out_file_cache.py
+-rw-rw-r--   0 kavi      (1000) kavi      (1000)     2291 2024-05-23 01:04:01.000000 permacache-3.7.1/tests/test_parallel_cache.py
```

### Comparing `permacache-3.7.0/PKG-INFO` & `permacache-3.7.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,79 @@
-Metadata-Version: 2.1
-Name: permacache
-Version: 3.7.0
-Summary: Permanant cache.
-Home-page: https://github.com/kavigupta/permacache
-Author: Kavi Gupta
-Author-email: permacache@kavigupta.org
-License: UNKNOWN
-Description: 
-        # Permacache
-        
-        Add a permanant disk-backed cache for a given function.
-        
-        ## Simple usage
-        
-        ```
-        from permacache import permacache
-        
-        @permacache("unique/path/for/this/function")
-        def f(x):
-            out = x ** 2 # do some fancy compute here
-            return out
-        ```
-        
-        You can simply annotate your function with the permacache annotation as shown above
-        
-        ## Compressing arguments
-        
-        By default, permacache uses a full json stringification of the arguments of your function, with a few special cases given to numpy, torch, and attr classes. If you want to use other classes or only use part of an argument as a key, you can pass in a key_function as such
-        
-        ```
-        from permacache import permacache, stable_hash
-        @permacache(
-            "path",
-            key_function=dict(large_argument=stable_hash, not_json_argument=lambda x: str(x), transient_flag=None)
-        )
-        def f(large_argument, not_json_argument, transient_flag):
-            ...
-        ```
-        
-        The dictionary has keys that correspond to each of the arguments, and the values are applied to them before placing them in the key. Here, `stable_hash` can be used to hash the json stringification of the value, saving disk space but making recovering the value impossible if you want to do that later. Additionally, `str` can be used to stringify objects that you are convinced have stable `str` representations but cannot be represented in json. Finally, the flag argument is ignored in the JSON representation, this is useful for verbosity flags, etc., that don't affect the output.
-        
-        ## Aliasing
-        
-        Permacache uses the underlying function signature to construct the key. For example, for the function
-        
-        ```
-        @permacache("path/f")
-        def f(x, y=2, z=3):
-            pass
-        ```
-        
-        The calls `f(2)`, `f(2, 2, 3)`, `f(2, z=3, y=2)`, and `f(x=2, y=2, z=3)` are all cached using the same key.
-        
-        If you want to add an extra argument, you can keep backwards compatibility using the following code.
-        
-        ```
-        from permacache import drop_if_equal
-        
-        @permacache("path/f", key_function=dict(t=drop_if_equal(0)))
-        def f(x, y=2, z=3, t=0):
-            pass
-        ```
-        
-        In the above code, `t` is dropped from consideration if `t == 0`, allowing us to reuse our old calls.
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+
+# Permacache
+
+Add a permanant disk-backed cache for a given function.
+
+## Simple usage
+
+```
+from permacache import permacache
+
+@permacache("unique/path/for/this/function")
+def f(x):
+    out = x ** 2 # do some fancy compute here
+    return out
+```
+
+You can simply annotate your function with the permacache annotation as shown above
+
+## Compressing arguments
+
+By default, permacache uses a full json stringification of the arguments of your function, with a few special cases given to numpy, torch, and attr classes. If you want to use other classes or only use part of an argument as a key, you can pass in a key_function as such
+
+```
+from permacache import permacache, stable_hash
+@permacache(
+    "path",
+    key_function=dict(large_argument=stable_hash, not_json_argument=lambda x: str(x), transient_flag=None)
+)
+def f(large_argument, not_json_argument, transient_flag):
+    ...
+```
+
+The dictionary has keys that correspond to each of the arguments, and the values are applied to them before placing them in the key. Here, `stable_hash` can be used to hash the json stringification of the value, saving disk space but making recovering the value impossible if you want to do that later. Additionally, `str` can be used to stringify objects that you are convinced have stable `str` representations but cannot be represented in json. Finally, the flag argument is ignored in the JSON representation, this is useful for verbosity flags, etc., that don't affect the output.
+
+## Aliasing
+
+Permacache uses the underlying function signature to construct the key. For example, for the function
+
+```
+@permacache("path/f")
+def f(x, y=2, z=3):
+    pass
+```
+
+The calls `f(2)`, `f(2, 2, 3)`, `f(2, z=3, y=2)`, and `f(x=2, y=2, z=3)` are all cached using the same key.
+
+If you want to add an extra argument, you can keep backwards compatibility using the following code.
+
+```
+from permacache import drop_if_equal
+
+@permacache("path/f", key_function=dict(t=drop_if_equal(0)))
+def f(x, y=2, z=3, t=0):
+    pass
+```
+
+In the above code, `t` is dropped from consideration if `t == 0`, allowing us to reuse our old calls.
+
+## Out Files
+
+You can specify one or more input parameters to be the "out files" of the function. These are files
+    that the function creates and writes to. If the function is called with the same arguments except
+    for these paths, the function will not be recomputed, so long as some path still exists that was
+    written to by this function historically. This is useful for functions whose output is writing
+    to a file rather than returning a value. The function can also have a return value, which is
+    cached normally.
+
+You are responsible for ensuring that the output parameter is not used in the body of the function
+    except for writing to it.
+
+This feature is not supported on Windows.
+
+```python
+@permacache("path/f", out_file=["loc"])
+def f(x, loc):
+    with open(loc, "w") as f:
+        f.write(str(x) * 10000)
+    return [x]
+```
```

### Comparing `permacache-3.7.0/README.md` & `permacache-3.7.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: permacache
+Version: 3.7.1
+Summary: Permanant cache.
+Home-page: https://github.com/kavigupta/permacache
+Author: Kavi Gupta
+Author-email: permacache@kavigupta.org
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # Permacache
 
 Add a permanant disk-backed cache for a given function.
 
 ## Simple usage
 
@@ -50,8 +67,30 @@
 from permacache import drop_if_equal
 
 @permacache("path/f", key_function=dict(t=drop_if_equal(0)))
 def f(x, y=2, z=3, t=0):
     pass
 ```
 
-In the above code, `t` is dropped from consideration if `t == 0`, allowing us to reuse our old calls.
+In the above code, `t` is dropped from consideration if `t == 0`, allowing us to reuse our old calls.
+
+## Out Files
+
+You can specify one or more input parameters to be the "out files" of the function. These are files
+    that the function creates and writes to. If the function is called with the same arguments except
+    for these paths, the function will not be recomputed, so long as some path still exists that was
+    written to by this function historically. This is useful for functions whose output is writing
+    to a file rather than returning a value. The function can also have a return value, which is
+    cached normally.
+
+You are responsible for ensuring that the output parameter is not used in the body of the function
+    except for writing to it.
+
+This feature is not supported on Windows.
+
+```python
+@permacache("path/f", out_file=["loc"])
+def f(x, loc):
+    with open(loc, "w") as f:
+        f.write(str(x) * 10000)
+    return [x]
+```
```

### Comparing `permacache-3.7.0/permacache/cache_miss_error.py` & `permacache-3.7.1/permacache/cache_miss_error.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,13 +23,17 @@
     """
     context manager that sets the error on miss attribute globally, and the
     resets it when the context is exited
     """
 
     error_on_miss = False
 
+    def __init__(self):
+        self.old = None
+
     def __enter__(self):
         self.old = error_on_miss_global.error_on_miss
         error_on_miss_global.error_on_miss = True
 
     def __exit__(self, *args):
+        assert self.old is not None
         error_on_miss_global.error_on_miss = self.old
```

### Comparing `permacache-3.7.0/permacache/dict_function.py` & `permacache-3.7.1/permacache/dict_function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import attr
+from dataclasses import dataclass
+from typing import List
 
-from .utils import parallelize_arguments, bind_arguments
+from .utils import bind_arguments, parallelize_arguments
 
 DEFAULT_FUNCTIONS = {None: lambda x: None}
 
 
 class drop_if:
     def __init__(self, predicate, mapper=lambda x: x):
         self.predicate = predicate
         self.mapper = mapper
 
 
-@attr.s
+@dataclass
 class parallel_output:
-    values = attr.ib()
+    values: List[object]
 
 
 def drop_if_equal(value, mapper=lambda x: x):
     return drop_if(lambda x: x == value, mapper)
 
 
 def dict_function(d, fn):
```

### Comparing `permacache-3.7.0/permacache/hash.py` & `permacache-3.7.1/permacache/hash.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,75 @@
-import json
+import enum
 import hashlib
-from types import SimpleNamespace
+import json
 import numbers
-
-import enum
+from types import SimpleNamespace
 
 
 class TensorEncoder(json.JSONEncoder):
     fast_bytes = False
 
-    def default(self, obj):
-        original = obj
-        if hasattr(type(obj), "__permacache_hash__"):
-            obj = {".custom": True, "content": type(obj).__permacache_hash__(obj)}
-        if hasattr(obj, "__attrs_attrs__"):
-            typename = type(obj).__name__
-            obj = {a.name: getattr(obj, a.name) for a in obj.__attrs_attrs__}
-            obj[".attr.__name__"] = typename
-        if isinstance(obj, SimpleNamespace):
-            obj = obj.__dict__
-            obj[".builtin.__name__"] = "types.SimpleNamespace"
+    def default(self, o):
+        original = o
+        if hasattr(type(o), "__permacache_hash__"):
+            o = {".custom": True, "content": type(o).__permacache_hash__(o)}
+        if hasattr(o, "__attrs_attrs__"):
+            typename = type(o).__name__
+            o = {a.name: getattr(o, a.name) for a in o.__attrs_attrs__}
+            o[".attr.__name__"] = typename
+        if isinstance(o, SimpleNamespace):
+            o = o.__dict__
+            o[".builtin.__name__"] = "types.SimpleNamespace"
         if (
-            type(obj).__module__ == "torch.nn.parameter"
-            and type(obj).__name__ == "Parameter"
+            type(o).__module__ == "torch.nn.parameter"
+            and type(o).__name__ == "Parameter"
         ):
-            obj = obj.data
-        obj = best_effort_to_bytes(obj)
-        if isinstance(obj, bytes):
+            o = o.data
+        o = best_effort_to_bytes(o)
+        if isinstance(o, bytes):
             if self.fast_bytes:
-                obj = hashlib.sha256(obj).hexdigest()
+                o = hashlib.sha256(o).hexdigest()
             else:
-                obj = str(obj)
-        if isinstance(obj, range):
-            obj = {".type": "range", "representation": str(obj)}
-        if isinstance(obj, type):
-            obj = {".type": "type", "name": obj.__module__ + "." + obj.__qualname__}
-        if self.isinstance_str(obj, "Module"):
-            obj = {
+                o = str(o)
+        if isinstance(o, range):
+            o = {".type": "range", "representation": str(o)}
+        if isinstance(o, type):
+            o = {".type": "type", "name": o.__module__ + "." + o.__qualname__}
+        if self.isinstance_str(o, "Module"):
+            o = {
                 ".type": "Module",
                 "hash": dict(
                     other_dict={
-                        k: v for k, v in obj.__dict__.items() if not k.startswith("_")
+                        k: v for k, v in o.__dict__.items() if not k.startswith("_")
                     },
-                    state_dict=obj.state_dict(),
+                    state_dict=o.state_dict(),
                 ),
             }
-        if self.isinstance_str(obj, "DataFrame"):
+        if self.isinstance_str(o, "DataFrame"):
             return {
                 ".type": "pandas.DataFrame",
-                "columns": list(obj),
-                "values": {k: obj[k] for k in obj},
+                "columns": list(o),
+                "values": {k: o[k] for k in o},
             }
-        if self.isinstance_str(obj, "Series"):
+        if self.isinstance_str(o, "Series"):
             return {
                 ".type": "pandas.Series",
-                "index": list(obj.index),
-                "values": list(obj),
+                "index": list(o.index),
+                "values": list(o),
             }
-        if isinstance(obj, enum.Enum):
+        if isinstance(o, enum.Enum):
             return {
                 ".type": "enum",
-                "enum.name": type(obj).__name__,
-                "enum.value": obj.value,
+                "enum.name": type(o).__name__,
+                "enum.value": o.value,
             }
-        obj = fix_dictionary(obj)
-        if obj is original:
-            return super().default(obj)
-        return obj
+        o = fix_dictionary(o)
+        if o is original:
+            return super().default(o)
+        return o
 
     def isinstance_str(self, obj, str_type):
         try:
             return any(x.__name__ == str_type for x in type(obj).mro())
         except TypeError:
             return False
 
@@ -101,15 +100,15 @@
         if obj.is_cuda:
             obj = obj.cpu()
         obj = obj.detach().numpy()
     if type(obj).__module__ == "numpy":
         if type(obj).__name__ == "dtype":
             obj = str(obj).encode("utf-8")
         else:
-            obj = obj.tostring()
+            obj = obj.tobytes()
     return obj
 
 
 def stringify(obj, *, fast_bytes=False):
     return json.dumps(
         fix_dictionary(obj),
         cls=FastTensorEncoder if fast_bytes else TensorEncoder,
```

### Comparing `permacache-3.7.0/permacache/locked_shelf.py` & `permacache-3.7.1/permacache/locked_shelf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import os
-
-from filelock import FileLock
 import shelve
 import time
 
+from filelock import FileLock
+
 
 class Lock:
     def __init__(self, lock_path, time_path):
         self.lock = FileLock(lock_path)
         self.time_path = time_path
         self.last_opened = float("-inf")
         self.unlocked = False
 
     def _get_last_modified(self):
         self._check()
         try:
             with open(self.time_path) as f:
                 return float(f.read())
-        except:
+        # pylint: disable=broad-except
+        except Exception:
             self.set_last_modified()
             return self._get_last_modified()
 
     def opened_after_last_modification(self):
         self._check()
         last_modified_time = self._get_last_modified()
         return self.last_opened >= last_modified_time
@@ -82,17 +83,16 @@
             if not self.lock.opened_after_last_modification():
                 self.cache = {}
                 self.lock.set_last_opened()
 
     def _read_from_underlying_shelf(self, key):
         if self.read_from_shelf_context_manager is None:
             return self.shelf[key]
-        else:
-            with self.read_from_shelf_context_manager:
-                return self.shelf[key]
+        with self.read_from_shelf_context_manager:
+            return self.shelf[key]
 
     def __getitem__(self, key):
         self._update()
 
         if key not in self.cache:
             result = self.cache[key] = self._read_from_underlying_shelf(key)
             return result
```

### Comparing `permacache-3.7.0/permacache/main.py` & `permacache-3.7.1/permacache/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 
-from .cache import to_file, from_file
+from .cache import from_file, to_file
 
 
 def cache_args(parser):
     parser.add_argument("cache_name", help="The name of the cache to export")
     parser.add_argument("zip_path", help="The path to export the zip path to")
```

### Comparing `permacache-3.7.0/permacache/swap_unpickler.py` & `permacache-3.7.1/permacache/swap_unpickler.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,13 +7,14 @@
         self._unpickler_class = unpickler_class
         self._previous_unpickler = None
 
     def __enter__(self):
         self._previous_unpickler = shelve.Unpickler
         shelve.Unpickler = self._unpickler_class
 
-    def __exit__(self, type, value, traceback):
+    def __exit__(self, typ, value, traceback):
+        del typ, value, traceback
         if self._previous_unpickler is not None:
             shelve.Unpickler = self._previous_unpickler
             self._previous_unpickler = None
         else:
             shelve.Unpickler = pickle.Unpickler
```

### Comparing `permacache-3.7.0/permacache/utils.py` & `permacache-3.7.1/permacache/utils.py`

 * *Files identical despite different names*

### Comparing `permacache-3.7.0/setup.py` & `permacache-3.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="permacache",
-    version="3.7.0",
+    version="3.7.1",
     author="Kavi Gupta",
     author_email="permacache@kavigupta.org",
     description="Permanant cache.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kavigupta/permacache",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=["filelock>=3.0.12", "appdirs>=1.4.4"],
     entry_points={
         "console_scripts": ["permacache=permacache.main:main"],
     },
```

