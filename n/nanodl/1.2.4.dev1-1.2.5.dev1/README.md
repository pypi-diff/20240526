# Comparing `tmp/nanodl-1.2.4.dev1.tar.gz` & `tmp/nanodl-1.2.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanodl-1.2.4.dev1.tar", last modified: Sun May 12 20:02:22 2024, max compression
+gzip compressed data, was "nanodl-1.2.5.dev1.tar", last modified: Sun May 26 21:28:48 2024, max compression
```

## Comparing `nanodl-1.2.4.dev1.tar` & `nanodl-1.2.5.dev1.tar`

### file list

```diff
@@ -1,52 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.177702 nanodl-1.2.4.dev1/nanodl/
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-12 20:02:21.000000 nanodl-1.2.4.dev1/nanodl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.181702 nanodl-1.2.4.dev1/nanodl/__src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.181702 nanodl-1.2.4.dev1/nanodl/__src/classical/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/dsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/classical/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/nanodl/__src/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    28091 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)    21694 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    26729 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)    40104 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    28059 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/ijepa.py
--rw-r--r--   0 runner    (1001) docker     (127)    26261 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/lamda.py
--rw-r--r--   0 runner    (1001) docker     (127)    27736 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)    47242 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/mixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/reward.py
--rw-r--r--   0 runner    (1001) docker     (127)    29222 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/t5.py
--rw-r--r--   0 runner    (1001) docker     (127)    31917 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20510 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)    32356 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/models/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/nanodl/__src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/ml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/nanodl/__src/utils/vision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/nanodl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 20:02:22.000000 nanodl-1.2.4.dev1/nanodl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-12 20:02:21.000000 nanodl-1.2.4.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 20:02:22.185702 nanodl-1.2.4.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/tests/test_sklearn_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-12 20:02:12.000000 nanodl-1.2.4.dev1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:48.262506 nanodl-1.2.5.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-26 21:28:48.262506 nanodl-1.2.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:48.254505 nanodl-1.2.5.dev1/nanodl/
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-26 21:28:48.000000 nanodl-1.2.5.dev1/nanodl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:48.254505 nanodl-1.2.5.dev1/nanodl/__src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:48.254505 nanodl-1.2.5.dev1/nanodl/__src/classical/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/classical/bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/classical/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/classical/dimensionality_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/classical/dsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/classical/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:48.258505 nanodl-1.2.5.dev1/nanodl/__src/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/experimental/bitlinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/experimental/gat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8332 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/experimental/kan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21404 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/experimental/mamba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13098 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/experimental/rlhf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/experimental/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:48.258505 nanodl-1.2.5.dev1/nanodl/__src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22870 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28091 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21694 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26729 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40104 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28059 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/ijepa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26261 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/lamda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27736 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47242 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15511 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/reward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29222 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31917 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20510 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32356 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/models/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:48.262506 nanodl-1.2.5.dev1/nanodl/__src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8851 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/utils/ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/utils/nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10048 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/nanodl/__src/utils/vision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:48.262506 nanodl-1.2.5.dev1/nanodl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-05-26 21:28:48.000000 nanodl-1.2.5.dev1/nanodl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-26 21:28:48.000000 nanodl-1.2.5.dev1/nanodl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 21:28:48.000000 nanodl-1.2.5.dev1/nanodl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 21:28:48.000000 nanodl-1.2.5.dev1/nanodl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-26 21:28:48.000000 nanodl-1.2.5.dev1/nanodl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 21:28:48.262506 nanodl-1.2.5.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-26 21:28:48.000000 nanodl-1.2.5.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 21:28:48.262506 nanodl-1.2.5.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/tests/test_sklearn_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-26 21:28:40.000000 nanodl-1.2.5.dev1/tests/test_utils.py
```

### Comparing `nanodl-1.2.4.dev1/LICENSE` & `nanodl-1.2.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/PKG-INFO` & `nanodl-1.2.5.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanodl
-Version: 1.2.4.dev1
+Version: 1.2.5.dev1
 Summary: A Jax-based library for designing and training transformer models from scratch.
 Home-page: https://github.com/hmunachi/nanodl
 Author: Henry Ndubuaku
 Author-email: ndubuakuhenry@gmail.com
 Keywords: transformers jax machine learning deep learning pytorch tensorflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nanodl-1.2.4.dev1/README.md` & `nanodl-1.2.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__init__.py` & `nanodl-1.2.5.dev1/nanodl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.4.dev1"
