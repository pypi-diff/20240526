# Comparing `tmp/rshf-0.0.1.tar.gz` & `tmp/rshf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rshf-0.0.1.tar", last modified: Sun May 26 00:37:17 2024, max compression
+gzip compressed data, was "rshf-0.0.3.tar", last modified: Sun May 26 02:06:57 2024, max compression
```

## Comparing `rshf-0.0.1.tar` & `rshf-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxr-xr-x   0 s.sastry (2034283) Domain Users (1000070)        0 2024-05-26 00:37:17.090687 rshf-0.0.1/
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)    11357 2024-05-25 23:34:50.000000 rshf-0.0.1/LICENSE
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)      974 2024-05-26 00:37:17.090687 rshf-0.0.1/PKG-INFO
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)      373 2024-05-25 23:48:18.000000 rshf-0.0.1/README.md
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)      103 2024-05-26 00:12:23.000000 rshf-0.0.1/pyproject.toml
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)       62 2024-05-26 00:03:39.000000 rshf-0.0.1/requirements.txt
-drwxr-xr-x   0 s.sastry (2034283) Domain Users (1000070)        0 2024-05-26 00:37:17.086687 rshf-0.0.1/rshf/
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)        0 2024-05-26 00:25:49.000000 rshf-0.0.1/rshf/__init__.py
-drwxr-xr-x   0 s.sastry (2034283) Domain Users (1000070)        0 2024-05-26 00:37:17.086687 rshf-0.0.1/rshf/geoclip/
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)       45 2024-05-25 23:46:47.000000 rshf-0.0.1/rshf/geoclip/__init__.py
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)     5210 2024-05-25 23:46:07.000000 rshf-0.0.1/rshf/geoclip/model.py
-drwxr-xr-x   0 s.sastry (2034283) Domain Users (1000070)        0 2024-05-26 00:37:17.086687 rshf-0.0.1/rshf/rvsa/
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)       49 2024-05-25 23:49:50.000000 rshf-0.0.1/rshf/rvsa/__init__.py
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)    15196 2024-05-25 23:50:36.000000 rshf-0.0.1/rshf/rvsa/model.py
-drwxr-xr-x   0 s.sastry (2034283) Domain Users (1000070)        0 2024-05-26 00:37:17.090687 rshf-0.0.1/rshf/satmae/
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)       49 2024-05-25 23:41:18.000000 rshf-0.0.1/rshf/satmae/__init__.py
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)    11255 2024-05-25 23:39:44.000000 rshf-0.0.1/rshf/satmae/model.py
-drwxr-xr-x   0 s.sastry (2034283) Domain Users (1000070)        0 2024-05-26 00:37:17.090687 rshf-0.0.1/rshf/satmaepp/
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)       51 2024-05-25 23:58:29.000000 rshf-0.0.1/rshf/satmaepp/__init__.py
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)    14183 2024-05-25 23:45:16.000000 rshf-0.0.1/rshf/satmaepp/model.py
-drwxr-xr-x   0 s.sastry (2034283) Domain Users (1000070)        0 2024-05-26 00:37:17.090687 rshf-0.0.1/rshf/scalemae/
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)       48 2024-05-25 23:58:20.000000 rshf-0.0.1/rshf/scalemae/__init__.py
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)     9905 2024-05-25 23:56:58.000000 rshf-0.0.1/rshf/scalemae/model.py
-drwxr-xr-x   0 s.sastry (2034283) Domain Users (1000070)        0 2024-05-26 00:37:17.090687 rshf-0.0.1/rshf.egg-info/
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)      974 2024-05-26 00:37:17.000000 rshf-0.0.1/rshf.egg-info/PKG-INFO
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)      473 2024-05-26 00:37:17.000000 rshf-0.0.1/rshf.egg-info/SOURCES.txt
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)        1 2024-05-26 00:37:17.000000 rshf-0.0.1/rshf.egg-info/dependency_links.txt
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)        1 2024-05-26 00:37:16.000000 rshf-0.0.1/rshf.egg-info/not-zip-safe
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)       63 2024-05-26 00:37:17.000000 rshf-0.0.1/rshf.egg-info/requires.txt
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)        5 2024-05-26 00:37:17.000000 rshf-0.0.1/rshf.egg-info/top_level.txt
--rw-r--r--   0 s.sastry (2034283) Domain Users (1000070)      628 2024-05-26 00:37:17.090687 rshf-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:57.882793 rshf-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 02:06:50.000000 rshf-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-26 02:06:57.882793 rshf-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-26 02:06:50.000000 rshf-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-26 02:06:50.000000 rshf-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-26 02:06:50.000000 rshf-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:57.870792 rshf-0.0.3/rshf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:57.870792 rshf-0.0.3/rshf/geoclip/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/geoclip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/geoclip/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:57.870792 rshf-0.0.3/rshf/rvsa/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/rvsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15196 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/rvsa/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:57.874792 rshf-0.0.3/rshf/satclip/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/satclip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/satclip/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/satclip/spherical_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/satclip/spherical_harmonics_closed_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)  7765721 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/satclip/spherical_harmonics_ylm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:57.882793 rshf-0.0.3/rshf/satmae/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/satmae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/satmae/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:57.882793 rshf-0.0.3/rshf/satmaepp/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/satmaepp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/satmaepp/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:57.882793 rshf-0.0.3/rshf/scalemae/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/scalemae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-26 02:06:50.000000 rshf-0.0.3/rshf/scalemae/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:06:57.882793 rshf-0.0.3/rshf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-26 02:06:57.000000 rshf-0.0.3/rshf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-26 02:06:57.000000 rshf-0.0.3/rshf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 02:06:57.000000 rshf-0.0.3/rshf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 02:06:57.000000 rshf-0.0.3/rshf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-26 02:06:57.000000 rshf-0.0.3/rshf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 02:06:57.000000 rshf-0.0.3/rshf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-26 02:06:57.882793 rshf-0.0.3/setup.cfg
```

### Comparing `rshf-0.0.1/LICENSE` & `rshf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rshf-0.0.1/PKG-INFO` & `rshf-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rshf
-Version: 0.0.1
+Version: 0.0.3
 Summary: RS pretrained models in huggingface style
 Home-page: https://github.com/mvrl/rshf
 Author: Srikumar Sastry
 Author-email: s.sastry@wustl.edu
 Keywords: Remote Sensing,Huggingface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,14 +12,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch==2.3.0
 Requires-Dist: timm==1.0.3
 Requires-Dist: numpy==1.26.4
 Requires-Dist: huggingface_hub==0.23.1
