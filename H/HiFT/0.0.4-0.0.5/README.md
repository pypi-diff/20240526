# Comparing `tmp/HiFT-0.0.4.tar.gz` & `tmp/HiFT-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HiFT-0.0.4.tar", last modified: Tue May 21 01:02:20 2024, max compression
+gzip compressed data, was "dist/HiFT-0.0.5.tar", last modified: Sat May 25 22:39:48 2024, max compression
```

## Comparing `HiFT-0.0.4.tar` & `HiFT-0.0.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.687325 HiFT-0.0.4/
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.627328 HiFT-0.0.4/HiFT.egg-info/
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-21 01:02:20.000000 HiFT-0.0.4/HiFT.egg-info/PKG-INFO
--rw-r--r--   0 yongkang (31362) cisintern (30001)     1250 2024-05-21 01:02:20.000000 HiFT-0.0.4/HiFT.egg-info/SOURCES.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)        1 2024-05-21 01:02:20.000000 HiFT-0.0.4/HiFT.egg-info/dependency_links.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)       14 2024-05-21 01:02:20.000000 HiFT-0.0.4/HiFT.egg-info/top_level.txt
--rw-r--r--   0 yongkang (31362) cisintern (30001)    11324 2024-05-14 23:32:09.000000 HiFT-0.0.4/LICENSE.md
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-21 01:02:20.687325 HiFT-0.0.4/PKG-INFO
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12282 2024-05-01 15:36:00.000000 HiFT-0.0.4/README.md
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.647327 HiFT-0.0.4/examples/
--rw-r--r--   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:30:41.000000 HiFT-0.0.4/examples/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     4135 2024-05-14 12:27:27.000000 HiFT-0.0.4/examples/build_dataset.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    23087 2024-05-14 20:25:29.000000 HiFT-0.0.4/examples/instruct_tuning.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     8321 2024-05-12 21:30:41.000000 HiFT-0.0.4/examples/llama2_flash_attn_monkey_patch.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     4054 2024-05-12 21:30:41.000000 HiFT-0.0.4/examples/llama_flash_attn_monkey_patch.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     4916 2024-05-12 21:30:42.000000 HiFT-0.0.4/examples/llama_xformers_attn_monkey_patch.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    30731 2024-05-14 15:18:26.000000 HiFT-0.0.4/examples/pretrain_tuning.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    35374 2024-05-20 23:57:56.000000 HiFT-0.0.4/examples/run_generation.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    33754 2024-05-14 20:20:10.000000 HiFT-0.0.4/examples/run_glue.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    32543 2024-05-14 20:20:40.000000 HiFT-0.0.4/examples/run_ner.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    37615 2024-05-14 20:20:53.000000 HiFT-0.0.4/examples/run_qa.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    22777 2024-05-12 21:30:42.000000 HiFT-0.0.4/examples/utils_qa.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    20863 2024-05-14 20:21:08.000000 HiFT-0.0.4/examples/vicuna_train.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.655326 HiFT-0.0.4/hift/
--rw-r--r--   0 yongkang (31362) cisintern (30001)      268 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/__init__.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.671326 HiFT-0.0.4/hift/optimizers/
--rw-r--r--   0 yongkang (31362) cisintern (30001)      761 2024-05-14 15:15:35.000000 HiFT-0.0.4/hift/optimizers/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14454 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/adagrad.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.683325 HiFT-0.0.4/hift/optimizers/bitsandbytes/
--rw-r--r--   0 yongkang (31362) cisintern (30001)     1001 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     7897 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/adagrad.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    23872 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/adam.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14509 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/adamw.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     7944 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/lamb.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     9373 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/lars.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    11596 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/lion.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     7769 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/rmsprop.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     6444 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/bitsandbytes/sgd.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    34481 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/optimization.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    74393 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/optimizer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    37568 2024-05-14 15:15:17.000000 HiFT-0.0.4/hift/optimizers/replace_operation.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    15390 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/rmsprop.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    14715 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/sgd.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    29623 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/torchAdam.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    29240 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/optimizers/torchAdamw.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12180 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/qatrainer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    12599 2024-05-21 01:00:32.000000 HiFT-0.0.4/hift/registerCallBack.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    30885 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/seqtrainer.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)    77451 2024-05-14 15:15:05.000000 HiFT-0.0.4/hift/trainer.py
-drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-21 01:02:20.683325 HiFT-0.0.4/hift/utils/
--rw-r--r--   0 yongkang (31362) cisintern (30001)       32 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/utils/__init__.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)     6997 2024-05-12 21:31:32.000000 HiFT-0.0.4/hift/utils/utils.py
--rw-r--r--   0 yongkang (31362) cisintern (30001)       38 2024-05-21 01:02:20.687325 HiFT-0.0.4/setup.cfg
--rw-r--r--   0 yongkang (31362) cisintern (30001)      783 2024-05-21 01:00:41.000000 HiFT-0.0.4/setup.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-25 22:39:48.004726 HiFT-0.0.5/
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-25 22:39:47.592743 HiFT-0.0.5/HiFT.egg-info/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-25 22:39:47.000000 HiFT-0.0.5/HiFT.egg-info/PKG-INFO
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     1250 2024-05-25 22:39:47.000000 HiFT-0.0.5/HiFT.egg-info/SOURCES.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)        1 2024-05-25 22:39:47.000000 HiFT-0.0.5/HiFT.egg-info/dependency_links.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       14 2024-05-25 22:39:47.000000 HiFT-0.0.5/HiFT.egg-info/top_level.txt
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    11324 2024-05-14 23:32:09.000000 HiFT-0.0.5/LICENSE.md
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12834 2024-05-25 22:39:48.004726 HiFT-0.0.5/PKG-INFO
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12282 2024-05-01 15:36:00.000000 HiFT-0.0.5/README.md
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-25 22:39:47.808734 HiFT-0.0.5/examples/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)        0 2024-05-12 21:30:41.000000 HiFT-0.0.5/examples/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4135 2024-05-14 12:27:27.000000 HiFT-0.0.5/examples/build_dataset.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    23087 2024-05-14 20:25:29.000000 HiFT-0.0.5/examples/instruct_tuning.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     8321 2024-05-12 21:30:41.000000 HiFT-0.0.5/examples/llama2_flash_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4054 2024-05-12 21:30:41.000000 HiFT-0.0.5/examples/llama_flash_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     4916 2024-05-12 21:30:42.000000 HiFT-0.0.5/examples/llama_xformers_attn_monkey_patch.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    30731 2024-05-14 15:18:26.000000 HiFT-0.0.5/examples/pretrain_tuning.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    35374 2024-05-20 23:57:56.000000 HiFT-0.0.5/examples/run_generation.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    33754 2024-05-14 20:20:10.000000 HiFT-0.0.5/examples/run_glue.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    32543 2024-05-14 20:20:40.000000 HiFT-0.0.5/examples/run_ner.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    37790 2024-05-25 20:53:35.000000 HiFT-0.0.5/examples/run_qa.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    22777 2024-05-12 21:30:42.000000 HiFT-0.0.5/examples/utils_qa.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    20863 2024-05-14 20:21:08.000000 HiFT-0.0.5/examples/vicuna_train.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-25 22:39:47.920729 HiFT-0.0.5/hift/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      268 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/__init__.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-25 22:39:47.976727 HiFT-0.0.5/hift/optimizers/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      761 2024-05-14 15:15:35.000000 HiFT-0.0.5/hift/optimizers/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14454 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/adagrad.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-25 22:39:48.000726 HiFT-0.0.5/hift/optimizers/bitsandbytes/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     1001 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/bitsandbytes/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7897 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/bitsandbytes/adagrad.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    23872 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/bitsandbytes/adam.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14509 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/bitsandbytes/adamw.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7944 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/bitsandbytes/lamb.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     9373 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/bitsandbytes/lars.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    11596 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/bitsandbytes/lion.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     7769 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/bitsandbytes/rmsprop.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     6444 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/bitsandbytes/sgd.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    34481 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/optimization.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    74393 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/optimizer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    37568 2024-05-14 15:15:17.000000 HiFT-0.0.5/hift/optimizers/replace_operation.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    15390 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/rmsprop.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    14715 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/sgd.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    29623 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/torchAdam.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    29240 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/optimizers/torchAdamw.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12180 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/qatrainer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    12599 2024-05-21 01:00:32.000000 HiFT-0.0.5/hift/registerCallBack.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    30885 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/seqtrainer.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)    67001 2024-05-25 22:37:26.000000 HiFT-0.0.5/hift/trainer.py
+drwxr-xr-x   0 yongkang (31362) cisintern (30001)        0 2024-05-25 22:39:48.004726 HiFT-0.0.5/hift/utils/
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       32 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/utils/__init__.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)     6997 2024-05-12 21:31:32.000000 HiFT-0.0.5/hift/utils/utils.py
+-rw-r--r--   0 yongkang (31362) cisintern (30001)       38 2024-05-25 22:39:48.004726 HiFT-0.0.5/setup.cfg
+-rw-r--r--   0 yongkang (31362) cisintern (30001)      783 2024-05-25 22:38:25.000000 HiFT-0.0.5/setup.py
```

### Comparing `HiFT-0.0.4/HiFT.egg-info/PKG-INFO` & `HiFT-0.0.5/HiFT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiFT
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.
 Home-page: https://github.com/misonsky/HiFT
 Author: Yongkang Liu
 Author-email: misonsky@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HiFT-0.0.4/HiFT.egg-info/SOURCES.txt` & `HiFT-0.0.5/HiFT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/LICENSE.md` & `HiFT-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/PKG-INFO` & `HiFT-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HiFT
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.
 Home-page: https://github.com/misonsky/HiFT
 Author: Yongkang Liu
 Author-email: misonsky@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HiFT-0.0.4/README.md` & `HiFT-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/build_dataset.py` & `HiFT-0.0.5/examples/build_dataset.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/instruct_tuning.py` & `HiFT-0.0.5/examples/instruct_tuning.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/llama2_flash_attn_monkey_patch.py` & `HiFT-0.0.5/examples/llama2_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/llama_flash_attn_monkey_patch.py` & `HiFT-0.0.5/examples/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/llama_xformers_attn_monkey_patch.py` & `HiFT-0.0.5/examples/llama_xformers_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/pretrain_tuning.py` & `HiFT-0.0.5/examples/pretrain_tuning.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/run_generation.py` & `HiFT-0.0.5/examples/run_generation.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/run_glue.py` & `HiFT-0.0.5/examples/run_glue.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/run_ner.py` & `HiFT-0.0.5/examples/run_ner.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/run_qa.py` & `HiFT-0.0.5/examples/run_qa.py`

 * *Files 0% similar despite different names*

```diff
@@ -522,16 +522,18 @@
         # Let's label those examples!
         tokenized_examples["start_positions"] = []
         tokenized_examples["end_positions"] = []
 
         for i, offsets in enumerate(offset_mapping):
             # We will label impossible answers with the index of the CLS token.
             input_ids = tokenized_examples["input_ids"][i]
