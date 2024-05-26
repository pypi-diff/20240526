# Comparing `tmp/ImbalancedLearningRegression-0.0.1.tar.gz` & `tmp/imbalancedlearningregression-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImbalancedLearningRegression-0.0.1.tar", last modified: Tue May  3 19:39:37 2022, max compression
+gzip compressed data, was "imbalancedlearningregression-0.0.2.tar", last modified: Sun May 26 03:36:49 2024, max compression
```

## Comparing `ImbalancedLearningRegression-0.0.1.tar` & `imbalancedlearningregression-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,45 @@
-drwxrwxrwx   0        0        0        0 2022-05-03 19:39:37.944390 ImbalancedLearningRegression-0.0.1/
-drwxrwxrwx   0        0        0        0 2022-05-03 19:39:37.931390 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/
--rw-rw-rw-   0        0        0     1028 2022-04-03 23:56:10.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/__init__.py
--rw-rw-rw-   0        0        0    15918 2022-05-03 16:12:51.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/adasyn.py
--rw-rw-rw-   0        0        0     3350 2020-04-04 06:27:42.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/box_plot_stats.py
--rw-rw-rw-   0        0        0    10589 2022-04-27 03:14:37.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/cnn.py
--rw-rw-rw-   0        0        0     3577 2020-04-04 06:27:42.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/dist_metrics.py
--rw-rw-rw-   0        0        0    10341 2022-04-27 03:14:47.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/enn.py
--rw-rw-rw-   0        0        0    12628 2022-03-20 23:22:58.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/gn.py
--rw-rw-rw-   0        0        0    10298 2022-05-03 16:12:51.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/over_sampling_adasyn.py
--rw-rw-rw-   0        0        0     8490 2022-03-21 17:49:02.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/over_sampling_gn.py
--rw-rw-rw-   0        0        0     7676 2022-03-21 17:51:27.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/over_sampling_ro.py
--rw-rw-rw-   0        0        0    14467 2022-05-03 16:12:51.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/over_sampling_smote.py
--rw-rw-rw-   0        0        0     5222 2020-04-04 06:27:42.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/phi.py
--rw-rw-rw-   0        0        0     7209 2022-03-20 22:55:53.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/phi_ctrl_pts.py
--rw-rw-rw-   0        0        0    10462 2022-04-28 14:43:58.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/random_under.py
--rw-rw-rw-   0        0        0    11273 2022-03-20 23:24:18.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/ro.py
--rw-rw-rw-   0        0        0     9994 2022-04-27 14:47:34.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/smote.py
--rw-rw-rw-   0        0        0     8108 2022-05-03 16:12:51.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/tomeklinks.py
--rw-rw-rw-   0        0        0     8268 2022-05-03 16:12:51.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/under_sampling_cnn.py
--rw-rw-rw-   0        0        0     6121 2022-04-07 01:33:59.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/under_sampling_enn.py
--rw-rw-rw-   0        0        0     7027 2022-05-03 16:12:51.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/under_sampling_random.py
--rw-rw-rw-   0        0        0    11042 2022-05-03 16:12:51.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/under_sampling_tomeklinks.py
-drwxrwxrwx   0        0        0        0 2022-05-03 19:39:37.943390 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression.egg-info/
--rw-rw-rw-   0        0        0     7103 2022-05-03 19:39:37.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2022-05-03 19:39:37.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-03 19:39:37.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2022-05-03 19:39:37.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2022-05-03 19:39:37.000000 ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35149 2020-04-04 06:27:42.000000 ImbalancedLearningRegression-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       50 2022-01-30 17:45:15.000000 ImbalancedLearningRegression-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7103 2022-05-03 19:39:37.944390 ImbalancedLearningRegression-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5944 2022-05-03 18:56:19.000000 ImbalancedLearningRegression-0.0.1/README.md
--rw-rw-rw-   0        0        0      949 2022-05-03 16:12:51.000000 ImbalancedLearningRegression-0.0.1/UPDATES
--rw-rw-rw-   0        0        0       42 2022-05-03 19:39:37.945392 ImbalancedLearningRegression-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1544 2022-04-03 23:56:02.000000 ImbalancedLearningRegression-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:36:49.498624 imbalancedlearningregression-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-26 03:36:49.471476 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/
+-rw-rw-rw-   0        0        0     1028 2024-05-26 03:31:04.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/__init__.py
+-rw-rw-rw-   0        0        0    15918 2022-05-03 16:12:51.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/adasyn.py
+-rw-rw-rw-   0        0        0     3350 2020-04-04 06:27:42.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/box_plot_stats.py
+-rw-rw-rw-   0        0        0    10589 2022-04-27 03:14:37.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/cnn.py
+-rw-rw-rw-   0        0        0     3577 2020-04-04 06:27:42.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/dist_metrics.py
+-rw-rw-rw-   0        0        0    10341 2022-04-27 03:14:47.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/enn.py
+-rw-rw-rw-   0        0        0    12628 2022-03-20 23:22:58.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/gn.py
+-rw-rw-rw-   0        0        0    10298 2022-05-03 16:12:51.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/over_sampling_adasyn.py
+-rw-rw-rw-   0        0        0     8490 2022-03-21 17:49:02.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/over_sampling_gn.py
+-rw-rw-rw-   0        0        0     7676 2022-03-21 17:51:27.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/over_sampling_ro.py
+-rw-rw-rw-   0        0        0    14467 2022-05-03 16:12:51.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/over_sampling_smote.py
+-rw-rw-rw-   0        0        0     5222 2020-04-04 06:27:42.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/phi.py
+-rw-rw-rw-   0        0        0     7209 2022-03-20 22:55:53.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/phi_ctrl_pts.py
+-rw-rw-rw-   0        0        0    10462 2022-04-28 14:43:58.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/random_under.py
+-rw-rw-rw-   0        0        0    11273 2022-03-20 23:24:18.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/ro.py
+-rw-rw-rw-   0        0        0     9994 2022-04-27 14:47:34.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/smote.py
+-rw-rw-rw-   0        0        0     8108 2022-05-03 16:12:51.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/tomeklinks.py
+-rw-rw-rw-   0        0        0     8268 2022-05-03 16:12:51.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/under_sampling_cnn.py
+-rw-rw-rw-   0        0        0     6121 2022-04-07 01:33:59.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/under_sampling_enn.py
+-rw-rw-rw-   0        0        0     7027 2022-05-03 16:12:51.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/under_sampling_random.py
+-rw-rw-rw-   0        0        0    11042 2022-05-03 16:12:51.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/under_sampling_tomeklinks.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:36:49.496731 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression.egg-info/
+-rw-rw-rw-   0        0        0     8021 2024-05-26 03:36:49.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1396 2024-05-26 03:36:49.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 03:36:49.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-26 03:36:49.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-26 03:36:49.000000 imbalancedlearningregression-0.0.2/ImbalancedLearningRegression.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35149 2020-04-04 06:27:42.000000 imbalancedlearningregression-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       50 2022-01-30 17:45:15.000000 imbalancedlearningregression-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     8021 2024-05-26 03:36:49.497235 imbalancedlearningregression-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6808 2024-05-26 00:19:36.000000 imbalancedlearningregression-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1083 2024-05-26 03:29:32.000000 imbalancedlearningregression-0.0.2/UPDATES
+-rw-rw-rw-   0        0        0       42 2024-05-26 03:36:49.499629 imbalancedlearningregression-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1593 2024-05-26 03:29:43.000000 imbalancedlearningregression-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:36:49.495726 imbalancedlearningregression-0.0.2/tests/
+-rw-rw-rw-   0        0        0     3407 2022-04-28 01:59:39.000000 imbalancedlearningregression-0.0.2/tests/test_adasyn.py
+-rw-rw-rw-   0        0        0     4792 2022-04-25 03:47:15.000000 imbalancedlearningregression-0.0.2/tests/test_cnn.py
+-rw-rw-rw-   0        0        0     4249 2022-04-25 03:56:56.000000 imbalancedlearningregression-0.0.2/tests/test_enn.py
+-rw-rw-rw-   0        0        0     4638 2022-04-25 03:45:33.000000 imbalancedlearningregression-0.0.2/tests/test_gn.py
+-rw-rw-rw-   0        0        0     3449 2022-04-25 03:44:42.000000 imbalancedlearningregression-0.0.2/tests/test_ro.py
+-rw-rw-rw-   0        0        0     3746 2022-04-28 13:34:02.000000 imbalancedlearningregression-0.0.2/tests/test_ru.py
+-rw-rw-rw-   0        0        0     3380 2022-04-28 01:55:35.000000 imbalancedlearningregression-0.0.2/tests/test_smote.py
+-rw-rw-rw-   0        0        0     2951 2022-04-28 13:39:39.000000 imbalancedlearningregression-0.0.2/tests/test_tomeklinks.py
```

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/__init__.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # __init__.py
 
 # Version of the ImbalancedLearningRegression package
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 """
 Imbalanced Learning for Regression
 https://github.com/paobranco/ImbalancedLearningRegression
 """
 
 from ImbalancedLearningRegression.box_plot_stats import box_plot_stats
```

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/adasyn.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/adasyn.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/box_plot_stats.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/box_plot_stats.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/cnn.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/cnn.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/dist_metrics.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/dist_metrics.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/enn.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/enn.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/gn.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/gn.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/over_sampling_adasyn.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/over_sampling_adasyn.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/over_sampling_gn.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/over_sampling_gn.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/over_sampling_ro.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/over_sampling_ro.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/over_sampling_smote.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/over_sampling_smote.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/phi.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/phi.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/phi_ctrl_pts.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/phi_ctrl_pts.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/random_under.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/random_under.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/ro.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/ro.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/smote.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/smote.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/tomeklinks.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/tomeklinks.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/under_sampling_cnn.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/under_sampling_cnn.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/under_sampling_enn.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/under_sampling_enn.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/under_sampling_random.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/under_sampling_random.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression/under_sampling_tomeklinks.py` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression/under_sampling_tomeklinks.py`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression.egg-info/PKG-INFO` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,60 @@
 Metadata-Version: 2.1
 Name: ImbalancedLearningRegression
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementations of preprocesssing imbalanced data for regression
 Home-page: https://github.com/paobranco/ImbalancedLearningRegression
 Author: Paula Branco, Wenglei Wu, Alex Chengen Lyu, Lingyi Kong, Gloria Hu
 Author-email: pbranco@uottawa.ca, wwu077@uottawa.ca, clyu039@uottawa.ca, lkong073@uottawa.ca, xhu005@uottawa.ca
-License: UNKNOWN
 Keywords: smote,Gaussian noise,condensed nearest neighbour,edited nearest neighbour,Tomek links,ADASYN,over-sampling,under-sampling,synthetic data,imbalanced data,pre-processing,regression
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: tqdm
+Requires-Dist: scikit-learn
 
 
 ## Imbalanced Learning Regression
 [![PyPI version](https://badge.fury.io/py/ImbalancedLearningRegression.svg)](https://badge.fury.io/py/ImbalancedLearningRegression)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![GitHub last commit](https://img.shields.io/github/last-commit/paobranco/ImbalancedLearningRegression)
 
 ## Description
 A Python implementation of sampling techniques for Regression. Conducts different sampling techniques for Regression. Useful for prediction problems where regression is applicable, but the values in the interest of predicting are rare or uncommon. This can also serve as a useful alternative to log transforming a skewed response variable, especially if generating synthetic data is also of interest.
 <br>
 
+## Citation
+If you use the code from this repository, please cite the following article:
+
+*Wu, W., Kunz, N., & Branco, P. (2022, September). ImbalancedLearningRegression-A Python Package to Tackle the Imbalanced Regression Problem. In Joint European Conference on Machine Learning and Knowledge Discovery in Databases (pp. 645-648). Cham: Springer Nature Switzerland.*
+
+For bibtex users:
+
+@inproceedings{wu2022imbalancedlearningregression,
+  title={ImbalancedLearningRegression-A Python Package to Tackle the Imbalanced Regression Problem},
+  author={Wu, Wenglei and Kunz, Nicholas and Branco, Paula},
+  booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
+  pages={645--648},
+  year={2022},
+  organization={Springer}
+}
+
+Article Link: 
+https://link.springer.com/chapter/10.1007/978-3-031-26422-1_48
+
+
 ## Features
 1. An open-source Python supported version of sampling techniques for Regression, a variation of Nick Kunz's package SMOGN.
 
 2. Supports Pandas DataFrame inputs containing mixed data types.
 
 3. Flexible inputs available to control the areas of interest within a continuous response variable and friendly parameters for re-sampling data.
 
@@ -120,9 +142,7 @@
 Torgo, L., Ribeiro, R. P., Pfahringer, B., & Branco, P. (2013, September). Smote for regression. In Portuguese conference on artificial intelligence (pp. 378-389). Springer, Berlin, Heidelberg. https://link.springer.com/chapter/10.1007/978-3-642-40669-0_33
 
 Wilson, D. L. (1972). Asymptotic properties of nearest neighbor rules using edited data. IEEE Transactions on Systems, Man, and Cybernetics, (3), 408-421. https://ieeexplore.ieee.org/abstract/document/4309137
 
 
 
 
-
-
```

