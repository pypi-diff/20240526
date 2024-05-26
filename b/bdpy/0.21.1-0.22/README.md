# Comparing `tmp/bdpy-0.21.1.tar.gz` & `tmp/bdpy-0.22.tar.gz`

## Comparing `bdpy-0.21.1.tar` & `bdpy-0.22.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/bdata/__init__.py
--rw-r--r--   0        0        0    27829 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/bdata/bdata.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/bdata/featureselector.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/bdata/metadata.py
--rw-r--r--   0        0        0     8551 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/bdata/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dataform/__init__.py
--rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dataform/datastore.py
--rw-r--r--   0        0        0    17537 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dataform/features.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dataform/pd.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dataform/sparse.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dataset/__init__.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dataset/utils.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/distcomp/__init__.py
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/distcomp/distcomp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dl/__init__.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dl/caffe.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dl/torch/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dl/torch/base.py
--rw-r--r--   0        0        0    33214 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dl/torch/models.py
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/dl/torch/torch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/evals/__init__.py
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/evals/metrics.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/feature/__init__.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/feature/feature.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/fig/__init__.py
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/fig/draw_group_image_set.py
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/fig/fig.py
--rw-r--r--   0        0        0    26579 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/fig/makeplots.py
--rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/fig/tile_images.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/ml/__init__.py
--rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/ml/crossvalidation.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/ml/ensemble.py
--rw-r--r--   0        0        0    21498 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/ml/learning.py
--rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/ml/model.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/ml/regress.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/ml/searchlight.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/mri/__init__.py
--rw-r--r--   0        0        0    35073 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/mri/fmriprep.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/mri/glm.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/mri/image.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/mri/load_epi.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/mri/load_mri.py
--rw-r--r--   0        0        0    18772 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/mri/roi.py
--rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/mri/spm.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/opendata/__init__.py
--rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/opendata/openneuro.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/pipeline/config.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/preproc/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/preproc/interface.py
--rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/preproc/preprocessor.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/preproc/select_top.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/preproc/util.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/recon/__init__.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/recon/utils.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/recon/torch/__init__.py
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/recon/torch/icnn.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/stats/__init__.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/stats/corr.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/util/__init__.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/util/info.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/util/math.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 bdpy-0.21.1/bdpy/util/utils.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bdpy-0.21.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bdpy-0.21.1/LICENSE
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 bdpy-0.21.1/README.md
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 bdpy-0.21.1/pyproject.toml
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 bdpy-0.21.1/PKG-INFO
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/__init__.py
+-rw-r--r--   0        0        0    28717 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/bdata.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/featureselector.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/metadata.py
+-rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/bdata/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/__init__.py
+-rw-r--r--   0        0        0     7238 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/datastore.py
+-rw-r--r--   0        0        0    18041 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/features.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/pd.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/sparse.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataform/utils.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataset/__init__.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dataset/utils.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/distcomp/__init__.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/distcomp/distcomp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/__init__.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/caffe.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/torch/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/torch/base.py
+-rw-r--r--   0        0        0    33330 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/torch/models.py
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/dl/torch/torch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/evals/__init__.py
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/evals/metrics.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/feature/__init__.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/feature/feature.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/__init__.py
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/draw_group_image_set.py
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/fig.py
+-rw-r--r--   0        0        0    26579 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/makeplots.py
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/fig/tile_images.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/__init__.py
+-rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/crossvalidation.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/ensemble.py
+-rw-r--r--   0        0        0    21455 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/learning.py
+-rw-r--r--   0        0        0     8658 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/model.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/regress.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/ml/searchlight.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/__init__.py
+-rw-r--r--   0        0        0    35073 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/fmriprep.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/glm.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/image.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/load_epi.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/load_mri.py
+-rw-r--r--   0        0        0    18772 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/roi.py
+-rw-r--r--   0        0        0    11280 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/mri/spm.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/opendata/__init__.py
+-rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/opendata/openneuro.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/pipeline/config.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/interface.py
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/preprocessor.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/select_top.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/preproc/util.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/__init__.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/utils.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/torch/__init__.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/torch/deep.py
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/recon/torch/icnn.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/stats/__init__.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/stats/corr.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/util/__init__.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/util/info.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/util/math.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 bdpy-0.22/bdpy/util/utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 bdpy-0.22/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 bdpy-0.22/LICENSE
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 bdpy-0.22/README.md
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 bdpy-0.22/pyproject.toml
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 bdpy-0.22/PKG-INFO
```

### Comparing `bdpy-0.21.1/bdpy/bdata/bdata.py` & `bdpy-0.22/bdpy/bdata/bdata.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-'''BrainDecoderToolbox2/BdPy data class
-
-This file is a part of BdPy
+"""BrainDecoderToolbox2/BdPy data class.
 
+This file is a part of BdPy.
 
 API list
 --------
 
 - Data modification
     - add
     - update
@@ -16,22 +15,23 @@
     - select
     - get
     - get_metadata
     - show_metadata
 - File I/O
     - load
     - save
-'''
+"""
 
 
 __all__ = ['BData']
 
 
+from typing import Optional, Tuple, Union
+
 import os
-import sys
 import warnings
 import time
 import datetime
 import inspect
 import re
 
 import h5py
@@ -41,15 +41,15 @@
 from .metadata import MetaData
 from .featureselector import FeatureSelector
 
 
 # BData class ##########################################################
 
 class BData(object):
-    '''BrainDecoderToolbox2/BdPy data class
+    """BrainDecoderToolbox2/BdPy data class.
 
     The instance of class `BData` contains `dataset` and `metadata` as instance
     variables.
 
     Parameters
     ----------
     file_name : str, optional
@@ -58,22 +58,22 @@
         File type (default: None)
 
     If `file_name` was not given, BData.__init__() creates an empty
     dataset and metadata.
 
     Attributes
     ----------
-    dataset : numpy array (dtype=float)
+    dataset : numpy.ndarray (dtype=float)
         Dataset array
-    metadata : metadata object
+    metadata : MetaData object
         Meta-data object
