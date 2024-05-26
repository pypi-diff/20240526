# Comparing `tmp/phylokrr-0.4.9.tar.gz` & `tmp/phylokrr-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phylokrr-0.4.9.tar", last modified: Sun May 19 01:50:59 2024, max compression
+gzip compressed data, was "dist/phylokrr-0.5.0.tar", last modified: Sun May 26 19:07:53 2024, max compression
```

## Comparing `phylokrr-0.4.9.tar` & `phylokrr-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-05-19 01:50:59.000000 phylokrr-0.4.9/
--rw-r--r--   0 ulises     (502) staff       (20)      204 2024-05-19 01:50:59.000000 phylokrr-0.4.9/PKG-INFO
--rw-r--r--   0 ulises     (502) staff       (20)     3913 2024-05-19 01:50:12.000000 phylokrr-0.4.9/README.md
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/
--rw-r--r--   0 ulises     (502) staff       (20)      204 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/PKG-INFO
--rw-r--r--   0 ulises     (502) staff       (20)      329 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/SOURCES.txt
--rw-r--r--   0 ulises     (502) staff       (20)        1 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/dependency_links.txt
--rw-r--r--   0 ulises     (502) staff       (20)        1 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/not-zip-safe
--rw-r--r--   0 ulises     (502) staff       (20)        6 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/requires.txt
--rw-r--r--   0 ulises     (502) staff       (20)        9 2024-05-19 01:50:59.000000 phylokrr-0.4.9/phylokrr.egg-info/top_level.txt
--rw-r--r--   0 ulises     (502) staff       (20)       38 2024-05-19 01:50:59.000000 phylokrr-0.4.9/setup.cfg
--rw-r--r--   0 ulises     (502) staff       (20)      656 2024-05-19 01:39:58.000000 phylokrr-0.4.9/setup.py
-drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-05-19 01:50:59.000000 phylokrr-0.4.9/src/
--rw-r--r--   0 ulises     (502) staff       (20)        0 2023-09-27 05:08:48.000000 phylokrr-0.4.9/src/__init__.py
--rw-r--r--   0 ulises     (502) staff       (20)     6916 2024-02-11 02:35:07.000000 phylokrr-0.4.9/src/core.py
--rw-r--r--   0 ulises     (502) staff       (20)     1381 2024-04-28 06:42:39.000000 phylokrr-0.4.9/src/datasets.py
--rw-r--r--   0 ulises     (502) staff       (20)     3106 2024-05-06 19:17:07.000000 phylokrr-0.4.9/src/inspection.py
--rw-r--r--   0 ulises     (502) staff       (20)     8047 2024-05-19 01:09:11.000000 phylokrr-0.4.9/src/kernels.py
--rw-r--r--   0 ulises     (502) staff       (20)      339 2024-02-25 06:38:58.000000 phylokrr-0.4.9/src/metrics.py
--rw-r--r--   0 ulises     (502) staff       (20)    20652 2024-04-23 23:32:36.000000 phylokrr-0.4.9/src/phylosig.py
--rw-r--r--   0 ulises     (502) staff       (20)    16152 2024-04-28 06:39:18.000000 phylokrr-0.4.9/src/utils.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-05-26 19:07:53.000000 phylokrr-0.5.0/
+-rw-r--r--   0 ulises     (502) staff       (20)      204 2024-05-26 19:07:53.000000 phylokrr-0.5.0/PKG-INFO
+-rw-r--r--   0 ulises     (502) staff       (20)     3923 2024-05-26 19:06:35.000000 phylokrr-0.5.0/README.md
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-05-26 19:07:53.000000 phylokrr-0.5.0/phylokrr.egg-info/
+-rw-r--r--   0 ulises     (502) staff       (20)      204 2024-05-26 19:07:53.000000 phylokrr-0.5.0/phylokrr.egg-info/PKG-INFO
+-rw-r--r--   0 ulises     (502) staff       (20)      329 2024-05-26 19:07:53.000000 phylokrr-0.5.0/phylokrr.egg-info/SOURCES.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        1 2024-05-26 19:07:53.000000 phylokrr-0.5.0/phylokrr.egg-info/dependency_links.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        1 2024-05-26 17:57:07.000000 phylokrr-0.5.0/phylokrr.egg-info/not-zip-safe
+-rw-r--r--   0 ulises     (502) staff       (20)        6 2024-05-26 19:07:53.000000 phylokrr-0.5.0/phylokrr.egg-info/requires.txt
+-rw-r--r--   0 ulises     (502) staff       (20)        9 2024-05-26 19:07:53.000000 phylokrr-0.5.0/phylokrr.egg-info/top_level.txt
+-rw-r--r--   0 ulises     (502) staff       (20)       38 2024-05-26 19:07:53.000000 phylokrr-0.5.0/setup.cfg
+-rw-r--r--   0 ulises     (502) staff       (20)      656 2024-05-26 19:07:22.000000 phylokrr-0.5.0/setup.py
+drwxr-xr-x   0 ulises     (502) staff       (20)        0 2024-05-26 19:07:53.000000 phylokrr-0.5.0/src/
+-rw-r--r--   0 ulises     (502) staff       (20)        0 2023-09-27 05:08:48.000000 phylokrr-0.5.0/src/__init__.py
+-rw-r--r--   0 ulises     (502) staff       (20)     6916 2024-02-11 02:35:07.000000 phylokrr-0.5.0/src/core.py
+-rw-r--r--   0 ulises     (502) staff       (20)     4509 2024-05-26 18:01:34.000000 phylokrr-0.5.0/src/datasets.py
+-rw-r--r--   0 ulises     (502) staff       (20)     3392 2024-05-21 16:08:05.000000 phylokrr-0.5.0/src/inspection.py
+-rw-r--r--   0 ulises     (502) staff       (20)     8047 2024-05-19 01:09:11.000000 phylokrr-0.5.0/src/kernels.py
+-rw-r--r--   0 ulises     (502) staff       (20)      339 2024-02-25 06:38:58.000000 phylokrr-0.5.0/src/metrics.py
+-rw-r--r--   0 ulises     (502) staff       (20)     3408 2024-05-22 14:25:11.000000 phylokrr-0.5.0/src/phylosig.py
+-rw-r--r--   0 ulises     (502) staff       (20)    13258 2024-05-26 18:00:23.000000 phylokrr-0.5.0/src/utils.py
```

### Comparing `phylokrr-0.4.9/README.md` & `phylokrr-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -123,10 +123,10 @@
 ```
 
 <p align="center">
 <img src="https://github.com/Ulises-Rosas/phylokrr/blob/main/data/imgs/phyloKRR_vs_PGLS_cv.png" alt="drawing" width="600px"/>
 </p>
  -->
 
-# Reference
+<!--  # Reference
 
-Rosas-Puchuri, U., Santaquiteria, A., Khanmohammadi, S., Solis-Lemus, C., & Betancur-R, R. (2023). [Non-linear phylogenetic regression using regularized kernels](https://www.biorxiv.org/content/10.1101/2023.10.04.560983v1.abstract). bioRxiv, 2023-10.
+Rosas-Puchuri, U., Santaquiteria, A., Khanmohammadi, S., Solis-Lemus, C., & Betancur-R, R. (2023). [Non-linear phylogenetic regression using regularized kernels](https://www.biorxiv.org/content/10.1101/2023.10.04.560983v1.abstract). bioRxiv, 2023-10. -->
```