-            cls_index = input_ids.index(tokenizer.cls_token_id)
-
+            if tokenizer.cls_token_id is not None:
+                cls_index = input_ids.index(tokenizer.cls_token_id)
+            elif tokenizer.bos_token_id is not None:
+                cls_index = input_ids.index(tokenizer.bos_token_id)
             # Grab the sequence corresponding to that example (to know what is the context and what is the question).
             sequence_ids = tokenized_examples.sequence_ids(i)
 
             # One example can give several spans, this is the index of the example containing this span of text.
             sample_index = sample_mapping[i]
             answers = examples[answer_column_name][sample_index]
             # If no answers are given, set the cls_index as answer.
```

### Comparing `HiFT-0.0.4/examples/utils_qa.py` & `HiFT-0.0.5/examples/utils_qa.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/examples/vicuna_train.py` & `HiFT-0.0.5/examples/vicuna_train.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/__init__.py` & `HiFT-0.0.5/hift/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/adagrad.py` & `HiFT-0.0.5/hift/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/bitsandbytes/__init__.py` & `HiFT-0.0.5/hift/optimizers/bitsandbytes/__init__.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/bitsandbytes/adagrad.py` & `HiFT-0.0.5/hift/optimizers/bitsandbytes/adagrad.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/bitsandbytes/adam.py` & `HiFT-0.0.5/hift/optimizers/bitsandbytes/adam.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/bitsandbytes/adamw.py` & `HiFT-0.0.5/hift/optimizers/bitsandbytes/adamw.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/bitsandbytes/lamb.py` & `HiFT-0.0.5/hift/optimizers/bitsandbytes/lamb.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/bitsandbytes/lars.py` & `HiFT-0.0.5/hift/optimizers/bitsandbytes/lars.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/bitsandbytes/lion.py` & `HiFT-0.0.5/hift/optimizers/bitsandbytes/lion.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/bitsandbytes/rmsprop.py` & `HiFT-0.0.5/hift/optimizers/bitsandbytes/rmsprop.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/bitsandbytes/sgd.py` & `HiFT-0.0.5/hift/optimizers/bitsandbytes/sgd.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/optimization.py` & `HiFT-0.0.5/hift/optimizers/optimization.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/optimizer.py` & `HiFT-0.0.5/hift/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/replace_operation.py` & `HiFT-0.0.5/hift/optimizers/replace_operation.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/rmsprop.py` & `HiFT-0.0.5/hift/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/sgd.py` & `HiFT-0.0.5/hift/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/torchAdam.py` & `HiFT-0.0.5/hift/optimizers/torchAdam.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/optimizers/torchAdamw.py` & `HiFT-0.0.5/hift/optimizers/torchAdamw.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/qatrainer.py` & `HiFT-0.0.5/hift/qatrainer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/registerCallBack.py` & `HiFT-0.0.5/hift/registerCallBack.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/seqtrainer.py` & `HiFT-0.0.5/hift/seqtrainer.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/hift/trainer.py` & `HiFT-0.0.5/hift/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,58 +114,14 @@
 logger = logging.get_logger(__name__)
 from .optimizers import replace_backward
 
 class PEFTrainer(Trainer):
     def __init__(self,peft_type=None,*args,**kwargs):
         super().__init__(*args, **kwargs)
         self.peft_type = peft_type