### Comparing `ImbalancedLearningRegression-0.0.1/ImbalancedLearningRegression.egg-info/SOURCES.txt` & `imbalancedlearningregression-0.0.2/ImbalancedLearningRegression.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -24,8 +24,16 @@
 ImbalancedLearningRegression/under_sampling_enn.py
 ImbalancedLearningRegression/under_sampling_random.py
 ImbalancedLearningRegression/under_sampling_tomeklinks.py
 ImbalancedLearningRegression.egg-info/PKG-INFO
 ImbalancedLearningRegression.egg-info/SOURCES.txt
 ImbalancedLearningRegression.egg-info/dependency_links.txt
 ImbalancedLearningRegression.egg-info/requires.txt
-ImbalancedLearningRegression.egg-info/top_level.txt
+ImbalancedLearningRegression.egg-info/top_level.txt
+tests/test_adasyn.py
+tests/test_cnn.py
+tests/test_enn.py
+tests/test_gn.py
+tests/test_ro.py
+tests/test_ru.py
+tests/test_smote.py
+tests/test_tomeklinks.py
```

### Comparing `ImbalancedLearningRegression-0.0.1/LICENSE` & `imbalancedlearningregression-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ImbalancedLearningRegression-0.0.1/PKG-INFO` & `imbalancedlearningregression-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,60 @@
 Metadata-Version: 2.1
 Name: ImbalancedLearningRegression
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementations of preprocesssing imbalanced data for regression
 Home-page: https://github.com/paobranco/ImbalancedLearningRegression
 Author: Paula Branco, Wenglei Wu, Alex Chengen Lyu, Lingyi Kong, Gloria Hu
 Author-email: pbranco@uottawa.ca, wwu077@uottawa.ca, clyu039@uottawa.ca, lkong073@uottawa.ca, xhu005@uottawa.ca
