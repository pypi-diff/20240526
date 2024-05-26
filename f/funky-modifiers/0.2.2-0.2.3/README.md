# Comparing `tmp/funky_modifiers-0.2.2.tar.gz` & `tmp/funky_modifiers-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.2.2.tar", last modified: Sun May 26 13:17:45 2024, max compression
+gzip compressed data, was "funky_modifiers-0.2.3.tar", last modified: Sun May 26 14:11:10 2024, max compression
```

## Comparing `funky_modifiers-0.2.2.tar` & `funky_modifiers-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.272052 funky_modifiers-0.2.2/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      483 2024-05-26 13:17:45.271556 funky_modifiers-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.2.2/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 13:17:45.272052 funky_modifiers-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-05-26 13:17:23.000000 funky_modifiers-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.240309 funky_modifiers-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.244772 funky_modifiers-0.2.2/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.2.2/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.248741 funky_modifiers-0.2.2/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.2.2/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.2.2/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.2.2/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.251221 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.2.2/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.2.2/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.2.2/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.254197 funky_modifiers-0.2.2/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.2.2/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.2.2/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    36675 2024-05-26 13:12:47.000000 funky_modifiers-0.2.2/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.2.2/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.257670 funky_modifiers-0.2.2/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.2.2/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.2.2/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.2.2/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.2.2/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.271060 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      483 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 13:17:45.000000 funky_modifiers-0.2.2/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 13:17:45.270069 funky_modifiers-0.2.2/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.2.2/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.2.2/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.2.2/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.2.2/test/test_converters.py
--rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.2.2/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    13608 2024-05-26 13:08:42.000000 funky_modifiers-0.2.2/test/test_dict_builder.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.2.2/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.2.2/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.2.2/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.2.2/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.2.2/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:10.514594 funky_modifiers-0.2.3/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      483 2024-05-26 14:11:10.514099 funky_modifiers-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.2.3/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:11:10.514594 funky_modifiers-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-05-26 14:10:17.000000 funky_modifiers-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:10.485330 funky_modifiers-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:10.489794 funky_modifiers-0.2.3/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.2.3/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:10.493266 funky_modifiers-0.2.3/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.2.3/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.2.3/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.2.3/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:10.496242 funky_modifiers-0.2.3/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.2.3/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.2.3/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.2.3/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.2.3/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.2.3/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.2.3/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:10.498722 funky_modifiers-0.2.3/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.2.3/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.2.3/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    40365 2024-05-26 13:50:11.000000 funky_modifiers-0.2.3/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.2.3/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:10.501201 funky_modifiers-0.2.3/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.2.3/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.2.3/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.2.3/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.2.3/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:10.513602 funky_modifiers-0.2.3/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      483 2024-05-26 14:11:10.000000 funky_modifiers-0.2.3/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2024-05-26 14:11:10.000000 funky_modifiers-0.2.3/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:11:10.000000 funky_modifiers-0.2.3/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 14:11:10.000000 funky_modifiers-0.2.3/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 14:11:10.000000 funky_modifiers-0.2.3/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 14:11:10.512610 funky_modifiers-0.2.3/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.2.3/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.2.3/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.2.3/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.2.3/test/test_converters.py
+-rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.2.3/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    14746 2024-05-26 14:08:21.000000 funky_modifiers-0.2.3/test/test_dict_builder.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.2.3/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.2.3/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.2.3/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.2.3/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.2.3/test/test_pick.py
```

### Comparing `funky_modifiers-0.2.2/LICENSE` & `funky_modifiers-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/setup.py` & `funky_modifiers-0.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.2.2',
+    version='0.2.3',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `funky_modifiers-0.2.2/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.2.3/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.2.3/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.2.3/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.2.3/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.2.3/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/modularity/logging.py` & `funky_modifiers-0.2.3/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.2.3/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/sorting/converters.py` & `funky_modifiers-0.2.3/src/funk_py/sorting/converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.2.3/src/funk_py/sorting/dict_manip.py`

 * *Files 4% similar despite different names*

