# Comparing `tmp/first-breaks-picking-gpu-0.6.2.tar.gz` & `tmp/first_breaks_picking_gpu-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\a\first_breaks_picking\first_breaks_picking\dist\.tmp-ugeuqr_u\first-breaks-picking-gpu-0.6.2.tar", last modified: Sun Feb 25 15:22:36 2024, max compression
+gzip compressed data, was "D:\a\first_breaks_picking\first_breaks_picking\dist\.tmp-_0spd6zl\first_breaks_picking_gpu-0.7.1.tar", last modified: Sun May 26 20:44:34 2024, max compression
```

## Comparing `first-breaks-picking-gpu-0.6.2.tar` & `first_breaks_picking_gpu-0.7.1.tar`

### file list

```diff
@@ -1,59 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-02-25 15:22:36.050280 first-breaks-picking-gpu-0.6.2/
--rw-rw-rw-   0        0        0    11558 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/LICENSE
--rw-rw-rw-   0        0        0       98 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0    39635 2024-02-25 15:22:36.050280 first-breaks-picking-gpu-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0    24912 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-25 15:22:36.019030 first-breaks-picking-gpu-0.6.2/first_breaks/
--rw-rw-rw-   0        0        0        5 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/VERSION
--rw-rw-rw-   0        0        0     1125 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/__init__.py
--rw-rw-rw-   0        0        0       96 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/__main__.py
--rw-rw-rw-   0        0        0      369 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/cli.py
--rw-rw-rw-   0        0        0     1090 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/const.py
-drwxrwxrwx   0        0        0        0 2024-02-25 15:22:36.019030 first-breaks-picking-gpu-0.6.2/first_breaks/data_models/
--rw-rw-rw-   0        0        0        0 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/data_models/__init__.py
--rw-rw-rw-   0        0        0     2695 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/data_models/dependent.py
--rw-rw-rw-   0        0        0     5628 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/data_models/independent.py
--rw-rw-rw-   0        0        0      730 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/data_models/initialised_defaults.py
-drwxrwxrwx   0        0        0        0 2024-02-25 15:22:36.034656 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/
--rw-rw-rw-   0        0        0        0 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/__init__.py
--rw-rw-rw-   0        0        0     4586 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/bandfilter_widget.py
--rw-rw-rw-   0        0        0     5684 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/byte_encode_unit_widget.py
--rw-rw-rw-   0        0        0     1969 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/combobox_with_mapping.py
--rw-rw-rw-   0        0        0    23064 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/graph.py
--rw-rw-rw-   0        0        0    19218 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/main_gui.py
--rw-rw-rw-   0        0        0     3340 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/nn_manager.py
--rw-rw-rw-   0        0        0     6908 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/picking_widget.py
--rw-rw-rw-   0        0        0     2752 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/radioset_widget.py
--rw-rw-rw-   0        0        0     5246 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/roi_manager.py
--rw-rw-rw-   0        0        0    18696 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/settings_processing_widget.py
--rw-rw-rw-   0        0        0     3672 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/slider_with_values.py
--rw-rw-rw-   0        0        0     5211 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/spectrum_window.py
--rw-rw-rw-   0        0        0     2978 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/threads.py
--rw-rw-rw-   0        0        0     6984 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/tooltip_widget.py
--rw-rw-rw-   0        0        0     7054 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/desktop/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-25 15:22:36.034656 first-breaks-picking-gpu-0.6.2/first_breaks/picking/
--rw-rw-rw-   0        0        0        0 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/picking/__init__.py
--rw-rw-rw-   0        0        0     1283 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/picking/ipicker.py
--rw-rw-rw-   0        0        0     5736 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/picking/picker_onnx.py
--rw-rw-rw-   0        0        0     6957 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/picking/task.py
--rw-rw-rw-   0        0        0     2715 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/picking/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-25 15:22:36.034656 first-breaks-picking-gpu-0.6.2/first_breaks/sgy/
--rw-rw-rw-   0        0        0        0 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/sgy/__init__.py
--rw-rw-rw-   0        0        0     8852 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/sgy/headers.py
--rw-rw-rw-   0        0        0    16727 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/sgy/reader.py
-drwxrwxrwx   0        0        0        0 2024-02-25 15:22:36.034656 first-breaks-picking-gpu-0.6.2/first_breaks/utils/
--rw-rw-rw-   0        0        0        0 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/utils/__init__.py
--rw-rw-rw-   0        0        0     3058 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/utils/cuda.py
--rw-rw-rw-   0        0        0      654 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/utils/debug.py
--rw-rw-rw-   0        0        0     4195 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/utils/fourier_transforms.py
--rw-rw-rw-   0        0        0     6468 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/utils/utils.py
--rw-rw-rw-   0        0        0     3937 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/first_breaks/utils/visualizations.py
-drwxrwxrwx   0        0        0        0 2024-02-25 15:22:36.050280 first-breaks-picking-gpu-0.6.2/first_breaks_picking_gpu.egg-info/
--rw-rw-rw-   0        0        0    39635 2024-02-25 15:22:35.000000 first-breaks-picking-gpu-0.6.2/first_breaks_picking_gpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1674 2024-02-25 15:22:36.000000 first-breaks-picking-gpu-0.6.2/first_breaks_picking_gpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-25 15:22:35.000000 first-breaks-picking-gpu-0.6.2/first_breaks_picking_gpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-02-25 15:22:35.000000 first-breaks-picking-gpu-0.6.2/first_breaks_picking_gpu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      157 2024-02-25 15:22:35.000000 first-breaks-picking-gpu-0.6.2/first_breaks_picking_gpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-02-25 15:22:35.000000 first-breaks-picking-gpu-0.6.2/first_breaks_picking_gpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2466 2024-02-25 15:20:59.000000 first-breaks-picking-gpu-0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0      433 2024-02-25 15:22:36.050280 first-breaks-picking-gpu-0.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:34.988333 first_breaks_picking_gpu-0.7.1/
+-rw-rw-rw-   0        0        0    11558 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0       98 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    40276 2024-05-26 20:44:34.988333 first_breaks_picking_gpu-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    25526 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:34.957082 first_breaks_picking_gpu-0.7.1/first_breaks/
+-rw-rw-rw-   0        0        0        5 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/VERSION
+-rw-rw-rw-   0        0        0     1176 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/__init__.py
+-rw-rw-rw-   0        0        0       96 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/__main__.py
+-rw-rw-rw-   0        0        0      369 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/cli.py
+-rw-rw-rw-   0        0        0     1144 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/const.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:34.972708 first_breaks_picking_gpu-0.7.1/first_breaks/data_models/
+-rw-rw-rw-   0        0        0        0 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/data_models/__init__.py
+-rw-rw-rw-   0        0        0     2695 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/data_models/dependent.py
+-rw-rw-rw-   0        0        0     4736 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/data_models/independent.py
+-rw-rw-rw-   0        0        0      696 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/data_models/initialised_defaults.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:34.972708 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/
+-rw-rw-rw-   0        0        0        0 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/__init__.py
+-rw-rw-rw-   0        0        0     4586 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/bandfilter_widget.py
+-rw-rw-rw-   0        0        0     5816 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/byte_encode_unit_widget.py
+-rw-rw-rw-   0        0        0     1969 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/combobox_with_mapping.py
+-rw-rw-rw-   0        0        0    10802 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/export_widgets.py
+-rw-rw-rw-   0        0        0    22914 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/graph.py
+-rw-rw-rw-   0        0        0      776 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/last_folder_manager.py
+-rw-rw-rw-   0        0        0    15866 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/main_gui.py
+-rw-rw-rw-   0        0        0    12133 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/multiselect_widget.py
+-rw-rw-rw-   0        0        0     3340 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/nn_manager.py
+-rw-rw-rw-   0        0        0    22055 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/picks_manager_widget.py
+-rw-rw-rw-   0        0        0     2752 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/radioset_widget.py
+-rw-rw-rw-   0        0        0     5246 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/roi_manager.py
+-rw-rw-rw-   0        0        0    15998 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/settings_processing_widget.py
+-rw-rw-rw-   0        0        0     3672 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/slider_with_values.py
+-rw-rw-rw-   0        0        0     5211 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/spectrum_window.py
+-rw-rw-rw-   0        0        0     2978 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/threads.py
+-rw-rw-rw-   0        0        0     6984 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/tooltip_widget.py
+-rw-rw-rw-   0        0        0     8104 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/desktop/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:34.972708 first_breaks_picking_gpu-0.7.1/first_breaks/exports/
+-rw-rw-rw-   0        0        0        0 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/exports/__init__.py
+-rw-rw-rw-   0        0        0     4352 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/exports/export_picks.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:34.988333 first_breaks_picking_gpu-0.7.1/first_breaks/picking/
+-rw-rw-rw-   0        0        0        0 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/picking/__init__.py
+-rw-rw-rw-   0        0        0     1283 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/picking/ipicker.py
+-rw-rw-rw-   0        0        0     6267 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/picking/picker_onnx.py
+-rw-rw-rw-   0        0        0     5412 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/picking/picks.py
+-rw-rw-rw-   0        0        0     2902 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/picking/task.py
+-rw-rw-rw-   0        0        0     2715 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/picking/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:34.988333 first_breaks_picking_gpu-0.7.1/first_breaks/sgy/
+-rw-rw-rw-   0        0        0        0 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/sgy/__init__.py
+-rw-rw-rw-   0        0        0     8852 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/sgy/headers.py
+-rw-rw-rw-   0        0        0    16909 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/sgy/reader.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:34.988333 first_breaks_picking_gpu-0.7.1/first_breaks/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/utils/__init__.py
+-rw-rw-rw-   0        0        0     3058 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/utils/cuda.py
+-rw-rw-rw-   0        0        0      654 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/utils/debug.py
+-rw-rw-rw-   0        0        0     4195 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/utils/fourier_transforms.py
+-rw-rw-rw-   0        0        0     6863 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/utils/utils.py
+-rw-rw-rw-   0        0        0     3937 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/first_breaks/utils/visualizations.py
+drwxrwxrwx   0        0        0        0 2024-05-26 20:44:34.988333 first_breaks_picking_gpu-0.7.1/first_breaks_picking_gpu.egg-info/
+-rw-rw-rw-   0        0        0    40276 2024-05-26 20:44:34.000000 first_breaks_picking_gpu-0.7.1/first_breaks_picking_gpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1906 2024-05-26 20:44:34.000000 first_breaks_picking_gpu-0.7.1/first_breaks_picking_gpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 20:44:34.000000 first_breaks_picking_gpu-0.7.1/first_breaks_picking_gpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-26 20:44:34.000000 first_breaks_picking_gpu-0.7.1/first_breaks_picking_gpu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      174 2024-05-26 20:44:34.000000 first_breaks_picking_gpu-0.7.1/first_breaks_picking_gpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-26 20:44:34.000000 first_breaks_picking_gpu-0.7.1/first_breaks_picking_gpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2485 2024-05-26 20:43:07.000000 first_breaks_picking_gpu-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0      433 2024-05-26 20:44:34.988333 first_breaks_picking_gpu-0.7.1/setup.cfg
```

### Comparing `first-breaks-picking-gpu-0.6.2/LICENSE` & `first_breaks_picking_gpu-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/PKG-INFO` & `first_breaks_picking_gpu-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking-gpu
-Version: 0.6.2
+Version: 0.7.1
 Summary: Project is devoted to pick waves that are the first to be detected on a seismogram with neural network (CUDA accelerated)
 Author: Aleksei Tarasov
 Author-email: Aleksei Tarasov <aleksei.v.tarasov@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,31 +213,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <=3.10,>=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.28.2
-Requires-Dist: numpy==1.24.2
-Requires-Dist: pandas==2.0.0
-Requires-Dist: PyQt5==5.15.9
-Requires-Dist: pyqtgraph==0.13.3
-Requires-Dist: tqdm==4.65.0
-Requires-Dist: click==8.1.3
-Requires-Dist: pydantic==2.0.3
-Requires-Dist: pytest==7.3.2
-Requires-Dist: onnxruntime-gpu==1.14.1
+Requires-Dist: requests>=2.28.2
+Requires-Dist: numpy>=1.24.2
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: PyQt5>=5.15.9
+Requires-Dist: pyqtgraph>=0.13.3
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: click>=8.1.3
+Requires-Dist: pydantic>=2.0.3
+Requires-Dist: pytest>=7.3.2
+Requires-Dist: pytest-qt>=4.4.0
+Requires-Dist: onnxruntime-gpu>=1.14.1
 
 # FirstBreaksPicking
 This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
 Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
 thousands. Existing analytical methods allow you to automate picking only on high-quality data with a high
 signal / noise ratio.
 
@@ -396,35 +397,33 @@
 from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 download_demo_sgy(fname=sgy_filename)
 sgy = SGY(sgy_filename)
 