-    def create_optimizer(self):
-        """
-        Setup the optimizer.
-
-        We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
-        Trainer's init through `optimizers`, or subclass and override this method in a subclass.
-        """
-        opt_model = self.model_wrapped if is_sagemaker_mp_enabled() else self.model
-        if self.optimizer is None:
-            decay_parameters = self.get_decay_parameter_names(opt_model)
-            optimizer_grouped_parameters = [
-                {
-                    "params": [
-                        p for n, p in opt_model.named_parameters() if (n in decay_parameters and p.requires_grad)
-                    ],
-                    "weight_decay": self.args.weight_decay,
-                },
-                {
-                    "params": [
-                        p for n, p in opt_model.named_parameters() if (n not in decay_parameters and p.requires_grad)
-                    ],
-                    "weight_decay": 0.0,
-                },
-            ]
-
-            optimizer_cls, optimizer_kwargs = PEFTrainer.get_optimizer_cls_and_kwargs(self.args)
-
-            self.optimizer = optimizer_cls(optimizer_grouped_parameters, **optimizer_kwargs)
-            if optimizer_cls.__name__ == "Adam8bit":
-                import bitsandbytes
-
-                manager = bitsandbytes.optim.GlobalOptimManager.get_instance()
-
-                skipped = 0
-                for module in opt_model.modules():
-                    if isinstance(module, nn.Embedding):
-                        skipped += sum({p.data_ptr(): p.numel() for p in module.parameters()}.values())
-                        logger.info(f"skipped {module}: {skipped/2**20}M params")
-                        manager.register_module_override(module, "weight", {"optim_bits": 32})
-                        logger.debug(f"bitsandbytes: will optimize {module} in fp32")
-                logger.info(f"skipped: {skipped/2**20}M params")
-        if is_sagemaker_mp_enabled():
-            self.optimizer = smp.DistributedOptimizer(self.optimizer)
-        return self.optimizer
     def training_step(self, model: nn.Module, inputs: Dict[str, Union[torch.Tensor, Any]]) -> torch.Tensor:
         return super().training_step(model, inputs)
     def _inner_training_loop(
         self, batch_size=None, args=None, resume_from_checkpoint=None, trial=None, ignore_keys_for_eval=None
     ):
         self.accelerator.free_memory()
         self._train_batch_size = batch_size
