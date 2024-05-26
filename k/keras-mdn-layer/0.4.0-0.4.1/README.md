# Comparing `tmp/keras_mdn_layer-0.4.0.tar.gz` & `tmp/keras_mdn_layer-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_mdn_layer-0.4.0.tar", max compression
+gzip compressed data, was "keras_mdn_layer-0.4.1.tar", max compression
```

## Comparing `keras_mdn_layer-0.4.0.tar` & `keras_mdn_layer-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1055 2024-04-02 01:45:40.378650 keras_mdn_layer-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     6271 2024-05-07 05:20:40.827978 keras_mdn_layer-0.4.0/README.md
--rw-r--r--   0        0        0    11003 2024-04-02 01:45:40.379305 keras_mdn_layer-0.4.0/keras_mdn_layer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 01:45:40.379390 keras_mdn_layer-0.4.0/keras_mdn_layer/tests/__init__.py
--rw-r--r--   0        0        0     1755 2024-05-07 05:20:14.085692 keras_mdn_layer-0.4.0/keras_mdn_layer/tests/test_mdn.py
--rw-r--r--   0        0        0       22 2024-05-07 05:36:23.633125 keras_mdn_layer-0.4.0/keras_mdn_layer/version.py
--rw-r--r--   0        0        0      663 2024-05-07 05:37:22.504410 keras_mdn_layer-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6916 1970-01-01 00:00:00.000000 keras_mdn_layer-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2019-06-11 23:37:31.000000 keras_mdn_layer-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     6355 2024-05-26 12:13:20.095479 keras_mdn_layer-0.4.1/README.md
+-rw-r--r--   0        0        0    11003 2024-05-26 12:13:20.096526 keras_mdn_layer-0.4.1/keras_mdn_layer/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:13:20.096673 keras_mdn_layer-0.4.1/keras_mdn_layer/tests/__init__.py
+-rw-r--r--   0        0        0     1755 2024-05-26 12:13:20.097036 keras_mdn_layer-0.4.1/keras_mdn_layer/tests/test_mdn.py
+-rw-r--r--   0        0        0       22 2024-05-26 12:18:47.880495 keras_mdn_layer-0.4.1/keras_mdn_layer/version.py
+-rw-r--r--   0        0        0      942 2024-05-26 12:20:02.431681 keras_mdn_layer-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7277 1970-01-01 00:00:00.000000 keras_mdn_layer-0.4.1/PKG-INFO
```

### Comparing `keras_mdn_layer-0.4.0/LICENSE.md` & `keras_mdn_layer-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `keras_mdn_layer-0.4.0/README.md` & `keras_mdn_layer-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 
     python3 -m pip install keras-mdn-layer
 
 And finally, import the module in Python: `import keras_mdn_layer as mdn`
 
 Alternatively, you can clone or download this repository and then install via `python setup.py install`, or copy the `mdn` folder into your own project.
 
+## Build
+
+This project builds using `poetry`. To build a wheel use `poetry build`.
+
 ## Examples
 
 Some examples are provided in the notebooks directory.
 
 There's scripts for fitting multivalued functions, a standard MDN toy problem:
 
 <img src="https://preview.ibb.co/mZzkpd/Keras_MDN_Demo.jpg" alt="Keras MDN Demo" border="0">
```

### Comparing `keras_mdn_layer-0.4.0/keras_mdn_layer/__init__.py` & `keras_mdn_layer-0.4.1/keras_mdn_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_mdn_layer-0.4.0/keras_mdn_layer/tests/test_mdn.py` & `keras_mdn_layer-0.4.1/keras_mdn_layer/tests/test_mdn.py`

 * *Files identical despite different names*

### Comparing `keras_mdn_layer-0.4.0/PKG-INFO` & `keras_mdn_layer-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: keras-mdn-layer
-Version: 0.4.0
+Version: 0.4.1
 Summary: An MDN Layer for Keras using TensorFlow's distributions module
+Home-page: https://github.com/cpmpercussion/keras-mdn-layer
 License: MIT
+Keywords: mixture density layer,neural network,machine learning
 Author: Charles Martin
 Author-email: cpm@charlesmartin.au
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: tensorflow (==2.15.0) ; sys_platform == "linux"
+Requires-Dist: tensorflow (>=2.15.0,<2.16.0) ; sys_platform == "linux"
 Requires-Dist: tensorflow-macos (==2.15.0) ; sys_platform == "darwin"
 Requires-Dist: tensorflow-probability (==0.23.0)
+Project-URL: Repository, https://github.com/cpmpercussion/keras-mdn-layer
 Description-Content-Type: text/markdown
 
 # Keras Mixture Density Network Layer
 
 [![Build and test keras-mdn-layer](https://github.com/cpmpercussion/keras-mdn-layer/actions/workflows/python-app.yml/badge.svg)](https://github.com/cpmpercussion/keras-mdn-layer/actions/workflows/python-app.yml)
 ![MIT License](https://img.shields.io/github/license/cpmpercussion/keras-mdn-layer.svg?style=flat)
 [![DOI](https://zenodo.org/badge/137585470.svg)](https://zenodo.org/badge/latestdoi/137585470)
@@ -39,14 +43,18 @@
 
     python3 -m pip install keras-mdn-layer
 
 And finally, import the module in Python: `import keras_mdn_layer as mdn`
 
 Alternatively, you can clone or download this repository and then install via `python setup.py install`, or copy the `mdn` folder into your own project.
 
+## Build
+
+This project builds using `poetry`. To build a wheel use `poetry build`.
+
 ## Examples
 
 Some examples are provided in the notebooks directory.
 
 There's scripts for fitting multivalued functions, a standard MDN toy problem:
 
 <img src="https://preview.ibb.co/mZzkpd/Keras_MDN_Demo.jpg" alt="Keras MDN Demo" border="0">
```

