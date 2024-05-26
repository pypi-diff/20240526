# Comparing `tmp/funky_modifiers-0.2.0.tar.gz` & `tmp/funky_modifiers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.2.0.tar", last modified: Sun May 19 19:50:40 2024, max compression
+gzip compressed data, was "funky_modifiers-0.2.2.tar", last modified: Sun May 26 13:17:45 2024, max compression
```

## Comparing `funky_modifiers-0.2.0.tar` & `funky_modifiers-0.2.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.080443 funky_modifiers-0.2.0/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      474 2024-05-19 19:50:40.079945 funky_modifiers-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.2.0/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 19:50:40.080443 funky_modifiers-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      711 2024-05-19 19:48:14.000000 funky_modifiers-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.043739 funky_modifiers-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.049193 funky_modifiers-0.2.0/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.2.0/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.053659 funky_modifiers-0.2.0/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.2.0/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.2.0/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.2.0/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.057131 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.2.0/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.2.0/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.060602 funky_modifiers-0.2.0/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.2.0/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20021 2024-05-05 16:10:17.000000 funky_modifiers-0.2.0/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    32960 2024-05-19 13:15:49.000000 funky_modifiers-0.2.0/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.2.0/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.063578 funky_modifiers-0.2.0/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.2.0/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.2.0/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.2.0/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.2.0/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.078954 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.078461 funky_modifiers-0.2.0/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.2.0/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.2.0/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.2.0/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.2.0/test/test_converters.py
--rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.2.0/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    10746 2024-05-19 13:19:52.000000 funky_modifiers-0.2.0/test/test_dict_builder.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.2.0/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.2.0/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.2.0/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.2.0/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.2.0/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.272052 funky_modifiers-0.2.2/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      483 2024-05-26 13:17:45.271556 funky_modifiers-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.2.2/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 13:17:45.272052 funky_modifiers-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-05-26 13:17:23.000000 funky_modifiers-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.240309 funky_modifiers-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.244772 funky_modifiers-0.2.2/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.2.2/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.248741 funky_modifiers-0.2.2/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.2.2/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.2.2/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.2.2/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.251221 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.2.2/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.2.2/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.254197 funky_modifiers-0.2.2/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.2.2/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.2.2/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    36675 2024-05-26 13:12:47.000000 funky_modifiers-0.2.2/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.2.2/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.257670 funky_modifiers-0.2.2/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.2.2/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.2.2/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.2.2/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.2.2/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.271060 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      483 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.270069 funky_modifiers-0.2.2/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.2.2/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.2.2/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.2.2/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.2.2/test/test_converters.py
+-rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.2.2/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    13608 2024-05-26 13:08:42.000000 funky_modifiers-0.2.2/test/test_dict_builder.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.2.2/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.2.2/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.2.2/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.2.2/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.2.2/test/test_pick.py
```

### Comparing `funky_modifiers-0.2.0/LICENSE` & `funky_modifiers-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/setup.py` & `funky_modifiers-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.2.0',
+    version='0.2.2',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
-        'Development Status :: 1 - Planning',
+        'Development Status :: 5 - Production/Stable',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3.7'
     ],
     python_requires='>3.6',
     install_requires=install_requires
 )
```

### Comparing `funky_modifiers-0.2.0/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.2.2/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.2.2/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.2.2/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.2.2/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.2.2/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/modularity/logging.py` & `funky_modifiers-0.2.2/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.2.2/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/sorting/converters.py` & `funky_modifiers-0.2.2/src/funk_py/sorting/converters.py`

 * *Files 8% similar despite different names*

```diff
@@ -579,7 +579,28 @@
     """
     return [json.loads(p) for p in data.split('\n')]
 
 
 def json_to_jsonl(data: List[Union[list, dict]]) -> str:
     return '\n'.join(json.dumps(line) for line in data)
 
+
+def list_to_string_list(data: list) -> str:
+    """
+    Generates a string representation of a list in proper sentence form. Uses the Oxford comma.
+
+    :param data: The list to convert.
+    :type data: list
+    :return: A string containing the list converted to proper sentence form.
+    """
+    if (t := len(data)) == 0:
+        return ''
+
+    elif t == 1:
+        return str(data[0])
+
+    elif t == 2:
+        return f'{data[0]} and {data[1]}'
+
+    else:
+        return ', '.join(str(d) for d in data[:-1]) + f', and {data[-1]}'
+
```

### Comparing `funky_modifiers-0.2.0/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.2.2/src/funk_py/sorting/dict_manip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from copy import deepcopy
-from typing import Generator, Optional, Union, Any, Callable, Dict, Tuple, Iterable, Mapping, Type
+from typing import (Generator, Optional, Union, Any, Callable, Dict, Tuple, Iterable, Mapping,
+                    Type, List)
 
 from funk_py.modularity.basic_structures import pass_
 from funk_py.modularity.logging import make_logger, logs_vars
 
 main_logger = make_logger('dict_manip', env_var='DICT_MANIP_LOG_LEVEL', default_level='warning')
 
 
@@ -476,15 +477,17 @@
         ``default``.
     """
     for key in path:
         if key in source:
             source = source[key]
 
         elif unsafe:
