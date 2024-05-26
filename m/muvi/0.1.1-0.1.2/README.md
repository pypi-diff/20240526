# Comparing `tmp/muvi-0.1.1.tar.gz` & `tmp/muvi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muvi-0.1.1.tar", max compression
+gzip compressed data, was "muvi-0.1.2.tar", max compression
```

## Comparing `muvi-0.1.1.tar` & `muvi-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rwxr-xr-x   0        0        0     1515 2023-01-23 16:36:17.349155 muvi-0.1.1/LICENSE
--rw-r--r--   0        0        0     1700 2023-10-23 19:57:43.839171 muvi-0.1.1/README.md
--rwxr-xr-x   0        0        0      605 2023-10-23 20:09:10.600003 muvi-0.1.1/muvi/__init__.py
--rwxr-xr-x   0        0        0      419 2023-10-19 16:30:08.290310 muvi-0.1.1/muvi/core/__init__.py
--rwxr-xr-x   0        0        0    11045 2023-10-20 15:40:49.314779 muvi-0.1.1/muvi/core/callbacks.py
--rwxr-xr-x   0        0        0      394 2023-07-03 15:07:40.752312 muvi-0.1.1/muvi/core/gpu.py
--rwxr-xr-x   0        0        0     1641 2023-10-19 16:30:08.290101 muvi-0.1.1/muvi/core/index.py
--rwxr-xr-x   0        0        0    60285 2023-10-21 17:17:31.949153 muvi-0.1.1/muvi/core/models.py
--rwxr-xr-x   0        0        0    21997 2023-10-20 15:45:43.134655 muvi-0.1.1/muvi/core/synthetic.py
--rwxr-xr-x   0        0        0      285 2023-01-23 16:36:17.418703 muvi-0.1.1/muvi/log.conf
--rwxr-xr-x   0        0        0      108 2023-10-19 16:30:08.289013 muvi-0.1.1/muvi/tools/__init__.py
--rwxr-xr-x   0        0        0     3681 2023-10-19 16:30:08.289048 muvi-0.1.1/muvi/tools/cache.py
--rw-r--r--   0        0        0     4358 2023-10-20 16:05:23.499794 muvi-0.1.1/muvi/tools/external.py
--rwxr-xr-x   0        0        0    21698 2023-10-20 15:47:32.496783 muvi-0.1.1/muvi/tools/feature_sets.py
--rwxr-xr-x   0        0        0    29514 2023-10-20 15:48:32.256590 muvi-0.1.1/muvi/tools/plotting.py
--rwxr-xr-x   0        0        0    26445 2023-10-20 15:56:14.797234 muvi-0.1.1/muvi/tools/utils.py
--rwxr-xr-x   0        0        0     2643 2023-10-23 20:09:52.319037 muvi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 muvi-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1515 2023-01-23 16:36:17.349155 muvi-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4733 2023-10-24 14:53:35.030001 muvi-0.1.2/README.md
+-rwxr-xr-x   0        0        0      582 2024-05-26 20:36:44.623539 muvi-0.1.2/muvi/__init__.py
+-rwxr-xr-x   0        0        0      424 2024-05-26 20:36:44.626371 muvi-0.1.2/muvi/core/__init__.py
+-rwxr-xr-x   0        0        0     9150 2024-05-26 20:36:44.628594 muvi-0.1.2/muvi/core/callbacks.py
+-rwxr-xr-x   0        0        0     1817 2024-05-26 20:36:44.630678 muvi-0.1.2/muvi/core/early_stopping.py
+-rwxr-xr-x   0        0        0      394 2024-05-09 18:16:27.710380 muvi-0.1.2/muvi/core/gpu.py
+-rwxr-xr-x   0        0        0     3941 2024-05-26 20:36:44.632935 muvi-0.1.2/muvi/core/index.py
+-rwxr-xr-x   0        0        0    71140 2024-05-26 20:36:44.634969 muvi-0.1.2/muvi/core/models.py
+-rwxr-xr-x   0        0        0    21949 2024-05-26 20:36:44.638061 muvi-0.1.2/muvi/core/synthetic.py
+-rwxr-xr-x   0        0        0      285 2024-05-09 18:15:08.122336 muvi-0.1.2/muvi/log.conf
+-rwxr-xr-x   0        0        0      108 2024-05-09 18:17:03.362634 muvi-0.1.2/muvi/tools/__init__.py
+-rwxr-xr-x   0        0        0     3719 2024-05-26 20:36:44.642634 muvi-0.1.2/muvi/tools/cache.py
+-rw-r--r--   0        0        0     4358 2024-05-09 18:17:21.029149 muvi-0.1.2/muvi/tools/external.py
+-rwxr-xr-x   0        0        0    22083 2024-05-26 20:36:44.645212 muvi-0.1.2/muvi/tools/feature_sets.py
+-rwxr-xr-x   0        0        0    34430 2024-05-26 20:36:44.647589 muvi-0.1.2/muvi/tools/plotting.py
+-rw-r--r--   0        0        0    30931 2024-05-26 20:36:44.648921 muvi-0.1.2/muvi/tools/utils.py
+-rwxr-xr-x   0        0        0     2789 2024-05-26 20:36:44.656677 muvi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6097 1970-01-01 00:00:00.000000 muvi-0.1.2/PKG-INFO
```

### Comparing `muvi-0.1.1/LICENSE` & `muvi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `muvi-0.1.1/muvi/core/callbacks.py` & `muvi-0.1.2/muvi/core/callbacks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,20 @@
-"""Collection of MuVI callbacks."""
+"""Collection of training callbacks."""
 from collections import defaultdict
 from typing import Callable
-from typing import List
 from typing import Optional
 
 import numpy as np
 
 from sklearn.metrics import precision_recall_fscore_support
 
 from muvi.tools.utils import rmse
 from muvi.tools.utils import variance_explained
 
 
-class EarlyStoppingCallback:
-    def __init__(
-        self,
-        n_epochs: int,
-        min_epochs: int = 100,
-        tolerance: float = 1e-5,
-        patience: int = 10,
-    ):
-        """Early stopping callback.
-
-        Parameters
-        ----------
-        n_epochs : int
-            Number of training epochs
-        min_epochs : int, optional
-            Minimal number of epochs before deploying early stopping,
-            by default 100
-        tolerance : float, optional
-            Improvement ratio between two consecutive evaluations,
-            by default 1e-5
-        patience : int, optional
-            Number of patience steps before terminating training,
-            by default 10
-        """
-        self.n_epochs = n_epochs
-        self.min_epochs = min_epochs
-        self.tolerance = tolerance
-        self.patience = patience
-
-        self.early_stop_counter = 0
-        self.min_loss = np.inf
-
-    def __call__(self, loss_history):
-        epoch_idx = len(loss_history) - 1
-        if epoch_idx < self.min_epochs:
-            return False
-
-        current_loss = loss_history[epoch_idx]
-        if self.min_loss == np.inf:
-            self.min_loss = current_loss
-            return False
-
-        stop_early = False
-
-        relative_improvement = (self.min_loss - current_loss) / np.abs(self.min_loss)
-        self.min_loss = min(self.min_loss, current_loss)
-
-        if relative_improvement < self.tolerance:
-            self.early_stop_counter += 1
-        else:
-            self.early_stop_counter = 0
-        stop_early = self.early_stop_counter >= self.patience
-
-        if stop_early:
-            print(
-                "Relative improvement of "
-                f"{relative_improvement:0.4g} < {self.tolerance:0.4g} "
-                f"for {self.patience} step(s) in a row, stopping early."
-            )
-
-        return stop_early
-
-
 class CheckpointCallback:
     def __init__(
         self,
         model,
         n_epochs: int,
         n_checkpoints: int = 10,
         callback: Optional[Callable] = None,
@@ -125,30 +61,30 @@
     ]
 
     def __init__(
         self,
         model,
         n_epochs: int,
         n_checkpoints: int = 10,
-        active_callbacks: Optional[List[str]] = None,
+        active_callbacks: Optional[list[str]] = None,
         view_wise: bool = True,
         **kwargs,
     ) -> None:
         """Log callback.
 
         Parameters
         ----------
         model : MuVI
             A MuVI object
         n_epochs : int
             Number of training epochs
         n_checkpoints : int, optional
             Number of times to execute during training,
             by default 10
-        active_callbacks : List[str], optional
+        active_callbacks : list[str], optional
             List of callback names from LogCallback._CALLBACK_KEYS,
             by default None (all)
         view_wise : bool, optional
             Whether to report scores for each view,
             by default True
         """
         self.kwargs = kwargs
```

### Comparing `muvi-0.1.1/muvi/core/models.py` & `muvi-0.1.2/muvi/core/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import time
 
+from importlib.metadata import version
 from typing import Any
 from typing import Callable
-from typing import Dict
-from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
 import pyro
 import pyro.distributions as dist
@@ -18,141 +17,181 @@
 from pyro.distributions import constraints
 from pyro.infer.autoguide.guides import deep_getattr
 from pyro.infer.autoguide.guides import deep_setattr
 from pyro.nn import PyroModule
 from pyro.nn import PyroParam
 from pyro.optim import Adam
 from pyro.optim import ClippedAdam
+from tabulate import tabulate
+from tensordict import TensorDict
 from torch.utils.data import DataLoader
-from torch.utils.data import Dataset
 from tqdm import tqdm
 
+from muvi.core.early_stopping import EarlyStoppingCallback
+from muvi.core.index import _make_index_unique
 from muvi.core.index import _normalize_index
 
 
 logger = logging.getLogger(__name__)
 
-Index = Union[int, str, List[int], List[str], np.ndarray, pd.Index]
+Index = Union[int, str, list[int], list[str], np.ndarray, pd.Index]
 SingleView = Union[np.ndarray, pd.DataFrame]
-MultiView = Union[Dict[str, SingleView], List[SingleView]]
+MultiView = Union[dict[str, SingleView], list[SingleView]]
 
 
-class DictDataset(Dataset):
-    """Dictionary based PyTorch dataset."""
-
-    def __init__(self, tensor_dict, idx_key="sample_idx", **kwargs):
-        self.tensor_dict = tensor_dict
-        self.idx_key = idx_key
-        # just stores them
-        self.kwargs = kwargs
-        self._len = tensor_dict[next(iter(tensor_dict))].shape[0]
-
-    def __len__(self):
-        return self._len
-
-    def __getitem__(self, index):
-        item = {self.idx_key: index}
-        for k, v in self.tensor_dict.items():
-            item[k] = v[index]
-        return item
+def identity(x):
+    return x
 
 
 class MuVI(PyroModule):
     def __init__(
         self,
         observations: MultiView,
         prior_masks: Optional[MultiView] = None,
         covariates: Optional[SingleView] = None,
-        prior_confidence: Union[float, str] = 0.99,
+        prior_confidence: Optional[Union[float, str]] = "med",
         n_factors: Optional[int] = None,
-        view_names: Optional[List[str]] = None,
-        likelihoods: Optional[Union[Dict[str, str], List[str]]] = None,
+        view_names: Optional[list[str]] = None,
+        likelihoods: Optional[Union[dict[str, str], list[str]]] = None,
         reg_hs: bool = True,
-        nmf: Optional[Union[Dict[str, bool], List[bool]]] = None,
+        nmf: Optional[Union[dict[str, bool], list[bool]]] = None,
+        pos_transform: str = "relu",
+        normalize: bool = True,
         device: str = "cuda",
     ):
         """MuVI module.
 
         Parameters
         ----------
         observations : MultiView
             Collection of observations as list or dict.
         prior_masks : MultiView, optional
             Prior feature sets as a collection of binary masks,
             by default None
         covariates : SingleView, optional
             Additional observed covariates, by default None
-        prior_confidence : float or string
+        prior_confidence : float or string, optional
             Confidence of prior belief from 0 to 1 (exclusive),
-            typical values are 'low' (0.95), 'med' (0.99) and 'high' (0.999),
-            by default 0.99
+            typical values are 'low' (0.99), 'med' (0.995) and 'high' (0.999),
+            by default 'med'
         n_factors : int, optional
             Number of latent factors,
             can be omitted when providing prior masks,
+            or it can be used to introduce additional dense factors
+            if larger than the informed factors,
             by default None
-        view_names : List[str], optional
+        view_names : list[str], optional
             List of names for each view,
             determines view order as well,
             by default None
-        likelihoods : Union[Dict[str, str], List[str]], optional
+        likelihoods : Union[dict[str, str], list[str]], optional
             Likelihoods for each view,
             either "normal" or "bernoulli",
             by default None (all "normal")
         reg_hs : bool, optional
             Whether to use the regularized version of HS,
             by default True,
             only relevant when NOT using informative priors
-        nmf : Union[Dict[str, bool], List[bool]], optional
+        nmf : Union[dict[str, bool], list[bool]], optional
             Whether to use non-negative matrix factorization,
             by default False
+        normalize : bool, optional
+            Whether to normalize observations,
+            by default True
         device : str, optional
             Device to run computations on, by default "cuda" (GPU)
         """
         super().__init__(name="MuVI")
         self.observations = self._setup_observations(observations, view_names)
