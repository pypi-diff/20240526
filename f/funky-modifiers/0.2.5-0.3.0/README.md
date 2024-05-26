# Comparing `tmp/funky_modifiers-0.2.5.tar.gz` & `tmp/funky_modifiers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.2.5.tar", last modified: Sun May 26 14:49:49 2024, max compression
+gzip compressed data, was "funky_modifiers-0.3.0.tar", last modified: Sun May 26 17:10:31 2024, max compression
```

## Comparing `funky_modifiers-0.2.5.tar` & `funky_modifiers-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.415243 funky_modifiers-0.2.5/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.2.5/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      483 2024-05-26 14:49:49.414747 funky_modifiers-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.2.5/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.2.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 14:49:49.415739 funky_modifiers-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-05-26 14:49:05.000000 funky_modifiers-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.383994 funky_modifiers-0.2.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.388459 funky_modifiers-0.2.5/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.2.5/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.392924 funky_modifiers-0.2.5/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.2.5/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.2.5/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.2.5/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.395919 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.2.5/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.2.5/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.398877 funky_modifiers-0.2.5/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.2.5/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.2.5/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    41378 2024-05-26 14:46:58.000000 funky_modifiers-0.2.5/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.2.5/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.401355 funky_modifiers-0.2.5/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.2.5/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.2.5/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.2.5/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.2.5/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.414251 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      483 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.413258 funky_modifiers-0.2.5/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.2.5/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.2.5/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.2.5/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.2.5/test/test_converters.py
--rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.2.5/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    14746 2024-05-26 14:08:21.000000 funky_modifiers-0.2.5/test/test_dict_builder.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.2.5/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.2.5/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.2.5/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.2.5/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.2.5/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.823249 funky_modifiers-0.3.0/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      483 2024-05-26 17:10:31.822755 funky_modifiers-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.3.0/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 17:10:31.823249 funky_modifiers-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-05-26 17:08:33.000000 funky_modifiers-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.793985 funky_modifiers-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.798449 funky_modifiers-0.3.0/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.3.0/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.801425 funky_modifiers-0.3.0/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.3.0/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.3.0/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.3.0/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.804897 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.3.0/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.3.0/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.3.0/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.807873 funky_modifiers-0.3.0/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.3.0/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.3.0/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    52352 2024-05-26 17:08:33.000000 funky_modifiers-0.3.0/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.3.0/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.810354 funky_modifiers-0.3.0/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.3.0/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.3.0/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.3.0/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.3.0/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.822257 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      483 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 17:10:31.000000 funky_modifiers-0.3.0/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 17:10:31.821266 funky_modifiers-0.3.0/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.3.0/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.3.0/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.3.0/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.3.0/test/test_converters.py
+-rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.3.0/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    15923 2024-05-26 17:05:25.000000 funky_modifiers-0.3.0/test/test_dict_builder.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.3.0/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.3.0/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.3.0/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.3.0/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.3.0/test/test_pick.py
```

### Comparing `funky_modifiers-0.2.5/LICENSE` & `funky_modifiers-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/setup.py` & `funky_modifiers-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.2.5',
+    version='0.3.0',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `funky_modifiers-0.2.5/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.3.0/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.3.0/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.3.0/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.3.0/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.3.0/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/modularity/logging.py` & `funky_modifiers-0.3.0/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.3.0/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/sorting/converters.py` & `funky_modifiers-0.3.0/src/funk_py/sorting/converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.3.0/src/funk_py/sorting/dict_manip.py`

 * *Files 18% similar despite different names*

