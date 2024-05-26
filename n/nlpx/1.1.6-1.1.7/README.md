# Comparing `tmp/nlpx-1.1.6.tar.gz` & `tmp/nlpx-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.1.6.tar", last modified: Sat May 25 22:35:31 2024, max compression
+gzip compressed data, was "nlpx-1.1.7.tar", last modified: Sun May 26 05:47:47 2024, max compression
```

## Comparing `nlpx-1.1.6.tar` & `nlpx-1.1.7.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.355486 nlpx-1.1.6/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 22:35:31.354333 nlpx-1.1.6/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.6/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.327505 nlpx-1.1.6/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.6/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.344467 nlpx-1.1.6/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.1.6/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     4610 2024-05-25 21:31:44.000000 nlpx-1.1.6/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.6/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.349225 nlpx-1.1.6/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.6/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.6/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)    41938 2024-05-25 13:14:44.000000 nlpx-1.1.6/nlpx/text_token.py
--rw-r--r--   0 summy      (501) staff       (20)     3916 2024-05-25 22:26:52.000000 nlpx-1.1.6/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.333893 nlpx-1.1.6/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 22:35:31.000000 nlpx-1.1.6/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      347 2024-05-25 22:35:31.000000 nlpx-1.1.6/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 22:35:31.000000 nlpx-1.1.6/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.6/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 22:35:31.000000 nlpx-1.1.6/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 22:35:31.356033 nlpx-1.1.6/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1025 2024-05-25 22:35:25.000000 nlpx-1.1.6/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.351541 nlpx-1.1.6/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.6/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.962214 nlpx-1.1.7/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-26 05:47:47.961166 nlpx-1.1.7/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.7/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.940409 nlpx-1.1.7/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.7/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.949961 nlpx-1.1.7/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.1.7/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5102 2024-05-26 05:21:03.000000 nlpx-1.1.7/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.7/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.954087 nlpx-1.1.7/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.7/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.7/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.958375 nlpx-1.1.7/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.1.7/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25392 2024-05-26 05:41:52.000000 nlpx-1.1.7/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.1.7/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     3916 2024-05-25 22:26:52.000000 nlpx-1.1.7/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.944349 nlpx-1.1.7/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      412 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-26 05:47:47.000000 nlpx-1.1.7/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-26 05:47:47.962702 nlpx-1.1.7/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-26 05:47:41.000000 nlpx-1.1.7/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-26 05:47:47.959548 nlpx-1.1.7/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.7/test/test.py
```

### Comparing `nlpx-1.1.6/PKG-INFO` & `nlpx-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.6
+Version: 1.1.7
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.6/nlpx/llm/_model_wrapper.py` & `nlpx-1.1.7/nlpx/llm/_model_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import torch
 import numpy as np
 from torch import optim
 from pathlib import Path
 from typing import Union, List
+from torch.nn import functional as F
 from torch.utils.data import DataLoader, TensorDataset, Dataset
 
 from nlpx.text_token import get_texts_max_length
 from nlpx.training import Trainer, SimpleTrainer, evaluate
 
 
 class ModelWrapper:
@@ -27,28 +28,38 @@
 						  batch_size, eval_batch_size,
 						  num_workers, num_eval_workers,
 						  early_stopping_rounds,  # 早停，等10轮决策，评价指标不在变化，停止
 						  self.device)
 		self.model = trainer.train()
 
 	def predict(self, X: torch.FloatTensor):
-		self.model.eval()
-		with torch.no_grad():
-			logits = self.model(X)
+		logits = self._predict(X)
 		return logits.argmax(1)
 
 	def predict_classes(self, X: torch.FloatTensor):
 		assert self.classes is not None, 'classes must be specified'
 		pred = self.predict(X)
 		return [self.classes[i] for i in pred.detach().numpy().ravel()]
 
+	def predict_proba(self, X: torch.FloatTensor):
+		logits = self._predict(X)
+		result = F.softmax(logits).max(1)
+		return result.indices, result.values
+
+	def _predict(self, X: torch.FloatTensor):
+		self.model.eval()
+		with torch.no_grad():
+			logits = self.model(X)
+		return logits
+
 	def evaluate(self, eval_set: Dataset, batch_size=16, num_workers=0, max_length: int = 0,  collate_fn=None):
 		eval_loader = DataLoader(dataset=eval_set, batch_size=batch_size,
 								 num_workers=num_workers, collate_fn=collate_fn)
