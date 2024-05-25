# Comparing `tmp/nlpx-1.1.4.tar.gz` & `tmp/nlpx-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.1.4.tar", last modified: Sat May 25 02:27:57 2024, max compression
+gzip compressed data, was "nlpx-1.1.5.tar", last modified: Sat May 25 13:32:15 2024, max compression
```

## Comparing `nlpx-1.1.4.tar` & `nlpx-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.187419 nlpx-1.1.4/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 02:27:57.186027 nlpx-1.1.4/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.4/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.170997 nlpx-1.1.4/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.4/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.179535 nlpx-1.1.4/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)       61 2024-05-25 01:16:11.000000 nlpx-1.1.4/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.4/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.183215 nlpx-1.1.4/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.4/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.4/nlpx/models/_text_cnn.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-1.1.4/nlpx/text_token.py
--rw-r--r--   0 summy      (501) staff       (20)     3856 2024-05-25 02:21:52.000000 nlpx-1.1.4/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.177246 nlpx-1.1.4/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 02:27:57.000000 nlpx-1.1.4/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      320 2024-05-25 02:27:57.000000 nlpx-1.1.4/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 02:27:57.000000 nlpx-1.1.4/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.4/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 02:27:57.000000 nlpx-1.1.4/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 02:27:57.189000 nlpx-1.1.4/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1025 2024-05-25 02:27:53.000000 nlpx-1.1.4/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 02:27:57.184127 nlpx-1.1.4/test/
--rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.4/test/test.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.130393 nlpx-1.1.5/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 13:32:15.129726 nlpx-1.1.5/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.1.5/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.107550 nlpx-1.1.5/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.1.5/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.116559 nlpx-1.1.5/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)       87 2024-05-25 13:32:05.000000 nlpx-1.1.5/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     3289 2024-05-25 13:32:05.000000 nlpx-1.1.5/nlpx/llm/_model.py
+-rw-r--r--   0 summy      (501) staff       (20)     8014 2024-05-25 01:46:32.000000 nlpx-1.1.5/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.125362 nlpx-1.1.5/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.1.5/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2932 2024-05-25 02:26:48.000000 nlpx-1.1.5/nlpx/models/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)    41938 2024-05-25 13:14:44.000000 nlpx-1.1.5/nlpx/text_token.py
+-rw-r--r--   0 summy      (501) staff       (20)     3915 2024-05-25 12:52:10.000000 nlpx-1.1.5/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.113790 nlpx-1.1.5/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-25 13:32:14.000000 nlpx-1.1.5/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      339 2024-05-25 13:32:14.000000 nlpx-1.1.5/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 13:32:14.000000 nlpx-1.1.5/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-25 01:23:04.000000 nlpx-1.1.5/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-25 13:32:14.000000 nlpx-1.1.5/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-25 13:32:15.130613 nlpx-1.1.5/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1025 2024-05-25 13:32:05.000000 nlpx-1.1.5/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-25 13:32:15.127370 nlpx-1.1.5/test/
+-rw-r--r--   0 summy      (501) staff       (20)      202 2024-05-25 00:36:45.000000 nlpx-1.1.5/test/test.py
```

### Comparing `nlpx-1.1.4/PKG-INFO` & `nlpx-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.4
+Version: 1.1.5
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.4/nlpx/llm/_tokenize_vec.py` & `nlpx-1.1.5/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.4/nlpx/models/_text_cnn.py` & `nlpx-1.1.5/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.1.4/nlpx/text_token.py` & `nlpx-1.1.5/nlpx/text_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from functools import reduce
 from typing import List, Union, Iterable, Any
 
 UTF8 = 'utf-8'
 REMOVE_CHARS = '[·’!"\#$%&\'()＃！（）*+,-./:;<=>?\@，：?￥★、…．＞【】［］《》？“”‘’\[\\]^_`{|}~]+'
 
 