```diff
@@ -540,62 +540,138 @@
             return inst
 
         else:
             msg = f'clazz must inherit from dict, but it does not. Provided {clazz}.'
             main_logger.error(msg)
             raise TypeError(msg)
 
-    def __init__(self, _map: Mapping = ..., *, clazz: Type = dict, **kwargs):
+    def __init__(self, _map: Mapping = ..., *, clazz: Type = dict, _other: dict = None,
+                 _transformer: Callable = pass_, **kwargs):
         """
         A builder for dictionaries that has a few helpful methods for merging in data from other
         dictionaries.
 
         :param _map: The ``Mapping`` to start the builder out with. Works like it does for ``dict``.
         :type _map: Mapping
         :param clazz: A dictionary class to inherit from. Used to make sure the builder is the
             desired type of dictionary.
         :type clazz: Type
+        :param _other: The *other* dictionary to use for :meth:`~DictBuilder.pull_from_other`,
+            :meth:`~DictBuilder.get_from_other`, :meth:`~DictBuilder.update_from_other`,
+            and :meth:`~DictBuilder.get_one_of_keys_from_other`. If this is not specified, those
+            methods will not work. It can be changed later.
+        :type _other: dict
+        :param _transformer: The default transformer to use for values retrieved from another dict.
+            Defaults to a function that does nothing to the input.
+        :type _transformer: Callable
         :param kwargs: The ``kwargs`` to construct the starting builder with. Works like it does for
             ``dict``.
         """
         if 'clazz' in kwargs:
             del kwargs['clazz']
 
         if _map is ...:
             self.__builder = self.__class(**kwargs)
 
         else:
             self.__builder = self.__class(_map, **kwargs)
 
+        if _other is not None:
+            self._check_dict(_other)
+
+        self.__other = _other
+
+        self._check_transformer(_transformer)
+        self.__transformer = _transformer
+
     @property
     def clazz(self) -> type:
         """The default class for the ``DictBuilder``."""
         return self.__class
 
+    @property
+    def other(self) -> dict:
+        return self.__other
+
+    @other.setter
+    def other(self, other: dict):
+        if other is not None:
+            self._check_dict(other)
+
+        self.__other = other
+
+    @property
+    def transformer(self) -> Callable:
+        return self.__transformer
+
+    @transformer.setter
+    def transformer(self, transformer: Callable):
+        self._check_transformer(transformer)
+        self.__transformer = transformer
+
+    def use(self, other: dict = ..., transformer: Callable = ...) -> 'DictBuilder':
+        """
+        Set parameter defaults for ``other`` and/or ``transformer``.
+
+        :param other: The new ``other`` to use. If omitted ``other`` will not be changed. If
+            ``None`` is given, then the current ``other`` will be erased, and
+            :meth:`~DictBuilder.pull_from_other`, :meth:`~DictBuilder.get_from_other`,
+            :meth:`~DictBuilder.update_from_other`, and
+            :meth:`~DictBuilder.get_one_of_keys_from_other` will cease to work until a new ``other``
+            is specified.
+        :param transformer: The new ``transformer`` to use as a default transformer in functions. If
+            omitted, ``transformer`` will remain the same. If ``None`` is given, then transformer
+            will be set to its default value (a non-transforming function).
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        if other is not ...:
+            self._check_dict(other)
+            self.__other = other
+
+        if transformer is not ...:
+            self._check_transformer(transformer)
+            self.__transformer = transformer
+
     @staticmethod
     def _check_dict(other: dict):
         if not isinstance(other, dict):
             raise TypeError('Invalid type for other.')
 
     @staticmethod
+    def _check_transformer(transformer: Callable):
+        if not callable(transformer):
+            raise TypeError('Invalid type for transformer.')
+
+    def _choose_transformer(self, transformer: Optional[Callable]):
+        if transformer is None:
+            return self.__transformer
+
+        self._check_transformer(transformer)
+        return transformer
+
+    def _check_has_other(self):
+        if self.__other is None:
+            raise TypeError('No other is set for this DictBuilder. Cannot complete request.')
+
+    @staticmethod
     def _pathify_as(_as: Union[Any, list], val: Any):
         if isinstance(_as, list):
             (path := list(_as)).append(val)
 
         else:
             path = _as, val
 
         return path
 
     @logs_vars(main_logger, start_message='Getting a value from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to get a value from another dictionary.',
                end_message_level='info')
-    def pull_from_other(self, other: dict, key: Union[Any, list], _as: Union[Any, list],
-                        transformer: Callable = pass_) -> 'DictBuilder':
+    def pull_from(self, other: dict, key: Union[Any, list], _as: Union[Any, list],
+                  transformer: Callable = None) -> 'DictBuilder':
         """
         Get a value from another dictionary at a given key, and insert it at the key specified in
         ``_as``. Using this will raise an error if the key doesn't exist in ``other`` or if it
         cannot safely be added to the ``DictBuilder``.
 
         :param other: The dictionary to grab the key from.
         :type other: dict
@@ -604,33 +680,53 @@
         :param _as: The key at which to place the found value from ``other``.
         :type _as: Union[Any, list]
         :param transformer: A transformer that should be called on a value if found.
         :type transformer: Callable
         :return: The current ``DictBuilder`` for chaining.
         """
         self._check_dict(other)
+        transformer = self._choose_transformer(transformer)
 
         # Get the value.
         if isinstance(key, list):
             val = transformer(get_val_from_path(other, *key, unsafe=True))
 
         else:
             val = transformer(other[key])
 
         path = self._pathify_as(_as, val)
         merge_tuplish_pair(path, self.__builder, unsafe=True)
 
         return self
 
+    def pull_from_other(self, key: Union[Any, list], _as: Union[Any, list],
+                        transformer: Callable = None) -> 'DictBuilder':
+        """
+        Get a value from the ``DictBuilder's`` ``other`` at a given key, and insert it at the key
+        specified in ``_as``. Using this will raise an error if the key doesn't exist in ``other``
+        or if it cannot safely be added to the ``DictBuilder``.
+
+        :param key: The key at which to find a value in ``other``.
+        :type key: Union[Any, list]
+        :param _as: The key at which to place the found value from ``other``.
+        :type _as: Union[Any, list]
+        :param transformer: A transformer that should be called on a value if found.
+        :type transformer: Callable
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        self._check_has_other()
+        self.pull_from(self.__other, key, _as, transformer)
+        return self
+
     @logs_vars(main_logger, start_message='Getting a value from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to get a value from another dictionary.',
                end_message_level='info')
-    def get_from_other(self, other: dict, key: Union[Any, list], _as: Union[Any, list],
-                       transformer: Callable = pass_, default: Any = ...) -> 'DictBuilder':
+    def get_from(self, other: dict, key: Union[Any, list], _as: Union[Any, list],
+                 transformer: Callable = None, default: Any = ...) -> 'DictBuilder':
         """
         Get a value from another dictionary at a given key, and insert it at the key specified in
         ``_as``. If ``key`` cannot be found in other or ``the value cannot be added to this
         ``DictBuilder``, then the value simply won't be added.
 
         :param other: The dictionary to grab the key from.
         :type other: dict
@@ -641,14 +737,15 @@
         :param transformer: A transformer that should be called on a value if found.
         :type transformer: Callable
         :param default: The default value to use if a value cannot be found. If omitted, and the
             value is not found, then the value simply won't be added.
         :return: The current ``DictBuilder`` for chaining.
         """
         self._check_dict(other)
+        transformer = self._choose_transformer(transformer)
 
         # Get the value.
         if isinstance(key, list):
             val = get_val_from_path(other, *key, default=...)
 
         else:
             val = other.get(key, ...)
@@ -662,22 +759,43 @@
         else:
             val = transformer(val)
 
         path = self._pathify_as(_as, val)
         merge_tuplish_pair(path, self.__builder)
 
         return self
+
+    def get_from_other(self, key: Union[Any, list], _as: Union[Any, list],
+                       transformer: Callable = None, default: Any = ...) -> 'DictBuilder':
+        """
+        Get a value from the ``DictBuilder's`` ``other`` at a given key, and insert it at the key
+        specified in ``_as``. If ``key`` cannot be found in ``other`` or the value cannot be added
+        to this ``DictBuilder``, then the value simply won't be added.
+
+        :param key: The key at which to find a value in ``other``.
+        :type key: Union[Any, list]
+        :param _as: The key at which to place the found value from ``other``.
+        :type _as: Union[Any, list]
+        :param transformer: A transformer that should be called on a value if found.
+        :type transformer: Callable
+        :param default: The default value to use if a value cannot be found. If omitted, and the
+            value is not found, then the value simply won't be added.
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        self._check_has_other()
+        self.get_from(self.__other, key, _as, transformer, default)
+        return self
     
     @logs_vars(main_logger, start_message='Updating from a list...',
                start_message_level='info',
                end_message='Finished attempt to update from list.',
                end_message_level='info')
     def update_from_list(self, other: List[dict],
                           _as: Union[Any, None, list] = None,
-                          transformer: Callable = pass_,
+                          transformer: Callable = None,
                           unsafe: bool = False,
                           classes: Union[List[Type[dict]], Type[dict]] = None) -> 'DictBuilder':
         """
         Update this ``DictBuilder`` from another dict.
 
         :param other: The dictionary to update with.
         :type other: dict
@@ -702,14 +820,16 @@
             - If this is a single type, any new dicts generated when following the path described by
               ``_as`` will be of the type specified.
             - If this is not specified, each generated dictionary will be of the same type as the
               ``DictBuilder.clazz``.
         :type classes: Optional[Union[List[Type[dict]], Type[dict]]]
         :return: The current ``DictBuilder`` for chaining.
         """
+        transformer = self._choose_transformer(transformer)
+
         worker = self.__builder
         worker = self._update_seek(_as, worker, unsafe, classes)
         for val in dive_to_dicts(other):
             if not isinstance(t := transformer(val), dict):
                 if unsafe:
                     main_logger.error(_NO_MERGE)
                     raise ValueError(_NO_MERGE)
@@ -720,22 +840,22 @@
 
         return self
 
     @logs_vars(main_logger, start_message='Updating from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to update from another dictionary.',
                end_message_level='info')
-    def update_from_other(self, other: dict,
-                          key: Any = None,
-                          _as: Union[Any, None, list] = None,
-                          keys: List[Any] = None,
-                          transformer: Callable = pass_,
-                          unsafe: bool = False,
-                          classes: Union[List[Type[dict]], Type[dict]] = None,
-                          val_is_list: bool = False) -> 'DictBuilder':
+    def update_from(self, other: dict,
+                    key: Any = None,
+                    _as: Union[Any, None, list] = None,
+                    keys: List[Any] = None,
+                    transformer: Callable = None,
+                    unsafe: bool = False,
+                    classes: Union[List[Type[dict]], Type[dict]] = None,
+                    val_is_list: bool = False) -> 'DictBuilder':
         """
         Update this ``DictBuilder`` from another dict.
 
         :param other: The dictionary to update with.
         :type other: dict
         :param key: The key at which the source dictionary should be in ``other``. If not specified
             ``other`` will be used as-is unless ``keys`` is specified.
@@ -770,14 +890,15 @@
         :param val_is_list: Whether the value at ``key`` in ``other`` should be considered as a list
             and its values iterated over and individually used to update the ``DictBuilder``.
             Defaults to ``False``.
         :type val_is_list: bool
         :return: The current ``DictBuilder`` for chaining.
         """
         self._check_dict(other)
+        transformer = self._choose_transformer(transformer)
 
         val = self._update_find_in_other(other, key, keys, unsafe)
         if val is ...:
             main_logger.info('Target value could not be located.')
             if unsafe:
                 k = [key]
                 if keys is not None:
@@ -790,58 +911,123 @@
         if not (val_is_list or isinstance(transformer(val), dict)):
             if unsafe:
                 main_logger.error(_NO_MERGE)
                 raise ValueError(_NO_MERGE)
 
             return self
 
+        self._update_vals(val, _as, unsafe, transformer, classes, val_is_list)
+        return self
+
+    def update_from_other(self, key: Any = None,
+                          _as: Union[Any, None, list] = None,
+                          keys: List[Any] = None,
+                          transformer: Callable = None,
+                          unsafe: bool = False,
+                          classes: Union[List[Type[dict]], Type[dict]] = None,
+                          val_is_list: bool = False) -> 'DictBuilder':
+        """
+        Update this ``DictBuilder`` from it's stored ``other``.
+
+        :param key: The key at which the source dictionary should be in ``other``. If not specified
+            ``other`` will be used as-is unless ``keys`` is specified.
+        :type key: Optional[Union[Any, None, list]]
+        :param _as: The key at which to place update with the found value from ``other``. If not
+            specified, will simply update the entire ``DictBuilder``.
+        :type _as: Union[Any, None, list]
+        :param keys: A list of possible keys at which the source dictionary might be located in
+            ``other``. Each key should follow the same rules as ``key``. If ``key`` is specified,
+            ``key`` will be attempted first, then ``keys`` will be attempted.
+        :type keys: Optional[List[Union[Any, None, list]]]
+        :param transformer: A transformer that should be called on the value being used to update
+            the ``DictBuilder``.
+        :type transformer: Callable
+        :param unsafe: Whether an error should be raised if the desired operation cannot be
+            completed.
+        :type unsafe: bool
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
+        :param val_is_list: Whether the value at ``key`` in ``other`` should be considered as a list
+            and its values iterated over and individually used to update the ``DictBuilder``.
+            Defaults to ``False``.
+        :type val_is_list: bool
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        self._check_has_other()
+        self.update_from(self.__other, key, _as, keys, transformer, unsafe, classes, val_is_list)
+        return self
+
+    def _update_vals(self, val: Any,
+                     _as: Any,
+                     unsafe: bool,
+                     transformer: Callable,
+                     classes: Union[List[Type[dict]], Type[dict]],
+                     val_is_list: bool):
         worker = self.__builder
         worker = self._update_seek(_as, worker, unsafe, classes)
         if val_is_list:
+            # Don't assume there is a list just because the user expected one to be there.
             if isinstance(val, list):
                 for _val in dive_to_dicts(val):
                     if not isinstance(t := transformer(_val), dict):
                         if unsafe:
                             main_logger.error(_NO_MERGE)
                             raise ValueError(_NO_MERGE)
 
                         continue
 
                     worker.update(t)
 
             elif not isinstance(t := transformer(val), dict):
+                # If we don't have a list, make sure we don't need to raise an exception.
                 if unsafe:
                     main_logger.error(_NO_MERGE)
                     raise ValueError(_NO_MERGE)
 
-                return self
-
             else:
+                # If a dictionary is present instead of a list, use that to update.
                 worker.update(t)
 
+            return
 
-        else:
-            worker.update(transformer(val))
-
-        return self
+        worker.update(transformer(val))
 
     @staticmethod
     def _update_find_in_other(other: dict, key: Any, keys: List[Any], unsafe: bool = False):
+        # Find a key in other, if it exists. Return ... if it doesn't.
         if key is not None:
             if keys is not None:
+                # If the user specified both key and keys, that is silly, but handle feeding both
+                # into get_one_of_keys for them. No need to raise an exception.
                 return get_one_of_keys(other, key, *keys, default=...)
 
             elif isinstance(key, list):
+                # Only a key is present and it specifies a path. Follow the path.
                 return get_val_from_path(other, *key, unsafe=unsafe, default=...)
 
+            # Simple key is specified.
             return other.get(key, ...)
 
         elif keys is not None:
+            # key isn't specified, but keys is. Try to get one of keys.
             return get_one_of_keys(other, *keys, default=...)
 
+        # If neither keys nor key is specified, assume the user wants the entire dictionary.
         return other
 
     @logs_vars(main_logger, start_message='Attempting to locate target to update...')
     def _update_seek(self, _as: Any,
                      worker: dict,
                      unsafe: bool,
                      classes: Union[None, List[Type[dict]], Type[dict]]):
@@ -894,17 +1080,19 @@
 
         return worker
 
     @logs_vars(main_logger, start_message='Getting one of the keys from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to get one of the keys from another dictionary.',
                end_message_level='info')
-    def get_one_of_keys_from_other(self, other: dict, _as: Union[Any, list],
-                                   *keys: Union[Any, list], transformer: Callable = pass_,
-                                   default: Any = ...) -> 'DictBuilder':
+    def get_one_of_keys_from(self, other: dict,
+                             _as: Union[Any, list],
+                             *keys: Union[Any, list],
+                             transformer: Callable = None,
+                             default: Any = ...) -> 'DictBuilder':
         """
         Gets the value at one of the keys (or key paths) specified in ``keys`` from ``other`` and
         adds it at ``_as`` within the ``DictBuilder``.
 
         :param other: The source ``dict`` to get the value from.
         :type other: dict
         :param _as: The key or key path to add a found value at.
@@ -912,14 +1100,17 @@
         :param keys: The possible keys or key paths the sought value could be located at.
         :type keys: Union[Any, list]
         :param default: The default value to return if the target value cannot be found. If this is
             not specified, then should no value be found, a value simply won't be added.
         :type default: Any
         :return: The current ``DictBuilder`` for chaining.
         """
+        self._check_dict(other)
+        transformer = self._choose_transformer(transformer)
+
         val = get_one_of_keys(other, *keys, ...)
         if val is ...:
             if default is ...:
                 return self
 
             val = default
 
@@ -927,14 +1118,35 @@
             val = transformer(val)
 
         path = self._pathify_as(_as, val)
         merge_tuplish_pair(path, self.__builder)
 
         return self
 
+    def get_one_of_keys_from_other(self, _as: Union[Any, list],
+                                   *keys: Union[Any, list], transformer: Callable = None,
+                                   default: Any = ...) -> 'DictBuilder':
+        """
+        Gets the value at one of the keys (or key paths) specified in ``keys`` from the
+        ``DictBuilder's`` ``other`` and adds it at ``_as`` within the ``DictBuilder``.
+
+        :param _as: The key or key path to add a found value at.
+        :type _as: Union[Any, list]
+        :param keys: The possible keys or key paths the sought value could be located at.
+        :type keys: Union[Any, list]
+        :param default: The default value to return if the target value cannot be found. If this is
+            not specified, then should no value be found, a value simply won't be added.
+        :type default: Any
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        self._check_has_other()
+        self.get_one_of_keys_from(self.__other, _as, *keys, transformer=transformer,
+                                  default=default)
+        return self
+
     @logs_vars(main_logger, start_message='Updating dictionary...', start_message_level='info',
                end_message='Finished updating.', end_message_level='info')
     def update(self, _map: Mapping = ..., **kwargs) -> 'DictBuilder':
         self.__builder.update(_map, **kwargs)
         return self
 
     def __delitem__(self, key) -> 'DictBuilder':
@@ -964,14 +1176,15 @@
         result = deepcopy(self.__builder)
         if strict:
             return result
 
         return self._convert_all_to_dicts(result)
 
     def _convert_all_to_dicts(self, source: dict) -> dict:
+        # One return statement. Returns worker.
         if type(source) is dict:
             worker = source
 
         else:
             worker = dict(source)
 
         for key, val in source.items():
```