```diff
@@ -522,14 +522,17 @@
 
         elif key in source:
             return source[key]
 
     return default
 
 
+_NO_MERGE = 'Cannot merge a non-dict to a dict.'
+
+
 class DictBuilder:
     def __new__(cls, *args, clazz: Type = dict, **kwargs):
         if clazz is None:
             clazz = dict
 
         inst = super().__new__(cls)
         if issubclass(clazz, dict):
@@ -659,25 +662,79 @@
         else:
             val = transformer(val)
 
         path = self._pathify_as(_as, val)
         merge_tuplish_pair(path, self.__builder)
 
         return self
+    
+    @logs_vars(main_logger, start_message='Updating from a list...',
+               start_message_level='info',
+               end_message='Finished attempt to update from list.',
+               end_message_level='info')
+    def update_from_list(self, other: List[dict],
+                          _as: Union[Any, None, list] = None,
+                          transformer: Callable = pass_,
+                          unsafe: bool = False,
+                          classes: Union[List[Type[dict]], Type[dict]] = None) -> 'DictBuilder':
+        """
+        Update this ``DictBuilder`` from another dict.
+
+        :param other: The dictionary to update with.
+        :type other: dict
+        :param _as: The key at which to place update with the found value from ``other``. If not
+            specified, will simply update the entire ``DictBuilder``.
+        :type _as: Union[Any, None, list]
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
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        worker = self.__builder
+        worker = self._update_seek(_as, worker, unsafe, classes)
+        for val in dive_to_dicts(other):
+            if not isinstance(t := transformer(val), dict):
+                if unsafe:
+                    main_logger.error(_NO_MERGE)
+                    raise ValueError(_NO_MERGE)
+
+                continue
+
+            worker.update(t)
+
+        return self
 
     @logs_vars(main_logger, start_message='Updating from another dictionary...',
                start_message_level='info',
                end_message='Finished attempt to update from another dictionary.',
                end_message_level='info')
     def update_from_other(self, other: dict,
                           key: Union[Any, None, list] = None,
                           _as: Union[Any, None, list] = None,
                           transformer: Callable = pass_,
                           unsafe: bool = False,
-                          classes: Union[List[Type[dict]], Type[dict]] = None) -> 'DictBuilder':
+                          classes: Union[List[Type[dict]], Type[dict]] = None,
+                          val_is_list: bool = False) -> 'DictBuilder':
         """
         Update this ``DictBuilder`` from another dict.
 
         :param other: The dictionary to update with.
         :type other: dict
         :param key: The key at which the source dictionary should be in ``other``. If not specified
             ``other`` will be used as-is.
@@ -701,49 +758,67 @@
               will be of the same type as the ``DictBuilder.clazz``. If this longer than ``_as``, it
               will only be used for needed locations.
             - If this is a single type, any new dicts generated when following the path described by
               ``_as`` will be of the type specified.
             - If this is not specified, each generated dictionary will be of the same type as the
               ``DictBuilder.clazz``.
         :type classes: Optional[Union[List[Type[dict]], Type[dict]]]
+        :param val_is_list: Whether the value at ``key`` in ``other`` should be considered as a list
+            and its values iterated over and individually used to update the ``DictBuilder``.
+            Defaults to ``False``.
+        :type val_is_list: bool
         :return: The current ``DictBuilder`` for chaining.
         """
         self._check_dict(other)
-        # Get the value.
-        if key is not None:
-            if isinstance(key, list):
-                val = get_val_from_path(other, *key, unsafe=unsafe, default=...)
-
-            elif unsafe:
-                val = other[key]
-
-            else:
-                val = other.get(key, ...)
-
-        else:
-            val = other
+        val = self._update_find_in_other(other, key, unsafe)
 
         if val is ...:
             main_logger.info('Target value could not be located.')
             return self
 
-        if not isinstance(val, dict):
+        if not ((val_is_list and type(val) is list) or isinstance(transformer(val), dict)):
             if unsafe:
-                msg = 'Cannot merge a dict to a value.'
-                main_logger.error(msg)
-                raise ValueError(msg)
+                main_logger.error(_NO_MERGE)
+                raise ValueError(_NO_MERGE)
 
             return self
 
         worker = self.__builder
         worker = self._update_seek(_as, worker, unsafe, classes)
-        worker.update(transformer(val))
+        if val_is_list:
+            for _val in dive_to_dicts(val):
+                if not isinstance(t := transformer(_val), dict):
+                    if unsafe:
+                        main_logger.error(_NO_MERGE)
+                        raise ValueError(_NO_MERGE)
+
+                    continue
+
+                worker.update(t)
+
+        else:
+            worker.update(transformer(val))
 
         return self
 
+    @staticmethod
+    def _update_find_in_other(other: dict,
+                              key: Union[Any, None, list] = None,
+                              unsafe: bool = False):
+        if key is not None:
+            if isinstance(key, list):
+                return get_val_from_path(other, *key, unsafe=unsafe, default=...)
+
+            elif unsafe:
+                return other[key]
+
+            return other.get(key, ...)
+
+        return other
+
     @logs_vars(main_logger, start_message='Attempting to locate target to update...')
     def _update_seek(self, _as: Any,
                      worker: dict,
                      unsafe: bool,
                      classes: Union[None, List[Type[dict]], Type[dict]]):
         if _as is not None:
             needed = len(_as)
```

