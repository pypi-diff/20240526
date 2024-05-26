# Comparing `tmp/xtrain-0.3.2.tar.gz` & `tmp/xtrain-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtrain-0.3.2.tar", max compression
+gzip compressed data, was "xtrain-0.3.3.tar", max compression
```

## Comparing `xtrain-0.3.2.tar` & `xtrain-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2024-05-10 19:15:25.469526 xtrain-0.3.2/LICENSE
--rw-r--r--   0        0        0     1832 2024-05-10 19:15:25.469526 xtrain-0.3.2/README.md
--rw-r--r--   0        0        0      833 2024-05-10 19:15:42.133483 xtrain-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      203 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/__init__.py
--rw-r--r--   0        0        0    13430 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/base_trainer.py
--rw-r--r--   0        0        0     3968 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/closure.py
--rw-r--r--   0        0        0     1631 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/loss.py
--rw-r--r--   0        0        0     4215 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/strategy.py
--rw-r--r--   0        0        0     7892 2024-05-10 19:15:25.469526 xtrain-0.3.2/xtrain/utils.py
--rw-r--r--   0        0        0     2165 1970-01-01 00:00:00.000000 xtrain-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-26 16:35:05.907687 xtrain-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1832 2024-05-26 16:35:05.907687 xtrain-0.3.3/README.md
+-rw-r--r--   0        0        0      658 2024-05-26 16:35:21.764054 xtrain-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-05-26 16:35:05.907687 xtrain-0.3.3/xtrain/__init__.py
+-rw-r--r--   0        0        0    13430 2024-05-26 16:35:05.907687 xtrain-0.3.3/xtrain/base_trainer.py
+-rw-r--r--   0        0        0     3968 2024-05-26 16:35:05.907687 xtrain-0.3.3/xtrain/closure.py
+-rw-r--r--   0        0        0     1631 2024-05-26 16:35:05.907687 xtrain-0.3.3/xtrain/loss.py
+-rw-r--r--   0        0        0     4215 2024-05-26 16:35:05.911687 xtrain-0.3.3/xtrain/strategy.py
+-rw-r--r--   0        0        0     7892 2024-05-26 16:35:05.911687 xtrain-0.3.3/xtrain/utils.py
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 xtrain-0.3.3/PKG-INFO
```

### Comparing `xtrain-0.3.2/LICENSE` & `xtrain-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xtrain-0.3.2/README.md` & `xtrain-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `xtrain-0.3.2/xtrain/base_trainer.py` & `xtrain-0.3.3/xtrain/base_trainer.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.3.2/xtrain/closure.py` & `xtrain-0.3.3/xtrain/closure.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.3.2/xtrain/loss.py` & `xtrain-0.3.3/xtrain/loss.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.3.2/xtrain/strategy.py` & `xtrain-0.3.3/xtrain/strategy.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.3.2/xtrain/utils.py` & `xtrain-0.3.3/xtrain/utils.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.3.2/PKG-INFO` & `xtrain-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: xtrain
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Flax trainer
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: cuda12
 Requires-Dist: flax (>=0.8,<0.9)
+Requires-Dist: jax[cuda12] (>=0.4,<0.5) ; extra == "cuda12"
 Description-Content-Type: text/markdown
 
 ## XTRAIN: a tiny library for training [Flax](https://github.com/google/flax) models.
 
 Design goals:
 
   - Help avoiding boiler-plate code
```