### Comparing `funky_modifiers-0.2.5/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.3.0/src/funk_py/sorting/pieces.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.3.0/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.3.0/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.3.0/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.3.0/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.3.0/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_check_dict_equality.py` & `funky_modifiers-0.3.0/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_check_list_equality.py` & `funky_modifiers-0.3.0/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.3.0/test/test_convert_tuplish_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_converters.py` & `funky_modifiers-0.3.0/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_converts_enums.py` & `funky_modifiers-0.3.0/test/test_converts_enums.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_dict_builder.py` & `funky_modifiers-0.3.0/test/test_dict_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import Counter
 from copy import deepcopy
 
 import pytest
 
+from funk_py.modularity.basic_structures import pass_
 from t_support import cov, cov_counter
 from funk_py.sorting.dict_manip import DictBuilder
 
 
 # The following manages whether the generated coverage instance from t_support should report. This
 # method of coverage is used so that coverage can be turned off to not interfere in timed tests.
 @pytest.fixture(scope='session', autouse=True)
@@ -126,19 +127,32 @@
 
 def test_can_instantiate(instantiation_pattern, type_spec):
     testy = instantiate(*instantiation_pattern[:2], type_spec)
     if type_spec is not None:
         assert testy.clazz is type_spec
         # Don't test build inside the instantiation test.
 
