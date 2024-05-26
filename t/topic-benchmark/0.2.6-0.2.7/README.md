# Comparing `tmp/topic_benchmark-0.2.6.tar.gz` & `tmp/topic_benchmark-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic_benchmark-0.2.6.tar", max compression
+gzip compressed data, was "topic_benchmark-0.2.7.tar", max compression
```

## Comparing `topic_benchmark-0.2.6.tar` & `topic_benchmark-0.2.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1071 2024-02-19 07:38:43.381533 topic_benchmark-0.2.6/LICENSE
--rw-r--r--   0        0        0     1881 2024-04-09 07:01:18.311495 topic_benchmark-0.2.6/README.md
--rw-r--r--   0        0        0      768 2024-05-23 13:32:50.242709 topic_benchmark-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      153 2024-03-22 10:07:39.674258 topic_benchmark-0.2.6/topic_benchmark/__init__.py
--rw-r--r--   0        0        0       78 2024-02-19 10:22:20.253816 topic_benchmark-0.2.6/topic_benchmark/__main__.py
--rw-r--r--   0        0        0      384 2024-02-19 09:24:15.274817 topic_benchmark-0.2.6/topic_benchmark/base.py
--rw-r--r--   0        0        0     3044 2024-03-07 13:00:54.142517 topic_benchmark-0.2.6/topic_benchmark/benchmark.py
--rw-r--r--   0        0        0     4215 2024-05-23 12:19:51.911005 topic_benchmark-0.2.6/topic_benchmark/cli.py
--rw-r--r--   0        0        0     2353 2024-05-23 12:19:51.911005 topic_benchmark-0.2.6/topic_benchmark/cluster_problem.py
--rw-r--r--   0        0        0      146 2024-05-23 12:19:51.931005 topic_benchmark-0.2.6/topic_benchmark/datasets/__init__.py
--rw-r--r--   0        0        0      326 2024-05-23 12:19:51.931005 topic_benchmark-0.2.6/topic_benchmark/datasets/arxiv_ml.py
--rw-r--r--   0        0        0      244 2024-05-23 12:19:51.931005 topic_benchmark-0.2.6/topic_benchmark/datasets/bbc_news.py
--rw-r--r--   0        0        0      806 2024-03-07 13:02:16.230526 topic_benchmark-0.2.6/topic_benchmark/datasets/newsgroups.py
--rw-r--r--   0        0        0      126 2024-02-19 10:05:20.151719 topic_benchmark-0.2.6/topic_benchmark/defaults.py
--rw-r--r--   0        0        0       50 2024-03-22 10:07:39.678258 topic_benchmark-0.2.6/topic_benchmark/encoders/__init__.py
--rw-r--r--   0        0        0      842 2024-03-22 10:07:39.678258 topic_benchmark-0.2.6/topic_benchmark/encoders/e5_encoders.py
--rw-r--r--   0        0        0     3354 2024-04-09 06:46:05.698513 topic_benchmark-0.2.6/topic_benchmark/figures.py
--rw-r--r--   0        0        0    12974 2024-05-23 12:19:51.911005 topic_benchmark-0.2.6/topic_benchmark/figures_plt.py
--rw-r--r--   0        0        0      133 2024-02-19 10:25:03.206775 topic_benchmark-0.2.6/topic_benchmark/metrics/__init__.py
--rw-r--r--   0        0        0      539 2024-02-25 14:06:04.842162 topic_benchmark-0.2.6/topic_benchmark/metrics/diversity.py
--rw-r--r--   0        0        0      881 2024-03-05 08:34:40.883831 topic_benchmark-0.2.6/topic_benchmark/metrics/npmi.py
--rw-r--r--   0        0        0     1613 2024-05-23 12:19:51.931005 topic_benchmark-0.2.6/topic_benchmark/metrics/wec.py
--rw-r--r--   0        0        0      185 2024-02-25 14:34:59.468057 topic_benchmark-0.2.6/topic_benchmark/models/__init__.py
--rw-r--r--   0        0        0      960 2024-05-23 13:30:14.158465 topic_benchmark-0.2.6/topic_benchmark/models/bertopic.py
--rw-r--r--   0        0        0     3208 2024-05-23 12:19:51.935005 topic_benchmark-0.2.6/topic_benchmark/models/classical.py
--rw-r--r--   0        0        0      984 2024-05-23 13:30:19.186472 topic_benchmark-0.2.6/topic_benchmark/models/top2vec.py
--rw-r--r--   0        0        0     1463 2024-05-23 12:19:51.935005 topic_benchmark-0.2.6/topic_benchmark/models/turftopic.py
--rw-r--r--   0        0        0      316 2024-03-22 10:07:39.678258 topic_benchmark-0.2.6/topic_benchmark/registries.py
--rw-r--r--   0        0        0     4714 2024-05-23 12:18:52.982894 topic_benchmark-0.2.6/topic_benchmark/table.py
--rw-r--r--   0        0        0      620 2024-02-25 14:32:02.743581 topic_benchmark-0.2.6/topic_benchmark/utils.py
--rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 topic_benchmark-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-19 07:38:43.381533 topic_benchmark-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1881 2024-04-09 07:01:18.311495 topic_benchmark-0.2.7/README.md
+-rw-r--r--   0        0        0      768 2024-05-26 12:53:11.715846 topic_benchmark-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      153 2024-03-22 10:07:39.674258 topic_benchmark-0.2.7/topic_benchmark/__init__.py
+-rw-r--r--   0        0        0       78 2024-02-19 10:22:20.253816 topic_benchmark-0.2.7/topic_benchmark/__main__.py
+-rw-r--r--   0        0        0      384 2024-02-19 09:24:15.274817 topic_benchmark-0.2.7/topic_benchmark/base.py
+-rw-r--r--   0        0        0     3044 2024-03-07 13:00:54.142517 topic_benchmark-0.2.7/topic_benchmark/benchmark.py
+-rw-r--r--   0        0        0     4215 2024-05-23 12:19:51.911005 topic_benchmark-0.2.7/topic_benchmark/cli.py
+-rw-r--r--   0        0        0     2353 2024-05-23 12:19:51.911005 topic_benchmark-0.2.7/topic_benchmark/cluster_problem.py
+-rw-r--r--   0        0        0      146 2024-05-23 12:19:51.931005 topic_benchmark-0.2.7/topic_benchmark/datasets/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-23 12:19:51.931005 topic_benchmark-0.2.7/topic_benchmark/datasets/arxiv_ml.py
+-rw-r--r--   0        0        0      244 2024-05-23 12:19:51.931005 topic_benchmark-0.2.7/topic_benchmark/datasets/bbc_news.py
+-rw-r--r--   0        0        0      806 2024-03-07 13:02:16.230526 topic_benchmark-0.2.7/topic_benchmark/datasets/newsgroups.py
+-rw-r--r--   0        0        0      126 2024-02-19 10:05:20.151719 topic_benchmark-0.2.7/topic_benchmark/defaults.py
+-rw-r--r--   0        0        0       50 2024-03-22 10:07:39.678258 topic_benchmark-0.2.7/topic_benchmark/encoders/__init__.py
+-rw-r--r--   0        0        0      842 2024-03-22 10:07:39.678258 topic_benchmark-0.2.7/topic_benchmark/encoders/e5_encoders.py
+-rw-r--r--   0        0        0     3354 2024-04-09 06:46:05.698513 topic_benchmark-0.2.7/topic_benchmark/figures.py
+-rw-r--r--   0        0        0    12974 2024-05-23 12:19:51.911005 topic_benchmark-0.2.7/topic_benchmark/figures_plt.py
+-rw-r--r--   0        0        0      133 2024-02-19 10:25:03.206775 topic_benchmark-0.2.7/topic_benchmark/metrics/__init__.py
+-rw-r--r--   0        0        0      539 2024-02-25 14:06:04.842162 topic_benchmark-0.2.7/topic_benchmark/metrics/diversity.py
+-rw-r--r--   0        0        0      881 2024-03-05 08:34:40.883831 topic_benchmark-0.2.7/topic_benchmark/metrics/npmi.py
+-rw-r--r--   0        0        0     1613 2024-05-23 12:19:51.931005 topic_benchmark-0.2.7/topic_benchmark/metrics/wec.py
+-rw-r--r--   0        0        0      185 2024-02-25 14:34:59.468057 topic_benchmark-0.2.7/topic_benchmark/models/__init__.py
+-rw-r--r--   0        0        0      960 2024-05-23 13:30:14.158465 topic_benchmark-0.2.7/topic_benchmark/models/bertopic.py
+-rw-r--r--   0        0        0     3208 2024-05-23 12:19:51.935005 topic_benchmark-0.2.7/topic_benchmark/models/classical.py
+-rw-r--r--   0        0        0      984 2024-05-23 13:30:19.186472 topic_benchmark-0.2.7/topic_benchmark/models/top2vec.py
+-rw-r--r--   0        0        0     1462 2024-05-26 12:46:58.701045 topic_benchmark-0.2.7/topic_benchmark/models/turftopic.py
+-rw-r--r--   0        0        0      316 2024-03-22 10:07:39.678258 topic_benchmark-0.2.7/topic_benchmark/registries.py
+-rw-r--r--   0        0        0     5882 2024-05-23 14:11:31.140139 topic_benchmark-0.2.7/topic_benchmark/table.py
+-rw-r--r--   0        0        0      620 2024-02-25 14:32:02.743581 topic_benchmark-0.2.7/topic_benchmark/utils.py
+-rw-r--r--   0        0        0     3223 1970-01-01 00:00:00.000000 topic_benchmark-0.2.7/PKG-INFO
```

### Comparing `topic_benchmark-0.2.6/LICENSE` & `topic_benchmark-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/README.md` & `topic_benchmark-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/pyproject.toml` & `topic_benchmark-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 line-length=79
 
 [tool.ruff]
 line-length=79
 
 [tool.poetry]
 name = "topic-benchmark"