-task = Task(source=sgy_filename,
+task = Task(source=sgy,
             traces_per_gather=12,
             maximum_time=100,
             gain=2)
 picker = PickerONNX()
 task = picker.process_task(task)
-
-# create an image with default parameters
-image_filename = 'default_view.png'
-export_image(task, image_filename)
+task.picks.color = (255, 0, 0)
 
 # create an image from the project preview
 image_filename = 'project_preview.png'
 export_image(task, image_filename,
              time_window=(0, 60),
              traces_window=(79.5, 90.5),
              show_processing_region=False,
              headers_total_pixels=80,
              height=500,
              width=700,
-             hide_traces_axis=True)
+             hide_traces_axis=True
+             )
 ```
 [code-block-end]:e2e-example
 
 For a better understanding of the steps taken, expand and read the next section.
 
 ### Detailed examples
 
@@ -574,15 +573,15 @@
 picker_cpu.change_settings(device='cuda', batch_size=3)
 picker_gpu.change_settings(device='cpu', batch_size=1)
 ```
 [code-block-end]:create-picker
 
 ### Pick first breaks
 
-Now, using all the created components, we can pick the first breaks and export the results.
+Now, using all the created components, we can pick the first breaks and retrieve results.
 
 [code-block-start]:pick-fb
 ```python
 from first_breaks.picking.task import Task
 from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.sgy.reader import SGY
 
@@ -591,31 +590,63 @@
 
 task = Task(source=sgy,
             traces_per_gather=24,
             maximum_time=200)
 picker = PickerONNX()
 task = picker.process_task(task)
 
-# you can see results of picking
-print(task.picks_in_samples)
-print(task.picks_in_ms)
-print(task.confidence)
-
-# you can export picks to file as plain text
-task.export_result_as_txt('result.txt')
-# or save as json file
-task.export_result_as_json('result.json')
-# or make a copy of source SGY and put picks to 236 byte
-task.export_result_as_sgy('result.segy',
-                          byte_position=236,
-                          encoding='i',
-                          picks_unit='mcs')
+# picks available from attribute
+picks = task.picks
+
+# or by method
+picks = task.get_result()
+
+# print values and confidence of picks
+print(picks.picks_in_mcs, picks.confidence)
+
+# print picking parameters
+print(picks.picking_parameters, task.picking_parameters)
 ```
 [code-block-end]:pick-fb
 
+
+### Picks
+
+The picks are stored in class `Picks`. In addition to the pick values, the class stores additional
+information (picking parameters, color, etc.). The class instance is returned as a picking result, but can
+also be created manually.
+
+[code-block-start]:picks
+```python
+from first_breaks.picking.picks import Picks
+
+
+picks_in_samples = [1, 10, 20, 30, 50, 100]
+dt_mcs = 250
+
+picks = Picks(values=picks_in_samples, unit="mcs", dt_mcs=dt_mcs)
+
+# get values
+print(picks.picks_in_samples)
+print(picks.picks_in_mcs)
+print(picks.picks_in_ms)
+
+# change color and width for visualisation
+picks.color = (255, 0, 0)
+picks.width = 5
+
+# if picks are obtained by NN you can read extra attributes
+print(picks.confidence)
+print(picks.picking_parameters)
+print(picks.created_by_nn)
+
+```
+[code-block-end]:picks
+
+
 ### Visualizations
 
 You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
 scenarios.
 
 We've added named arguments to various scenarios for demonstration purposes, but in practice you can
 use them all. See the function arguments for more visualization options.
@@ -666,27 +697,28 @@
 [code-block-end]:plot-np
 
 Plot `SGY` with custom picks:
 
 [code-block-start]:plot-sgy-custom-picks
 ```python
 import numpy as np
+from first_breaks.picking.picks import Picks
 from first_breaks.sgy.reader import SGY
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
 sgy = SGY(sgy_filename)
 picks_ms = np.random.uniform(low=0,
                              high=sgy.ns * sgy.dt_ms,
                              size=sgy.ntr)
+picks = Picks(values=picks_ms, unit="ms", dt_mcs=sgy.dt_mcs, color=(0, 100, 100))
 export_image(sgy, image_filename,
-             picks_ms=picks_ms,
-             picks_color=(0, 100, 100))
+             picks=picks)
 ```
 [code-block-end]:plot-sgy-custom-picks
 
 Plot result of picking:
 
 [code-block-start]:plot-sgy-real-picks
 ```python
```

### Comparing `first-breaks-picking-gpu-0.6.2/README.md` & `first_breaks_picking_gpu-0.7.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -159,35 +159,33 @@
 from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 download_demo_sgy(fname=sgy_filename)
 sgy = SGY(sgy_filename)
 
-task = Task(source=sgy_filename,
+task = Task(source=sgy,
             traces_per_gather=12,
             maximum_time=100,
             gain=2)
 picker = PickerONNX()
 task = picker.process_task(task)
-
-# create an image with default parameters
-image_filename = 'default_view.png'
-export_image(task, image_filename)
+task.picks.color = (255, 0, 0)
 
 # create an image from the project preview
 image_filename = 'project_preview.png'
 export_image(task, image_filename,
              time_window=(0, 60),
              traces_window=(79.5, 90.5),
              show_processing_region=False,
              headers_total_pixels=80,
              height=500,
              width=700,
-             hide_traces_axis=True)
+             hide_traces_axis=True
+             )
 ```
 [code-block-end]:e2e-example
 
 For a better understanding of the steps taken, expand and read the next section.
 
 ### Detailed examples
 
@@ -337,15 +335,15 @@
 picker_cpu.change_settings(device='cuda', batch_size=3)
 picker_gpu.change_settings(device='cpu', batch_size=1)
 ```
 [code-block-end]:create-picker
 
 ### Pick first breaks
 
-Now, using all the created components, we can pick the first breaks and export the results.
+Now, using all the created components, we can pick the first breaks and retrieve results.
 
 [code-block-start]:pick-fb
 ```python
 from first_breaks.picking.task import Task
 from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.sgy.reader import SGY
 
@@ -354,31 +352,63 @@
 
 task = Task(source=sgy,
             traces_per_gather=24,
             maximum_time=200)
 picker = PickerONNX()
 task = picker.process_task(task)
 
-# you can see results of picking
-print(task.picks_in_samples)
-print(task.picks_in_ms)
-print(task.confidence)
-
-# you can export picks to file as plain text
-task.export_result_as_txt('result.txt')
-# or save as json file
-task.export_result_as_json('result.json')
-# or make a copy of source SGY and put picks to 236 byte
-task.export_result_as_sgy('result.segy',
-                          byte_position=236,
-                          encoding='i',
-                          picks_unit='mcs')
+# picks available from attribute
+picks = task.picks
+
+# or by method
+picks = task.get_result()
+
+# print values and confidence of picks
+print(picks.picks_in_mcs, picks.confidence)
+
+# print picking parameters
+print(picks.picking_parameters, task.picking_parameters)
 ```
 [code-block-end]:pick-fb
 
+
+### Picks
+
+The picks are stored in class `Picks`. In addition to the pick values, the class stores additional
+information (picking parameters, color, etc.). The class instance is returned as a picking result, but can
+also be created manually.
+
+[code-block-start]:picks
+```python
+from first_breaks.picking.picks import Picks
+
+
+picks_in_samples = [1, 10, 20, 30, 50, 100]
+dt_mcs = 250
+
+picks = Picks(values=picks_in_samples, unit="mcs", dt_mcs=dt_mcs)
+
+# get values
+print(picks.picks_in_samples)
+print(picks.picks_in_mcs)
+print(picks.picks_in_ms)
+
+# change color and width for visualisation
+picks.color = (255, 0, 0)
+picks.width = 5
+
+# if picks are obtained by NN you can read extra attributes
+print(picks.confidence)
+print(picks.picking_parameters)
+print(picks.created_by_nn)
+
+```
+[code-block-end]:picks
+
+
 ### Visualizations
 
 You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
 scenarios.
 
 We've added named arguments to various scenarios for demonstration purposes, but in practice you can
 use them all. See the function arguments for more visualization options.
