# Comparing `tmp/gliner-0.1.9.tar.gz` & `tmp/gliner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-0.1.9.tar", last modified: Sun Apr 21 22:01:02 2024, max compression
+gzip compressed data, was "gliner-0.2.0.tar", last modified: Sun May 26 12:26:20 2024, max compression
```

## Comparing `gliner-0.1.9.tar` & `gliner-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-21 22:01:02.789799 gliner-0.1.9/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.1.9/LICENSE
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11188 2024-04-21 22:01:02.789509 gliner-0.1.9/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10463 2024-04-21 21:55:50.000000 gliner-0.1.9/README.md
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-21 22:01:02.785684 gliner-0.1.9/gliner/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-04-21 22:00:29.000000 gliner-0.1.9/gliner/__init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    20447 2024-04-01 10:36:39.000000 gliner-0.1.9/gliner/model.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-21 22:01:02.788897 gliner-0.1.9/gliner/modules/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.1.9/gliner/modules/__init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     6308 2024-04-21 21:59:59.000000 gliner-0.1.9/gliner/modules/base.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2350 2024-03-12 13:03:35.000000 gliner-0.1.9/gliner/modules/data_proc.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     4805 2024-04-09 17:30:41.000000 gliner-0.1.9/gliner/modules/evaluator.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1088 2024-03-12 13:03:35.000000 gliner-0.1.9/gliner/modules/layers.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-04-09 17:30:19.000000 gliner-0.1.9/gliner/modules/run_evaluation.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10357 2024-03-12 13:03:35.000000 gliner-0.1.9/gliner/modules/span_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-04-09 17:20:30.000000 gliner-0.1.9/gliner/modules/token_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1071 2024-04-01 02:23:01.000000 gliner-0.1.9/gliner/modules/token_splitter.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-04-21 22:01:02.789245 gliner-0.1.9/gliner.egg-info/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11188 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)      468 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/SOURCES.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/dependency_links.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       97 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/requires.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-04-21 22:01:02.000000 gliner-0.1.9/gliner.egg-info/top_level.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1046 2024-04-18 19:46:25.000000 gliner-0.1.9/pyproject.toml
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-04-21 22:01:02.789845 gliner-0.1.9/setup.cfg
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-26 12:26:20.461176 gliner-0.2.0/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.2.0/LICENSE
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    12205 2024-05-26 12:26:20.460907 gliner-0.2.0/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11480 2024-05-25 10:03:53.000000 gliner-0.2.0/README.md
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-26 12:26:20.456832 gliner-0.2.0/gliner/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-05-26 12:25:24.000000 gliner-0.2.0/gliner/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    14903 2024-05-26 04:58:35.000000 gliner-0.2.0/gliner/model.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-26 12:26:20.460203 gliner-0.2.0/gliner/modules/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.2.0/gliner/modules/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9988 2024-05-25 22:08:09.000000 gliner-0.2.0/gliner/modules/base.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     8330 2024-05-26 12:03:54.000000 gliner-0.2.0/gliner/modules/data.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2352 2024-05-25 16:08:03.000000 gliner-0.2.0/gliner/modules/data_proc.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5047 2024-04-22 09:17:20.000000 gliner-0.2.0/gliner/modules/evaluator.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     6248 2024-05-26 04:49:34.000000 gliner-0.2.0/gliner/modules/layers.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2148 2024-05-25 16:08:03.000000 gliner-0.2.0/gliner/modules/loss_functions.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-05-11 10:05:18.000000 gliner-0.2.0/gliner/modules/run_evaluation.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10015 2024-05-25 10:03:53.000000 gliner-0.2.0/gliner/modules/span_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-04-09 17:20:30.000000 gliner-0.2.0/gliner/modules/token_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1660 2024-04-24 10:13:06.000000 gliner-0.2.0/gliner/modules/token_splitter.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-26 12:26:20.460628 gliner-0.2.0/gliner.egg-info/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    12205 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)      524 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/SOURCES.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/dependency_links.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       97 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/requires.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/top_level.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1046 2024-04-24 10:21:08.000000 gliner-0.2.0/pyproject.toml
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-05-26 12:26:20.461218 gliner-0.2.0/setup.cfg
```

### Comparing `gliner-0.1.9/LICENSE` & `gliner-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gliner-0.1.9/PKG-INFO` & `gliner-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner
-Version: 0.1.9
+Version: 0.2.0
 Summary: Generalist model for NER (Extract any entity types from texts)
 Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
 Maintainer: Urchade Zaratiana
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/urchade/GLiNER
 Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
 Requires-Python: >=3.8
