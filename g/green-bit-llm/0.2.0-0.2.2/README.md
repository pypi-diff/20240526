# Comparing `tmp/green-bit-llm-0.2.0.tar.gz` & `tmp/green_bit_llm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "green-bit-llm-0.2.0.tar", last modified: Wed May 22 21:36:24 2024, max compression
+gzip compressed data, was "green_bit_llm-0.2.2.tar", last modified: Fri May 24 17:06:42 2024, max compression
```

## Comparing `green-bit-llm-0.2.0.tar` & `green_bit_llm-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.293589 green-bit-llm-0.2.0/
--rw-r--r--   0 haojin     (501) staff       (20)    11357 2024-04-07 20:16:16.000000 green-bit-llm-0.2.0/LICENSE
--rw-r--r--   0 haojin     (501) staff       (20)     9658 2024-05-22 21:36:24.291640 green-bit-llm-0.2.0/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)     8889 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/README.md
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.281710 green-bit-llm-0.2.0/green_bit_llm/
--rw-r--r--   0 haojin     (501) staff       (20)       33 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     1920 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/args_parser.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.283052 green-bit-llm-0.2.0/green_bit_llm/common/
--rw-r--r--   0 haojin     (501) staff       (20)       34 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/common/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)      156 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/common/enum.py
--rw-r--r--   0 haojin     (501) staff       (20)    18420 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/common/model.py
--rw-r--r--   0 haojin     (501) staff       (20)     8507 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/common/utils.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.284287 green-bit-llm-0.2.0/green_bit_llm/evaluation/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     9588 2024-05-01 10:29:45.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/datautils.py
--rw-r--r--   0 haojin     (501) staff       (20)     8542 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/evaluate.py
--rw-r--r--   0 haojin     (501) staff       (20)     4569 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/lmclass.py
--rw-r--r--   0 haojin     (501) staff       (20)     2840 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/evaluation/utils.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.288579 green-bit-llm-0.2.0/green_bit_llm/inference/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)    21289 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/chat_base.py
--rw-r--r--   0 haojin     (501) staff       (20)     5319 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/chat_cli.py
--rw-r--r--   0 haojin     (501) staff       (20)    18476 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/conversation.py
--rw-r--r--   0 haojin     (501) staff       (20)     4195 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/sim_gen.py
--rw-r--r--   0 haojin     (501) staff       (20)     4536 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/inference/utils.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.290049 green-bit-llm-0.2.0/green_bit_llm/sft/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     5110 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/sft/finetune.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.290768 green-bit-llm-0.2.0/green_bit_llm/sft/optim/
--rw-r--r--   0 haojin     (501) staff       (20)       32 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/optim/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     6260 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/sft/optim/adamw8bit.py
--rw-r--r--   0 haojin     (501) staff       (20)    21387 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/optim/bnb_optimizer.py
--rw-r--r--   0 haojin     (501) staff       (20)     4333 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/sft/peft_lora.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.291330 green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/
--rw-r--r--   0 haojin     (501) staff       (20)        0 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/__init__.py
--rw-r--r--   0 haojin     (501) staff       (20)     9361 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/gba_lora.py
--rw-r--r--   0 haojin     (501) staff       (20)     2662 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/model.py
--rw-r--r--   0 haojin     (501) staff       (20)     2997 2024-05-22 21:28:03.000000 green-bit-llm-0.2.0/green_bit_llm/sft/trainer.py
--rw-r--r--   0 haojin     (501) staff       (20)     5587 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/green_bit_llm/sft/utils.py
--rw-r--r--   0 haojin     (501) staff       (20)       22 2024-05-22 21:36:20.000000 green-bit-llm-0.2.0/green_bit_llm/version.py
-drwxr-xr-x   0 haojin     (501) staff       (20)        0 2024-05-22 21:36:24.282267 green-bit-llm-0.2.0/green_bit_llm.egg-info/
--rw-r--r--   0 haojin     (501) staff       (20)     9658 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/PKG-INFO
--rw-r--r--   0 haojin     (501) staff       (20)     1192 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/SOURCES.txt
--rw-r--r--   0 haojin     (501) staff       (20)        1 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/dependency_links.txt
--rw-r--r--   0 haojin     (501) staff       (20)      180 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/requires.txt
--rw-r--r--   0 haojin     (501) staff       (20)       14 2024-05-22 21:36:24.000000 green-bit-llm-0.2.0/green_bit_llm.egg-info/top_level.txt
--rw-r--r--   0 haojin     (501) staff       (20)       38 2024-05-22 21:36:24.293639 green-bit-llm-0.2.0/setup.cfg
--rw-r--r--   0 haojin     (501) staff       (20)      865 2024-04-27 11:19:52.000000 green-bit-llm-0.2.0/setup.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2024-05-24 17:06:42.098670 green_bit_llm-0.2.2/
+-rw-r--r--   0 joseph     (501) staff       (20)    11357 2024-04-25 14:58:30.000000 green_bit_llm-0.2.2/LICENSE
+-rw-r--r--   0 joseph     (501) staff       (20)     9658 2024-05-24 17:06:42.098473 green_bit_llm-0.2.2/PKG-INFO
+-rw-r--r--   0 joseph     (501) staff       (20)     8889 2024-05-24 17:00:44.000000 green_bit_llm-0.2.2/README.md
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2024-05-24 17:06:42.091154 green_bit_llm-0.2.2/green_bit_llm/
+-rw-r--r--   0 joseph     (501) staff       (20)       33 2024-04-25 15:41:49.000000 green_bit_llm-0.2.2/green_bit_llm/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     1920 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/args_parser.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2024-05-24 17:06:42.092840 green_bit_llm-0.2.2/green_bit_llm/common/
+-rw-r--r--   0 joseph     (501) staff       (20)       34 2024-04-25 15:43:21.000000 green_bit_llm-0.2.2/green_bit_llm/common/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)      156 2024-04-25 14:58:30.000000 green_bit_llm-0.2.2/green_bit_llm/common/enum.py
+-rw-r--r--   0 joseph     (501) staff       (20)    18420 2024-05-24 17:00:44.000000 green_bit_llm-0.2.2/green_bit_llm/common/model.py
+-rw-r--r--   0 joseph     (501) staff       (20)     8507 2024-05-24 17:00:44.000000 green_bit_llm-0.2.2/green_bit_llm/common/utils.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2024-05-24 17:06:42.094238 green_bit_llm-0.2.2/green_bit_llm/evaluation/
+-rw-r--r--   0 joseph     (501) staff       (20)        0 2024-04-25 14:58:30.000000 green_bit_llm-0.2.2/green_bit_llm/evaluation/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     9588 2024-05-06 08:30:51.000000 green_bit_llm-0.2.2/green_bit_llm/evaluation/datautils.py
+-rw-r--r--   0 joseph     (501) staff       (20)     8542 2024-05-24 17:00:44.000000 green_bit_llm-0.2.2/green_bit_llm/evaluation/evaluate.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4569 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/evaluation/lmclass.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2840 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/evaluation/utils.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2024-05-24 17:06:42.095768 green_bit_llm-0.2.2/green_bit_llm/inference/
+-rw-r--r--   0 joseph     (501) staff       (20)        0 2024-04-25 14:58:30.000000 green_bit_llm-0.2.2/green_bit_llm/inference/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)    21289 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/inference/chat_base.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5319 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/inference/chat_cli.py
+-rw-r--r--   0 joseph     (501) staff       (20)    18476 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/inference/conversation.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4195 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/inference/sim_gen.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4536 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/inference/utils.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2024-05-24 17:06:42.096724 green_bit_llm-0.2.2/green_bit_llm/sft/
+-rw-r--r--   0 joseph     (501) staff       (20)        0 2024-04-25 14:58:30.000000 green_bit_llm-0.2.2/green_bit_llm/sft/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5110 2024-05-24 17:00:44.000000 green_bit_llm-0.2.2/green_bit_llm/sft/finetune.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2024-05-24 17:06:42.097293 green_bit_llm-0.2.2/green_bit_llm/sft/optim/
+-rw-r--r--   0 joseph     (501) staff       (20)       32 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/sft/optim/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     6260 2024-05-24 17:00:44.000000 green_bit_llm-0.2.2/green_bit_llm/sft/optim/adamw8bit.py
+-rw-r--r--   0 joseph     (501) staff       (20)    21387 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/sft/optim/bnb_optimizer.py
+-rw-r--r--   0 joseph     (501) staff       (20)     4333 2024-05-24 17:00:44.000000 green_bit_llm-0.2.2/green_bit_llm/sft/peft_lora.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2024-05-24 17:06:42.097980 green_bit_llm-0.2.2/green_bit_llm/sft/peft_utils/
+-rw-r--r--   0 joseph     (501) staff       (20)        0 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/sft/peft_utils/__init__.py
+-rw-r--r--   0 joseph     (501) staff       (20)     9361 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/sft/peft_utils/gba_lora.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2662 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/sft/peft_utils/model.py
+-rw-r--r--   0 joseph     (501) staff       (20)     2997 2024-05-24 17:00:44.000000 green_bit_llm-0.2.2/green_bit_llm/sft/trainer.py
+-rw-r--r--   0 joseph     (501) staff       (20)     5587 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/green_bit_llm/sft/utils.py
+-rw-r--r--   0 joseph     (501) staff       (20)       22 2024-05-24 17:02:35.000000 green_bit_llm-0.2.2/green_bit_llm/version.py
+drwxr-xr-x   0 joseph     (501) staff       (20)        0 2024-05-24 17:06:42.098235 green_bit_llm-0.2.2/green_bit_llm.egg-info/
+-rw-r--r--   0 joseph     (501) staff       (20)     9658 2024-05-24 17:06:42.000000 green_bit_llm-0.2.2/green_bit_llm.egg-info/PKG-INFO
+-rw-r--r--   0 joseph     (501) staff       (20)     1192 2024-05-24 17:06:42.000000 green_bit_llm-0.2.2/green_bit_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 joseph     (501) staff       (20)        1 2024-05-24 17:06:42.000000 green_bit_llm-0.2.2/green_bit_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 joseph     (501) staff       (20)      180 2024-05-24 17:06:42.000000 green_bit_llm-0.2.2/green_bit_llm.egg-info/requires.txt
+-rw-r--r--   0 joseph     (501) staff       (20)       14 2024-05-24 17:06:42.000000 green_bit_llm-0.2.2/green_bit_llm.egg-info/top_level.txt
+-rw-r--r--   0 joseph     (501) staff       (20)       38 2024-05-24 17:06:42.098708 green_bit_llm-0.2.2/setup.cfg
+-rw-r--r--   0 joseph     (501) staff       (20)      865 2024-04-29 09:08:03.000000 green_bit_llm-0.2.2/setup.py
```

### Comparing `green-bit-llm-0.2.0/LICENSE` & `green_bit_llm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/PKG-INFO` & `green_bit_llm-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green-bit-llm
-Version: 0.2.0
+Version: 0.2.2
 Summary: A toolkit for fine-tuning, inferencing, and evaluating GreenBitAI's LLMs.
 Home-page: https://github.com/GreenBitAI/green-bit-llm
 Author: GreenBitAI Contributors
 Author-email: team@greenbit.ai
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `green-bit-llm-0.2.0/README.md` & `green_bit_llm-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/args_parser.py` & `green_bit_llm-0.2.2/green_bit_llm/args_parser.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/common/model.py` & `green_bit_llm-0.2.2/green_bit_llm/common/model.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/common/utils.py` & `green_bit_llm-0.2.2/green_bit_llm/common/utils.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/evaluation/datautils.py` & `green_bit_llm-0.2.2/green_bit_llm/evaluation/datautils.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/evaluation/evaluate.py` & `green_bit_llm-0.2.2/green_bit_llm/evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/evaluation/lmclass.py` & `green_bit_llm-0.2.2/green_bit_llm/evaluation/lmclass.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/evaluation/utils.py` & `green_bit_llm-0.2.2/green_bit_llm/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/inference/chat_base.py` & `green_bit_llm-0.2.2/green_bit_llm/inference/chat_base.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/inference/chat_cli.py` & `green_bit_llm-0.2.2/green_bit_llm/inference/chat_cli.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/inference/conversation.py` & `green_bit_llm-0.2.2/green_bit_llm/inference/conversation.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/inference/sim_gen.py` & `green_bit_llm-0.2.2/green_bit_llm/inference/sim_gen.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/inference/utils.py` & `green_bit_llm-0.2.2/green_bit_llm/inference/utils.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/sft/finetune.py` & `green_bit_llm-0.2.2/green_bit_llm/sft/finetune.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/sft/optim/adamw8bit.py` & `green_bit_llm-0.2.2/green_bit_llm/sft/optim/adamw8bit.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/sft/optim/bnb_optimizer.py` & `green_bit_llm-0.2.2/green_bit_llm/sft/optim/bnb_optimizer.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/sft/peft_lora.py` & `green_bit_llm-0.2.2/green_bit_llm/sft/peft_lora.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/gba_lora.py` & `green_bit_llm-0.2.2/green_bit_llm/sft/peft_utils/gba_lora.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/sft/peft_utils/model.py` & `green_bit_llm-0.2.2/green_bit_llm/sft/peft_utils/model.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/sft/trainer.py` & `green_bit_llm-0.2.2/green_bit_llm/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm/sft/utils.py` & `green_bit_llm-0.2.2/green_bit_llm/sft/utils.py`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/green_bit_llm.egg-info/PKG-INFO` & `green_bit_llm-0.2.2/green_bit_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: green-bit-llm
-Version: 0.2.0
+Version: 0.2.2
 Summary: A toolkit for fine-tuning, inferencing, and evaluating GreenBitAI's LLMs.
 Home-page: https://github.com/GreenBitAI/green-bit-llm
 Author: GreenBitAI Contributors
 Author-email: team@greenbit.ai
 License: Apache-2.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `green-bit-llm-0.2.0/green_bit_llm.egg-info/SOURCES.txt` & `green_bit_llm-0.2.2/green_bit_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `green-bit-llm-0.2.0/setup.py` & `green_bit_llm-0.2.2/setup.py`

 * *Files identical despite different names*

