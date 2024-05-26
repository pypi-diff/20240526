# Comparing `tmp/funky_modifiers-0.3.1.tar.gz` & `tmp/funky_modifiers-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.3.1.tar", last modified: Sun May 26 20:44:41 2024, max compression
+gzip compressed data, was "funky_modifiers-0.3.2.tar", last modified: Sun May 26 21:42:20 2024, max compression
```

## Comparing `funky_modifiers-0.3.1.tar` & `funky_modifiers-0.3.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.464642 funky_modifiers-0.3.1/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      483 2024-05-26 20:44:41.464146 funky_modifiers-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.3.1/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 20:44:41.465138 funky_modifiers-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-05-26 20:42:39.000000 funky_modifiers-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.410578 funky_modifiers-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.435379 funky_modifiers-0.3.1/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.3.1/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.439844 funky_modifiers-0.3.1/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.3.1/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.3.1/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.3.1/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.443314 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.3.1/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.3.1/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.3.1/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.446290 funky_modifiers-0.3.1/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.3.1/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.3.1/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    58158 2024-05-26 20:43:05.000000 funky_modifiers-0.3.1/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.3.1/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.449267 funky_modifiers-0.3.1/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.3.1/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.3.1/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.3.1/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.3.1/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.463674 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      483 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 20:44:41.000000 funky_modifiers-0.3.1/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 20:44:41.462186 funky_modifiers-0.3.1/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.3.1/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.3.1/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.3.1/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.3.1/test/test_converters.py
--rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.3.1/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    16939 2024-05-26 20:32:05.000000 funky_modifiers-0.3.1/test/test_dict_builder.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.3.1/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.3.1/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.3.1/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.3.1/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.3.1/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2024-05-26 21:42:20.217367 funky_modifiers-0.3.2/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      483 2024-05-26 21:42:20.216871 funky_modifiers-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.3.2/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.3.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 21:42:20.217367 funky_modifiers-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-05-26 21:41:35.000000 funky_modifiers-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 21:42:20.185126 funky_modifiers-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 21:42:20.190085 funky_modifiers-0.3.2/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.3.2/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 21:42:20.194584 funky_modifiers-0.3.2/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.3.2/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.3.2/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.3.2/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-05-26 21:42:20.197029 funky_modifiers-0.3.2/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.3.2/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.3.2/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.3.2/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.3.2/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.3.2/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.3.2/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-26 21:42:20.200005 funky_modifiers-0.3.2/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.3.2/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.3.2/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    58181 2024-05-26 21:41:35.000000 funky_modifiers-0.3.2/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.3.2/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-05-26 21:42:20.202485 funky_modifiers-0.3.2/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.3.2/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.3.2/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.3.2/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.3.2/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-26 21:42:20.215879 funky_modifiers-0.3.2/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      483 2024-05-26 21:42:20.000000 funky_modifiers-0.3.2/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2024-05-26 21:42:20.000000 funky_modifiers-0.3.2/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 21:42:20.000000 funky_modifiers-0.3.2/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 21:42:20.000000 funky_modifiers-0.3.2/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 21:42:20.000000 funky_modifiers-0.3.2/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 21:42:20.215382 funky_modifiers-0.3.2/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.3.2/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.3.2/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.3.2/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.3.2/test/test_converters.py
+-rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.3.2/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    17001 2024-05-26 21:41:35.000000 funky_modifiers-0.3.2/test/test_dict_builder.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.3.2/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.3.2/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.3.2/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.3.2/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.3.2/test/test_pick.py
```

### Comparing `funky_modifiers-0.3.1/LICENSE` & `funky_modifiers-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/setup.py` & `funky_modifiers-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.3.1',
+    version='0.3.2',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `funky_modifiers-0.3.1/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.3.2/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.3.2/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.3.2/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.3.2/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.3.2/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/modularity/logging.py` & `funky_modifiers-0.3.2/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.3.2/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/sorting/converters.py` & `funky_modifiers-0.3.2/src/funk_py/sorting/converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.3.2/src/funk_py/sorting/dict_manip.py`

 * *Files 1% similar despite different names*

```diff
@@ -719,14 +719,16 @@
             self._check_dict(other)
             self.__other = other
 
         if transformer is not ...:
             self._check_transformer(transformer)
             self.__transformer = transformer
 
+        return self
+
     def _check_dict(self,
                     other: Union[dict, 'DictBuilder._Cur', 'DictBuilder._Instruction']) -> dict:
         if type(other) is DictBuilder._Cur:
             return self.__builder
 
         elif type(other) is DictBuilder._Instruction:
             # Evaluate the instruction first to make sure it produces a dictionary.
```

### Comparing `funky_modifiers-0.3.1/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.3.2/src/funk_py/sorting/pieces.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.3.2/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.3.2/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.3.2/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.3.2/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.3.2/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_check_dict_equality.py` & `funky_modifiers-0.3.2/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_check_list_equality.py` & `funky_modifiers-0.3.2/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.3.2/test/test_convert_tuplish_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_converters.py` & `funky_modifiers-0.3.2/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_converts_enums.py` & `funky_modifiers-0.3.2/test/test_converts_enums.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_dict_builder.py` & `funky_modifiers-0.3.2/test/test_dict_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,19 +321,21 @@
 def test_use(base_dict1):
     def t_func(x):
         return {K1: str(x)}
 
     testy = DictBuilder()
     assert testy.other is None and testy.transformer is pass_, 'Not instantiated correctly.'
 
-    testy.use(other=base_dict1)
+    ans = testy.use(other=base_dict1)
     assert testy.other is base_dict1 and testy.transformer is pass_, 'Setting other failed.'
+    assert ans is testy
 
-    testy.use(transformer=t_func)
+    ans = testy.use(transformer=t_func)
     assert testy.other is base_dict1 and testy.transformer is t_func, 'Setting transformer failed.'
+    assert ans is testy
 
 TOP_LVL = 'top level'
 TOP_LVL_LST = 'top level (list)'
 NEW_TOP_LVL = 'new top level'
 NEW_TOP_LVL_LST = 'new top level (list)'
 NEW_1ST_2ND_LVL = 'new first and second level'
 NEW_2ND_LVL = 'new second level'
```

### Comparing `funky_modifiers-0.3.1/test/test_drop_none_dict.py` & `funky_modifiers-0.3.2/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_function_hash_and_equality.py` & `funky_modifiers-0.3.2/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_logs_vars.py` & `funky_modifiers-0.3.2/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_obj.py` & `funky_modifiers-0.3.2/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.3.1/test/test_pick.py` & `funky_modifiers-0.3.2/test/test_pick.py`

 * *Files identical despite different names*