@@ -429,27 +459,28 @@
 [code-block-end]:plot-np
 
 Plot `SGY` with custom picks:
 
 [code-block-start]:plot-sgy-custom-picks
 ```python
 import numpy as np
+from first_breaks.picking.picks import Picks
 from first_breaks.sgy.reader import SGY
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
 sgy = SGY(sgy_filename)
 picks_ms = np.random.uniform(low=0,
                              high=sgy.ns * sgy.dt_ms,
                              size=sgy.ntr)
+picks = Picks(values=picks_ms, unit="ms", dt_mcs=sgy.dt_mcs, color=(0, 100, 100))
 export_image(sgy, image_filename,
-             picks_ms=picks_ms,
-             picks_color=(0, 100, 100))
+             picks=picks)
 ```
 [code-block-end]:plot-sgy-custom-picks
 
 Plot result of picking:
 
 [code-block-start]:plot-sgy-real-picks
 ```python
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/__init__.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,19 @@
         extra_potential_paths = []
         extra_potential_paths.extend(list(Path(r"C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA").glob("*")))
         extra_potential_paths.extend(list(Path(r"C:\Program Files\NVIDIA GPU Computing Toolkit").glob("*")))
         extra_potential_paths.extend(list(Path(r"C:\Program Files\NVIDIA\CUDNN").glob("*")))
         extra_potential_paths = [str(p) for p in extra_potential_paths]
         separator = ";"
     elif is_linux():
-        extra_potential_paths = ["/usr/local/cuda", "/usr/include", "/lib/x86_64-linux-gnu"]
+        extra_potential_paths = [
+            "/usr/local/cuda",
+            "/usr/include",
+            "/lib/x86_64-linux-gnu",
+        ]
         separator = ":"
     else:
         extra_potential_paths = []
         separator = ":"
 
     os.environ["PATH"] = separator.join([os.environ["PATH"]] + extra_potential_paths)
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/const.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/const.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,8 +27,10 @@
 
 MODEL_ONNX_PATH = CACHE_FOLDER / "fb.onnx"
 MODEL_ONNX_URL = "https://oml.daloroserver.com/download/seis/fb.onnx"
 MODEL_ONNX_HASH = "7e39e017b01325180e36885eccaeb17a"
 
 TIMEOUT = 60
 
-HIGH_DPI = os.getenv("HIGH_DPI", True)
+HIGH_DPI = bool(os.getenv("HIGH_DPI", True))
+
+FIRST_BYTE = int(os.getenv("FIRST_BYTE", 1))
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/data_models/dependent.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/data_models/dependent.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/data_models/independent.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/data_models/independent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import traceback
-from typing import List, Literal, Optional, Sequence, Tuple, Union
+from typing import Literal, Optional, Sequence, Tuple, Union
 from uuid import uuid4
 
 import numpy as np
 from pydantic import UUID4, BaseModel, Field, field_validator
 
 TColor = Union[Tuple[int, int, int, int], Tuple[int, int, int]]
 TNormalize = Union[Literal["trace", "gather"], float, int, np.ndarray, None]
@@ -80,18 +80,14 @@
 class FillBlack(DefaultModel):
     fill_black: Optional[Literal["left", "right"]] = Field(
         "left",
         description="Where and how to fill wiggles with black",
     )
 
 
-class PicksColor(DefaultModel):
-    picks_color: TColor = Field((255, 0, 0), description="Color for picks")
-
-
 class RegionPolyColor(DefaultModel):
     region_poly_color: TColor = Field((100, 100, 100, 50), description="Color of region below maximum time")
 
 
 class RegionContourColor(DefaultModel):
     region_contour_color: TColor = Field(
         (100, 100, 100),
@@ -106,41 +102,18 @@
     )
 
 
 class TraceBytePosition(DefaultModel):
     byte_position: int = Field(0, ge=0, lt=240, description="Byte index in trace headers")
 
 
-class PicksUnit(DefaultModel):
-    picks_unit: Literal["ms", "mcs", "sample"] = Field("mcs", description="First breaks / picks unit")
-
-
-class PicksInSamplesOptional(DefaultModel):
-    picks_in_samples: Optional[Union[np.ndarray, Sequence[Union[float]]]] = Field(  # todo: replace to "int" later
-        None, description="First breaks presented as samples"
-    )
-
-
-class ConfidenceOptional(DefaultModel):
-    confidence: Optional[Union[np.ndarray, Sequence[Union[int, float]]]] = Field(
-        None, description="Confidence of first breaks"
-    )
-
-
 class ModelHashOptional(DefaultModel):
     model_hash: Optional[str] = Field(None, description="Hash of model checkpoint")
 
 
-class PicksValue(DefaultModel):
-    picks_value: Union[np.ndarray, List[Union[int, float]], Tuple[Union[int, float], ...]] = Field(
-        ...,
-        description="Values of first breaks",
-    )
-
-
 class VSPView(DefaultModel):
     vsp_view: bool = Field(
         False, description="Set the view when the vertical axis is the trace number and the horizontal axis is time"
     )
 
 
 class InvertX(DefaultModel):
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/data_models/initialised_defaults.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/data_models/initialised_defaults.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,27 @@
     Clip,
     FillBlack,
     Gain,
     InvertX,
     InvertY,
     MaximumTime,
     Normalize,
-    PicksColor,
     RegionContourColor,
     RegionContourWidth,
     RegionPolyColor,
     TracesPerGather,
     VSPView,
 )
 
 
 class Defaults(
     Normalize,
     Gain,
     Clip,
     FillBlack,
-    PicksColor,
     RegionPolyColor,
     RegionContourColor,
     RegionContourWidth,
     XAxis,
     F1F2,
     F3F4,
     VSPView,
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/bandfilter_widget.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/bandfilter_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/byte_encode_unit_widget.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/byte_encode_unit_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     QHBoxLayout,
     QLabel,
     QSpinBox,
     QVBoxLayout,
     QWidget,
 )
 
-from first_breaks.const import HIGH_DPI
+from first_breaks.const import FIRST_BYTE, HIGH_DPI
 from first_breaks.desktop.combobox_with_mapping import QComboBoxMapping
 from first_breaks.sgy.headers import Headers
 
 if HIGH_DPI:
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
     QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
 
@@ -45,19 +45,19 @@
 class QByteEncodeUnitWidget(QWidget):
     values_changed_signal = pyqtSignal(dict)
 
     def __init__(
         self,
         byte_position: int = 0,
         encoding: str = "I",
-        first_byte: int = 0,
+        first_byte: int = FIRST_BYTE,
         picks_unit: str = "mcs",
         margins: Optional[int] = None,
         *args: Any,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         super().__init__(*args, **kwargs)
 
         self.layout = QHBoxLayout()
         if margins is not None:
             self.layout.setContentsMargins(margins, margins, margins, margins)
         self.setLayout(self.layout)
@@ -74,20 +74,24 @@
         self.byte_position_widget.setRange(self.first_byte, self.byte_position_maximum)
         self.byte_position_widget.setValue(self.byte_position_value)
         self.byte_position_widget.valueChanged.connect(self.values_changed)
 
         self.layout.addWidget(self.byte_position_label)
         self.layout.addWidget(self.byte_position_widget)
 
+        self.layout.addStretch(1)
+
         self.encoding_label = QLabel("Encoding")
         self.encoding_widget = QComboBoxMapping(ENCODING_MAPPING, current_value=self.encoding_value)  # type: ignore
 
         self.layout.addWidget(self.encoding_label)
         self.layout.addWidget(self.encoding_widget)
 
+        self.layout.addStretch(1)
+
         self.picks_unit_label = QLabel("Unit")
         self.picks_unit_widget = QComboBoxMapping(
             {0: ("Microseconds", "mcs"), 1: ("Milliseconds", "ms"), 2: ("Samples", "sample")},
             current_value=self.picks_unit_value,
         )
 
         self.layout.addWidget(self.picks_unit_label)
@@ -137,17 +141,17 @@
 
         self.layout = QVBoxLayout()
         self.setLayout(self.layout)
 
         self.widget = QByteEncodeUnitWidget(*args, **kwargs)
         self.layout.addWidget(self.widget)
 
-        self.button_box = QDialogButtonBox()
-        self.button_box.addButton("Ok", QDialogButtonBox.AcceptRole)
+        self.button_box = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel, self)
         self.button_box.accepted.connect(self.accept)
+        self.button_box.rejected.connect(self.reject)
 
         self.layout.addWidget(self.button_box)
 
     def get_values(self) -> Dict[str, Any]:
         return self.widget.get_values()
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/combobox_with_mapping.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/combobox_with_mapping.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/graph.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 import ast
 import os
 import warnings
 from pathlib import Path
-from typing import Any, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pyqtgraph as pg
-from PyQt5.QtCore import Qt, QTimer, pyqtSlot
+from PyQt5.QtCore import Qt, QTimer, pyqtSignal, pyqtSlot
 from PyQt5.QtGui import QCloseEvent, QColor, QFont, QPainterPath, QPen
 from PyQt5.QtWidgets import QApplication
 from pyqtgraph import AxisItem
 from pyqtgraph.exporters import ImageExporter
 from pyqtgraph.GraphicsScene.mouseEvents import MouseClickEvent
 
 from first_breaks.const import HIGH_DPI
 from first_breaks.data_models.independent import TColor, TNormalize
 from first_breaks.data_models.initialised_defaults import DEFAULTS
 from first_breaks.desktop.roi_manager import RoiManager
 from first_breaks.desktop.spectrum_window import SpectrumWindow
+from first_breaks.picking.picks import Picks
 from first_breaks.picking.task import Task
 from first_breaks.picking.utils import preprocess_gather
 from first_breaks.sgy.reader import SGY
 from first_breaks.utils.utils import resolve_postime2xy as postime2xy
 from first_breaks.utils.utils import resolve_xy2postime as xy2postime
 
 if HIGH_DPI:
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
     QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
 
 
 class GraphWidget(pg.PlotWidget):
+    picks_manual_edited_signal = pyqtSignal(Picks)
+    about_to_change_nn_picks_signal = pyqtSignal()
+    graph_updated_signal = pyqtSignal()
+
     def __init__(self, use_open_gl: bool = True, *args: Any, **kwargs: Any):
         super().__init__(useOpenGL=use_open_gl, *args, **kwargs)
         self.plotItem.disableAutoRange()
         self.setAntialiasing(False)
         self.plotItem.setClipToView(True)
         self.plotItem.setDownsampling(mode="peak")
         self.plotItem.ctrlMenu = None
 
         self.invert_x = DEFAULTS.invert_x
         self.invert_y = DEFAULTS.invert_y
         self.vsp_view = DEFAULTS.vsp_view
         self.sgy: Optional[SGY] = None
-        self.nn_picks_in_ms: Optional[np.ndarray] = None
-        self.nn_picks_as_item: Optional[pg.PlotCurveItem] = None
-        self.extra_picks_as_item_list: Optional[List[pg.PlotCurveItem]] = []
+        # self.picks_as_items: List[pg.PlotCurveItem] = []
+        self.picks2items: Dict[Picks, pg.PlotCurveItem] = {}
         self.processing_region_as_items: List[pg.QtWidgets.QGraphicsPathItem] = []
         self.traces_as_items: List[pg.QtWidgets.QGraphicsPathItem] = []
-        self.is_picks_modified_manually = False
         self.pos_ax_header: Optional[str] = None
 
         self.x_ax: Optional[AxisItem] = None
         self.y_ax: Optional[AxisItem] = None
         self.pos_ax: Optional[AxisItem] = None
         self.time_ax: Optional[AxisItem] = None
         self.setup_axes()
@@ -73,34 +76,33 @@
         self.getPlotItem().showAxis("bottom", False)
 
         self.x_ax = self.getPlotItem().getAxis("top")
         self.y_ax = self.getPlotItem().getAxis("left")
 
         self.pos_ax, self.time_ax = self.resolve_xy2postime(self.x_ax, self.y_ax)
 
-        self.pos_ax.tickStrings = self.replace_tick_labels
+        self.pos_ax.tickStrings = self._replace_tick_labels
 
         text_size = 12
         self.label_style = {"font-size": f"{text_size}pt"}
         font = QFont()
         font.setPointSize(text_size)
         self.pos_ax.setLabel(None, **self.label_style)
         self.time_ax.setLabel("t, ms", **self.label_style)
         self.pos_ax.setTickFont(font)
         self.time_ax.setTickFont(font)
+        self.graph_updated_signal.emit()
 
     def full_clean(self) -> None:
-        self.remove_nn_picks()
+        self.remove_picks()
         self.remove_traces()
         self.remove_processing_region()
-        self.nn_picks_as_item = None
-        self.nn_picks_in_ms = None
-        self.is_picks_modified_manually = False
         self.spectrum_roi_manager.delete_all_rois()
         self.clear()
+        self.graph_updated_signal.emit()
 
     def plotseis(
         self,
         sgy: SGY,
         clip: float = DEFAULTS.clip,
         gain: float = DEFAULTS.gain,
         normalize: TNormalize = DEFAULTS.normalize,
@@ -162,30 +164,35 @@
             self.getPlotItem().setYRange(min=0, max=y_max)
             self.getPlotItem().setXRange(min=0, max=x_max)
 
         for idx in range(num_traces):
             self._plot_trace_fast(trace=traces[:, idx], time=t, shift=idx + 1, fill_black=fill_black)
 
         self.pos_ax.showLabel()
+        self.graph_updated_signal.emit()
 
     def _plot_trace_fast(self, trace: np.ndarray, time: np.ndarray, shift: int, fill_black: Optional[str]) -> None:
         connect = np.ones(len(time), dtype=np.int32)
         connect[-1] = 0
 
+        if fill_black == "right":
+            trace = np.sign(trace) * trace**3
+            trace = np.gradient(np.gradient(trace)) * 10
+
         trace[0] = 0
         trace[-1] = 0
 
         shifted_trace = trace + shift
 
         path_x, path_y = self.resolve_postime2xy(shifted_trace, time)
         path = pg.arrayToQPath(x=path_x, y=path_y, connect=connect)
 
         item = pg.QtWidgets.QGraphicsPathItem(path)
         pen = QPen(Qt.black, 1, Qt.SolidLine, Qt.FlatCap, Qt.MiterJoin)
-        pen.setWidth(0.1)
+        pen.setCosmetic(True)  # 1 pixel width for any scale and resolution
         item.setPen(pen)
         item.setBrush(Qt.white)
         self.addItem(item)
         self.traces_as_items.append(item)
 
         if fill_black is None:
             return
@@ -198,21 +205,21 @@
             rect = QPainterPath()
             rect.addRect(x, y, w, h)
 
             patch = path.intersected(rect)
             item = pg.QtWidgets.QGraphicsPathItem(patch)
 
             pen = QPen(QColor(255, 255, 255, 0), 1, Qt.SolidLine, Qt.FlatCap, Qt.MiterJoin)
-            pen.setWidth(0.1)
+            pen.setCosmetic(True)  # 1 pixel width for any scale and resolution
             item.setPen(pen)
             item.setBrush(Qt.black)
             self.addItem(item)
             self.traces_as_items.append(item)
 
-    def replace_tick_labels(self, *args: Any, **kwargs: Any) -> List[str]:
+    def _replace_tick_labels(self, *args: Any, **kwargs: Any) -> List[str]:
         self.pos_ax.setLabel(self.pos_ax_header, **self.label_style)
         previous_labels = AxisItem.tickStrings(self.pos_ax, *args, **kwargs)
 
         if self.pos_ax_header is not None:
             labels_from_headers = []
             for v in previous_labels:
                 v = ast.literal_eval(v)
@@ -224,34 +231,25 @@
                         labels_from_headers.append("")
                 else:
                     labels_from_headers.append("")
             return labels_from_headers
         else:
             return previous_labels
 
-    def remove_nn_picks(self) -> None:
-        self.is_picks_modified_manually = False
-        if self.nn_picks_as_item:
-            self.removeItem(self.nn_picks_as_item)
-            self.nn_picks_as_item = None
-            self.nn_picks_in_ms = None
-
-    def remove_extra_picks(self) -> None:
-        for item in self.extra_picks_as_item_list:
-            self.removeItem(item)
-
     def remove_processing_region(self) -> None:
         if self.processing_region_as_items:
             for item in self.processing_region_as_items:
                 self.removeItem(item)
+        self.graph_updated_signal.emit()
 
     def remove_traces(self) -> None:
         if self.traces_as_items:
             for item in self.traces_as_items:
                 self.removeItem(item)
+        self.graph_updated_signal.emit()
 
     def plot_processing_region(
         self,
         traces_per_gather: int,
         maximum_time: float,
         region_contour_color: TColor = DEFAULTS.region_contour_color,
         region_poly_color: TColor = DEFAULTS.region_poly_color,
@@ -284,60 +282,68 @@
         poly_path = pg.arrayToQPath(poly_x, poly_y, np.ones(4, dtype=np.int32))
         poly_item = pg.QtWidgets.QGraphicsPathItem(poly_path)
         poly_item.setPen(contour_pen)
         poly_item.setBrush(poly_brush)
         self.processing_region_as_items.append(poly_item)
         self.addItem(poly_item)
 
-    def get_picks_as_item(
-        self,
-        picks_ms: Sequence[float],
-        color: TColor = DEFAULTS.picks_color,
-    ) -> pg.PlotCurveItem:
-        x, y = self.resolve_postime2xy(np.arange(self.sgy.num_traces) + 1, np.array(picks_ms))
+    def _get_picks_as_item(self, picks: Picks) -> pg.PlotCurveItem:
+        x, y = self.resolve_postime2xy(np.arange(self.sgy.num_traces) + 1, np.array(picks.picks_in_ms))
 
         line = pg.PlotCurveItem()
         line.setData(x, y)
-        pen = pg.mkPen(color=color, width=3)
+        pen = pg.mkPen(color=picks.color, width=picks.width)
         line.setPen(pen)
 
         return line
 
-    def plot_nn_picks(self, picks_ms: Sequence[float], color: TColor = DEFAULTS.picks_color) -> None:
-        self.remove_nn_picks()
-        self.is_picks_modified_manually = False
+    def plot_picks(self, picks: Picks) -> None:
+        picks_item = self._get_picks_as_item(picks)
+        self.addItem(picks_item)
+        self.picks2items[picks] = picks_item
+        self.graph_updated_signal.emit()
+
+    def remove_picks(self) -> None:
+        for picks in list(self.picks2items.keys()):
+            self.removeItem(self.picks2items[picks])
+            del self.picks2items[picks]
+        self.graph_updated_signal.emit()
 
-        self.nn_picks_in_ms = np.array(picks_ms)
-        self.nn_picks_as_item = self.get_picks_as_item(self.nn_picks_in_ms, color)
-
-        self.addItem(self.nn_picks_as_item)
+    def mouse_clicked(self, ev: Tuple[MouseClickEvent]) -> None:
+        ev = ev[0]
+        active_picks_list = [k for k in self.picks2items.keys() if k.active]
 
-    def plot_extra_picks(self, picks_ms: Sequence[float], color: TColor = DEFAULTS.picks_color) -> None:
-        picks = self.get_picks_as_item(picks_ms, color)
+        if active_picks_list:
+            active_picks = active_picks_list[0]
+        else:
+            return
 
-        self.addItem(picks)
-        self.extra_picks_as_item_list.append(picks)
+        if active_picks.created_by_nn and not active_picks.modified_manually:
+            self.about_to_change_nn_picks_signal.emit()
+            self.mouse_clicked((ev,))
+            return
 
-    def mouse_clicked(self, ev: Tuple[MouseClickEvent]) -> None:
-        ev = ev[0]
-        if self.nn_picks_as_item is not None and ev.button() == 1:
+        if active_picks and ev.button() == 1:
             mouse_xy = self.getPlotItem().vb.mapSceneToView(ev.scenePos())
             mouse_pos, mouse_time = self.resolve_xy2postime(mouse_xy.x(), mouse_xy.y())
 
-            picks_x, picks_y = self.nn_picks_as_item.getData()
+            picks_x, picks_y = self.picks2items[active_picks].getData()
             picks_pos, picks_time = self.resolve_xy2postime(picks_x, picks_y)
 
             closest = np.argmin(np.abs(picks_pos - mouse_pos))
             mouse_time = np.clip(mouse_time, 0, self.sgy.max_time_ms)
             picks_time[closest] = mouse_time
 
             picks_x, picks_y = self.resolve_postime2xy(picks_pos, picks_time)
-            self.nn_picks_as_item.setData(picks_x, picks_y)
-            self.nn_picks_in_ms = picks_time
-            self.is_picks_modified_manually = True
+
+            self.picks2items[active_picks].setData(picks_x, picks_y)
+            active_picks.from_ms(picks_time)
+
+            self.picks_manual_edited_signal.emit(active_picks)
+            self.graph_updated_signal.emit()
 
     def closeEvent(self, e: QCloseEvent) -> None:
         self.spectrum_window.close()
         e.accept()
 
 
 class HighMemoryConsumption(Exception):
@@ -404,18 +410,17 @@
         # content parameters
         clip: float = DEFAULTS.clip,
         gain: float = DEFAULTS.gain,
         normalize: TNormalize = DEFAULTS.normalize,
         fill_black: Optional[str] = DEFAULTS.fill_black,
         time_window: Optional[Tuple[float, float]] = None,
         traces_window: Optional[Tuple[float, float]] = None,
-        picks_ms: Optional[Sequence[float]] = None,
+        picks: Optional[Picks] = None,
         task: Optional[Task] = None,
         show_processing_region: bool = True,
-        picks_color: TColor = DEFAULTS.picks_color,
         contour_color: TColor = DEFAULTS.region_contour_color,
         poly_color: TColor = DEFAULTS.region_poly_color,
         contour_width: float = DEFAULTS.region_contour_width,
         x_axis: Optional[str] = DEFAULTS.x_axis,
         # rendering parameters
         height: int = 500,
         width: Optional[int] = None,
@@ -425,16 +430,16 @@
         time_spacing: Optional[int] = None,
         traces_spacing: Optional[int] = None,
         hide_traces_axis: bool = False,
     ) -> None:
         if args:
             raise need_kwargs_exception
 
-        if picks_ms is not None and task is not None:
-            raise ValueError("'picks_ms' and 'task' are mutually exclusive. Use only one of them or none")
+        if picks is not None and task is not None:
+            raise ValueError("'picks' and 'task' are mutually exclusive. Use only one of them or none")
 
         if width is None:
             if traces_window is None:
                 num_traces = sgy.num_traces
                 width = int(width_per_trace * num_traces) + headers_total_pixels
             else:
                 width = int(width_per_trace * (traces_window[1] - traces_window[0])) + headers_total_pixels
@@ -443,22 +448,17 @@
 
         self.x_ax_header = x_axis
 
         self.clear()
         self.plotseis(sgy, normalize=normalize, clip=clip, gain=gain, fill_black=fill_black, refresh_view=True)
 
         if task:
-            picks_to_plot = task.picks_in_ms  # type: ignore
-        elif picks_ms is not None:
-            picks_to_plot = picks_ms  # type: ignore
-        else:
-            picks_to_plot = None  # type: ignore
-
-        if picks_to_plot is not None:
-            self.plot_nn_picks(picks_to_plot, color=picks_color)
+            self.plot_picks(task.picks)
+        elif picks is not None:
+            self.plot_picks(picks)
 
         if task is not None and show_processing_region:
             self.plot_processing_region(
                 maximum_time=task.maximum_time,
                 traces_per_gather=task.traces_per_gather,
                 region_contour_color=contour_color,
                 region_poly_color=poly_color,
@@ -517,17 +517,16 @@
     dt_mcs: float = 1e3,
     clip: float = DEFAULTS.clip,
     gain: float = DEFAULTS.gain,
     normalize: TNormalize = DEFAULTS.normalize,
     fill_black: Optional[str] = DEFAULTS.fill_black,
     time_window: Optional[Tuple[float, float]] = None,
     traces_window: Optional[Tuple[float, float]] = None,
-    picks_ms: Optional[Sequence[float]] = None,
+    picks: Optional[Picks] = None,
     show_processing_region: bool = True,
-    picks_color: TColor = DEFAULTS.picks_color,
     contour_color: TColor = DEFAULTS.region_contour_color,
     poly_color: TColor = DEFAULTS.region_poly_color,
     contour_width: float = DEFAULTS.region_contour_width,
     x_axis: Optional[str] = DEFAULTS.x_axis,
     # rendering parameters
     height: int = 500,
     width: Optional[int] = None,
@@ -567,18 +566,17 @@
         image_filename=image_filename,
         clip=clip,
         gain=gain,
         normalize=normalize,
         fill_black=fill_black,
         time_window=time_window,
         traces_window=traces_window,
-        picks_ms=picks_ms,
+        picks=picks,
         task=task,
         show_processing_region=show_processing_region,
-        picks_color=picks_color,
         contour_color=contour_color,
         poly_color=poly_color,
         contour_width=contour_width,
         x_axis=x_axis,
         height=height,
         width=width,
         width_per_trace=width_per_trace,
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/main_gui.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/main_gui.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 import warnings
 from pathlib import Path
 from typing import Any, Dict, Optional, Tuple, Union
 
-from pydantic import UUID4
-from PyQt5.QtCore import QSize, Qt, QThreadPool
+from PyQt5.QtCore import QSize, Qt, QThreadPool, pyqtSignal
 from PyQt5.QtGui import QCloseEvent
 from PyQt5.QtWidgets import (
     QAction,
     QApplication,
     QFileDialog,
     QHBoxLayout,
     QLabel,
@@ -17,35 +16,28 @@
     QSizePolicy,
     QStyle,
     QToolBar,
     QWidget,
 )
 
 from first_breaks.const import DEMO_SGY_PATH, HIGH_DPI, MODEL_ONNX_HASH, MODEL_ONNX_PATH
-from first_breaks.data_models.dependent import TraceHeaderParams
 from first_breaks.data_models.independent import ExceptionOptional
-from first_breaks.desktop.byte_encode_unit_widget import QDialogByteEncodeUnit
 from first_breaks.desktop.graph import GraphWidget
+from first_breaks.desktop.last_folder_manager import last_folder_manager
 from first_breaks.desktop.nn_manager import NNManager
+from first_breaks.desktop.picks_manager_widget import PicksManager
 from first_breaks.desktop.settings_processing_widget import (
     PickingSettings,
-    PicksFromFileSettings,
     PlotseisSettings,
     SettingsProcessingWidget,
 )
 from first_breaks.desktop.utils import MessageBox, set_geometry
 from first_breaks.picking.task import Task
 from first_breaks.sgy.reader import SGY
-from first_breaks.utils.utils import (
-    UnitsConverter,
-    calc_hash,
-    download_demo_sgy,
-    download_model_onnx,
-    multiply_iterable_by,
-)
+from first_breaks.utils.utils import calc_hash, download_demo_sgy, download_model_onnx
 
 warnings.filterwarnings("ignore")
 
 if HIGH_DPI:
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
     QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
 
@@ -68,15 +60,23 @@
     model_loaded: bool = False
 
     def is_ready(self) -> bool:
         return (self.sgy_selected == self.model_loaded) is True
 
 
 class MainWindow(QMainWindow):
-    def __init__(self, use_open_gl: bool = True):  # type: ignore
+    TOOLBAR_LOAD_MODEL = "Load model"
+    TOOLDBAR_OPEN_SGY = "Open SGY-file"
+    TOOLBAR_SETTINGS_AND_PROCESSINGS = "Settings and Processing"
+    TOOLBAR_SHOW_GRID = "Show processing grid"
+    TOOLBAR_PICKS_MANAGER = "Picks manager"
+
+    processing_finished_signal = pyqtSignal()
+
+    def __init__(self, use_open_gl: bool = True, show: bool = True):  # type: ignore
         super(MainWindow, self).__init__()
 
         if getattr(sys, "frozen", False):
             self.main_folder = Path(sys._MEIPASS)  # type: ignore
         else:
             self.main_folder = Path(__file__).parent
 
@@ -89,54 +89,54 @@
         self.toolbar = QToolBar()
         self.toolbar.setIconSize(QSize(30, 30))
         self.addToolBar(self.toolbar)
 
         # buttons on toolbar
         icon_load_nn = self.style().standardIcon(QStyle.SP_ComputerIcon)
         # icon_load_nn = QIcon(str(self.main_folder / "icons" / "nn.png"))
-        self.button_load_nn = QAction(icon_load_nn, "Load model", self)
+        self.button_load_nn = QAction(icon_load_nn, self.TOOLBAR_LOAD_MODEL, self)
         self.button_load_nn.triggered.connect(self.load_nn)
         self.button_load_nn.setEnabled(True)
         self.toolbar.addAction(self.button_load_nn)
 
         icon_get_filename = self.style().standardIcon(QStyle.SP_DirIcon)
         # icon_get_filename = QIcon(str(self.main_folder / "icons" / "sgy.png"))
-        self.button_get_filename = QAction(icon_get_filename, "Open SGY-file", self)
+        self.button_get_filename = QAction(icon_get_filename, self.TOOLDBAR_OPEN_SGY, self)
         self.button_get_filename.triggered.connect(self.get_filename)
         self.button_get_filename.setEnabled(True)
         self.toolbar.addAction(self.button_get_filename)
 
         self.toolbar.addSeparator()
 
         icon_visual_settings = self.style().standardIcon(QStyle.SP_FileDialogContentsView)
-        self.button_settings_processing = QAction(icon_visual_settings, "Settings and Processing", self)
+        self.button_settings_processing = QAction(icon_visual_settings, self.TOOLBAR_SETTINGS_AND_PROCESSINGS, self)
         self.button_settings_processing.triggered.connect(self.show_settings_processing_window)
         self.button_settings_processing.setEnabled(False)
         self.toolbar.addAction(self.button_settings_processing)
 
         self.need_processing_region = True
         icon_processing_show = self.style().standardIcon(QStyle.SP_FileDialogListView)
         # icon_export = QIcon(str(self.main_folder / "icons" / "export.png"))
-        self.button_processing_show = QAction(icon_processing_show, "Show processing grid", self)
+        self.button_processing_show = QAction(icon_processing_show, self.TOOLBAR_SHOW_GRID, self)
         self.button_processing_show.triggered.connect(self.processing_region_changed)
         self.button_processing_show.setChecked(self.need_processing_region)
         self.button_processing_show.setEnabled(True)
         self.button_processing_show.setCheckable(True)
         if self.need_processing_region:
             self.button_processing_show.toggle()
         self.toolbar.addAction(self.button_processing_show)
 
         self.toolbar.addSeparator()
 
-        icon_export = self.style().standardIcon(QStyle.SP_DialogSaveButton)
+        icon_picks_manager = self.style().standardIcon(QStyle.SP_FileDialogDetailedView)
         # icon_export = QIcon(str(self.main_folder / "icons" / "export.png"))
-        self.button_export = QAction(icon_export, "Export picks to file", self)
-        self.button_export.triggered.connect(self.export)
-        self.button_export.setEnabled(False)
-        self.toolbar.addAction(self.button_export)
+        self.button_picks_manager = QAction(icon_picks_manager, self.TOOLBAR_PICKS_MANAGER, self)
+        self.button_picks_manager.triggered.connect(self.show_picks_manager)
+        self.button_picks_manager.setEnabled(False)
+        self.toolbar.addAction(self.button_picks_manager)
 
         spacer = QWidget(self)
         spacer.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         self.toolbar.addWidget(spacer)
 
         self.status = self.statusBar()
         self.status_progress = QProgressBar()
@@ -156,92 +156,77 @@
         # graph widget
         self.graph = GraphWidget(use_open_gl=use_open_gl, background="w")
         self.graph.hide()
         self.setCentralWidget(self.graph)
 
         # visual settings widget
         self.plotseis_settings = PlotseisSettings()
-        first_byte = 1
-        self.picks_from_file_settings = PicksFromFileSettings(byte_position=first_byte)
         self.settings_processing_widget = SettingsProcessingWidget(
             hide_on_close=True,
-            first_byte=first_byte,
-            **{**self.plotseis_settings.model_dump(), **self.picks_from_file_settings.model_dump()},
+            **self.plotseis_settings.model_dump(),
         )
         self.settings_processing_widget.hide()
         self.settings_processing_widget.export_plotseis_settings_signal.connect(self.update_plotseis_settings)
         self.settings_processing_widget.export_picking_settings_signal.connect(self.pick_fb)
-        self.settings_processing_widget.export_picks_from_file_settings_signal.connect(
-            self.update_picks_from_file_settings
-        )
-        self.settings_processing_widget.toggle_picks_from_file_signal.connect(self.toggle_picks_from_file)
 
         # nn manager
         self.nn_manager = NNManager(
             status_progress=self.status_progress,
             status_message=self.status_message,
             threadpool=self.threadpool,
             interrupt_on=self.settings_processing_widget.interrupt_signal,
         )
         self.nn_manager.picking_finished_signal.connect(self.on_picking_finished)
         self.nn_manager.picking_not_started_error_signal.connect(self.on_picking_not_started_error)
 
+        # picks manager
+        self.picks_manager = PicksManager()
+        self.picks_manager.picks_updated_signal.connect(self.update_plot)
+        self.picks_manager.hide()
+
+        self.graph.picks_manual_edited_signal.connect(self.picks_manager.update_picks_from_external)
+        self.graph.about_to_change_nn_picks_signal.connect(self.picks_manager.duplicate_active_created_by_nn_picks)
+
         self.is_toggled_picks_from_file = False
         # placeholders
         self.sgy: Optional[SGY] = None
         self.fn_sgy: Optional[Union[str, Path]] = None
         self.ready_to_process = ReadyToProcess()
         self.last_task: Optional[Task] = None
         self.settings: Optional[Dict[str, Any]] = None
         self.last_folder: Optional[Union[str, Path]] = None
         self.picks_from_file_in_ms: Optional[Tuple[Union[int, float], ...]] = None
         self.picker_hash = MODEL_ONNX_HASH
-        self.last_picks_id: Optional[UUID4] = None
 
-        self.show()
-
-    def get_last_folder(self) -> str:
-        if self.last_folder is None:
-            return str(Path.home())
-        else:
-            if Path(self.last_folder).exists():
-                return str(Path(self.last_folder).resolve())
-            else:
-                return str(Path.home())
-
-    def set_last_folder_based_on_file(self, file: Union[str, Path]) -> None:
-        file = Path(file)
-        if file.exists():
-            self.last_folder = str(file.parent)
-        else:
-            self.last_folder = None
+        if show:
+            self.show()
 
     def pick_fb(self, settings: PickingSettings) -> None:
         self.button_get_filename.setEnabled(False)
         self.nn_manager.pick_fb(self.sgy, settings)
 
     def on_picking_not_started_error(self, exc: ExceptionOptional) -> None:
         self.settings_processing_widget.set_selection_mode()
         window_error = MessageBox(
             self,
             title=exc.exception.__class__.__name__,
             message=str(exc),
             detailed_message=exc.get_formatted_traceback(),
         )
         window_error.exec_()
+        self.processing_finished_signal.emit()
 
     def on_picking_finished(self, result: Task) -> None:
         self.settings_processing_widget.set_selection_mode()
         self.last_task = result
 
         if result.success:
-            self.last_picks_id = self.last_task.picks_id
-            self.graph.plot_nn_picks(self.last_task.picks_in_ms)
+            self.picks_manager.add_nn_picks(result.picks)
+            self.update_plot(refresh_view=False)
             self.run_processing_region()
-            self.button_export.setEnabled(True)
         else:
             if isinstance(result.exception, InterruptedError):
                 window_error = MessageBox(
                     self,
                     title="Interruption",
                     message="The picking process has been interrupted. Intermediate results will not be saved",
                 )
@@ -250,81 +235,49 @@
                     self,
                     title=result.exception.__class__.__name__,
                     message=result.error_message,
                     detailed_message=result.get_formatted_traceback(),
                 )
             window_error.exec_()
 
+        self.processing_finished_signal.emit()
         self.button_get_filename.setEnabled(True)
 
     def processing_region_changed(self, toggle: bool) -> None:
         self.need_processing_region = toggle
         self.run_processing_region()
 
     def run_processing_region(self) -> None:
         if self.need_processing_region:
             self.show_processing_region()
         else:
             self.hide_processing_region()
 
     def show_processing_region(self) -> None:
-        if self.last_task and self.last_task.success:
-            self.graph.plot_processing_region(self.last_task.traces_per_gather, self.last_task.maximum_time)
+        for picks in self.picks_manager.picks_mapping.values():
+            if picks.created_by_nn and picks.active:
+                tps, max_time = picks.picking_parameters.traces_per_gather, picks.picking_parameters.maximum_time
+                self.graph.plot_processing_region(tps, max_time)
+                break
 
     def hide_processing_region(self) -> None:
         if self.last_task and self.last_task.success:
             self.graph.remove_processing_region()
 
-    def show_nn_picks(self) -> None:
-        if self.last_task and self.last_task.success:
-            if self.last_task.picks_id != self.last_picks_id:
-                self.graph.plot_nn_picks(self.last_task.picks_in_ms)
-            else:
-                # todo: implement later in a better way
-                # this case mean that we don't rerun picking, so we replicate settings
-                is_picks_modified_manually = self.graph.is_picks_modified_manually
-                self.graph.plot_nn_picks(self.graph.nn_picks_in_ms)
-                self.graph.is_picks_modified_manually = is_picks_modified_manually
-
-    def read_picks_from_file(self) -> None:
-        picks = self.sgy.read_custom_trace_header(
-            **TraceHeaderParams(**self.picks_from_file_settings.model_dump()).model_dump(),
-        )
-        units_converter = UnitsConverter(sgy_mcs=self.sgy.dt_mcs)
-        if self.picks_from_file_settings.picks_unit == "sample":
-            self.picks_from_file_in_ms = units_converter.index2ms(picks)  # type: ignore
-        elif self.picks_from_file_settings.picks_unit == "mcs":
-            self.picks_from_file_in_ms = units_converter.mcs2ms(picks)  # type: ignore
-        else:
-            self.picks_from_file_in_ms = picks
-
-    def update_picks_from_file_settings(self, new_settings: PicksFromFileSettings) -> None:
-        print(new_settings)
-        self.picks_from_file_settings = new_settings
-
-    def toggle_picks_from_file(self, toggled: bool) -> None:
-        self.is_toggled_picks_from_file = toggled
-        self.show_picks_from_file()
-
-    def show_picks_from_file(self) -> None:
-        if self.is_toggled_picks_from_file:
-            self.read_picks_from_file()
-            self.graph.plot_extra_picks(picks_ms=self.picks_from_file_in_ms, color=(0, 0, 255))
-        else:
-            self.graph.remove_extra_picks()
-
     def update_plotseis_settings(self, new_settings: PlotseisSettings) -> None:
         self.plotseis_settings = new_settings
         self.update_plot(False)
 
     def update_plot(self, refresh_view: bool = False) -> None:
         self.graph.plotseis(self.sgy, refresh_view=refresh_view, **self.plotseis_settings.model_dump())
         self.show_processing_region()
-        self.show_nn_picks()
-        self.show_picks_from_file()
+
+        self.graph.remove_picks()
+        for picks in self.picks_manager.get_selected_picks():
+            self.graph.plot_picks(picks)
 
     def show_settings_processing_window(self) -> None:
         self.settings_processing_widget.show()
         self.settings_processing_widget.focusWidget()
 
     def unlock_pickng_if_ready(self) -> None:
         if self.ready_to_process.is_ready():
@@ -333,124 +286,105 @@
             self.settings_processing_widget.enable_picking()
             self.status_message.setText("Click on picking to start processing")
 
     def load_nn(self, filename: Optional[Union[str, Path]] = None) -> None:
         if not filename:
             options = QFileDialog.Options()
             filename, _ = QFileDialog.getOpenFileName(
-                self, "Select file with NN weights", directory=self.get_last_folder(), options=options
+                self, "Select file with NN weights", directory=last_folder_manager.get_last_folder(), options=options
             )
 
         if filename:
             if FileState.get_file_state(filename, self.picker_hash) == FileState.valid_file:
                 self.nn_manager.init_net(weights=filename)
                 self.button_load_nn.setEnabled(False)
                 self.ready_to_process.model_loaded = True
 
                 status_message = "Model loaded successfully"
                 if not self.ready_to_process.sgy_selected:
                     status_message += ". Open SGY file to start picking"
                 self.status_message.setText(status_message)
-
+                self.settings_processing_widget.enable_picking()
                 self.unlock_pickng_if_ready()
-                self.set_last_folder_based_on_file(filename)
+                last_folder_manager.set_last_folder(filename)
             else:
                 window_err = MessageBox(
                     self,
                     title="Model loading error",
                     message="The file cannot be used as model weights. "
                     "Download the file according to the manual and select it.",
                 )
                 window_err.exec_()
 
     def get_filename(self, filename: Optional[Union[str, Path]] = None) -> None:
         if not filename:
             filename, _ = QFileDialog.getOpenFileName(
                 self,
                 "Open SEGY-file",
-                directory=self.get_last_folder(),
+                directory=last_folder_manager.get_last_folder(),
                 filter="SEGY-file (*.segy *.sgy);; Any file (*)",
             )
         if filename:
             try:
                 self.fn_sgy = Path(filename)
                 self.last_task = None
                 self.sgy = SGY(self.fn_sgy)
                 self.picks_from_file_in_ms = None
+                self.picks_manager.reset_manager()
+                self.picks_manager.set_sgy(sgy=self.sgy)
 
                 self.graph.full_clean()
                 self.update_plot(refresh_view=True)
                 self.graph.show()
-                self.button_export.setEnabled(False)
+                self.button_picks_manager.setEnabled(True)
                 self.button_settings_processing.setEnabled(True)
                 self.settings_processing_widget.enable_only_visualizations_settings()
 
                 self.button_get_filename.setEnabled(True)
                 self.ready_to_process.sgy_selected = True
 
                 if not self.ready_to_process.model_loaded:
                     status_message = "Load model to start picking"
                     self.status_message.setText(status_message)
 
                 self.unlock_pickng_if_ready()
-                self.set_last_folder_based_on_file(filename)
+                last_folder_manager.set_last_folder(filename)
 
             except Exception as e:
                 window_err = MessageBox(self, title=e.__class__.__name__, message=str(e))
                 window_err.exec_()
 
-    def export(self) -> None:
-        formats = ["SEGY-file (*.segy *.sgy)", "JSON-file (*.json)", "TXT-file (*.txt)"]
-        formats = ";; ".join(formats)
-        filename, _ = QFileDialog.getSaveFileName(self, "Save result", directory=self.get_last_folder(), filter=formats)
-
-        if filename:
-            filename = Path(filename).resolve()
-            if self.last_task is not None and self.last_task.success:
-                filename.parent.mkdir(parents=True, exist_ok=True)
-
-                picks_in_samples_prev = self.last_task.picks_in_samples
-                if self.graph.is_picks_modified_manually:
-                    self.last_task.picks_in_samples = multiply_iterable_by(
-                        self.graph.nn_picks_in_ms, 1 / self.sgy.dt_ms, float
-                    )
-                if filename.suffix.lower() in (".sgy", ".segy"):
-                    save_params = QDialogByteEncodeUnit(first_byte=1, byte_position=237, encoding="I", picks_unit="mcs")
-                    save_params.setWindowTitle("How to save first breaks")
-                    save_params.show()
-                    save_params.exec_()
-                    export_params = save_params.get_values()
-                    self.last_task.export_result_as_sgy(str(filename), **export_params)  # type: ignore
-                elif filename.suffix.lower() == ".txt":
-                    self.last_task.export_result_as_txt(str(filename))
-                elif filename.suffix.lower() == ".json":
-                    self.last_task.export_result_as_json(str(filename))
-                else:
-                    message_er = "The file can only be saved in '.sgy', '.segy', '.txt, or '.json' formats"
-                    window_err = MessageBox(self, title="Wrong filename", message=message_er)
-                    window_err.exec_()
-                if self.graph.is_picks_modified_manually:
-                    self.last_task.picks_in_samples = picks_in_samples_prev
+    def show_picks_manager(self) -> None:
+        if self.picks_manager.isMinimized():
+            self.picks_manager.showNormal()
+        else:
+            self.picks_manager.show()
+        self.picks_manager.raise_()
+        self.picks_manager.activateWindow()
 
     def closeEvent(self, e: QCloseEvent) -> None:
         self.graph.spectrum_window.close()
+        self.picks_manager.close()
         e.accept()
 
 
+def create_app() -> Tuple[QApplication, MainWindow]:
+    return QApplication([]), MainWindow()
+
+
 def run_app() -> None:
-    app = QApplication([])
-    _ = MainWindow()
+    app, _ = create_app()
     app.exec_()
 
 
 def fetch_data_and_run_app() -> None:
     download_model_onnx(MODEL_ONNX_PATH)
     download_demo_sgy(DEMO_SGY_PATH)
-    app = QApplication([])
-    window = MainWindow()
+    app, window = create_app()
     window.load_nn(MODEL_ONNX_PATH)
     window.get_filename(DEMO_SGY_PATH)
     app.exec_()
 
 
 if __name__ == "__main__":
+    # run_app()
     fetch_data_and_run_app()
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/nn_manager.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/nn_manager.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/radioset_widget.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/radioset_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/roi_manager.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/roi_manager.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/settings_processing_widget.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/settings_processing_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,33 +14,31 @@
     QLineEdit,
     QPushButton,
     QSpinBox,
     QWidget,
 )
 
 from first_breaks.const import HIGH_DPI
-from first_breaks.data_models.dependent import Device, TraceHeaderParams, XAxis
+from first_breaks.data_models.dependent import Device, XAxis
 from first_breaks.data_models.independent import (
     F1F2,
     F3F4,
     Clip,
     FillBlack,
     Gain,
     InvertX,
     InvertY,
     MaximumTime,
     Normalize,
-    PicksUnit,
     TNormalize,
     TracesPerGather,
     VSPView,
 )
 from first_breaks.data_models.initialised_defaults import DEFAULTS
 from first_breaks.desktop.bandfilter_widget import QBandFilterWidget
-from first_breaks.desktop.byte_encode_unit_widget import QByteEncodeUnitWidget
 from first_breaks.desktop.combobox_with_mapping import QComboBoxMapping
 from first_breaks.desktop.radioset_widget import QRadioSetWidget
 from first_breaks.desktop.utils import QHSeparationLine, set_geometry
 from first_breaks.utils.cuda import ONNX_CUDA_AVAILABLE, get_recommended_device
 
 if HIGH_DPI:
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
@@ -80,18 +78,14 @@
     pass
 
 
 class PickingSettings(Gain, Clip, Normalize, F1F2, F3F4, MaximumTime, TracesPerGather, Device):
     pass
 
 
-class PicksFromFileSettings(TraceHeaderParams, PicksUnit):
-    pass
-
-
 def get_value(qline: QLineEdit, minimum: Optional[float] = None, default: Optional[float] = 1.0) -> float:
     value = qline.text()
     qline.setPlaceholderText(str(default))
     if value.lstrip("-").lstrip("+").lstrip(".").lstrip(","):
         value = float(value)
         if minimum:
             value = max(minimum, value)
@@ -288,64 +282,21 @@
             sub_layout.setContentsMargins(0, 0, 0, 0)
             self.layout.addLayout(sub_layout)
 
     def dict(self) -> Dict[str, Any]:
         return {k: w.isChecked() for _, w, _, k in self.widgets}
 
 
-class PicksFromFileLine(QWidget, _Extras):
-    toggle_picks_from_file_signal = pyqtSignal(bool)
-    export_picks_from_file_settings_signal = pyqtSignal(PicksFromFileSettings)
-
-    def __init__(self, byte_position: int = 1, first_byte: int = 1, encoding: str = "I", picks_unit: str = "mcs"):
-
-        super().__init__()
-        self.picks_from_file_toggle = QCheckBox()
-        self.picks_from_file_toggle.setCheckState(False)
-        # self.picks_from_file_toggle.stateChanged.connect(self.export_picks_from_file_settings)
-        self.picks_from_file_toggle.clicked.connect(self.export_picks_from_file_settings)
-        self.picks_from_file_widget = QByteEncodeUnitWidget(
-            byte_position=byte_position, first_byte=first_byte, encoding=encoding, picks_unit=picks_unit, margins=0
-        )
-        self.picks_from_file_widget.values_changed_signal.connect(self.update_picks_from_file_settings)
-        self.picks_from_file_settings = self.picks_from_file_widget.get_values()
-
-        sub_layout = QHBoxLayout()
-        sub_layout.addWidget(self.picks_from_file_toggle)
-        sub_layout.addWidget(self.picks_from_file_widget)
-        self.setLayout(sub_layout)
-
-    def update_picks_from_file_settings(self, params: Dict[str, Any]) -> None:
-        self.picks_from_file_settings = params
-
-    def export_picks_from_file_settings(self, checked: bool) -> None:
-        if checked:
-            self.picks_from_file_widget.setEnabled(False)
-            self.export_picks_from_file_settings_signal.emit(PicksFromFileSettings(**self.picks_from_file_settings))
-            self.toggle_picks_from_file_signal.emit(True)
-        else:
-            self.toggle_picks_from_file_signal.emit(False)
-            self.picks_from_file_widget.setEnabled(True)
-
-    def enable_fields(self) -> None:
-        self.picks_from_file_toggle.setEnabled(True)
-        if not self.picks_from_file_toggle.isChecked():
-            self.picks_from_file_widget.setEnabled(True)
-
-    def disable_fields(self) -> None:
-        self.picks_from_file_toggle.setEnabled(False)
-        self.picks_from_file_widget.setEnabled(False)
-
-
 class TracesPerGatherLine(QSpinBox, _Extras):
     changed_signal = pyqtSignal()
 
     def __init__(self, traces_per_gather: int = DEFAULTS.traces_per_gather, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.setMinimum(1)
+        self.setMaximum(1_000_000)
         self.setValue(traces_per_gather)
 
     def dict(self) -> Dict[str, Any]:
         return {"traces_per_gather": int(self.text())}
 
 
 class MaximumTimeLine(QLineEdit, _Extras):
@@ -359,47 +310,56 @@
         self.setText(str(maximum_time))
 
     def dict(self) -> Dict[str, Any]:
         return {"maximum_time": float(self.text())}
 
 
 class DeviceLine(QComboBoxMapping, _Extras):
+    CUDA_INDEX = 0
+    CPU_INEDX = 1
+
     def __init__(self, device: str = DEFAULTS.device):
         if device == "cuda" and ONNX_CUDA_AVAILABLE:
             current_value = device
         else:
             current_value = "cpu"
-        super().__init__({0: ["GPU/CUDA", "cuda"], 1: ["CPU", "cpu"]}, current_value=current_value)
+
+        if not ONNX_CUDA_AVAILABLE:
+            cuda_postfix = "(CUDA drivers or CUDA compatible app are not installed)"
+        else:
+            cuda_postfix = ""
+
+        super().__init__(
+            {self.CUDA_INDEX: [f"GPU/CUDA {cuda_postfix}", "cuda"], self.CPU_INEDX: ["CPU", "cpu"]},
+            current_value=current_value,
+        )
+
         if not ONNX_CUDA_AVAILABLE:
-            self.setEnabled(False)
+            item = self.model().item(self.CUDA_INDEX)
+            if not ONNX_CUDA_AVAILABLE:
+                item.setFlags(item.flags() & ~Qt.ItemIsEnabled)
 
     def dict(self) -> Dict[str, Any]:
         return {"device": self.value()}
 
 
 class SettingsProcessingWidget(QDialog):
     export_plotseis_settings_signal = pyqtSignal(PlotseisSettings)
     export_picking_settings_signal = pyqtSignal(PickingSettings)
-    export_picks_from_file_settings_signal = pyqtSignal(PicksFromFileSettings)
-    toggle_picks_from_file_signal = pyqtSignal(bool)
     interrupt_signal = pyqtSignal()
 
     def __init__(
         self,
         gain: float = 1.0,
         clip: float = 1.0,
         normalize: Optional[str] = "trace",
         f1_f2: Optional[Tuple[float, float]] = None,
         f3_f4: Optional[Tuple[float, float]] = None,
         fill_black: Optional[str] = "left",
         x_axis: Optional[str] = None,
-        byte_position: int = 1,
-        first_byte: int = 1,
-        encoding: str = "I",
-        picks_unit: str = "mcs",
         hide_on_close: bool = False,
         vsp_view: bool = False,
         invert_x: bool = False,
         invert_y: bool = True,
         traces_per_gather: int = 12,
         maximum_time: float = 0.0,
         device: str = get_recommended_device(),
@@ -413,68 +373,58 @@
 
         self.layout = QGridLayout()
         self.setLayout(self.layout)
 
         self._separators = [
             [QHSeparationLine("Processing"), 0],
             [QHSeparationLine("View"), 5],
-            [QHSeparationLine("External"), 9],
-            [QHSeparationLine("NN picking"), 11],
+            [QHSeparationLine("NN picking"), 10],
         ]
 
         for sep, line in self._separators:
             self.layout.addWidget(sep, line, 0, 1, 2)
 
         self._inputs = [
             ("Gain", GainLine(gain=gain), 1, True),
             ("Clip", ClipLine(clip=clip), 2, True),
             ("Normalization", NormalizationLine(normalize=normalize), 3, True),
             ("Band filter", BandfilterLine(f1_f2=f1_f2, f3_f4=f3_f4), 4, True),
             ("Filling wiggles with color", WigglesLine(fill_black=fill_black), 6, True),
             ("X Axis", XAxisLine(x_axis=x_axis), 7, True),
             ("Orientation", OrientationLine(vsp_view=vsp_view, invert_x=invert_x, invert_y=invert_y), 8, True),
-            ("Traces per gather", TracesPerGatherLine(traces_per_gather=traces_per_gather), 12, False),
-            ("Maximum time", MaximumTimeLine(maximum_time=maximum_time), 13, False),
-            ("Runtime", DeviceLine(device=device), 14, False),
+            ("Traces per gather", TracesPerGatherLine(traces_per_gather=traces_per_gather), 11, False),
+            ("Maximum time", MaximumTimeLine(maximum_time=maximum_time), 12, False),
+            ("Runtime", DeviceLine(device=device), 13, False),
         ]
 
         for label, widget, line, is_plotseis_param in self._inputs:
             label = QLabel(label)
             if is_plotseis_param:
                 widget.changed_signal.connect(self.export_plotseis_settings)  # type: ignore
             self.layout.addWidget(label, line, 0)
             self.layout.addWidget(widget, line, 1)
 
-        picks_from_file_label = QLabel("Show picks from file")
-        picks_from_file_widget = PicksFromFileLine(
-            byte_position=byte_position, first_byte=first_byte, encoding=encoding, picks_unit=picks_unit
-        )
-        picks_from_file_widget.toggle_picks_from_file_signal.connect(self.toggle_picks_from_file_signal)
-        picks_from_file_widget.export_picks_from_file_settings_signal.connect(
-            self.export_picks_from_file_settings_signal
-        )
-        self.layout.addWidget(picks_from_file_label, 10, 0)
-        self.layout.addWidget(picks_from_file_widget, 10, 1)
-
         self.picking_run = False
         self.run_button = QPushButton("Run picking", self)
         self.run_button.clicked.connect(self.picking_click)
+        self.run_button.setToolTip("Load NN to unlock picking")
         self.layout.addWidget(self.run_button)
         self.disable_picking()
 
         self.set_selection_mode()
 
         self.show()
 
     def enable_only_visualizations_settings(self) -> None:
         self.setEnabled(True)
         self.disable_picking()
 
     def enable_picking(self) -> None:
         self.run_button.setEnabled(True)
+        self.run_button.setToolTip("")
 
     def disable_picking(self) -> None:
         self.run_button.setEnabled(False)
 
     def picking_click(self) -> None:
         self.picking_run = not self.picking_run
         if self.picking_run:
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/slider_with_values.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/slider_with_values.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/spectrum_window.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/spectrum_window.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/threads.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/threads.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/tooltip_widget.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/tooltip_widget.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/desktop/utils.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/desktop/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
-from PyQt5 import QtWidgets
+from PyQt5 import QtCore, QtGui, QtWidgets
 from PyQt5.QtCore import QEvent, QPoint, QPointF, Qt
 from PyQt5.QtWidgets import (
     QDesktopWidget,
     QDialog,
     QDialogButtonBox,
     QGraphicsSceneMouseEvent,
+    QHBoxLayout,
     QLabel,
     QPushButton,
+    QSizePolicy,
+    QStyle,
     QTextEdit,
     QVBoxLayout,
     QWidget,
 )
 from pyqtgraph import ViewBox
 
 
@@ -90,55 +93,60 @@
         center_point = QDesktopWidget().availableGeometry().center()
         qt_rectangle.moveCenter(center_point)
         widget.move(qt_rectangle.topLeft())
 
     if fix_size:
         widget.setFixedSize(width, height)
 
-    monitor = QDesktopWidget().screenGeometry(1)
-    widget.move(monitor.left(), monitor.top())
+    # monitor = QDesktopWidget().screenGeometry(1)
+    # widget.move(monitor.left(), monitor.top())
 
 
-class QHSeparationLine(QtWidgets.QWidget):
-    def __init__(self, text: str = ""):
+class QSeparationLine(QtWidgets.QWidget):
+    def __init__(self, text: str = "", type_line: Literal["h", "v"] = "h"):
         super().__init__()
 
-        # Create the horizontal line (QFrame)
+        assert type_line in ["h", "v"]
+
+        if type_line == "h":
+            layout = QtWidgets.QHBoxLayout(self)
+            size_policy = (QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
+            frame_shape = QtWidgets.QFrame.HLine
+        else:
+            layout = QtWidgets.QVBoxLayout(self)
+            size_policy = (QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Expanding)
+            frame_shape = QtWidgets.QFrame.VLine
+
         self.line = QtWidgets.QFrame(self)
-        self.line.setFrameShape(QtWidgets.QFrame.HLine)
+        self.line.setFrameShape(frame_shape)
         self.line.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line.setSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Fixed)
 
-        # Create the label for the text
-        self.label = QtWidgets.QLabel(text, self)
-        self.label.setStyleSheet("background-color: transparent; color: grey;")
-        self.label.setAlignment(Qt.AlignCenter)
-
-        # Create a horizontal layout to hold the line and the label
-        layout = QtWidgets.QHBoxLayout(self)
-        layout.setContentsMargins(0, 0, 0, 0)
-        layout.addWidget(self.line, 1)
-        layout.addWidget(self.label, 0)
-        layout.addWidget(self.line, 1)
-
-        # Adjust margins and spacing
-        layout.setSpacing(10)  # space between label and line
-        layout.setContentsMargins(0, 10, 0, 0)  # top margin to position label above line
+        self.line.setSizePolicy(*size_policy)
+
+        if text:
+            self.label = QtWidgets.QLabel(text, self)
+            self.label.setStyleSheet("background-color: transparent; color: grey;")
+            self.label.setAlignment(Qt.AlignCenter)
+            layout.addWidget(self.label)
+            layout.setSpacing(10)
+
+        layout.addWidget(self.line)
+        layout.setContentsMargins(1, 1, 1, 1)
 
         self.setLayout(layout)
 
 
-# class QHSeparationLine(QtWidgets.QFrame):
-#     def __init__(self) -> None:
-#         super().__init__()
-#         self.setMinimumWidth(1)
-#         self.setFixedHeight(20)
-#         self.setFrameShape(QtWidgets.QFrame.HLine)
-#         self.setFrameShadow(QtWidgets.QFrame.Sunken)
-#         self.setSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Minimum)
+class QHSeparationLine(QSeparationLine):
+    def __init__(self, text: str = ""):
+        super().__init__(text=text, type_line="h")
+
+
+class QVSeparationLine(QSeparationLine):
+    def __init__(self, text: str = ""):
+        super().__init__(text=text, type_line="v")
 
 
 TMappingSetup = Dict[int, Union[Tuple[str, Any], List[Any]]]
 
 
 def validate_mapping_setup_and_get_current_index(
     mapping: TMappingSetup,
@@ -192,7 +200,31 @@
     elif isinstance(event_or_point, QEvent):
         point = event_or_point.localPos()
     elif isinstance(event_or_point, (QPointF, QPoint)):
         point = event_or_point
     else:
         raise TypeError("Only events and points are available")
     return viewbox.mapSceneToView(point)
+
+
+class LabelWithHelp(QWidget):
+    def __init__(self, text: str, help_string: str, move_help_close_to_label: bool = True) -> None:
+        super().__init__()
+        self.layout = QHBoxLayout()
+        self.setLayout(self.layout)
+
+        self.label = QLabel(text)
+        self.label.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
+
+        self.help_button = QPushButton()
+        self.help_button.setFixedWidth(20)
+        icon = self.style().standardIcon(QStyle.SP_MessageBoxQuestion)
+        self.help_button.setIcon(icon)
+        self.help_button.setToolTip(help_string)
+        self.help_button.setStyleSheet("QPushButton { border: none; background-color: transparent; }")
+        self.help_button.setCursor(QtGui.QCursor(QtCore.Qt.WhatsThisCursor))
+
+        self.layout.addWidget(self.label)
+        self.layout.addWidget(self.help_button)
+        if move_help_close_to_label:
+            self.layout.addStretch(1)
+        self.layout.setContentsMargins(0, 0, 0, 0)
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/picking/ipicker.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/picking/ipicker.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/picking/picker_onnx.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/picking/picker_onnx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from pathlib import Path
 from typing import Any, Dict, Generator, Optional, Tuple, Union
 
 import numpy as np
 import onnxruntime as ort
 
 from first_breaks.picking.ipicker import IPicker
+from first_breaks.picking.picks import Picks
 from first_breaks.picking.task import Task
 from first_breaks.picking.utils import preprocess_gather
 from first_breaks.utils.cuda import ONNX_DEVICE2PROVIDER, get_recommended_device
-from first_breaks.utils.utils import calc_hash, chunk_iterable, download_model_onnx
+from first_breaks.utils.utils import (
+    calc_hash,
+    chunk_iterable,
+    download_model_onnx,
+    generate_color,
+)
 
 
 class IteratorOfTask:
     gather_key = "gather"
     gather_ids_key = "gather_ids"
 
     def __init__(self, task: Task):
@@ -29,14 +35,16 @@
 
     def __getitem__(self, idx: int) -> Dict[str, np.ndarray]:
         gather_ids = self.idx2gather_ids[idx]
         amplitudes = np.array(
             [-1 if idx in self.task.traces_to_inverse else 1 for idx in range(len(gather_ids))], dtype=np.float32
         )
         gather = self.task.sgy.read_traces_by_ids(gather_ids)
+        # gather = np.sign(gather) * gather ** 2
+        # gather = np.gradient(np.gradient(gather, axis=0), axis=0)
         gather = preprocess_gather(
             data=gather,
             gain=self.task.gain,
             clip=self.task.clip,
             normalize=self.task.normalize,
             f1_f2=self.task.f1_f2,
             f3_f4=self.task.f3_f4,
@@ -135,16 +143,27 @@
             task_confidence[indices.flatten()] = confidence.flatten()
 
             counter_step_finished += len(data)
             self.callback_step_finished(counter_step_finished)
 
         self.callback_processing_finished()
 
+        picks = Picks(
+            values=task_picks_in_sample.astype(int).tolist(),
+            unit="sample",
+            dt_mcs=task.sgy.dt_mcs,
+            confidence=task_confidence.tolist(),
+            modified_manually=False,
+            created_manually=False,
+            created_by_nn=True,
+            picks_color=generate_color(),
+            picking_parameters=task.picking_parameters,
+        )
+
         task.success = True
-        task.picks_in_samples = task_picks_in_sample.astype(int).tolist()
-        task.confidence = task_confidence.tolist()
+        task.picks = picks
         task.model_hash = self.model_hash
         task.assign_new_picks_id()
 
         self.need_interrupt = False
 
         return task
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/picking/utils.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/picking/utils.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/sgy/headers.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/sgy/headers.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/sgy/reader.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/sgy/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,16 +217,19 @@
             header = self._read_custom_trace_header_with_existed_descriptor(offset, fmt)
             traces_headers[name] = header
 
         self._traces_headers_raw = pd.DataFrame(data=traces_headers)
 
     def _scalar_raw_traces_headers(self) -> None:
         self.traces_headers = self._traces_headers_raw.copy()
-        for scalar_from, apply_to_columns in self._traces_headers_schema.scalar_from2apply.items():
-            scalar = self._traces_headers_raw[scalar_from].copy()
+        for (
+            scalar_from,
+            apply_to_columns,
+        ) in self._traces_headers_schema.scalar_from2apply.items():
+            scalar = np.array(self._traces_headers_raw[scalar_from].copy())
 
             scalar[scalar == 0] = 1
             scalar[scalar < 0] = 1 / abs(scalar[scalar < 0])
             self.traces_headers[apply_to_columns] = self.traces_headers[apply_to_columns].apply(lambda x: scalar * x)
 
     def _read_custom_trace_header_with_existed_descriptor(self, byte_position: int, encoding: str) -> Tuple[Any, ...]:
         size = self._traces_headers_schema.get_num_bytes(encoding)
@@ -251,24 +254,30 @@
     def read(self, min_sample: Optional[int] = None, max_sample: Optional[int] = None) -> np.ndarray:
         ids = list(range(self.num_traces))
         traces = self.read_traces_by_ids(ids, min_sample, max_sample)
         self.replace_traces(traces)
         return traces
 
     def get_chunked_reader(
-        self, chunk_size: int, min_sample: Optional[int] = None, max_sample: Optional[int] = None
+        self,
+        chunk_size: int,
+        min_sample: Optional[int] = None,
+        max_sample: Optional[int] = None,
     ) -> Generator[np.ndarray, None, None]:
         chunk_size = min(chunk_size, self.num_traces)
         all_ids = list(range(self.num_traces))
 
         for ids in chunk_iterable(all_ids, chunk_size):
             yield self.read_traces_by_ids(ids, min_sample, max_sample)
 
     def read_traces_by_ids(
-        self, ids: Sequence[int], min_sample: Optional[int] = None, max_sample: Optional[int] = None
+        self,
+        ids: Sequence[int],
+        min_sample: Optional[int] = None,
+        max_sample: Optional[int] = None,
     ) -> np.ndarray:
 
         if min_sample is not None:
             if min_sample < 0 or not isinstance(min_sample, int):
                 raise InvalidSamplesSlice("Invalid minimum slice index")
             min_sample = int(np.clip(min_sample, 0, self.num_samples))
         else:
@@ -370,22 +379,22 @@
 
     def _read_traces_double(self, buffer: bytes, shape: SizeHW) -> np.ndarray:
         return np.ndarray(shape, f"{self._endianess}f8", buffer, order="F")
 
     def export_sgy_with_picks(
         self,
         output_fname: Union[str, Path],
-        picks_in_samples: List[float],
+        picks_in_mcs: List[float],
         byte_position: int = 236,
         encoding: Optional[str] = None,
         picks_unit: Optional[str] = "mcs",
     ) -> None:
         assert not self.is_source_ndarray, "Only true SGY can be used for importing picks"
         assert 0 <= byte_position <= 236, "Only 0-236 bytes can be ised for writing"
-        assert len(picks_in_samples) == self.num_traces, "Number of traces and picks differs"
+        assert len(picks_in_mcs) == self.num_traces, "Number of traces and picks differs"
         assert picks_unit in ["ms", "mcs", "sample"]
 
         Path(output_fname).parent.mkdir(exist_ok=True, parents=True)
 
         if isinstance(self.source, (str, Path)):
             if Path(self.source).resolve() != Path(output_fname).resolve():
                 shutil.copyfile(str(self.source), str(output_fname))
@@ -401,19 +410,21 @@
                 for _, header, pack_type in self._traces_headers_schema.headers_schema
                 if header == self._traces_headers_schema.fb_pick_default
             ][0]
 
         cast_to = float if encoding in ["f", "d"] else int
 
         if picks_unit == "ms":
-            picks = self.units_converter.index2ms(picks_in_samples, cast_to=cast_to)
+            picks = self.units_converter.mcs2ms(picks_in_mcs, cast_to=cast_to)
         elif picks_unit == "mcs":
-            picks = self.units_converter.index2mcs(picks_in_samples, cast_to=cast_to)
+            picks = picks_in_mcs
+        elif picks_unit == "sample":
+            picks = self.units_converter.mcs2index(picks_in_mcs, cast_to=cast_to)
         else:
-            picks = picks_in_samples
+            raise ValueError("Unsupported 'picking unit'")
 
         self._descriptor = get_io(output_fname, mode="r+b")
         for idx, pick in enumerate(picks):  # type: ignore
             pointer = 3600 + (240 + self.num_samples * self._bps) * idx + byte_position
             pick_byte = struct.pack(f"{self._endianess}{encoding}", pick)
             self._descriptor.seek(pointer)
             self._descriptor.write(pick_byte)
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/utils/cuda.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/utils/debug.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/utils/debug.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/utils/fourier_transforms.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/utils/fourier_transforms.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/utils/utils.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/utils/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import io
 import random
 from itertools import islice
 from pathlib import Path
 from typing import Any, Dict, Generator, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
+import pandas as pd
 import requests
 
 from first_breaks.const import (
     DEMO_SGY_HASH,
     DEMO_SGY_PATH,
     DEMO_SGY_URL,
     MODEL_ONNX_HASH,
@@ -176,7 +177,18 @@
 
 
 def resolve_xy2postime(vsp_view: bool, x: Any, y: Any) -> Tuple[Any, Any]:
     if vsp_view:
         return y, x
     else:
         return x, y
+
+
+def as_list(sequence: Iterable[Any]) -> List[Any]:
+    if isinstance(sequence, (np.ndarray, pd.Series)):
+        return sequence.tolist()
+    elif isinstance(sequence, (list, tuple)):
+        return list(sequence)
+    elif isinstance(sequence, (np.number, float, int)):
+        return [sequence]
+    else:
+        raise TypeError("Unsupported 'sequence' type")
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks/utils/visualizations.py` & `first_breaks_picking_gpu-0.7.1/first_breaks/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks_picking_gpu.egg-info/PKG-INFO` & `first_breaks_picking_gpu-0.7.1/first_breaks_picking_gpu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: first-breaks-picking-gpu
-Version: 0.6.2
+Version: 0.7.1
 Summary: Project is devoted to pick waves that are the first to be detected on a seismogram with neural network (CUDA accelerated)
 Author: Aleksei Tarasov
 Author-email: Aleksei Tarasov <aleksei.v.tarasov@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,31 +213,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <=3.10,>=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests==2.28.2
-Requires-Dist: numpy==1.24.2
-Requires-Dist: pandas==2.0.0
-Requires-Dist: PyQt5==5.15.9
-Requires-Dist: pyqtgraph==0.13.3
-Requires-Dist: tqdm==4.65.0
-Requires-Dist: click==8.1.3
-Requires-Dist: pydantic==2.0.3
-Requires-Dist: pytest==7.3.2
-Requires-Dist: onnxruntime-gpu==1.14.1
+Requires-Dist: requests>=2.28.2
+Requires-Dist: numpy>=1.24.2
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: PyQt5>=5.15.9
+Requires-Dist: pyqtgraph>=0.13.3
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: click>=8.1.3
+Requires-Dist: pydantic>=2.0.3
+Requires-Dist: pytest>=7.3.2
+Requires-Dist: pytest-qt>=4.4.0
+Requires-Dist: onnxruntime-gpu>=1.14.1
 
 # FirstBreaksPicking
 This project is devoted to pick waves that are the first to be detected on a seismogram (first breaks, first arrivals).
 Traditionally, this procedure is performed manually. When processing field data, the number of picks reaches hundreds of
 thousands. Existing analytical methods allow you to automate picking only on high-quality data with a high
 signal / noise ratio.
 
@@ -396,35 +397,33 @@
 from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 download_demo_sgy(fname=sgy_filename)
 sgy = SGY(sgy_filename)
 
-task = Task(source=sgy_filename,
+task = Task(source=sgy,
             traces_per_gather=12,
             maximum_time=100,
             gain=2)
 picker = PickerONNX()
 task = picker.process_task(task)
-
-# create an image with default parameters
-image_filename = 'default_view.png'
-export_image(task, image_filename)
+task.picks.color = (255, 0, 0)
 
 # create an image from the project preview
 image_filename = 'project_preview.png'
 export_image(task, image_filename,
              time_window=(0, 60),
              traces_window=(79.5, 90.5),
              show_processing_region=False,
              headers_total_pixels=80,
              height=500,
              width=700,
-             hide_traces_axis=True)
+             hide_traces_axis=True
+             )
 ```
 [code-block-end]:e2e-example
 
 For a better understanding of the steps taken, expand and read the next section.
 
 ### Detailed examples
 
