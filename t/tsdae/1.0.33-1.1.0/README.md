# Comparing `tmp/tsdae-1.0.33.tar.gz` & `tmp/tsdae-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsdae-1.0.33.tar", last modified: Sat Feb  3 23:58:36 2024, max compression
+gzip compressed data, was "tsdae-1.1.0.tar", last modified: Sun May 26 11:47:48 2024, max compression
```

## Comparing `tsdae-1.0.33.tar` & `tsdae-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-02-03 23:58:36.958417 tsdae-1.0.33/
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)    11357 2024-01-29 19:54:24.000000 tsdae-1.0.33/LICENSE
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     7082 2024-02-03 23:58:36.957709 tsdae-1.0.33/PKG-INFO
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     6209 2024-02-03 23:24:59.000000 tsdae-1.0.33/README.md
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     1711 2024-02-03 23:58:24.000000 tsdae-1.0.33/pyproject.toml
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)       38 2024-02-03 23:58:36.958698 tsdae-1.0.33/setup.cfg
-drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-02-03 23:58:36.949270 tsdae-1.0.33/src/
-drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-02-03 23:58:36.953543 tsdae-1.0.33/src/tsdae/
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)      205 2024-02-03 22:03:12.000000 tsdae-1.0.33/src/tsdae/__init__.py
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)    29297 2024-02-03 23:58:06.000000 tsdae-1.0.33/src/tsdae/tsdae.py
-drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-02-03 23:58:36.956834 tsdae-1.0.33/src/tsdae.egg-info/
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     7082 2024-02-03 23:58:36.000000 tsdae-1.0.33/src/tsdae.egg-info/PKG-INFO
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)      205 2024-02-03 23:58:36.000000 tsdae-1.0.33/src/tsdae.egg-info/SOURCES.txt
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)        1 2024-02-03 23:58:36.000000 tsdae-1.0.33/src/tsdae.egg-info/dependency_links.txt
--rw-r--r--   0 louisbrulenaudet   (501) staff       (20)        6 2024-02-03 23:58:36.000000 tsdae-1.0.33/src/tsdae.egg-info/top_level.txt
+drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 11:47:48.142215 tsdae-1.1.0/
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)    11357 2024-05-26 11:31:17.000000 tsdae-1.1.0/LICENSE
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     7081 2024-05-26 11:47:48.141452 tsdae-1.1.0/PKG-INFO
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     6209 2024-05-26 11:31:17.000000 tsdae-1.1.0/README.md
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     1709 2024-05-26 11:47:21.000000 tsdae-1.1.0/pyproject.toml
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)       38 2024-05-26 11:47:48.142447 tsdae-1.1.0/setup.cfg
+drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 11:47:48.132254 tsdae-1.1.0/src/
+drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 11:47:48.136900 tsdae-1.1.0/src/tsdae/
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)      205 2024-05-26 11:31:17.000000 tsdae-1.1.0/src/tsdae/__init__.py
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)    29376 2024-05-26 11:31:17.000000 tsdae-1.1.0/src/tsdae/tsdae.py
+drwxr-xr-x   0 louisbrulenaudet   (501) staff       (20)        0 2024-05-26 11:47:48.140562 tsdae-1.1.0/src/tsdae.egg-info/
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)     7081 2024-05-26 11:47:48.000000 tsdae-1.1.0/src/tsdae.egg-info/PKG-INFO
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)      205 2024-05-26 11:47:48.000000 tsdae-1.1.0/src/tsdae.egg-info/SOURCES.txt
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)        1 2024-05-26 11:47:48.000000 tsdae-1.1.0/src/tsdae.egg-info/dependency_links.txt
+-rw-r--r--   0 louisbrulenaudet   (501) staff       (20)        6 2024-05-26 11:47:48.000000 tsdae-1.1.0/src/tsdae.egg-info/top_level.txt
```

### Comparing `tsdae-1.0.33/LICENSE` & `tsdae-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsdae-1.0.33/PKG-INFO` & `tsdae-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsdae
-Version: 1.0.33
+Version: 1.1.0
 Summary: Tranformer-based Denoising AutoEncoder for Sentence Transformers Unsupervised pre-training.
 Keywords: transformers,sentence-transformers,tsdae,bert,machine-learning,NLP,sentence-similarity,nltk,pre-training,embeddings
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tsdae-1.0.33/README.md` & `tsdae-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tsdae-1.0.33/pyproject.toml` & `tsdae-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tsdae"
-version = "1.0.33"
+version = "1.1.0"
 description = "Tranformer-based Denoising AutoEncoder for Sentence Transformers Unsupervised pre-training."
 readme = "README.md"
 keywords = ["transformers", "sentence-transformers", "tsdae", "bert", "machine-learning", "NLP", "sentence-similarity", "nltk", "pre-training", "embeddings"]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Education",
@@ -29,15 +29,15 @@
     "datasets",
     "sentence_transformers",
     "torch"
 ]
 
 [metadata]
 name = "tsdae"
-version = "1.0.33"
+version = "1.1.0"
 license = "Apache License 2.0"
 author = "Louis Brulé Naudet"
 author_email = "louisbrulenaudet@icloud.com"
 description = "Tranformer-based Denoising AutoEncoder for Sentence Transformers Unsupervised pre-training."
 long_description = "file: README.md"
 long_description_content_type = "text/markdown"
 url = "https://github.com/louisbrulenaudet/balena"
