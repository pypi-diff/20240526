# Comparing `tmp/funky_modifiers-0.3.0.tar.gz` & `tmp/funky_modifiers-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.3.0.tar", last modified: Sun May 26 17:10:31 2024, max compression
+gzip compressed data, was "funky_modifiers-0.3.1.tar", last modified: Sun May 26 20:44:41 2024, max compression
```

## Comparing `funky_modifiers-0.3.0.tar` & `funky_modifiers-0.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.823249 funky_modifiers-0.3.0/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      483 2024-05-26 17:10:31.822755 funky_modifiers-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.3.0/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 17:10:31.823249 funky_modifiers-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-05-26 17:08:33.000000 funky_modifiers-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.793985 funky_modifiers-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.798449 funky_modifiers-0.3.0/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.3.0/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.801425 funky_modifiers-0.3.0/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.3.0/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.3.0/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.3.0/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.804897 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.3.0/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.3.0/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.807873 funky_modifiers-0.3.0/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.3.0/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.3.0/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    52352 2024-05-26 17:08:33.000000 funky_modifiers-0.3.0/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.3.0/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.810354 funky_modifiers-0.3.0/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.3.0/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.3.0/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.3.0/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.3.0/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.822257 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      483 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.821266 funky_modifiers-0.3.0/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.3.0/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.3.0/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.3.0/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.3.0/test/test_converters.py
--rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.3.0/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    15923 2024-05-26 17:05:25.000000 funky_modifiers-0.3.0/test/test_dict_builder.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.3.0/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.3.0/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.3.0/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.3.0/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.3.0/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.464642 funky_modifiers-0.3.1/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      483 2024-05-26 20:44:41.464146 funky_modifiers-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.3.1/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 20:44:41.465138 funky_modifiers-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-05-26 20:42:39.000000 funky_modifiers-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.410578 funky_modifiers-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.435379 funky_modifiers-0.3.1/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.3.1/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.439844 funky_modifiers-0.3.1/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.3.1/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.3.1/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.3.1/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.443314 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.3.1/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.3.1/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.446290 funky_modifiers-0.3.1/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.3.1/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.3.1/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    58158 2024-05-26 20:43:05.000000 funky_modifiers-0.3.1/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.3.1/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.449267 funky_modifiers-0.3.1/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.3.1/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.3.1/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.3.1/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.3.1/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.463674 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      483 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.462186 funky_modifiers-0.3.1/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.3.1/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.3.1/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.3.1/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.3.1/test/test_converters.py
+-rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.3.1/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    16939 2024-05-26 20:32:05.000000 funky_modifiers-0.3.1/test/test_dict_builder.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.3.1/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.3.1/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.3.1/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.3.1/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.3.1/test/test_pick.py
```

### Comparing `funky_modifiers-0.3.0/LICENSE` & `funky_modifiers-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/setup.py` & `funky_modifiers-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.3.0',
+    version='0.3.1',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `funky_modifiers-0.3.0/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.3.1/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.3.1/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.3.1/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.3.1/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.3.1/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/modularity/logging.py` & `funky_modifiers-0.3.1/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.3.1/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/sorting/converters.py` & `funky_modifiers-0.3.1/src/funk_py/sorting/converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.3.1/src/funk_py/sorting/dict_manip.py`

 * *Files 6% similar despite different names*

