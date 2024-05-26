# Comparing `tmp/sequifier-2.1.0.tar.gz` & `tmp/sequifier-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequifier-2.1.0.tar", max compression
+gzip compressed data, was "sequifier-2.2.0.tar", max compression
```

## Comparing `sequifier-2.1.0.tar` & `sequifier-2.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1669 2024-04-06 10:15:07.075618 sequifier-2.1.0/LICENSE
--rw-r--r--   0        0        0     5162 2024-04-20 13:01:12.270656 sequifier-2.1.0/README.md
--rw-r--r--   0        0        0      919 2024-05-01 11:32:11.870741 sequifier-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4707 2024-05-01 11:32:11.871058 sequifier-2.1.0/src/sequifier/config/infer_config.py
--rw-r--r--   0        0        0     1760 2024-05-01 11:32:11.871370 sequifier-2.1.0/src/sequifier/config/preprocess_config.py
--rw-r--r--   0        0        0     7430 2024-05-01 11:32:11.871712 sequifier-2.1.0/src/sequifier/config/train_config.py
--rw-r--r--   0        0        0     2322 2024-05-01 11:32:11.872088 sequifier-2.1.0/src/sequifier/helpers.py
--rw-r--r--   0        0        0    21156 2024-05-01 11:32:11.872493 sequifier-2.1.0/src/sequifier/infer.py
--rw-r--r--   0        0        0    12716 2024-05-01 11:32:11.872842 sequifier-2.1.0/src/sequifier/preprocess.py
--rw-r--r--   0        0        0     2234 2024-04-20 13:01:12.278568 sequifier-2.1.0/src/sequifier/sequifier.py
--rw-r--r--   0        0        0    22866 2024-05-01 11:32:11.873256 sequifier-2.1.0/src/sequifier/train.py
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 sequifier-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1669 2024-04-06 10:15:07.075618 sequifier-2.2.0/LICENSE
+-rw-r--r--   0        0        0     5162 2024-04-20 13:01:12.270656 sequifier-2.2.0/README.md
+-rw-r--r--   0        0        0      919 2024-05-26 14:50:12.735681 sequifier-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4707 2024-05-01 11:32:11.871058 sequifier-2.2.0/src/sequifier/config/infer_config.py
+-rw-r--r--   0        0        0     1760 2024-05-01 11:32:11.871370 sequifier-2.2.0/src/sequifier/config/preprocess_config.py
+-rw-r--r--   0        0        0     7582 2024-05-26 14:50:12.736059 sequifier-2.2.0/src/sequifier/config/train_config.py
+-rw-r--r--   0        0        0     2851 2024-05-26 14:50:12.736267 sequifier-2.2.0/src/sequifier/helpers.py
+-rw-r--r--   0        0        0    20796 2024-05-26 14:50:12.736739 sequifier-2.2.0/src/sequifier/infer.py
+-rw-r--r--   0        0        0    12716 2024-05-01 11:32:11.872842 sequifier-2.2.0/src/sequifier/preprocess.py
+-rw-r--r--   0        0        0     2234 2024-04-20 13:01:12.278568 sequifier-2.2.0/src/sequifier/sequifier.py
+-rw-r--r--   0        0        0    23893 2024-05-26 14:50:12.737107 sequifier-2.2.0/src/sequifier/train.py
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 sequifier-2.2.0/PKG-INFO
```

### Comparing `sequifier-2.1.0/LICENSE` & `sequifier-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sequifier-2.1.0/README.md` & `sequifier-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sequifier-2.1.0/pyproject.toml` & `sequifier-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sequifier"
-version = "2.1.0"
+version = "2.2.0"
 authors = ["Leon Luithlen <leontimnaluithlen@gmail.com>"]
 description = "Train a transformer model with the command line"
 keywords = ["transformer", "sequence classification", "machine learning", "sequence", "sequence modelling", "nlp", "language", "language modelling", "torch", "pytorch"]
 readme = "README.md"
 license = "BSD 3-Clause"
 homepage = "https://github.com/0xideas/sequifier"
 repository = "https://github.com/0xideas/sequifier"
```

### Comparing `sequifier-2.1.0/src/sequifier/config/infer_config.py` & `sequifier-2.2.0/src/sequifier/config/infer_config.py`

 * *Files identical despite different names*

### Comparing `sequifier-2.1.0/src/sequifier/config/preprocess_config.py` & `sequifier-2.2.0/src/sequifier/config/preprocess_config.py`

 * *Files identical despite different names*

### Comparing `sequifier-2.1.0/src/sequifier/config/train_config.py` & `sequifier-2.2.0/src/sequifier/config/train_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,16 @@
             config_values.get(
                 "validation_data_path",
                 dd_config["split_paths"][min(1, len(dd_config["split_paths"]) - 1)],
             ),
             config_values["project_path"],
         )
 
