# Comparing `tmp/dltrain-0.1.2.tar.gz` & `tmp/dltrain-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dltrain-0.1.2.tar", last modified: Wed May  8 06:35:18 2024, max compression
+gzip compressed data, was "dltrain-0.1.3.tar", last modified: Sun May 26 15:34:41 2024, max compression
```

## Comparing `dltrain-0.1.2.tar` & `dltrain-0.1.3.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.815354 dltrain-0.1.2/
--rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6714 2024-05-08 06:35:18.814354 dltrain-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6077 2024-05-08 06:33:51.000000 dltrain-0.1.2/README.md
--rw-rw-rw-   0        0        0      625 2024-05-08 02:25:24.000000 dltrain-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 06:35:18.815354 dltrain-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.579814 dltrain-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.678369 dltrain-0.1.2/src/dltrain/
--rw-rw-rw-   0        0        0      229 2024-05-05 13:13:52.000000 dltrain-0.1.2/src/dltrain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.788369 dltrain-0.1.2/src/dltrain/builder/
--rw-rw-rw-   0        0        0       32 2024-05-04 13:43:22.000000 dltrain-0.1.2/src/dltrain/builder/__init__.py
--rw-rw-rw-   0        0        0     1207 2024-05-07 01:28:09.000000 dltrain-0.1.2/src/dltrain/builder/base.py
--rw-rw-rw-   0        0        0     3219 2024-05-07 03:07:53.000000 dltrain-0.1.2/src/dltrain/builder/builder.py
--rw-rw-rw-   0        0        0      212 2024-05-04 13:37:24.000000 dltrain-0.1.2/src/dltrain/builder/core.py
--rw-rw-rw-   0        0        0      714 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/builder/criterion.py
--rw-rw-rw-   0        0        0     2264 2024-05-08 02:25:24.000000 dltrain-0.1.2/src/dltrain/builder/dataset.py
--rw-rw-rw-   0        0        0      721 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/builder/delineator.py
--rw-rw-rw-   0        0        0     1556 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/builder/evaluation.py
--rw-rw-rw-   0        0        0      488 2024-05-07 01:12:49.000000 dltrain-0.1.2/src/dltrain/builder/forward.py
--rw-rw-rw-   0        0        0      281 2024-05-07 03:07:32.000000 dltrain-0.1.2/src/dltrain/builder/inject.py
--rw-rw-rw-   0        0        0      861 2024-05-08 02:46:50.000000 dltrain-0.1.2/src/dltrain/builder/model.py
--rw-rw-rw-   0        0        0     1169 2024-05-07 01:28:56.000000 dltrain-0.1.2/src/dltrain/builder/optimizer.py
--rw-rw-rw-   0        0        0      533 2024-05-04 13:52:21.000000 dltrain-0.1.2/src/dltrain/builder/scheduler.py
--rw-rw-rw-   0        0        0      834 2024-05-08 02:35:03.000000 dltrain-0.1.2/src/dltrain/builder/transforms.py
--rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.1.2/src/dltrain/checkpoint.py
--rw-rw-rw-   0        0        0     5177 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/dataset.py
--rw-rw-rw-   0        0        0     1300 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/delineator.py
--rw-rw-rw-   0        0        0      935 2024-05-03 11:30:58.000000 dltrain-0.1.2/src/dltrain/error.py
--rw-rw-rw-   0        0        0     3949 2024-05-05 13:08:13.000000 dltrain-0.1.2/src/dltrain/evaluation.py
--rw-rw-rw-   0        0        0     6478 2024-05-07 02:10:02.000000 dltrain-0.1.2/src/dltrain/forward.py
--rw-rw-rw-   0        0        0     1203 2024-05-07 03:07:32.000000 dltrain-0.1.2/src/dltrain/inject.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.811359 dltrain-0.1.2/src/dltrain/models/
--rw-rw-rw-   0        0        0      101 2024-05-08 02:46:50.000000 dltrain-0.1.2/src/dltrain/models/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-05-08 06:15:11.000000 dltrain-0.1.2/src/dltrain/models/component.py
--rw-rw-rw-   0        0        0     1607 2024-05-08 02:46:50.000000 dltrain-0.1.2/src/dltrain/models/model.py
--rw-rw-rw-   0        0        0     3040 2024-05-08 02:46:50.000000 dltrain-0.1.2/src/dltrain/models/wrapper.py
--rw-rw-rw-   0        0        0     1290 2024-04-07 09:09:29.000000 dltrain-0.1.2/src/dltrain/options.py
--rw-rw-rw-   0        0        0    11930 2024-05-07 02:10:30.000000 dltrain-0.1.2/src/dltrain/train.py
--rw-rw-rw-   0        0        0     1405 2024-05-08 02:35:03.000000 dltrain-0.1.2/src/dltrain/transform.py
--rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.1.2/src/dltrain/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 06:35:18.813355 dltrain-0.1.2/src/dltrain.egg-info/
--rw-rw-rw-   0        0        0     6714 2024-05-08 06:35:18.000000 dltrain-0.1.2/src/dltrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1015 2024-05-08 06:35:18.000000 dltrain-0.1.2/src/dltrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:35:18.000000 dltrain-0.1.2/src/dltrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-08 06:35:18.000000 dltrain-0.1.2/src/dltrain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.300329 dltrain-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6988 2024-05-26 15:34:41.299329 dltrain-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6351 2024-05-26 15:34:09.000000 dltrain-0.1.3/README.md
+-rw-rw-rw-   0        0        0      625 2024-05-21 08:07:45.000000 dltrain-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:34:41.300329 dltrain-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.079808 dltrain-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.158810 dltrain-0.1.3/src/dltrain/
+-rw-rw-rw-   0        0        0      229 2024-05-05 13:13:52.000000 dltrain-0.1.3/src/dltrain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.259332 dltrain-0.1.3/src/dltrain/builder/
+-rw-rw-rw-   0        0        0       32 2024-05-04 13:43:22.000000 dltrain-0.1.3/src/dltrain/builder/__init__.py
+-rw-rw-rw-   0        0        0     1366 2024-05-23 07:36:29.000000 dltrain-0.1.3/src/dltrain/builder/base.py
+-rw-rw-rw-   0        0        0     3219 2024-05-07 03:07:53.000000 dltrain-0.1.3/src/dltrain/builder/builder.py
+-rw-rw-rw-   0        0        0      212 2024-05-04 13:37:24.000000 dltrain-0.1.3/src/dltrain/builder/core.py
+-rw-rw-rw-   0        0        0      714 2024-05-05 13:08:13.000000 dltrain-0.1.3/src/dltrain/builder/criterion.py
+-rw-rw-rw-   0        0        0     2264 2024-05-08 02:25:24.000000 dltrain-0.1.3/src/dltrain/builder/dataset.py
+-rw-rw-rw-   0        0        0      721 2024-05-05 13:08:13.000000 dltrain-0.1.3/src/dltrain/builder/delineator.py
+-rw-rw-rw-   0        0        0     1556 2024-05-05 13:08:13.000000 dltrain-0.1.3/src/dltrain/builder/evaluation.py
+-rw-rw-rw-   0        0        0      488 2024-05-07 01:12:49.000000 dltrain-0.1.3/src/dltrain/builder/forward.py
+-rw-rw-rw-   0        0        0      281 2024-05-07 03:07:32.000000 dltrain-0.1.3/src/dltrain/builder/inject.py
+-rw-rw-rw-   0        0        0     1454 2024-05-21 09:17:11.000000 dltrain-0.1.3/src/dltrain/builder/model.py
+-rw-rw-rw-   0        0        0     1169 2024-05-07 01:28:56.000000 dltrain-0.1.3/src/dltrain/builder/optimizer.py
+-rw-rw-rw-   0        0        0      533 2024-05-04 13:52:21.000000 dltrain-0.1.3/src/dltrain/builder/scheduler.py
+-rw-rw-rw-   0        0        0      834 2024-05-08 02:35:03.000000 dltrain-0.1.3/src/dltrain/builder/transforms.py
+-rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.1.3/src/dltrain/checkpoint.py
+-rw-rw-rw-   0        0        0     5857 2024-05-26 15:34:09.000000 dltrain-0.1.3/src/dltrain/dataset.py
+-rw-rw-rw-   0        0        0     1300 2024-05-05 13:08:13.000000 dltrain-0.1.3/src/dltrain/delineator.py
+-rw-rw-rw-   0        0        0      935 2024-05-03 11:30:58.000000 dltrain-0.1.3/src/dltrain/error.py
+-rw-rw-rw-   0        0        0     3955 2024-05-26 15:27:39.000000 dltrain-0.1.3/src/dltrain/evaluation.py
+-rw-rw-rw-   0        0        0     6478 2024-05-07 02:10:02.000000 dltrain-0.1.3/src/dltrain/forward.py
+-rw-rw-rw-   0        0        0     1203 2024-05-07 03:07:32.000000 dltrain-0.1.3/src/dltrain/inject.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.296328 dltrain-0.1.3/src/dltrain/models/
+-rw-rw-rw-   0        0        0      150 2024-05-21 09:08:46.000000 dltrain-0.1.3/src/dltrain/models/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-05-21 09:08:46.000000 dltrain-0.1.3/src/dltrain/models/builder.py
+-rw-rw-rw-   0        0        0     1617 2024-05-21 09:08:46.000000 dltrain-0.1.3/src/dltrain/models/component.py
+-rw-rw-rw-   0        0        0     1975 2024-05-26 15:34:09.000000 dltrain-0.1.3/src/dltrain/models/model.py
+-rw-rw-rw-   0        0        0     3040 2024-05-08 02:46:50.000000 dltrain-0.1.3/src/dltrain/models/wrapper.py
+-rw-rw-rw-   0        0        0     1326 2024-05-23 06:05:54.000000 dltrain-0.1.3/src/dltrain/options.py
+-rw-rw-rw-   0        0        0    13122 2024-05-21 08:05:29.000000 dltrain-0.1.3/src/dltrain/train.py
+-rw-rw-rw-   0        0        0     1405 2024-05-08 02:35:03.000000 dltrain-0.1.3/src/dltrain/transform.py
+-rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.1.3/src/dltrain/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:34:41.298329 dltrain-0.1.3/src/dltrain.egg-info/
+-rw-rw-rw-   0        0        0     6988 2024-05-26 15:34:41.000000 dltrain-0.1.3/src/dltrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2024-05-26 15:34:41.000000 dltrain-0.1.3/src/dltrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:34:41.000000 dltrain-0.1.3/src/dltrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 15:34:41.000000 dltrain-0.1.3/src/dltrain.egg-info/top_level.txt
```

### Comparing `dltrain-0.1.2/LICENSE` & `dltrain-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/PKG-INFO` & `dltrain-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,18 @@
 # dltrain
 这是一个 PyTorch 训练包，本项目提供了大量的高级训练 API 和低级接口，满足所有训练需求
 <br/>
 安装仅在Shell中使用pip安装即可
 ```bash
 pip install dltrain
 ```
