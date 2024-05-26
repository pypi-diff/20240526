# Comparing `tmp/nlpx-1.1.5.tar.gz` & `tmp/nlpx-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.1.5.tar", last modified: Sat May 25 13:32:15 2024, max compression
+gzip compressed data, was "nlpx-1.1.6.tar", last modified: Sat May 25 22:35:31 2024, max compression
```

## Comparing `nlpx-1.1.5.tar` & `nlpx-1.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.130393 nlpx-1.1.5/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 13:32:15.129726 nlpx-1.1.5/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.5/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.107550 nlpx-1.1.5/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.5/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.116559 nlpx-1.1.5/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)       87 2024-05-25 13:32:05.000000 nlpx-1.1.5/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     3289 2024-05-25 13:32:05.000000 nlpx-1.1.5/nlpx/llm/_model.py
--rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.5/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.125362 nlpx-1.1.5/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.5/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.5/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)    41938 2024-05-25 13:14:44.000000 nlpx-1.1.5/nlpx/text_token.py
--rw-r--r--   0 summy      (501) staff       (20)     3915 2024-05-25 12:52:10.000000 nlpx-1.1.5/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.113790 nlpx-1.1.5/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 13:32:14.000000 nlpx-1.1.5/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      339 2024-05-25 13:32:14.000000 nlpx-1.1.5/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 13:32:14.000000 nlpx-1.1.5/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.5/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 13:32:14.000000 nlpx-1.1.5/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 13:32:15.130613 nlpx-1.1.5/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1025 2024-05-25 13:32:05.000000 nlpx-1.1.5/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.127370 nlpx-1.1.5/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.5/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.355486 nlpx-1.1.6/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 22:35:31.354333 nlpx-1.1.6/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.6/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.327505 nlpx-1.1.6/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.6/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.344467 nlpx-1.1.6/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      122 2024-05-25 21:19:20.000000 nlpx-1.1.6/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     4610 2024-05-25 21:31:44.000000 nlpx-1.1.6/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.6/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.349225 nlpx-1.1.6/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.6/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.6/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)    41938 2024-05-25 13:14:44.000000 nlpx-1.1.6/nlpx/text_token.py
+-rw-r--r--   0 summy      (501) staff       (20)     3916 2024-05-25 22:26:52.000000 nlpx-1.1.6/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.333893 nlpx-1.1.6/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 22:35:31.000000 nlpx-1.1.6/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      347 2024-05-25 22:35:31.000000 nlpx-1.1.6/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 22:35:31.000000 nlpx-1.1.6/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.6/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 22:35:31.000000 nlpx-1.1.6/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 22:35:31.356033 nlpx-1.1.6/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1025 2024-05-25 22:35:25.000000 nlpx-1.1.6/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 22:35:31.351541 nlpx-1.1.6/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.6/test/test.py
```

### Comparing `nlpx-1.1.5/PKG-INFO` & `nlpx-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.5
+Version: 1.1.6
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.5/nlpx/llm/_model.py` & `nlpx-1.1.6/nlpx/llm/_model_wrapper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,110 @@
 import torch
+import numpy as np
 from torch import optim
 from pathlib import Path
 from typing import Union, List
-from nlpx.training import SimpleTrainer, evaluate
-from torch.utils.data import DataLoader, TensorDataset
+from torch.utils.data import DataLoader, TensorDataset, Dataset
+
 from nlpx.text_token import get_texts_max_length
+from nlpx.training import Trainer, SimpleTrainer, evaluate
 
 
-class Model:
+class ModelWrapper:
 