+        self.prior_confidence = self._setup_prior_confidence(prior_confidence)
         self.prior_masks, self.prior_scales = self._setup_prior_masks(
-            prior_masks, prior_confidence, n_factors
+            prior_masks, n_factors
         )
         self.covariates = self._setup_covariates(covariates)
         self.likelihoods = self._setup_likelihoods(likelihoods)
         self.nmf = self._setup_nmf(nmf)
+        self.pos_transform = pos_transform
 
         self.reg_hs = reg_hs
         self._informed = self.prior_masks is not None
         if not self.reg_hs and self._informed:
             logger.warning(
                 "Informative priors require regularized horseshoe, "
                 "setting `reg_hs` to True."
             )
             self.reg_hs = True
 
+        self.normalize = normalize
+        if self.normalize:
+            self.observations = self._normalize_observations()
+
         self.device = self._setup_device(device)
         self.to(self.device)
 
         self._model = None
         self._guide = None
         self._built = False
         self._trained = False
-        self._training_log: Dict[str, Any] = {}
+        self._training_log: dict[str, Any] = {}
         self._cache = None
 
-    @property
-    def _factor_signs(self):
-        signs = 1.0
+        self._version = version("muvi")
+
+    def __repr__(self):
+        table = [
+            ["n_views", self.n_views],
+            ["n_samples", self.n_samples],
+            [
+                "n_features",
+                ", ".join([f"{vn}: {self.n_features[vn]}" for vn in self.view_names]),
+            ],
+            ["n_factors", self.n_factors],
+            ["prior_confidence", self.prior_confidence],
+            ["n_covariates", self.n_covariates],
+            [
+                "likelihoods",
+                ", ".join([f"{vn}: {self.likelihoods[vn]}" for vn in self.view_names]),
+            ],
+            ["nmf", ", ".join([f"{vn}: {self.nmf[vn]}" for vn in self.view_names])],
+            ["reg_hs", self.reg_hs],
+        ]
+
+        if any(self.nmf.values()):
+            table.append(["pos_transform", self.pos_transform])
+        table.append(["device", self.device])
+
+        header = f" MuVI version {self._version} "
+        body = tabulate(table, headers=["Parameter", "Value"], tablefmt="github")
+        row_len = len(body.split("\n")[0])
+        left_padding_len = (row_len - len(header) - 2) // 2
+
+        empty_line = "|" + "=" * (row_len - 2) + "|\n"
+        header = "|" + " " * left_padding_len + header
+        header = (
+            empty_line + header + " " * (row_len - len(header) - 1) + "|\n" + empty_line
+        )
+        output = header + body + "\n" + empty_line
+        return output
+
+    def _get_factor_signs(self):
+        signs = np.ones(self.n_factors, dtype=np.float32)
         # only compute signs if model is trained
         # and there is no nmf constraint
-        if self._trained and not any(self.nmf.values()):
+        if self._trained:
             w = self._guide.get_w()
             # TODO: looking at top loadings works better than including all
             # 100 feels a bit arbitrary though
             w = np.array(
                 list(map(lambda x, y: y[x], np.argsort(-np.abs(w), axis=1)[:, :100], w))
             )
             signs = (w.sum(axis=1) > 0) * 2 - 1
 
+        # if nmf is enabled, all factors are positive
+        if any(self.nmf.values()):
+            signs = np.ones(self.n_factors, dtype=np.float32)
         return pd.Series(signs, index=self.factor_names, dtype=np.float32)
 
     def _setup_device(self, device):
         cuda_available = torch.cuda.is_available()
 
         try:
             mps_available = torch.backends.mps.is_available()
@@ -168,17 +207,87 @@
 
         logger.info(f"Running all computations on `{device}`.")
         return torch.device(device)
 
     def _validate_index(self, idx):
         if not is_string_dtype(idx):
             logger.warning("Transforming to str index.")
-            return idx.astype(str)
+            idx = idx.astype(str)
+        if not idx.is_unique:
+            logger.warning("Making index unique.")
+            idx = _make_index_unique(idx)
         return idx
 
+    def _normalize_observations(self):
+        logger.info("Normalizing observations.")
+        for vn, obs in self.observations.items():
+            if self.nmf[vn]:
+                logger.info(f"Setting min value of view `{vn}` to 0.")
+                obs -= np.nanmin(obs, axis=0)
+            else:
+                logger.info(f"Centering features of view `{vn}`.")
+                obs -= np.nanmean(obs, axis=0)
+            global_std = np.nanstd(obs)
+            logger.info(
+                f"Setting global standard deviation to 1.0 (from {global_std:.3f})."
+            )
+            obs /= global_std
+
+        return self.observations
+
+    def _merge(self, matrix_collection, method="union"):
+        all_array = all(
+            isinstance(matrix, np.ndarray) for matrix in matrix_collection.values()
+        )
+        all_dataframe = all(
+            isinstance(matrix, pd.DataFrame) for matrix in matrix_collection.values()
+        )
+
+        if not all_array and not all_dataframe:
+            raise ValueError(
+                "All input must be of the same type, either np.ndarray or pd.DataFrame."
+            )
+
+        if all_array:
+            matrix_collection = {
+                k: pd.DataFrame(matrix) for k, matrix in matrix_collection.items()
+            }
+
+        key_list = []
+        value_list = []
+        for k, v in matrix_collection.items():
+            key_list.append(k)
+            value_list.append(v)
+
+        index_offsets = [0, *list(np.cumsum([v.shape[1] for v in value_list]))]
+
+        if method == "intersection":
+            merged_matrix_collection = pd.concat(value_list, axis=1, join="inner")
+        elif method == "union":
+            merged_matrix_collection = pd.concat(value_list, axis=1, join="outer")
+        else:
+            raise ValueError(
+                'Invalid merge method. Please choose either "intersection" or "union".'
+            )
+
+        merged_matrix_collection = {
+            k: merged_matrix_collection.iloc[
+                :, index_offsets[i] : index_offsets[i + 1]
+            ].copy()
+            for i, k in enumerate(key_list)
+        }
+
+        if all_array:
+            merged_matrix_collection = {
+                k: v.to_numpy(dtype=np.float32)
+                for k, v in merged_matrix_collection.items()
+            }
+
+        return merged_matrix_collection
+
     def _setup_views(self, observations, view_names):
         if view_names is None:
             logger.warning("No view names provided!")
             if isinstance(observations, list):
                 logger.info(
                     "Setting the name of each view to `view_idx` for list observations."
                 )
@@ -208,15 +317,15 @@
 
         if len(view_names) < len(observations):
             logger.warning(
                 "Number of views is larger than the length of `view_names`, "
                 "using only the subset of views defined in `view_names`."
             )
 
-        observations = {vn: observations[vn] for vn in view_names}
+        observations = self._merge({vn: observations[vn] for vn in view_names})
 
         n_views = len(observations)
         if n_views == 1:
             logger.warning("Running MuVI on a single view.")
 
         view_names = pd.Index(view_names)
 
@@ -298,29 +407,57 @@
     def _setup_observations(self, observations, view_names):
         if observations is None:
             raise ValueError(
                 "Observations is None, please provide a valid list of observations."
             )
 
         observations = self._setup_views(observations, view_names)
-        # from now on only working with nested dictonaries
+        # from now on only working with dictonaries
         observations = self._setup_samples(observations)
         observations = self._setup_features(observations)
 
         # keep only numpy arrays, convert to np.float32 dtypes
         return {
             vn: (
                 obs.to_numpy(dtype=np.float32)
                 if isinstance(obs, pd.DataFrame)
                 else np.array(obs, dtype=np.float32)
             )
             for vn, obs in observations.items()
         }
 