+利用该工具包我们可用通过如下结构构建训练代码
+<img src="img/dltrain.png"/>
+
+## Example
 ### example .1 在iris数据集上使用多层感知器进行分类
 ```python
 from dltrain import TaskBuilder, SimpleTrainer
 
 builder = TaskBuilder('iris')
 builder.base.use_epoch(100).use_batch_size(8).use_device('cuda')
 builder.model.use_mlp(4, 3)
@@ -88,15 +92,15 @@
 builder.evaluation_handler.add_accuracy()
 builder.delineator.use_train_eval(builder.dataset.use_mnist('./dataset', True),
                                   builder.dataset.use_mnist('./dataset', False))
 SimpleTrainer().run(builder.build())
 ```
 模型向导对象的use_model接口允许用户传入自己的模型
 
-### Example .2.1 使用torchvision的自带模型
+### example .2.1 使用torchvision的自带模型
 ```python
 from dltrain import TaskBuilder, SimpleTrainer
 
 builder = TaskBuilder('mnist')
 builder.model.use_pytorch_model('resnet18', num_classes=10)
 builder.base.use_device('cuda')
 builder.optimizer.use_adam()
@@ -133,31 +137,34 @@
 
     swin_b, swin_t, swin_s, swin_v2_b, swin_v2_t, swin_v2_s,
 
     mnasnet0_5, mnasnet1_0, mnasnet1_3, mnasnet0_75
 ]
 ```
 ### default about the arguments