+    assert testy.other is None
+    assert testy.transformer is pass_
+
+
+def test_instantiate_with_defaults(base_dict1):
+    def t_func(x):
+        return {K1: str(x)}
+
+    testy = DictBuilder(_other=base_dict1, _transformer=t_func)
+    assert testy.other is base_dict1, 'Other did not match expected.'
+    assert testy.transformer is t_func, 'Transformer did not match expected.'
+
 
 def test_can_build(instantiation_pattern, type_spec):
     testy = instantiate(*instantiation_pattern[:2], type_spec)
+    t = testy.build()
     if type_spec is not None:
-        assert type(testy.build()) is type_spec
+        assert type(t) is type_spec
 
 
 def test_can_setitem(instantiation_pattern, type_spec):
     testy = instantiate(*instantiation_pattern[:2], type_spec)
     testy[T_KEY] = T_VAL
     result = instantiation_pattern[2]
     result[T_KEY] = T_VAL
@@ -177,95 +191,95 @@
     result = instantiation_pattern[2]
     result.update(base_dict1)
     assert testy.build() == result
     if type_spec is not None:
         assert testy.clazz is type_spec
 
 
-def test_can_update_from_other(instantiation_pattern, base_dict1, type_spec):
+def test_can_update_from(instantiation_pattern, base_dict1, type_spec):
     testy = instantiate(*instantiation_pattern[:2], type_spec)