-		return evaluate(self.model, eval_loader, self.device)
+		_, acc = evaluate(self.model, eval_loader, self.device)
+		return acc
 
 	def save(self, model_path: Union[str, Path]):
 		torch.save(model_path, self.model)
 
 	def load(self, model_path: Union[str, Path]):
 		self.model = torch.load(model_path, map_location=self.device)
 
@@ -63,48 +74,53 @@
 	def train(self, model, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], max_length: int = 0,
 			  eval_size=0.2, random_state=None, collate_fn=None,max_iter=100,
 			  optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
 			  batch_size=8, eval_batch_size=16,
 			  num_workers=4, num_eval_workers=2,
 			  early_stopping_rounds=10):
 		max_length = self.get_max_length(texts, max_length)
-		X = self._get_vec(texts, max_length=max_length)
+		X = self.get_vec(texts, max_length=max_length)
 		if isinstance(y, List) or isinstance(y, np.ndarray):
 			y = torch.tensor(y, dtype=torch.long)
 		trainer = SimpleTrainer(model, X, y, eval_size, random_state, collate_fn,
 								 max_iter, optimizer, learning_rate, T_max,
 								 batch_size, eval_batch_size,
 								 num_workers, num_eval_workers,
 								 early_stopping_rounds,
 								 self.device)
 		self.model = trainer.train()
 
 	def predict(self, texts: List[str], max_length: int = 0):
 		max_length = self.get_max_length(texts, max_length)
-		X = self._get_vec(texts, max_length=max_length)
+		X = self.get_vec(texts, max_length=max_length)
 		return super().predict(X)
 
 	def predict_classes(self, texts: List[str], max_length: int = 0):
 		assert self.classes is not None, 'classes must be specified'
 		pred = self.predict(texts, max_length)
 		return [self.classes[i] for i in pred.detach().numpy().ravel()]
+	
+	def predict_proba(self, texts: List[str], max_length: int = 0):
+		max_length = self.get_max_length(texts, max_length)
+		X = self.get_vec(texts, max_length=max_length)
+		return super().predict_proba(X)
 
 	def evaluate(self, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], batch_size=16, num_workers=0,
 				 max_length: int = 0, collate_fn=None):
 		max_length = self.get_max_length(texts, max_length)
-		X = self._get_vec(texts, max_length=max_length)
+		X = self.get_vec(texts, max_length=max_length)
 		if isinstance(y, List) or isinstance(y, np.ndarray):
 			y = torch.tensor(y, dtype=torch.long)
 		eval_set = TensorDataset(X, y)
 		return super().evaluate(eval_set, batch_size=batch_size, num_workers=num_workers, collate_fn=collate_fn)
 
 	@staticmethod
 	def get_max_length(texts: List[str], max_length: int = 0) -> int:
 		if max_length and max_length > 0:
 			return max_length
 		return get_texts_max_length(texts, cut_type='char')
 
-	def _get_vec(self, texts: List[str], max_length: int):
+	def get_vec(self, texts: List[str], max_length: int):
 		return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
 														truncation=True, add_special_tokens=True,
 														return_token_type_ids=True,return_attention_mask=True,
 														return_tensors='pt')
```

### Comparing `nlpx-1.1.6/nlpx/llm/_tokenize_vec.py` & `nlpx-1.1.7/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.6/nlpx/models/_text_cnn.py` & `nlpx-1.1.7/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.6/nlpx/training.py` & `nlpx-1.1.7/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.6/nlpx.egg-info/PKG-INFO` & `nlpx-1.1.7/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.6
+Version: 1.1.7
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.6/setup.py` & `nlpx-1.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 
 long_description = read("README.rst")
 
 
 setup(
     name='nlpx',
-    packages=['nlpx', 'nlpx.models', 'nlpx.llm'],
+    packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.6',
+    version='1.1.7',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

