# Comparing `tmp/bragi-0.5.tar.gz` & `tmp/bragi-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bragi-0.5.tar", last modified: Tue Apr  4 19:29:41 2023, max compression
+gzip compressed data, was "bragi-0.6.tar", last modified: Sun May 26 19:21:28 2024, max compression
```

## Comparing `bragi-0.5.tar` & `bragi-0.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.942680 bragi-0.5/
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.936013 bragi-0.5/.github/
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/.github/workflows/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      841 2023-04-04 19:19:40.000000 bragi-0.5/.github/workflows/ci.yml
--rw-r--r--   0 qookie    (1000) qookie    (1000)      166 2023-04-04 19:29:41.942680 bragi-0.5/PKG-INFO
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/bin/
--rwxr-xr-x   0 qookie    (1000) qookie    (1000)      959 2023-04-04 19:19:40.000000 bragi-0.5/bin/bragi
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/bragi/
--rw-r--r--   0 qookie    (1000) qookie    (1000)       22 2023-04-04 19:19:40.000000 bragi-0.5/bragi/__init__.py
--rw-r--r--   0 qookie    (1000) qookie    (1000)    37534 2023-04-04 19:19:40.000000 bragi-0.5/bragi/cpp_generator.py
--rw-r--r--   0 qookie    (1000) qookie    (1000)    14265 2023-04-04 19:19:40.000000 bragi-0.5/bragi/parser.py
--rw-r--r--   0 qookie    (1000) qookie    (1000)     3657 2023-04-04 19:19:40.000000 bragi-0.5/bragi/tokens.py
--rw-r--r--   0 qookie    (1000) qookie    (1000)     2871 2023-04-04 19:19:40.000000 bragi-0.5/bragi/types.py
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/bragi.egg-info/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      166 2023-04-04 19:29:41.000000 bragi-0.5/bragi.egg-info/PKG-INFO
--rw-r--r--   0 qookie    (1000) qookie    (1000)      918 2023-04-04 19:29:41.000000 bragi-0.5/bragi.egg-info/SOURCES.txt
--rw-r--r--   0 qookie    (1000) qookie    (1000)        1 2023-04-04 19:29:41.000000 bragi-0.5/bragi.egg-info/dependency_links.txt
--rw-r--r--   0 qookie    (1000) qookie    (1000)       12 2023-04-04 19:29:41.000000 bragi-0.5/bragi.egg-info/requires.txt
--rw-r--r--   0 qookie    (1000) qookie    (1000)        6 2023-04-04 19:29:41.000000 bragi-0.5/bragi.egg-info/top_level.txt
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.936013 bragi-0.5/include/
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/include/bragi/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      772 2023-04-04 19:19:40.000000 bragi-0.5/include/bragi/helpers-all.hpp
--rw-r--r--   0 qookie    (1000) qookie    (1000)     1363 2023-04-04 19:19:40.000000 bragi-0.5/include/bragi/helpers-frigg.hpp
--rw-r--r--   0 qookie    (1000) qookie    (1000)      925 2023-04-04 19:19:40.000000 bragi-0.5/include/bragi/helpers-std.hpp
--rw-r--r--   0 qookie    (1000) qookie    (1000)     4264 2023-04-04 19:19:40.000000 bragi-0.5/include/bragi/internals.hpp
--rw-r--r--   0 qookie    (1000) qookie    (1000)      438 2023-04-04 19:19:40.000000 bragi-0.5/meson.build
--rw-r--r--   0 qookie    (1000) qookie    (1000)      109 2023-04-04 19:19:40.000000 bragi-0.5/meson_options.txt
--rw-r--r--   0 qookie    (1000) qookie    (1000)       38 2023-04-04 19:29:41.942680 bragi-0.5/setup.cfg
--rwxr-xr-x   0 qookie    (1000) qookie    (1000)      408 2023-04-04 19:20:06.000000 bragi-0.5/setup.py
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/subprojects/
--rw-r--r--   0 qookie    (1000) qookie    (1000)       91 2023-04-04 19:19:40.000000 bragi-0.5/subprojects/frigg.wrap
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/tests/
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/tests/arrays/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      252 2023-04-04 19:19:40.000000 bragi-0.5/tests/arrays/arrays.bragi
--rw-r--r--   0 qookie    (1000) qookie    (1000)     5037 2023-04-04 19:19:40.000000 bragi-0.5/tests/arrays/arrays.cpp
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/tests/basic/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      133 2023-04-04 19:19:40.000000 bragi-0.5/tests/basic/basic.bragi
--rw-r--r--   0 qookie    (1000) qookie    (1000)      912 2023-04-04 19:19:40.000000 bragi-0.5/tests/basic/basic.cpp
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/tests/empty/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      210 2023-04-04 19:19:40.000000 bragi-0.5/tests/empty/empty.bragi
--rw-r--r--   0 qookie    (1000) qookie    (1000)     2211 2023-04-04 19:19:40.000000 bragi-0.5/tests/empty/empty.cpp
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/tests/enums/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      183 2023-04-04 19:19:40.000000 bragi-0.5/tests/enums/enums.bragi
--rw-r--r--   0 qookie    (1000) qookie    (1000)     1321 2023-04-04 19:19:40.000000 bragi-0.5/tests/enums/enums.cpp
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.942680 bragi-0.5/tests/group/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      121 2023-04-04 19:19:40.000000 bragi-0.5/tests/group/group.bragi
--rw-r--r--   0 qookie    (1000) qookie    (1000)      318 2023-04-04 19:19:40.000000 bragi-0.5/tests/group/group.cpp
--rw-r--r--   0 qookie    (1000) qookie    (1000)      975 2023-04-04 19:19:40.000000 bragi-0.5/tests/meson.build
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.942680 bragi-0.5/tests/preamble/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      104 2023-04-04 19:19:40.000000 bragi-0.5/tests/preamble/preamble.bragi
--rw-r--r--   0 qookie    (1000) qookie    (1000)     1656 2023-04-04 19:19:40.000000 bragi-0.5/tests/preamble/preamble.cpp
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.942680 bragi-0.5/tests/struct/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      265 2023-04-04 19:19:40.000000 bragi-0.5/tests/struct/struct.bragi
--rw-r--r--   0 qookie    (1000) qookie    (1000)     3222 2023-04-04 19:19:40.000000 bragi-0.5/tests/struct/struct.cpp
--rw-r--r--   0 qookie    (1000) qookie    (1000)     1901 2023-04-04 19:24:17.000000 bragi-0.5/tests/test-util.hpp
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.942680 bragi-0.5/tests/using/
--rw-r--r--   0 qookie    (1000) qookie    (1000)      129 2023-04-04 19:19:40.000000 bragi-0.5/tests/using/using.bragi
--rw-r--r--   0 qookie    (1000) qookie    (1000)      464 2023-04-04 19:19:40.000000 bragi-0.5/tests/using/using.cpp
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.939346 bragi-0.5/vim/
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.942680 bragi-0.5/vim/ftdetect/
--rw-r--r--   0 qookie    (1000) qookie    (1000)       49 2023-04-04 19:19:40.000000 bragi-0.5/vim/ftdetect/bragi.vim
-drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2023-04-04 19:29:41.942680 bragi-0.5/vim/syntax/
--rw-r--r--   0 qookie    (1000) qookie    (1000)     1480 2023-04-04 19:19:40.000000 bragi-0.5/vim/syntax/bragi.vim
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.860377 bragi-0.6/
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.850377 bragi-0.6/.github/
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.853710 bragi-0.6/.github/workflows/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      841 2023-04-04 19:19:40.000000 bragi-0.6/.github/workflows/ci.yml
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      193 2024-05-26 19:21:28.860377 bragi-0.6/PKG-INFO
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.853710 bragi-0.6/bin/
+-rwxr-xr-x   0 qookie    (1000) qookie    (1000)      959 2023-04-04 19:19:40.000000 bragi-0.6/bin/bragi
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.853710 bragi-0.6/bragi/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)       22 2023-04-04 19:19:40.000000 bragi-0.6/bragi/__init__.py
+-rw-r--r--   0 qookie    (1000) qookie    (1000)    37820 2024-05-26 19:00:59.000000 bragi-0.6/bragi/cpp_generator.py
+-rw-r--r--   0 qookie    (1000) qookie    (1000)    14265 2023-04-04 19:19:40.000000 bragi-0.6/bragi/parser.py
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     3657 2023-04-04 19:19:40.000000 bragi-0.6/bragi/tokens.py
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     2871 2023-04-04 19:19:40.000000 bragi-0.6/bragi/types.py
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.860377 bragi-0.6/bragi.egg-info/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      193 2024-05-26 19:21:28.000000 bragi-0.6/bragi.egg-info/PKG-INFO
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      918 2024-05-26 19:21:28.000000 bragi-0.6/bragi.egg-info/SOURCES.txt
+-rw-r--r--   0 qookie    (1000) qookie    (1000)        1 2024-05-26 19:21:28.000000 bragi-0.6/bragi.egg-info/dependency_links.txt
+-rw-r--r--   0 qookie    (1000) qookie    (1000)       12 2024-05-26 19:21:28.000000 bragi-0.6/bragi.egg-info/requires.txt
+-rw-r--r--   0 qookie    (1000) qookie    (1000)        6 2024-05-26 19:21:28.000000 bragi-0.6/bragi.egg-info/top_level.txt
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.850377 bragi-0.6/include/
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/include/bragi/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      772 2023-04-04 19:19:40.000000 bragi-0.6/include/bragi/helpers-all.hpp
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     1363 2023-04-04 19:19:40.000000 bragi-0.6/include/bragi/helpers-frigg.hpp
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      925 2023-04-04 19:19:40.000000 bragi-0.6/include/bragi/helpers-std.hpp
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     4264 2023-04-04 19:19:40.000000 bragi-0.6/include/bragi/internals.hpp
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      438 2023-04-04 19:19:40.000000 bragi-0.6/meson.build
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      109 2023-04-04 19:19:40.000000 bragi-0.6/meson_options.txt
+-rw-r--r--   0 qookie    (1000) qookie    (1000)       38 2024-05-26 19:21:28.860377 bragi-0.6/setup.cfg
+-rwxr-xr-x   0 qookie    (1000) qookie    (1000)      408 2024-05-26 19:01:22.000000 bragi-0.6/setup.py
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/subprojects/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)       91 2023-04-04 19:19:40.000000 bragi-0.6/subprojects/frigg.wrap
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/tests/
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/tests/arrays/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      252 2023-04-04 19:19:40.000000 bragi-0.6/tests/arrays/arrays.bragi
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     4826 2024-05-26 19:00:59.000000 bragi-0.6/tests/arrays/arrays.cpp
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/tests/basic/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      133 2023-04-04 19:19:40.000000 bragi-0.6/tests/basic/basic.bragi
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      912 2023-04-04 19:19:40.000000 bragi-0.6/tests/basic/basic.cpp
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/tests/empty/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      210 2023-04-04 19:19:40.000000 bragi-0.6/tests/empty/empty.bragi
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     2211 2023-04-04 19:19:40.000000 bragi-0.6/tests/empty/empty.cpp
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/tests/enums/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      183 2023-04-04 19:19:40.000000 bragi-0.6/tests/enums/enums.bragi
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     1313 2024-05-26 19:00:59.000000 bragi-0.6/tests/enums/enums.cpp
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/tests/group/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      121 2023-04-04 19:19:40.000000 bragi-0.6/tests/group/group.bragi
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      318 2023-04-04 19:19:40.000000 bragi-0.6/tests/group/group.cpp
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      975 2023-04-04 19:19:40.000000 bragi-0.6/tests/meson.build
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/tests/preamble/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      104 2023-04-04 19:19:40.000000 bragi-0.6/tests/preamble/preamble.bragi
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     1656 2023-04-04 19:19:40.000000 bragi-0.6/tests/preamble/preamble.cpp
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.857044 bragi-0.6/tests/struct/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      265 2023-04-04 19:19:40.000000 bragi-0.6/tests/struct/struct.bragi
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     3222 2023-04-04 19:19:40.000000 bragi-0.6/tests/struct/struct.cpp
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     1706 2024-05-26 19:00:59.000000 bragi-0.6/tests/test-util.hpp
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.860377 bragi-0.6/tests/using/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      129 2023-04-04 19:19:40.000000 bragi-0.6/tests/using/using.bragi
+-rw-r--r--   0 qookie    (1000) qookie    (1000)      464 2023-04-04 19:19:40.000000 bragi-0.6/tests/using/using.cpp
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.853710 bragi-0.6/vim/
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.860377 bragi-0.6/vim/ftdetect/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)       49 2023-04-04 19:19:40.000000 bragi-0.6/vim/ftdetect/bragi.vim
+drwxr-xr-x   0 qookie    (1000) qookie    (1000)        0 2024-05-26 19:21:28.860377 bragi-0.6/vim/syntax/
+-rw-r--r--   0 qookie    (1000) qookie    (1000)     1480 2023-04-04 19:19:40.000000 bragi-0.6/vim/syntax/bragi.vim
```

### Comparing `bragi-0.5/.github/workflows/ci.yml` & `bragi-0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bragi-0.5/bin/bragi` & `bragi-0.6/bin/bragi`

 * *Files identical despite different names*

### Comparing `bragi-0.5/bragi/cpp_generator.py` & `bragi-0.6/bragi/cpp_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,38 +4,42 @@
 class StdlibTraits:
     def needs_allocator(self):
         return False
     def allocator_argument(self):
         return ''
     def allocator_parameter(self):
         return ''