-| 参数名称             | 默认值                                                |
+| 参数名称             | 默认值                                                |    
 |------------------|----------------------------------------------------|
 | optimizer        | Sgd(lr=0.01,momentum=0,dampening=0,weight_decay=0) |
 | scheduler        | User-set                                           |
 | criterion*       | None,Must be specified by the user                 |    
 | model*           | None,Must be specified by the user                 |
 | epoch            | 10                                                 |
 | batch_size       | 16                                                 |
 | seed             | 3407                                               |
 | device           | cpu                                                |
 | save_checkpoint  | False                                              |
-| start_checkpoint | User-set                                           |
+| start_checkpoint | None,User-set                                      |
 | delineator*      | None,Must be specified by the user                 |
 | forward          | SimpleForward                                      |
 | trainer          | SimpleTrainer                                      |
 
 ## Version Log
 - 0.0.1<br/>
 1、构造整体模型框架
 - 0.0.2<br/>
 1、加入了TaskBuilder方便构造模型
 - 0.1.2<br/>
-1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)
+1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)<br/>
 2、将models.py封装到models包，添加了许多拆箱可用模型
+- 0.1.3<br/>
+1、引入错误处理机制，防止由于EventHandler设置问题导致的结果保存错误<br/>
+2、引入VectorSequenceDataset<br/>
```

### Comparing `dltrain-0.1.2/README.md` & `dltrain-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # dltrain
 这是一个 PyTorch 训练包，本项目提供了大量的高级训练 API 和低级接口，满足所有训练需求
 <br/>
 安装仅在Shell中使用pip安装即可
 ```bash
 pip install dltrain
 ```