```

### Comparing `tsdae-1.0.33/src/tsdae/tsdae.py` & `tsdae-1.1.0/src/tsdae/tsdae.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # limitations under the License.
 
 import re
 import ssl
 import nltk
 import random
 import logging
-from typing import Union, Optional, List
-from datasets import concatenate_datasets, load_dataset, Dataset, IterableDataset
+from typing import Union, Optional
+from datasets import concatenate_datasets, load_dataset, Dataset
 
 from sentence_transformers.datasets import DenoisingAutoEncoderDataset
 from torch.utils.data import DataLoader
 
 from sentence_transformers import SentenceTransformer, models
 from sentence_transformers.losses import DenoisingAutoEncoderLoss
 
@@ -313,16 +313,16 @@
         except Exception as e:
             self.logger.error(f"Error in shuffle_datasets: {str(e)}")
             return dataset
 
 
     def splitter_config(
         self,
-        regex: Optional[any]=re.compile(r'\.\s?\n?')
-        ) -> any:
+        regex: Optional[Pattern]=re.compile(r'\.\s?\n?')
+        ) -> Pattern:
         """
         Configures and returns a compiled regular expression pattern for text splitting.
 
         Parameters
         ----------
         regex : Optional[re.Pattern], optional
             A compiled regular expression pattern for text splitting. Default is `r'\.\s?\n?'`.
@@ -404,15 +404,15 @@
         )
 
 
     def constrain_dataset(
         self,
         shuffled_dataset:Union[List[Dataset], Dataset, IterableDataset],
         column:str,
-        splitter:any,
+        splitter:re.Pattern,
         num_to_keep:int=100000,
         total_sentences:int=100000,
         num_chars:Optional[int] = 40
         ) -> list:
         """
         Processes shuffled datasets to constrain the number of sentences in a dataset.
 
@@ -504,15 +504,15 @@
             raise Exception(f"Error in constrain_dataset: {str(e)}")
 
 
     def create_denoising_loader(
         self,
         sentences: list,
         batch_size: Optional[int] = 4
-        ) -> any:
+        ) -> DataLoader:
         """
         Creates a DataLoader with noise functionality for a DenoisingAutoEncoderDataset.
 
         Parameters
         ----------
         sentences : list
             List of sentences to be used in the dataset.
@@ -561,15 +561,15 @@
             raise Exception(f"Error in create_denoising_loader: {str(e)}")
 
 
     def create_sentence_transformer_model(
         self,
         model_name:str="bert-base-multilingual-uncased",
         pooling_method:Optional[str]="cls"
-        ) -> any:
+        ) -> SentenceTransformer:
         """
         Creates a SentenceTransformer model using a specified transformer and pooling method.
 
         Parameters
         ----------
         model_name : str, optional
             The name of the transformer model to use. Default is "bert-base-multilingual-uncased".
@@ -620,17 +620,17 @@
             raise Exception(
                 f"Error in create_sentence_transformer_model: {str(e)}"
             )
 
 
     def create_denoising_autoencoder_loss(
         self,
-        model:any,
+        model:SentenceTransformer,
         tie_encoder_decoder:Optional[bool]=True
-        ) -> any:
+        ) -> DenoisingAutoEncoderLoss:
         """
         Creates a DenoisingAutoEncoderLoss object for a given model.
 
         Parameters
         ----------
         model : SentenceTransformer
             SentenceTransformer model initialized with the specified transformer and pooling methods.
@@ -675,16 +675,16 @@
             )
 
 
     def train_model(
         self,
         model:any,
         output_path:str,
-        loader:any,
-        loss:any,
+        loader:DataLoader,
+        loss:DenoisingAutoEncoderLoss,
         epochs:int=1,
         weight_decay:float=0,
         scheduler:str="constantlr",
         optimizer_params:dict={"lr": 3e-5},
         show_progress_bar:bool=True
         ) -> None:
         """
@@ -852,15 +852,15 @@
 
             # Configure splitter
             splitter = self.splitter_config()
 
             # Constrain dataset
             constrained_data = self.constrain_dataset(
                 shuffled_dataset=shuffled_dataset,
-                column="output",
+                column=column,
                 splitter=splitter,
                 num_to_keep=num_to_keep,
                 total_sentences=total_sentences,
                 num_chars=num_chars
             )
 
             # Create DataLoader
@@ -900,8 +900,8 @@
 
         except TypeError as te:
             raise TypeError(f"TypeError in train: {str(te)}")
             return None
 
         except Exception as e:
             raise Exception(f"Error in train: {str(e)}")
-            return None
+            return None
```

### Comparing `tsdae-1.0.33/src/tsdae.egg-info/PKG-INFO` & `tsdae-1.1.0/src/tsdae.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsdae
-Version: 1.0.33
+Version: 1.1.0
 Summary: Tranformer-based Denoising AutoEncoder for Sentence Transformers Unsupervised pre-training.
 Keywords: transformers,sentence-transformers,tsdae,bert,machine-learning,NLP,sentence-similarity,nltk,pre-training,embeddings
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