-    '''
-
+    """
 
-    def __init__(self, file_name=None, file_type=None):
+    def __init__(self, file_name: Optional[str] = None, file_type: Optional[str] = None) -> None:
+        """Initialize BData instance."""
         self.__dataset = np.ndarray((0, 0), dtype=float)
         self.__metadata = MetaData()
         self.__header = {}
         self.__vmap = {}
 
         if file_name is not None:
             self.load(file_name, file_type)
@@ -120,44 +120,42 @@
     @metaData.setter
     def metaData(self, value):
         self.__metadata = value
 
     # Misc -------------------------------------------------------------
 
     def __obsoleted_method(alternative):
-        '''Decorator for obsoleted functions'''
+        """Decorator for obsoleted functions."""
         def __obsoleted_method_in(func):
             import functools
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
                 funcname = func.__name__
-                warnings.warn("'%s' is obsoleted and kept for compatibility. Use '%s' instead." % (funcname, alternative),
-                              UserWarning, stacklevel=2)
+                warnings.warn("'%s' is obsoleted and kept for compatibility. Use '%s' instead." % (funcname, alternative), UserWarning, stacklevel=2)
                 return func(*args, **kwargs)
             return wrapper
         return __obsoleted_method_in
 
 
     # Data modification ------------------------------------------------
 
-    def add(self, x, name):
-        '''Add `x` to dataset as `name`.`
+    def add(self, x: np.ndarray, name: str) -> None:
+        """Add `x` to dataset as `name`.
 
         Parameters
         ----------
-        x : array
+        x : numpy.ndarray
             Data matrix to be added in dataset
         name : str
             Name of the data `x`
 
         Returns
         -------
         None
-        '''
-
+        """
         if x.ndim == 1:
             x = x[:, np.newaxis]
 
         colnum_has = self.dataset.shape[1] # Num of existing columns in 'dataset'
         colnum_add = x.shape[1]            # Num of columns to be added
 
         # Add 'x' to dataset
@@ -170,70 +168,68 @@
         # Add new metadata
         column_description = '1 = %s' % name
         column_value = [np.nan for _ in range(colnum_has)] + [1 for _ in range(colnum_add)]
 
         self.metadata.set(name, column_value, column_description,
                           lambda x, y: np.hstack((y[:colnum_has], x[-colnum_add:])))
 
-
     @__obsoleted_method('add')
-    def add_dataset(self, x, attribute_key):
-        '''Add `x` to dataset with attribute meta-data key `attribute_key`
+    def add_dataset(self, x: np.ndarray, attribute_key: str) -> None:
+        """Add `x` to dataset with attribute meta-data key `attribute_key`.
 
         Parameters
         ----------
-        x : array
-            Data matrix to be added in dataset
+        x : numpy.ndarray
+            Data matrix to be added in dataset.
         attribute_key : str
-            Key of attribute meta-data, which specifies the columns containing `x`
+            Key of attribute meta-data, which specifies the columns containing `x`.
 
         Returns
         -------
         None
-        '''
+        """
         return self.add(x, attribute_key)
 
-
-    def update(self, key, dat):
-        '''Update dataset
+    def update(self, key: str, dat: np.ndarray) -> None:
+        """Update dataset.
 
         Parameters
         ----------
         key : str
-           Name of columns to be updated
-        dat : array_like
-           New data array
+           Name of columns to be updated.
+        dat : np.ndarray
+           New data array.
 
         Returns
         -------
         None
-        '''
+        """
         mdind = [a == 1 for a in self.get_metadata(key)]
         self.dataset[:, np.array(mdind)] = dat
 
-
-    def add_metadata(self, key, value, description='', where=None, attribute=None):
-        '''Add meta-data with `key`, `description`, and `value` to metadata
+    def add_metadata(self, key: str, value: np.ndarray, description: str = '', where: Optional[str] = None, attribute: Optional[str] = None) -> None:
+        """Add meta-data with `key`, `description`, and `value` to metadata.
 
         Parameters
         ----------
         key : str
-            Meta-data key
-        value : array
-            Meta-data array
+            Meta-data key.
+        value : numpy.ndarray
+            Meta-data array.
         description : str, optional
-            Meta-data description
+            Meta-data description.
         where : str, optional
-            Meta-data key masking the columns in the dataset
+            Meta-data key masking the columns in the dataset.
+        attribute : str, optional
+            Meta-data key masking the columns in the dataset.
 
         Returns
         -------
         None
-        '''
-
+        """
         # TODO: Add attribute specifying
         # TODO: Add size check of metadata/value
 
         if attribute is not None:
             warnings.warn("Keyword argument 'attribute' is obsoleted and kept for compatibility. Use 'where' instead.",
                           UserWarning, stacklevel=2)
             if where is not None:
@@ -247,90 +243,82 @@
             add_value = np.array([np.nan for _ in range(self.metadata.get_value_len())])
             add_value[attr_ind] = value
         else:
             add_value = value
 
         self.metadata.set(key, add_value, description)
 
-
-    def merge_metadata(self, key, sources, description='', where=None, method='logical_or'):
-        '''Merage metadata rows.'''
-
+    def merge_metadata(self, key: str, sources, description: str = '', where: Optional[str] = None, method: str = 'logical_or') -> None:
+        """Merage metadata rows."""
         if not method == 'logical_or':
             raise NotImplementedError('Only `logical_or` is implemented')
 
         if where is None:
             raise ValueError('You need to specify `where`.')
 
         mdv_lst = [self.get_metadata(s, where=where) for s in sources]
         mdv_new = np.nansum(np.vstack(mdv_lst), axis=0)
         mdv_new[mdv_new > 1] = 1
 
         self.add_metadata(key, mdv_new, description, where=where)
 
-
-    def rename_metadata(self, key_old, key_new):
-        '''Rename meta-data key
+    def rename_metadata(self, key_old: str, key_new: str) -> None:
+        """Rename meta-data key.
 
         Parameters
         ----------
         key_old, key_new : str
             Old and new meta-data keys
 
         Returns
         -------
         None
-        '''
+        """
         self.metadata.key[self.metadata.key.index(key_old)] = key_new
         return None
 
-
-    def set_metadatadescription(self, key, description):
-        '''Set description of metadata specified by `key`
+    def set_metadatadescription(self, key: str, description: str) -> None:
+        """Set description of metadata specified by `key`.
 
         Parameters
         ----------
         key : str
             Meta-data key
         description : str
             Meta-data description
 
         Returns
         -------
         None
-        '''
-
-        self.metadata.set(key, None, description,
-                          lambda x, y: y)
-
+        """
+        self.metadata.set(key, None, description, lambda x, y: y)
 
     @__obsoleted_method('set_metadatadescription')
-    def edit_metadatadescription(self, metakey, description):
-        '''Set description of metadata specified by `key`
+    def edit_metadatadescription(self, metakey: str, description: str) -> None:
+        """Set description of metadata specified by `key`.
 
         Parameters
         ----------
         key : str
             Meta-data key
         description : str
             Meta-data description
 
         Returns
         -------
         None
-        '''
+        """
         self.set_metadatadescription(metakey, description)
 
-    def update_header(self, header):
-        '''Update header.'''
+    def update_header(self, header) -> None:
+        """Update header."""
         self.__header.update(header)
 
     def applyfunc(self, func, where=None, **kargs):
-        '''Apply `func` to the dataset.'''
-
+        """Apply `func` to the dataset."""
         if where is None:
             # FIXME
             fout = func(self.dataset, **kargs)
 
             if isinstance(fout, tuple):
                 self.dataset = fout[0]
             else:
@@ -365,43 +353,42 @@
                 # No index mapping
                 self.dataset[:, x_ind] = fout
 
         return self
 
     # Data access ------------------------------------------------------
 
-    def select(self, condition, return_index=False, verbose=True):
-        '''Select data (columns) from dataset.
+    def select(self, condition: str, return_index: bool = False, verbose: bool = True) -> Union[np.ndarray, Tuple[np.ndarray, list]]:
+        """Select data (columns) from dataset.
 
         Parameters
         ----------
         condition : str
             Condition specifying columns.
         retrun_index : bool, optional
             If True, return index of selected columns (default: False).
         verbose : bool, optional
             If True, display verbose messages (default: True).
 
         Returns
         -------
-        array-like
+        numpy.ndarray
             Selected data
         list, optional
             Selected index
 
         Note
         ----
         The following operators are acceptable in `condition`.
 
         - | (or)
         - & (and)
         - = (equal)
         - @ (conditional)
-        '''
-
+        """
         expr_rpn = FeatureSelector(condition).rpn
 
         stack = []
         buf_sel = []
 
         for i in expr_rpn:
             if i == '=':
@@ -478,190 +465,181 @@
         # If buf_sel still has an element, `select_index` should be an order vector.
         # Select N elements based on the order vector.
         if buf_sel:
             num_sel = buf_sel.pop()
             selected_index = [n < num_sel for n in selected_index]
 
         # Very dirty solution
-        selected_index = np.array(selected_index) == True
+        selected_index = np.array(selected_index) == True  # Should use "==" instead of "is" here.
 
         if return_index:
             return self.dataset[:, np.array(selected_index)], selected_index
         else:
             return self.dataset[:, np.array(selected_index)]
 
-
     @__obsoleted_method('select')
-    def select_dataset(self, condition, return_index=False, verbose=True):
-        '''Select data (columns) from dataset.
+    def select_dataset(self, condition: str, return_index: bool = False, verbose: bool = True) -> Union[np.ndarray, Tuple[np.ndarray, list]]:
+        """Select data (columns) from dataset.
 
         Parameters
         ----------
         condition : str
             Condition specifying columns.
         retrun_index : bool, optional
             If True, return index of selected columns (default: False).
         verbose : bool, optional
             If True, display verbose messages (default: True).
 
         Returns
         -------
-        array-like
+        numpy.ndarray
             Selected data
         list, optional
             Selected index
 
         Note
         ----
         The following operators are acceptable in `condition`.
 
         - | (or)
         - & (and)
         - = (equal)
         - @ (conditional)
-        '''
+        """
         return self.select(condition, return_index, verbose)
 
-
     @__obsoleted_method('select')
-    def select_feature(self, condition, return_index=False, verbose=True):
-        '''Select data (columns) from dataset.
+    def select_feature(self, condition: str, return_index: bool = False, verbose: bool = True) -> Union[np.ndarray, Tuple[np.ndarray, list]]:
+        """Select data (columns) from dataset.
 
         Parameters
         ----------
         condition : str
             Condition specifying columns.
         retrun_index : bool, optional
             If True, return index of selected columns (default: False).
         verbose : bool, optional
             If True, display verbose messages (default: True).
 
         Returns
         -------
-        array-like
+        numpy.ndarray
             Selected data
         list, optional
             Selected index
 
         Note
         ----
         The following operators are acceptable in `condition`.
 
         - | (or)
         - & (and)
         - = (equal)
         - @ (conditional)
-        '''
+        """
         return self.select(condition, return_index, verbose)
 
-
-    def get(self, key=None):
-        '''Get dataset
+    def get(self, key: Optional[str] = None) -> np.ndarray:
+        """Get dataset.
 
         When `key` is not given, `get_dataset` returns `dataset`. When `key` is
         given, `get_dataset` returns data specified by `key`
-        '''
-
+        """
         if key is None:
             return self.dataset
         else:
             query = '%s = 1' % key
             return self.select(query, return_index=False, verbose=False)
 
-
     @__obsoleted_method('get')
-    def get_dataset(self, key=None):
-        '''Get dataset
+    def get_dataset(self, key: Optional[str] = None) -> np.ndarray:
+        """Get dataset.
 
         When `key` is not given, `get_dataset` returns `dataset`. When `key` is
         given, `get_dataset` returns data specified by `key`
-        '''
+        """
         return self.get(key)
 
-
-    def get_metadata(self, key, where=None):
-        '''Get value of meta-data specified by `key`
+    def get_metadata(self, key: str, where: Optional[str] = None) -> np.ndarray:
+        """Get value of meta-data specified by `key`.
 
         Parameters
         ----------
         key : str
             Meta-data key.
 
         where : str, optional
             Columns which mask meta-data array.
 
         Returns
         -------
-        array-like
-        '''
-
+        numpy.ndarray
+        """
         md = self.metadata.get(key, 'value')
 
-        if where != None:
+        if where is not None:
             # Mask the metadata array with columns specified with `where`
-            ind = self.metadata.get(where, 'value') == True
+            ind = self.metadata.get(where, 'value') == 1
             md = md[ind]
 
         return md
 
-
-    def show_metadata(self):
-        '''Show all the key and description in metadata'''
-
+    def show_metadata(self) -> None:
+        """Show all the key and description in metadata."""
         # Get max length
         max_key = max([len(k) for k in self.metadata.key])
         max_desc = max([len(k) for k in self.metadata.description])
 
         # Disp header
         print('| ' + 'Key' + ' ' * (max_key - 3) + ' | ' + 'Description' + ' ' * (max_desc - 11) + ' |')
         print('|-' + '-' * max_key + '-|-' + '-' * max_desc + '-|')
 
         # Disp key and description
         for k, d in zip(self.metadata.key, self.metadata. description):
             print('| ' + k + ' ' * (max_key - len(k)) + ' | ' + d + ' ' * (max_desc - len(d)) + ' |')
 
     # Value-label map --------------------------------------------------------
 
-    def get_labels(self, key):
-        '''Get `key` as labels.'''
-        if not key in self.__vmap:
+    def get_labels(self, key: str) -> list:
+        """Get `key` as labels."""
+        if key not in self.__vmap:
             raise ValueError('Key not found in vmap: %s' % key)
         value = self.select(key).flatten()
         label = []
         for x in value:
             if np.isnan(x):
                 v = 'n/a'
             else:
                 v = self.__vmap[key][x]
             label.append(v)
         return label
 
-    def get_label(self, key):
-        '''Get `key` as labels.'''
+    def get_label(self, key: str) -> list:
+        """Get `key` as labels."""
         return self.get_labels(key)
 
-    def get_vmap(self, key):
-        '''Returns vmap of `key`.'''
+    def get_vmap(self, key: str) -> dict:
+        """Returns vmap of `key`."""
         if key in self.__vmap:
             return self.__vmap[key]
         else:
             raise ValueError('%s not found in vmap' % key)
 
     def get_vmap_keys(self):
         return self.__vmap.keys()
 
-    def add_vmap(self, key, vmap):
-        '''Add vmap.'''
-        if not key in self.__metadata.key:
+    def add_vmap(self, key: str, vmap: dict) -> None:
+        """Add vmap."""
+        if key not in self.__metadata.key:
             raise ValueError('%s not found in metadata.' % key)
 
-        if type(vmap) is not dict:
+        if not isinstance(vmap, dict):
             raise TypeError('`vmap` should be a dictionary.')
         for k in vmap.keys():
-            if type(k) is str:
+            if isinstance(k, str):
                 raise TypeError('Keys of `vmap` should be numerical.')
 
         if key in self.__vmap:
             # Check vmap consistency
             if self.__check_vmap_consistency(vmap, self.__vmap[key]):
                 vmap.update(self.__vmap[key])
                 vmap_add = self.__get_act_vmap(key, vmap)
@@ -670,67 +648,65 @@
                 raise ValueError('Invalid vmap: labels are inconsistent between old and new vmaps.')
         else:
             vmap_add = self.__get_act_vmap(key, vmap)
             self.__vmap.update({key: vmap_add})
 
         return None
 
-    def __get_act_vmap(self, key, vmap):
+    def __get_act_vmap(self, key: str, vmap: dict) -> dict:
         values = np.unique(self.get(key))
         try:
             vmap_add = {}
             for val in values:
                 if np.isnan(val):
                     continue
                 vmap_add.update({val: vmap[val]})
-        except KeyError:
-            raise ValueError('Invalid vmap: label for %f not found.' % val)
+        except KeyError as err:
+            raise ValueError('Invalid vmap: label for %f not found.' % val) from err
         return vmap_add
 
-    def __check_vmap_consistency(self, vmap_new, vmap_old):
+    def __check_vmap_consistency(self, vmap_new: dict, vmap_old: dict) -> bool:
         for key in vmap_new.keys():
-            if not key in vmap_old:
+            if key not in vmap_old:
                 continue
             if vmap_old[key] != vmap_new[key]:
                 print('Inconsistent label:')
                 print('    Key: %f' % key)
                 print('    Old label: %s' % vmap_old[key])
                 print('    New label: %s' % vmap_new[key])
                 return False
         return True
 
     # File I/O---------------------------------------------------------
 
-    def load(self, load_filename, load_type=None):
-        '''Load 'dataset' and 'metadata' from a given file'''
-
+    def load(self, load_filename: str, load_type: Optional[str] = None) -> None:
+        """Load 'dataset' and 'metadata' from a given file."""
         if load_type is None:
             load_type = self.__get_filetype(load_filename)
 
         if load_type == "Matlab":
             self.__load_mat(load_filename)
         elif load_type == "HDF5":
             self.__load_h5(load_filename)
         else:
             raise ValueError("Unknown file type: %s" % (load_type))
 
-
-    def save(self, file_name, file_type=None):
-        '''Save 'dataset' and 'metadata' to a file'''
-
+    def save(self, file_name: str, file_type: Optional[str] = None) -> None:
+        """Save 'dataset' and 'metadata' to a file."""
         # Store data creation information
         t_now = time.time()
         t_now_str = datetime.datetime.fromtimestamp(t_now).strftime('%Y-%m-%d %H:%M:%S')
 
         callstack = []
         callstack_code = []
         f = inspect.currentframe()
         while True:
             f = f.f_back
-            if f is None: break
+            if f is None:
+                break
             fname = os.path.abspath(f.f_code.co_filename)
             fline = f.f_lineno
             callstack.append('%s:%d' % (fname, fline))
             if os.path.exists(fname):
                 with open(fname, 'r') as fl:
                     fcode = fl.read()
             else:
@@ -745,61 +721,57 @@
         if file_type is None:
             file_type = self.__get_filetype(file_name)
 
         if file_type == "Matlab":
             raise RuntimeError('Saving BData as a mat file is no longer supported. Please save the data as HDF5 (.h5).')
         elif file_type == "HDF5":
             self.__save_h5(file_name, header=self.__header)
-
         else:
             raise ValueError("Unknown file type: %s" % (file_type))
 
-
     # Private methods --------------------------------------------------
 
-    def __metadata_key_to_bool_vector(self, key):
-        '''Convert meta-dat key(s) to boolean vector.'''
+    def __metadata_key_to_bool_vector(self, key: str) -> np.ndarray:
+        """Convert meta-dat key(s) to boolean vector."""
         key_esc = re.escape(key).replace('\*', '.*') + '$'  # `fullmatch` is available in Python >= 3.4
         keys = [k for k in self.metadata.key if re.match(key_esc, k)]
         if len(keys) == 0:
             raise RuntimeError('Meta-data %s not found' % key)
         vals = np.vstack([
             self.get_metadata(k)
             for k in keys])
         vals = (vals == 1)
         vec = np.sum(vals, axis=0).astype(bool)
         return vec
 
-    def __get_order(self, v, sort_order='descend'):
+    def __get_order(self, v: np.ndarray, sort_order: str = 'descend') -> np.ndarray:
 
         # 'np.nan' comes to the last of an acending series, and thus the top of a decending series.
         # To avoid that, convert 'np.nan' to -Inf.
         v[np.isnan(v)] = -np.inf
 
         sorted_index = np.argsort(v)[::-1] # Decending order
         order = np.arange(len(v))
         for i, x in enumerate(sorted_index):
             order[x] = i
 
         return np.array(order, dtype=float)
 
-
-    def __get_top_elm_from_order(self, order, n):
-        '''Get a boolean index of top `n` elements from `order`'''
+    def __get_top_elm_from_order(self, order: np.ndarray, n: int) -> np.ndarray:
+        """Get a boolean index of top `n` elements from `order`."""
         sorted_index = np.argsort(order)
         for i, x in enumerate(sorted_index):
             order[x] = i
 
         index = np.array([r < n for r in order], dtype=bool)
 
         return index
 
-
-    def __save_h5(self, file_name, header=None):
-        '''Save data in HDF5 format (*.h5)'''
+    def __save_h5(self, file_name: str, header: Optional[dict] = None) -> None:
+        """Save data in HDF5 format (*.h5)."""
         with h5py.File(file_name, 'w') as h5file:
             # dataset
             h5file.create_dataset('/dataset', data=self.dataset)
 
             # metadata
             md_keys = self.metadata.key
             md_desc = self.metadata.description
@@ -822,17 +794,16 @@
             # vmap
             h5file.create_group('/vmap')
             for mk, vm in self.__vmap.items():
                 h5file.create_group('/vmap/' + mk)
                 for k, v in vm.items():
                     h5file.create_dataset('/vmap/' + mk + '/' + str(k), data=self.__to_bytes(v)) # FIXME: save unicode str as is
 
-    def __load_mat(self, load_filename):
-        '''Load dataset and metadata from Matlab file'''
-
+    def __load_mat(self, load_filename: str) -> None:
+        """Load dataset and metadata from Matlab file."""
         dat = sio.loadmat(load_filename)
 
         if 'metaData' in dat:
             md_keys = [str(i[0]).strip() for i in np.asarray(dat["metaData"]['key'][0, 0])[0].tolist()]
             md_descs = [str(i[0]).strip() for i in np.asarray(dat["metaData"]['description'][0, 0])[0].tolist()]
             md_values = np.asarray(dat["metaData"]['value'][0, 0])
         else:
@@ -848,18 +819,16 @@
         if 'header' in dat:
             self.__header = dat['header']
 
         self.__metadata.key = md_keys
         self.__metadata.value = md_values
         self.__metadata.description = md_descs
 
-
-    def __load_h5(self, load_filename):
-        '''Load dataset and metadata from HDF5 file'''
-
+    def __load_h5(self, load_filename: str) -> None:
+        """Load dataset and metadata from HDF5 file."""
         dat = h5py.File(load_filename, 'r')
 
         if 'metaData' in dat:
             md_keys = [self.__to_unicode(x) for x in dat["metaData"]['key'][:].tolist()]
             md_descs = [self.__to_unicode(x) for x in dat["metaData"]['description'][:].tolist()]
             md_values = np.asarray(dat["metaData"]['value'], dtype=float)
         else:
@@ -882,40 +851,34 @@
                 self.__header.update({k: v})
 
         if 'vmap' in dat:
             for mk in dat['vmap'].keys():
                 vmap = {}
                 for k in dat['vmap'][mk].keys():
                     vmap.update({float(k): self.__to_unicode(dat['vmap'][mk][k][()])})
-                # TODO: fix this dirty solution
-                if sys.version_info.major == 2:
-                    mk = mk.encode('utf-8')
                 self.__vmap.update({mk: vmap})
 
         self.__metadata.key = md_keys
         self.__metadata.value = md_values
         self.__metadata.description = md_descs
 
     def __to_unicode(self, s):
-        '''Convert s (bytes) to unicode str.'''
-        if sys.version_info.major == 3:
-            if isinstance(s, bytes):
-                return s.decode('utf-8')
+        """Convert s (bytes) to unicode str."""
+        if isinstance(s, bytes):
+            return s.decode('utf-8')
         return s
 
     def __to_bytes(self, s):
-        '''Convert s (unicode str) to bytes.'''
-        if sys.version_info.major == 3:
-            if isinstance(s, str):
-                return s.encode('utf-8')
+        """Convert s (unicode str) to bytes."""
+        if isinstance(s, str):
+            return s.encode('utf-8')
         return s
 
-    def __get_filetype(self, file_name):
-        '''Return the type of `file_name` based on the file extension'''
-
+    def __get_filetype(self, file_name: str):
+        """Return the type of `file_name` based on the file extension."""
         _, ext = os.path.splitext(file_name)
 
         if ext == ".mat":
             file_type = "Matlab"
         elif ext == ".h5":
             file_type = "HDF5"
         else:
```

