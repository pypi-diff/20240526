# Comparing `tmp/heflwr-0.1.4.tar.gz` & `tmp/heflwr-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heflwr-0.1.4.tar", last modified: Mon May 20 06:34:44 2024, max compression
+gzip compressed data, was "heflwr-0.1.5.tar", last modified: Sun May 26 10:41:08 2024, max compression
```

## Comparing `heflwr-0.1.4.tar` & `heflwr-0.1.5.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.828838 heflwr-0.1.4/
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:05:22.000000 heflwr-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       15 2024-05-14 16:05:22.000000 heflwr-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      552 2024-05-20 06:34:44.828838 heflwr-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-14 16:05:22.000000 heflwr-0.1.4/README.rst
--rw-rw-rw-   0        0        0       42 2024-05-20 06:34:44.828838 heflwr-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      608 2024-05-20 06:33:33.000000 heflwr-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.719585 heflwr-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.735432 heflwr-0.1.4/src/heflwr/
--rw-rw-rw-   0        0        0      104 2024-05-15 12:54:23.000000 heflwr-0.1.4/src/heflwr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.751134 heflwr-0.1.4/src/heflwr/fed/
--rw-rw-rw-   0        0        0       94 2024-05-20 06:25:41.000000 heflwr-0.1.4/src/heflwr/fed/__init__.py
--rw-rw-rw-   0        0        0     6687 2024-05-19 16:30:24.000000 heflwr-0.1.4/src/heflwr/fed/aggregate.py
--rw-rw-rw-   0        0        0     4796 2024-05-20 06:33:33.000000 heflwr-0.1.4/src/heflwr/fed/heflwr_aggregate.py
--rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/fed/heflwr_client_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.766957 heflwr-0.1.4/src/heflwr/log/
--rw-rw-rw-   0        0        0       22 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/log/__init__.py
--rw-rw-rw-   0        0        0     3458 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/log/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.766957 heflwr-0.1.4/src/heflwr/monitor/
--rw-rw-rw-   0        0        0       61 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.781421 heflwr-0.1.4/src/heflwr/monitor/process_monitor/
--rw-rw-rw-   0        0        0       92 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/process_monitor/__init__.py
--rw-rw-rw-   0        0        0     5522 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/process_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5541 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/process_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5356 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/process_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.797045 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/
--rw-rw-rw-   0        0        0       92 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/__init__.py
--rw-rw-rw-   0        0        0     4938 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/file_monitor.py
--rw-rw-rw-   0        0        0     5299 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
--rw-rw-rw-   0        0        0     5025 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/thread_monitor/remote_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.812876 heflwr-0.1.4/src/heflwr/monitor/utils/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/utils/__init__.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/utils/network.py
--rw-rw-rw-   0        0        0     4500 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/monitor/utils/power.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.828838 heflwr-0.1.4/src/heflwr/nn/
--rw-rw-rw-   0        0        0      153 2024-05-14 16:05:22.000000 heflwr-0.1.4/src/heflwr/nn/__init__.py
--rw-rw-rw-   0        0        0      359 2024-05-19 19:11:39.000000 heflwr-0.1.4/src/heflwr/nn/scaler.py
--rw-rw-rw-   0        0        0     3832 2024-05-19 19:19:04.000000 heflwr-0.1.4/src/heflwr/nn/ssbatchnorm2d.py
--rw-rw-rw-   0        0        0     9704 2024-05-19 19:11:39.000000 heflwr-0.1.4/src/heflwr/nn/ssconv2d.py
--rw-rw-rw-   0        0        0     9292 2024-05-19 19:11:39.000000 heflwr-0.1.4/src/heflwr/nn/sslinear.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.751134 heflwr-0.1.4/src/heflwr.egg-info/
--rw-rw-rw-   0        0        0      552 2024-05-20 06:34:44.000000 heflwr-0.1.4/src/heflwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1077 2024-05-20 06:34:44.000000 heflwr-0.1.4/src/heflwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 06:34:44.000000 heflwr-0.1.4/src/heflwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-20 06:34:44.000000 heflwr-0.1.4/src/heflwr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 06:34:44.828838 heflwr-0.1.4/tests/
--rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.4/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.746721 heflwr-0.1.5/
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:05:22.000000 heflwr-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       15 2024-05-14 16:05:22.000000 heflwr-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      495 2024-05-26 10:41:08.745725 heflwr-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2024-05-26 10:34:11.000000 heflwr-0.1.5/README.rst
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:41:08.746721 heflwr-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      608 2024-05-26 10:40:41.000000 heflwr-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.720599 heflwr-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.725069 heflwr-0.1.5/src/heflwr/
+-rw-rw-rw-   0        0        0      104 2024-05-26 10:40:41.000000 heflwr-0.1.5/src/heflwr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.729454 heflwr-0.1.5/src/heflwr/fed/
+-rw-rw-rw-   0        0        0       86 2024-05-26 07:46:59.000000 heflwr-0.1.5/src/heflwr/fed/__init__.py
+-rw-rw-rw-   0        0        0     6697 2024-05-26 08:10:01.000000 heflwr-0.1.5/src/heflwr/fed/aggregate.py
+-rw-rw-rw-   0        0        0     4782 2024-05-25 12:38:47.000000 heflwr-0.1.5/src/heflwr/fed/heflwr_aggregate.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/fed/heflwr_client_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.733125 heflwr-0.1.5/src/heflwr/log/
+-rw-rw-rw-   0        0        0      116 2024-05-23 14:23:17.000000 heflwr-0.1.5/src/heflwr/log/__init__.py
+-rw-rw-rw-   0        0        0     1396 2024-05-23 14:19:38.000000 heflwr-0.1.5/src/heflwr/log/configurator.py
+-rw-rw-rw-   0        0        0      984 2024-05-23 14:03:31.000000 heflwr-0.1.5/src/heflwr/log/handlers.py
+-rw-rw-rw-   0        0        0      661 2024-05-23 14:19:38.000000 heflwr-0.1.5/src/heflwr/log/log_info.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.733125 heflwr-0.1.5/src/heflwr/monitor/
+-rw-rw-rw-   0        0        0       61 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/monitor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.735854 heflwr-0.1.5/src/heflwr/monitor/process_monitor/
+-rw-rw-rw-   0        0        0      133 2024-05-25 11:52:25.000000 heflwr-0.1.5/src/heflwr/monitor/process_monitor/__init__.py
+-rw-rw-rw-   0        0        0     5523 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/process_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5542 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/process_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5350 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/process_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.738844 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/
+-rw-rw-rw-   0        0        0      133 2024-05-25 11:52:25.000000 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/__init__.py
+-rw-rw-rw-   0        0        0     4939 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/file_monitor.py
+-rw-rw-rw-   0        0        0     5300 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/prometheus_monitor.py
+-rw-rw-rw-   0        0        0     5019 2024-05-25 13:52:47.000000 heflwr-0.1.5/src/heflwr/monitor/thread_monitor/remote_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.740693 heflwr-0.1.5/src/heflwr/monitor/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/monitor/utils/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/monitor/utils/network.py
+-rw-rw-rw-   0        0        0     4500 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/monitor/utils/power.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.743726 heflwr-0.1.5/src/heflwr/nn/
+-rw-rw-rw-   0        0        0      153 2024-05-14 16:05:22.000000 heflwr-0.1.5/src/heflwr/nn/__init__.py
+-rw-rw-rw-   0        0        0      359 2024-05-19 19:11:39.000000 heflwr-0.1.5/src/heflwr/nn/scaler.py
+-rw-rw-rw-   0        0        0     4840 2024-05-26 09:58:40.000000 heflwr-0.1.5/src/heflwr/nn/ssbatchnorm2d.py
+-rw-rw-rw-   0        0        0     9704 2024-05-19 19:11:39.000000 heflwr-0.1.5/src/heflwr/nn/ssconv2d.py
+-rw-rw-rw-   0        0        0     9292 2024-05-19 19:11:39.000000 heflwr-0.1.5/src/heflwr/nn/sslinear.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.727427 heflwr-0.1.5/src/heflwr.egg-info/
+-rw-rw-rw-   0        0        0      495 2024-05-26 10:41:08.000000 heflwr-0.1.5/src/heflwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1137 2024-05-26 10:41:08.000000 heflwr-0.1.5/src/heflwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:41:08.000000 heflwr-0.1.5/src/heflwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 10:41:08.000000 heflwr-0.1.5/src/heflwr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 10:41:08.744728 heflwr-0.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-14 16:05:22.000000 heflwr-0.1.5/tests/test.py
```

### Comparing `heflwr-0.1.4/LICENSE` & `heflwr-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.4/setup.py` & `heflwr-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.rst", encoding="UTF-8") as f:
         return f.read()
 
 
 setup(
     name="heflwr",
-    version="0.1.4",
+    version="0.1.5",
     description="「HeFlwr」is a federated learning package for heterogeneous devices.",
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     author="Zhu Yaolin",
     author_email="zhuyaolinluck@qq.com",
     long_description=readme(),
     long_description_content_type='text/x-rst',
```

### Comparing `heflwr-0.1.4/src/heflwr/fed/aggregate.py` & `heflwr-0.1.5/src/heflwr/fed/aggregate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Union, List
 
 import torch
 
 from ..nn import SSLinear, SSConv2d
+from ..nn import SUPPORT_LAYER
 
 
 # Function to aggregate weight into the final result weight with weighted average
 def aggregate_weight(global_matrix, matrix, row_index, col_index, weight, total_weights):
     """
     Aggregates the weighted parameters between two matrices, updating the target matrix in place.
 
@@ -38,14 +39,15 @@
                 global_matrix[row_start:row_end, col_start:col_end] = (
                     (global_matrix_section * total_weights[row_start:row_end, col_start:col_end]
                      + matrix_section * weight) /
                     (total_weights[row_start:row_end, col_start:col_end] + weight)
                 )
                 total_weights[row_start:row_end, col_start:col_end] += weight
 
+
 # Function to aggregate bias into the final result bias with weighted average
 def aggregate_bias(global_bias, bias, row_index, weight, total_weights):
     """
     Aggregates the weighted bias between two bias vectors, updating the target bias vector in place.
 
     This method performs a weighted aggregation of bias values from a source bias vector to a target bias vector
     based on given row indices, as well as the specified weight.
@@ -72,16 +74,16 @@
             global_bias[start_int:end_int] = (
                 (global_bias_section * total_weights[start_int:end_int] + bias_section * weight) /
                 (total_weights[start_int:end_int] + weight)
             )
             total_weights[start_int:end_int] += weight
 
 
-def aggregate_layer(global_layer: Union[SSLinear, SSConv2d],
-                    subset_layers: List[Union[SSLinear, SSConv2d]],
+def aggregate_layer(global_layer: SUPPORT_LAYER,
+                    subset_layers: List[SUPPORT_LAYER],
                     weights: List[int]) -> None:
     """
     Performs aggregation of layer parameters from multiple subset layers into a global layer,
     taking into account specific layer types (SSLinear or SSConv2d).
 
     This function aggregates parameters (weights and biases) from a collection of subset layers
     (either SSLinear or SSConv2d) into a global layer of the same type.
```

### Comparing `heflwr-0.1.4/src/heflwr/fed/heflwr_aggregate.py` & `heflwr-0.1.5/src/heflwr/fed/heflwr_aggregate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import List, Union, Tuple
+from typing import List, Tuple
 
 import numpy as np
 import torch
 import torch.nn as nn
 from flwr.common.parameter import parameters_to_ndarrays, ndarrays_to_parameters
 from flwr.common.typing import Parameters, FitRes
 from flwr.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate_layer
 from ..nn import SUPPORT_LAYER
-from ..log.logger import logger
+from ..log import logger
 
 
 def extract(parameters: Parameters, client_net: nn.Module, server_net: nn.Module) -> Parameters:
     """
     Extracts the parameters of a client model (`client_net`) from the global server model (`server_net`)
     based on a given `Parameters` object.
```

### Comparing `heflwr-0.1.4/src/heflwr/monitor/process_monitor/file_monitor.py` & `heflwr-0.1.5/src/heflwr/monitor/process_monitor/file_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.interval = interval
         self.monitoring = multiprocessing.Event()
         self.monitor_process = None  # monitoring process
         self.metrics = {
             'cpu': True,
             'memory': True,
             'network': True,
-            'power': True,
+            'power': False,
         }
         manager = multiprocessing.Manager()
         self._stats = manager.dict({
             'cpu_usage': manager.list(),
             'memory_usage': manager.list(),
             'network_bytes_sent': manager.list(),
             'network_bytes_recv': manager.list(),
```

### Comparing `heflwr-0.1.4/src/heflwr/monitor/process_monitor/prometheus_monitor.py` & `heflwr-0.1.5/src/heflwr/monitor/process_monitor/prometheus_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.interval = interval
         self.monitoring = multiprocessing.Event()
         self.monitor_process = None  # Monitoring process
         self.metrics = {
             'cpu': True,
             'memory': True,
             'network': True,
-            'power': True,
+            'power': False,
         }
         manager = multiprocessing.Manager()
         self._stats = manager.dict({
             'cpu_usage': manager.list(),
             'memory_usage': manager.list(),
             'network_bytes_sent': manager.list(),
             'network_bytes_recv': manager.list(),
```

### Comparing `heflwr-0.1.4/src/heflwr/monitor/process_monitor/remote_monitor.py` & `heflwr-0.1.5/src/heflwr/monitor/process_monitor/remote_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 import multiprocessing
 
 import psutil
 import uuid
 
-from ...log.logger import logger, configure
+from ...log import logger, configure
 from ..utils.network import NetTrafficMonitor
 from ..utils.power import PowerMonitor
 
 
 class RemoteMonitor:
     def __init__(self, host, interval=5, identifier=None, simple=True):
         self.pid = os.getpid()
@@ -18,15 +18,15 @@
         self.interval = interval
         self.monitoring = multiprocessing.Event()
         self.monitor_process = None
         self.metrics = {
             'cpu': True,
             'memory': True,
             'network': True,
-            'power': True,
+            'power': False,
         }
         manager = multiprocessing.Manager()
         self._stats = manager.dict({
             'cpu_usage': manager.list(),
             'memory_usage': manager.list(),
             'network_bytes_sent': manager.list(),
             'network_bytes_recv': manager.list(),
```

### Comparing `heflwr-0.1.4/src/heflwr/monitor/thread_monitor/file_monitor.py` & `heflwr-0.1.5/src/heflwr/monitor/thread_monitor/file_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.interval = interval
         self.monitoring = False
         self.thread = None
         self.metrics = {
             'cpu': True,
             'memory': True,
             'network': True,
-            'power': True,
+            'power': False,
         }
         self._stats = dict({
             'cpu_usage': list(),
             'memory_usage': list(),
             'network_bytes_sent': list(),
             'network_bytes_recv': list(),
             'power_vdd_in': list(),
```

### Comparing `heflwr-0.1.4/src/heflwr/monitor/thread_monitor/prometheus_monitor.py` & `heflwr-0.1.5/src/heflwr/monitor/thread_monitor/prometheus_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.interval = interval
         self.monitoring = False
         self.thread = None
         self.metrics = {
             'cpu': True,
             'memory': True,
             'network': True,
-            'power': True,
+            'power': False,
         }
         self._stats = dict({
             'cpu_usage': list(),
             'memory_usage': list(),
             'network_bytes_sent': list(),
             'network_bytes_recv': list(),
             'power_vdd_in': list(),
```

### Comparing `heflwr-0.1.4/src/heflwr/monitor/thread_monitor/remote_monitor.py` & `heflwr-0.1.5/src/heflwr/monitor/thread_monitor/remote_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import time
 import threading
 
 import psutil
 import uuid
 
-from ...log.logger import logger, configure
+from ...log import logger, configure
 from ..utils.network import NetTrafficMonitor
 from ..utils.power import PowerMonitor
 
 
 class RemoteMonitor:
     def __init__(self, host, interval=5, identifier=None, simple=True):
         self.pid = os.getpid()
@@ -18,15 +18,15 @@
         self.interval = interval
         self.monitoring = False
         self.thread = None
         self.metrics = {
             'cpu': True,
             'memory': True,
             'network': True,
-            'power': True,
+            'power': False,
         }
         self._stats = dict({
             'cpu_usage': list(),
             'memory_usage': list(),
             'network_bytes_sent': list(),
             'network_bytes_recv': list(),
             'power_vdd_in': list(),
```

### Comparing `heflwr-0.1.4/src/heflwr/monitor/utils/network.py` & `heflwr-0.1.5/src/heflwr/monitor/utils/network.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.4/src/heflwr/monitor/utils/power.py` & `heflwr-0.1.5/src/heflwr/monitor/utils/power.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.4/src/heflwr/nn/ssbatchnorm2d.py` & `heflwr-0.1.5/src/heflwr/nn/ssbatchnorm2d.py`

 * *Files 22% similar despite different names*

```diff
@@ -87,8 +87,32 @@
             else None,
             self.running_var if not self.training or self.track_running_stats else None,
             self.weight,
             self.bias,
             bn_training,
             exponential_average_factor,
             self.eps,
-        )
+        )
+
+    @staticmethod
+    def parse_fraction_strings(fraction_str: str) -> Fraction:
+        """
+        A static method that parses a fraction in string format and returns it as a Fraction object.
+
+        The method expects the input string to represent a fraction in the format 'numerator/denominator'.
+        Special cases are '0', which returns Fraction(0, 1), and '1', which returns Fraction(1, 1).
+
+        :param fraction_str: A string that represents a fraction in the format 'numerator/denominator'.
+
+        :return: A Fraction object that corresponds to the fraction represented by the input string.
+        """
+        if fraction_str == '0':
+            return Fraction(0, 1)
+        if fraction_str == '1':
+            return Fraction(1, 1)
+        numerator, denominator = map(int, fraction_str.split('/'))
+        return Fraction(numerator, denominator)
+
+
+if __name__ == '__main__':
+    bn1 = SSBatchNorm2d(16)
+    bn2 = SSBatchNorm2d(16, channels_ranges=('0', '1/2'))
```

### Comparing `heflwr-0.1.4/src/heflwr/nn/ssconv2d.py` & `heflwr-0.1.5/src/heflwr/nn/ssconv2d.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.4/src/heflwr/nn/sslinear.py` & `heflwr-0.1.5/src/heflwr/nn/sslinear.py`

 * *Files identical despite different names*

### Comparing `heflwr-0.1.4/src/heflwr.egg-info/SOURCES.txt` & `heflwr-0.1.5/src/heflwr.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 src/heflwr.egg-info/dependency_links.txt
 src/heflwr.egg-info/top_level.txt
 src/heflwr/fed/__init__.py
 src/heflwr/fed/aggregate.py
 src/heflwr/fed/heflwr_aggregate.py
 src/heflwr/fed/heflwr_client_manager.py
 src/heflwr/log/__init__.py
-src/heflwr/log/logger.py
+src/heflwr/log/configurator.py
+src/heflwr/log/handlers.py
+src/heflwr/log/log_info.py
 src/heflwr/monitor/__init__.py
 src/heflwr/monitor/process_monitor/__init__.py
 src/heflwr/monitor/process_monitor/file_monitor.py
 src/heflwr/monitor/process_monitor/prometheus_monitor.py
 src/heflwr/monitor/process_monitor/remote_monitor.py
 src/heflwr/monitor/thread_monitor/__init__.py
 src/heflwr/monitor/thread_monitor/file_monitor.py
```