-    testy.update_from_other(base_dict1)
+    testy.update_from(base_dict1)
     result = instantiation_pattern[2]
     result.update(base_dict1)
     assert testy.build() == result
     if type_spec is not None:
         assert testy.clazz is type_spec
 
 
-def test_nested_can_update_from_nested_other(higher_dict1, higher_dict2):
+def test_nested_can_update_from(higher_dict1, higher_dict2):
     testy = DictBuilder(deepcopy(higher_dict2))
-    testy.update_from_other(deepcopy(higher_dict1))
+    testy.update_from(deepcopy(higher_dict1))
     result = deepcopy(higher_dict2)
     result.update(deepcopy(higher_dict1))
     assert testy.build() == result
 
     testy = DictBuilder(deepcopy(higher_dict2))
-    testy.update_from_other(deepcopy(higher_dict1), K6)
+    testy.update_from(deepcopy(higher_dict1), K6)
     result = deepcopy(higher_dict2)
     result.update(deepcopy(higher_dict1[K6]))
     assert testy.build() == result
 
     testy = DictBuilder(deepcopy(higher_dict2))
-    testy.update_from_other(deepcopy(higher_dict1), [K6, K4])
+    testy.update_from(deepcopy(higher_dict1), [K6, K4])
     result = deepcopy(higher_dict2)
     result.update(deepcopy(higher_dict1[K6][K4]))
     assert testy.build() == result
 
     testy = DictBuilder(deepcopy(higher_dict2))