```diff
@@ -523,17 +523,112 @@
         elif key in source:
             return source[key]
 
     return default
 
 
 _NO_MERGE = 'Cannot merge a non-dict to a dict.'
+_METHOD = 'method'
+_ARGS = 'args'
+_KWARGS = 'kwargs'
 
 
 class DictBuilder:
+    """
+    A builder for dictionaries that has a few helpful methods for merging in data from other
+    dictionaries.
+    """
+
+    class _Instruction:
+        def __init__(inner_self, method: str, *args, **kwargs):
+            # Construct the base of a chain.
+            inner_self._chain = [{_METHOD: method, _ARGS: args, _KWARGS: kwargs}]
+
+        def __call__(inner_self, *args, **kwargs) -> 'DictBuilder._Instruction':
+            # Update the last instruction in chain with the received args and kwargs. The user
+            # intends to call a function and did not just want a value.
+            inner_self._chain[-1].update({_ARGS: args, _KWARGS: kwargs})
+            # Return self so that the reference doesn't go away.
+            return inner_self
+
+        def __getattr__(inner_self, item: str) -> 'DictBuilder._Instruction':
+            # Add the new method to the chain, but don't assume the arguments. If there are any,
+            # they will be added by __call__.
+            inner_self._chain.append({_METHOD: item})
+            # Return self so that the reference doesn't go away.
+            return inner_self
+
+        def __getitem__(inner_self, key: str):
+            # Add __getitem__ and args/kawrgs to chain.
+            inner_self._chain.append({_METHOD: '__getitem__', _ARGS: (key,), _KWARGS: {}})
+            # Return self so that the reference doesn't go away.
+            return inner_self
+
+        def list(inner_self) -> 'DictBuilder._Instruction':
+            inner_self._chain.append({_METHOD: lambda x: list(x)})
+            return inner_self
+
+        def tuple(inner_self) -> 'DictBuilder._Instruction':
+            inner_self._chain.append({_METHOD: lambda x: tuple(x)})
+            return inner_self
+
+        def _evaluate(inner_self, parent: 'DictBuilder') -> Any:
+            attr = parent
+            for instruction in inner_self._chain:
+                if type(t := instruction[_METHOD]) is not str:
+                    attr = t(attr)
+
+                else:
+                    attr = getattr(attr, t)
+
+                if _ARGS in instruction:
+                    attr = attr(*[a._evaluate()
+                                  if type(a) in (DictBuilder._Cur, DictBuilder._Instruction)
+                                  else a
+                                  for a in instruction[_ARGS]],
+                                **{k: v._evaluate()
+                                   if v in (DictBuilder._Cur, DictBuilder._Instruction)
+                                   else v
+                                   for k, v in instruction[_KWARGS].items()})
+
+            return attr
+
+    class _Cur:
+        def __getitem__(self, key):
+            return DictBuilder._Instruction('__getitem__', key)
+
+        @staticmethod
+        def get(key: Any, default: Any = None):
+            return DictBuilder._Instruction('get', key, default)
+
+        @staticmethod
+        def keys() -> 'DictManip._Instruction':
+            return DictBuilder._Instruction('keys')
+
+        @staticmethod
+        def values() -> 'DictManip._Instruction':
+            return DictBuilder._Instruction('values')
+
+        @staticmethod
+        def items() -> 'DictManip._Instruction':
+            return DictBuilder._Instruction('items')
+
+        @staticmethod
+        def _evaluate(parent: 'DictBuilder') -> Any:
+            return parent
+
+    #: _Cur: A placeholder that can be used to represent the current ``DictBuilder`` inside its own
+    #: methods and allows the use of a few types of getters including __getitem__, get, keys,
+    #: values, and items' methods.
+    #:
+    #: .. warning::
+    #:     Using this can have unintended consequences and can allow recursion. Use at your own
+    #:     risk.
+    CUR = _Cur() 
+
     def __new__(cls, *args, clazz: Type = dict, **kwargs):
         if clazz is None:
             clazz = dict
 
         inst = super().__new__(cls)
         if issubclass(clazz, dict):
             inst.__class = clazz
@@ -543,17 +638,14 @@
             msg = f'clazz must inherit from dict, but it does not. Provided {clazz}.'
             main_logger.error(msg)
             raise TypeError(msg)
 
     def __init__(self, _map: Mapping = ..., *, clazz: Type = dict, _other: dict = None,
                  _transformer: Callable = pass_, **kwargs):
         """
-        A builder for dictionaries that has a few helpful methods for merging in data from other
-        dictionaries.
-
         :param _map: The ``Mapping`` to start the builder out with. Works like it does for ``dict``.
         :type _map: Mapping
         :param clazz: A dictionary class to inherit from. Used to make sure the builder is the
             desired type of dictionary.
         :type clazz: Type
         :param _other: The *other* dictionary to use for :meth:`~DictBuilder.pull_from_other`,
             :meth:`~DictBuilder.get_from_other`, :meth:`~DictBuilder.update_from_other`,
@@ -627,19 +719,31 @@
             self._check_dict(other)
             self.__other = other
 
         if transformer is not ...:
             self._check_transformer(transformer)
             self.__transformer = transformer
 
-    @staticmethod
-    def _check_dict(other: dict):
-        if not isinstance(other, dict):
+    def _check_dict(self,
+                    other: Union[dict, 'DictBuilder._Cur', 'DictBuilder._Instruction']) -> dict:
+        if type(other) is DictBuilder._Cur:
+            return self.__builder
+
+        elif type(other) is DictBuilder._Instruction:
+            # Evaluate the instruction first to make sure it produces a dictionary.
+            if not isinstance(t := other._evaluate(self), dict):
+                raise TypeError('Invalid type for other.')
+
+            return t
+
+        elif not isinstance(other, dict):
             raise TypeError('Invalid type for other.')
 
+        return other
+
     @staticmethod
     def _check_transformer(transformer: Callable):
         if not callable(transformer):
             raise TypeError('Invalid type for transformer.')
 
     def _choose_transformer(self, transformer: Optional[Callable]):
         if transformer is None:
@@ -658,19 +762,46 @@
             (path := list(_as)).append(val)
 
         else:
             path = _as, val
 
         return path
 
+    def _process_key(self, other: dict,
+                     key: Any,
+                     transformer: Callable,
+                     unsafe: bool,
+                     default: Any = ...) -> Any:
+        if type(key) in (DictBuilder._Cur, DictBuilder._Instruction):
+            key = key._evaluate(self)
+
+        if isinstance(key, list):
+            key = [v._evaluate()
+                   if type(v) in (DictBuilder._Cur, DictBuilder._Instruction)
+                   else v
+                   for v in key]
+            val = get_val_from_path(other, *key, unsafe=unsafe, default=...)
+            if val is ...:
+                return default
+
+            return transformer(val)
+
+        val = other.get(key, ...)
+        if val is ...:
+            return default
+
+        return transformer(val)
+
     @logs_vars(main_logger, start_message='Getting a value from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to get a value from another dictionary.',
                end_message_level='info')
-    def pull_from(self, other: dict, key: Union[Any, list], _as: Union[Any, list],
+    def pull_from(self, other: Union[dict, 'DictBuilder._Cur', 'DictBuilder._Instruction'],
+                  key: Any,
+                  _as: Any,
                   transformer: Callable = None) -> 'DictBuilder':
         """
         Get a value from another dictionary at a given key, and insert it at the key specified in
         ``_as``. Using this will raise an error if the key doesn't exist in ``other`` or if it
         cannot safely be added to the ``DictBuilder``.
 
         :param other: The dictionary to grab the key from.
@@ -679,30 +810,26 @@
         :type key: Union[Any, list]
         :param _as: The key at which to place the found value from ``other``.
         :type _as: Union[Any, list]
         :param transformer: A transformer that should be called on a value if found.
         :type transformer: Callable
         :return: The current ``DictBuilder`` for chaining.
         """
-        self._check_dict(other)
+        other = self._check_dict(other)
         transformer = self._choose_transformer(transformer)
-
-        # Get the value.
-        if isinstance(key, list):
-            val = transformer(get_val_from_path(other, *key, unsafe=True))
-
-        else:
-            val = transformer(other[key])
+        val = self._process_key(other, key, transformer, True)
+        if val is ...:
+            raise ValueError('An invalid value was used.')
 
         path = self._pathify_as(_as, val)
         merge_tuplish_pair(path, self.__builder, unsafe=True)
-
         return self
 
-    def pull_from_other(self, key: Union[Any, list], _as: Union[Any, list],
+    def pull_from_other(self, key: Any,
+                        _as: Any,
                         transformer: Callable = None) -> 'DictBuilder':
         """
         Get a value from the ``DictBuilder's`` ``other`` at a given key, and insert it at the key
         specified in ``_as``. Using this will raise an error if the key doesn't exist in ``other``
         or if it cannot safely be added to the ``DictBuilder``.
 
         :param key: The key at which to find a value in ``other``.
@@ -717,16 +844,19 @@
         self.pull_from(self.__other, key, _as, transformer)
         return self
 
     @logs_vars(main_logger, start_message='Getting a value from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to get a value from another dictionary.',
                end_message_level='info')
-    def get_from(self, other: dict, key: Union[Any, list], _as: Union[Any, list],
-                 transformer: Callable = None, default: Any = ...) -> 'DictBuilder':
+    def get_from(self, other: Union[dict, 'DictBuilder._Cur', 'DictBuilder._Instruction'],
+                 key: Any,
+                 _as: Any,
+                 transformer: Callable = None,
+                 default: Any = ...) -> 'DictBuilder':
         """
         Get a value from another dictionary at a given key, and insert it at the key specified in
         ``_as``. If ``key`` cannot be found in other or ``the value cannot be added to this
         ``DictBuilder``, then the value simply won't be added.
 
         :param other: The dictionary to grab the key from.
         :type other: dict
@@ -736,40 +866,28 @@
         :type _as: Union[Any, list]
         :param transformer: A transformer that should be called on a value if found.
         :type transformer: Callable
         :param default: The default value to use if a value cannot be found. If omitted, and the
             value is not found, then the value simply won't be added.
         :return: The current ``DictBuilder`` for chaining.
         """
-        self._check_dict(other)
+        other = self._check_dict(other)
         transformer = self._choose_transformer(transformer)
-
-        # Get the value.
-        if isinstance(key, list):
-            val = get_val_from_path(other, *key, default=...)
-
-        else:
-            val = other.get(key, ...)
-
+        val = self._process_key(other, key, transformer, False, default)
         if val is ...:
-            if default is ...:
-                return self
-
-            val = default
-
-        else:
-            val = transformer(val)
+            return self
 
         path = self._pathify_as(_as, val)
         merge_tuplish_pair(path, self.__builder)
-
         return self
 
-    def get_from_other(self, key: Union[Any, list], _as: Union[Any, list],
-                       transformer: Callable = None, default: Any = ...) -> 'DictBuilder':
+    def get_from_other(self, key: Any,
+                       _as: Any,
+                       transformer: Callable = None,
+                       default: Any = ...) -> 'DictBuilder':
         """
         Get a value from the ``DictBuilder's`` ``other`` at a given key, and insert it at the key
         specified in ``_as``. If ``key`` cannot be found in ``other`` or the value cannot be added
         to this ``DictBuilder``, then the value simply won't be added.
 
         :param key: The key at which to find a value in ``other``.
         :type key: Union[Any, list]
@@ -786,15 +904,15 @@
         return self
     
     @logs_vars(main_logger, start_message='Updating from a list...',
                start_message_level='info',
                end_message='Finished attempt to update from list.',
                end_message_level='info')
     def update_from_list(self, other: List[dict],
-                          _as: Union[Any, None, list] = None,
+                          _as: Any = None,
                           transformer: Callable = None,
                           unsafe: bool = False,
                           classes: Union[List[Type[dict]], Type[dict]] = None) -> 'DictBuilder':
         """
         Update this ``DictBuilder`` from another dict.
 
         :param other: The dictionary to update with.
@@ -840,30 +958,30 @@
 
         return self
 
     @logs_vars(main_logger, start_message='Updating from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to update from another dictionary.',
                end_message_level='info')
-    def update_from(self, other: dict,
+    def update_from(self, other: Union[dict, 'DictBuilder._Cur', 'DictBuilder._Instruction'],
                     key: Any = None,
-                    _as: Union[Any, None, list] = None,
-                    keys: List[Any] = None,
+                    _as: Any = None,
+                    keys: list = None,
                     transformer: Callable = None,
                     unsafe: bool = False,
                     classes: Union[List[Type[dict]], Type[dict]] = None,
                     val_is_list: bool = False) -> 'DictBuilder':
         """
         Update this ``DictBuilder`` from another dict.
 
         :param other: The dictionary to update with.
         :type other: dict
         :param key: The key at which the source dictionary should be in ``other``. If not specified
             ``other`` will be used as-is unless ``keys`` is specified.
-        :type key: Optional[Union[Any, None, list]]
+        :type key: Union[Any, None, list]
         :param _as: The key at which to place update with the found value from ``other``. If not
             specified, will simply update the entire ``DictBuilder``.
         :type _as: Union[Any, None, list]
         :param keys: A list of possible keys at which the source dictionary might be located in
             ``other``. Each key should follow the same rules as ``key``. If ``key`` is specified,
             ``key`` will be attempted first, then ``keys`` will be attempted.
         :type keys: Optional[List[Union[Any, None, list]]]
@@ -889,15 +1007,15 @@
         :type classes: Optional[Union[List[Type[dict]], Type[dict]]]
         :param val_is_list: Whether the value at ``key`` in ``other`` should be considered as a list
             and its values iterated over and individually used to update the ``DictBuilder``.
             Defaults to ``False``.
         :type val_is_list: bool
         :return: The current ``DictBuilder`` for chaining.
         """
-        self._check_dict(other)
+        other = self._check_dict(other)
         transformer = self._choose_transformer(transformer)
 
         val = self._update_find_in_other(other, key, keys, unsafe)
         if val is ...:
             main_logger.info('Target value could not be located.')
             if unsafe:
                 k = [key]
@@ -999,32 +1117,46 @@
                 # If a dictionary is present instead of a list, use that to update.
                 worker.update(t)
 
             return
 
         worker.update(transformer(val))
 
-    @staticmethod
-    def _update_find_in_other(other: dict, key: Any, keys: List[Any], unsafe: bool = False):
+    def _update_process_key(self, key: Any):
+        if type(key) in (DictBuilder._Cur, DictBuilder._Instruction):
+            return key._evaluate(self)
+
+        if isinstance(key, list):
+            return [v._evaluate()
+                    if type(v) in (DictBuilder._Cur, DictBuilder._Instruction)
+                    else v
+                    for v in key]
+
+        return key
+
+    def _update_find_in_other(self, other: dict, key: Any, keys: List[Any], unsafe: bool = False):
         # Find a key in other, if it exists. Return ... if it doesn't.
         if key is not None:
+            key = self._update_process_key(key)
             if keys is not None:
+                keys = [self._update_process_key(k) for k in keys]
                 # If the user specified both key and keys, that is silly, but handle feeding both
                 # into get_one_of_keys for them. No need to raise an exception.
                 return get_one_of_keys(other, key, *keys, default=...)
 
             elif isinstance(key, list):
                 # Only a key is present and it specifies a path. Follow the path.
                 return get_val_from_path(other, *key, unsafe=unsafe, default=...)
 
             # Simple key is specified.
             return other.get(key, ...)
 
         elif keys is not None:
             # key isn't specified, but keys is. Try to get one of keys.
+            keys = [self._update_process_key(k) for k in keys]
             return get_one_of_keys(other, *keys, default=...)
 
         # If neither keys nor key is specified, assume the user wants the entire dictionary.
         return other
 
     @logs_vars(main_logger, start_message='Attempting to locate target to update...')
     def _update_seek(self, _as: Any,
@@ -1081,16 +1213,16 @@
         return worker
 
     @logs_vars(main_logger, start_message='Getting one of the keys from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to get one of the keys from another dictionary.',
                end_message_level='info')
     def get_one_of_keys_from(self, other: dict,
-                             _as: Union[Any, list],
-                             *keys: Union[Any, list],
+                             _as: Any,
+                             *keys: Any,
                              transformer: Callable = None,
                              default: Any = ...) -> 'DictBuilder':
         """
         Gets the value at one of the keys (or key paths) specified in ``keys`` from ``other`` and
         adds it at ``_as`` within the ``DictBuilder``.
 
         :param other: The source ``dict`` to get the value from.
@@ -1100,16 +1232,17 @@
         :param keys: The possible keys or key paths the sought value could be located at.
         :type keys: Union[Any, list]
         :param default: The default value to return if the target value cannot be found. If this is
             not specified, then should no value be found, a value simply won't be added.
         :type default: Any
         :return: The current ``DictBuilder`` for chaining.
         """
-        self._check_dict(other)
+        other = self._check_dict(other)
         transformer = self._choose_transformer(transformer)
+        keys = [self._update_process_key(k) for k in keys]
 
         val = get_one_of_keys(other, *keys, ...)
         if val is ...:
             if default is ...:
                 return self
 
             val = default
@@ -1135,17 +1268,16 @@
         :type keys: Union[Any, list]
         :param default: The default value to return if the target value cannot be found. If this is
             not specified, then should no value be found, a value simply won't be added.
         :type default: Any
         :return: The current ``DictBuilder`` for chaining.
         """
         self._check_has_other()
-        self.get_one_of_keys_from(self.__other, _as, *keys, transformer=transformer,
-                                  default=default)
-        return self
+        return self.get_one_of_keys_from(self.__other, _as, *keys, transformer=transformer,
+                                         default=default)
 
     @logs_vars(main_logger, start_message='Updating dictionary...', start_message_level='info',
                end_message='Finished updating.', end_message_level='info')
     def update(self, _map: Mapping = ..., **kwargs) -> 'DictBuilder':
         self.__builder.update(_map, **kwargs)
         return self
 
@@ -1159,14 +1291,23 @@
     def get(self, key: Any, default: Any = None):
         return self.__builder.get(key, default)
 
     def __setitem__(self, key, value) -> 'DictBuilder':
         self.__builder[key] = value
         return self
 
+    def keys(self) -> list:
+        return list(self.__builder.keys())
+
+    def values(self) -> list:
+        return list(self.__builder.values())
+
+    def items(self) -> list:
+        return list(self.__builder.items())
+
     def build(self, strict: bool = True) -> dict:
         """
         Build the dictionary from the DictBuilder.
 
         :param strict: Whether to return a strict copy of the dictionary, maintaining all types.
             ``True`` will result all internal dictionaries being maintained as their original types.
             ``False`` will result in all internal dictionaries being converted to ``dict``.
```