+    def array(self):
+        return 'std::array'
     def vector(self):
         return 'std::vector'
     def string(self):
         return 'std::string'
     def assert_func(self):
         return 'assert'
     def includes(self):
-        return ['<stdint.h>', '<stddef.h>', '<vector>', '<cassert>', '<optional>', '<string>']
+        return ['<stdint.h>', '<stddef.h>', '<array>', '<vector>', '<cassert>', '<optional>', '<string>']
 
 class FriggTraits:
     def needs_allocator(self):
         return True
     def allocator_argument(self):
         return 'Allocator allocator = Allocator()'
     def allocator_parameter(self):
         return 'allocator'
+    def array(self):
+        return 'std::array'
     def vector(self):
         return 'frg::vector'
     def string(self):
         return 'frg::string'
     def assert_func(self):
         return 'FRG_ASSERT'
     def includes(self):
-        return ['<stdint.h>', '<stddef.h>', '<frg/vector.hpp>', '<frg/macros.hpp>', '<frg/optional.hpp>', '<frg/string.hpp>']
+        return ['<stdint.h>', '<stddef.h>', '<array>', '<frg/vector.hpp>', '<frg/macros.hpp>', '<frg/optional.hpp>', '<frg/string.hpp>']
 
 flatten = lambda l: [item for sublist in l for item in sublist]
 
 class CodeGenerator:
     def __init__(self, unit, stdlib, protobuf_compat = False):
         self.unit = unit
         self.protobuf_compat = protobuf_compat