-            raise KeyError(f'Path failed at {key}.')
+            msg = f'Path failed at {key}'
+            main_logger.error(msg)
+            raise KeyError(msg)
 
         else:
             return default
 
     return source
 
 
@@ -521,40 +524,54 @@
             return source[key]
 
     return default
 
 
 class DictBuilder:
     def __new__(cls, *args, clazz: Type = dict, **kwargs):
+        if clazz is None:
+            clazz = dict
+
         inst = super().__new__(cls)
-        inst.__class = clazz
-        return inst
+        if issubclass(clazz, dict):
+            inst.__class = clazz
+            return inst
+
+        else:
+            msg = f'clazz must inherit from dict, but it does not. Provided {clazz}.'
+            main_logger.error(msg)
+            raise TypeError(msg)
 
     def __init__(self, _map: Mapping = ..., *, clazz: Type = dict, **kwargs):
         """
         A builder for dictionaries that has a few helpful methods for merging in data from other
         dictionaries.
 
         :param _map: The ``Mapping`` to start the builder out with. Works like it does for ``dict``.
         :type _map: Mapping
-        :param clazz: A ``dictionary class to inherit from. Used to make sure the builder is the
+        :param clazz: A dictionary class to inherit from. Used to make sure the builder is the
             desired type of dictionary.
         :type clazz: Type
         :param kwargs: The ``kwargs`` to construct the starting builder with. Works like it does for
             ``dict``.
         """
         if 'clazz' in kwargs:
             del kwargs['clazz']
 
         if _map is ...:
             self.__builder = self.__class(**kwargs)
 
         else:
             self.__builder = self.__class(_map, **kwargs)
 
+    @property
+    def clazz(self) -> type:
+        """The default class for the ``DictBuilder``."""
+        return self.__class
+
     @staticmethod
     def _check_dict(other: dict):
         if not isinstance(other, dict):
             raise TypeError('Invalid type for other.')
 
     @staticmethod
     def _pathify_as(_as: Union[Any, list], val: Any):
@@ -647,17 +664,20 @@
 
         return self
 
     @logs_vars(main_logger, start_message='Updating from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to update from another dictionary.',
                end_message_level='info')
-    def update_from_other(self, other: dict, key: Union[Any, None, list] = None,
-                          _as: Union[Any, None, list] = None, transformer: Callable = pass_,
-                          unsafe: bool = False) -> 'DictBuilder':
+    def update_from_other(self, other: dict,
+                          key: Union[Any, None, list] = None,
+                          _as: Union[Any, None, list] = None,
+                          transformer: Callable = pass_,
+                          unsafe: bool = False,
+                          classes: Union[List[Type[dict]], Type[dict]] = None) -> 'DictBuilder':
         """
         Update this ``DictBuilder`` from another dict.
 
         :param other: The dictionary to update with.
         :type other: dict
         :param key: The key at which the source dictionary should be in ``other``. If not specified
             ``other`` will be used as-is.
@@ -667,14 +687,28 @@
         :type _as: Union[Any, None, list]
         :param transformer: A transformer that should be called on the value being used to update
             the ``DictBuilder``.
         :type transformer: Callable
         :param unsafe: Whether an error should be raised if the desired operation cannot be
             completed.
         :type unsafe: bool
+        :param classes: The types of internal dictionaries to generate if parts of paths do not
+            exist. Will override what type of dictionary is used at each point in the path until
+            the end of ``_as``. There are different behaviors based on how this is specified (or not
+            specified).
+
+            - If this is a ``list``, each class will be used in succession while following the path
+              specified by ``_as``. If the end is reached before ``_as`` is over, new dictionaries
+              will be of the same type as the ``DictBuilder.clazz``. If this longer than ``_as``, it
+              will only be used for needed locations.
+            - If this is a single type, any new dicts generated when following the path described by
+              ``_as`` will be of the type specified.
+            - If this is not specified, each generated dictionary will be of the same type as the
+              ``DictBuilder.clazz``.
+        :type classes: Optional[Union[List[Type[dict]], Type[dict]]]
         :return: The current ``DictBuilder`` for chaining.
         """
         self._check_dict(other)
         # Get the value.
         if key is not None:
             if isinstance(key, list):
                 val = get_val_from_path(other, *key, unsafe=unsafe, default=...)