### Comparing `bdpy-0.21.1/bdpy/bdata/featureselector.py` & `bdpy-0.22/bdpy/bdata/featureselector.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/bdata/metadata.py` & `bdpy-0.22/bdpy/bdata/metadata.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/bdata/utils.py` & `bdpy-0.22/bdpy/bdata/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-'''Utility functions for BData'''
+"""Utility functions for BData."""
 
 
+from typing import List
+
 import copy
-import sys
 
 import numpy as np
 
 from .bdata import BData
 
 
 def vstack(bdata_list, successive=[], metadata_merge='strict', ignore_metadata_description=False):
-    '''Concatenate datasets vertically.
+    """Concatenate datasets vertically.
 
     Currently, `concat_dataset` does not validate the consistency of meta-data
     among data.
 
     Parameters
     ----------
     bdata_list : list of BData
@@ -34,15 +35,15 @@
     dat : BData
         Concatenated data
 
     Example
     -------
 
         data = vstack([data0, data1, data2], successive=['Session', 'Run', 'Block'])
-    '''
+    """
 
     suc_cols = {s : 0 for s in successive}
 
     dat = BData()  # Concatenated BData
 
     for ds in bdata_list:
         ds_copy = copy.deepcopy(ds)
@@ -58,18 +59,15 @@
             # Create new BData
             dat.dataset = ds_copy.dataset
             dat.metadata = ds_copy.metadata
 
             # vmap
             vmap_keys = ds_copy.get_vmap_keys()
             for vk in vmap_keys:
-                if sys.version_info.major == 2:
-                    dat.add_vmap(vk.encode(), ds_copy.get_vmap(vk.encode()))
-                else:
-                    dat.add_vmap(vk, ds_copy.get_vmap(vk))
+                dat.add_vmap(vk, ds_copy.get_vmap(vk))
         else:
             # Check metadata consistency
             if metadata_merge == 'strict':
                 if not metadata_equal(dat, ds_copy):
                     raise ValueError('Inconsistent meta-data.')
             elif metadata_merge == 'minimal':
                 # Only meta-data shared across BDatas are kept.
@@ -98,92 +96,89 @@
 
             # Concatenate BDatas
             dat.dataset = np.vstack([dat.dataset, ds_copy.dataset])
 
             # Merge vmap
             vmap_keys = ds_copy.get_vmap_keys()
             for vk in vmap_keys:
-                if sys.version_info.major == 2:
-                    dat.add_vmap(vk.encode(), ds_copy.get_vmap(vk.encode()))
-                else:
-                    dat.add_vmap(vk, ds_copy.get_vmap(vk))
+                dat.add_vmap(vk, ds_copy.get_vmap(vk))
 
         # Update the last values in sucessive columns
         for s in successive:
             v = dat.select(s)
             suc_cols[s] = np.max(v)
 
     return dat
 
 
 def resolve_vmap(bdata_list):
-    """ Replace the conflicting vmaps for multiple bdata with non-conflicting vmaps.
+    """Replace the conflicting vmaps for multiple bdata with non-conflicting vmaps.
 
     Parameters
     ----------
     bdata_list : list of BData
         Data to be concatenated
-        
+
     Returns
-    -------        
-    bdata_list : list of BData 
+    -------
+    bdata_list : list of BData
         The vmap is fixed to avoid a collision.
     """
     # Get the vmap key list.
     vmap_keys = bdata_list[0].get_vmap_keys()