+利用该工具包我们可用通过如下结构构建训练代码
+<img src="img/dltrain.png"/>
+
+## Example
 ### example .1 在iris数据集上使用多层感知器进行分类
 ```python
 from dltrain import TaskBuilder, SimpleTrainer
 
 builder = TaskBuilder('iris')
 builder.base.use_epoch(100).use_batch_size(8).use_device('cuda')
 builder.model.use_mlp(4, 3)
@@ -74,15 +78,15 @@
 builder.evaluation_handler.add_accuracy()
 builder.delineator.use_train_eval(builder.dataset.use_mnist('./dataset', True),
                                   builder.dataset.use_mnist('./dataset', False))
 SimpleTrainer().run(builder.build())
 ```
 模型向导对象的use_model接口允许用户传入自己的模型
 
-### Example .2.1 使用torchvision的自带模型
+### example .2.1 使用torchvision的自带模型
 ```python
 from dltrain import TaskBuilder, SimpleTrainer
 
 builder = TaskBuilder('mnist')
 builder.model.use_pytorch_model('resnet18', num_classes=10)
 builder.base.use_device('cuda')
 builder.optimizer.use_adam()
@@ -119,31 +123,34 @@
 
     swin_b, swin_t, swin_s, swin_v2_b, swin_v2_t, swin_v2_s,
 
     mnasnet0_5, mnasnet1_0, mnasnet1_3, mnasnet0_75
 ]
 ```
 ### default about the arguments
-| 参数名称             | 默认值                                                |
+| 参数名称             | 默认值                                                |    
 |------------------|----------------------------------------------------|
 | optimizer        | Sgd(lr=0.01,momentum=0,dampening=0,weight_decay=0) |
 | scheduler        | User-set                                           |
 | criterion*       | None,Must be specified by the user                 |    
 | model*           | None,Must be specified by the user                 |
 | epoch            | 10                                                 |
 | batch_size       | 16                                                 |
 | seed             | 3407                                               |
 | device           | cpu                                                |
 | save_checkpoint  | False                                              |
-| start_checkpoint | User-set                                           |
+| start_checkpoint | None,User-set                                      |
 | delineator*      | None,Must be specified by the user                 |
 | forward          | SimpleForward                                      |
 | trainer          | SimpleTrainer                                      |
 
 ## Version Log
 - 0.0.1<br/>
 1、构造整体模型框架
 - 0.0.2<br/>
 1、加入了TaskBuilder方便构造模型
 - 0.1.2<br/>
-1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)
+1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)<br/>
 2、将models.py封装到models包，添加了许多拆箱可用模型
+- 0.1.3<br/>
+1、引入错误处理机制，防止由于EventHandler设置问题导致的结果保存错误<br/>
+2、引入VectorSequenceDataset<br/>
```

### Comparing `dltrain-0.1.2/pyproject.toml` & `dltrain-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dltrain"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="XiaosYu", email="lijingyu_ai@163.com" },
 ]
 description = "This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dltrain-0.1.2/src/dltrain/builder/base.py` & `dltrain-0.1.3/src/dltrain/builder/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,35 +10,43 @@
     def __init__(self):
         self._batch_size = 16
         self._seed = 3407
         self._start_checkpoint: str = None
         self._save_checkpoint: bool = False
         self._epochs: int = 10
         self._device: torch.device = torch.device('cpu')
+        self._log_level: int = 0
 
     def use_batch_size(self, bs):
         self._batch_size = bs
         return self
 
     def use_seed(self, seed):
         self._seed = seed
         return self
 
-    def set_checkpoint(self, checkpoint: bool = False):
-        self._save_checkpoint = checkpoint
+    def use_log_level(self, level: int):
+        self._log_level = level
         return self
 