+def get_texts_max_length(texts: List[str], language='cn', cut_type='word', keep_punctuation=False) -> int:
+    batch_cuts = batch_cut(texts, language, cut_type, keep_punctuation)
+    return max(list(map(lambda s: len(s), batch_cuts)))
+
+
 # -----------------------------------------------------------Read file-------------------------------------------------------------------
 def read_file(path: str, encoding=UTF8):
     """
     读取文件内容
     :param path: 文件名，不能是文件夹
     :param encoding: 编码
     :return: 包含非空文本行的生成器，如 ['上课时学生手机响个不停，老师一怒之下把手机摔了。', '家长拿发票让老师赔', ...]
```

### Comparing `nlpx-1.1.4/nlpx/training.py` & `nlpx-1.1.5/nlpx/training.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 import torch
-from torch import nn, optim
-from torch.utils.data import DataLoader, TensorDataset
+from torch import optim
+from torch.utils.data import DataLoader, TensorDataset, Dataset
 from torch.optim.lr_scheduler import CosineAnnealingLR
 from sklearn.model_selection import train_test_split
 
 
+def evaluate(model, eval_loader, device):
+	total = 0.0
+	losses = 0.0
+	correct = 0.0
+	model.eval()
+	with torch.no_grad():
+		for x, y in eval_loader:
+			x, y = x.to(device), y.to(device)
+			loss, logits = model(x, y)
+			correct += (logits.argmax(1) == y).sum().item()
+			losses += loss.item()
+			total += len(y)
+	return losses / total, correct / total
+
+
 class Trainer:
 
-	def __init__(self, model, train_set, eval_set, collate_fn=None,max_iter=100,
-				optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
-				batch_size=8, eval_batch_size=16,
-				num_workers=4, num_eval_workers=2,
-				early_stopping_rounds=10,  # 早停，等10轮决策，评价指标不在变化，停止
-				device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
-				):
+	def __init__(self, model, train_set: Dataset, eval_set: Dataset, collate_fn=None,
+				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
+				 batch_size=8, eval_batch_size=16,
+				 num_workers=4, num_eval_workers=2,
+				 early_stopping_rounds=10,  # 早停，等10轮决策，评价指标不在变化，停止
+				 device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')
+				 ):
 		self.model = model.to(device)
 		self.train_loader = DataLoader(dataset=train_set, batch_size=batch_size,
 									   num_workers=num_workers, shuffle=True, collate_fn=collate_fn)
 		self.eval_loader = DataLoader(dataset=eval_set, batch_size=eval_batch_size,
 									  num_workers=num_eval_workers, collate_fn=collate_fn)
 		self.max_iter = max_iter
 		self.optimizer = optimizer(model.parameters(), lr=learning_rate)
@@ -47,15 +62,15 @@
 				if self.T_max and self.T_max > 0:
 					scheduler.step()
 
 				losses += loss.item()
 				correct += (logits.argmax(1) == y).sum().item()
 				total += len(y)
 
-			val_loss, val_acc = self.eval()
+			val_loss, val_acc = evaluate(self.model, self.eval_loader, self.device)
 			print('epoch-{}/{}\tlr: {:.6f}, train_loss: {:.4f}, train_acc: {:.4f}, val_loss: {:.4f}, val_acc: {:.4f}'.format(
 				epoch + 1, self.max_iter, self.optimizer.param_groups[0]['lr'], losses / total, correct / total, val_loss, val_acc
 			))
 			if epoch > 5 and val_acc > best_acc:
 				best_acc = val_acc
 				best_model = self.model
 
@@ -72,28 +87,14 @@
 			if epoch > 5 and (
 					cnt > self.early_stopping_rounds or cnt2 > self.early_stopping_rounds):  # x次epoch的val_acc不提升或x次epoch的val_acc不变化
 				print("Early stopping at epoch-{}/{}".format(epoch + 1, self.max_iter))
 				break
 
 		return best_model
 
-	def eval(self):
-		total = 0.0
-		losses = 0.0
-		correct = 0.0
-		self.model.eval()
-		with torch.no_grad():
-			for x, y in self.eval_loader:
-				x, y = x.to(self.device), y.to(self.device)
-				loss, logits = self.model(x, y)
-				correct += (logits.argmax(1) == y).sum().item()
-				losses += loss.item()
-				total += len(y)
-		return losses / total, correct / total
-
 
 class SimpleTrainer(Trainer):
 
 	def __init__(self, model, X, y, eval_size=0.2, random_state=None, collate_fn=None,
 				 max_iter=100, optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
 				 batch_size=8, eval_batch_size=16,
 				 num_workers=4, num_eval_workers=2,
```

### Comparing `nlpx-1.1.4/nlpx.egg-info/PKG-INFO` & `nlpx-1.1.5/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.1.4
+Version: 1.1.5
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.1.4/setup.py` & `nlpx-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.1.4',
+    version='1.1.5',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