-	def __init__(self, tokenize_vec, model_path: Union[str, Path] = None, classes: List[str] = None,
+	def __init__(self, model_path: Union[str, Path], classes: List[str] = None,
 					device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
-		self.tokenize_vec = tokenize_vec
 		self.classes = classes
-		self.model = torch.load(model_path, map_location=device) if model_path else None
 		self.device = device
+		self.model = torch.load(model_path, map_location=device) if model_path else None
+
+	def train(self, train_set: Dataset, eval_set: Dataset, collate_fn=None, max_iter=100,
+				optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
+				batch_size=8, eval_batch_size=16,
+				num_workers=4, num_eval_workers=2,
+				early_stopping_rounds=10):
+		trainer = Trainer(self.model, train_set, eval_set, collate_fn,
+						  max_iter, optimizer, learning_rate, T_max,
+						  batch_size, eval_batch_size,
+						  num_workers, num_eval_workers,
+						  early_stopping_rounds,  # 早停，等10轮决策，评价指标不在变化，停止
+						  self.device)
+		self.model = trainer.train()
+
+	def predict(self, X: torch.FloatTensor):
+		self.model.eval()
+		with torch.no_grad():
+			logits = self.model(X)
+		return logits.argmax(1)
+
+	def predict_classes(self, X: torch.FloatTensor):
+		assert self.classes is not None, 'classes must be specified'
+		pred = self.predict(X)
+		return [self.classes[i] for i in pred.detach().numpy().ravel()]
+
+	def evaluate(self, eval_set: Dataset, batch_size=16, num_workers=0, max_length: int = 0,  collate_fn=None):
+		eval_loader = DataLoader(dataset=eval_set, batch_size=batch_size,
+								 num_workers=num_workers, collate_fn=collate_fn)
+		return evaluate(self.model, eval_loader, self.device)
+
+	def save(self, model_path: Union[str, Path]):
+		torch.save(model_path, self.model)
+
+	def load(self, model_path: Union[str, Path]):
+		self.model = torch.load(model_path, map_location=self.device)
+
 
-	def train(self, model, texts: List[str], y: torch.Tensor, max_length: int = None,
+class SimpleModelWrapper(ModelWrapper):
+
+	def __init__(self, tokenize_vec, model_path: Union[str, Path] = None, classes: List[str] = None,
+					device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
+		super().__init__(model_path, classes, device)
+		self.tokenize_vec = tokenize_vec
+
+	def train(self, model, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], max_length: int = 0,
 			  eval_size=0.2, random_state=None, collate_fn=None,max_iter=100,
 			  optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
 			  batch_size=8, eval_batch_size=16,
 			  num_workers=4, num_eval_workers=2,
 			  early_stopping_rounds=10):
-		max_length = max_length or self.get_max_length(texts)
+		max_length = self.get_max_length(texts, max_length)
 		X = self._get_vec(texts, max_length=max_length)
+		if isinstance(y, List) or isinstance(y, np.ndarray):
+			y = torch.tensor(y, dtype=torch.long)
 		trainer = SimpleTrainer(model, X, y, eval_size, random_state, collate_fn,
 								 max_iter, optimizer, learning_rate, T_max,
 								 batch_size, eval_batch_size,
 								 num_workers, num_eval_workers,
-								 early_stopping_rounds,  # 早停，等10轮决策，评价指标不在变化，停止
+								 early_stopping_rounds,
 								 self.device)
 		self.model = trainer.train()
 
-	def predict(self, texts: List[str]):
-		max_length = self.get_max_length(texts)
+	def predict(self, texts: List[str], max_length: int = 0):
+		max_length = self.get_max_length(texts, max_length)
 		X = self._get_vec(texts, max_length=max_length)
-		self.model.eval()
-		with torch.no_grad():
-			logits = self.model(X)
-		return logits.argmax(1)
+		return super().predict(X)
 
-	def predict_classes(self, texts: List[str]):
+	def predict_classes(self, texts: List[str], max_length: int = 0):
 		assert self.classes is not None, 'classes must be specified'
-		pred = self.predict(texts)
+		pred = self.predict(texts, max_length)
 		return [self.classes[i] for i in pred.detach().numpy().ravel()]
 
-	def evaluate(self, texts: List[str], y: torch.LongTensor, batch_size=16, num_workers=0, collate_fn=None):
-		max_length = self.get_max_length(texts)
+	def evaluate(self, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], batch_size=16, num_workers=0,
+				 max_length: int = 0, collate_fn=None):
+		max_length = self.get_max_length(texts, max_length)
 		X = self._get_vec(texts, max_length=max_length)
+		if isinstance(y, List) or isinstance(y, np.ndarray):
+			y = torch.tensor(y, dtype=torch.long)
 		eval_set = TensorDataset(X, y)
-		eval_loader = DataLoader(dataset=eval_set, batch_size=batch_size,
-								 num_workers=num_workers, collate_fn=collate_fn)
-		return evaluate(self.model, eval_loader, self.device)
+		return super().evaluate(eval_set, batch_size=batch_size, num_workers=num_workers, collate_fn=collate_fn)
+
+	@staticmethod
+	def get_max_length(texts: List[str], max_length: int = 0) -> int:
+		if max_length and max_length > 0:
+			return max_length
+		return get_texts_max_length(texts, cut_type='char')
 
 	def _get_vec(self, texts: List[str], max_length: int):
 		return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
 														truncation=True, add_special_tokens=True,
 														return_token_type_ids=True,return_attention_mask=True,
 														return_tensors='pt')
-
-	@staticmethod
-	def get_max_length(texts: List[str]) -> int:
-		return get_texts_max_length(texts, cut_type='char')
-
-
-# class SimpleModel:
-#
-# 	def __init__(self, tokenize_vec, model_path: Union[str, Path], classes: List[str] = None,
-# 					device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
-# 		self.tokenize_vec = tokenize_vec
-# 		self.classes = classes
-# 		self.model = torch.load(model_path, map_location=device) if model_path else None
-#
-# 	def train(self, train_set: Dataset, eval_set: Dataset, collate_fn=None,max_iter=100,
-# 				optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
-# 				batch_size=8, eval_batch_size=16,
-# 				num_workers=4, num_eval_workers=2,
-# 				early_stopping_rounds=10):
-
```

### Comparing `nlpx-1.1.5/nlpx/llm/_tokenize_vec.py` & `nlpx-1.1.6/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.5/nlpx/models/_text_cnn.py` & `nlpx-1.1.6/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.5/nlpx/text_token.py` & `nlpx-1.1.6/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.5/nlpx/training.py` & `nlpx-1.1.6/nlpx/training.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,16 +80,15 @@
 			if last_acc == val_acc:  # val_acc不在变化
 				cnt2 += 1
 			else:
 				cnt2 = 0
 
 			last_acc = val_acc
 			cnt += 1
-			if epoch > 5 and (
-					cnt > self.early_stopping_rounds or cnt2 > self.early_stopping_rounds):  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
+			if epoch >= min(5, self.early_stopping_rounds) and max(cnt, cnt2) >= self.early_stopping_rounds:  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
 				print("Early stopping at epoch-{}/{}".format(epoch + 1, self.max_iter))
 				break
 
 		return best_model
 
 
 class SimpleTrainer(Trainer):
```

### Comparing `nlpx-1.1.5/nlpx.egg-info/PKG-INFO` & `nlpx-1.1.6/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.5
+Version: 1.1.6
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.5/setup.py` & `nlpx-1.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.5',
+    version='1.1.6',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