-    def use_checkpoint(self, checkpoint: str) -> CheckPoint:
+    def use_log_loss(self):
+        pass
+
+    def use_checkpoint(self):
+        self._save_checkpoint = True
+        return self
+
+    def use_checkpoint_path(self, checkpoint: str) -> CheckPoint:
         self._start_checkpoint = torch.load(checkpoint)
         return self._start_checkpoint
 
     def use_epoch(self, epochs: int = 10):
         self._epochs = epochs
         return self
 
-    def use_device(self, device: Union[torch.device, str]):
+    def use_device(self, device: Union[torch.device, str] = 'cuda'):
         if isinstance(device, str):
             self._device = torch.device(device)
         elif isinstance(device, torch.device):
             self._device = device
 
         return self
```

### Comparing `dltrain-0.1.2/src/dltrain/builder/builder.py` & `dltrain-0.1.3/src/dltrain/builder/builder.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/builder/criterion.py` & `dltrain-0.1.3/src/dltrain/builder/criterion.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/builder/dataset.py` & `dltrain-0.1.3/src/dltrain/builder/dataset.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/builder/delineator.py` & `dltrain-0.1.3/src/dltrain/builder/delineator.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/builder/evaluation.py` & `dltrain-0.1.3/src/dltrain/builder/evaluation.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/builder/optimizer.py` & `dltrain-0.1.3/src/dltrain/builder/optimizer.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/builder/scheduler.py` & `dltrain-0.1.3/src/dltrain/builder/scheduler.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/builder/transforms.py` & `dltrain-0.1.3/src/dltrain/builder/transforms.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/checkpoint.py` & `dltrain-0.1.3/src/dltrain/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/dataset.py` & `dltrain-0.1.3/src/dltrain/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import torch
 from torch.utils.data import Dataset, DataLoader
 from torch import Tensor, cat
 from abc import ABCMeta, abstractmethod
 from .error import check_length, try_convert, raise_error
 
 import os
@@ -65,14 +66,33 @@
     def index_of(self, idx):
         return None
 
     def get_length(self):
         return 0
 
 
+class VectorSequenceDataset(DLDataset):
+    def __init__(self, data, seq_length=3):
+        # data shape like [batch_size, features_length]
+        # convert shape like [batch_size, seq_length, features_length]
+        data = np.array(data)
+        data = np.lib.stride_tricks.sliding_window_view(data, window_shape=(seq_length + 1, len(data[0]))).reshape(
+            (-1, seq_length + 1, data.shape[1]))
+        self.data = data
+
+    def get_length(self):
+        return self.data.shape[0]
+
+    def index_of(self, idx):
+        seq = self.data[idx]
+        features = seq[: -1]
+        targets = seq[-1]
+        return features, targets
+
+
 class PyTorchNativeDataset(DLDataset):
     def __init__(self, dataset):
         self.dataset = dataset
 
     def index_of(self, idx):
         return self.dataset[idx]
```

### Comparing `dltrain-0.1.2/src/dltrain/delineator.py` & `dltrain-0.1.3/src/dltrain/delineator.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/error.py` & `dltrain-0.1.3/src/dltrain/error.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/evaluation.py` & `dltrain-0.1.3/src/dltrain/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,21 +18,24 @@
 
 
 class Evaluation:
     def __init__(self):
         self.predictions = None
         self.exacts = None
 
+
     def append(self, prediction):
         self.predictions = prediction if self.predictions is None else torch.cat([self.predictions, prediction], dim=0)
 
     def reset(self):
         self.predictions = None
 
 
+
+
 class EvaluationHandler(metaclass=ABCMeta):
     def __init__(self, drawable=False):
         self.drawable = drawable
 
     def __call__(self, *args, **kwargs):
         return self.compute(*args, **kwargs)
```

### Comparing `dltrain-0.1.2/src/dltrain/forward.py` & `dltrain-0.1.3/src/dltrain/forward.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/inject.py` & `dltrain-0.1.3/src/dltrain/inject.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/models/component.py` & `dltrain-0.1.3/src/dltrain/models/component.py`

 * *Files 22% similar despite different names*

```diff
@@ -50,18 +50,7 @@
         data = data.reshape(data.shape[0], 1, -1)
         data = self.conv_list(data)
         data = data.reshape(data.shape[0], -1)
         data = self.linear_avg(data)
         return data
 
 