@@ -574,15 +573,15 @@
 picker_cpu.change_settings(device='cuda', batch_size=3)
 picker_gpu.change_settings(device='cpu', batch_size=1)
 ```
 [code-block-end]:create-picker
 
 ### Pick first breaks
 
-Now, using all the created components, we can pick the first breaks and export the results.
+Now, using all the created components, we can pick the first breaks and retrieve results.
 
 [code-block-start]:pick-fb
 ```python
 from first_breaks.picking.task import Task
 from first_breaks.picking.picker_onnx import PickerONNX
 from first_breaks.sgy.reader import SGY
 
@@ -591,31 +590,63 @@
 
 task = Task(source=sgy,
             traces_per_gather=24,
             maximum_time=200)
 picker = PickerONNX()
 task = picker.process_task(task)
 
-# you can see results of picking
-print(task.picks_in_samples)
-print(task.picks_in_ms)
-print(task.confidence)
-
-# you can export picks to file as plain text
-task.export_result_as_txt('result.txt')
-# or save as json file
-task.export_result_as_json('result.json')
-# or make a copy of source SGY and put picks to 236 byte
-task.export_result_as_sgy('result.segy',
-                          byte_position=236,
-                          encoding='i',
-                          picks_unit='mcs')
+# picks available from attribute
+picks = task.picks
+
+# or by method
+picks = task.get_result()
+
+# print values and confidence of picks
+print(picks.picks_in_mcs, picks.confidence)
+
+# print picking parameters
+print(picks.picking_parameters, task.picking_parameters)
 ```
 [code-block-end]:pick-fb
 
+
+### Picks
+
+The picks are stored in class `Picks`. In addition to the pick values, the class stores additional
+information (picking parameters, color, etc.). The class instance is returned as a picking result, but can
+also be created manually.
+
+[code-block-start]:picks
+```python
+from first_breaks.picking.picks import Picks
+
+
+picks_in_samples = [1, 10, 20, 30, 50, 100]
+dt_mcs = 250
+
+picks = Picks(values=picks_in_samples, unit="mcs", dt_mcs=dt_mcs)
+
+# get values
+print(picks.picks_in_samples)
+print(picks.picks_in_mcs)
+print(picks.picks_in_ms)
+
+# change color and width for visualisation
+picks.color = (255, 0, 0)
+picks.width = 5
+
+# if picks are obtained by NN you can read extra attributes
+print(picks.confidence)
+print(picks.picking_parameters)
+print(picks.created_by_nn)
+
+```
+[code-block-end]:picks
+
+
 ### Visualizations
 
 You can save the seismogram and picks as an image. We use Qt backend for visualizations. Here we describe some usage
 scenarios.
 
 We've added named arguments to various scenarios for demonstration purposes, but in practice you can
 use them all. See the function arguments for more visualization options.
@@ -666,27 +697,28 @@
 [code-block-end]:plot-np
 
 Plot `SGY` with custom picks:
 
 [code-block-start]:plot-sgy-custom-picks
 ```python
 import numpy as np
