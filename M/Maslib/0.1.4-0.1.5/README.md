# Comparing `tmp/Maslib-0.1.4.tar.gz` & `tmp/Maslib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Maslib-0.1.4.tar", last modified: Sun May 26 15:43:18 2024, max compression
+gzip compressed data, was "Maslib-0.1.5.tar", last modified: Sun May 26 15:49:59 2024, max compression
```

## Comparing `Maslib-0.1.4.tar` & `Maslib-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 15:43:18.122193 Maslib-0.1.4/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.1.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-26 15:43:18.097172 Maslib-0.1.4/MasLib/
--rw-rw-rw-   0        0        0     1310 2024-05-26 07:57:21.000000 Maslib-0.1.4/MasLib/__init__.py
--rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 Maslib-0.1.4/MasLib/classification.py
--rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 Maslib-0.1.4/MasLib/clustering.py
--rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 Maslib-0.1.4/MasLib/correlation.py
--rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 Maslib-0.1.4/MasLib/encoding.py
--rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 Maslib-0.1.4/MasLib/loading.py
--rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 Maslib-0.1.4/MasLib/regressions.py
--rw-rw-rw-   0        0        0    11632 2024-05-26 09:23:14.000000 Maslib-0.1.4/MasLib/text_coding.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:43:18.119191 Maslib-0.1.4/Maslib.egg-info/
--rw-rw-rw-   0        0        0      912 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-26 15:43:17.000000 Maslib-0.1.4/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      912 2024-05-26 15:43:18.120192 Maslib-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-26 09:52:47.000000 Maslib-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 15:43:18.122193 Maslib-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      830 2024-05-26 15:42:47.000000 Maslib-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 15:43:18.117189 Maslib-0.1.4/tests/
--rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 Maslib-0.1.4/tests/test_clustering.py
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.1.4/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.1.4/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.1.4/tests/test_grid_search.py
--rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 Maslib-0.1.4/tests/test_loading.py
--rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 Maslib-0.1.4/tests/test_regression.py
--rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 Maslib-0.1.4/tests/test_text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:49:59.717412 Maslib-0.1.5/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.1.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-26 15:49:59.693390 Maslib-0.1.5/MasLib/
+-rw-rw-rw-   0        0        0     1289 2024-05-26 15:49:25.000000 Maslib-0.1.5/MasLib/__init__.py
+-rw-rw-rw-   0        0        0    19758 2024-05-26 09:46:27.000000 Maslib-0.1.5/MasLib/classification.py
+-rw-rw-rw-   0        0        0    10049 2024-05-26 09:34:23.000000 Maslib-0.1.5/MasLib/clustering.py
+-rw-rw-rw-   0        0        0     1820 2024-05-26 09:28:23.000000 Maslib-0.1.5/MasLib/correlation.py
+-rw-rw-rw-   0        0        0     3677 2024-05-26 09:52:52.000000 Maslib-0.1.5/MasLib/encoding.py
+-rw-rw-rw-   0        0        0      563 2024-05-26 09:24:37.000000 Maslib-0.1.5/MasLib/loading.py
+-rw-rw-rw-   0        0        0    10025 2024-05-26 09:23:11.000000 Maslib-0.1.5/MasLib/regressions.py
+-rw-rw-rw-   0        0        0    11006 2024-05-26 15:49:15.000000 Maslib-0.1.5/MasLib/text_coding.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:49:59.714409 Maslib-0.1.5/Maslib.egg-info/
+-rw-rw-rw-   0        0        0      863 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 15:49:59.000000 Maslib-0.1.5/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      863 2024-05-26 15:49:59.715411 Maslib-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-26 09:52:47.000000 Maslib-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:49:59.717412 Maslib-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      790 2024-05-26 15:49:39.000000 Maslib-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:49:59.711407 Maslib-0.1.5/tests/
+-rw-rw-rw-   0        0        0     1604 2024-05-19 12:47:10.000000 Maslib-0.1.5/tests/test_clustering.py
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.1.5/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.1.5/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.1.5/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0      424 2024-05-19 12:45:36.000000 Maslib-0.1.5/tests/test_loading.py
+-rw-rw-rw-   0        0        0     2323 2024-05-19 11:18:27.000000 Maslib-0.1.5/tests/test_regression.py
+-rw-rw-rw-   0        0        0     1438 2024-05-19 12:44:54.000000 Maslib-0.1.5/tests/test_text_coding.py
```

### Comparing `Maslib-0.1.4/MasLib/__init__.py` & `Maslib-0.1.5/MasLib/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 from .classification import print_metrics, classification_with_svc, classification_with_random_forest, classification_with_knn, classification_with_logistic_regression, classification_with_naive_bayes, classification_with_decision_tree, classification_with_gradient_boosting, classification_with_adaboost,  optimize_svc, optimize_random_forest, optimize_knn, optimize_logistic_regression, optimize_naive_bayes, optimize_decision_tree, optimize_gradient_boosting, optimize_adaboost, grid_search_optimization
 from .clustering import scale_data, kmeans_clustering, hierarchical_clustering, dbscan_clustering, birch_clustering, mean_shift_clustering, spectral_clustering, affinity_propagation_clustering, calculate_metrics, plot_clusters, ClusteringModel, optimize_clustering
 from .correlation import compute_phik_matrix, plot_phik_correlation_matrix
 from .encoding import number_encode_features, process_column_and_merge, json_to_dataframe
 from .loading import save_model
 from .regressions import gb_regression, rf_regression, lr_regression, catboost_regression, xgb_regression, cross_val_evaluate, optimize_model