@@ -685,56 +719,82 @@
             else:
                 val = other.get(key, ...)
 
         else:
             val = other
 
         if val is ...:
+            main_logger.info('Target value could not be located.')
             return self
 
         if not isinstance(val, dict):
             if unsafe:
                 msg = 'Cannot merge a dict to a value.'
                 main_logger.error(msg)
                 raise ValueError(msg)
 
             return self
 
         worker = self.__builder
-        worker = self._update_seek(_as, worker, unsafe)
+        worker = self._update_seek(_as, worker, unsafe, classes)
         worker.update(transformer(val))
 
         return self
 
-    def _update_seek(self, _as: Any, worker: dict, unsafe: bool):
+    @logs_vars(main_logger, start_message='Attempting to locate target to update...')
+    def _update_seek(self, _as: Any,
+                     worker: dict,
+                     unsafe: bool,
+                     classes: Union[None, List[Type[dict]], Type[dict]]):
         if _as is not None:
+            needed = len(_as)
+            if type(classes) is list:
+                if (t := len(classes) - needed) < 0:
+                    classes += [self.__class] * -t
+
+            elif classes is None:
+                classes = [self.__class] * needed
+
+            else:
+                classes = [classes] * needed
+
+            for t in classes:
+                if not issubclass(t, dict):
+                    msg = (f'All used classes must inherit from dict, but it does not. Provided'
+                           f'{classes}.')
+                    main_logger.error(msg)
+                    raise TypeError(msg)
+
+            clazz = iter(classes)
             if isinstance(_as, list):
                 for val in _as:
-                    worker = self._update_seek_next(val, worker, unsafe)
+                    worker = self._update_seek_next(val, worker, unsafe, next(clazz))
 
             else:
-                worker = self._update_seek_next(_as, worker, unsafe)
+                worker = self._update_seek_next(_as, worker, unsafe, next(clazz))
 
+        main_logger.debug(f'Found the target worker. Value is {worker}.')
         return worker
 
-    def _update_seek_next(self, val: Any, worker: dict, unsafe: bool):
+    @staticmethod
+    def _update_seek_next(val: Any, worker: dict, unsafe: bool, clazz: Type[dict]):
         if val in worker:
             if isinstance(worker[val], dict):
                 worker = worker[val]
 
             elif unsafe:
-                msg = 'An invalid path was encountered'
-                main_logger.error(msg + ' while updating from another dictionary.')
-                raise ValueError(msg + '.')
+                msg = 'An invalid path was encountered while updating from another dictionary.'
+                main_logger.error(msg)
+                raise ValueError(msg)
 
             else:
-                worker[val] = worker = self.clazz()
+                worker[val] = worker = clazz()
 
         else:
-            worker[val] = worker = self.clazz()
+            worker[val] = worker = clazz()
 
         return worker
 
     @logs_vars(main_logger, start_message='Getting one of the keys from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to get one of the keys from another dictionary.',
                end_message_level='info')
@@ -787,9 +847,38 @@
     def get(self, key: Any, default: Any = None):
         return self.__builder.get(key, default)
 
     def __setitem__(self, key, value) -> 'DictBuilder':
         self.__builder[key] = value
         return self
 