+        config_values["id_maps"] = dd_config["id_maps"]
+
     return TrainModel(**config_values)
 
 
 VALID_LOSS_FUNCTIONS = [
     "L1Loss",
     "MSELoss",
     "CrossEntropyLoss",
@@ -128,14 +130,15 @@
 
 
 @dataclass
 class TrainingSpecModel(BaseModel):
     device: str
     epochs: int
     log_interval: int = 10
+    class_share_log_columns: list[str] = []
     early_stopping_epochs: Optional[int]
     iter_save: int
     batch_size: int
     lr: float  # learning rate
     criterion: dict[str, str]
     accumulation_steps: Optional[int]
     dropout: float = 0.0
@@ -200,14 +203,15 @@
 
     selected_columns: Optional[list[str]]
     column_types: dict[str, str]
     categorical_columns: list[str]
     real_columns: list[str]
     target_columns: list[str]
     target_column_types: dict[str, str]
+    id_maps: dict[str, dict[Union[str, int], int]]
 
     seq_length: int
     n_classes: dict[str, int]
     inference_batch_size: int
     seed: int
 
     export_onnx: bool = True
```

### Comparing `sequifier-2.1.0/src/sequifier/helpers.py` & `sequifier-2.2.0/src/sequifier/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,29 @@
 import pandas as pd
 import torch
 from torch import tensor
 
 PANDAS_TO_TORCH_TYPES = {"int64": torch.int64, "float64": torch.float32}
 
 
+def construct_index_maps(id_maps, target_columns_index_map, map_to_id):
+    index_map = {}
+    if map_to_id is not None:
+        for target_column in target_columns_index_map:
+            map_ = (
+                {v: k for k, v in id_maps[target_column].items()} if map_to_id else None
+            )
+            if isinstance(list(map_.values())[0], str):
+                map_[0] = "unknown"
+            else:
+                map_[0] = np.min(map_.values()) - 1
+            index_map[target_column] = map_
+    return index_map
+
+
 def read_data(path, read_format, columns=None):
     if read_format == "csv":
         return pd.read_csv(path, sep=",", decimal=".", index_col=False)
     if read_format == "parquet":
         return pd.read_parquet(path, columns=columns)
```

### Comparing `sequifier-2.1.0/src/sequifier/infer.py` & `sequifier-2.2.0/src/sequifier/infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 import numpy as np
 import onnxruntime
 import pandas as pd
 import torch
 
 from sequifier.config.infer_config import load_inferer_config
-from sequifier.helpers import (PANDAS_TO_TORCH_TYPES, normalize_path,
-                               numpy_to_pytorch, read_data,
+from sequifier.helpers import (PANDAS_TO_TORCH_TYPES, construct_index_maps,
+                               normalize_path, numpy_to_pytorch, read_data,
                                subset_to_selected_columns, write_data)
 from sequifier.train import infer_with_model, load_inference_model
 
 
 def infer(args, args_config):
     config_path = (
         args.config_path if args.config_path is not None else "configs/infer.yaml"
     )
 
     config = load_inferer_config(config_path, args_config, args.on_unprocessed)
 
     if config.map_to_id or (len(config.real_columns) > 0):
         assert config.ddconfig_path is not None, (
-            "If you want to map to id, you need to provide a file path to a json that contains: {{'id_map':{...}}} to ddconfig_path"
+            "If you want to map to id, you need to provide a file path to a json that contains: {{'id_maps':{...}}} to ddconfig_path"
             "\nIf you have real columns in the data, you need to provide a json that contains: {{'min_max_values':{COL_NAME:{'min':..., 'max':...}}}}"
         )
         with open(normalize_path(config.ddconfig_path, config.project_path), "r") as f:
             dd_config = json.loads(f.read())
             id_maps = dd_config["id_maps"]
             min_max_values = dd_config["min_max_values"]
     else:
@@ -327,15 +327,15 @@
 
 
 class Inferer(object):
     def __init__(
         self,
         model_path,
         project_path,
-        id_map,
+        id_maps,
         min_max_values,
         map_to_id,
         categorical_columns,
         real_columns,
         target_columns,
         target_column_types,
         sample_from_distribution,
@@ -343,28 +343,20 @@
         inference_batch_size,
         device,
         args_config,
         training_config_path,
     ):
         self.map_to_id = map_to_id
         self.min_max_values = min_max_values
-        if self.map_to_id:
-            self.index_map = {}
-            for target_column in target_columns:
-                if target_column_types[target_column] == "categorical":
-                    map_ = (
-                        {v: k for k, v in id_map[target_column].items()}
-                        if map_to_id
-                        else None
-                    )
-                    if isinstance(list(map_.values())[0], str):
-                        map_[0] = "unknown"
-                    else:
-                        map_[0] = np.min(map_.values()) - 1
-                    self.index_map[target_column] = map_
+        target_columns_index_map = [
+            c for c in target_columns if target_column_types[c] == "categorical"
+        ]
+        self.index_map = construct_index_maps(
+            id_maps, target_columns_index_map, map_to_id
+        )
 
         self.device = device
         self.categorical_columns = categorical_columns
         self.real_columns = real_columns
         self.target_columns = target_columns
         self.target_column_types = target_column_types
         self.sample_from_distribution = sample_from_distribution
```

### Comparing `sequifier-2.1.0/src/sequifier/preprocess.py` & `sequifier-2.2.0/src/sequifier/preprocess.py`

 * *Files identical despite different names*

### Comparing `sequifier-2.1.0/src/sequifier/sequifier.py` & `sequifier-2.2.0/src/sequifier/sequifier.py`

 * *Files identical despite different names*

### Comparing `sequifier-2.1.0/src/sequifier/train.py` & `sequifier-2.2.0/src/sequifier/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import numpy as np
 import pandas as pd
 import torch
 from torch import Tensor, nn
 from torch.nn import ModuleDict, TransformerEncoder, TransformerEncoderLayer
 
 from sequifier.config.train_config import load_train_config
-from sequifier.helpers import (PANDAS_TO_TORCH_TYPES, LogFile, normalize_path,
+from sequifier.helpers import (PANDAS_TO_TORCH_TYPES, LogFile,
+                               construct_index_maps, normalize_path,
                                numpy_to_pytorch, read_data,
                                subset_to_selected_columns)
 
 
 def train(args, args_config):
     config_path = (
         args.config_path if args.config_path is not None else "configs/train.yaml"
@@ -109,14 +110,18 @@
         self.target_columns = hparams.target_columns
         self.target_column_types = hparams.target_column_types
         self.loss_weights = hparams.training_spec.loss_weights
         self.seq_length = hparams.seq_length
         self.n_classes = hparams.n_classes
         self.inference_batch_size = hparams.inference_batch_size
         self.log_interval = hparams.training_spec.log_interval
+        self.class_share_log_columns = hparams.training_spec.class_share_log_columns
+        self.index_maps = construct_index_maps(
+            hparams.id_maps, self.class_share_log_columns, True
+        )
         self.export_onnx = hparams.export_onnx
         self.export_pt = hparams.export_pt
         self.export_with_dropout = hparams.export_with_dropout
         self.early_stopping_epochs = hparams.training_spec.early_stopping_epochs
         self.hparams = hparams
 
         self.drop = nn.Dropout(hparams.training_spec.dropout)
@@ -270,30 +275,45 @@
 
             if (
                 self.early_stopping_epochs is None
                 or n_epochs_no_improvemet < self.early_stopping_epochs
             ):
                 epoch_start_time = time.time()
                 self.train_epoch(X_train, y_train, epoch)
-                total_loss, total_losses = self.evaluate(X_valid, y_valid)
+                total_loss, total_losses, output = self.evaluate(X_valid, y_valid)
                 elapsed = time.time() - epoch_start_time
                 self.log_file.write("-" * 89)
                 self.log_file.write(
                     f"| end of epoch {epoch:3d} | time: {elapsed:5.2f}s | "
                     f"valid loss {(total_loss * 1000):5.5f}"
                 )
+
                 if len(total_losses) > 1:
                     self.log_file.write(
                         " - ".join(
                             [
                                 f"{target_column} loss: {(tloss*1000):5.2f}"
                                 for target_column, tloss in total_losses.items()
                             ]
                         )
                     )
+                for categorical_column in self.class_share_log_columns:
+                    output_values = (
+                        output[categorical_column].argmax(1).cpu().detach().numpy()
+                    )
+                    output_counts = pd.Series(output_values).value_counts().sort_index()
+                    output_counts = output_counts / output_counts.sum()
+                    value_shares = " | ".join(
+                        [
+                            f"{self.index_maps[categorical_column][value]}: {share:5.5f}"
+                            for value, share in output_counts.to_dict().items()
+                        ]
+                    )
+                    self.log_file.write(f"{categorical_column}: {value_shares}")
+
                 self.log_file.write("-" * 89)
 
                 if total_loss < best_val_loss:
                     best_val_loss = total_loss
                     best_model = self.copy_model()
 
                     n_epochs_no_improvemet = 0
@@ -412,15 +432,15 @@
 
         denominator = X_valid[self.target_columns[0]].size(0)  # any column will do
         total_loss = total_loss / denominator
         total_losses = {
             target_column: tloss / denominator
             for target_column, tloss in total_losses.items()
         }
-        return total_loss, total_losses
+        return total_loss, total_losses, output
 
     def get_batch(self, X, y, batch_start, batch_size, to_device):
         if to_device:
             return (
                 {
                     col: X[col][batch_start : batch_start + batch_size, :].to(
                         self.device
```

### Comparing `sequifier-2.1.0/PKG-INFO` & `sequifier-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequifier
-Version: 2.1.0
+Version: 2.2.0
 Summary: Train a transformer model with the command line
 Home-page: https://github.com/0xideas/sequifier
 License: BSD 3-Clause
 Keywords: transformer,sequence classification,machine learning,sequence,sequence modelling,nlp,language,language modelling,torch,pytorch
 Author: Leon Luithlen
 Author-email: leontimnaluithlen@gmail.com
 Requires-Python: >=3.9,<4.0
```