+Requires-Dist: einops==0.8.0
 
 # rshf
 ### Remote sensing pretrained models easy loading using huggingface -- PyTorch (for fast benchmarking)
 
 ### Installation:
 ```bash
 pip install rshf
@@ -27,7 +28,9 @@
 
 ### Example:
 ```python
 from rshf.satmae import SatMAE
 model = SatMAE.from_pretrained("MVRL/satmae-vitlarge-fmow-pretrain-800")
 print(model.forward_encoder(torch.randn(1, 3, 224, 224), mask_ratio=0.0)[0].shape)
 ```
+
+### List of models available here: [Link](https://huggingface.co/collections/MVRL/remote-sensing-foundation-models-664e8fcd67d8ca8c03f42d00)
```

### Comparing `rshf-0.0.1/rshf/geoclip/model.py` & `rshf-0.0.3/rshf/geoclip/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.1/rshf/rvsa/model.py` & `rshf-0.0.3/rshf/rvsa/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.1/rshf/satmae/model.py` & `rshf-0.0.3/rshf/satmae/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.1/rshf/satmaepp/model.py` & `rshf-0.0.3/rshf/satmaepp/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.1/rshf/scalemae/model.py` & `rshf-0.0.3/rshf/scalemae/model.py`

 * *Files identical despite different names*

### Comparing `rshf-0.0.1/rshf.egg-info/PKG-INFO` & `rshf-0.0.3/rshf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rshf
-Version: 0.0.1
+Version: 0.0.3
 Summary: RS pretrained models in huggingface style
 Home-page: https://github.com/mvrl/rshf
 Author: Srikumar Sastry
 Author-email: s.sastry@wustl.edu
 Keywords: Remote Sensing,Huggingface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,14 +12,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch==2.3.0
 Requires-Dist: timm==1.0.3
 Requires-Dist: numpy==1.26.4
 Requires-Dist: huggingface_hub==0.23.1
+Requires-Dist: einops==0.8.0
 
 # rshf
 ### Remote sensing pretrained models easy loading using huggingface -- PyTorch (for fast benchmarking)
 
 ### Installation:
 ```bash
 pip install rshf
@@ -27,7 +28,9 @@
 
 ### Example:
 ```python
 from rshf.satmae import SatMAE
 model = SatMAE.from_pretrained("MVRL/satmae-vitlarge-fmow-pretrain-800")
 print(model.forward_encoder(torch.randn(1, 3, 224, 224), mask_ratio=0.0)[0].shape)
 ```
+
+### List of models available here: [Link](https://huggingface.co/collections/MVRL/remote-sensing-foundation-models-664e8fcd67d8ca8c03f42d00)
```

### Comparing `rshf-0.0.1/setup.cfg` & `rshf-0.0.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rshf
-version = 0.0.1
+version = 0.0.3
 author = Srikumar Sastry
 author_email = s.sastry@wustl.edu
 description = RS pretrained models in huggingface style
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mvrl/rshf
 keywords = Remote Sensing, Huggingface
```