-    
+
     # Check each vmap key.
     for vmap_key in vmap_keys:
         new_vmap = {}
         # Check each bdata vmap.
         for ds in bdata_list:
             vmap = ds.get_vmap(vmap_key)
             ds_values, selector = ds.select(vmap_key, return_index = True) # keep original dataset values
             new_dsvalues = copy.deepcopy(ds_values)  # to update
-            
+
             # Sanity check
             if not vmap_key in ds.metadata.key:
                 raise ValueError('%s not found in metadata.' % vmap_key)
             if type(vmap) is not dict:
                 raise TypeError('`vmap` should be a dictionary.')
             for vk in vmap.keys():
                 if type(vk) is str:
                     raise TypeError('Keys of `vmap` should be numerical.')
-            
+
             # Check duplicate and create new vmap
             for vk in vmap.keys():
                 if vk not in new_vmap.keys():
                     # If find a novel key, add the new key and new value
                     new_vmap[vk] = vmap[vk]
                 elif new_vmap[vk] != vmap[vk]:
                     # If find the exisiting key and the values are different,
                     # assign a new key by incrementing 1 to the maximum exisiting key.
-                    inflation_key_value = max(new_vmap.keys()) 
+                    inflation_key_value = max(new_vmap.keys())
                     new_vmap[inflation_key_value + 1] = vmap[vk]
                     # Update dataset values
                     new_dsvalues[ds_values == vk] = inflation_key_value + 1
                 else:
                     # If the key and value is same, nothing to do.
                     pass
