# Comparing `tmp/neuralnetlib-2.6.1.tar.gz` & `tmp/neuralnetlib-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.6.1.tar", last modified: Sat May 18 15:56:27 2024, max compression
+gzip compressed data, was "neuralnetlib-2.6.2.tar", last modified: Sun May 26 09:05:20 2024, max compression
```

## Comparing `neuralnetlib-2.6.1.tar` & `neuralnetlib-2.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:56:27.536441 neuralnetlib-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-18 15:56:27.536441 neuralnetlib-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:56:27.536441 neuralnetlib-2.6.1/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    45889 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14018 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:56:27.536441 neuralnetlib-2.6.1/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-18 15:56:27.000000 neuralnetlib-2.6.1/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-18 15:56:27.000000 neuralnetlib-2.6.1/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:56:27.000000 neuralnetlib-2.6.1/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 15:56:27.000000 neuralnetlib-2.6.1/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 15:56:27.000000 neuralnetlib-2.6.1/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 15:56:27.536441 neuralnetlib-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-18 15:56:17.000000 neuralnetlib-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:05:20.111579 neuralnetlib-2.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-26 09:05:20.111579 neuralnetlib-2.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:05:20.111579 neuralnetlib-2.6.2/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45889 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13974 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-26 09:05:11.000000 neuralnetlib-2.6.2/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:05:20.111579 neuralnetlib-2.6.2/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-26 09:05:20.000000 neuralnetlib-2.6.2/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-26 09:05:20.000000 neuralnetlib-2.6.2/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 09:05:20.000000 neuralnetlib-2.6.2/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 09:05:20.000000 neuralnetlib-2.6.2/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 09:05:20.000000 neuralnetlib-2.6.2/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-26 09:05:20.111579 neuralnetlib-2.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-26 09:05:12.000000 neuralnetlib-2.6.2/setup.py
```

### Comparing `neuralnetlib-2.6.1/LICENSE` & `neuralnetlib-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.6.1/PKG-INFO` & `neuralnetlib-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.6.1
+Version: 2.6.2
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.6.1/README.md` & `neuralnetlib-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.6.1/neuralnetlib/activations.py` & `neuralnetlib-2.6.2/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.6.1/neuralnetlib/callbacks.py` & `neuralnetlib-2.6.2/neuralnetlib/callbacks.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.6.1/neuralnetlib/layers.py` & `neuralnetlib-2.6.2/neuralnetlib/layers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.6.1/neuralnetlib/losses.py` & `neuralnetlib-2.6.2/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.6.1/neuralnetlib/metrics.py` & `neuralnetlib-2.6.2/neuralnetlib/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.6.1/neuralnetlib/model.py` & `neuralnetlib-2.6.2/neuralnetlib/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 
 from neuralnetlib.activations import ActivationFunction
 from neuralnetlib.layers import Layer, Input, Activation, Dropout, compatibility_dict
 from neuralnetlib.losses import LossFunction, CategoricalCrossentropy
 from neuralnetlib.optimizers import Optimizer
 from neuralnetlib.preprocessing import PCA
-from neuralnetlib.utils import shuffle, progress_bar, is_interactive
+from neuralnetlib.utils import shuffle, progress_bar, is_interactive, is_display_available
 
 
 class Model:
     def __init__(self):
         self.layers = []
         self.loss_function = None
         self.optimizer = None
@@ -122,15 +122,15 @@
             metrics: List of metric functions to evaluate the model
             random_state: Random seed for shuffling the data
             validation_data: Tuple of validation data and labels
             callbacks: List of callback objects (e.g., EarlyStopping)
             plot_decision_boundary: Whether to plot the decision boundary
         """
 
-        if plot_decision_boundary and os.getenv('DISPLAY', '') == '' and not is_interactive():
+        if plot_decision_boundary and not is_interactive() and not is_display_available():
             raise ValueError(
                 "Cannot display the plot. Please run the script in an environment with a display.")
 
         x_train = np.array(x_train) if not isinstance(
             x_train, np.ndarray) else x_train
         y_train = np.array(y_train) if not isinstance(
             y_train, np.ndarray) else y_train
@@ -228,15 +228,15 @@
                     break
 
             if verbose:
                 print()
 
             if plot_decision_boundary:
                 self.__update_plot(i, x_train, y_train, random_state)
-                plt.pause(0.1)  # Pause pour laisser le temps de mettre à jour le graphique
+                plt.pause(0.1)
 
         if plot_decision_boundary:
             plt.show(block=False)
 
         if verbose:
             print()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `neuralnetlib-2.6.1/neuralnetlib/optimizers.py` & `neuralnetlib-2.6.2/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.6.1/neuralnetlib/preprocessing.py` & `neuralnetlib-2.6.2/neuralnetlib/preprocessing.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.6.1/neuralnetlib/utils.py` & `neuralnetlib-2.6.2/neuralnetlib/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import sys
 import time
-
+import os
+import platform
+import subprocess
 import numpy as np
 
 
 def dict_with_ndarray_to_dict_with_list(d: dict) -> dict:
     """Converts all numpy arrays in a dictionary to lists. This is useful for serializing the dictionary to JSON."""
     for k, v in d.items():
         if isinstance(v, np.ndarray):
@@ -74,7 +76,37 @@
 
 def is_interactive():
     try:
         import __main__ as main
         return not hasattr(main, '__file__')
     except:
         return False
+
+
+def is_display_available():
+    system = platform.system()
+    
+    if system == "Linux":
+        return is_display_available_linux()
+    elif system == "Windows":
+        return is_display_available_windows()
+    else:
+        raise NotImplementedError(f"Display check not implemented for {system}")
+
+
+def is_display_available_linux():
+    if "DISPLAY" in os.environ:
+        try:
+            output = subprocess.check_output(["xdpyinfo"], stderr=subprocess.STDOUT)
+            return True
+        except subprocess.CalledProcessError:
+            return False
+    return False
+
+
+def is_display_available_windows():
+    try:
+        import win32api
+        display_devices = win32api.EnumDisplayDevices()
+        return bool(display_devices)
+    except Exception:
+        return False
```

### Comparing `neuralnetlib-2.6.1/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.6.2/neuralnetlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.6.1
+Version: 2.6.2
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.6.1/setup.py` & `neuralnetlib-2.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.6.1',
+    version='2.6.2',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```