-    testy.update_from_other(deepcopy(higher_dict1), _as=K8)
+    testy.update_from(deepcopy(higher_dict1), _as=K8)
     result = deepcopy(higher_dict2)
     result[K8].update(deepcopy(higher_dict1))
     assert testy.build() == result
 
     testy = DictBuilder(deepcopy(higher_dict2))
-    testy.update_from_other(deepcopy(higher_dict1), K6, K8)
+    testy.update_from(deepcopy(higher_dict1), K6, K8)
     result = deepcopy(higher_dict2)
     result[K8].update(deepcopy(higher_dict1[K6]))
     assert testy.build() == result
 
     testy = DictBuilder(deepcopy(higher_dict2))
-    testy.update_from_other(deepcopy(higher_dict1), [K6, K4], K8)
+    testy.update_from(deepcopy(higher_dict1), [K6, K4], K8)
     result = deepcopy(higher_dict2)
     result[K8].update(deepcopy(higher_dict1[K6][K4]))
     assert testy.build() == result
 
     testy = DictBuilder(deepcopy(higher_dict2))
-    testy.update_from_other(deepcopy(higher_dict1), _as=[K8, K6])
+    testy.update_from(deepcopy(higher_dict1), _as=[K8, K6])
     result = deepcopy(higher_dict2)
     result[K8][K6].update(deepcopy(higher_dict1))
     assert testy.build() == result
 
     testy = DictBuilder(deepcopy(higher_dict2))