### Comparing `funky_modifiers-0.3.0/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.3.1/src/funk_py/sorting/pieces.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.3.1/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.3.1/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.3.1/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.3.1/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.3.1/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_check_dict_equality.py` & `funky_modifiers-0.3.1/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_check_list_equality.py` & `funky_modifiers-0.3.1/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.3.1/test/test_convert_tuplish_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_converters.py` & `funky_modifiers-0.3.1/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_converts_enums.py` & `funky_modifiers-0.3.1/test/test_converts_enums.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_dict_builder.py` & `funky_modifiers-0.3.1/test/test_dict_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import Counter
 from copy import deepcopy
 
 import pytest
 
 from funk_py.modularity.basic_structures import pass_
+from funk_py.modularity.type_matching import check_dict_equality
 from t_support import cov, cov_counter
 from funk_py.sorting.dict_manip import DictBuilder
 
 
 # The following manages whether the generated coverage instance from t_support should report. This
 # method of coverage is used so that coverage can be turned off to not interfere in timed tests.
 @pytest.fixture(scope='session', autouse=True)
@@ -412,15 +413,15 @@
         to_desc(NEW_1ST_2ND_3RD_LVL),
 ))
 def tos(request):
     return request.param
 
 
 @pytest.fixture
-def get_from_other_params(froms, tos, higher_dict1, higher_dict2):
+def get_from_params(froms, tos, higher_dict1, higher_dict2):
     def copies():
         return deepcopy(higher_dict1), deepcopy(higher_dict2)
 
     def to_val_tuple(k1, k2, _from):
         d1, d2 = copies()
         d2[k2] = _from(d1, k1)
         return d2