@@ -182,14 +186,17 @@
                 out += f'{self.indent}using {to_name} = {from_full}<Allocator>;\n\n'
             else:
                 out += f'{self.indent}using {to_name} = {from_full};\n\n'
 
             return out
 
     def check_needs_allocator(self, t):
+        if t.identity is TypeIdentity.ARRAY and t.n_elements is not None:
+            return False
+
         return (t.identity in [TypeIdentity.STRING, TypeIdentity.ARRAY, TypeIdentity.STRUCT]
                 or t.dynamic) and self.stdlib_traits.needs_allocator()
 
     def generate_type(self, t):
         if t.identity is TypeIdentity.INTEGER:
             if t.name == 'char':
                 return 'char'
@@ -197,15 +204,18 @@
         elif t.identity is TypeIdentity.CONSTS:
             return self.generate_type(t.subtype)
         elif t.identity is TypeIdentity.ENUM:
             return t.name
         elif t.identity is TypeIdentity.STRING:
             return f'{self.stdlib_traits.string()}{"<Allocator>" if self.stdlib_traits.needs_allocator() else ""}'
         elif t.identity is TypeIdentity.ARRAY:
-            return f'{self.stdlib_traits.vector()}<{self.generate_type(t.subtype)}{", Allocator" if self.stdlib_traits.needs_allocator() else ""}>'
+            if t.n_elements is None:
+                return f'{self.stdlib_traits.vector()}<{self.generate_type(t.subtype)}{", Allocator" if self.stdlib_traits.needs_allocator() else ""}>'
+            else:
+                return f'{self.stdlib_traits.array()}<{self.generate_type(t.subtype)}, {t.n_elements}>'
         elif t.identity is TypeIdentity.STRUCT:
             return f'{t.name}{"<Allocator>" if self.stdlib_traits.needs_allocator() else ""}'
         else:
             raise RuntimeError('unknown type in generate_type')
 
     def is_simple_integer(self, t):
         return t in ['char', 'int8_t', 'uint8_t', 'int16_t', 'uint16_t', 'int32_t', 'uint32_t', 'int64_t', 'uint64_t']