-    testy.update_from_other(deepcopy(higher_dict1), K6, [K8, K6])
+    testy.update_from(deepcopy(higher_dict1), K6, [K8, K6])
     result = deepcopy(higher_dict2)
     result[K8][K6].update(deepcopy(higher_dict1[K6]))
     assert testy.build() == result
 
     testy = DictBuilder(deepcopy(higher_dict2))
-    testy.update_from_other(deepcopy(higher_dict1), [K6, K4], [K8, K6])
+    testy.update_from(deepcopy(higher_dict1), [K6, K4], [K8, K6])
     result = deepcopy(higher_dict2)
     result[K8][K6].update(deepcopy(higher_dict1[K6][K4]))
     assert testy.build() == result
 
 
-def test_update_from_other_with_classes_generates_correct(base_dict1, base_dict2):
+def test_update_from_with_classes_generates_correct(base_dict1, base_dict2):
     testy = DictBuilder(deepcopy(base_dict2))
-    testy.update_from_other(deepcopy(base_dict1), _as=K5, classes=Counter)
+    testy.update_from(deepcopy(base_dict1), _as=K5, classes=Counter)
     result = deepcopy(base_dict2)
     result[K5] = base_dict1
     built = testy.build()
     assert built == result
     assert type(built) is dict
     assert type(built[K5]) is Counter
 
 
-def test_update_from_other_with_classes_behaves_expected(base_dict1, base_dict2):
+def test_update_from_with_classes_behaves_expected(base_dict1, base_dict2):
     testy = DictBuilder(deepcopy(base_dict2))
-    testy.update_from_other(deepcopy(base_dict1), _as=K5, classes=Counter)
-    testy.update_from_other(deepcopy(base_dict1), _as=K5)
+    testy.update_from(deepcopy(base_dict1), _as=K5, classes=Counter)
+    testy.update_from(deepcopy(base_dict1), _as=K5)
 
     expectation = Counter(base_dict1)
     expectation.update(base_dict1)
     _known_result = {k: 2*v for k, v in base_dict1.items()}
     assert _known_result == expectation, ('The behavior of Counter seems to have changed. '
                                           'This test is no longer valid.')
 
