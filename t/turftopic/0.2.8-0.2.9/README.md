# Comparing `tmp/turftopic-0.2.8.tar.gz` & `tmp/turftopic-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turftopic-0.2.8.tar", max compression
+gzip compressed data, was "turftopic-0.2.9.tar", max compression
```

## Comparing `turftopic-0.2.8.tar` & `turftopic-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-11-28 09:10:15.078288 turftopic-0.2.8/LICENSE
--rw-r--r--   0        0        0     6595 2024-02-23 08:33:52.800699 turftopic-0.2.8/README.md
--rw-r--r--   0        0        0      616 2024-02-26 08:41:24.233870 turftopic-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      610 2023-12-18 10:12:04.650988 turftopic-0.2.8/turftopic/__init__.py
--rw-r--r--   0        0        0    11307 2024-02-15 11:38:24.443979 turftopic-0.2.8/turftopic/base.py
--rw-r--r--   0        0        0      775 2023-11-28 10:57:10.653184 turftopic-0.2.8/turftopic/centroid_distance.py
--rw-r--r--   0        0        0      353 2024-02-06 14:29:11.817843 turftopic-0.2.8/turftopic/data.py
--rw-r--r--   0        0        0     7775 2024-02-19 07:23:22.675347 turftopic-0.2.8/turftopic/dynamic.py
--rw-r--r--   0        0        0      327 2024-01-06 13:57:17.838014 turftopic-0.2.8/turftopic/encoders/__init__.py
--rw-r--r--   0        0        0      549 2024-02-06 14:40:28.674251 turftopic-0.2.8/turftopic/encoders/base.py
--rw-r--r--   0        0        0     2115 2024-02-06 14:40:28.674251 turftopic-0.2.8/turftopic/encoders/cohere.py
--rw-r--r--   0        0        0     1977 2024-02-06 14:40:28.674251 turftopic-0.2.8/turftopic/encoders/openai.py
--rw-r--r--   0        0        0     1767 2024-02-06 14:40:28.674251 turftopic-0.2.8/turftopic/encoders/voyage.py
--rw-r--r--   0        0        0      739 2024-01-06 13:36:54.154387 turftopic-0.2.8/turftopic/error.py
--rw-r--r--   0        0        0        0 2024-02-06 14:40:28.674251 turftopic-0.2.8/turftopic/models/__init__.py
--rw-r--r--   0        0        0     6618 2024-02-06 14:40:28.674251 turftopic-0.2.8/turftopic/models/cluster.py
--rw-r--r--   0        0        0    10412 2024-02-26 08:39:42.952529 turftopic-0.2.8/turftopic/models/ctm.py
--rw-r--r--   0        0        0     4127 2024-02-06 14:40:28.674251 turftopic-0.2.8/turftopic/models/decomp.py
--rw-r--r--   0        0        0     6374 2024-02-23 08:32:55.800827 turftopic-0.2.8/turftopic/models/gmm.py
--rw-r--r--   0        0        0    10643 2024-02-07 11:01:45.719674 turftopic-0.2.8/turftopic/models/keynmf.py
--rw-r--r--   0        0        0      503 2023-12-13 10:26:44.031626 turftopic-0.2.8/turftopic/soft_ctf_idf.py
--rw-r--r--   0        0        0      167 2024-01-06 12:41:09.491532 turftopic-0.2.8/turftopic/vectorizer.py
--rw-r--r--   0        0        0     7519 1970-01-01 00:00:00.000000 turftopic-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-11-28 09:10:15.078288 turftopic-0.2.9/LICENSE
+-rw-r--r--   0        0        0     6595 2024-02-23 08:33:52.800699 turftopic-0.2.9/README.md
+-rw-r--r--   0        0        0      616 2024-02-26 13:27:40.447906 turftopic-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      610 2023-12-18 10:12:04.650988 turftopic-0.2.9/turftopic/__init__.py
+-rw-r--r--   0        0        0    11307 2024-02-15 11:38:24.443979 turftopic-0.2.9/turftopic/base.py
+-rw-r--r--   0        0        0      353 2024-02-06 14:29:11.817843 turftopic-0.2.9/turftopic/data.py
+-rw-r--r--   0        0        0     7775 2024-02-19 07:23:22.675347 turftopic-0.2.9/turftopic/dynamic.py
+-rw-r--r--   0        0        0      327 2024-01-06 13:57:17.838014 turftopic-0.2.9/turftopic/encoders/__init__.py
+-rw-r--r--   0        0        0      549 2024-02-06 14:40:28.674251 turftopic-0.2.9/turftopic/encoders/base.py
+-rw-r--r--   0        0        0     2115 2024-02-06 14:40:28.674251 turftopic-0.2.9/turftopic/encoders/cohere.py
+-rw-r--r--   0        0        0     1977 2024-02-06 14:40:28.674251 turftopic-0.2.9/turftopic/encoders/openai.py
+-rw-r--r--   0        0        0     1767 2024-02-06 14:40:28.674251 turftopic-0.2.9/turftopic/encoders/voyage.py
+-rw-r--r--   0        0        0      739 2024-01-06 13:36:54.154387 turftopic-0.2.9/turftopic/error.py
+-rw-r--r--   0        0        0     1627 2024-02-26 12:20:30.768390 turftopic-0.2.9/turftopic/feature_importance.py
+-rw-r--r--   0        0        0        0 2024-02-06 14:40:28.674251 turftopic-0.2.9/turftopic/models/__init__.py
+-rw-r--r--   0        0        0    11626 2024-02-26 13:20:55.770750 turftopic-0.2.9/turftopic/models/cluster.py
+-rw-r--r--   0        0        0    10412 2024-02-26 08:39:42.952529 turftopic-0.2.9/turftopic/models/ctm.py
+-rw-r--r--   0        0        0     4127 2024-02-06 14:40:28.674251 turftopic-0.2.9/turftopic/models/decomp.py
+-rw-r--r--   0        0        0     6380 2024-02-26 12:12:10.171638 turftopic-0.2.9/turftopic/models/gmm.py
+-rw-r--r--   0        0        0    10643 2024-02-07 11:01:45.719674 turftopic-0.2.9/turftopic/models/keynmf.py
+-rw-r--r--   0        0        0      167 2024-01-06 12:41:09.491532 turftopic-0.2.9/turftopic/vectorizer.py
+-rw-r--r--   0        0        0     7519 1970-01-01 00:00:00.000000 turftopic-0.2.9/PKG-INFO
```

### Comparing `turftopic-0.2.8/LICENSE` & `turftopic-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/README.md` & `turftopic-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/pyproject.toml` & `turftopic-0.2.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length=79
 
 [tool.poetry]
 name = "turftopic"