-    def build(self) -> dict:
-        return deepcopy(self.__builder)
+    def build(self, strict: bool = True) -> dict:
+        """
+        Build the dictionary from the DictBuilder.
+
+        :param strict: Whether to return a strict copy of the dictionary, maintaining all types.
+            ``True`` will result all internal dictionaries being maintained as their original types.
+            ``False`` will result in all internal dictionaries being converted to ``dict``.
+        :type strict: bool
+        :return: The dictionary that was built.
+        """
+        result = deepcopy(self.__builder)
+        if strict:
+            return result
+
+        return self._convert_all_to_dicts(result)
+
+    def _convert_all_to_dicts(self, source: dict) -> dict:
+        if type(source) is dict:
+            worker = source
+
+        else:
+            worker = dict(source)
+
+        for key, val in source.items():
+            if isinstance(val, dict):
+                worker[key] = self._convert_all_to_dicts(val)
+
+            else:
+                worker[key] = val
+
+        return worker
```

### Comparing `funky_modifiers-0.2.0/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.2.2/src/funk_py/sorting/pieces.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.2.2/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.2.2/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.2.2/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.2.2/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.2.2/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_check_dict_equality.py` & `funky_modifiers-0.2.2/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_check_list_equality.py` & `funky_modifiers-0.2.2/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.2.2/test/test_convert_tuplish_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_converters.py` & `funky_modifiers-0.2.2/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_converts_enums.py` & `funky_modifiers-0.2.2/test/test_converts_enums.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_dict_builder.py` & `funky_modifiers-0.2.2/test/test_dict_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import Counter
 from copy import deepcopy
 
 import pytest
 
 from t_support import cov, cov_counter
 from funk_py.sorting.dict_manip import DictBuilder
 
@@ -101,65 +102,97 @@
 
 
 @pytest.fixture
 def higher_dict2():
     return {K7: V7, K8: {K5: V5, K6: {K3: V3, K4: V4}}}
 
 
-def instantiate(_map, kwargs) -> DictBuilder:
+@pytest.fixture(params=(None, Counter), ids=('normal', 'specified class at init'))
+def type_spec(request):
+    return request.param
+
+
+def instantiate(_map, kwargs, clazz=None) -> DictBuilder:
     if _map is ...:
-        return DictBuilder(**kwargs)
+        if clazz is None:
+            return DictBuilder(**kwargs)
+
+        return DictBuilder(**kwargs, clazz=clazz)
+
+    elif clazz is None:
+        return DictBuilder(_map, **kwargs)
 
-    return DictBuilder(_map, **kwargs)
+    return DictBuilder(_map, **kwargs, clazz=clazz)
 
 
-def test_can_instantiate(instantiation_pattern):
-    testy = instantiate(*instantiation_pattern[:2])
+def test_can_instantiate(instantiation_pattern, type_spec):
+    testy = instantiate(*instantiation_pattern[:2], type_spec)
+    if type_spec is not None:
+        assert testy.clazz is type_spec
+        # Don't test build inside the instantiation test.
 
 
-def test_can_setitem(instantiation_pattern):
-    testy = instantiate(*instantiation_pattern[:2])
+def test_can_build(instantiation_pattern, type_spec):
+    testy = instantiate(*instantiation_pattern[:2], type_spec)
+    if type_spec is not None:
+        assert type(testy.build()) is type_spec
+
+
+def test_can_setitem(instantiation_pattern, type_spec):
+    testy = instantiate(*instantiation_pattern[:2], type_spec)
     testy[T_KEY] = T_VAL
     result = instantiation_pattern[2]
     result[T_KEY] = T_VAL
 
     assert testy.build() == result
+    if type_spec is not None:
+        assert testy.clazz is type_spec
 
 
-def test_can_getitem(base_dict1):
-    testy = DictBuilder(base_dict1)
+def test_can_getitem(base_dict1, type_spec):
+    testy = DictBuilder(base_dict1, clazz=type_spec)
     assert testy[K1] == V1
     assert testy[K2] == V2
+    if type_spec is not None:
+        assert testy.clazz is type_spec
 
 
-def test_can_get(base_dict1):
-    testy = DictBuilder(base_dict1)
+def test_can_get(base_dict1, type_spec):
+    testy = DictBuilder(base_dict1, clazz=type_spec)
     assert testy.get(K1) == V1
     assert testy.get(K2) == V2
+    if type_spec is not None:
+        assert testy.clazz is type_spec
 
 
-def test_can_get_missing(base_dict1):
-    testy = DictBuilder(base_dict1)
+def test_can_get_missing(base_dict1, type_spec):
+    testy = DictBuilder(base_dict1, clazz=type_spec)
     assert testy.get(KB) is None