-version = "0.2.6"
+version = "0.2.7"
 description = "Benchmarking topic models for a paper"
 authors = ["Márton Kardos <power.up1163@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.23.0"
 scikit-learn = "^1.2.0"
 sentence-transformers = "^2.2.0"
 torch = "^2.1.0"
-scipy = "^1.10.0"
+scipy = "~1.10.0"
 rich = "^13.6.0"
 pyro-ppl = "^1.8.0"
-turftopic = "^0.2.13"
+turftopic = "^0.2.14"
 umap-learn = "^0.5.0"
 hdbscan = "^0.8.0"
 catalogue = "^2.0.0"
 gensim = "^4.3.2"
 radicli = "^0.0.25"
 pandas = "^2.1.0"
 plotly = "^5.18.0"
```

### Comparing `topic_benchmark-0.2.6/topic_benchmark/benchmark.py` & `topic_benchmark-0.2.7/topic_benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/cli.py` & `topic_benchmark-0.2.7/topic_benchmark/cli.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/cluster_problem.py` & `topic_benchmark-0.2.7/topic_benchmark/cluster_problem.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/datasets/newsgroups.py` & `topic_benchmark-0.2.7/topic_benchmark/datasets/newsgroups.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/encoders/e5_encoders.py` & `topic_benchmark-0.2.7/topic_benchmark/encoders/e5_encoders.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/figures.py` & `topic_benchmark-0.2.7/topic_benchmark/figures.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/figures_plt.py` & `topic_benchmark-0.2.7/topic_benchmark/figures_plt.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/metrics/diversity.py` & `topic_benchmark-0.2.7/topic_benchmark/metrics/diversity.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/metrics/npmi.py` & `topic_benchmark-0.2.7/topic_benchmark/metrics/npmi.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/metrics/wec.py` & `topic_benchmark-0.2.7/topic_benchmark/metrics/wec.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/models/bertopic.py` & `topic_benchmark-0.2.7/topic_benchmark/models/bertopic.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/models/classical.py` & `topic_benchmark-0.2.7/topic_benchmark/models/classical.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/models/top2vec.py` & `topic_benchmark-0.2.7/topic_benchmark/models/top2vec.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/topic_benchmark/models/turftopic.py` & `topic_benchmark-0.2.7/topic_benchmark/models/turftopic.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 # @model_registry.register("GMM")
 def load_gmm(encoder, vectorizer: CountVectorizer) -> Loader:
     return partial(
         GMM, encoder=encoder, vectorizer=vectorizer, random_state=42
     )
 
-
 # @model_registry.register("KeyNMF")
 def load_keynmf(encoder, vectorizer: CountVectorizer) -> Loader:
     return partial(
         KeyNMF, encoder=encoder, vectorizer=vectorizer, random_state=42
     )
```

### Comparing `topic_benchmark-0.2.6/topic_benchmark/utils.py` & `topic_benchmark-0.2.7/topic_benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `topic_benchmark-0.2.6/PKG-INFO` & `topic_benchmark-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topic-benchmark
-Version: 0.2.6
+Version: 0.2.7
 Summary: Benchmarking topic models for a paper
 License: MIT
 Author: Márton Kardos
 Author-email: power.up1163@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,19 +21,19 @@
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: pandas (>=2.1.0,<3.0.0)
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: pyro-ppl (>=1.8.0,<2.0.0)
 Requires-Dist: radicli (>=0.0.25,<0.0.26)
 Requires-Dist: rich (>=13.6.0,<14.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
-Requires-Dist: scipy (>=1.10.0,<2.0.0)
+Requires-Dist: scipy (>=1.10.0,<1.11.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: sentence-transformers (>=2.2.0,<3.0.0)
 Requires-Dist: torch (>=2.1.0,<3.0.0)
-Requires-Dist: turftopic (>=0.2.13,<0.3.0)
+Requires-Dist: turftopic (>=0.2.14,<0.3.0)
 Requires-Dist: umap-learn (>=0.5.0,<0.6.0)
 Description-Content-Type: text/markdown
 
 # topic-benchmark
 Command Line Interface for benchmarking topic models.
 
 The package contains `catalogue` registries for all models, datasets and metrics for model evaluation,
```

