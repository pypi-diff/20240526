# Comparing `tmp/yymake-0.8.5.tar.gz` & `tmp/yymake-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yymake-0.8.5.tar", last modified: Fri Apr  5 02:29:16 2024, max compression
+gzip compressed data, was "yymake-0.8.7.tar", last modified: Sun May 26 02:38:42 2024, max compression
```

## Comparing `yymake-0.8.5.tar` & `yymake-0.8.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-04-05 02:29:16.185274 yymake-0.8.5/
--rw-r--r--   0 evil       (501) staff       (20)     1067 2023-09-22 13:25:57.000000 yymake-0.8.5/LICENSE
--rw-r--r--   0 evil       (501) staff       (20)      886 2024-04-05 02:29:16.184400 yymake-0.8.5/PKG-INFO
--rw-r--r--   0 evil       (501) staff       (20)      279 2023-10-10 14:20:53.000000 yymake-0.8.5/README.md
--rw-r--r--   0 evil       (501) staff       (20)       38 2024-04-05 02:29:16.185440 yymake-0.8.5/setup.cfg
--rw-r--r--   0 evil       (501) staff       (20)     1112 2024-03-31 02:31:09.000000 yymake-0.8.5/setup.py
-drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-04-05 02:29:16.175643 yymake-0.8.5/ymake/
--rw-r--r--   0 evil       (501) staff       (20)        0 2023-09-29 15:05:14.000000 yymake-0.8.5/ymake/__init__.py
--rw-r--r--   0 evil       (501) staff       (20)     3186 2024-03-24 17:42:02.000000 yymake-0.8.5/ymake/automake.py
--rw-r--r--   0 evil       (501) staff       (20)    17474 2024-03-25 14:05:53.000000 yymake-0.8.5/ymake/builder.py
--rw-r--r--   0 evil       (501) staff       (20)      830 2023-09-29 15:57:02.000000 yymake-0.8.5/ymake/cmake.py
--rw-r--r--   0 evil       (501) staff       (20)     1091 2023-10-08 14:34:08.000000 yymake-0.8.5/ymake/detect.py
--rw-r--r--   0 evil       (501) staff       (20)    19584 2024-03-30 06:14:38.000000 yymake-0.8.5/ymake/function.py
--rw-r--r--   0 evil       (501) staff       (20)      333 2023-11-04 13:27:31.000000 yymake-0.8.5/ymake/globa.py
--rw-r--r--   0 evil       (501) staff       (20)     2615 2024-04-05 01:54:59.000000 yymake-0.8.5/ymake/graph.py
--rw-r--r--   0 evil       (501) staff       (20)     1057 2023-09-24 16:51:29.000000 yymake-0.8.5/ymake/log.py
--rw-r--r--   0 evil       (501) staff       (20)     8083 2024-03-31 02:30:02.000000 yymake-0.8.5/ymake/node.py
--rw-r--r--   0 evil       (501) staff       (20)     3575 2023-11-04 07:58:55.000000 yymake-0.8.5/ymake/op.py
--rw-r--r--   0 evil       (501) staff       (20)      400 2023-09-29 15:56:48.000000 yymake-0.8.5/ymake/toolchain.py
--rw-r--r--   0 evil       (501) staff       (20)      336 2023-09-29 15:19:38.000000 yymake-0.8.5/ymake/version.py
--rw-r--r--   0 evil       (501) staff       (20)    10868 2024-03-13 14:18:51.000000 yymake-0.8.5/ymake/yaya.py
-drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-04-05 02:29:16.183199 yymake-0.8.5/ymake/yymake.egg-info/
--rw-r--r--   0 evil       (501) staff       (20)      886 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/PKG-INFO
--rw-r--r--   0 evil       (501) staff       (20)      465 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/SOURCES.txt
--rw-r--r--   0 evil       (501) staff       (20)        1 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/dependency_links.txt
--rw-r--r--   0 evil       (501) staff       (20)       99 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/entry_points.txt
--rw-r--r--   0 evil       (501) staff       (20)       44 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/requires.txt
--rw-r--r--   0 evil       (501) staff       (20)        1 2024-04-05 02:29:16.000000 yymake-0.8.5/ymake/yymake.egg-info/top_level.txt
+drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-05-26 02:38:42.381530 yymake-0.8.7/
+-rw-r--r--   0 evil       (501) staff       (20)     1067 2023-09-22 13:25:57.000000 yymake-0.8.7/LICENSE
+-rw-r--r--   0 evil       (501) staff       (20)      886 2024-05-26 02:38:42.380494 yymake-0.8.7/PKG-INFO
+-rw-r--r--   0 evil       (501) staff       (20)      279 2023-10-10 14:20:53.000000 yymake-0.8.7/README.md
+-rw-r--r--   0 evil       (501) staff       (20)       38 2024-05-26 02:38:42.383727 yymake-0.8.7/setup.cfg
+-rw-r--r--   0 evil       (501) staff       (20)     1112 2024-05-26 02:38:32.000000 yymake-0.8.7/setup.py
+drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-05-26 02:38:42.371624 yymake-0.8.7/ymake/
+-rw-r--r--   0 evil       (501) staff       (20)        0 2023-09-29 15:05:14.000000 yymake-0.8.7/ymake/__init__.py
+-rw-r--r--   0 evil       (501) staff       (20)     3186 2024-03-24 17:42:02.000000 yymake-0.8.7/ymake/automake.py
+-rw-r--r--   0 evil       (501) staff       (20)    17474 2024-03-25 14:05:53.000000 yymake-0.8.7/ymake/builder.py
+-rw-r--r--   0 evil       (501) staff       (20)      830 2023-09-29 15:57:02.000000 yymake-0.8.7/ymake/cmake.py
+-rw-r--r--   0 evil       (501) staff       (20)     1091 2023-10-08 14:34:08.000000 yymake-0.8.7/ymake/detect.py
+-rw-r--r--   0 evil       (501) staff       (20)    19700 2024-04-05 04:05:54.000000 yymake-0.8.7/ymake/function.py
+-rw-r--r--   0 evil       (501) staff       (20)      333 2023-11-04 13:27:31.000000 yymake-0.8.7/ymake/globa.py
+-rw-r--r--   0 evil       (501) staff       (20)     2615 2024-04-05 01:54:59.000000 yymake-0.8.7/ymake/graph.py
+-rw-r--r--   0 evil       (501) staff       (20)     1057 2023-09-24 16:51:29.000000 yymake-0.8.7/ymake/log.py
+-rw-r--r--   0 evil       (501) staff       (20)     8140 2024-05-26 02:38:10.000000 yymake-0.8.7/ymake/node.py
+-rw-r--r--   0 evil       (501) staff       (20)     3575 2023-11-04 07:58:55.000000 yymake-0.8.7/ymake/op.py
+-rw-r--r--   0 evil       (501) staff       (20)      400 2023-09-29 15:56:48.000000 yymake-0.8.7/ymake/toolchain.py
+-rw-r--r--   0 evil       (501) staff       (20)      336 2023-09-29 15:19:38.000000 yymake-0.8.7/ymake/version.py
+-rw-r--r--   0 evil       (501) staff       (20)    11282 2024-05-05 15:15:37.000000 yymake-0.8.7/ymake/yaya.py
+drwxr-xr-x   0 evil       (501) staff       (20)        0 2024-05-26 02:38:42.379207 yymake-0.8.7/ymake/yymake.egg-info/
+-rw-r--r--   0 evil       (501) staff       (20)      886 2024-05-26 02:38:42.000000 yymake-0.8.7/ymake/yymake.egg-info/PKG-INFO
+-rw-r--r--   0 evil       (501) staff       (20)      465 2024-05-26 02:38:42.000000 yymake-0.8.7/ymake/yymake.egg-info/SOURCES.txt
+-rw-r--r--   0 evil       (501) staff       (20)        1 2024-05-26 02:38:42.000000 yymake-0.8.7/ymake/yymake.egg-info/dependency_links.txt
+-rw-r--r--   0 evil       (501) staff       (20)       99 2024-05-26 02:38:42.000000 yymake-0.8.7/ymake/yymake.egg-info/entry_points.txt
+-rw-r--r--   0 evil       (501) staff       (20)       44 2024-05-26 02:38:42.000000 yymake-0.8.7/ymake/yymake.egg-info/requires.txt
+-rw-r--r--   0 evil       (501) staff       (20)        1 2024-05-26 02:38:42.000000 yymake-0.8.7/ymake/yymake.egg-info/top_level.txt
```

### Comparing `yymake-0.8.5/LICENSE` & `yymake-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yymake-0.8.5/PKG-INFO` & `yymake-0.8.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yymake
-Version: 0.8.5
+Version: 0.8.7
 Summary: A cross build dsl make tool
 Home-page: https://github.com/evilbinary/ymake
 Author: evilbinary
 Author-email: rootntsd@gmail.com
 Project-URL: Bug Tracker, https://github.com/evilbinary/ymake/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yymake-0.8.5/setup.py` & `yymake-0.8.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 import os,sys,re
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="yymake",
-    version="0.8.5",
+    version="0.8.7",
     author="evilbinary",
     author_email="rootntsd@gmail.com",
     description="A cross build dsl make tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/evilbinary/ymake",
     project_urls={
```

### Comparing `yymake-0.8.5/ymake/automake.py` & `yymake-0.8.7/ymake/automake.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.5/ymake/builder.py` & `yymake-0.8.7/ymake/builder.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.5/ymake/cmake.py` & `yymake-0.8.7/ymake/cmake.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.5/ymake/detect.py` & `yymake-0.8.7/ymake/detect.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.5/ymake/function.py` & `yymake-0.8.7/ymake/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,27 +120,29 @@
 
     files = kwargs.pop('files', [])
     if len(files)>0:
         add_files(files[0])
 
 def toolchain(name, **kwargs):
     prefix=kwargs.pop('prefix','')
+    suffix=kwargs.pop('suffix','')
     node = {
         'name': name,
         'type':'toolchain',
-        'cc': prefix+'gcc',
-        'cxx': prefix+'c++',
-        'ld': prefix+'ld',
-        'ar': prefix+'ar',
-        'as': prefix+'as',
-        'objcopy': prefix+'objcopy',
-        'sh': prefix+'gcc',
-        'ranlib': prefix+'ranlib',
+        'cc': prefix+'gcc'+suffix,
+        'cxx': prefix+'c++'+suffix,
+        'ld': prefix+'ld'+suffix,
+        'ar': prefix+'ar'+suffix,
+        'as': prefix+'as'+suffix,
+        'objcopy': prefix+'objcopy'+suffix,
+        'sh': prefix+'gcc'+suffix,
+        'ranlib': prefix+'ranlib'+suffix,
         'is_modify': is_file_modified,
         'prefix': prefix,
+        'suffix': suffix
     }
     node.update(kwargs)
     node_start(node)
 
 def option(name,**kwargs):
     node=nodes_get_type_and_name('option',name)
     if not node:
```

### Comparing `yymake-0.8.5/ymake/graph.py` & `yymake-0.8.7/ymake/graph.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.5/ymake/log.py` & `yymake-0.8.7/ymake/log.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.5/ymake/node.py` & `yymake-0.8.7/ymake/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,16 @@
 
 def node_update(data):
     n=node_current()
     return n.update(data)
 
 def node_extend(key,value,t=1):
     n=node_current()
+    if not isinstance(value,list):
+        value=[value]
     return node_op_extend(n,key,value,t)
 
 def node_op_extend(n,key,value,tail=True,nodup=False):
     if not n.get(key):       
         # caller_frame = inspect.currentframe().f_back
         # caller_file_path = inspect.getframeinfo(caller_frame)
         # print('call==>',caller_file_path)
```

### Comparing `yymake-0.8.5/ymake/op.py` & `yymake-0.8.7/ymake/op.py`

 * *Files identical despite different names*

### Comparing `yymake-0.8.5/ymake/yaya.py` & `yymake-0.8.7/ymake/yaya.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,15 +249,15 @@
     root('root')
     add_toolchain_dirs('toolchains')
     
     # 默认工具
     toolchain('gcc',build=gcc_build,build_prepare=build_prepare)
     if platform.system()=='Darwin':
         add_ldflags('-lSystem')
-        add_ldflags('-arch', platform.machine())
+        #add_ldflags('-arch', platform.machine())
     elif platform.system()=='Linux':
         add_ldflags('-lc')
         cur=node_current()
         prefix= cur.get('prefix')
         set_toolset('ld',prefix+'gcc')
 
     toolchain('arm-none-eabi',
@@ -277,14 +277,31 @@
         clean=gcc_clean)
     toolchain('i686-elf',
         prefix='i686-elf-',
         build=gcc_build,
         build_prepare=build_prepare,
         clean=gcc_clean)
 
+    toolchain('gcc-13',
+    prefix='gcc-',
+    suffix='-13',
+    build=gcc_build,build_prepare=build_prepare)
+    add_ldflags('-lc')
+    cur=node_current()
+    prefix= cur.get('prefix')
+    set_toolset('ld',prefix+'')
+    set_toolset('cc','gcc-13')
+
+    toolchain('aarch64-none-elf',
+        prefix='aarch64-none-elf-',
+        build=gcc_build,
+        build_prepare=build_prepare,
+        clean=gcc_clean)
+    
+
     toolchains_init()
     toolchain_end()
 
 
     rule('mode.debug')
     def build_config(target):
         if is_mode("debug"):
```

### Comparing `yymake-0.8.5/ymake/yymake.egg-info/PKG-INFO` & `yymake-0.8.7/ymake/yymake.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yymake
-Version: 0.8.5
+Version: 0.8.7
 Summary: A cross build dsl make tool
 Home-page: https://github.com/evilbinary/ymake
 Author: evilbinary
 Author-email: rootntsd@gmail.com
 Project-URL: Bug Tracker, https://github.com/evilbinary/ymake/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