-from .text_coding import preprocess_text, vectorize_text, tfidf_vectorize_texts, lda_model, nmf_model, lsa_model, elbow_method_tfidf, bert_topic_modeling, sentiment_analysis, lda_topic_modeling
+from .text_coding import preprocess_text, vectorize_text, tfidf_vectorize_texts, lda_model, nmf_model, lsa_model, elbow_method_tfidf, sentiment_analysis, lda_topic_modeling
```

### Comparing `Maslib-0.1.4/MasLib/classification.py` & `Maslib-0.1.5/MasLib/classification.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/MasLib/clustering.py` & `Maslib-0.1.5/MasLib/clustering.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/MasLib/correlation.py` & `Maslib-0.1.5/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/MasLib/encoding.py` & `Maslib-0.1.5/MasLib/encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/MasLib/loading.py` & `Maslib-0.1.5/MasLib/loading.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/MasLib/regressions.py` & `Maslib-0.1.5/MasLib/regressions.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/MasLib/text_coding.py` & `Maslib-0.1.5/MasLib/text_coding.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,25 +160,14 @@
     plt.xlabel('Number of Clusters')
     plt.ylabel('Silhouette Score')
     plt.title('Elbow Method for Optimal Number of Clusters')
     plt.xticks(k_range)
     plt.grid(True)
     plt.show()
 
-def bert_topic_modeling(texts,language='english'):
-    """
-    Eng: Topic modeling using BERTopic.
-    Fra: Modélisation thématique à l'aide de BERTopic.
-    Rus: Тематическое моделирование с использованием BERTopic.
-    Ger: Themenmodellierung mit BERTopic.
-    """
-    topic_model = BERTopic(language=language, calculate_probabilities=True, verbose=True, embedding_model='sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2', n_gram_range=(2, 2))
-    topics, probs = topic_model.fit_transform(texts)
-    topic_model.visualize_barchart()
-    return topics, probs
 
 def sentiment_analysis(df, text_column,language='english'):
     """
     Eng: Example of sentiment analysis using a simple SVM classifier.
     Fra: Exemple d'analyse des sentiments à l'aide d'un simple classificateur SVM.
     Rus: Пример анализа настроений с использованием простого классификатора SVM.
     Ger: Beispiel für die Stimmungsanalyse mit einem einfachen SVM-Klassifikator.
```

### Comparing `Maslib-0.1.4/Maslib.egg-info/PKG-INFO` & `Maslib-0.1.5/Maslib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.4
+Version: 0.1.5
 Summary: This is a library for optimizing code for python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -14,16 +14,14 @@
 Requires-Dist: phik
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: joblib
 Requires-Dist: wordcloud
 Requires-Dist: xgboost
-Requires-Dist: bertopic
-Requires-Dist: hdbscan
 
 # MasLib
 
 MasLib - this is a Python library for code reduction
 
 My library can safely optimize everyday tasks for python
```

### Comparing `Maslib-0.1.4/Maslib.egg-info/SOURCES.txt` & `Maslib-0.1.5/Maslib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/PKG-INFO` & `Maslib-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.1.4
+Version: 0.1.5
 Summary: This is a library for optimizing code for python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -14,16 +14,14 @@
 Requires-Dist: phik
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: joblib
 Requires-Dist: wordcloud
 Requires-Dist: xgboost
-Requires-Dist: bertopic
-Requires-Dist: hdbscan
 
 # MasLib
 
 MasLib - this is a Python library for code reduction
 
 My library can safely optimize everyday tasks for python
```

### Comparing `Maslib-0.1.4/setup.py` & `Maslib-0.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'phik',
         'matplotlib',
         'scikit-learn',
         'catboost',
         'joblib',
         'wordcloud',
         'xgboost',
-        'bertopic',
-        'hdbscan'
 
     ],
     author='Alecsandr_C.V.V',
     author_email='dxomko@gmail.com',
     description='This is a library for optimizing code for python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `Maslib-0.1.4/tests/test_clustering.py` & `Maslib-0.1.5/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/tests/test_correlation.py` & `Maslib-0.1.5/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/tests/test_encoding.py` & `Maslib-0.1.5/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/tests/test_grid_search.py` & `Maslib-0.1.5/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/tests/test_regression.py` & `Maslib-0.1.5/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.1.4/tests/test_text_coding.py` & `Maslib-0.1.5/tests/test_text_coding.py`

 * *Files identical despite different names*