+from first_breaks.picking.picks import Picks
 from first_breaks.sgy.reader import SGY
 from first_breaks.desktop.graph import export_image
 
 sgy_filename = 'data.sgy'
 image_filename = 'image.png'
 
 sgy = SGY(sgy_filename)
 picks_ms = np.random.uniform(low=0,
                              high=sgy.ns * sgy.dt_ms,
                              size=sgy.ntr)
+picks = Picks(values=picks_ms, unit="ms", dt_mcs=sgy.dt_mcs, color=(0, 100, 100))
 export_image(sgy, image_filename,
-             picks_ms=picks_ms,
-             picks_color=(0, 100, 100))
+             picks=picks)
 ```
 [code-block-end]:plot-sgy-custom-picks
 
 Plot result of picking:
 
 [code-block-start]:plot-sgy-real-picks
 ```python
```

### Comparing `first-breaks-picking-gpu-0.6.2/first_breaks_picking_gpu.egg-info/SOURCES.txt` & `first_breaks_picking_gpu-0.7.1/first_breaks_picking_gpu.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,29 +12,35 @@
 first_breaks/data_models/dependent.py
 first_breaks/data_models/independent.py
 first_breaks/data_models/initialised_defaults.py
 first_breaks/desktop/__init__.py
 first_breaks/desktop/bandfilter_widget.py
 first_breaks/desktop/byte_encode_unit_widget.py
 first_breaks/desktop/combobox_with_mapping.py