-class TaskModel(nn.Module):
-    def __init__(self, feature_model: nn.Module, header_model: nn.Module):
-        super().__init__()
-
-        self.feature_model = feature_model
-        self.header_model = header_model
-
-    def forward(self, data):
-        data = self.feature_model(data)
-        data = self.header_model(data)
-        return data
```

### Comparing `dltrain-0.1.2/src/dltrain/models/model.py` & `dltrain-0.1.3/src/dltrain/models/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 __Activation__ = [
     Sigmoid, ReLU, LeakyReLU, Tanh, Hardswish,
     BatchNorm1d, BatchNorm2d, LazyBatchNorm1d
 ]
 
 __all__ = [
-    'MultilayerPerceptron'
+    'MultilayerPerceptron',
+    'TaskModel'
 ]
 
 
 class MultilayerPerceptron(Module):
     def __init__(self, features, targets, layers=None, activation='sigmoid'):
         super().__init__()
 
@@ -43,7 +44,20 @@
         self.layers = Sequential(
             *modules
         )
 
     def forward(self, data):
         data = data.reshape(data.shape[0], -1)
         return self.layers(data)
+
+
+class TaskModel(Module):
+    def __init__(self, feature_model: Module, header_model: Module):
+        super().__init__()
+
+        self.feature_model = feature_model
+        self.header_model = header_model
+
+    def forward(self, data):
+        data = self.feature_model(data)
+        data = self.header_model(data)
+        return data
```

### Comparing `dltrain-0.1.2/src/dltrain/models/wrapper.py` & `dltrain-0.1.3/src/dltrain/models/wrapper.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/options.py` & `dltrain-0.1.3/src/dltrain/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,7 +40,8 @@
         self.train_evaluation_handlers: Dict[str, EvaluationHandler] = None
         self.eval_evaluation_handlers: Dict[str, EvaluationHandler] = None
 
         self.features_transform: Transform = None
         self.targets_transform: Transform = None
 
         self.device: device = None
+        self.log_level: int = None
```

### Comparing `dltrain-0.1.2/src/dltrain/train.py` & `dltrain-0.1.3/src/dltrain/train.py`

 * *Files 17% similar despite different names*

```diff
@@ -195,95 +195,127 @@
 
                 logger.info(f'Eval Loss: {total_eval_loss[-1]:.4f}')
                 if eval_evaluation_handlers is not None:
                     for key in eval_evaluation_handlers:
                         logger.info(f'Eval {key}: {total_eval_evaluation[key][-1]}')
 
                 if options.save_checkpoint:
-                    # Save checkpoint
-                    checkpoint = CheckPoint(
-                        epoch,
-                        optimizer.state_dict() if optimizer is not None else None,
-                        scheduler.state_dict() if scheduler is not None else None,
-                        total_train_loss,
-                        total_eval_loss,
-                        total_train_evaluation,
-                        total_eval_evaluation,
-                        options,
-                        best_eval_loss
-                    )
-
-                    checkpoint.save(options.task_name)
-                    del checkpoint
+                    try:
+                        # Save checkpoint
+                        checkpoint = CheckPoint(
+                            epoch,
+                            optimizer.state_dict() if optimizer is not None else None,
+                            scheduler.state_dict() if scheduler is not None else None,
+                            total_train_loss,
+                            total_eval_loss,
+                            total_train_evaluation,
+                            total_eval_evaluation,
+                            options,
+                            best_eval_loss
+                        )
+
+                        checkpoint.save(options.task_name)
+                        del checkpoint
+                    except Exception as e:
+                        logger.error(e)
 
                 print()
 
         # Draw results of total training and evaluation
-        plt.figure()
-        plt.plot(total_train_loss, label='Epoch Train Loss')
-        plt.plot(total_eval_loss, label='Epoch Eval Loss')
-        plt.legend()
-        plt.savefig(f'{options.task_name}/loss.png', dpi=300)
-
-        torch.save(model.cpu(), f'{options.task_name}/weights/last.pt')
-
-        loss_frame = pd.DataFrame({
-            'Train Loss': total_train_loss,
-            'Eval Loss': total_eval_loss
-        })
-        loss_frame.index.name = 'Epoch'
-        loss_frame.to_csv(f'{options.task_name}/loss_result.csv', encoding='utf-8')
+        try:
+            plt.figure()
+            plt.plot(total_train_loss, label='Epoch Train Loss')
+            plt.plot(total_eval_loss, label='Epoch Eval Loss')
+            plt.legend()
+            plt.savefig(f'{options.task_name}/loss.png', dpi=300)
+        except Exception as e:
+            logger.error(e)
+
+        try:
+            torch.save(model.cpu(), f'{options.task_name}/weights/last.pt')
+        except Exception as e:
+            logger.error(e)
+
+        try:
+            loss_frame = pd.DataFrame({
+                'Train Loss': total_train_loss,
+                'Eval Loss': total_eval_loss
+            })
+            loss_frame.index.name = 'Epoch'
+            loss_frame.to_csv(f'{options.task_name}/loss_result.csv', encoding='utf-8')
+        except Exception as e:
+            logger.error(e)
 
         # 映射可计算列