@@ -485,34 +486,34 @@
 
     k1, _from = froms
     k2, to = tos
     result = to_lookup[to](k1, k2, from_lookup[_from])
     return k1, k2, result
 
 
-def test_get_from(get_from_other_params, higher_dict1, higher_dict2):
+def test_get_from(get_from_params, higher_dict1, higher_dict2):
     testy = DictBuilder(higher_dict2)
-    testy.get_from(higher_dict1, get_from_other_params[0], get_from_other_params[1])
-    assert testy.build() == get_from_other_params[2]
+    testy.get_from(higher_dict1, get_from_params[0], get_from_params[1])
+    assert testy.build() == get_from_params[2]
 
 
 @pytest.fixture(params=(
         ((KB,),(K6,)),
         ((), (K6,)),
         (([K6, K5],), (K7,)),
         ((KB, [K6, K7], K8), ()),
 ), ids=(
         'bad key before, good key after',
         'no key before, good key after',
         'partly-good key before, bad key after',
         'bad keys and partly good key before, no key after',
 ))
-def get_one_key_params(request, get_from_other_params):
+def get_one_key_params(request, get_from_params):
     before, after = request.param
-    return (*before, get_from_other_params[0], *after), *get_from_other_params[1:]
+    return (*before, get_from_params[0], *after), *get_from_params[1:]
 
 
 def test_get_one_key_from(get_one_key_params, higher_dict1, higher_dict2):
     testy = DictBuilder(higher_dict2)
     testy.get_one_of_keys_from(higher_dict1, get_one_key_params[1], *get_one_key_params[0])
     assert testy.build() == get_one_key_params[2]
 