@@ -558,19 +568,14 @@
                 return out
             elif expr_type.identity is TypeIdentity.ARRAY:
                 assert not expr_type.subtype.dynamic
                 assert expr_type.n_elements
 
                 out = ''
 
-                if self.parent.check_needs_allocator(expr_type.subtype):
-                    out = f'{self.parent.indent}{expr}.resize({expr_type.n_elements}, allocator);\n'
-                else:
-                    out = f'{self.parent.indent}{expr}.resize({expr_type.n_elements});\n'
-
                 out += f'{self.parent.indent}for (size_t i{array_depth} = 0; i{array_depth} < {expr_type.n_elements}; i{array_depth}++) {{\n'
                 self.parent.enter_indent()
                 out += self.emit_decode_fixed_internal(f'{expr}[i{array_depth}]', expr_type.subtype, array_depth + 1)
                 self.parent.leave_indent()
                 out += f'{self.parent.indent}}}\n'
 
                 return out
@@ -638,18 +643,19 @@
                 out += self.parent.emit_stmt_checked(f'de.read_varint(rd, size)')
 
                 target_size = 'size'
 
                 if expr_type.identity is TypeIdentity.ARRAY and expr_type.n_elements:
                     target_size = expr_type.n_elements
 
-                if self.parent.check_needs_allocator(expr_type.subtype):
-                    out += f'{self.parent.indent}{expr}.resize({target_size}, allocator);\n'
-                else:
-                    out += f'{self.parent.indent}{expr}.resize({target_size});\n'
+                if not (expr_type.identity is TypeIdentity.ARRAY and expr_type.n_elements is not None):
+                    if self.parent.check_needs_allocator(expr_type.subtype):
+                        out += f'{self.parent.indent}{expr}.resize({target_size}, allocator);\n'
+                    else:
+                        out += f'{self.parent.indent}{expr}.resize({target_size});\n'
                 out += f'{self.parent.indent}for (size_t i{array_depth} = 0; i{array_depth} < {target_size}; i{array_depth}++)\n'
                 if target_size != 'size':
                     self.parent.enter_indent()
                     out += f'{self.parent.indent}if (i{array_depth} < size)\n'
 
                 self.parent.enter_indent()
                 out += self.emit_decode_dynamic_internal(f'{expr}[i{array_depth}]', expr_type.subtype, array_depth + 1)