-    def _setup_prior_masks(self, masks, confidence, n_factors):
+    def _setup_prior_confidence(self, prior_confidence):
+        low = 0.99
+        med = 0.995
+        high = 0.999
+        if prior_confidence is None:
+            logger.info(
+                f"No prior confidence provided, setting `prior_confidence` to {med}."
+            )
+            prior_confidence = med
+
+        if isinstance(prior_confidence, str):
+            try:
+                prior_confidence = {"low": low, "med": med, "high": high}[
+                    prior_confidence.lower()
+                ]
+            except KeyError as e:
+                raise KeyError(
+                    "Invalid prior confidence, please provide one of `low`, `med`,"
+                    " `high` or a positive value less than 1."
+                ) from e
+
+        if not (0 < prior_confidence < 1.0):
+            raise ValueError(
+                "Invalid prior confidence, please provide a positive value less than 1."
+            )
+
+        return prior_confidence
+
+    def _setup_prior_masks(self, masks, n_factors):
         informed = masks is not None and len(masks) > 0
         valid_n_factors = n_factors is not None and n_factors > 0
         if not informed and not valid_n_factors:
             raise ValueError(
                 "Invalid latent configuration, "
                 "please provide either a collection of prior masks, "
                 "or set `n_factors` to a positive integer."
@@ -328,38 +465,20 @@
 
         if not informed:
             self.n_factors = n_factors
             # TODO: duplicate line...see below
             self.factor_names = pd.Index([f"factor_{k}" for k in range(n_factors)])
             return None, None
 
-        if confidence is None:
-            logger.info(
-                "No prior confidence provided, setting `prior_confidence` to 0.99."
-            )
-            confidence = 0.99
-
-        if isinstance(confidence, str):
-            try:
-                confidence = {"low": 0.95, "med": 0.99, "high": 0.999}[
-                    confidence.lower()
-                ]
-            except KeyError as e:
-                logger.error(e)
-                raise
-
-        if not (0 < confidence < 1.0):
-            raise ValueError(
-                "Invalid prior confidence, please provide a positive value less than 1."
-            )
-
         # if list convert to dict
         if isinstance(masks, list):
             masks = {self.view_names[m]: mask for m, mask in enumerate(masks)}
 
+        masks = self._merge(masks)
+
         informed_views = [vn for vn in self.view_names if vn in masks]
 
         n_prior_factors = masks[informed_views[0]].shape[0]
         if n_factors is None:
             n_factors = n_prior_factors
 
         if n_prior_factors > n_factors:
@@ -392,49 +511,118 @@
                 masks[vn] = np.zeros((n_prior_factors, self.n_features[vn])).astype(
                     bool
                 )
                 continue
             view_mask = masks[vn]
             if view_mask.shape[0] != n_prior_factors:
                 raise ValueError(
-                    f"Mask `{vn}` has {view_mask.shape[0]} factors "
+                    f"Mask of `{vn}` has {view_mask.shape[0]} factors "
                     f"instead of {n_prior_factors}, "
                     "all masks must have the same number of factors."
                 )
-            if view_mask.shape[1] != self.n_features[vn]:
-                raise ValueError(
-                    f"Mask `{vn}` has {view_mask.shape[1]} features "
-                    f"instead of {self.n_features[vn]}, "
-                    "each mask must match the number of features of its view."
-                )
+
+            n_features_view = self.n_features[vn]
+
+            if isinstance(view_mask, np.ndarray):
+                logger.info("np.ndarray detected.")
+                n_features_mask = view_mask.shape[1]
+                if n_features_mask != n_features_view:
+                    logger.warning(
+                        f"Mask `{vn}` has {n_features_mask} features "
+                        f"instead of {n_features_view}, "
+                        "matching mask features to the view."
+                    )
+
+                    if n_features_mask > n_features_view:
+                        # clip to the number of view features
+                        logger.info(
+                            "Mask has more features than expected, "
+                            f"keeping only the first {n_features_view} features."
+                        )
+                        view_mask = np.copy(view_mask[:, :n_features_view])
+                    else:
+                        # pad with False to match the number of view features
+                        logger.info(
+                            "Mask has fewer features than expected, "
+                            "padding the remaining features with False."
+                        )
+                        view_mask = np.concatenate(
+                            [
+                                view_mask,
+                                np.zeros(
+                                    (n_factors, n_features_view - n_features_mask)
+                                ),
+                            ],
+                            axis=1,
+                        )
 
             if isinstance(view_mask, pd.DataFrame):
                 logger.info("pd.DataFrame detected.")
 
+                feature_intersection = [
+                    fn for fn in self.feature_names[vn] if fn in view_mask.columns
+                ]
+                n_feature_intersection = len(feature_intersection)
+                if n_feature_intersection == 0:
+                    raise ValueError(
+                        f"None of the feature names for mask `{vn}` "
+                        "match the feature names of its corresponding view. "
+                        "Possible indication of passing np.array observations "
+                        "with pd.DataFrame prior masks."
+                    )
+                if n_feature_intersection < n_features_view:
+                    # pad with False to match the number of view features
+                    logger.info(
+                        "Mask has fewer features than expected, "
+                        "padding the remaining features with False."
+                    )
+                    missing_features = [
+                        fn
+                        for fn in self.feature_names[vn]
+                        if fn not in view_mask.columns
+                    ]
+                    view_mask = pd.concat(
+                        [
+                            view_mask,
+                            pd.DataFrame(
+                                False,
+                                index=view_mask.index,
+                                columns=missing_features,
+                            ),
+                        ],
+                        axis=1,
+                    )
+
+                    feature_intersection += missing_features
+
+                # otherwise simply subset features to the ones present
+                view_mask = view_mask.loc[:, feature_intersection].copy()
                 mask_factor_names = view_mask.index.copy()
                 if factor_names is None:
                     logger.info(
                         f"Storing the index of the mask `{vn}` as factor names."
                     )
                     factor_names = mask_factor_names
                 if any(factor_names != mask_factor_names):
                     logger.info(
                         f"Factor names for mask `{vn}` "
                         f"do not match the factor names of mask `{informed_views[0]}`, "
                         f"sorting names according to mask `{informed_views[0]}`."
                     )
-                    masks[vn] = view_mask.loc[factor_names, :]
+                    view_mask = view_mask.loc[factor_names, :]
 
                 if any(self.feature_names[vn] != view_mask.columns):
                     logger.info(
                         f"Feature names for mask `{vn}` "
                         "do not match the feature names of its corresponding view, "
                         "sorting names according to the view features."
                     )
-                    masks[vn] = view_mask.loc[:, self.feature_names[vn]]
+                    view_mask = view_mask.loc[:, self.feature_names[vn]]
+
+            masks[vn] = view_mask
 
         if factor_names is None:
             factor_names = [f"factor_{k}" for k in range(n_prior_factors)]
         if n_dense_factors > 0:
             factor_names = list(factor_names) + [
                 f"dense_{k}" for k in range(n_dense_factors)
             ]
@@ -455,18 +643,27 @@
                 vn: np.concatenate(
                     [vm, np.ones((n_dense_factors, self.n_features[vn])).astype(bool)]
                 )
                 for vn, vm in masks.items()
             }
 
         prior_scales = {
-            vn: np.clip(vm.astype(np.float32) + (1.0 - confidence), 1e-4, 1.0)
+            vn: np.clip(
+                vm.astype(np.float32) + (1.0 - self.prior_confidence), 1e-8, 1.0
+            )
             for vn, vm in prior_masks.items()
         }
+
+        if n_dense_factors > 0:
+            dense_scale = 1.0
+            for vn in self.view_names:
+                prior_scales[vn][n_prior_factors:, :] = dense_scale
+
         self.n_factors = n_factors
+        self.n_dense_factors = n_dense_factors
         return prior_masks, prior_scales
 
     def _setup_likelihoods(self, likelihoods):
         if likelihoods is None:
             likelihoods = ["normal" for _ in range(self.n_views)]
         if isinstance(likelihoods, list):
             likelihoods = {self.view_names[m]: ll for m, ll in enumerate(likelihoods)}
@@ -486,14 +683,57 @@
         return nmf
 
     def _setup_covariates(self, covariates):
         n_covariates = 0
         if covariates is not None:
             n_covariates = covariates.shape[1]
 
+        if isinstance(covariates, np.ndarray):
+            logger.info("np.ndarray detected.")
+            n_samples_cov = covariates.shape[0]
+            if n_samples_cov != self.n_samples:
+                logger.warning(
+                    f"Covariates have {n_samples_cov} samples "
+                    f"instead of {self.n_samples}, matching samples."
+                )
+
+                if n_samples_cov > self.n_samples:
+                    logger.info(
+                        "Covariates have more samples than expected, "
+                        f"keeping only the first {n_samples_cov} samples."
+                    )
+                    covariates = np.copy(covariates[: self.n_samples, :])
+                else:
+                    raise ValueError(
+                        "Covariates have fewer samples than expected, "
+                        "current version does not handle missing covariates"
+                    )
+
+        if isinstance(covariates, pd.DataFrame):
+            logger.info("pd.DataFrame detected.")
+
+            sample_intersection = [
+                sn for sn in self.sample_names if sn in covariates.index
+            ]
+            n_sample_intersection = len(sample_intersection)
+            if n_sample_intersection == 0:
+                raise ValueError(
+                    "None of the sample names for the covariates "
+                    "match the sample names of the observations. "
+                    "Possible indication of passing np.array observations "
+                    "with pd.DataFrame covariates."
+                )
+            if n_sample_intersection < self.n_samples:
+                raise ValueError(
+                    "Covariates have fewer samples than expected, "
+                    "current version does not handle missing covariates"
+                )
+
+            covariates = covariates.loc[sample_intersection, :].copy()
+
         covariate_names = None
         if isinstance(covariates, pd.DataFrame):
             logger.info("pd.DataFrame detected.")
             if self.n_samples != covariates.shape[0]:
                 raise ValueError(
                     f"Number of observed samples for ({self.n_samples}) "
                     "does not match the number of samples "
@@ -509,15 +749,15 @@
                 covariates = covariates.loc[self.sample_names, :]
             covariate_names = covariates.columns.copy()
             covariates = covariates.to_numpy()
         if covariate_names is None:
             covariate_names = pd.Index([f"covariate_{k}" for k in range(n_covariates)])
 
         self.n_covariates = n_covariates
-        self.covariate_names = covariate_names
+        self.covariate_names = self._validate_index(covariate_names)
         return covariates
 
     def _raise_untrained_error(self):
         if not self._trained:
             raise AttributeError(
                 "Requested attribute cannot be found on an untrained model! "
                 "Run the `fit` method to train a MuVI model."
@@ -633,26 +873,26 @@
             attr, sample_idx, self.sample_names, other_idx, other_names, as_df
         )
 
     def get_observations(
         self,
         view_idx: Index = "all",
         sample_idx: Index = "all",
-        feature_idx: Union[Index, List[Index], Dict[str, Index]] = "all",
+        feature_idx: Union[Index, list[Index], dict[str, Index]] = "all",
         as_df: bool = False,
     ):
         """Get observations.
 
         Parameters
         ----------
         view_idx : Index, optional
             View index, by default "all"
         sample_idx : Index, optional
             Sample index, by default "all"
-        feature_idx : Union[Index, List[Index], Dict[str, Index]], optional
+        feature_idx : Union[Index, list[Index], dict[str, Index]], optional
             Feature index, by default "all"
         as_df : bool, optional
             Whether to return a pandas dataframe,
             by default False
 
         Returns
         -------
@@ -674,28 +914,28 @@
             return (param > 0.5).astype(np.int32)
         return param
 
     def get_reconstructed(
         self,
         view_idx: Index = "all",
         sample_idx: Index = "all",
-        feature_idx: Union[Index, List[Index], Dict[str, Index]] = "all",
+        feature_idx: Union[Index, list[Index], dict[str, Index]] = "all",
         factor_idx: Index = "all",
         cov_idx: Index = "all",
         as_df: bool = False,
     ):
         """Get reconstructed observations.
 
         Parameters
         ----------
         view_idx : Index, optional
             View index, by default "all"
         sample_idx : Index, optional
             Sample index, by default "all"
-        feature_idx : Union[Index, List[Index], Dict[str, Index]], optional
+        feature_idx : Union[Index, list[Index], dict[str, Index]], optional
             Feature index, by default "all"
         factor_idx : Index, optional
             Factor index, by default "all"
         cov_idx : Index, optional
             Covariate index, by default "all"
         as_df : bool, optional
             Whether to return a pandas dataframe,
@@ -745,26 +985,26 @@
 
         return obs_hat
 
     def get_imputed(
         self,
         view_idx: Index = "all",
         sample_idx: Index = "all",
-        feature_idx: Union[Index, List[Index], Dict[str, Index]] = "all",
+        feature_idx: Union[Index, list[Index], dict[str, Index]] = "all",
         as_df: bool = False,
     ):
         """Get imputed observations.
 
         Parameters
         ----------
         view_idx : Index, optional
             View index, by default "all"
         sample_idx : Index, optional
             Sample index, by default "all"
-        feature_idx : Union[Index, List[Index], Dict[str, Index]], optional
+        feature_idx : Union[Index, list[Index], dict[str, Index]], optional
             Feature index, by default "all"
         as_df : bool, optional
             Whether to return a pandas dataframe,
             by default False
 
         Returns
         -------
@@ -783,26 +1023,26 @@
             }
         return obs_imputed
 
     def get_prior_masks(
         self,
         view_idx: Index = "all",
         factor_idx: Index = "all",
-        feature_idx: Union[Index, List[Index], Dict[str, Index]] = "all",
+        feature_idx: Union[Index, list[Index], dict[str, Index]] = "all",
         as_df: bool = False,
     ):
         """Get prior masks.
 
         Parameters
         ----------
         view_idx : Index, optional
             View index, by default "all"
         factor_idx : Index, optional
             Factor index, by default "all"
-        feature_idx : Union[Index, List[Index], Dict[str, Index]], optional
+        feature_idx : Union[Index, list[Index], dict[str, Index]], optional
             Feature index, by default "all"
         as_df : bool, optional
             Whether to return a pandas dataframe,
             by default False
 
         Returns
         -------
@@ -820,66 +1060,66 @@
             as_df=as_df,
         )
 
     def get_factor_loadings(
         self,
         view_idx: Index = "all",
         factor_idx: Index = "all",
-        feature_idx: Union[Index, List[Index], Dict[str, Index]] = "all",
+        feature_idx: Union[Index, list[Index], dict[str, Index]] = "all",
         as_df: bool = False,
     ):
         """Get factor loadings.
 
         Parameters
         ----------
         view_idx : Index, optional
             View index, by default "all"
         factor_idx : Index, optional
             Factor index, by default "all"
-        feature_idx : Union[Index, List[Index], Dict[str, Index]], optional
+        feature_idx : Union[Index, list[Index], dict[str, Index]], optional
             Feature index, by default "all"
         as_df : bool, optional
             Whether to return a pandas dataframe,
             by default False
 
         Returns
         -------
         dict
             Dictionary with view names as keys,
             and np.ndarray or pd.DataFrame as values.
         """
         self._raise_untrained_error()
 
         ws = self._guide.get_w(as_list=True)