### Comparing `funky_modifiers-0.2.2/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.2.3/src/funk_py/sorting/pieces.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.2.3/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.2.3/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.2.3/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.2.3/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.2.3/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_check_dict_equality.py` & `funky_modifiers-0.2.3/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_check_list_equality.py` & `funky_modifiers-0.2.3/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.2.3/test/test_convert_tuplish_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_converters.py` & `funky_modifiers-0.2.3/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_converts_enums.py` & `funky_modifiers-0.2.3/test/test_converts_enums.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_dict_builder.py` & `funky_modifiers-0.2.3/test/test_dict_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -469,7 +469,35 @@
     return (*before, get_from_other_params[0], *after), *get_from_other_params[1:]
 
 
 def test_get_one_key_from_other(get_one_key_params, higher_dict1, higher_dict2):
     testy = DictBuilder(higher_dict2)
     testy.get_one_of_keys_from_other(higher_dict1, get_one_key_params[1], *get_one_key_params[0])
     assert testy.build() == get_one_key_params[2]
+
+
+SIMP_DICT = {K8: V1}
+
+
+def test_update_from_list(base_dict1, high_dict1, higher_dict1):
+    testy = DictBuilder()
+    testy.update_from_list([deepcopy(base_dict1), deepcopy(high_dict1), deepcopy(higher_dict1)])
+    result = {}
+    result.update(deepcopy(base_dict1))
+    result.update(deepcopy(high_dict1))
+    result.update(deepcopy(higher_dict1))
+    assert testy.build() == result, 'Failed for a simple list!'
+
+    testy = DictBuilder()
+    testy.update_from_list([[deepcopy(base_dict1)], [deepcopy(high_dict1)],
+                            [deepcopy(higher_dict1)]])
+    assert testy.build() == result, 'Failed for list containing one item in each list!'
+
+    testy = DictBuilder()
+    testy.update_from_list([deepcopy(base_dict1), deepcopy(high_dict1),
+                            {K8: deepcopy(higher_dict1)}])
+    result = {}
+    result.update(deepcopy(base_dict1))
+    result.update(deepcopy(high_dict1))
+    result.update({K8: deepcopy(higher_dict1)})
+    assert testy.build() == result, ('Failed for a list with one item in a dictionary with only one'
+                                     ' key.')
```

### Comparing `funky_modifiers-0.2.2/test/test_drop_none_dict.py` & `funky_modifiers-0.2.3/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_function_hash_and_equality.py` & `funky_modifiers-0.2.3/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_logs_vars.py` & `funky_modifiers-0.2.3/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_obj.py` & `funky_modifiers-0.2.3/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.2/test/test_pick.py` & `funky_modifiers-0.2.3/test/test_pick.py`

 * *Files identical despite different names*