@@ -812,20 +818,21 @@
                 out += f'{self.indent}void set_{m.name}(size_t i, {self.generate_type(m.type.subtype)} val) {{\n'
                 self.enter_indent()
                 out += f'{self.indent}p_{m.name} = true;\n'
                 out += f'{self.indent}m_{m.name}[i] = val;\n'
                 self.leave_indent()
                 out += f'{self.indent}}}\n\n'
 
-                out += f'{self.indent}void add_{m.name}({self.generate_type(m.type.subtype)} v) {{\n'
-                self.enter_indent()
-                out += f'{self.indent}p_{m.name} = true;\n'
-                out += f'{self.indent}m_{m.name}.push_back(v);\n'
-                self.leave_indent()
-                out += f'{self.indent}}}\n\n'
+                if m.type.n_elements is None:
+                    out += f'{self.indent}void add_{m.name}({self.generate_type(m.type.subtype)} v) {{\n'
+                    self.enter_indent()
+                    out += f'{self.indent}p_{m.name} = true;\n'
+                    out += f'{self.indent}m_{m.name}.push_back(v);\n'
+                    self.leave_indent()
+                    out += f'{self.indent}}}\n\n'
 
         return out
 
     def emit_constructor(self, name, members):
         out = f'{self.indent}{name}({self.stdlib_traits.allocator_argument()})'
 
         if len(members) > 0 or self.stdlib_traits.needs_allocator():
