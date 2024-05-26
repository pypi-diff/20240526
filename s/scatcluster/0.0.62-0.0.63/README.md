# Comparing `tmp/scatcluster-0.0.62.tar.gz` & `tmp/scatcluster-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.62.tar", last modified: Sun May 26 19:15:28 2024, max compression
+gzip compressed data, was "scatcluster-0.0.63.tar", last modified: Sun May 26 19:28:55 2024, max compression
```

## Comparing `scatcluster-0.0.62.tar` & `scatcluster-0.0.63.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:15:28.236158 scatcluster-0.0.62/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-26 19:15:24.000000 scatcluster-0.0.62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 19:15:24.000000 scatcluster-0.0.62/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 19:15:28.236158 scatcluster-0.0.62/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:15:28.232158 scatcluster-0.0.62/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:15:28.236158 scatcluster-0.0.62/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:15:28.236158 scatcluster-0.0.62/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16096 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    24715 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-26 19:15:24.000000 scatcluster-0.0.62/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:15:28.236158 scatcluster-0.0.62/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 19:15:28.000000 scatcluster-0.0.62/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-26 19:15:28.000000 scatcluster-0.0.62/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:15:28.000000 scatcluster-0.0.62/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-26 19:15:28.000000 scatcluster-0.0.62/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 19:15:28.000000 scatcluster-0.0.62/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 19:15:28.236158 scatcluster-0.0.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-26 19:15:25.000000 scatcluster-0.0.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:28:55.744891 scatcluster-0.0.63/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-26 19:28:52.000000 scatcluster-0.0.63/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 19:28:52.000000 scatcluster-0.0.63/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 19:28:55.744891 scatcluster-0.0.63/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:28:55.740891 scatcluster-0.0.63/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:28:55.740891 scatcluster-0.0.63/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:28:55.744891 scatcluster-0.0.63/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24715 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-26 19:28:52.000000 scatcluster-0.0.63/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 19:28:55.744891 scatcluster-0.0.63/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 19:28:55.000000 scatcluster-0.0.63/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-26 19:28:55.000000 scatcluster-0.0.63/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 19:28:55.000000 scatcluster-0.0.63/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-26 19:28:55.000000 scatcluster-0.0.63/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 19:28:55.000000 scatcluster-0.0.63/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 19:28:55.744891 scatcluster-0.0.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-26 19:28:52.000000 scatcluster-0.0.63/setup.py
```

### Comparing `scatcluster-0.0.62/LICENSE` & `scatcluster-0.0.63/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/PKG-INFO` & `scatcluster-0.0.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.62
+Version: 0.0.63
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.62/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.63/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.63/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.63/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/analysis/predictions.py` & `scatcluster-0.0.63/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/analysis/processing.py` & `scatcluster-0.0.63/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.63/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.63/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/helper.py` & `scatcluster-0.0.63/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/processing/ica.py` & `scatcluster-0.0.63/scatcluster/processing/ica.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
                     f'Timestamp {UTCDateTime(ts)} - '
                     f'{UTCDateTime(ts) + (self.network_segment * exclude_timestamps_skip)} has been excluded from the '
                     f'Scaling fit and Model fit.')
                 ts_index = self._get_index_from_UTC_timestamp(ts)
                 scat_coeff_data = np.delete(scat_coeff_data, np.s_[ts_index:ts_index + exclude_timestamps_skip], 0)
 
         print('Fitting FastICA')
+        model.fit(scat_coeff_data)
         features = model.transform(scat_coeff_data)
 
         features_inverse = model.inverse_transform(features)
         score_exp_var = explained_variance_score(scat_coeff_data, features_inverse)
         score_mse = mean_squared_error(scat_coeff_data, features_inverse)
         print(f'      ICAs #{num_ICA}: Explained Variance {score_exp_var * 100:0.5f}%: MSE {score_mse:0.5f}')
```

### Comparing `scatcluster-0.0.62/scatcluster/processing/scattering.py` & `scatcluster-0.0.63/scatcluster/processing/scattering.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/scatcluster.py` & `scatcluster-0.0.63/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster/structure.py` & `scatcluster-0.0.63/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.63/scatcluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.62
+Version: 0.0.63
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.62/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.63/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.62/setup.py` & `scatcluster-0.0.63/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.62',
+    version='0.0.63',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