@@ -627,212 +583,14 @@
 
         # After training we make sure to retrieve back the original forward pass method
         # for the embedding layer by removing the forward post hook.
         if self.neftune_noise_alpha is not None:
             self._deactivate_neftune(self.model)
 
         return TrainOutput(self.state.global_step, train_loss, metrics)
-
-    @staticmethod
-    def get_optimizer_cls_and_kwargs(args: TrainingArguments) -> Tuple[Any, Any]:
-        """
-        Returns the optimizer class and optimizer parameters based on the training arguments.
-
-        Args:
-            args (`transformers.training_args.TrainingArguments`):
-                The training arguments for the training session.
-
-        """
-
-        for optimizer in OptimizerNames:
-            print(optimizer.name, optimizer.value)
-        # parse args.optim_args
-        optim_args = {}
-        if args.optim_args:
-            for mapping in args.optim_args.replace(" ", "").split(","):
-                key, value = mapping.split("=")
-                optim_args[key] = value
-
-        optimizer_kwargs = {"lr": args.learning_rate}
-
-        adam_kwargs = {
-            "betas": (args.adam_beta1, args.adam_beta2),
-            "eps": args.adam_epsilon,
-        }
-        if args.optim == OptimizerNames.ADAFACTOR:
-            optimizer_cls = Adafactor
-            optimizer_kwargs.update({"scale_parameter": False, "relative_step": False})
-        elif args.optim == OptimizerNames.ADAMW_HF:
-            from .optimizers.optimization import AdamW
-
-            optimizer_cls = AdamW
-            optimizer_kwargs.update(adam_kwargs)
-        elif args.optim in [OptimizerNames.ADAMW_TORCH, OptimizerNames.ADAMW_TORCH_FUSED]:
-            from .optimizers.torchAdamw import AdamW
-
-            optimizer_cls = AdamW
-            optimizer_kwargs.update(adam_kwargs)
-            if args.optim == OptimizerNames.ADAMW_TORCH_FUSED:
-                optimizer_kwargs.update({"fused": True})
-        elif args.optim == OptimizerNames.ADAMW_TORCH_XLA:
-            try:
-                from torch_xla.amp.syncfree import AdamW
-
-                optimizer_cls = AdamW
-                optimizer_kwargs.update(adam_kwargs)
-            except ImportError:
-                raise ValueError("Trainer failed to import syncfree AdamW from torch_xla.")
-        elif args.optim == OptimizerNames.ADAMW_TORCH_NPU_FUSED:
-            try:
-                from torch_npu.optim import NpuFusedAdamW
-
-                optimizer_cls = NpuFusedAdamW
-                optimizer_kwargs.update(adam_kwargs)
-            except ImportError:
-                raise ValueError("Trainer failed to import FusedAdamW from torch_npu.")
-        elif args.optim == OptimizerNames.ADAMW_APEX_FUSED:
-            try:
-                from apex.optimizers import FusedAdam
-
-                optimizer_cls = FusedAdam
-                optimizer_kwargs.update(adam_kwargs)
-            except ImportError:
-                raise ValueError("Trainer tried to instantiate apex FusedAdam but apex is not installed!")
-        
-        elif args.optim in [
-            OptimizerNames.ADAMW_BNB,
-            OptimizerNames.ADAMW_8BIT,
-            OptimizerNames.PAGED_ADAMW,
-            OptimizerNames.PAGED_ADAMW_8BIT,
-            OptimizerNames.LION,
-            OptimizerNames.LION_8BIT,
-            OptimizerNames.PAGED_LION,
-            OptimizerNames.PAGED_LION_8BIT,
-        ]:
-            from .optimizers import BitAdamW, BitLion
-            is_paged = False
-            optim_bits = 32
-            optimizer_cls = None
-            additional_optim_kwargs = adam_kwargs
-            if "paged" in args.optim:
-                is_paged = True
-            if "8bit" in args.optim:
-                optim_bits = 8
-            if "adam" in args.optim:
-                optimizer_cls = BitAdamW
-            elif "lion" in args.optim:
-                optimizer_cls = BitLion
-                additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
-            bnb_kwargs = {"is_paged": is_paged, "optim_bits": optim_bits}
-            optimizer_kwargs.update(additional_optim_kwargs)
-            optimizer_kwargs.update(bnb_kwargs)
-        elif args.optim in [
-            OptimizerNames.ADAM,
-            OptimizerNames.ADAM_32BIT,
-            OptimizerNames.ADAM_8BIT,
-            OptimizerNames.PAGED_ADAM,
-            OptimizerNames.PAGED_ADAM_32BIT,
-            OptimizerNames.PAGED_ADAM_8BIT
-        ]:
-            from .optimizers import Adam32bit,Adam8bit,PagedAdam8bit,PagedAdam32bit
-            
-            additional_optim_kwargs = adam_kwargs
-            if "paged" in args.optim:
-                if "8bit" in args.optim:
-                    optimizer_cls = PagedAdam8bit
-                else:
-                    optimizer_cls = PagedAdam32bit
-            else:
-                if "8bit" in args.optim:
-                    optimizer_cls = Adam8bit
-                else:
-                    optimizer_cls = Adam32bit
-            optimizer_kwargs.update(additional_optim_kwargs)
-        elif args.optim in [
-            OptimizerNames.LAMB,
-            OptimizerNames.LAMB_32BIT,
-            OptimizerNames.LAMB_8BIT
-        ]:
-            from .optimizers import BitLAMB,LAMB32bit,LAMB8bit
-            if "8bit" in args.optim:
-                optimizer_cls = LAMB8bit
-            else:
-                ## bitsandbytes only support 8-bit lamb
-                optimizer_cls = LAMB8bit
-            additional_optim_kwargs = {"betas": (args.adam_beta1, args.adam_beta2)}
-            optimizer_kwargs.update(additional_optim_kwargs)
-        elif args.optim in [
-            OptimizerNames.LARS,
-            OptimizerNames.LARS_32BIT,
-            OptimizerNames.LARS_8BIT
-        ]:
-            from .optimizers import BitLARS,LARS8bit,LARS32bit
-            if "8bit" in args.optim:
-                optimizer_cls = LARS8bit
-            else:
-                ## bitsandbytes only support 8-bit lars
-                optimizer_cls = LARS8bit
-            additional_optim_kwargs = {"momentum": args.adam_beta1}
-            optimizer_kwargs.update(additional_optim_kwargs)
-        elif args.optim in [
-            OptimizerNames.BSGD,
-            OptimizerNames.BSGD_32BIT,
-            OptimizerNames.BSGD_8BIT
-        ]:
-            from .optimizers import BitSGD,SGD8bit,SGD32bit
-            if "8bit" in args.optim:
-                optimizer_cls = SGD8bit
-            else:
-                ## bitsandbytes only support 8-bit lars
-                optimizer_cls = SGD32bit
-        elif args.optim in [
-            OptimizerNames.BRMSPROP,
-            OptimizerNames.BRMSPROP_32BIT,
-            OptimizerNames.BRMSPROP_8BIT
-        ]:
-            from .optimizers import BitRMSprop,RMSprop8bit,RMSprop32bit
-            if "8bit" in args.optim:
-                optimizer_cls = RMSprop8bit
-            else:
-                ## bitsandbytes only support 8-bit lars
-                optimizer_cls = RMSprop32bit
-        elif args.optim == OptimizerNames.ADAMW_ANYPRECISION:
-            try:
-                from torchdistx.optimizers import AnyPrecisionAdamW
-
-                optimizer_cls = AnyPrecisionAdamW
-                optimizer_kwargs.update(adam_kwargs)
-
-                # TODO Change dtypes back to M=FP32, Var = BF16, Kahan = False once they can be cast together in torchdistx.
-                optimizer_kwargs.update(
-                    {
-                        "use_kahan_summation": strtobool(optim_args.get("use_kahan_summation", "False")),
-                        "momentum_dtype": getattr(torch, optim_args.get("momentum_dtype", "float32")),
-                        "variance_dtype": getattr(torch, optim_args.get("variance_dtype", "float32")),
-                        "compensation_buffer_dtype": getattr(
-                            torch, optim_args.get("compensation_buffer_dtype", "bfloat16")
-                        ),
-                    }
-                )
-            except ImportError:
-                raise ValueError("Please install https://github.com/pytorch/torchdistx")
-        elif args.optim == OptimizerNames.SGD:
-            from .optimizers.sgd import SGD
-            optimizer_cls = SGD
-        
-        elif args.optim == OptimizerNames.ADAGRAD:
-            from .optimizers.adagrad import Adagrad
-            optimizer_cls = Adagrad
-        elif args.optim == OptimizerNames.RMSPROP:
-            from .optimizers.rmsprop import RMSprop
-            optimizer_cls = RMSprop
-        else:
-            raise ValueError(f"Trainer cannot instantiate unsupported optimizer: {args.optim}")
-        logger.info(f"the optimizer you are using: {optimizer_cls}")
-        return optimizer_cls, optimizer_kwargs
     
 
 class HiFTrainer(Trainer):
     def __init__(self,
                 hiFThandler,
                 HiTaskType,
                 group_element=1,
```

### Comparing `HiFT-0.0.4/hift/utils/utils.py` & `HiFT-0.0.5/hift/utils/utils.py`

 * *Files identical despite different names*

### Comparing `HiFT-0.0.4/setup.py` & `HiFT-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="HiFT",
-    version="0.0.4",
+    version="0.0.5",
     author="Yongkang Liu",
     author_email="misonsky@163.com",
     description="PyTorch implementation of 'HiFT: A Hierarchical Full Parameter Fine-Tuning Strategy', a memory-efficient approach to adapt a large pre-trained deep learning model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/misonsky/HiFT",
     packages=setuptools.find_packages(),
```