```

### Comparing `bragi-0.5/bragi/parser.py` & `bragi-0.6/bragi/parser.py`

 * *Files identical despite different names*

### Comparing `bragi-0.5/bragi/tokens.py` & `bragi-0.6/bragi/tokens.py`

 * *Files identical despite different names*

### Comparing `bragi-0.5/bragi/types.py` & `bragi-0.6/bragi/types.py`

 * *Files identical despite different names*

### Comparing `bragi-0.5/bragi.egg-info/SOURCES.txt` & `bragi-0.6/bragi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bragi-0.5/include/bragi/helpers-all.hpp` & `bragi-0.6/include/bragi/helpers-all.hpp`

 * *Files identical despite different names*

### Comparing `bragi-0.5/include/bragi/helpers-frigg.hpp` & `bragi-0.6/include/bragi/helpers-frigg.hpp`

 * *Files identical despite different names*

### Comparing `bragi-0.5/include/bragi/helpers-std.hpp` & `bragi-0.6/include/bragi/helpers-std.hpp`

 * *Files identical despite different names*

### Comparing `bragi-0.5/include/bragi/internals.hpp` & `bragi-0.6/include/bragi/internals.hpp`

 * *Files identical despite different names*

### Comparing `bragi-0.5/tests/basic/basic.cpp` & `bragi-0.6/tests/basic/basic.cpp`

 * *Files identical despite different names*

### Comparing `bragi-0.5/tests/empty/empty.cpp` & `bragi-0.6/tests/empty/empty.cpp`

 * *Files identical despite different names*

### Comparing `bragi-0.5/tests/enums/enums.cpp` & `bragi-0.6/tests/enums/enums.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 int main() {
 	auto t1 = test::make_msg<Test>();
 	t1.set_foo(Foo::D);
 	t1.set_bar(Bar::E);
 
 	t1.set_foos(test::make_vector<Foo>(Foo::D, Foo::A, Foo::F, Foo::B));
-	t1.set_bars(test::make_vector<uint8_t>(Bar::E, Bar::B, Bar::A, Bar::C));
+	t1.set_bars(std::array<uint8_t, 4>{Bar::E, Bar::B, Bar::A, Bar::C});
 
 	assert(bragi::message_id<Test> == 1);
 	assert(bragi::head_size<Test> == 128);
 	assert(t1.size_of_tail() == 0);
 
 	assert(static_cast<int32_t>(Foo::A) == 1);
 	assert(static_cast<int32_t>(Foo::B) == 2);
@@ -44,10 +44,10 @@
 
 	assert(t2->foo() == Foo::D);
 	assert(t2->bar() == Bar::E);
 
 	auto foos = test::make_vector<Foo>(Foo::D, Foo::A, Foo::F, Foo::B);
 	assert(t2->foos() == foos);
 
-	auto bars = test::make_vector<uint8_t>(Bar::E, Bar::B, Bar::A, Bar::C);
+	auto bars = std::array<uint8_t, 4>{Bar::E, Bar::B, Bar::A, Bar::C};
 	assert(t2->bars() == bars);
 }