@@ -273,25 +287,53 @@
     result[K5] = expectation
     built = testy.build()
     assert built == result
     assert type(built) is dict
     assert type(built[K5]) is Counter
 
 
-def test_update_from_other_with_classes_can_be_made_dict(base_dict1, base_dict2):
+def test_update_from_with_classes_can_be_made_dict(base_dict1, base_dict2):
     testy = DictBuilder(deepcopy(base_dict2))
-    testy.update_from_other(deepcopy(base_dict1), _as=K5, classes=Counter)
+    testy.update_from(deepcopy(base_dict1), _as=K5, classes=Counter)
     result = deepcopy(base_dict2)
     result[K5] = base_dict1
     built = testy.build(False)
     assert built == result
     assert type(built) is dict
     assert type(built[K5]) is dict
 
 
+def test_fails_other_when_no_other(base_dict1):
+    testy = DictBuilder()
+    with pytest.raises(TypeError):
+        testy.get_from_other(K1, K2)
+
+    with pytest.raises(TypeError):
+        testy.get_one_of_keys_from_other(K1, K1, K2)
+
+    with pytest.raises(TypeError):
+        testy.update_from_other()
+
+    with pytest.raises(TypeError):
+        testy.pull_from_other(K1, K2)
+
+
+def test_use(base_dict1):
+    def t_func(x):
+        return {K1: str(x)}
+
+    testy = DictBuilder()
+    assert testy.other is None and testy.transformer is pass_, 'Not instantiated correctly.'
+
+    testy.use(other=base_dict1)
+    assert testy.other is base_dict1 and testy.transformer is pass_, 'Setting other failed.'
+
+    testy.use(transformer=t_func)
+    assert testy.other is base_dict1 and testy.transformer is t_func, 'Setting transformer failed.'
+
 TOP_LVL = 'top level'
 TOP_LVL_LST = 'top level (list)'
 NEW_TOP_LVL = 'new top level'
 NEW_TOP_LVL_LST = 'new top level (list)'
 NEW_1ST_2ND_LVL = 'new first and second level'
 NEW_2ND_LVL = 'new second level'
 SCND_LVL = 'second level'
@@ -443,17 +485,17 @@
 
     k1, _from = froms
     k2, to = tos
     result = to_lookup[to](k1, k2, from_lookup[_from])
     return k1, k2, result
 
 
-def test_get_from_other(get_from_other_params, higher_dict1, higher_dict2):
+def test_get_from(get_from_other_params, higher_dict1, higher_dict2):
     testy = DictBuilder(higher_dict2)
-    testy.get_from_other(higher_dict1, get_from_other_params[0], get_from_other_params[1])
+    testy.get_from(higher_dict1, get_from_other_params[0], get_from_other_params[1])
     assert testy.build() == get_from_other_params[2]
 
 
 @pytest.fixture(params=(
         ((KB,),(K6,)),
         ((), (K6,)),
         (([K6, K5],), (K7,)),
@@ -465,17 +507,17 @@
         'bad keys and partly good key before, no key after',
 ))
 def get_one_key_params(request, get_from_other_params):
     before, after = request.param
     return (*before, get_from_other_params[0], *after), *get_from_other_params[1:]
 
 
-def test_get_one_key_from_other(get_one_key_params, higher_dict1, higher_dict2):
+def test_get_one_key_from(get_one_key_params, higher_dict1, higher_dict2):
     testy = DictBuilder(higher_dict2)
-    testy.get_one_of_keys_from_other(higher_dict1, get_one_key_params[1], *get_one_key_params[0])
+    testy.get_one_of_keys_from(higher_dict1, get_one_key_params[1], *get_one_key_params[0])
     assert testy.build() == get_one_key_params[2]
 
 
 SIMP_DICT = {K8: V1}
 
 
 def test_update_from_list(base_dict1, high_dict1, higher_dict1):
```

### Comparing `funky_modifiers-0.2.5/test/test_drop_none_dict.py` & `funky_modifiers-0.3.0/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_function_hash_and_equality.py` & `funky_modifiers-0.3.0/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_logs_vars.py` & `funky_modifiers-0.3.0/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_obj.py` & `funky_modifiers-0.3.0/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.5/test/test_pick.py` & `funky_modifiers-0.3.0/test/test_pick.py`

 * *Files identical despite different names*