-                
+
             # Update dataset
             ds.dataset[:, selector] = new_dsvalues
 
         # Update each bdata vmap.
         for ds in bdata_list:
             vmap = ds.get_vmap(vmap_key)
-            if not np.array_equal(sorted(list(vmap.keys())), sorted(list(new_vmap.keys()))): 
+            if not np.array_equal(sorted(list(vmap.keys())), sorted(list(new_vmap.keys()))):
                 # If the present vmap is different from new_vmap, update it.
                 ds._BData__vmap[vmap_key] = new_vmap # BDataクラスにvmapのsetterがあると良い
-        
-    return bdata_list   
+
+    return bdata_list
 
 
 def concat_dataset(data_list, successive=[]):
-    '''Concatenate datasets
+    """Concatenate datasets
 
     Currently, `concat_dataset` does not validate the consistency of meta-data
     among data.
 
     Parameters
     ----------
     data_list : list of BData
@@ -197,31 +192,31 @@
     dat : BData
         Concatenated data
 
     Example
     -------
 
         data = concat_dataset([data0, data1, data2], successive=['Session', 'Run', 'Block'])
-    '''
+    """
 
     return vstack(data_list, successive=successive)
 
 
 def metadata_equal(d0, d1, strict=False):
-    '''Check whether `d0` and `d1` share the same meta-data.
+    """Check whether `d0` and `d1` share the same meta-data.
 
     Parameters
     ----------
     d0, d1 : BData
     strict : bool, optional
 
     Returns
     -------
     bool