-License: UNKNOWN
 Keywords: smote,Gaussian noise,condensed nearest neighbour,edited nearest neighbour,Tomek links,ADASYN,over-sampling,under-sampling,synthetic data,imbalanced data,pre-processing,regression
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: tqdm
+Requires-Dist: scikit-learn
 
 
 ## Imbalanced Learning Regression
 [![PyPI version](https://badge.fury.io/py/ImbalancedLearningRegression.svg)](https://badge.fury.io/py/ImbalancedLearningRegression)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![GitHub last commit](https://img.shields.io/github/last-commit/paobranco/ImbalancedLearningRegression)
 
 ## Description
 A Python implementation of sampling techniques for Regression. Conducts different sampling techniques for Regression. Useful for prediction problems where regression is applicable, but the values in the interest of predicting are rare or uncommon. This can also serve as a useful alternative to log transforming a skewed response variable, especially if generating synthetic data is also of interest.
 <br>
 
+## Citation
+If you use the code from this repository, please cite the following article:
+
+*Wu, W., Kunz, N., & Branco, P. (2022, September). ImbalancedLearningRegression-A Python Package to Tackle the Imbalanced Regression Problem. In Joint European Conference on Machine Learning and Knowledge Discovery in Databases (pp. 645-648). Cham: Springer Nature Switzerland.*
+
+For bibtex users:
+
+@inproceedings{wu2022imbalancedlearningregression,
+  title={ImbalancedLearningRegression-A Python Package to Tackle the Imbalanced Regression Problem},
+  author={Wu, Wenglei and Kunz, Nicholas and Branco, Paula},
+  booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
+  pages={645--648},
+  year={2022},
+  organization={Springer}
+}
+
+Article Link: 
+https://link.springer.com/chapter/10.1007/978-3-031-26422-1_48
+
+
 ## Features
 1. An open-source Python supported version of sampling techniques for Regression, a variation of Nick Kunz's package SMOGN.
 
 2. Supports Pandas DataFrame inputs containing mixed data types.
 
 3. Flexible inputs available to control the areas of interest within a continuous response variable and friendly parameters for re-sampling data.
 
@@ -120,9 +142,7 @@
 Torgo, L., Ribeiro, R. P., Pfahringer, B., & Branco, P. (2013, September). Smote for regression. In Portuguese conference on artificial intelligence (pp. 378-389). Springer, Berlin, Heidelberg. https://link.springer.com/chapter/10.1007/978-3-642-40669-0_33
 
 Wilson, D. L. (1972). Asymptotic properties of nearest neighbor rules using edited data. IEEE Transactions on Systems, Man, and Cybernetics, (3), 408-421. https://ieeexplore.ieee.org/abstract/document/4309137
 
 
 
 
-
-
```

### Comparing `ImbalancedLearningRegression-0.0.1/README.md` & `imbalancedlearningregression-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,34 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![GitHub last commit](https://img.shields.io/github/last-commit/paobranco/ImbalancedLearningRegression)
 
 ## Description
 A Python implementation of sampling techniques for Regression. Conducts different sampling techniques for Regression. Useful for prediction problems where regression is applicable, but the values in the interest of predicting are rare or uncommon. This can also serve as a useful alternative to log transforming a skewed response variable, especially if generating synthetic data is also of interest.
 <br>
 
+## Citation
+If you use the code from this repository, please cite the following article:
+
+*Wu, W., Kunz, N., & Branco, P. (2022, September). ImbalancedLearningRegression-A Python Package to Tackle the Imbalanced Regression Problem. In Joint European Conference on Machine Learning and Knowledge Discovery in Databases (pp. 645-648). Cham: Springer Nature Switzerland.*
+
+For bibtex users:
+
+@inproceedings{wu2022imbalancedlearningregression,
+  title={ImbalancedLearningRegression-A Python Package to Tackle the Imbalanced Regression Problem},
+  author={Wu, Wenglei and Kunz, Nicholas and Branco, Paula},
+  booktitle={Joint European Conference on Machine Learning and Knowledge Discovery in Databases},
+  pages={645--648},
+  year={2022},
+  organization={Springer}
+}
+
+Article Link: 
+https://link.springer.com/chapter/10.1007/978-3-031-26422-1_48
+
+
 ## Features
 1. An open-source Python supported version of sampling techniques for Regression, a variation of Nick Kunz's package SMOGN.
 
 2. Supports Pandas DataFrame inputs containing mixed data types.
 
 3. Flexible inputs available to control the areas of interest within a continuous response variable and friendly parameters for re-sampling data.
```

### Comparing `ImbalancedLearningRegression-0.0.1/UPDATES` & `imbalancedlearningregression-0.0.2/UPDATES`

 * *Files 7% similar despite different names*

```diff
@@ -18,7 +18,11 @@
 - Check the code of the eight re-sampling methods
 - Write tests
 - Write "read the docs" documentation
 - Re-organize the Github repository
 - Write a 4-page thesis of description
 - Published the package to PyPI
 
+ImbalancedLearningRegression-0.0.2: 2024-05-25
+==========================
+- Replace the dependency "sklearn" with "scikit-learn"
+
```