-        ws = [w * self._factor_signs.to_numpy()[:, np.newaxis] for w in ws]
+        ws = [w * self._get_factor_signs().to_numpy()[:, np.newaxis] for w in ws]
         return self._get_view_attr(
             {vn: ws[m] for m, vn in enumerate(self.view_names)},
             view_idx,
             feature_idx,
             other_idx=factor_idx,
             other_names=self.factor_names,
             as_df=as_df,
         )
 
     def get_covariate_coefficients(
         self,
         view_idx: Index = "all",
         cov_idx: Index = "all",
-        feature_idx: Union[Index, List[Index], Dict[str, Index]] = "all",
+        feature_idx: Union[Index, list[Index], dict[str, Index]] = "all",
         as_df: bool = False,
     ):
         """Get factor loadings.
 
         Parameters
         ----------
         view_idx : Index, optional
             View index, by default "all"
         cov_idx : Index, optional
             Covariate index, by default "all"
-        feature_idx : Union[Index, List[Index], Dict[str, Index]], optional
+        feature_idx : Union[Index, list[Index], dict[str, Index]], optional
             Feature index, by default "all"
         as_df : bool, optional
             Whether to return a pandas dataframe,
             by default False
 
         Returns
         -------
@@ -918,15 +1158,15 @@
         -------
         Union[np.ndarray, pd.DataFrame]
             A single np.ndarray or pd.DataFrame of shape `n_samples` x `n_factors`.
         """
         self._raise_untrained_error()
 
         return self._get_sample_attr(
-            self._guide.get_z() * self._factor_signs.to_numpy(),
+            self._guide.get_z() * self._get_factor_signs().to_numpy(),
             sample_idx,
             other_idx=factor_idx,
             other_names=self.factor_names,
             as_df=as_df,
         )
 
     def get_covariates(
@@ -967,28 +1207,35 @@
 
         Returns
         -------
         bool
             Whether the build was successful
         """
         if not self._built:
+            prior_scales = None
             if not self._informed:
                 logger.warning(
                     "No prior feature sets provided, running model uninformed."
                 )
+            else:
+                prior_scales = [
+                    torch.Tensor(self.prior_scales[vn]) for vn in self.view_names
+                ]
 
             self._model = MuVIModel(
                 self.n_samples,
                 n_subsamples=batch_size,
                 n_features=[self.n_features[vn] for vn in self.view_names],
                 n_factors=self.n_factors,
+                prior_scales=prior_scales,
                 n_covariates=self.n_covariates,
                 likelihoods=[self.likelihoods[vn] for vn in self.view_names],
                 reg_hs=self.reg_hs,
                 nmf=[self.nmf[vn] for vn in self.view_names],
+                pos_transform=self.pos_transform,
                 scale_elbo=scale_elbo,
                 device=self.device,
             )
             self._guide = MuVIGuide(self._model)
             self._built = True
         return self._built
 
@@ -1086,119 +1333,125 @@
         # self.presence mask takes care of gradient updates
         train_obs = torch.nan_to_num(train_obs)
 
         train_covs = None
         if self.covariates is not None:
             train_covs = torch.Tensor(self.covariates)
 
-        train_prior_scales = None
-        if self._informed:
-            train_prior_scales = torch.cat(
-                [torch.Tensor(self.prior_scales[vn]) for vn in self.view_names], 1
-            )
-
         # make sure keys match the arguments in the forward method of the MuVIModel
         training_data = {
             "obs": train_obs,
             "mask": mask_obs,
             "covs": train_covs,
-            "prior_scales": train_prior_scales,
         }
         return {k: v for k, v in training_data.items() if v is not None}
 
     def fit(
         self,
         batch_size: int = 0,
-        n_epochs: int = 1000,
+        n_epochs: int = 0,
         n_particles: int = 0,
         learning_rate: float = 0.005,
         optimizer: str = "clipped",
         scale_elbo: bool = True,
-        callbacks: Optional[List[Callable]] = None,
+        early_stopping: bool = True,
+        callbacks: Optional[list[Callable]] = None,
         verbose: bool = True,
         seed: Optional[int] = None,
+        **kwargs,
     ):
         """Perform inference.
 
         Parameters
         ----------
         batch_size : int, optional
             Batch size, by default 0 (all samples)
         n_epochs : int, optional
             Number of iterations over the whole dataset,
-            by default 1000
+            by default 0 (10k steps)
         n_particles : int, optional
             Number of particles/samples used to form the ELBO (gradient) estimators,
             by default 0 (1000 // batch_size)
         learning_rate : float, optional
             Learning rate, by default 0.005
-        scale_elbo : bool
+        scale_elbo : bool, optional
             Whether to scale the ELBO across views, by default True
         optimizer : str, optional
-            Optimizer as string, 'adam' or 'clipped', by default "clipped"
-        callbacks : List[Callable], optional
+            Optimizer as string, "adam" or "clipped", by default "clipped"
+        early_stopping : bool, optional
+            Whether to stop training early, by default True
+        callbacks : list[Callable], optional
             List of callbacks during training, by default None
-        verbose : bool
+        verbose : bool, optional
             Whether to log progress, by default True
         seed : int, optional
             Training seed, by default None
         """
 
         # if invalid or out of bounds set to n_samples
         if batch_size is None or not (0 < batch_size <= self.n_samples):
             batch_size = self.n_samples
 
+        n_batches_per_epoch = max(1, self.n_samples // batch_size)
+        if n_epochs is None or n_epochs == 0:
+            n_epochs = 10000 // n_batches_per_epoch
+
         if n_particles < 1:
             n_particles = max(1, 1000 // batch_size)
         if n_particles > 1:
             logger.info(f"Using {n_particles} particles in parallel.")
         logger.info("Preparing model and guide...")
         self._setup_model_guide(batch_size, scale_elbo)
         logger.info("Preparing optimizer...")
         opt = self._setup_optimizer(batch_size, n_epochs, learning_rate, optimizer)
         logger.info("Preparing SVI...")
         svi = self._setup_svi(opt, n_particles, scale=True)
         logger.info("Preparing training data...")
         training_data = self._setup_training_data()
-        training_prior_scales = training_data.pop("prior_scales", None)
-        if training_prior_scales is not None:
-            training_prior_scales = training_prior_scales.to(self.device)
+
+        min_epochs = kwargs.pop("min_epochs", n_epochs // 10)
+        patience = kwargs.pop("patience", max(10, int(5 * n_batches_per_epoch)))
+        early_stopping_callback = EarlyStoppingCallback(
+            min_epochs, patience=patience, **kwargs
+        )
+
+        if callbacks is None:
+            callbacks = []
 
         if batch_size < self.n_samples:
             logger.info(f"Using batches of size `{batch_size}`.")
 
+            training_data = TensorDict(
+                dict(training_data.items()), batch_size=[self.n_samples]
+            )
+            training_data["sample_idx"] = torch.arange(self.n_samples)
+
             data_loader = DataLoader(
-                DictDataset(training_data, idx_key="sample_idx"),
+                training_data,
                 batch_size=batch_size,
                 shuffle=True,
                 num_workers=1,
+                collate_fn=identity,
                 pin_memory=str(self.device) != "cpu",
                 drop_last=False,
             )
 
             def _step():
                 iteration_loss = 0
                 for _, tensor_dict in enumerate(data_loader):
-                    iteration_loss += svi.step(
-                        **{k: v.to(self.device) for k, v in tensor_dict.items()},
-                        prior_scales=training_prior_scales,
-                    )
+                    iteration_loss += svi.step(**tensor_dict.to(self.device))
                 return iteration_loss
 
         else:
             logger.info("Using complete dataset.")
             # move all data to device once
             training_data = {k: v.to(self.device) for k, v in training_data.items()}
 
             def _step():
-                return svi.step(
-                    None,
-                    **training_data,
-                    prior_scales=training_prior_scales,
-                )
+                return svi.step(None, **training_data)
 
         if seed is not None:
             try:
                 seed = int(seed)
             except ValueError:
                 logger.warning(f"Could not convert `{seed}` to integer.")
                 seed = None
@@ -1226,19 +1479,19 @@
             for epoch_idx in pbar:
                 epoch_loss = _step()
                 history.append(epoch_loss)
                 if verbose and (
                     epoch_idx % window_size == 0 or epoch_idx == n_epochs - 1
                 ):
                     pbar.set_postfix({"ELBO": epoch_loss})
-                if callbacks is not None:
-                    # TODO: dont really like this, a bit sloppy
-                    stop_early = any(callback(history) for callback in callbacks)
-                    if stop_early:
-                        break
+                for callback in callbacks:
+                    callback(history)
+                if early_stopping and early_stopping_callback(history):
+                    stop_early = True
+                    break
         except KeyboardInterrupt:
             logger.info("Keyboard interrupt, stopping training and saving progress...")
 
         self._training_log = {
             "n_epochs": n_epochs,
             "batch_size": batch_size,
             "n_particles": n_particles,
@@ -1256,73 +1509,85 @@
 
 
 class MuVIModel(PyroModule):
     def __init__(
         self,
         n_samples: int,
         n_subsamples: int,
-        n_features: List[int],
+        n_features: list[int],
         n_factors: int,
+        prior_scales: Optional[list[torch.Tensor]],
         n_covariates: int,
-        likelihoods: List[str],
+        likelihoods: list[str],
         global_prior_scale: float = 1.0,
         reg_hs: bool = True,
-        nmf: Optional[List[bool]] = None,
+        nmf: Optional[list[bool]] = None,
+        pos_transform=None,
         scale_elbo: bool = True,
         device=None,
     ):
         """MuVI generative model.
 
         Parameters
         ----------
         n_samples : int
             Number of samples
         n_subsamples : int
             Number of subsamples (batch size)
-        n_features : List[int]
+        n_features : list[int]
             Number of features as list for each view
         n_factors : int
             Number of latent factors
+        prior_scales : list[torch.Tensor], optional
+            Local prior scales with prior information,
+            by default None (uninformed)
         n_covariates : int
             Number of covariates
-        likelihoods : List[str], optional
+        likelihoods : list[str], optional
             List of likelihoods for each view,
             either "normal" or "bernoulli", by default None
         global_prior_scale : float, optional
             Determine the level of global sparsity, by default 1.0
         reg_hs : bool, optional
             Whether to use the regularized version of HS,
             by default True
-        nmf : List[bool], optional
+        nmf : list[bool], optional
             Whether to use non-negative matrix factorization,
             by default empty (False for all views)
         scale_elbo : bool
             Whether to scale the ELBO across views, by default True
         device : str, optional
             Device to run computations on, by default "cuda" (GPU)
         """
         super().__init__(name="MuVIModel")
         self.n_samples = n_samples
         self.n_subsamples = n_subsamples
         self.n_features = n_features
         self.feature_offsets = [0, *np.cumsum(self.n_features).tolist()]
         self.n_views = len(self.n_features)
         self.n_factors = n_factors
+        self.prior_scales = prior_scales
+        if self.prior_scales is not None:
+            self.prior_scales = torch.cat(self.prior_scales, 1).to(device)
         self.n_covariates = n_covariates
         self.likelihoods = likelihoods
         self.same_likelihood = len(set(self.likelihoods)) == 1
         self.global_prior_scale = (
             1.0 if global_prior_scale is None else global_prior_scale
         )
         self.reg_hs = reg_hs
         if nmf is None:
             nmf = [False for _ in range(self.n_views)]
         self.nmf = nmf
         # only needed if nmf is True
-        self.pos_transform = torch.nn.ReLU()
+        self.pos_transform = None
+        if pos_transform == "softplus":
+            self.pos_transform = torch.nn.Softplus()
+        if pos_transform == "relu":
+            self.pos_transform = torch.nn.ReLU()
 
         self.scale_elbo = scale_elbo
         self.view_scales = np.ones(self.n_views)
         if self.scale_elbo and self.n_views > 1:
             self.view_scales = (self.n_views / (self.n_views - 1)) * (
                 1.0 - np.array([nf / sum(n_features) for nf in n_features])
             )
@@ -1339,15 +1604,19 @@
         Returns
         -------
         PlateMessenger
             A pyro plate.
         """
         plate_kwargs = {
             "view": {"name": "view", "size": self.n_views, "dim": -1},
-            "factor_left": {"name": "factor_left", "size": self.n_factors, "dim": -2},
+            "factor_left": {
+                "name": "factor_left",
+                "size": self.n_factors,
+                "dim": -2,
+            },
             "sample": {"name": "sample", "size": self.n_samples, "dim": -2},
             "covariate": {"name": "covariate", "size": self.n_covariates, "dim": -2},
         }
         for m, n_features in zip(range(self.n_views), self.n_features):
             plate_kwargs[f"feature_{m}"] = {
                 "name": f"feature_{m}",
                 "size": n_features,
@@ -1363,29 +1632,25 @@
 
     def forward(
         self,
         sample_idx: torch.Tensor,
         obs: torch.Tensor,
         mask: torch.Tensor,
         covs: Optional[torch.Tensor] = None,
-        prior_scales: Optional[torch.Tensor] = None,
     ):
         """Generate samples.
 
         Parameters
         ----------
         obs : torch.Tensor
             Observations to condition the model on
         mask : torch.Tensor
             Binary mask of missing data
         covs : torch.Tensor, optional
             Additional covariate matrix, by default None
-        prior_scales : torch.Tensor, optional
-            Local prior scales with prior information,
-            by default None
 
         Returns
         -------
         dict
             Samples from each sampling site
         """
 
@@ -1427,18 +1692,18 @@
                         output_dict[f"caux_{m}"] = pyro.sample(
                             f"caux_{m}",
                             dist.InverseGamma(
                                 0.5 * self._ones((1,)), 0.5 * self._ones((1,))
                             ),
                         )
                         c = torch.sqrt(output_dict[f"caux_{m}"])
-                        if prior_scales is not None:
+                        if self.prior_scales is not None:
                             c = (
                                 c
-                                * prior_scales[
+                                * self.prior_scales[
                                     :,
                                     self.feature_offsets[m] : self.feature_offsets[
                                         m + 1
                                     ],
                                 ]
                             )
                         w_scale = (self.global_prior_scale * c * w_scale) / torch.sqrt(
@@ -1460,18 +1725,22 @@
 
                 if self.n_covariates > 0:
                     with covariate_plate:
                         output_dict[f"beta_{m}"] = pyro.sample(
                             f"beta_{m}",
                             dist.Normal(self._zeros((1,)), self._ones((1,))),
                         )
+                        if self.nmf[m]:
+                            output_dict[f"beta_{m}"] = self.pos_transform(
+                                output_dict[f"beta_{m}"]
+                            )
 
                 output_dict[f"sigma_{m}"] = pyro.sample(
                     f"sigma_{m}",
-                    dist.InverseGamma(self._ones((1,)), self._ones((1,))),
+                    dist.LogNormal(self._zeros((1,)), self._ones((1,))),
                 )
 
         with sample_plate:
             output_dict["z"] = pyro.sample(
                 "z",
                 dist.Normal(
                     self._zeros((self.n_factors,)),
@@ -1485,27 +1754,28 @@
                     y_loc = torch.matmul(output_dict["z"], output_dict[f"w_{m}"])
                     if self.n_covariates > 0:
                         y_loc = y_loc + torch.matmul(covs, output_dict[f"beta_{m}"])
 
                     if self.likelihoods[m] == "normal":
                         y_dist = dist.Normal(
                             y_loc,
-                            torch.sqrt(output_dict[f"sigma_{m}"]),
+                            output_dict[f"sigma_{m}"],
                         )
                     else:
                         y_dist = dist.Bernoulli(logits=y_loc)
 
                     feature_idx = slice(
                         self.feature_offsets[m],
                         self.feature_offsets[m + 1],
                     )
 
-                    with pyro.poutine.mask(
-                        mask=mask[..., feature_idx]
-                    ), pyro.poutine.scale(scale=self.view_scales[m]):
+                    with (
+                        pyro.poutine.mask(mask=mask[..., feature_idx]),
+                        pyro.poutine.scale(scale=self.view_scales[m]),
+                    ):
                         output_dict[f"y_{m}"] = pyro.sample(
                             f"y_{m}",
                             y_dist,
                             obs=obs[..., feature_idx],
                             infer={"is_auxiliary": True},
                         )
 
@@ -1695,15 +1965,14 @@
 
     def forward(
         self,
         sample_idx: torch.Tensor,
         obs: torch.Tensor,
         mask: torch.Tensor,
         covs: Optional[torch.Tensor] = None,
-        prior_scales: Optional[torch.Tensor] = None,
     ):
         """Approximate posterior."""
         output_dict = {}
 
         view_plate = self.model.get_plate("view")
         factor_l_plate = self.model.get_plate("factor_left")
         feature_plates = [
```

### Comparing `muvi-0.1.1/muvi/core/synthetic.py` & `muvi-0.1.2/muvi/core/synthetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 """Data module."""
+
 import itertools
 import logging
 import math
 
-from typing import List
 from typing import Optional
-from typing import Tuple
 
 import anndata as ad
 import mudata as mu
 import numpy as np
 
 
 logger = logging.getLogger(__name__)
 
 
 class DataGenerator:
     def __init__(
         self,
         n_samples: int = 1000,
-        n_features: Optional[List[int]] = None,
-        likelihoods: Optional[List[str]] = None,
+        n_features: Optional[list[int]] = None,
+        likelihoods: Optional[list[str]] = None,
         n_fully_shared_factors: int = 2,
         n_partially_shared_factors: int = 15,
         n_private_factors: int = 3,
-        factor_size_params: Optional[Tuple[float]] = None,
+        factor_size_params: Optional[tuple[float]] = None,
         factor_size_dist: str = "uniform",
         n_active_factors: float = 1.0,
         n_covariates: int = 0,
         n_response: int = 0,
-        nmf: Optional[List[bool]] = None,
+        nmf: Optional[list[bool]] = None,
         **kwargs,
     ) -> None:
         """Generate synthetic data
 
         Parameters
         ----------
         n_samples : int, optional
             Number of samples, by default 1000
-        n_features : List[int], optional
+        n_features : list[int], optional
             Number of features for each view, by default None
-        likelihoods : List[str], optional
+        likelihoods : list[str], optional
             Likelihoods for each view, 'normal' or 'bernoulli', by default None
         n_fully_shared_factors : int, optional
             Number of fully shared latent factors, by default 2
         n_partially_shared_factors : int, optional
             Number of partially shared latent factors, by default 15
         n_private_factors : int, optional
             Number of private latent factors, by default 3
-        factor_size_params : Tuple[float], optional
+        factor_size_params : tuple[float], optional
             Parameters for the distribution of the number
             of active factor loadings for the latent factors,
             by default None
         factor_size_dist : str, optional
             Distribution of the number of active factor loadings,
             either "uniform" or "gamma",
             by default "uniform"
         n_active_factors : float, optional
             Number or fraction of active factors, by default 1.0 (all)
         n_covariates : int, optional
             Number of observed covariates, by default 0
         n_response : int, optional
             Number of response variables from the latent factors, by default 0
-        nmf : List[bool], optional
+        nmf : list[bool], optional
             Whether to generate data from a non-negative matrix factorization,
             by default False
         """
 
         self.n_samples = n_samples
         self.n_features = n_features
         self.n_views = len(self.n_features)
```

### Comparing `muvi-0.1.1/muvi/tools/cache.py` & `muvi-0.1.2/muvi/tools/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,19 +83,19 @@
             )
 
     def update_uns(self, key, scores):
         self.uns[key].update(scores)
 
     def update_factor_metadata(self, scores):
         if self.factor_adata is not None:
-            self.factor_adata.varm[Cache.META_KEY].update(scores)
+            self.factor_adata.varm[Cache.META_KEY].update(scores.astype(np.float32))
 
     def update_cov_metadata(self, scores):
         if self.cov_adata is not None:
-            self.cov_adata.varm[Cache.META_KEY].update(scores)
+            self.cov_adata.varm[Cache.META_KEY].update(scores.astype(np.float32))
 
     def filter_factors(self, factor_idx):
         self.factor_adata.obsm[Cache.FILTERED_KEY] = (
             self.factor_adata.to_df().loc[:, factor_idx].copy()
         )
         self.use_rep = Cache.FILTERED_KEY
         uns_keys = list(self.factor_adata.uns.keys())
```

### Comparing `muvi-0.1.1/muvi/tools/external.py` & `muvi-0.1.2/muvi/tools/external.py`

 * *Files identical despite different names*

### Comparing `muvi-0.1.1/muvi/tools/feature_sets.py` & `muvi-0.1.2/muvi/tools/feature_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # Highly inspired by https://github.com/krassowski/gsea-api
 import logging
 
 from collections import Counter
+from collections.abc import Collection
+from collections.abc import Iterable
 from pathlib import Path
-from typing import Collection
-from typing import Dict
-from typing import Iterable
 from typing import Optional
-from typing import Set
-from typing import Tuple
 
 import numpy as np
 import pandas as pd
 
 from sklearn.metrics import pairwise_distances
 
 
@@ -20,15 +17,15 @@
 
 
 class FeatureSet:
     def __init__(
         self,
         features: Collection[str],
         name: str,
-        description: str = "",
+        description: str = "NO_DESC",
     ):
         self.name = name
         self.features = frozenset(features)
         self.description = description
 
         if self.empty:
             logger.warning(f"FeatureSet {name!r} is empty.")
@@ -283,15 +280,16 @@
             name=self.name,
         )
 
     def filter(
         self,
         features: Iterable[str],
         min_fraction: float = 0.5,
-        min_count: int = 1,
+        min_count: int = 5,
+        max_count: Optional[int] = None,
         keep: Optional[Iterable[str]] = None,
         subset: bool = True,
     ):
         """Filter feature sets.
 
         Parameters
         ----------
@@ -299,15 +297,19 @@
             Features to filter.
         min_fraction : float, optional
             Mininimum portion of the feature set to be present in `features`,
             by default 0.5
         min_count : int, optional
             Minimum size of the intersection set
             between a feature set and the set of `features`,
-            by default 1
+            by default 5
+        max_count : int, optional
+            Maximum size of the intersection set
+            between a feature set and the set of `features`,
+            by default None
         keep : Iterable[str], optional
             Feature sets to keep regardless of the filter conditions,
             by default None
         subset : bool, optional
             Whether to subset the resulting feature sets based on `features`,
             by default True
 
@@ -326,15 +328,19 @@
         for feature_set in self.feature_sets:
             if feature_set.name in keep:
                 feature_set_subset.add(feature_set)
                 continue
             intersection = features & feature_set.features
             count = len(intersection)
             fraction = count / len(feature_set)
-            if count >= min_count and fraction >= min_fraction:
+            if (
+                count >= min_count
+                and fraction >= min_fraction
+                and (max_count is None or count <= max_count)
+            ):
                 feature_set_subset.add(feature_set)
 
         filtered_feature_sets = FeatureSets(feature_set_subset, name=self.name)
         if subset:
             filtered_feature_sets = filtered_feature_sets.subset(features)
         return filtered_feature_sets
 
@@ -436,27 +442,27 @@
                 observations.loc[:, col_subset].mean(axis=1) - obs_mean
             )
 
         return pd.DataFrame(dist_to_mean_dict).corr()
 
     def _find_similar_pairs(
         self, sim_matrix: pd.DataFrame, similarity_threshold: float
-    ) -> Set[Tuple[str, str]]:
+    ) -> set[tuple[str, str]]:
         """Find similar pairs of feature sets.
 
         Parameters
         ----------
         sim_matrix : pd.DataFrame
             Similarity matrix.
         similarity_threshold : float
             Similarity threshold to consider similar pairs.
 
         Returns
         -------
-        Set[Tuple[str, str]]
+        set[tuple[str, str]]
             Similar pairs of feature sets.
         """
 
         pairs = set()
         visited = set()
 
         row_offset = 0
@@ -476,15 +482,15 @@
         return pairs
 
     def find_similar_pairs(
         self,
         observations: pd.DataFrame = None,
         metric: Optional[str] = None,
         similarity_threshold: float = 0.8,
-    ) -> Set[Tuple[str, str]]:
+    ) -> set[tuple[str, str]]:
         """Find similar pairs of feature sets.
 
         Parameters
         ----------
         observations : pd.DataFrame, optional
             Dataframe of observations, if provided, the similarity between feature sets
             is computed based on the correlation of the similarity from the mean
@@ -493,15 +499,15 @@
             Similarity metric, by default "jaccard" if observations not provided.
         similarity_threshold : float, optional
             Similarity threshold to consider similar pairs,
             by default 0.8.
 
         Returns
         -------
-        Set[Tuple[str, str]]
+        set[tuple[str, str]]
             Similar pairs of feature sets.
         """
         if observations is None and metric is None:
             logger.warning(
                 "Neither observations nor metric is provided,"
                 " using `metric=jaccard` as default."
             )
@@ -519,20 +525,20 @@
             sim_matrix = (2 * sim_matrix[0] * sim_matrix[1]) / (
                 sim_matrix[0] + sim_matrix[1]
             )
         else:
             sim_matrix = sim_matrix[0]
         return self._find_similar_pairs(sim_matrix.fillna(0.0), similarity_threshold)
 
-    def merge_pairs(self, pairs: Iterable[Tuple[str, str]]):
+    def merge_pairs(self, pairs: Iterable[tuple[str, str]]):
         """Merge pairs of feature sets.
 
         Parameters
         ----------
-        pairs : Iterable[Tuple[str, str]]
+        pairs : Iterable[tuple[str, str]]
             Pairs of feature sets.
 
         Returns
         -------
         FeatureSets
             Merged feature sets.
         """
@@ -613,20 +619,20 @@
                     + "\t"
                     + feature_set.description
                     + "\t"
                     + "\t".join(feature_set.features)
                     + "\n"
                 )
 
-    def to_dict(self) -> Dict[str, Iterable[str]]:
+    def to_dict(self) -> dict[str, Iterable[str]]:
         """Convert this feature set collection to a dictionary.
 
         Returns
         -------
-        Dict[str, Iterable[str]]
+        dict[str, Iterable[str]]
             Dictionary of feature sets.
         """
         return {fs.name: fs.features for fs in self.feature_sets}
 
 
 def from_gmt(path: Path, name: Optional[str] = None, **kwargs) -> FeatureSets:
     """Create a FeatureSets object from a GMT file.
@@ -653,23 +659,23 @@
                     description=description,
                 )
             )
     return FeatureSets(feature_sets, name=name or Path(path).name, **kwargs)
 
 
 def from_dict(
-    d: Dict[str, Iterable[str]],
+    d: dict[str, Iterable[str]],
     name: Optional[str] = None,
     **kwargs,
 ) -> FeatureSets:
     """Create a FeatureSets object from a dictionary.
 
     Parameters
     ----------
-    d : Dict[str, Iterable[str]]
+    d : dict[str, Iterable[str]]
         Dictionary of feature sets.
     name : str, optional
         Name of the collection, by default None.
 
     Returns
     -------
     FeatureSets
@@ -705,15 +711,18 @@
 
     Returns
     -------
     FeatureSets
     """
     feature_sets = set()
     for _, row in df.iterrows():
+        description = "NO_DESC"
+        if desc_col is not None and not pd.isna(row[desc_col]):
+            description = row[desc_col]
         feature_sets.add(
             FeatureSet(
                 row[features_col],
                 name=row[name_col],
-                description=desc_col is not None and row[desc_col],
+                description=description,
             )
         )
     return FeatureSets(feature_sets, name=name, **kwargs)
```

### Comparing `muvi-0.1.1/muvi/tools/plotting.py` & `muvi-0.1.2/muvi/tools/plotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Collection of plotting functions."""
+
 import logging
 
 from typing import Optional
 from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
@@ -28,50 +29,67 @@
 DOTPLOT = "dotplot"
 TRACKSPLOT = "tracksplot"
 VIOLIN = "violin"
 STACKED_VIOLIN = "stacked_violin"
 PL_TYPES = [HEATMAP, MATRIXPLOT, DOTPLOT, TRACKSPLOT, VIOLIN, STACKED_VIOLIN]
 
 
+STRIPPLOT = "stripplot"
+BOXPLOT = "boxplot"
+BOXENPLOT = "boxenplot"
+VIOLINPLOT = "violinplot"
+GROUP_PL_TYPES = [STRIPPLOT, BOXPLOT, BOXENPLOT, VIOLINPLOT]
+
+
 def savefig_or_show(
     writekey: str,
     show: Optional[bool] = None,
     dpi: Optional[int] = None,
     ext: Optional[str] = None,
     save: Union[bool, str, None] = None,
 ):
     return sc.pl._utils.savefig_or_show(writekey, show, dpi, ext, save)
 
 
 def _subset_df(data, groupby, groups, include_rest=True):
     if groups is None:
         return data
 
+    _groups = groups.copy()
+
     if include_rest:
         data[groupby] = data[groupby].cat.add_categories(include_rest)
-        data.loc[~data[groupby].isin(groups), groupby] = include_rest
-        groups.append(include_rest)
-    data = data.loc[data[groupby].isin(groups), :].copy()
+        data.loc[~data[groupby].isin(_groups), groupby] = include_rest
+        _groups.append(include_rest)
+    data = data.loc[data[groupby].isin(_groups), :].copy()
     data[groupby] = data[groupby].cat.remove_unused_categories()
 
     if data.empty:
         raise ValueError("Empty data, check whether the provided `groups` are correct.")
 
     return data
 
 
 def _setup_legend(
-    g, bbox_to_anchor=(1, 0.5), loc="center left", frameon=False, remove_last=False
+    g,
+    bbox_to_anchor=(1, 0.5),
+    loc="center left",
+    frameon=False,
+    remove_last=False,
+    fontsize=None,
 ):
     kwargs = {"bbox_to_anchor": bbox_to_anchor, "loc": loc, "frameon": frameon}
 
     if remove_last:
         handles, labels = g.get_legend_handles_labels()
         kwargs["handles"] = handles[:-1]
         kwargs["labels"] = labels[:-1]
+
+    if fontsize is not None:
+        kwargs["fontsize"] = fontsize
     g.legend(**kwargs)
 
     return g
 
 
 def _get_color_dict(factor_adata, groupby, include_rest=True):
     uns_colors_key = f"{groupby}_colors"
@@ -218,23 +236,25 @@
     data = data.pivot(
         index="Factor",
         columns=groupby,
         values=model_cache.METRIC_R2,
     )
     data = data.loc[factor_idx]
 
+    legend_fontsize = kwargs.pop("legend_fontsize", None)
+
     g = data.plot(
         kind=kind,
         stacked=stacked,
         color=kwargs.pop("color", _get_color_dict(model_cache.factor_adata, groupby)),
         **kwargs,
     )
     g.set_ylabel(r"$R^2$")
 
-    g = _setup_legend(g)
+    g = _setup_legend(g, fontsize=legend_fontsize)
 
     g.set_title(f"Variance explained across {groupby} groups in {', '.join(view_idx)}")
     g.set(xlabel="Factor")
 
     savefig_or_show("variance_explained_grouped", show=show, save=save)
     if not show:
         return g
@@ -591,31 +611,50 @@
 def factor_activity(
     true_w,
     approx_w,
     true_mask,
     noisy_mask,
     factor_idx=0,
     ylim=None,
+    top=None,
     **kwargs,
 ):
     true_w_col = true_w[factor_idx, :]
     w_col = approx_w[factor_idx, :]
     true_mask_col = true_mask[factor_idx, :]
     noisy_mask_col = noisy_mask[factor_idx, :]
+    if top is not None:
+        # descending order
+        argsort_indices = np.argsort(-np.abs(w_col))[:top]
+        w_col = w_col[argsort_indices]
+        # remove zeros
+        non_zero_indices = np.abs(w_col) > 0
+        if non_zero_indices.sum() < top:
+            logger.warning(
+                f"Found {sum(non_zero_indices)} (< {top}) non-zero weights found,"
+                " updating the `top` parameter."
+            )
+        top = min(top, sum(non_zero_indices))
+        # subset again
+        argsort_indices = argsort_indices[:top]
+        w_col = w_col[:top]
+        true_w_col = true_w_col[argsort_indices]
+        true_mask_col = true_mask_col[argsort_indices]
+        noisy_mask_col = noisy_mask_col[argsort_indices]
 
     activity_df = pd.DataFrame(
         {
             "true_weight": true_w_col,
             "weight": w_col,
             "true_mask": true_mask_col,
             "noisy_mask": noisy_mask_col,
-            "TP": true_mask_col * noisy_mask_col,
-            "FP": (1 - true_mask_col) * noisy_mask_col,
-            "TN": (1 - true_mask_col) * (1 - noisy_mask_col),
-            "FN": true_mask_col * (1 - noisy_mask_col),
+            "TP": true_mask_col & noisy_mask_col,
+            "FP": ~true_mask_col & noisy_mask_col,
+            "TN": ~true_mask_col & ~noisy_mask_col,
+            "FN": true_mask_col & ~noisy_mask_col,
         }
     )
     activity_df.sort_values(["true_weight"], inplace=True)
 
     score_cols = ["TP", "FP", "TN", "FN"]
 
     assert (activity_df.loc[:, score_cols].values.sum(1) == 1).all()
@@ -708,19 +747,22 @@
     try:
         pl_fn = type_to_fn[pl_type]
     except KeyError as e:
         raise ValueError(
             f"`{pl_type}` is not valid. Select one of {','.join(PL_TYPES)}."
         ) from e
 
-    adata = _get_model_cache(model).factor_adata
+    factor_adata = _get_model_cache(model).factor_adata.copy()
 
     return pl_fn(
-        adata[
-            _subset_df(adata.obs.copy(), groupby, groups, include_rest=False).index, :
+        factor_adata[
+            _subset_df(
+                factor_adata.obs.copy(), groupby, groups, include_rest=False
+            ).index,
+            :,
         ],
         factor_idx,
         groupby,
         **kwargs,
     )
 
 
@@ -833,18 +875,19 @@
 def clustermap(model, factor_idx="all", **kwargs):
     factor_idx = _normalize_index(factor_idx, model.factor_names, as_idx=False)
     return sc.pl.clustermap(
         _get_model_cache(model).factor_adata[:, factor_idx], **kwargs
     )
 
 
-def stripplot(
+def _groupplot(
     model,
     factor_idx,
     groupby,
+    pl_type=STRIPPLOT,
     groups=None,
     include_rest=True,
     rot: int = 45,
     show: Optional[bool] = None,
     save: Union[bool, str, None] = None,
     **kwargs,
 ):
@@ -864,37 +907,158 @@
         axis=1,
     )
 
     data = pd.melt(data, id_vars=[groupby], var_name="Factor", value_name="Score")
 
     data = _subset_df(data, groupby, groups, include_rest=include_rest)
 
-    g = sns.stripplot(
+    if pl_type is None:
+        pl_type = STRIPPLOT
+    pl_type = pl_type.lower().strip()
+
+    type_to_fn = {
+        STRIPPLOT: sns.stripplot,
+        BOXPLOT: sns.boxplot,
+        BOXENPLOT: sns.boxenplot,
+        VIOLINPLOT: sns.violinplot,
+    }
+
+    try:
+        pl_fn = type_to_fn[pl_type]
+    except KeyError as e:
+        raise ValueError(
+            f"`{pl_type}` is not valid. Select one of {', '.join(GROUP_PL_TYPES)}."
+        ) from e
+
+    legend_fontsize = kwargs.pop("legend_fontsize", None)
+
+    g = pl_fn(
         data=data,
         x="Factor",
         y="Score",
         hue=kwargs.pop("hue", groupby),
         palette=kwargs.pop(
             "palette",
             _get_color_dict(
                 model_cache.factor_adata, groupby, include_rest=include_rest
             ),
         ),
-        dodge=kwargs.pop("dodge", True),
         **kwargs,
     )
     if rot is not None:
         for label in g.get_xticklabels():
             label.set_rotation(rot)
-    g = _setup_legend(g, remove_last=groups is not None and include_rest)
-    savefig_or_show("stripplot", show=show, save=save)
+    g = _setup_legend(
+        g, remove_last=groups is not None and include_rest, fontsize=legend_fontsize
+    )
+    savefig_or_show(pl_type, show=show, save=save)
     if not show:
         return g
 
 
+def stripplot(
+    model,
+    factor_idx,
+    groupby,
+    groups=None,
+    include_rest=True,
+    rot: int = 45,
+    show: Optional[bool] = None,
+    save: Union[bool, str, None] = None,
+    **kwargs,
+):
+    return _groupplot(
+        model,
+        factor_idx,
+        groupby,
+        pl_type=STRIPPLOT,
+        groups=groups,
+        include_rest=include_rest,
+        rot=rot,
+        show=show,
+        save=save,
+        **kwargs,
+    )
+
+
+def boxplot(
+    model,
+    factor_idx,
+    groupby,
+    groups=None,
+    include_rest=True,
+    rot: int = 45,
+    show: Optional[bool] = None,
+    save: Union[bool, str, None] = None,
+    **kwargs,
+):
+    return _groupplot(
+        model,
+        factor_idx,
+        groupby,
+        pl_type=BOXPLOT,
+        groups=groups,
+        include_rest=include_rest,
+        rot=rot,
+        show=show,
+        save=save,
+        **kwargs,
+    )
+
+
+def boxenplot(
+    model,
+    factor_idx,
+    groupby,
+    groups=None,
+    include_rest=True,
+    rot: int = 45,
+    show: Optional[bool] = None,
+    save: Union[bool, str, None] = None,
+    **kwargs,
+):
+    return _groupplot(
+        model,
+        factor_idx,
+        groupby,
+        pl_type=BOXENPLOT,
+        groups=groups,
+        include_rest=include_rest,
+        rot=rot,
+        show=show,
+        save=save,
+        **kwargs,
+    )
+
+
+def violinplot(
+    model,
+    factor_idx,
+    groupby,
+    groups=None,
+    include_rest=True,
+    rot: int = 45,
+    show: Optional[bool] = None,
+    save: Union[bool, str, None] = None,
+    **kwargs,
+):
+    return _groupplot(
+        model,
+        factor_idx,
+        groupby,
+        pl_type=VIOLINPLOT,
+        groups=groups,
+        include_rest=include_rest,
+        rot=rot,
+        show=show,
+        save=save,
+        **kwargs,
+    )
+
+
 def scatter(
     model,
     x,
     y,
     groupby=None,
     groups=None,
     include_rest=True,
@@ -914,21 +1078,19 @@
     data = _subset_df(data, groupby, groups, include_rest=include_rest)
     palette = kwargs.pop(
         "palette",
         _get_color_dict(model_cache.factor_adata, groupby, include_rest=include_rest),
     )
 
     if style is None:
-        adata = model_cache.factor_adata
-        if include_rest and groups is not None:
-            groups = groups[:-1]
-        else:
-            adata = adata[data.index, :]
+        factor_adata = model_cache.factor_adata.copy()
+        if not include_rest:
+            factor_adata = factor_adata[data.index, :]
         return sc.pl.scatter(
-            adata,
+            factor_adata,
             x,
             y,
             groups=groups,
             **kwargs,
         )
 
     logger.warning(
@@ -936,14 +1098,15 @@
         "Passing a `style` argument does not rely on `sc.pl.scatter`, "
         "and may lead to undesired results."
     )
 
     size = kwargs.pop("size", None)
     show = kwargs.pop("show", None)
     save = kwargs.pop("save", None)
+    legend_fontsize = kwargs.pop("legend_fontsize", None)
 
     kwargs = {}
 
     if size is None:
         size = 120000 / data.shape[0]
     g = sns.scatterplot(
         data=data,
@@ -956,24 +1119,33 @@
         palette=palette,
         linewidth=kwargs.pop("linewidth", 0),
         ax=kwargs.pop("ax", None),
         **kwargs,
     )
 
     # getting as close as possible to scanpy plotting style
-    g = _setup_legend(g, remove_last=groups is not None and include_rest)
+    g = _setup_legend(
+        g, remove_last=groups is not None and include_rest, fontsize=legend_fontsize
+    )
 
     g.set_title(groupby)
     savefig_or_show("scatter", show=show, save=save)
     if not show:
         return g
 
 
-def scatter_rank(model, groupby=None, groups=None, **kwargs):
-    group_df = sc.get.rank_genes_groups_df(model._cache.factor_adata, group=groups)
+def scatter_rank(model, groups=None, **kwargs):
+    factor_adata = _get_model_cache(model).factor_adata
+    try:
+        groupby = factor_adata.uns["rank_genes_groups"]["params"]["groupby"]
+    except KeyError as e:
+        raise ValueError(
+            "No group-wise ranking found, run `muvi.tl.rank first.`"
+        ) from e
+    group_df = sc.get.rank_genes_groups_df(factor_adata, group=groups)
     group_df["scores_abs"] = group_df["scores"].abs()
 
     relevant_factors_dict = {}
     for group in group_df["group"].unique():
         relevant_factors_dict[group] = (
             group_df[group_df["group"] == group]
             .sort_values("scores_abs", ascending=False)
@@ -997,7 +1169,44 @@
         )
 
         g.set_title(f"{groupby} ({group})")
         savefig_or_show(f"scatter_rank_{group}", show=show, save=save)
         gs[group] = g
     if not show:
         return gs
+
+
+def groupplot_rank(model, groups=None, pl_type=STRIPPLOT, top=1, **kwargs):
+    factor_adata = _get_model_cache(model).factor_adata
+    try:
+        groupby = factor_adata.uns["rank_genes_groups"]["params"]["groupby"]
+    except KeyError as e:
+        raise ValueError(
+            "No group-wise ranking found, run `muvi.tl.rank first.`"
+        ) from e
+    group_df = sc.get.rank_genes_groups_df(factor_adata, group=groups)
+    group_df["scores_abs"] = group_df["scores"].abs()
+
+    relevant_factors = []
+    for group in group_df["group"].unique():
+        rfs = (
+            group_df[group_df["group"] == group]
+            .sort_values("scores_abs", ascending=False)
+            .iloc[:top]["names"]
+        )
+        for rf in rfs:
+            if rf not in relevant_factors:
+                relevant_factors.append(rf)
+
+    show = kwargs.pop("show", None)
+    save = kwargs.pop("save", None)
+
+    return relevant_factors, _groupplot(
+        model,
+        relevant_factors,
+        groupby,
+        pl_type=pl_type,
+        groups=groups,
+        show=show,
+        save=save,
+        **kwargs,
+    )
```

### Comparing `muvi-0.1.1/muvi/tools/utils.py` & `muvi-0.1.2/muvi/tools/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,39 @@
+import io
 import logging
 
 from pathlib import Path
-from typing import List
 from typing import Optional
 from typing import Union
 
 import anndata as ad
 import dill as pickle
 import mudata as md
 import numpy as np
 import pandas as pd
 import pyro
 import scanpy as sc
 import scipy
+import torch
 
+from kneed import KneeLocator
 from scipy.optimize import linprog
-from sklearn.metrics import mean_squared_error
+from sklearn.metrics import root_mean_squared_error
 from statsmodels.stats import multitest
 from tqdm import tqdm
 
 from muvi.core.index import _normalize_index
 from muvi.core.models import MuVI
+from muvi.tools import feature_sets as fs
 from muvi.tools.cache import Cache
 
 
 logger = logging.getLogger(__name__)
 
-Index = Union[int, str, List[int], List[str], np.ndarray, pd.Index]
+Index = Union[int, str, list[int], list[str], np.ndarray, pd.Index]
 
 
 def setup_cache(model, overwrite: bool = False):
     """Setup model cache."""
     # check if model has been trained?
     if overwrite:
         model._cache = None
@@ -115,16 +118,15 @@
         )
         return False
 
     factor_subset = r2_sorted.index
     if r2_thresh < 1.0:
         r2_thresh = (r2_sorted.cumsum() / r2_sorted.sum() < r2_thresh).sum() + 1
 
-    if r2_thresh > 1.0:
-        factor_subset = r2_sorted.iloc[: int(r2_thresh)].index
+    factor_subset = r2_sorted.iloc[: int(r2_thresh)].index
 
     factor_subset = factor_subset.tolist()
     logger.info(f"Filtering down to {len(factor_subset)} factors.")
     return _filter_factors(model, factor_subset)
 
 
 def _recon_error(
@@ -290,15 +292,15 @@
     subsample : int, optional
         Number of samples to estimate RMSE, by default 0 (all samples)
     cache : bool, optional
         Whether to store results in the model cache, by default True
     """
 
     def _rmse(y_true, y_pred):
-        return mean_squared_error(y_true, y_pred, squared=False)
+        return root_mean_squared_error(y_true, y_pred)
 
     return _recon_error(
         model,
         view_idx,
         sample_idx,
         feature_idx,
         factor_idx,
@@ -654,60 +656,169 @@
     """Compute hierarchical clustering for the given `groupby` categories."""
     model_cache = setup_cache(model)
     kwargs["use_rep"] = model_cache.use_rep
     kwargs["n_pcs"] = None
     return sc.tl.dendrogram(model_cache.factor_adata, groupby, **kwargs)
 
 
+def posterior_feature_sets(
+    model,
+    view_idx: Index = "all",
+    factor_idx: Index = "all",
+    r2_thresh: Union[int, float] = 0.95,
+    knee_sensitivity: float = 1.0,
+    dir_path=None,
+    **kwargs,
+):
+    model_cache = setup_cache(model)
+
+    r2_cols = [f"{Cache.METRIC_R2}_{vn}" for vn in model.view_names]
+    r2_df = model_cache.factor_metadata[r2_cols]
+
+    if r2_df.isna().all(None):
+        logger.warning(
+            "Unable to filter factors based on variance explained.\n"
+            "Run `muvi.tl.variance_explained` to compute "
+            "the variance explained by each factor first. "
+            "Extracting the posterior feature sets across all factors."
+        )
+        r2_thresh = model.n_factors
+
+    if int(r2_thresh) == 1:
+        logger.warning(
+            "Unable to filter factors based on variance explained.\n"
+            f"`r2_thresh` of `{r2_thresh}` is ambiguous, `r2_thresh` must be "
+            "less than 1.0 or an integer greater than 1. "
+            "Extracting the posterior feature sets across all factors."
+        )
+        r2_thresh = model.n_factors
+
+    ws = model.get_factor_loadings(view_idx, factor_idx, as_df=True)
+
+    posterior_feature_sets = {}
+
+    for view_name, view_loadings in ws.items():
+        _r2_thresh = r2_thresh
+        view_feature_sets = {}
+        r2_sorted = r2_df[f"{Cache.METRIC_R2}_{view_name}"].sort_values(ascending=False)
+        factor_subset = r2_sorted.index
+        if _r2_thresh < 1.0:
+            _r2_thresh = (r2_sorted.cumsum() / r2_sorted.sum() < _r2_thresh).sum() + 1
+
+        factor_subset = r2_sorted.iloc[: int(_r2_thresh)].index
+
+        factor_subset = factor_subset.tolist()
+        if len(factor_subset) < model.n_factors:
+            logger.info(
+                "Extracting the posterior feature sets from "
+                f"{len(factor_subset)}/{model.n_factors} "
+                f"factors for view {view_name}."
+            )
+        for factor_name in factor_subset:
+            loadings = (
+                view_loadings.loc[factor_name, :].abs().sort_values(ascending=False)
+            )
+            kn = KneeLocator(
+                range(len(loadings)),
+                loadings,
+                S=knee_sensitivity,
+                curve="convex",
+                direction="decreasing",
+                **kwargs,
+            )
+            view_feature_sets[factor_name] = loadings.iloc[: kn.knee].index.tolist()
+        posterior_feature_sets[view_name] = view_feature_sets
+
+    if dir_path is not None:
+        Path(dir_path).mkdir(parents=True, exist_ok=True)
+        pfs_df = pd.DataFrame(posterior_feature_sets)
+        pfs_df["name"] = pfs_df.index.astype(str)
+        for view_name in ws:
+            feature_sets = fs.from_dataframe(
+                pfs_df.loc[~pfs_df[view_name].isna()],
+                name=f"muvi_posterior_{view_name}",
+                features_col=view_name,
+            )
+            feature_sets.to_gmt(Path(dir_path) / f"muvi_posterior_{view_name}.gmt")
+
+    return posterior_feature_sets
+
+
 def from_adata(
     adata,
+    obs_key: Optional[str] = None,
     prior_mask_key: Optional[str] = None,
     covariate_key: Optional[str] = None,
     **kwargs,
 ):
-    observations = [adata.to_df().copy()]
+    if obs_key is None:
+        observations = [adata.to_df().copy()]
+    else:
+        if obs_key not in adata.obsm:
+            raise ValueError(f"Invalid `obs_key`, `{obs_key}` not found in `obsm`.")
+        observations = [adata.obsm[obs_key].copy()]
     prior_masks = None
     if prior_mask_key is not None:
-        if prior_mask_key in adata.varm:
-            prior_masks = [adata.varm[prior_mask_key].T.copy()]
+        if prior_mask_key not in adata.varm:
+            logger.warning(
+                f"Invalid `prior_mask_key`, `{prior_mask_key}` not found in `varm`."
+            )
         else:
-            logger.warning("No prior information found.")
+            prior_masks = [adata.varm[prior_mask_key].T.copy()]
 
     covariates = None
     if covariate_key is not None:
+        if covariate_key not in adata.obsm:
+            raise ValueError(
+                f"Invalid `covariate_key`, `{covariate_key}` not found in `obsm`."
+            )
         covariates = adata.obsm[covariate_key].copy()
 
     return MuVI(observations, prior_masks=prior_masks, covariates=covariates, **kwargs)
 
 
 def from_mdata(
     mdata,
+    obs_key: Optional[str] = None,
     prior_mask_key: Optional[str] = None,
     covariate_key: Optional[str] = None,
     **kwargs,
 ):
     view_names = sorted(mdata.mod.keys())
-    observations = {
-        view_name: mdata.mod[view_name].to_df().copy() for view_name in view_names
-    }
+
+    observations = {}
     prior_masks = {}
-    if prior_mask_key is not None:
-        for view_name in view_names:
-            if prior_mask_key in mdata.mod[view_name].varm:
+
+    for view_name in view_names:
+        if obs_key is None:
+            observations[view_name] = mdata.mod[view_name].to_df().copy()
+        else:
+            if obs_key not in mdata.mod[view_name].obsm:
+                raise ValueError(f"Invalid `obs_key`, `{obs_key}` not found in `obsm`.")
+            observations[view_name] = mdata.mod[view_name].obsm[obs_key].copy()
+
+        if prior_mask_key is not None:
+            if prior_mask_key not in mdata.mod[view_name].varm:
+                logger.warning(
+                    f"Invalid `prior_mask_key`, `{prior_mask_key}` not found in `varm`."
+                )
+            else:
                 prior_masks[view_name] = (
                     mdata.mod[view_name].varm[prior_mask_key].T.copy()
                 )
-            else:
-                logger.warning(f"No prior information found for `{view_name}`.")
 
     if len(prior_masks) == 0:
         prior_masks = None
 
     covariates = None
     if covariate_key is not None:
+        if covariate_key not in mdata.obsm:
+            raise ValueError(
+                f"Invalid `covariate_key`, `{covariate_key}` not found in `obsm`."
+            )
         covariates = mdata.obsm[covariate_key].copy()
 
     return MuVI(observations, prior_masks=prior_masks, covariates=covariates, **kwargs)
 
 
 def to_mdata(
     model,
@@ -746,14 +857,22 @@
 
     if model.n_covariates > 0:
         mdata.obsm[covariates_key] = model.get_covariates(as_df=True)
 
     return mdata
 
 
+class CPUUnpickler(pickle.Unpickler):
+    def find_class(self, module, name):
+        if module == "torch.storage" and name == "_load_from_bytes":
+            return lambda b: torch.load(io.BytesIO(b), map_location="cpu")
+        else:
+            return super().find_class(module, name)
+
+
 def save(model, dir_path="."):
     model_path = Path(dir_path) / "model.pkl"
     params_path = Path(dir_path) / "params.save"
     factor_adata_path = Path(dir_path) / "factor.h5ad"
     cov_adata_path = Path(dir_path) / "cov.h5ad"
     for pth in [model_path, params_path, factor_adata_path, cov_adata_path]:
         if pth.exists():
@@ -798,36 +917,36 @@
         if model._cache is not None:
             model._cache.cov_adata = cov_adata
 
     pyro.get_param_store().save(params_path)
     return dir_path
 
 
-def load(dir_path=".", with_params=True):
+def load(dir_path=".", with_params=True, map_location=None):
     model_path = Path(dir_path) / "model.pkl"
     params_path = Path(dir_path) / "params.save"
     factor_adata_path = Path(dir_path) / "factor.h5ad"
     cov_adata_path = Path(dir_path) / "cov.h5ad"
 
     with open(model_path, "rb") as f:
-        model = pickle.load(f)
+        model = pickle.load(f) if map_location is None else CPUUnpickler(f).load()
 
     if model._cache is not None:
         factor_adata = None
         cov_adata = None
 
         if factor_adata_path.exists():
             factor_adata = sc.read_h5ad(factor_adata_path)
         if cov_adata_path.exists():
             cov_adata = sc.read_h5ad(cov_adata_path)
 
         model._cache.factor_adata = factor_adata
         model._cache.cov_adata = cov_adata
     if with_params:
-        pyro.get_param_store().load(params_path)
+        pyro.get_param_store().load(params_path, map_location=map_location)
     # model = pyro.module("MuVI", model, update_module_params=True)  # noqa: ERA001
     return model
 
 
 def optim_perm(matrix):
     n, n = matrix.shape
     res = linprog(
```

### Comparing `muvi-0.1.1/pyproject.toml` & `muvi-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muvi"
-version = "0.1.1"
+version = "0.1.2"
 description = "MuVI: A multi-view latent variable model with domain-informed structured sparsity for integrating noisy feature sets."
 readme = "README.md"
 authors = ["Arber Qoku <arber.qoku@dkfz-heidelberg.com>"]
 homepage = "https://github.com/MLO-lab/MuVI"
 repository = "https://github.com/MLO-lab/MuVI"
 keywords = ["multi-view", "multi-omics", "feature sets", "latent variable model", "structured sparsity", "variational inference", "single-cell"]
 
@@ -18,20 +18,25 @@
 numpy = "^1.26.1"
 pandas = "^2.1.1"
 scikit-learn = "^1.3.1"
 scipy = "^1.11.3"
 statsmodels = "^0.14.0"
 seaborn = "^0.13.0"
 # https://stackoverflow.com/questions/76327419/valueerror-libcublas-so-0-9-not-found-in-the-system-path
-torch = ">=2.0.0, !=2.0.1, !=2.1.0"
-pyro-ppl = "^1.8.6"
+torch = "^2.3.0"
+pyro-ppl = "1.8.6"
 scanpy = "^1.9.5"
 mudata = "^0.2.3"
 dill = "^0.3.7"
 tqdm = "^4.66.1"
+tabulate = "^0.9.0"
+kneed = "^0.8.5"
+igraph = "^0.11.5"
+leidenalg = "^0.10.2"
+tensordict = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "2.20.0"
 jupyter = "^1.0.0"
 ipython = "^8.10.0"
 
 [tool.poetry.group.test.dependencies]
@@ -111,9 +116,11 @@
 
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover"
 ]
 omit = [
-    "**/tests/*"
+    "**/tests/*",
+    "**/muvi/tools/plotting.py",
+    "**/muvi/tools/external.py"
 ]
```

