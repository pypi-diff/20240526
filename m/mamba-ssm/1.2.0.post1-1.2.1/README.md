# Comparing `tmp/mamba_ssm-1.2.0.post1.tar.gz` & `tmp/mamba_ssm-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamba_ssm-1.2.0.post1.tar", last modified: Sat Mar  2 06:51:56 2024, max compression
+gzip compressed data, was "mamba_ssm-1.2.1.tar", last modified: Sun May 26 20:08:59 2024, max compression
```

## Comparing `mamba_ssm-1.2.0.post1.tar` & `mamba_ssm-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/mamba_ssm/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/mamba_ssm/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/models/config_mamba.py
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/models/mixer_seq_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/mamba_ssm/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/modules/mamba_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/mamba_ssm/ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/ops/selective_scan_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/mamba_ssm/ops/triton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/ops/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21303 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/ops/triton/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/ops/triton/selective_state_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/mamba_ssm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/utils/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/mamba_ssm/utils/hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/mamba_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9009 2024-03-02 06:51:56.000000 mamba_ssm-1.2.0.post1/mamba_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-02 06:51:56.000000 mamba_ssm-1.2.0.post1/mamba_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 06:51:56.000000 mamba_ssm-1.2.0.post1/mamba_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-02 06:51:56.000000 mamba_ssm-1.2.0.post1/mamba_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-02 06:51:56.000000 mamba_ssm-1.2.0.post1/mamba_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 06:51:56.137799 mamba_ssm-1.2.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-03-02 06:51:23.000000 mamba_ssm-1.2.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:59.602885 mamba_ssm-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-05-26 20:08:59.602885 mamba_ssm-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:59.598885 mamba_ssm-1.2.1/mamba_ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:59.598885 mamba_ssm-1.2.1/mamba_ssm/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/models/config_mamba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/models/mixer_seq_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:59.598885 mamba_ssm-1.2.1/mamba_ssm/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/modules/mamba_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:59.598885 mamba_ssm-1.2.1/mamba_ssm/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/ops/selective_scan_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:59.602885 mamba_ssm-1.2.1/mamba_ssm/ops/triton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/ops/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21303 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/ops/triton/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/ops/triton/selective_state_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:59.602885 mamba_ssm-1.2.1/mamba_ssm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/utils/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/mamba_ssm/utils/hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:08:59.598885 mamba_ssm-1.2.1/mamba_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-05-26 20:08:59.000000 mamba_ssm-1.2.1/mamba_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-26 20:08:59.000000 mamba_ssm-1.2.1/mamba_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:08:59.000000 mamba_ssm-1.2.1/mamba_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 20:08:59.000000 mamba_ssm-1.2.1/mamba_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 20:08:59.000000 mamba_ssm-1.2.1/mamba_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 20:08:59.602885 mamba_ssm-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-05-26 20:08:31.000000 mamba_ssm-1.2.1/setup.py
```

### Comparing `mamba_ssm-1.2.0.post1/LICENSE` & `mamba_ssm-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.0.post1/PKG-INFO` & `mamba_ssm-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mamba_ssm
-Version: 1.2.0.post1
+Version: 1.2.1
 Summary: Mamba state-space model
 Home-page: https://github.com/state-spaces/mamba
 Author: Tri Dao, Albert Gu
 Author-email: tri@tridao.me, agu@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
```

### Comparing `mamba_ssm-1.2.0.post1/README.md` & `mamba_ssm-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.0.post1/mamba_ssm/models/mixer_seq_simple.py` & `mamba_ssm-1.2.1/mamba_ssm/models/mixer_seq_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,16 +248,15 @@
 
     def save_pretrained(self, save_directory):
         """
         Minimal implementation of save_pretrained for MambaLMHeadModel.
         Save the model and its configuration file to a directory.
         """
         # Ensure save_directory exists
-        if not os.path.exists(save_directory):
-            os.makedirs(save_directory)
+        os.makedirs(save_directory, exist_ok=True)
 
         # Save the model's state_dict
         model_path = os.path.join(save_directory, 'pytorch_model.bin')
         torch.save(self.state_dict(), model_path)
 
         # Save the configuration of the model
         config_path = os.path.join(save_directory, 'config.json')
```

### Comparing `mamba_ssm-1.2.0.post1/mamba_ssm/modules/mamba_simple.py` & `mamba_ssm-1.2.1/mamba_ssm/modules/mamba_simple.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.0.post1/mamba_ssm/ops/selective_scan_interface.py` & `mamba_ssm-1.2.1/mamba_ssm/ops/selective_scan_interface.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.0.post1/mamba_ssm/ops/triton/layernorm.py` & `mamba_ssm-1.2.1/mamba_ssm/ops/triton/layernorm.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.0.post1/mamba_ssm/utils/generation.py` & `mamba_ssm-1.2.1/mamba_ssm/utils/generation.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.0.post1/mamba_ssm/utils/hf.py` & `mamba_ssm-1.2.1/mamba_ssm/utils/hf.py`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.0.post1/mamba_ssm.egg-info/PKG-INFO` & `mamba_ssm-1.2.1/mamba_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mamba-ssm
-Version: 1.2.0.post1
+Version: 1.2.1
 Summary: Mamba state-space model
 Home-page: https://github.com/state-spaces/mamba
 Author: Tri Dao, Albert Gu
 Author-email: tri@tridao.me, agu@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
```

### Comparing `mamba_ssm-1.2.0.post1/mamba_ssm.egg-info/SOURCES.txt` & `mamba_ssm-1.2.1/mamba_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mamba_ssm-1.2.0.post1/setup.py` & `mamba_ssm-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,19 +100,27 @@
     if CUDA_HOME is not None:
         _, bare_metal_version = get_cuda_bare_metal_version(CUDA_HOME)
         if bare_metal_version < Version("11.6"):
             raise RuntimeError(
                 f"{PACKAGE_NAME} is only supported on CUDA 11.6 and above.  "
                 "Note: make sure nvcc has a supported version by running nvcc -V."
             )
-
+            
+    cc_flag.append("-gencode")
+    cc_flag.append("arch=compute_53,code=sm_53")
+    cc_flag.append("-gencode")
+    cc_flag.append("arch=compute_62,code=sm_62")
     cc_flag.append("-gencode")
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