+    if type_spec is not None:
+        assert testy.clazz is type_spec
 
 
-def test_can_update(instantiation_pattern, base_dict1):
-    testy = instantiate(*instantiation_pattern[:2])
+def test_can_update(instantiation_pattern, base_dict1, type_spec):
+    testy = instantiate(*instantiation_pattern[:2], type_spec)
     testy.update(base_dict1)
     result = instantiation_pattern[2]
     result.update(base_dict1)
     assert testy.build() == result
+    if type_spec is not None:
+        assert testy.clazz is type_spec
 
 
-def test_can_update_from_other(instantiation_pattern, base_dict1):
-    testy = instantiate(*instantiation_pattern[:2])
+def test_can_update_from_other(instantiation_pattern, base_dict1, type_spec):
+    testy = instantiate(*instantiation_pattern[:2], type_spec)
     testy.update_from_other(base_dict1)
     result = instantiation_pattern[2]
     result.update(base_dict1)
     assert testy.build() == result
+    if type_spec is not None:
+        assert testy.clazz is type_spec
 
 
 def test_nested_can_update_from_nested_other(higher_dict1, higher_dict2):
     testy = DictBuilder(deepcopy(higher_dict2))
     testy.update_from_other(deepcopy(higher_dict1))
     result = deepcopy(higher_dict2)
     result.update(deepcopy(higher_dict1))
@@ -210,14 +243,55 @@
     testy = DictBuilder(deepcopy(higher_dict2))
     testy.update_from_other(deepcopy(higher_dict1), [K6, K4], [K8, K6])
     result = deepcopy(higher_dict2)
     result[K8][K6].update(deepcopy(higher_dict1[K6][K4]))
     assert testy.build() == result
 
 
+def test_update_from_other_with_classes_generates_correct(base_dict1, base_dict2):
+    testy = DictBuilder(deepcopy(base_dict2))
+    testy.update_from_other(deepcopy(base_dict1), _as=K5, classes=Counter)
+    result = deepcopy(base_dict2)
+    result[K5] = base_dict1
+    built = testy.build()
+    assert built == result
+    assert type(built) is dict
+    assert type(built[K5]) is Counter
+
+
+def test_update_from_other_with_classes_behaves_expected(base_dict1, base_dict2):
+    testy = DictBuilder(deepcopy(base_dict2))
+    testy.update_from_other(deepcopy(base_dict1), _as=K5, classes=Counter)
+    testy.update_from_other(deepcopy(base_dict1), _as=K5)
+
+    expectation = Counter(base_dict1)
+    expectation.update(base_dict1)
+    _known_result = {k: 2*v for k, v in base_dict1.items()}
+    assert _known_result == expectation, ('The behavior of Counter seems to have changed. '
+                                          'This test is no longer valid.')
+
+    result = deepcopy(base_dict2)
+    result[K5] = expectation
+    built = testy.build()
+    assert built == result
+    assert type(built) is dict
+    assert type(built[K5]) is Counter
+
+
+def test_update_from_other_with_classes_can_be_made_dict(base_dict1, base_dict2):
+    testy = DictBuilder(deepcopy(base_dict2))
+    testy.update_from_other(deepcopy(base_dict1), _as=K5, classes=Counter)
+    result = deepcopy(base_dict2)
+    result[K5] = base_dict1
+    built = testy.build(False)
+    assert built == result
+    assert type(built) is dict
+    assert type(built[K5]) is dict
+
+
 TOP_LVL = 'top level'
 TOP_LVL_LST = 'top level (list)'
 NEW_TOP_LVL = 'new top level'
 NEW_TOP_LVL_LST = 'new top level (list)'
 NEW_1ST_2ND_LVL = 'new first and second level'
 NEW_2ND_LVL = 'new second level'
 SCND_LVL = 'second level'
```

### Comparing `funky_modifiers-0.2.0/test/test_drop_none_dict.py` & `funky_modifiers-0.2.2/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_function_hash_and_equality.py` & `funky_modifiers-0.2.2/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_logs_vars.py` & `funky_modifiers-0.2.2/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_obj.py` & `funky_modifiers-0.2.2/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.0/test/test_pick.py` & `funky_modifiers-0.2.2/test/test_pick.py`

 * *Files identical despite different names*

