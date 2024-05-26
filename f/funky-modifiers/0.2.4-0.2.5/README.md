# Comparing `tmp/funky_modifiers-0.2.4.tar.gz` & `tmp/funky_modifiers-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.2.4.tar", last modified: Sun May 26 14:37:44 2024, max compression
+gzip compressed data, was "funky_modifiers-0.2.5.tar", last modified: Sun May 26 14:49:49 2024, max compression
```

## Comparing `funky_modifiers-0.2.4.tar` & `funky_modifiers-0.2.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 14:37:44.516785 funky_modifiers-0.2.4/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      483 2024-05-26 14:37:44.515793 funky_modifiers-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.2.4/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.2.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 14:37:44.516785 funky_modifiers-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-05-26 14:33:17.000000 funky_modifiers-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:37:44.487024 funky_modifiers-0.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 14:37:44.491489 funky_modifiers-0.2.4/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.2.4/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:37:44.494962 funky_modifiers-0.2.4/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.2.4/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.2.4/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.2.4/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:37:44.497444 funky_modifiers-0.2.4/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.2.4/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.2.4/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.2.4/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.2.4/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.2.4/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.2.4/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:37:44.499922 funky_modifiers-0.2.4/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.2.4/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.2.4/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    41055 2024-05-26 14:37:13.000000 funky_modifiers-0.2.4/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.2.4/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:37:44.502401 funky_modifiers-0.2.4/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.2.4/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.2.4/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.2.4/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.2.4/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-26 14:37:44.515297 funky_modifiers-0.2.4/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      483 2024-05-26 14:37:44.000000 funky_modifiers-0.2.4/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1285 2024-05-26 14:37:44.000000 funky_modifiers-0.2.4/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 14:37:44.000000 funky_modifiers-0.2.4/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-26 14:37:44.000000 funky_modifiers-0.2.4/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 14:37:44.000000 funky_modifiers-0.2.4/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-26 14:37:44.514305 funky_modifiers-0.2.4/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.2.4/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.2.4/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.2.4/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.2.4/test/test_converters.py
--rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.2.4/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    14746 2024-05-26 14:08:21.000000 funky_modifiers-0.2.4/test/test_dict_builder.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.2.4/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.2.4/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.2.4/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.2.4/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.2.4/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.415243 funky_modifiers-0.2.5/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      483 2024-05-26 14:49:49.414747 funky_modifiers-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.2.5/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:49:49.415739 funky_modifiers-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-05-26 14:49:05.000000 funky_modifiers-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.383994 funky_modifiers-0.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.388459 funky_modifiers-0.2.5/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.2.5/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.392924 funky_modifiers-0.2.5/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.2.5/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.2.5/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.2.5/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.395919 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.2.5/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.2.5/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.2.5/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.398877 funky_modifiers-0.2.5/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.2.5/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20576 2024-05-21 11:34:11.000000 funky_modifiers-0.2.5/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    41378 2024-05-26 14:46:58.000000 funky_modifiers-0.2.5/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.2.5/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.401355 funky_modifiers-0.2.5/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.2.5/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.2.5/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.2.5/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.2.5/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.414251 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      483 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 14:49:49.000000 funky_modifiers-0.2.5/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 14:49:49.413258 funky_modifiers-0.2.5/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.2.5/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.2.5/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.2.5/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.2.5/test/test_converters.py
+-rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.2.5/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    14746 2024-05-26 14:08:21.000000 funky_modifiers-0.2.5/test/test_dict_builder.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.2.5/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.2.5/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.2.5/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.2.5/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.2.5/test/test_pick.py
```

### Comparing `funky_modifiers-0.2.4/LICENSE` & `funky_modifiers-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/setup.py` & `funky_modifiers-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.2.4',
+    version='0.2.5',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `funky_modifiers-0.2.4/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.2.5/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.2.5/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.2.5/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.2.5/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.2.5/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/modularity/logging.py` & `funky_modifiers-0.2.5/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.2.5/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/sorting/converters.py` & `funky_modifiers-0.2.5/src/funk_py/sorting/converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.2.5/src/funk_py/sorting/dict_manip.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,34 +783,46 @@
                 if keys is not None:
                     k.extend(keys)
 
                 raise ValueError(f'Could not find key in other.\nkey={k}')
 
             return self
 
-        if not ((val_is_list and type(val) is list) or isinstance(transformer(val), dict)):
+        if not (val_is_list or isinstance(transformer(val), dict)):
             if unsafe:
                 main_logger.error(_NO_MERGE)
                 raise ValueError(_NO_MERGE)
 
             return self
 
         worker = self.__builder
         worker = self._update_seek(_as, worker, unsafe, classes)
         if val_is_list:
-            for _val in dive_to_dicts(val):
-                if not isinstance(t := transformer(_val), dict):
-                    if unsafe:
-                        main_logger.error(_NO_MERGE)
-                        raise ValueError(_NO_MERGE)
+            if isinstance(val, list):
+                for _val in dive_to_dicts(val):
+                    if not isinstance(t := transformer(_val), dict):
+                        if unsafe:
+                            main_logger.error(_NO_MERGE)
+                            raise ValueError(_NO_MERGE)
 
-                    continue
+                        continue
 
+                    worker.update(t)
+
+            elif not isinstance(t := transformer(val), dict):
+                if unsafe:
+                    main_logger.error(_NO_MERGE)
+                    raise ValueError(_NO_MERGE)
+
+                return self
+
+            else:
                 worker.update(t)
 
+
         else:
             worker.update(transformer(val))
 
         return self
 
     @staticmethod
     def _update_find_in_other(other: dict, key: Any, keys: List[Any], unsafe: bool = False):
```

### Comparing `funky_modifiers-0.2.4/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.2.5/src/funk_py/sorting/pieces.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.2.5/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.2.5/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.2.5/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.2.5/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.2.5/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_check_dict_equality.py` & `funky_modifiers-0.2.5/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_check_list_equality.py` & `funky_modifiers-0.2.5/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.2.5/test/test_convert_tuplish_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_converters.py` & `funky_modifiers-0.2.5/test/test_converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_converts_enums.py` & `funky_modifiers-0.2.5/test/test_converts_enums.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_dict_builder.py` & `funky_modifiers-0.2.5/test/test_dict_builder.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_drop_none_dict.py` & `funky_modifiers-0.2.5/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_function_hash_and_equality.py` & `funky_modifiers-0.2.5/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_logs_vars.py` & `funky_modifiers-0.2.5/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_obj.py` & `funky_modifiers-0.2.5/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.2.4/test/test_pick.py` & `funky_modifiers-0.2.5/test/test_pick.py`

 * *Files identical despite different names*