@@ -14,44 +14,59 @@
 Requires-Dist: transformers>=4.38.2
 Requires-Dist: huggingface_hub>=0.21.4
 Requires-Dist: flair==0.13.1
 Requires-Dist: scipy<=1.12
 Requires-Dist: seqeval
 Requires-Dist: tqdm
 
-# 🚀 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
+# 👑 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
 
 GLiNER is a Named Entity Recognition (NER) model capable of identifying any entity type using a bidirectional transformer encoder (BERT-like). It provides a practical alternative to traditional NER models, which are limited to predefined entities, and Large Language Models (LLMs) that, despite their flexibility, are costly and large for resource-constrained scenarios.
 
 * **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
 * **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
 * **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
+- 🔍 Join the GLiNER **discord** server: [https://discord.gg/Y2yVxpSQnG](https://discord.gg/Y2yVxpSQnG)
+- Synthetic data generation example is available (examples/synthetic_data_generation.ipynb).
 - 🆕 `gliner_multi_pii-v1` is available. This version has been optimized to recognize and classify Personally Identifiable Information (PII) within text. This version has been finetuned on six languages (English, French, German, Spanish, Italian, Portugese).
-- ⚙️ `pip install gliner>=0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
+- ⚙️ `pip install gliner>=0.1.12`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
 - 🚀 `gliner_multi-v2.1`, `gliner_small-v2.1`, `gliner_medium-v2.1`, and `gliner_large-v2.1` are available under the Apache 2.0 license.
 - 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
 - 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
-- 📘 Finetuning notebook is available: examples/finetune.ipynb
 - 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
 
+### Finetuning GLiNER
+- 📘 See this [directory](https://github.com/urchade/GLiNER/tree/main/examples/finetuning)
+
 ### 🌟 Available Models on Hugging Face
 
 #### 🇬🇧 For English
 - **GLiNER Base**: `urchade/gliner_base` *(CC BY NC 4.0)*
 - **GLiNER Small**: `urchade/gliner_small` *(CC BY NC 4.0)*
 - **GLiNER Small v2**: `urchade/gliner_small-v2` *(Apache 2.0)*
 - **GLiNER Small v2.1**: `urchade/gliner_small-v2.1` *(Apache 2.0)*
 - **GLiNER Medium**: `urchade/gliner_medium` *(CC BY NC 4.0)*
 - **GLiNER Medium v2**: `urchade/gliner_medium-v2` *(Apache 2.0)*
 - **GLiNER Medium v2.1**: `urchade/gliner_medium-v2.1` *(Apache 2.0)*
 - **GLiNER Large**: `urchade/gliner_large` *(CC BY NC 4.0)*
 - **GLiNER Large v2**: `urchade/gliner_large-v2` *(Apache 2.0)*
+- **GLiNER Large v2.1**: `urchade/gliner_large-v2.1` *(Apache 2.0)*
+
+
+- **GLiNER NuNerZero span**: `numind/NuNER_Zero-span`  *(MIT)* - +4.5% more powerful GLiNER Large v2.1
+- **GLiNER News**: `EmergentMethods/gliner_medium_news-v2.1` *(Apache 2.0)* 9.5% improvement over GLiNER Large v2.1 on 18 benchmark datasets
+
+##### 🇬🇧 English word-level Entity Recognition
+
+Word-level models work **better for finding multi-word entities, highlighting sentences or paragraphs**. They require additional output postprocessing that can be found in the corresponding model card.
+- **GLiNER NuNerZero**: `numind/NuNER_Zero`  *(MIT)* - +3% more powerful GLiNER Large v2.1, better suitable to detect multi-word entities
+- **GLiNER NuNerZero 4k context**: `numind/NuNER_Zero-4k`  *(MIT)* - 4k-long-context NuNerZero
 
 #### 🌍 For Other Languages
 - **Korean**: 🇰🇷 `taeminlee/gliner_ko`
 - **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
 - **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)* and `urchade/gliner_multi-v2.1` *(Apache 2.0)*
 
 #### 🔬 Domain Specific Models
@@ -156,26 +171,26 @@
 Microsoft => organization
 ```
 
 ##  📊 NER Benchmark Results
 
 <img align="center" src="https://cdn-uploads.huggingface.co/production/uploads/6317233cc92fd6fee317e030/Y5f7tK8lonGqeeO6L6bVI.png" />
 
-## 🛠️ Areas of Improvements / research
+## 🛠 Areas of Improvements / research
 
+- [ ] Extend the model to relation extraction. Our preliminary work [GraphER](https://github.com/urchade/GraphER).
 - [ ] Allow longer context (eg. train with long context transformers such as Longformer, LED, etc.)
 - [ ] Use Bi-encoder (entity encoder and span encoder) allowing precompute entity embeddings
 - [ ] Filtering mechanism to reduce number of spans before final classification to save memory and computation when the number entity types is large
 - [ ] Improve understanding of more detailed prompts/instruction, eg. "Find the first name of the person in the text"
 - [ ] Better loss function: for instance use ```Focal Loss``` (see [this paper](https://proceedings.neurips.cc/paper/2020/file/aeb7b30ef1d024a76f21a1d40e30c302-Paper.pdf)) instead of ```BCE``` to handle class imbalance, as some entity types are more frequent than others
 - [ ] Improve multi-lingual capabilities: train on more languages, and use multi-lingual training data
 - [ ] Decoding: allow a span to have multiple labels, eg: "Cristiano Ronaldo" is both a "person" and "football player"
 - [ ] Dynamic thresholding (in ```model.predict_entities(text, labels, threshold=0.5)```): allow the model to predict more entities, or less entities, depending on the context. Actually, the model tend to predict less entities where the entity type or the domain are not well represented in the training data.
 - [ ] Train with EMAs (Exponential Moving Averages) or merge multiple checkpoints to improve model robustness (see [this paper](https://openreview.net/forum?id=tq_J_MqB3UB))
-- [ ] Extend the model to relation extraction but need dataset with relation annotations. Our preliminary work [ATG](https://github.com/urchade/ATG).
 
 
 ## 👨‍💻 Model Authors
 The model authors are:
 * [Urchade Zaratiana](https://huggingface.co/urchade)
 * Nadi Tomeh
 * Pierre Holat
```

### Comparing `gliner-0.1.9/README.md` & `gliner-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,52 @@
-# 🚀 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
+# 👑 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
 
 GLiNER is a Named Entity Recognition (NER) model capable of identifying any entity type using a bidirectional transformer encoder (BERT-like). It provides a practical alternative to traditional NER models, which are limited to predefined entities, and Large Language Models (LLMs) that, despite their flexibility, are costly and large for resource-constrained scenarios.
 
 * **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
 * **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
 * **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
+- 🔍 Join the GLiNER **discord** server: [https://discord.gg/Y2yVxpSQnG](https://discord.gg/Y2yVxpSQnG)
+- Synthetic data generation example is available (examples/synthetic_data_generation.ipynb).
 - 🆕 `gliner_multi_pii-v1` is available. This version has been optimized to recognize and classify Personally Identifiable Information (PII) within text. This version has been finetuned on six languages (English, French, German, Spanish, Italian, Portugese).
-- ⚙️ `pip install gliner>=0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
+- ⚙️ `pip install gliner>=0.1.12`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
 - 🚀 `gliner_multi-v2.1`, `gliner_small-v2.1`, `gliner_medium-v2.1`, and `gliner_large-v2.1` are available under the Apache 2.0 license.
 - 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
 - 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
-- 📘 Finetuning notebook is available: examples/finetune.ipynb
 - 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
 
+### Finetuning GLiNER
+- 📘 See this [directory](https://github.com/urchade/GLiNER/tree/main/examples/finetuning)
+
 ### 🌟 Available Models on Hugging Face
 
 #### 🇬🇧 For English
 - **GLiNER Base**: `urchade/gliner_base` *(CC BY NC 4.0)*
 - **GLiNER Small**: `urchade/gliner_small` *(CC BY NC 4.0)*
 - **GLiNER Small v2**: `urchade/gliner_small-v2` *(Apache 2.0)*
 - **GLiNER Small v2.1**: `urchade/gliner_small-v2.1` *(Apache 2.0)*
 - **GLiNER Medium**: `urchade/gliner_medium` *(CC BY NC 4.0)*
 - **GLiNER Medium v2**: `urchade/gliner_medium-v2` *(Apache 2.0)*
 - **GLiNER Medium v2.1**: `urchade/gliner_medium-v2.1` *(Apache 2.0)*
 - **GLiNER Large**: `urchade/gliner_large` *(CC BY NC 4.0)*
 - **GLiNER Large v2**: `urchade/gliner_large-v2` *(Apache 2.0)*
+- **GLiNER Large v2.1**: `urchade/gliner_large-v2.1` *(Apache 2.0)*
+
+
+- **GLiNER NuNerZero span**: `numind/NuNER_Zero-span`  *(MIT)* - +4.5% more powerful GLiNER Large v2.1
+- **GLiNER News**: `EmergentMethods/gliner_medium_news-v2.1` *(Apache 2.0)* 9.5% improvement over GLiNER Large v2.1 on 18 benchmark datasets
+
+##### 🇬🇧 English word-level Entity Recognition
+
+Word-level models work **better for finding multi-word entities, highlighting sentences or paragraphs**. They require additional output postprocessing that can be found in the corresponding model card.
+- **GLiNER NuNerZero**: `numind/NuNER_Zero`  *(MIT)* - +3% more powerful GLiNER Large v2.1, better suitable to detect multi-word entities
+- **GLiNER NuNerZero 4k context**: `numind/NuNER_Zero-4k`  *(MIT)* - 4k-long-context NuNerZero
 
 #### 🌍 For Other Languages
 - **Korean**: 🇰🇷 `taeminlee/gliner_ko`
 - **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
 - **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)* and `urchade/gliner_multi-v2.1` *(Apache 2.0)*
 
 #### 🔬 Domain Specific Models
@@ -136,26 +151,26 @@
 Microsoft => organization
 ```
 
 ##  📊 NER Benchmark Results
 
 <img align="center" src="https://cdn-uploads.huggingface.co/production/uploads/6317233cc92fd6fee317e030/Y5f7tK8lonGqeeO6L6bVI.png" />
 
-## 🛠️ Areas of Improvements / research
+## 🛠 Areas of Improvements / research
 
+- [ ] Extend the model to relation extraction. Our preliminary work [GraphER](https://github.com/urchade/GraphER).
 - [ ] Allow longer context (eg. train with long context transformers such as Longformer, LED, etc.)
 - [ ] Use Bi-encoder (entity encoder and span encoder) allowing precompute entity embeddings
 - [ ] Filtering mechanism to reduce number of spans before final classification to save memory and computation when the number entity types is large
 - [ ] Improve understanding of more detailed prompts/instruction, eg. "Find the first name of the person in the text"
 - [ ] Better loss function: for instance use ```Focal Loss``` (see [this paper](https://proceedings.neurips.cc/paper/2020/file/aeb7b30ef1d024a76f21a1d40e30c302-Paper.pdf)) instead of ```BCE``` to handle class imbalance, as some entity types are more frequent than others
 - [ ] Improve multi-lingual capabilities: train on more languages, and use multi-lingual training data
 - [ ] Decoding: allow a span to have multiple labels, eg: "Cristiano Ronaldo" is both a "person" and "football player"
 - [ ] Dynamic thresholding (in ```model.predict_entities(text, labels, threshold=0.5)```): allow the model to predict more entities, or less entities, depending on the context. Actually, the model tend to predict less entities where the entity type or the domain are not well represented in the training data.
 - [ ] Train with EMAs (Exponential Moving Averages) or merge multiple checkpoints to improve model robustness (see [this paper](https://openreview.net/forum?id=tq_J_MqB3UB))
-- [ ] Extend the model to relation extraction but need dataset with relation annotations. Our preliminary work [ATG](https://github.com/urchade/ATG).
 
 
 ## 👨‍💻 Model Authors
 The model authors are:
 * [Urchade Zaratiana](https://huggingface.co/urchade)
 * Nadi Tomeh
 * Pierre Holat
```

### Comparing `gliner-0.1.9/gliner/modules/data_proc.py` & `gliner-0.2.0/gliner/modules/data_proc.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import ast, re
 
 path = 'train.json'
 
 with open(path, 'r') as f:
     data = json.load(f)
 
+
 def tokenize_text(text):
     return re.findall(r'\w+(?:[-_]\w+)*|\S', text)
 
+
 def extract_entity_spans(entry):
     text = ""
     len_start = len("What describes ")
     len_end = len(" in the text?")
     entity_types = []
     entity_texts = []
 
@@ -48,26 +50,25 @@
             if " ".join(tokenized_text[i:i + len(entity_tokens)]).lower() == " ".join(entity_tokens).lower():
                 matches.append((i, i + len(entity_tokens) - 1, entity_types[j]))
         if matches:
             entity_spans.extend(matches)
 
     return entity_spans, tokenized_text
 
+
 # Usage:
 # Replace 'entry' with the specific entry from your JSON data
 entry = data[17818]  # For example, taking the first entry
 entity_spans, tokenized_text = extract_entity_spans(entry)
 print("Entity Spans:", entity_spans)
-#print("Tokenized Text:", tokenized_text)
+# print("Tokenized Text:", tokenized_text)
 
 # create a dict: {"tokenized_text": tokenized_text, "entity_spans": entity_spans}
 
 all_data = []
 
 for entry in tqdm(data):
     entity_spans, tokenized_text = extract_entity_spans(entry)
     all_data.append({"tokenized_text": tokenized_text, "ner": entity_spans})
 
-
 with open('train_instruct.json', 'w') as f:
     json.dump(all_data, f)
-
```

### Comparing `gliner-0.1.9/gliner/modules/evaluator.py` & `gliner-0.2.0/gliner/modules/evaluator.py`

 * *Files 14% similar despite different names*

```diff
@@ -113,48 +113,50 @@
 
 
 def is_nested(idx1, idx2):
     # Return True if idx2 is nested inside idx1 or vice versa
     return (idx1[0] <= idx2[0] and idx1[1] >= idx2[1]) or (idx2[0] <= idx1[0] and idx2[1] >= idx1[1])
 
 
-def has_overlapping(idx1, idx2):
-    overlapping = True
-    if idx1[:2] == idx2[:2]:
-        return overlapping
-    if (idx1[0] > idx2[1] or idx2[0] > idx1[1]):
-        overlapping = False
-    return overlapping
+def has_overlapping(idx1, idx2, multi_label=False):
+    # Check for any overlap between two spans
+    if idx1[:2] == idx2[:2]:  # Exact same boundaries can be considered as overlapping
+        return not multi_label
+    if idx1[0] > idx2[1] or idx2[0] > idx1[1]:
+        return False
+    return True
 
 
-def has_overlapping_nested(idx1, idx2):
+def has_overlapping_nested(idx1, idx2, multi_label=False):
     # Return True if idx1 and idx2 overlap, but neither is nested inside the other
-    if idx1[:2] == idx2[:2]:
-        return True
-    if ((idx1[0] > idx2[1] or idx2[0] > idx1[1]) or is_nested(idx1, idx2)) and idx1 != idx2:
+    if idx1[:2] == idx2[:2]:  # Exact same boundaries, not considering labels here
+        return not multi_label
+    if (idx1[0] > idx2[1] or idx2[0] > idx1[1]) or is_nested(idx1, idx2):
         return False
-    else:
-        return True
+    return True
+
 
+from functools import partial
 
-def greedy_search(spans, flat_ner=True):  # start, end, class, score
+
+def greedy_search(spans, flat_ner=True, multi_label=False):  # start, end, class, score
 
     if flat_ner:
-        has_ov = has_overlapping
+        has_ov = partial(has_overlapping, multi_label=multi_label)
     else:
-        has_ov = has_overlapping_nested
+        has_ov = partial(has_overlapping_nested, multi_label=multi_label)
 
     new_list = []
     span_prob = sorted(spans, key=lambda x: -x[-1])
-    
+
     for i in range(len(spans)):
         b = span_prob[i]
         flag = False
         for new in new_list:
             if has_ov(b[:-1], new):
                 flag = True
                 break
         if not flag:
             new_list.append(b)
-            
+
     new_list = sorted(new_list, key=lambda x: x[0])
     return new_list
```

### Comparing `gliner-0.1.9/gliner/modules/run_evaluation.py` & `gliner-0.2.0/gliner/modules/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.9/gliner/modules/span_rep.py` & `gliner-0.2.0/gliner/modules/span_rep.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,12 @@
 import torch
 import torch.nn.functional as F
 from torch import nn
 
-def create_projection_layer(hidden_size: int, dropout: float, out_dim: int = None) -> nn.Sequential:
-    """
-    Creates a projection layer with specified configurations.
-    """
-    if out_dim is None:
-        out_dim = hidden_size
-
-    return nn.Sequential(
-        nn.Linear(hidden_size, out_dim * 4),
-        nn.ReLU(),
-        nn.Dropout(dropout),
-        nn.Linear(out_dim * 4, out_dim)
-    )
-
+from gliner.modules.layers import create_projection_layer
 
 class SpanQuery(nn.Module):
 
     def __init__(self, hidden_size, max_width, trainable=True):
         super().__init__()
 
         self.query_seg = nn.Parameter(torch.randn(hidden_size, max_width))
```

### Comparing `gliner-0.1.9/gliner/modules/token_rep.py` & `gliner-0.2.0/gliner/modules/token_rep.py`

 * *Files identical despite different names*

### Comparing `gliner-0.1.9/gliner.egg-info/PKG-INFO` & `gliner-0.2.0/gliner.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner
-Version: 0.1.9
+Version: 0.2.0
 Summary: Generalist model for NER (Extract any entity types from texts)
 Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
 Maintainer: Urchade Zaratiana
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/urchade/GLiNER
 Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
 Requires-Python: >=3.8
@@ -14,44 +14,59 @@
 Requires-Dist: transformers>=4.38.2
 Requires-Dist: huggingface_hub>=0.21.4
 Requires-Dist: flair==0.13.1
 Requires-Dist: scipy<=1.12
 Requires-Dist: seqeval
 Requires-Dist: tqdm
 
-# 🚀 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
+# 👑 GLiNER: Generalist and Lightweight Model for Named Entity Recognition
 
 GLiNER is a Named Entity Recognition (NER) model capable of identifying any entity type using a bidirectional transformer encoder (BERT-like). It provides a practical alternative to traditional NER models, which are limited to predefined entities, and Large Language Models (LLMs) that, despite their flexibility, are costly and large for resource-constrained scenarios.
 
 * **Paper**: 📄 [GLiNER: Generalist Model for Named Entity Recognition using Bidirectional Transformer](https://arxiv.org/abs/2311.08526)
 * **Getting Started:** &nbsp; [<img align="center" src="https://colab.research.google.com/assets/colab-badge.svg" />](https://colab.research.google.com/drive/1mhalKWzmfSTqMnR0wQBZvt9-ktTsATHB?usp=sharing)
 * **Demo:** 🤗 [Hugging Face](https://huggingface.co/spaces/urchade/gliner_mediumv2.1)
 
 ## Models Status
 ### 📢 Updates
+- 🔍 Join the GLiNER **discord** server: [https://discord.gg/Y2yVxpSQnG](https://discord.gg/Y2yVxpSQnG)
+- Synthetic data generation example is available (examples/synthetic_data_generation.ipynb).
 - 🆕 `gliner_multi_pii-v1` is available. This version has been optimized to recognize and classify Personally Identifiable Information (PII) within text. This version has been finetuned on six languages (English, French, German, Spanish, Italian, Portugese).
-- ⚙️ `pip install gliner>=0.1.7`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
+- ⚙️ `pip install gliner>=0.1.12`: Some of the previous versions contain a bug that causes bad performance. Please use version the newest version.
 - 🚀 `gliner_multi-v2.1`, `gliner_small-v2.1`, `gliner_medium-v2.1`, and `gliner_large-v2.1` are available under the Apache 2.0 license.
 - 🆕 [gliner-spacy](https://github.com/theirstory/gliner-spacy) is available. Install it with `pip install gliner-spacy`. See Example of usage [below](https://github.com/urchade/GLiNER/tree/main#-usage-with-spacy).
 - 🧬 `gliner_large_bio-v0.1` is a gliner model specialized for biomedical text. It is available under the Apache 2.0 license.
-- 📘 Finetuning notebook is available: examples/finetune.ipynb
 - 📚 Training dataset preprocessing scripts are now available in the `data/` directory, covering both [Pile-NER](https://huggingface.co/datasets/Universal-NER/Pile-NER-type) and [NuNER](https://huggingface.co/datasets/numind/NuNER) datasets.
 
+### Finetuning GLiNER
+- 📘 See this [directory](https://github.com/urchade/GLiNER/tree/main/examples/finetuning)
+
 ### 🌟 Available Models on Hugging Face
 
 #### 🇬🇧 For English
 - **GLiNER Base**: `urchade/gliner_base` *(CC BY NC 4.0)*
 - **GLiNER Small**: `urchade/gliner_small` *(CC BY NC 4.0)*
 - **GLiNER Small v2**: `urchade/gliner_small-v2` *(Apache 2.0)*
 - **GLiNER Small v2.1**: `urchade/gliner_small-v2.1` *(Apache 2.0)*
 - **GLiNER Medium**: `urchade/gliner_medium` *(CC BY NC 4.0)*
 - **GLiNER Medium v2**: `urchade/gliner_medium-v2` *(Apache 2.0)*
 - **GLiNER Medium v2.1**: `urchade/gliner_medium-v2.1` *(Apache 2.0)*
 - **GLiNER Large**: `urchade/gliner_large` *(CC BY NC 4.0)*
 - **GLiNER Large v2**: `urchade/gliner_large-v2` *(Apache 2.0)*
+- **GLiNER Large v2.1**: `urchade/gliner_large-v2.1` *(Apache 2.0)*
+
+
+- **GLiNER NuNerZero span**: `numind/NuNER_Zero-span`  *(MIT)* - +4.5% more powerful GLiNER Large v2.1
+- **GLiNER News**: `EmergentMethods/gliner_medium_news-v2.1` *(Apache 2.0)* 9.5% improvement over GLiNER Large v2.1 on 18 benchmark datasets
+
+##### 🇬🇧 English word-level Entity Recognition
+
+Word-level models work **better for finding multi-word entities, highlighting sentences or paragraphs**. They require additional output postprocessing that can be found in the corresponding model card.
+- **GLiNER NuNerZero**: `numind/NuNER_Zero`  *(MIT)* - +3% more powerful GLiNER Large v2.1, better suitable to detect multi-word entities
+- **GLiNER NuNerZero 4k context**: `numind/NuNER_Zero-4k`  *(MIT)* - 4k-long-context NuNerZero
 
 #### 🌍 For Other Languages
 - **Korean**: 🇰🇷 `taeminlee/gliner_ko`
 - **Italian**: 🇮🇹 `DeepMount00/universal_ner_ita`
 - **Multilingual**: 🌐 `urchade/gliner_multi` *(CC BY NC 4.0)* and `urchade/gliner_multi-v2.1` *(Apache 2.0)*
 
 #### 🔬 Domain Specific Models
@@ -156,26 +171,26 @@
 Microsoft => organization
 ```
 
 ##  📊 NER Benchmark Results
 
 <img align="center" src="https://cdn-uploads.huggingface.co/production/uploads/6317233cc92fd6fee317e030/Y5f7tK8lonGqeeO6L6bVI.png" />
 
-## 🛠️ Areas of Improvements / research
+## 🛠 Areas of Improvements / research
 
+- [ ] Extend the model to relation extraction. Our preliminary work [GraphER](https://github.com/urchade/GraphER).
 - [ ] Allow longer context (eg. train with long context transformers such as Longformer, LED, etc.)
 - [ ] Use Bi-encoder (entity encoder and span encoder) allowing precompute entity embeddings
 - [ ] Filtering mechanism to reduce number of spans before final classification to save memory and computation when the number entity types is large
 - [ ] Improve understanding of more detailed prompts/instruction, eg. "Find the first name of the person in the text"
 - [ ] Better loss function: for instance use ```Focal Loss``` (see [this paper](https://proceedings.neurips.cc/paper/2020/file/aeb7b30ef1d024a76f21a1d40e30c302-Paper.pdf)) instead of ```BCE``` to handle class imbalance, as some entity types are more frequent than others
 - [ ] Improve multi-lingual capabilities: train on more languages, and use multi-lingual training data
 - [ ] Decoding: allow a span to have multiple labels, eg: "Cristiano Ronaldo" is both a "person" and "football player"
 - [ ] Dynamic thresholding (in ```model.predict_entities(text, labels, threshold=0.5)```): allow the model to predict more entities, or less entities, depending on the context. Actually, the model tend to predict less entities where the entity type or the domain are not well represented in the training data.
 - [ ] Train with EMAs (Exponential Moving Averages) or merge multiple checkpoints to improve model robustness (see [this paper](https://openreview.net/forum?id=tq_J_MqB3UB))
-- [ ] Extend the model to relation extraction but need dataset with relation annotations. Our preliminary work [ATG](https://github.com/urchade/ATG).
 
 
 ## 👨‍💻 Model Authors
 The model authors are:
 * [Urchade Zaratiana](https://huggingface.co/urchade)
 * Nadi Tomeh
 * Pierre Holat
```

### Comparing `gliner-0.1.9/pyproject.toml` & `gliner-0.2.0/pyproject.toml`

 * *Files identical despite different names*