+__version__ = "1.2.5.dev1"
 
 from nanodl.__src.classical.bayes import NaiveBayesClassifier
 from nanodl.__src.classical.clustering import GaussianMixtureModel, KMeans
 from nanodl.__src.classical.dimensionality_reduction import PCA
 from nanodl.__src.classical.regression import (
     GaussianProcess,
     LinearRegression,
```

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/classical/bayes.py` & `nanodl-1.2.5.dev1/nanodl/__src/classical/bayes.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/classical/clustering.py` & `nanodl-1.2.5.dev1/nanodl/__src/classical/clustering.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/classical/dimensionality_reduction.py` & `nanodl-1.2.5.dev1/nanodl/__src/classical/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/classical/dsp.py` & `nanodl-1.2.5.dev1/nanodl/__src/classical/dsp.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/classical/regression.py` & `nanodl-1.2.5.dev1/nanodl/__src/classical/regression.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/attention.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/attention.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/clip.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/clip.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/diffusion.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/diffusion.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/gemma.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/gemma.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/gpt.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/gpt.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/ijepa.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/ijepa.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/lamda.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/lamda.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/llama.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/llama.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/mistral.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/mistral.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/mixer.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/mixer.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/reward.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/reward.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/t5.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/t5.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/transformer.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/transformer.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/vit.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/vit.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/models/whisper.py` & `nanodl-1.2.5.dev1/nanodl/__src/models/whisper.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/utils/data.py` & `nanodl-1.2.5.dev1/nanodl/__src/utils/data.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/utils/ml.py` & `nanodl-1.2.5.dev1/nanodl/__src/utils/ml.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/utils/nlp.py` & `nanodl-1.2.5.dev1/nanodl/__src/utils/nlp.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/utils/random.py` & `nanodl-1.2.5.dev1/nanodl/__src/utils/random.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl/__src/utils/vision.py` & `nanodl-1.2.5.dev1/nanodl/__src/utils/vision.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/nanodl.egg-info/PKG-INFO` & `nanodl-1.2.5.dev1/nanodl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanodl
-Version: 1.2.4.dev1
+Version: 1.2.5.dev1
 Summary: A Jax-based library for designing and training transformer models from scratch.
 Home-page: https://github.com/hmunachi/nanodl
 Author: Henry Ndubuaku
 Author-email: ndubuakuhenry@gmail.com
 Keywords: transformers jax machine learning deep learning pytorch tensorflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nanodl-1.2.4.dev1/nanodl.egg-info/SOURCES.txt` & `nanodl-1.2.5.dev1/nanodl.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 nanodl/__src/__init__.py
 nanodl/__src/classical/__init__.py
 nanodl/__src/classical/bayes.py
 nanodl/__src/classical/clustering.py
 nanodl/__src/classical/dimensionality_reduction.py
 nanodl/__src/classical/dsp.py
 nanodl/__src/classical/regression.py
+nanodl/__src/experimental/__init__.py
+nanodl/__src/experimental/bitlinear.py
+nanodl/__src/experimental/gat.py
+nanodl/__src/experimental/kan.py
+nanodl/__src/experimental/mamba.py
+nanodl/__src/experimental/rlhf.py
+nanodl/__src/experimental/tokenizer.py
 nanodl/__src/models/__init__.py
 nanodl/__src/models/attention.py
 nanodl/__src/models/clip.py
 nanodl/__src/models/diffusion.py
 nanodl/__src/models/gemma.py
 nanodl/__src/models/gpt.py
 nanodl/__src/models/ijepa.py
```

### Comparing `nanodl-1.2.4.dev1/setup.py` & `nanodl-1.2.5.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="nanodl",
-    version="1.2.4.dev1",
+    version="1.2.5.dev1",
     author="Henry Ndubuaku",
     author_email="ndubuakuhenry@gmail.com",
     description="A Jax-based library for designing and training transformer models from scratch.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hmunachi/nanodl",
     packages=find_packages(),
```

### Comparing `nanodl-1.2.4.dev1/tests/test_models.py` & `nanodl-1.2.5.dev1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/tests/test_random.py` & `nanodl-1.2.5.dev1/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/tests/test_sklearn_gpu.py` & `nanodl-1.2.5.dev1/tests/test_sklearn_gpu.py`

 * *Files identical despite different names*

### Comparing `nanodl-1.2.4.dev1/tests/test_utils.py` & `nanodl-1.2.5.dev1/tests/test_utils.py`

 * *Files identical despite different names*

