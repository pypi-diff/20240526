# Comparing `tmp/causal_conv1d-1.2.0.post2.tar.gz` & `tmp/causal_conv1d-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_conv1d-1.2.0.post2.tar", last modified: Sat Mar  2 08:34:25 2024, max compression
+gzip compressed data, was "causal_conv1d-1.2.1.tar", last modified: Sun May 26 19:21:04 2024, max compression
```

## Comparing `causal_conv1d-1.2.0.post2.tar` & `causal_conv1d-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 08:34:25.440474 causal_conv1d-1.2.0.post2/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-02 08:33:58.000000 causal_conv1d-1.2.0.post2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-02 08:33:58.000000 causal_conv1d-1.2.0.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-02 08:34:25.440474 causal_conv1d-1.2.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-02 08:33:58.000000 causal_conv1d-1.2.0.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 08:34:25.436474 causal_conv1d-1.2.0.post2/causal_conv1d/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-02 08:33:58.000000 causal_conv1d-1.2.0.post2/causal_conv1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-03-02 08:33:58.000000 causal_conv1d-1.2.0.post2/causal_conv1d/causal_conv1d_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 08:34:25.440474 causal_conv1d-1.2.0.post2/causal_conv1d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-02 08:34:25.000000 causal_conv1d-1.2.0.post2/causal_conv1d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-02 08:34:25.000000 causal_conv1d-1.2.0.post2/causal_conv1d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 08:34:25.000000 causal_conv1d-1.2.0.post2/causal_conv1d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-02 08:34:25.000000 causal_conv1d-1.2.0.post2/causal_conv1d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-02 08:34:25.000000 causal_conv1d-1.2.0.post2/causal_conv1d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 08:34:25.440474 causal_conv1d-1.2.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-03-02 08:33:58.000000 causal_conv1d-1.2.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:21:04.262669 causal_conv1d-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 19:20:30.000000 causal_conv1d-1.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-26 19:20:30.000000 causal_conv1d-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-26 19:21:04.262669 causal_conv1d-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-26 19:20:30.000000 causal_conv1d-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:21:04.258669 causal_conv1d-1.2.1/causal_conv1d/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-26 19:20:30.000000 causal_conv1d-1.2.1/causal_conv1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-26 19:20:30.000000 causal_conv1d-1.2.1/causal_conv1d/causal_conv1d_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:21:04.262669 causal_conv1d-1.2.1/causal_conv1d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-26 19:21:04.000000 causal_conv1d-1.2.1/causal_conv1d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-26 19:21:04.000000 causal_conv1d-1.2.1/causal_conv1d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:21:04.000000 causal_conv1d-1.2.1/causal_conv1d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 19:21:04.000000 causal_conv1d-1.2.1/causal_conv1d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 19:21:04.000000 causal_conv1d-1.2.1/causal_conv1d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 19:21:04.262669 causal_conv1d-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-05-26 19:20:30.000000 causal_conv1d-1.2.1/setup.py
```

### Comparing `causal_conv1d-1.2.0.post2/LICENSE` & `causal_conv1d-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_conv1d-1.2.0.post2/PKG-INFO` & `causal_conv1d-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal_conv1d
-Version: 1.2.0.post2
+Version: 1.2.1
 Summary: Causal depthwise conv1d in CUDA, with a PyTorch interface
 Home-page: https://github.com/Dao-AILab/causal-conv1d
 Author: Tri Dao
 Author-email: tri@tridao.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
```

### Comparing `causal_conv1d-1.2.0.post2/README.md` & `causal_conv1d-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `causal_conv1d-1.2.0.post2/causal_conv1d/causal_conv1d_interface.py` & `causal_conv1d-1.2.1/causal_conv1d/causal_conv1d_interface.py`

 * *Files identical despite different names*

### Comparing `causal_conv1d-1.2.0.post2/causal_conv1d.egg-info/PKG-INFO` & `causal_conv1d-1.2.1/causal_conv1d.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-conv1d
-Version: 1.2.0.post2
+Version: 1.2.1
 Summary: Causal depthwise conv1d in CUDA, with a PyTorch interface
 Home-page: https://github.com/Dao-AILab/causal-conv1d
 Author: Tri Dao
 Author-email: tri@tridao.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
```

### Comparing `causal_conv1d-1.2.0.post2/setup.py` & `causal_conv1d-1.2.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -98,17 +98,25 @@
         if bare_metal_version < Version("11.6"):
             raise RuntimeError(
                 "causal_conv1d is only supported on CUDA 11.6 and above.  "
                 "Note: make sure nvcc has a supported version by running nvcc -V."
             )
 
     cc_flag.append("-gencode")
+    cc_flag.append("arch=compute_53,code=sm_53")
+    cc_flag.append("-gencode")
+    cc_flag.append("arch=compute_62,code=sm_62")
+    cc_flag.append("-gencode")
     cc_flag.append("arch=compute_70,code=sm_70")
     cc_flag.append("-gencode")
+    cc_flag.append("arch=compute_72,code=sm_72")
+    cc_flag.append("-gencode")
     cc_flag.append("arch=compute_80,code=sm_80")
+    cc_flag.append("-gencode")
+    cc_flag.append("arch=compute_87,code=sm_87")
     if bare_metal_version >= Version("11.8"):
         cc_flag.append("-gencode")
         cc_flag.append("arch=compute_90,code=sm_90")
 
     # HACK: The compiler flag -D_GLIBCXX_USE_CXX11_ABI is set to be the same as
     # torch._C._GLIBCXX_USE_CXX11_ABI
     # https://github.com/pytorch/pytorch/blob/8472c24e3b5b60150096486616d98b7bea01500b/torch/utils/cpp_extension.py#L920
```