-version = "0.2.8"
+version = "0.2.9"
 description = "Topic modeling with contextual representations from sentence transformers."
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `turftopic-0.2.8/turftopic/__init__.py` & `turftopic-0.2.9/turftopic/__init__.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/base.py` & `turftopic-0.2.9/turftopic/base.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/dynamic.py` & `turftopic-0.2.9/turftopic/dynamic.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/encoders/base.py` & `turftopic-0.2.9/turftopic/encoders/base.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/encoders/cohere.py` & `turftopic-0.2.9/turftopic/encoders/cohere.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/encoders/openai.py` & `turftopic-0.2.9/turftopic/encoders/openai.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/encoders/voyage.py` & `turftopic-0.2.9/turftopic/encoders/voyage.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/error.py` & `turftopic-0.2.9/turftopic/error.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/models/ctm.py` & `turftopic-0.2.9/turftopic/models/ctm.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/models/decomp.py` & `turftopic-0.2.9/turftopic/models/decomp.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/turftopic/models/gmm.py` & `turftopic-0.2.9/turftopic/models/gmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from rich.console import Console
 from sentence_transformers import SentenceTransformer
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.mixture import BayesianGaussianMixture, GaussianMixture
 
 from turftopic.base import ContextualModel, Encoder
 from turftopic.dynamic import DynamicTopicModel, bin_timestamps
-from turftopic.soft_ctf_idf import soft_ctf_idf
+from turftopic.feature_importance import soft_ctf_idf
 from turftopic.vectorizer import default_vectorizer
 
 
 class GMM(ContextualModel, DynamicTopicModel):
     """Multivariate Gaussian Mixture Model over document embeddings.
     Models topics as mixture components.
```

### Comparing `turftopic-0.2.8/turftopic/models/keynmf.py` & `turftopic-0.2.9/turftopic/models/keynmf.py`

 * *Files identical despite different names*

### Comparing `turftopic-0.2.8/PKG-INFO` & `turftopic-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turftopic
-Version: 0.2.8
+Version: 0.2.9
 Summary: Topic modeling with contextual representations from sentence transformers.
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