-        for key in total_eval_evaluation:
-            data = total_eval_evaluation[key]
-            if isinstance(data, torch.Tensor):
-                total_eval_evaluation[key] = data.cpu().detach()
-
-        for key in total_train_evaluation:
-            data = total_train_evaluation[key]
-            if isinstance(data, torch.Tensor):
-                total_eval_evaluation[key] = data.cpu().detach()
+        try:
+            for key in total_eval_evaluation:
+                data = total_eval_evaluation[key]
+                if isinstance(data, torch.Tensor):
+                    total_eval_evaluation[key] = data.cpu().detach()
+        except Exception as e:
+            logger.error(e)
+
+        try:
+            for key in total_train_evaluation:
+                data = total_train_evaluation[key]
+                if isinstance(data, torch.Tensor):
+                    total_eval_evaluation[key] = data.cpu().detach()
+        except Exception as e:
+            logger.error(e)
 
         # 判断验证列是否可绘制
         for (key, value) in total_train_evaluation.items():
-            drawable = train_evaluation_handlers[key].drawable
-            if drawable:
-                value = try_convert(value, np.array, f'{key} train evaluation', 'numpy.array')
-                if len(value.shape) == 2 or len(value.shape) == 1:
-                    value = value.reshape(-1)
-                    plt.figure(dpi=300)
-                    plt.plot(value, label=key)
-                    plt.legend()
-                    plt.savefig(f'{options.task_name}/{key}-train.png')
+            try:
+                drawable = train_evaluation_handlers[key].drawable
+                if drawable:
+                    value = try_convert(value, np.array, f'{key} train evaluation', 'numpy.array')
+                    if len(value.shape) == 2 or len(value.shape) == 1:
+                        value = value.reshape(-1)
+                        plt.figure(dpi=300)
+                        plt.plot(value, label=key)
+                        plt.legend()
+                        plt.savefig(f'{options.task_name}/{key}-train.png')
+            except Exception as e:
+                logger.error(e)
 
         for (key, value) in total_eval_evaluation.items():
-            drawable = eval_evaluation_handlers[key].drawable
-            if drawable:
-                value = try_convert(value, np.array, f'{key} eval evaluation', 'numpy.array')
-                if len(value.shape) == 2 or len(value.shape) == 1:
-                    value = value.reshape(-1)
-                    plt.figure(dpi=300)
-                    plt.plot(value, label=key)
-                    plt.legend()
-                    plt.savefig(f'{options.task_name}/{key}-eval.png')
+            try:
+                drawable = eval_evaluation_handlers[key].drawable
+                if drawable:
+                    value = try_convert(value, np.array, f'{key} eval evaluation', 'numpy.array')
+                    if len(value.shape) == 2 or len(value.shape) == 1:
+                        value = value.reshape(-1)
+                        plt.figure(dpi=300)
+                        plt.plot(value, label=key)
+                        plt.legend()
+                        plt.savefig(f'{options.task_name}/{key}-eval.png')
+            except Exception as e:
+                logger.error(e)
 
         if train_evaluation_handlers is not None:
-            train_evaluation_frame = pd.DataFrame(
-                {
-                    **total_train_evaluation
-                }
-            )
-            train_evaluation_frame.index.name = 'Epoch'
-            train_evaluation_frame.to_csv(f'{options.task_name}/train_evaluation_result.csv', encoding='utf-8')
+            try:
+                train_evaluation_frame = pd.DataFrame(
+                    {
+                        **total_train_evaluation
+                    }
+                )
+                train_evaluation_frame.index.name = 'Epoch'
+                train_evaluation_frame.to_csv(f'{options.task_name}/train_evaluation_result.csv',
+                                              encoding='utf-8')
+            except Exception as e:
+                logger.error(e)
 
         if eval_evaluation_handlers is not None:
-            eval_evaluation_frame = pd.DataFrame(
-                {
-                    **total_eval_evaluation
-                }
-            )
-            eval_evaluation_frame.index.name = 'Epoch'
-            eval_evaluation_frame.to_csv(f'{options.task_name}/eval_evaluation_result.csv', encoding='utf-8')
+            try:
+                eval_evaluation_frame = pd.DataFrame(
+                    {
+                        **total_eval_evaluation
+                    }
+                )
+                eval_evaluation_frame.index.name = 'Epoch'
+                eval_evaluation_frame.to_csv(f'{options.task_name}/eval_evaluation_result.csv'
+                                             , encoding='utf-8')
+            except Exception as e:
+                logger.error(e)
 
         logger.save(f'{options.task_name}/log.txt')
```

### Comparing `dltrain-0.1.2/src/dltrain/transform.py` & `dltrain-0.1.3/src/dltrain/transform.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain/utils.py` & `dltrain-0.1.3/src/dltrain/utils.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.1.2/src/dltrain.egg-info/PKG-INFO` & `dltrain-0.1.3/src/dltrain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,18 @@
 # dltrain
 这是一个 PyTorch 训练包，本项目提供了大量的高级训练 API 和低级接口，满足所有训练需求
 <br/>
 安装仅在Shell中使用pip安装即可
 ```bash
 pip install dltrain
 ```
+利用该工具包我们可用通过如下结构构建训练代码
+<img src="img/dltrain.png"/>
+
+## Example
 ### example .1 在iris数据集上使用多层感知器进行分类
 ```python
 from dltrain import TaskBuilder, SimpleTrainer
 
 builder = TaskBuilder('iris')
 builder.base.use_epoch(100).use_batch_size(8).use_device('cuda')
 builder.model.use_mlp(4, 3)
@@ -88,15 +92,15 @@
 builder.evaluation_handler.add_accuracy()
 builder.delineator.use_train_eval(builder.dataset.use_mnist('./dataset', True),
                                   builder.dataset.use_mnist('./dataset', False))
 SimpleTrainer().run(builder.build())
 ```
 模型向导对象的use_model接口允许用户传入自己的模型
 
-### Example .2.1 使用torchvision的自带模型
+### example .2.1 使用torchvision的自带模型
 ```python
 from dltrain import TaskBuilder, SimpleTrainer
 
 builder = TaskBuilder('mnist')
 builder.model.use_pytorch_model('resnet18', num_classes=10)
 builder.base.use_device('cuda')
 builder.optimizer.use_adam()
@@ -133,31 +137,34 @@
 
     swin_b, swin_t, swin_s, swin_v2_b, swin_v2_t, swin_v2_s,
 
     mnasnet0_5, mnasnet1_0, mnasnet1_3, mnasnet0_75
 ]
 ```
 ### default about the arguments
-| 参数名称             | 默认值                                                |
+| 参数名称             | 默认值                                                |    
 |------------------|----------------------------------------------------|
 | optimizer        | Sgd(lr=0.01,momentum=0,dampening=0,weight_decay=0) |
 | scheduler        | User-set                                           |
 | criterion*       | None,Must be specified by the user                 |    
 | model*           | None,Must be specified by the user                 |
 | epoch            | 10                                                 |
 | batch_size       | 16                                                 |
 | seed             | 3407                                               |
 | device           | cpu                                                |
 | save_checkpoint  | False                                              |
-| start_checkpoint | User-set                                           |
+| start_checkpoint | None,User-set                                      |
 | delineator*      | None,Must be specified by the user                 |
 | forward          | SimpleForward                                      |
 | trainer          | SimpleTrainer                                      |
 
 ## Version Log
 - 0.0.1<br/>
 1、构造整体模型框架
 - 0.0.2<br/>
 1、加入了TaskBuilder方便构造模型
 - 0.1.2<br/>
-1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)
+1、加入了InjectForward(可以通过InjectWizard注入训练时策略，如实时检测模型参数梯度的分布等)<br/>
 2、将models.py封装到models包，添加了许多拆箱可用模型
+- 0.1.3<br/>
+1、引入错误处理机制，防止由于EventHandler设置问题导致的结果保存错误<br/>
+2、引入VectorSequenceDataset<br/>
```

### Comparing `dltrain-0.1.2/src/dltrain.egg-info/SOURCES.txt` & `dltrain-0.1.3/src/dltrain.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,10 +28,11 @@
 src/dltrain/builder/forward.py
 src/dltrain/builder/inject.py
 src/dltrain/builder/model.py
 src/dltrain/builder/optimizer.py
 src/dltrain/builder/scheduler.py
 src/dltrain/builder/transforms.py
 src/dltrain/models/__init__.py
+src/dltrain/models/builder.py
 src/dltrain/models/component.py
 src/dltrain/models/model.py
 src/dltrain/models/wrapper.py
```