### Comparing `phylokrr-0.4.9/setup.py` & `phylokrr-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "numpy"
 ]
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(name = "phylokrr",
-      version = '0.4.9',
+      version = '0.5.0',
     #   long_description = readme,
     #   long_description_content_type = 'text/markdown',
       packages = ['phylokrr'],
       package_dir = {'phylokrr': 'src'},
       python_requires='>=3.5',
       install_requires = dependencies,
       zip_safe = False,
```

### Comparing `phylokrr-0.4.9/src/core.py` & `phylokrr-0.5.0/src/core.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.9/src/inspection.py` & `phylokrr-0.5.0/src/inspection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 
 import numpy as np
 from phylokrr.utils import split_data
 
 def permutation_importance(X, y, model, num_test = 100, seed = 12038, iterations = 1000):
+    """
+    Permutation importance
+
+    X: data
+    y: target
+    model: model
+    num_test: number of test samples
+    seed: random seed
+    iterations: number of iterations
+
+    returns: Feature importance for all features. 
+        Each column represents the change in error
+    """
 
     np.random.seed(seed)
 
     n,p = X.shape
 
     X_train, X_test, y_train,y_test = split_data(X, y, num_test, seed = seed)
     model.fit(X_train, y_train)
```

### Comparing `phylokrr-0.4.9/src/kernels.py` & `phylokrr-0.5.0/src/kernels.py`

 * *Files identical despite different names*

### Comparing `phylokrr-0.4.9/src/utils.py` & `phylokrr-0.5.0/src/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -308,14 +308,18 @@
 
         if self.fit_intercept:
             X = np.hstack((np.ones((n,1)), X))
 
         self.beta = np.linalg.solve(X.T @ X, X.T @ y)
 
     def fit(self, X, y, vcv=None):
+        """
+        if vcv is not None, then we use phylogenetic covariance matrix
+        for Generalized Least Squares. Otherwise, we use Ordinary Least Squares
+        """
 
         if vcv is not None:
             self.std_PGLS(X, y, vcv)
 
         else:
             self.OLS(X, y)
 
@@ -379,119 +383,14 @@
         y =  np.sum(x, axis=1) ** b
 
     if add_noise:
         y += noise
 
     return y
 
-def sim_data(vcv, mean_vector, b, 
-             on_weighted=True, 
-             add_noise = True, 
-             noise_var = 1,
-             n_var = 3, 
-             extra_weights = [], 
-             type='pol',
-             weight_with_vcv = True,
-             vcv2 = None
-             ):
-    """
-    Simulate data for n_var independent variables
-
-    Parameters
-    ----------
-    vcv: np.array
-        covariance matrix where data is simulated from
-    
-    mean_vector: np.array
-        mean vector
-    
-    b: int
-        power of the polynomial function
-
-    on_weighted: bool
-        whether to use weighted data or not to obtain the response variable.
-        the weights are obtained using the 
-        squared root of the inverse of 
-        the covariance matrix
-
-    add_noise: bool
-        whether to add noise to the response variable
-
-    noise_var: float
-        variance of the noise
-
-    extra_weights: list
-        weights for the independent variables
-
-    type: str
-        type of the function to simulate the data
-        if 'sin' then a sine function is used over the
-        sum of the independent variables
-        if 'pol' then a polynomial function is used over the
-        sum of the independent variables
-    
-    weight_with_vcv: bool
-        if true (default) the weighting of the values is 
-        done using vcv. Otherwise, vcv2 is used
-
-    vcv2: np.array
-        if weight_with_vcv is false, then we use this covariance matrix
-        to weight the data
-    
-    Returns
-    -------
-    X_w_uc: np.array
-        weighted independent variables (uncentered)
-    
-    y_w_uc: np.array
-        weighted response variable (uncentered)
-    """
-    # n_var = 1
-    # mean_vector = np.zeros(vcv.shape[0])
-    # b = 3
-    n = vcv.shape[0]
-    if len(extra_weights):
-        assert len(extra_weights) == n_var, "extra weights must have the same length as the number of predictors"
-    
-    else:
-        extra_weights = np.ones(n_var)
-
-    X_uw_uc = np.zeros((n, n_var))
-    for j in range(n_var):
-        X_uw_uc[:,j] = np.random.multivariate_normal(mean=mean_vector, cov=vcv)*extra_weights[j]
-    
-    if add_noise:
-        noise = np.random.normal(0, noise_var, n)
-
-    if weight_with_vcv:
-        P = P_mat_simple(vcv)
-
-    else:
-        assert isinstance(vcv2, np.ndarray), 'vcv2 must be a numpy array'
-        P = P_mat_simple(vcv2)
-
-    if on_weighted:
-        X_w_uc = P @ X_uw_uc
-        # the variance and expectation 
-        # of the response variable will depend on the moment 
-        # that generates b. V(x^b) = E(x^2b) - E(x^b)^2
-        # E(x^b) is the expectation in the moment b.
-        # Both the expectation and variance are point estimates
-        y_w_uc = myfunc(X_w_uc, b=b, type=type, 
-                        add_noise=add_noise,
-                        noise=noise).ravel()
-    else:
-        y_uw_uc = myfunc(X_uw_uc, b=b, type=type, 
-                         add_noise=add_noise, 
-                         noise=noise).ravel()
-
-        X_w_uc = P @ X_uw_uc
-        y_w_uc = P @ y_uw_uc
-
-    return X_w_uc, y_w_uc
 
 def get_Xy_w_uc(X_uw_uc, P, b, type, on_weighted, add_noise, noise):    
 
     if on_weighted:
 
         X_w_uc = P @ X_uw_uc
         y_w_uc = myfunc(X_w_uc, b=b, type=type).ravel()
```