```

### Comparing `bragi-0.5/tests/meson.build` & `bragi-0.6/tests/meson.build`

 * *Files identical despite different names*

### Comparing `bragi-0.5/tests/preamble/preamble.cpp` & `bragi-0.6/tests/preamble/preamble.cpp`

 * *Files identical despite different names*

### Comparing `bragi-0.5/tests/struct/struct.cpp` & `bragi-0.6/tests/struct/struct.cpp`

 * *Files identical despite different names*

### Comparing `bragi-0.5/tests/test-util.hpp` & `bragi-0.6/tests/test-util.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -14,72 +14,64 @@
 #include <string>
 #endif
 
 namespace test {
 
 #ifdef TEST_FRIGG
 
-struct test_allocator {
-	test_allocator(int) {}
-
-	void *allocate(size_t sz) { return operator new(sz); }
-	void free(void *ptr) { operator delete(ptr); }
-	void deallocate(void *ptr, size_t sz) { operator delete(ptr, sz); }
-};
-
 template <typename T>
-using vec_of = frg::vector<T, test_allocator>;
+using vec_of = frg::vector<T, frg::stl_allocator>;
 
 #else
 
 template <typename T>
 using vec_of = std::vector<T>;
 
 #endif
 
 template <typename T, typename ...Ts>
 auto make_vector(Ts ...ts) {
 #ifdef TEST_FRIGG
-	frg::vector<T, test_allocator> vec{test_allocator{1}};
+	frg::vector<T, frg::stl_allocator> vec{frg::stl_allocator{}};
 
 	(vec.push_back(static_cast<T>(ts)), ...);
 
 	return vec;
 #else
 	return std::vector<T>{static_cast<T>(ts)...};
 #endif
 }
 
 auto make_string(const char *str) {
 #ifdef TEST_FRIGG
-	return frg::string<test_allocator>{str, test_allocator{1}};
+	return frg::string<frg::stl_allocator>{str, frg::stl_allocator{}};
 #else
 	return std::string{str};
 #endif
 }
 
 #ifdef TEST_FRIGG
 template <template<typename...> typename Msg>
 auto make_msg() {
-	return Msg<test_allocator>{test_allocator{1}};
+	return Msg<frg::stl_allocator>{frg::stl_allocator{}};
 }
 #else
 template <typename Msg>
 auto make_msg() {
 	return Msg{};
 }
 #endif
 
 #ifdef TEST_FRIGG
 template <template<typename...> typename Msg, typename ...Ts>
 auto parse_with(Ts &&...ts) {
 	if constexpr (sizeof...(ts) == 2)
-		return bragi::parse_head_tail<Msg>(std::forward<Ts>(ts)..., test_allocator{1});
+		return bragi::parse_head_tail<Msg>(std::forward<Ts>(ts)..., frg::stl_allocator{});
 	else
-		return bragi::parse_head_only<Msg>(std::forward<Ts>(ts)..., test_allocator{1});
+		return bragi::parse_head_only<Msg>(std::forward<Ts>(ts)..., frg::stl_allocator{});
 }
 #else
 template <typename Msg, typename ...Ts>
 auto parse_with(Ts &&...ts) {
 	if constexpr (sizeof...(ts) == 2)
 		return bragi::parse_head_tail<Msg>(std::forward<Ts>(ts)...);
 	else
```

### Comparing `bragi-0.5/vim/syntax/bragi.vim` & `bragi-0.6/vim/syntax/bragi.vim`

 * *Files identical despite different names*