@@ -539,7 +540,32 @@
                             {K8: deepcopy(higher_dict1)}])
     result = {}
     result.update(deepcopy(base_dict1))
     result.update(deepcopy(high_dict1))
     result.update({K8: deepcopy(higher_dict1)})
     assert testy.build() == result, ('Failed for a list with one item in a dictionary with only one'
                                      ' key.')
+
+
+class TestCur:
+    def test_recursive_cur(self, high_dict1):
+        testy = DictBuilder(deepcopy(high_dict1))
+        testy.get_from(DictBuilder.CUR, K4, [K4, K5])
+        result = deepcopy(high_dict1)
+        result[K4][K5] = result[K4]
+        # Special function check_dict_equality can handle comparing two infinitely-recursive
+        # dictionaries.
+        assert check_dict_equality(testy.build(), result)
+
+    def test_value_cur(self, high_dict1):
+        testy = DictBuilder(deepcopy(high_dict1))
+        testy.get_from(DictBuilder.CUR, [K4, K1], K1)
+        result = deepcopy(high_dict1)
+        result[K1] = result[K4][K1]
+        assert testy.build() == result
+
+    def test_key_cur(self, high_dict1, base_dict1):
+        testy = DictBuilder(deepcopy(high_dict1))
+        testy.get_from(base_dict1, DictBuilder.CUR[K4].keys().list()[0], K5)
+        result = deepcopy(high_dict1)
+        result[K5] = high_dict1[K4][K1]
+        assert testy.build() == result
```

### Comparing `funky_modifiers-0.3.0/test/test_drop_none_dict.py` & `funky_modifiers-0.3.1/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_function_hash_and_equality.py` & `funky_modifiers-0.3.1/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_logs_vars.py` & `funky_modifiers-0.3.1/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_obj.py` & `funky_modifiers-0.3.1/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.0/test/test_pick.py` & `funky_modifiers-0.3.1/test/test_pick.py`

 * *Files identical despite different names*

