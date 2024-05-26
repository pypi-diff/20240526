# Comparing `tmp/tf_nightly_cpu-2.17.0.dev20240525-cp39-cp39-win_amd64.whl.zip` & `tmp/tf_nightly_cpu-2.17.0.dev20240526-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
 Zip file size: 2209 bytes, number of entries: 4
--rw-rw-r--  2.0 unx     3267 b- defN 24-May-25 08:45 tf_nightly_cpu-2.17.0.dev20240525.dist-info/METADATA
--rw-rw-r--  2.0 unx       99 b- defN 24-May-25 08:45 tf_nightly_cpu-2.17.0.dev20240525.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 24-May-25 08:45 tf_nightly_cpu-2.17.0.dev20240525.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      377 b- defN 24-May-25 08:45 tf_nightly_cpu-2.17.0.dev20240525.dist-info/RECORD
+-rw-rw-r--  2.0 unx     3267 b- defN 24-May-26 08:45 tf_nightly_cpu-2.17.0.dev20240526.dist-info/METADATA
+-rw-rw-r--  2.0 unx       99 b- defN 24-May-26 08:45 tf_nightly_cpu-2.17.0.dev20240526.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 24-May-26 08:45 tf_nightly_cpu-2.17.0.dev20240526.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      377 b- defN 24-May-26 08:45 tf_nightly_cpu-2.17.0.dev20240526.dist-info/RECORD
 4 files, 3744 bytes uncompressed, 1467 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: tf_nightly_cpu-2.17.0.dev20240525.dist-info/METADATA
+Filename: tf_nightly_cpu-2.17.0.dev20240526.dist-info/METADATA
 Comment: 
 
-Filename: tf_nightly_cpu-2.17.0.dev20240525.dist-info/WHEEL
+Filename: tf_nightly_cpu-2.17.0.dev20240526.dist-info/WHEEL
 Comment: 
 
-Filename: tf_nightly_cpu-2.17.0.dev20240525.dist-info/top_level.txt
+Filename: tf_nightly_cpu-2.17.0.dev20240526.dist-info/top_level.txt
 Comment: 
 
-Filename: tf_nightly_cpu-2.17.0.dev20240525.dist-info/RECORD
+Filename: tf_nightly_cpu-2.17.0.dev20240526.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tf_nightly_cpu-2.17.0.dev20240525.dist-info/METADATA` & `tf_nightly_cpu-2.17.0.dev20240526.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-nightly-cpu
-Version: 2.17.0.dev20240525
+Version: 2.17.0.dev20240526
 Summary: TensorFlow is an open source machine learning framework for everyone.
 Home-page: https://www.tensorflow.org/
 Author: Google Inc.
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Download-URL: https://github.com/tensorflow/tensorflow/tags
 Keywords: tensorflow tensor machine learning
@@ -26,15 +26,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: tf-nightly-intel ==2.17.0-dev20240525 ; platform_system == "Windows"
+Requires-Dist: tf-nightly-intel ==2.17.0-dev20240526 ; platform_system == "Windows"
 Provides-Extra: and-cuda
 Requires-Dist: nvidia-cublas-cu12 ==12.3.4.1 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-cupti-cu12 ==12.3.101 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-nvcc-cu12 ==12.3.107 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-nvrtc-cu12 ==12.3.107 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cuda-runtime-cu12 ==12.3.101 ; extra == 'and-cuda'
 Requires-Dist: nvidia-cudnn-cu12 ==8.9.7.29 ; extra == 'and-cuda'
```