+first_breaks/desktop/export_widgets.py
 first_breaks/desktop/graph.py
+first_breaks/desktop/last_folder_manager.py
 first_breaks/desktop/main_gui.py
+first_breaks/desktop/multiselect_widget.py
 first_breaks/desktop/nn_manager.py
-first_breaks/desktop/picking_widget.py
+first_breaks/desktop/picks_manager_widget.py
 first_breaks/desktop/radioset_widget.py
 first_breaks/desktop/roi_manager.py
 first_breaks/desktop/settings_processing_widget.py
 first_breaks/desktop/slider_with_values.py
 first_breaks/desktop/spectrum_window.py
 first_breaks/desktop/threads.py
 first_breaks/desktop/tooltip_widget.py
 first_breaks/desktop/utils.py
+first_breaks/exports/__init__.py
+first_breaks/exports/export_picks.py
 first_breaks/picking/__init__.py
 first_breaks/picking/ipicker.py
 first_breaks/picking/picker_onnx.py
+first_breaks/picking/picks.py
 first_breaks/picking/task.py
 first_breaks/picking/utils.py
 first_breaks/sgy/__init__.py
 first_breaks/sgy/headers.py
 first_breaks/sgy/reader.py
 first_breaks/utils/__init__.py
 first_breaks/utils/cuda.py