-    '''
+    """
 
     equal = True
 
     # Strict check
     if not d0.metadata.key == d1.metadata.key:
         equal = False
     if not d0.metadata.description == d1.metadata.description:
@@ -252,7 +247,17 @@
 
         try:
             np.testing.assert_equal(d0_mval, d1_mval)
         except AssertionError:
             return False
 
     return True
+
+
+def select_data_multi_bdatas(bdatas: List[BData], roi_selector: str) -> np.ndarray:
+    """Load brain data from multiple BDatas."""
+    return np.vstack([b.select(roi_selector) for b in bdatas])
+
+
+def get_labels_multi_bdatas(bdatas: List[BData], label_name: str) -> List[str]:
+    """Load brain data from multiple BDatas."""
+    return [label for b in bdatas for label in b.get_labels(label_name)]
```

### Comparing `bdpy-0.21.1/bdpy/dataform/datastore.py` & `bdpy-0.22/bdpy/dataform/datastore.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/dataform/features.py` & `bdpy-0.22/bdpy/dataform/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import scipy.io as sio
 import hdf5storage
 
 
 def _load_array_with_key(key: str, path: str) -> np.ndarray:
     try:
         return sio.loadmat(path)[key]
-    except NotImplementedError:
+    except (NotImplementedError, ValueError):
         return hdf5storage.loadmat(path)[key]
 
 
 def _determine_num_parallel(num_files: int) -> int:
     # NOTE: optimal number of parallel processes is not clear. It could depend
     # on several factors such as the number of files, the size of files, the
     # number of cores, etc. For now, we use a simple heuristic based on the
@@ -142,16 +142,19 @@
         else:
             labels = label
 
         features: np.ndarray
         num_labels = len(labels)
         num_parallel = _determine_num_parallel(num_labels)
         path_iterator = map(lambda label: self.__feature_file_table[layer][label], labels)
-        with Pool(processes=num_parallel) as pool:
-            features = np.concatenate(pool.map(partial(_load_array_with_key, 'feat'), path_iterator), axis=0)
+        if num_parallel == 1:
+            features = np.concatenate(list(map(partial(_load_array_with_key, 'feat'), path_iterator)), axis=0)
+        else:
+            with Pool(processes=num_parallel) as pool:
+                features = np.concatenate(pool.map(partial(_load_array_with_key, 'feat'), path_iterator), axis=0)
 
         if self.__feat_index_table is not None:
             # Select features by index
             self.__feature_index = self.__feat_index_table[layer]
             n_sample = features.shape[0]
             n_feat = np.array(features.shape[1:]).prod()
 
@@ -211,16 +214,19 @@
             assert isinstance(self.__features, np.ndarray)
             return self.__features  # self.__features could be None
 
         features: np.ndarray
         num_labels = len(self.__labels)
         num_parallel = _determine_num_parallel(num_labels)
         path_iterator = map(lambda label: self.__feature_file_table[layer][label], self.__labels)
-        with Pool(processes=num_parallel) as pool:
-            features = np.concatenate(pool.map(partial(_load_array_with_key, 'feat'), path_iterator), axis=0)
+        if num_parallel == 1:
+            features = np.concatenate(list(map(partial(_load_array_with_key, 'feat'), path_iterator)), axis=0)
+        else:
+            with Pool(processes=num_parallel) as pool:
+                features = np.concatenate(pool.map(partial(_load_array_with_key, 'feat'), path_iterator), axis=0)
         self.__features = features
 
         self.__c_feature_name = layer
 
         if self.__feat_index_table is not None:
             # Select features by index
             self.__feature_index = self.__feat_index_table[layer]
@@ -372,16 +378,19 @@
 
         if len(files) == 0:
             raise RuntimeError('No decoded feature found')
 
         features: np.ndarray
         num_files = len(files)
         num_parallel = _determine_num_parallel(num_files)
-        with Pool(processes=num_parallel) as pool:
-            features = np.concatenate(pool.map(partial(_load_array_with_key, self.__file_key), files), axis=0)
+        if num_parallel == 1:
+            features = np.concatenate(list(map(partial(_load_array_with_key, self.__file_key), files)), axis=0)
+        else:
+            with Pool(processes=num_parallel) as pool:
+                features = np.concatenate(pool.map(partial(_load_array_with_key, self.__file_key), files), axis=0)
 
         if self.__squeeze:
             features = np.squeeze(features)
 
         return features
 
     def statistic(self, statistic='mean', layer=None, subject=None, roi=None, fold=None):
```

### Comparing `bdpy-0.21.1/bdpy/dataform/pd.py` & `bdpy-0.22/bdpy/dataform/pd.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/dataform/sparse.py` & `bdpy-0.22/bdpy/dataform/sparse.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/dataset/utils.py` & `bdpy-0.22/bdpy/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/distcomp/distcomp.py` & `bdpy-0.22/bdpy/distcomp/distcomp.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/dl/caffe.py` & `bdpy-0.22/bdpy/dl/caffe.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/dl/torch/base.py` & `bdpy-0.22/bdpy/dl/torch/base.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/dl/torch/models.py` & `bdpy-0.22/bdpy/dl/torch/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     Parameters
     ----------
     model : nn.Module
         Network model.
     layer_name : str
         Layer name. It accepts the following formats: 'layer_name',
-        'layer_name[index]', 'parent_name.child_name', and combinations of them.
+        '[index]', 'parent_name.child_name', and combinations of them.
 
     Returns
     -------
     nn.Module
         Layer object.
 
     Examples
@@ -119,26 +119,27 @@
 
     # parse layer name having parent name (e.g., 'features.conv1')
     if '.' in layer_name:
         top_most_layer_name, child_layer_name = layer_name.split('.', 1)
         model = _parse_layer_name(model, top_most_layer_name)
         return _parse_layer_name(model, child_layer_name)
 
-    # parse layer name having index (e.g., 'features[0]', 'backbone[0][1]')
-    pattern = re.compile(r'^(?P<layer_name>\w+)(?P<index>(\[(\d+)\])+)$')
+    # parse layer name having index (e.g., '[0]', 'features[0]', 'backbone[0][1]')
+    pattern = re.compile(r'^(?P<layer_name>[a-zA-Z_]+[a-zA-Z0-9_]*)?(?P<index>(\[(\d+)\])+)$')
     m = pattern.match(layer_name)
     if m is not None:
-        layer_name = m.group('layer_name')
+        layer_name: str | None = m.group('layer_name')  # NOTE: layer_name can be None
         index_str = m.group('index')
 
         indeces = re.findall(r'\[(\d+)\]', index_str)
         indeces = [int(i) for i in indeces]
 
-        if hasattr(model, layer_name):
-            return _get_value_by_indices(getattr(model, layer_name), indeces)
+        if isinstance(layer_name, str) and hasattr(model, layer_name):
+            model = getattr(model, layer_name)
+        return _get_value_by_indices(model, indeces)
 
     raise ValueError(
         f"Invalid layer name: '{layer_name}'. Either the syntax of '{layer_name}' is not supported, "
         f"or {type(model).__name__} object has no attribute '{layer_name}'.")
 
 
 def model_factory(name: str) -> nn.Module:
```

### Comparing `bdpy-0.21.1/bdpy/dl/torch/torch.py` & `bdpy-0.22/bdpy/dl/torch/torch.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/evals/metrics.py` & `bdpy-0.22/bdpy/evals/metrics.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/feature/feature.py` & `bdpy-0.22/bdpy/feature/feature.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/fig/draw_group_image_set.py` & `bdpy-0.22/bdpy/fig/draw_group_image_set.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/fig/fig.py` & `bdpy-0.22/bdpy/fig/fig.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/fig/makeplots.py` & `bdpy-0.22/bdpy/fig/makeplots.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/fig/tile_images.py` & `bdpy-0.22/bdpy/fig/tile_images.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/ml/crossvalidation.py` & `bdpy-0.22/bdpy/ml/crossvalidation.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/ml/ensemble.py` & `bdpy-0.22/bdpy/ml/ensemble.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/ml/learning.py` & `bdpy-0.22/bdpy/ml/learning.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,15 @@
         if self.__is_done(output_files_all):
             if os.path.isdir(self.save_path):
                 info_file = os.path.join(self.save_path, 'info.yaml')
 
                 if os.path.exists(info_file):
                     while True:
                         with open(info_file, 'r') as f:
-                            info = yaml.load(f)  # NOTE: this will raise an error, yaml.load() takes two arguments
+                            info = yaml.load(f, Loader=yaml.SafeLoader)
                         if info is None:
                             print('Failed to load info from %s. Retrying ...' % info_file)
                             sleep(1)
                         else:
                             print('Loaded info from %s' % info_file)
                             break
                 else:
```

### Comparing `bdpy-0.21.1/bdpy/ml/model.py` & `bdpy-0.22/bdpy/ml/model.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/ml/regress.py` & `bdpy-0.22/bdpy/ml/regress.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/ml/searchlight.py` & `bdpy-0.22/bdpy/ml/searchlight.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/mri/fmriprep.py` & `bdpy-0.22/bdpy/mri/fmriprep.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/mri/glm.py` & `bdpy-0.22/bdpy/mri/glm.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/mri/image.py` & `bdpy-0.22/bdpy/mri/image.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/mri/load_epi.py` & `bdpy-0.22/bdpy/mri/load_epi.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/mri/load_mri.py` & `bdpy-0.22/bdpy/mri/load_mri.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/mri/roi.py` & `bdpy-0.22/bdpy/mri/roi.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/mri/spm.py` & `bdpy-0.22/bdpy/mri/spm.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/opendata/openneuro.py` & `bdpy-0.22/bdpy/opendata/openneuro.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/pipeline/config.py` & `bdpy-0.22/bdpy/pipeline/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     # DictConfig of struct mode doesn't accept insertion of new keys.
     # Dirty solution
     OmegaConf.set_struct(cfg, False)
     cfg._run_ = {
         "name": called_by_name,
         "path": called_by_path,
         "timestamp": date_str,
+        "config_name": config_name,
+        "config_path": str(config_file.absolute()),
     }
 
     # code = cfg.get("code", None)
     cfg._analysis_name_ = args.analysis
     if cfg._analysis_name_ is None:
         cfg._analysis_name_ = called_by_name
```

### Comparing `bdpy-0.21.1/bdpy/preproc/interface.py` & `bdpy-0.22/bdpy/preproc/interface.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/preproc/preprocessor.py` & `bdpy-0.22/bdpy/preproc/preprocessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 import copy
 import sys
 from abc import ABCMeta, abstractmethod
 
 import numpy as np
 from numpy.matlib import repmat
+# NOTE: PendingDeprecationWarning: Importing from numpy.matlib is deprecated since 1.19.0.
+# repmat(a, m, n) is equivalent to tile(a, (m, n)). Use tile instead.
+# c.f. https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
 
 
 ## Abstract preprocessor #######################################################
 
 class Preprocessor(object):
     """
     Abstract class for preprocessing
```

### Comparing `bdpy-0.21.1/bdpy/preproc/select_top.py` & `bdpy-0.22/bdpy/preproc/select_top.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,25 +37,25 @@
         print_start_msg()
 
     num_elem = data.shape[axis]
 
     value = np.array([-np.inf if np.isnan(a) else a for a in value])
     sorted_index = np.argsort(value)[::-1]
 
-    rank = np.zeros(num_elem, dtype=np.int)
+    rank = np.zeros(num_elem, dtype=np.uint8)
     rank[sorted_index] = np.array(range(0, num_elem))
 
     selected_index_bool = rank < num
 
     if axis == 0:
         selected_data = data[selected_index_bool, :]
-        selected_index = np.array(range(0, num_elem), dtype=np.int)[selected_index_bool]
+        selected_index = np.array(range(0, num_elem), dtype=np.uint8)[selected_index_bool]
     elif axis == 1:
         selected_data = data[:, selected_index_bool]
-        selected_index = np.array(range(0, num_elem), dtype=np.int)[selected_index_bool]
+        selected_index = np.array(range(0, num_elem), dtype=np.uint8)[selected_index_bool]
     else:
         raise ValueError('Invalid axis')
 
     if verbose:
         print_finish_msg()
 
     return selected_data, selected_index
```

### Comparing `bdpy-0.21.1/bdpy/recon/utils.py` & `bdpy-0.22/bdpy/recon/utils.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/recon/torch/icnn.py` & `bdpy-0.22/bdpy/recon/torch/icnn.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/stats/corr.py` & `bdpy-0.22/bdpy/stats/corr.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/util/info.py` & `bdpy-0.22/bdpy/util/info.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/util/math.py` & `bdpy-0.22/bdpy/util/math.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/bdpy/util/utils.py` & `bdpy-0.22/bdpy/util/utils.py`

 * *Files identical despite different names*

### Comparing `bdpy-0.21.1/LICENSE` & `bdpy-0.22/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017-2023 Kamitani Lab
+Copyright (c) 2017-2024 Kamitani Lab
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `bdpy-0.21.1/README.md` & `bdpy-0.22/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,22 +27,27 @@
     - tqdm
 - `dl.torch` module
     - PyTorch
     - Pillow
 - `fig` module
     - matplotlib
     - Pillow
+- `bdpy.ml` module
+    - tqdm
 - `mri` module
     - nipy
     - nibabel
     - pandas
 - `recon.torch` module
     - PyTorch
     - Pillow
 
+### Optional requirements for testing
+- fastl2lir
+
 ## Installation
 
 Latest stable release:
 
 ``` shell
 $ pip install bdpy
 ```
```

### Comparing `bdpy-0.21.1/pyproject.toml` & `bdpy-0.22/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bdpy"
-version = "0.21.1"
+version = "0.22"
 description = "Brain decoder toolbox for Python"
 authors = [
     { name = "Shuntaro C. Aoki", email = "s_aoki@i.kyoto-u.ac.jp" }
 ]
 readme = "README.md"
 requires-python = ">= 3.6, < 3.12"
 license = { file = "LICENSE" }
```