```

### Comparing `first-breaks-picking-gpu-0.6.2/pyproject.toml` & `first_breaks_picking_gpu-0.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "first-breaks-picking-gpu"
 dynamic = ["version"]
 description = "Project is devoted to pick waves that are the first to be detected on a seismogram with neural network (CUDA accelerated)"
 readme = {file = "README.md", content-type = "text/markdown"}
 
-requires-python = ">=3.8,<=3.10"
+requires-python = ">=3.8"
 authors = [
     {name = "Aleksei Tarasov", email = "aleksei.v.tarasov@gmail.com"},
     {name = "Aleksei Tarasov"},
 ]
 urls = {Homepage = "https://github.com/DaloroAT/first_breaks_picking"}
 keywords = [
     "seismic",
@@ -29,31 +29,32 @@
     "Operating System :: OS Independent",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Recognition",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 entry-points = {console_scripts = {first-breaks-picking = "first_breaks.cli:cli_commands"}}
 dependencies = [
-    "requests==2.28.2",
-    "numpy==1.24.2",
-    "pandas==2.0.0",
-    "PyQt5==5.15.9",
-    "pyqtgraph==0.13.3",
-    "tqdm==4.65.0",
-    "click==8.1.3",
-    "pydantic==2.0.3",
-    "pytest==7.3.2",
-    "onnxruntime-gpu==1.14.1"
+    "requests>=2.28.2",
+    "numpy>=1.24.2",
+    "pandas>=2.0.0",
+    "PyQt5>=5.15.9",
+    "pyqtgraph>=0.13.3",
+    "tqdm>=4.65.0",
+    "click>=8.1.3",
+    "pydantic>=2.0.3",
+    "pytest>=7.3.2",
+    "pytest-qt>=4.4.0",
+    "onnxruntime-gpu>=1.14.1"
 ]
 
 
 [tool.setuptools.dynamic]
 version = {file = "first_breaks/VERSION"}
 
 
@@ -61,15 +62,15 @@
 exclude = ["first_breaks._pytorch*"]
 include = ["first_breaks*"]
 
 
 [tool.briefcase]
 project_name = "FirstBreaksPickingGPU"
 bundle = "com.example"
-version = "0.6.2"
+version = "0.7.1"
 url = "https://github.com/DaloroAT/first_breaks_picking"
 license = {file = "LICENSE"}
 
 [tool.briefcase.app.first_breaks]
 formal_name = "FirstBreaksPickingGPU"
 #description = "Project is devoted to pick waves that are the first to be detected on a seismogram with neural network"
 #icon = "src/mypysideapp/resources/appicon" # Briecase will choose the right extension depending the os (png,ico,...)
```

