# Comparing `tmp/dsgepy-0.1.tar.gz` & `tmp/dsgepy-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsgepy-0.1.tar", last modified: Fri Dec 30 13:29:42 2022, max compression
+gzip compressed data, was "dsgepy-1.0.tar", last modified: Sun May 26 19:06:21 2024, max compression
```

## Comparing `dsgepy-0.1.tar` & `dsgepy-1.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 gusamarante   (501) staff       (20)        0 2022-12-30 13:29:42.608751 dsgepy-0.1/
--rw-r--r--   0 gusamarante   (501) staff       (20)     1073 2022-12-30 12:31:40.000000 dsgepy-0.1/LICENSE
--rw-r--r--   0 gusamarante   (501) staff       (20)     4265 2022-12-30 13:29:42.608138 dsgepy-0.1/PKG-INFO
--rw-r--r--   0 gusamarante   (501) staff       (20)     4012 2022-12-30 13:22:06.000000 dsgepy-0.1/README.md
-drwxr-xr-x   0 gusamarante   (501) staff       (20)        0 2022-12-30 13:29:42.603263 dsgepy-0.1/dsgepy/
--rw-r--r--   0 gusamarante   (501) staff       (20)      146 2022-12-30 12:31:40.000000 dsgepy-0.1/dsgepy/__init__.py
--rw-r--r--   0 gusamarante   (501) staff       (20)     2356 2022-12-30 12:31:40.000000 dsgepy-0.1/dsgepy/apifred.py
--rw-r--r--   0 gusamarante   (501) staff       (20)    40540 2022-12-30 12:41:56.000000 dsgepy-0.1/dsgepy/lineardsge.py
--rw-r--r--   0 gusamarante   (501) staff       (20)    14556 2022-12-30 12:41:56.000000 dsgepy-0.1/dsgepy/pycsminwel.py
-drwxr-xr-x   0 gusamarante   (501) staff       (20)        0 2022-12-30 13:29:42.607169 dsgepy-0.1/dsgepy.egg-info/
--rw-r--r--   0 gusamarante   (501) staff       (20)     4265 2022-12-30 13:29:42.000000 dsgepy-0.1/dsgepy.egg-info/PKG-INFO
--rw-r--r--   0 gusamarante   (501) staff       (20)      254 2022-12-30 13:29:42.000000 dsgepy-0.1/dsgepy.egg-info/SOURCES.txt
--rw-r--r--   0 gusamarante   (501) staff       (20)        1 2022-12-30 13:29:42.000000 dsgepy-0.1/dsgepy.egg-info/dependency_links.txt
--rw-r--r--   0 gusamarante   (501) staff       (20)       41 2022-12-30 13:29:42.000000 dsgepy-0.1/dsgepy.egg-info/requires.txt
--rw-r--r--   0 gusamarante   (501) staff       (20)        7 2022-12-30 13:29:42.000000 dsgepy-0.1/dsgepy.egg-info/top_level.txt
--rw-r--r--   0 gusamarante   (501) staff       (20)       38 2022-12-30 13:29:42.608953 dsgepy-0.1/setup.cfg
--rw-r--r--   0 gusamarante   (501) staff       (20)      848 2022-12-30 13:23:43.000000 dsgepy-0.1/setup.py
+drwxr-xr-x   0 gustavoamarante   (501) staff       (20)        0 2024-05-26 19:06:21.075528 dsgepy-1.0/
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)     1073 2024-05-26 18:26:37.000000 dsgepy-1.0/LICENSE
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)     4218 2024-05-26 19:06:21.075264 dsgepy-1.0/PKG-INFO
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)     3834 2024-05-26 18:57:47.000000 dsgepy-1.0/README.md
+drwxr-xr-x   0 gustavoamarante   (501) staff       (20)        0 2024-05-26 19:06:21.073438 dsgepy-1.0/dsgepy/
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)      159 2024-05-26 18:57:47.000000 dsgepy-1.0/dsgepy/__init__.py
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)     5855 2024-05-26 18:57:47.000000 dsgepy-1.0/dsgepy/data_api.py
+drwxr-xr-x   0 gustavoamarante   (501) staff       (20)        0 2024-05-26 19:06:21.074802 dsgepy-1.0/dsgepy/kalman/
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)       61 2024-05-26 18:57:47.000000 dsgepy-1.0/dsgepy/kalman/__init__.py
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)    60878 2024-05-26 18:57:47.000000 dsgepy-1.0/dsgepy/kalman/kalman.py
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)     6355 2024-05-26 18:57:47.000000 dsgepy-1.0/dsgepy/kalman/utils.py
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)    41913 2024-05-26 18:57:47.000000 dsgepy-1.0/dsgepy/lineardsge.py
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)    14556 2024-05-26 18:26:37.000000 dsgepy-1.0/dsgepy/pycsminwel.py
+drwxr-xr-x   0 gustavoamarante   (501) staff       (20)        0 2024-05-26 19:06:21.074995 dsgepy-1.0/dsgepy.egg-info/
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)     4218 2024-05-26 19:06:21.000000 dsgepy-1.0/dsgepy.egg-info/PKG-INFO
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)      328 2024-05-26 19:06:21.000000 dsgepy-1.0/dsgepy.egg-info/SOURCES.txt
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)        1 2024-05-26 19:06:21.000000 dsgepy-1.0/dsgepy.egg-info/dependency_links.txt
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)       41 2024-05-26 19:06:21.000000 dsgepy-1.0/dsgepy.egg-info/requires.txt
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)        7 2024-05-26 19:06:21.000000 dsgepy-1.0/dsgepy.egg-info/top_level.txt
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)       38 2024-05-26 19:06:21.075569 dsgepy-1.0/setup.cfg
+-rw-r--r--   0 gustavoamarante   (501) staff       (20)      848 2024-05-26 18:57:47.000000 dsgepy-1.0/setup.py
```

### Comparing `dsgepy-0.1/LICENSE` & `dsgepy-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsgepy-0.1/PKG-INFO` & `dsgepy-1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,79 @@
-Metadata-Version: 2.1
-Name: dsgepy
-Version: 0.1
-Summary: Solve and estimate linearized DSGE models
-Author: Gustavo Amarante
-Author-email: developer@dsgepy.com
-Keywords: dsge,macroeconomics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # dsgepy
-This is a Python library to calibrate, estimate and analyze linearized DSGE models. The interface is inpired by the 
-dynare interface which allows for symbolic declarations of the variables and equations. The implemented bayesian 
-estimation method uses markov chain monte carlo (MCMC) to simulate the posterior distributions of the parameters. This 
-library is an effort to bring the DSGE toolset into the open-source world in a full python implementation, which allows 
-to embrace the advantages of this programming language when working with DSGEs.
+This is a Python library to specify, calibrate, solve, simulate, estimate and 
+analyze linearized DSGE models. The specification interface is inpired by 
+dynare, which allows for symbolic declarations of parameters, variables and 
+equations. Once a model is calbrated or estimated, it is solved using Sims 
+(2002) methodology. 
+Simulated trajectories can be generated from a calibrated model. Estimation 
+uses bayesian methods, specifically markov chain monte carlo (MCMC), to 
+simulate the posterior distributions of the parameters. Analysis tools include 
+impulse-response functions, historical decompostion and extraction of latent 
+variables.
+
+This library is an effort to bring the DSGE toolset into the open-source world 
+in a full python implementation, which allows to embrace the advantages of this 
+programming language when working with DSGEs.
 
 ---
 # Installation
 You can install this development version using:
 ```
 pip install dsgepy
 ```
 
-### Kalman Filter
-Computing the likelihood of models involve using the kalman filter. `pykalman` is available for python, but some 
-adjustments to the original library are needed to use with this library. So **in order for `dsgepy` to work you need 
-the corrected version of `pykalman`, available [here](https://github.com/gusamarante/pykalman). Make sure to clone this 
-version and add it to the interpreter befor using `dsgepy`**. The corrections here correct the way `pykalman` handles 
-masked numpy arrays and deals with ill-estimated covariance matrices. 
-
 ---
 # Example
 A full example on how to use this library with a small New Keynesian model is available in 
 [this Jupyter notebook](https://github.com/gusamarante/pydsge/blob/master/Example/example_snkm.ipynb). The model used 
-in the example is descibred briefly by the following equations: 
+in the example is descibred briefly by the following equations:
 
 <img src="http://latex.codecogs.com/gif.latex?\tilde{y}_{t}=E_{t}\left(\tilde{y}_{t+1}\right)-\frac{1}{\sigma}\left[\hat{i}_{t}-E_{t}\left(\pi_{t+1}\right)\right]+\psi_{ya}^{n}\left(\rho_{a}-1\right)a_{t}" />
 
 <img src="http://latex.codecogs.com/gif.latex?\pi_{t}=\beta E_{t}\left(\pi_{t+1}\right)+\kappa\tilde{y}_{t}+\sigma_{\pi}\varepsilon_{t}^{\pi}" />
 
 <img src="http://latex.codecogs.com/gif.latex?\hat{i}_{t}=\phi_{\pi}\pi_{t}+\phi_{y}\tilde{y}_{t}+v_{t}" />
 
 <img src="http://latex.codecogs.com/gif.latex?a_{t}=\rho_{a}a_{t-1}+\sigma_{a}\varepsilon_{t}^{a}" />
 
 <img src="http://latex.codecogs.com/gif.latex?v_{t}=\rho_{v}v_{t-1}+\sigma_{v}\varepsilon_{t}^{v}" />
 
 
 # Model Especification
 For now, the model equations have to be linearized around its steady-state. 
-Soon, there will be a functionality that allows for non-linearized declaration 
-of the equilibrium conditions.
+Soon, there will be a functionality that allows for declaration with 
+non-linearized equilibrium conditions.
 
 # Model Solution
 The solution method used is based on the implementation of Christopher A. Sims' `gensys` function. You can find the 
 author's original matlab code [here](https://dge.repec.org/codes/sims/linre3a/). The paper explaining the solution 
 method is [this one](https://dge.repec.org/codes/sims/linre3a/LINRE3A.pdf).
 
 # Model Estimation
 The models are estimated using Bayesian methdos, specifically, by simulating the posterior distribution using MCMC 
-sampling. Simulations are typically long, so there is a functionality that allows you to stop a simulation and continue 
+sampling. This process is slow, so there is a functionality that allows you to stop a simulation and continue 
 it later from where it stoped.
 
 # Analysis
 There are functionalities for computing Impulse-Response funcions for both state variables and observed variables. 
 Historical decomposition is also available, but only when the number of exogenous shocks matches the number of 
 observed variables.
 
 ---
 # Drawbacks
-Since there is symbolic declaration of variables and equations, methdos involving them are slow, so the MCMC methods 
-typically take a long time to run. Although there is room for improvement for the efficiency of these estimation
-algorithms.
+Since there is symbolic declaration of variables and equations, methdos 
+involving them are slow. Also, MCMC methods for macroeconomic models require 
+many iterations to achieve convergence. Clearly, there is room for improvement 
+on the efficiency of these estimation algorithms. Contributions are welcome.
+Speaking of contributions...
 
 ---
 # Contributing
 If you would like to contribute to this repository, plese check the 
 [contributing guidelines](https://github.com/gusamarante/pydsge/blob/master/CONTRIBUTING.md) here. A 
 [list of feature suggestions](https://github.com/gusamarante/pydsge/projects) is available on the projects page of this
 repository.
 
 ---
 # More Information and Help
-If you need more information and help, specially about contributing, you can contact Gustavo Amarante on 
-developer@dsgepy.com
+If you need more information and help, specially about contributing, you can 
+contact Gustavo Amarante on developer@dsgepy.com
```

### Comparing `dsgepy-0.1/README.md` & `dsgepy-1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,96 @@
+Metadata-Version: 2.1
+Name: dsgepy
+Version: 1.0
+Summary: Solve and estimate linearized DSGE models
+Author: Gustavo Amarante
+Author-email: developer@dsgepy.com
+Keywords: dsge,macroeconomics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: tqdm
+Requires-Dist: sympy
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+
+
 # dsgepy
-This is a Python library to calibrate, estimate and analyze linearized DSGE models. The interface is inpired by the 
-dynare interface which allows for symbolic declarations of the variables and equations. The implemented bayesian 
-estimation method uses markov chain monte carlo (MCMC) to simulate the posterior distributions of the parameters. This 
-library is an effort to bring the DSGE toolset into the open-source world in a full python implementation, which allows 
-to embrace the advantages of this programming language when working with DSGEs.
+This is a Python library to specify, calibrate, solve, simulate, estimate and 
+analyze linearized DSGE models. The specification interface is inpired by 
+dynare, which allows for symbolic declarations of parameters, variables and 
+equations. Once a model is calbrated or estimated, it is solved using Sims 
+(2002) methodology. 
+Simulated trajectories can be generated from a calibrated model. Estimation 
+uses bayesian methods, specifically markov chain monte carlo (MCMC), to 
+simulate the posterior distributions of the parameters. Analysis tools include 
+impulse-response functions, historical decompostion and extraction of latent 
+variables.
+
+This library is an effort to bring the DSGE toolset into the open-source world 
+in a full python implementation, which allows to embrace the advantages of this 
+programming language when working with DSGEs.
 
 ---
 # Installation
 You can install this development version using:
 ```
 pip install dsgepy
 ```
 
-### Kalman Filter
-Computing the likelihood of models involve using the kalman filter. `pykalman` is available for python, but some 
-adjustments to the original library are needed to use with this library. So **in order for `dsgepy` to work you need 
-the corrected version of `pykalman`, available [here](https://github.com/gusamarante/pykalman). Make sure to clone this 
-version and add it to the interpreter befor using `dsgepy`**. The corrections here correct the way `pykalman` handles 
-masked numpy arrays and deals with ill-estimated covariance matrices. 
-
 ---
 # Example
 A full example on how to use this library with a small New Keynesian model is available in 
 [this Jupyter notebook](https://github.com/gusamarante/pydsge/blob/master/Example/example_snkm.ipynb). The model used 
-in the example is descibred briefly by the following equations: 
+in the example is descibred briefly by the following equations:
 
 <img src="http://latex.codecogs.com/gif.latex?\tilde{y}_{t}=E_{t}\left(\tilde{y}_{t+1}\right)-\frac{1}{\sigma}\left[\hat{i}_{t}-E_{t}\left(\pi_{t+1}\right)\right]+\psi_{ya}^{n}\left(\rho_{a}-1\right)a_{t}" />
 
 <img src="http://latex.codecogs.com/gif.latex?\pi_{t}=\beta E_{t}\left(\pi_{t+1}\right)+\kappa\tilde{y}_{t}+\sigma_{\pi}\varepsilon_{t}^{\pi}" />
 
 <img src="http://latex.codecogs.com/gif.latex?\hat{i}_{t}=\phi_{\pi}\pi_{t}+\phi_{y}\tilde{y}_{t}+v_{t}" />
 
 <img src="http://latex.codecogs.com/gif.latex?a_{t}=\rho_{a}a_{t-1}+\sigma_{a}\varepsilon_{t}^{a}" />
 
 <img src="http://latex.codecogs.com/gif.latex?v_{t}=\rho_{v}v_{t-1}+\sigma_{v}\varepsilon_{t}^{v}" />
 
 
 # Model Especification
 For now, the model equations have to be linearized around its steady-state. 
-Soon, there will be a functionality that allows for non-linearized declaration 
-of the equilibrium conditions.
+Soon, there will be a functionality that allows for declaration with 
+non-linearized equilibrium conditions.
 
 # Model Solution
 The solution method used is based on the implementation of Christopher A. Sims' `gensys` function. You can find the 
 author's original matlab code [here](https://dge.repec.org/codes/sims/linre3a/). The paper explaining the solution 
 method is [this one](https://dge.repec.org/codes/sims/linre3a/LINRE3A.pdf).
 
 # Model Estimation
 The models are estimated using Bayesian methdos, specifically, by simulating the posterior distribution using MCMC 
-sampling. Simulations are typically long, so there is a functionality that allows you to stop a simulation and continue 
+sampling. This process is slow, so there is a functionality that allows you to stop a simulation and continue 
 it later from where it stoped.
 
 # Analysis
 There are functionalities for computing Impulse-Response funcions for both state variables and observed variables. 
 Historical decomposition is also available, but only when the number of exogenous shocks matches the number of 
 observed variables.
 
 ---
 # Drawbacks
-Since there is symbolic declaration of variables and equations, methdos involving them are slow, so the MCMC methods 
-typically take a long time to run. Although there is room for improvement for the efficiency of these estimation
-algorithms.
+Since there is symbolic declaration of variables and equations, methdos 
+involving them are slow. Also, MCMC methods for macroeconomic models require 
+many iterations to achieve convergence. Clearly, there is room for improvement 
+on the efficiency of these estimation algorithms. Contributions are welcome.
+Speaking of contributions...
 
 ---
 # Contributing
 If you would like to contribute to this repository, plese check the 
 [contributing guidelines](https://github.com/gusamarante/pydsge/blob/master/CONTRIBUTING.md) here. A 
 [list of feature suggestions](https://github.com/gusamarante/pydsge/projects) is available on the projects page of this
 repository.
 
 ---
 # More Information and Help
-If you need more information and help, specially about contributing, you can contact Gustavo Amarante on 
-developer@dsgepy.com
+If you need more information and help, specially about contributing, you can 
+contact Gustavo Amarante on developer@dsgepy.com
```

### Comparing `dsgepy-0.1/dsgepy/lineardsge.py` & `dsgepy-1.0/dsgepy/lineardsge.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # import warnings
 import pandas as pd
 from tqdm import tqdm
 from scipy.linalg import qz
 from math import ceil, floor
 import matplotlib.pyplot as plt
-from pykalman import KalmanFilter
+from dsgepy.kalman import KalmanFilter
 from sympy import simplify, Matrix
 # from tables import PerformanceWarning
 from dsgepy.pycsminwel import csminwel
 from scipy.optimize import minimize, basinhopping
 from numpy.random import multivariate_normal, rand, seed
 from scipy.stats import beta, gamma, invgamma, norm, uniform
 from numpy.linalg import svd, inv, eig, matrix_power, LinAlgError
@@ -352,40 +352,68 @@
         df_irf_obs = pd.DataFrame(columns=col_names_obs, index=mindex)
 
         for count, var in enumerate(idx_names):
             df_irf_obs.loc[var] = obs_irf_values[:, :, count]
 
         # Charts
         if show_charts:
-            shocks = df_irf.index.get_level_values(0).unique()
+            if self.obs_equations is None:  # TODO I need a cleaner way to do this
+                shocks = df_irf.index.get_level_values(0).unique()
 
-            n_subplots = df_irf.shape[1] + df_irf_obs.shape[1]
-            n_rows = floor(sqrt(n_subplots))
-            n_cols = ceil(n_subplots / n_rows)
-            subplot_shape = (n_rows, n_cols)
-
-            for ss in shocks:
-                plot_irfs = pd.concat([df_irf.loc[ss], df_irf_obs.loc[ss]], axis=1)
-                ax = plot_irfs.plot(title=f'Impulse Response Functions: Shock {ss}',
-                                    subplots=True,
-                                    layout=subplot_shape,
-                                    legend=None,
-                                    grid=True,
-                                    figsize=(12, 7),
-                                    sharey=False)
-
-                zero_irf = list(plot_irfs.columns[(plot_irfs.abs() < 1e-10).all()])
-
-                for axis, subptitle in zip(ax.ravel(), list(plot_irfs.columns)):
-                    axis.set_title(subptitle)
-                    if subptitle in zero_irf:
-                        axis.set_ylim((-1, 1))
+                n_subplots = df_irf.shape[1]
+                n_rows = floor(sqrt(n_subplots))
+                n_cols = ceil(n_subplots / n_rows)
+                subplot_shape = (n_rows, n_cols)
+
+                for ss in shocks:
+                    plot_irfs = pd.concat([df_irf.loc[ss]], axis=1)
+                    ax = plot_irfs.plot(title=f'Impulse Response Functions: Shock {ss}',
+                                        subplots=True,
+                                        layout=subplot_shape,
+                                        legend=None,
+                                        grid=True,
+                                        figsize=(12, 7),
+                                        sharey=False)
+
+                    zero_irf = list(plot_irfs.columns[(plot_irfs.abs() < 1e-10).all()])
+
+                    for axis, subptitle in zip(ax.ravel(), list(plot_irfs.columns)):
+                        axis.set_title(subptitle)
+                        if subptitle in zero_irf:
+                            axis.set_ylim((-1, 1))
 
-                plt.tight_layout()
-                plt.show()
+                    plt.tight_layout()
+                    plt.show()
+            else:
+                shocks = df_irf.index.get_level_values(0).unique()
+
+                n_subplots = df_irf.shape[1] + df_irf_obs.shape[1]
+                n_rows = floor(sqrt(n_subplots))
+                n_cols = ceil(n_subplots / n_rows)
+                subplot_shape = (n_rows, n_cols)
+
+                for ss in shocks:
+                    plot_irfs = pd.concat([df_irf.loc[ss], df_irf_obs.loc[ss]], axis=1)
+                    ax = plot_irfs.plot(title=f'Impulse Response Functions: Shock {ss}',
+                                        subplots=True,
+                                        layout=subplot_shape,
+                                        legend=None,
+                                        grid=True,
+                                        figsize=(12, 7),
+                                        sharey=False)
+
+                    zero_irf = list(plot_irfs.columns[(plot_irfs.abs() < 1e-10).all()])
+
+                    for axis, subptitle in zip(ax.ravel(), list(plot_irfs.columns)):
+                        axis.set_title(subptitle)
+                        if subptitle in zero_irf:
+                            axis.set_ylim((-1, 1))
+
+                    plt.tight_layout()
+                    plt.show()
 
         # Concatenate state and observed variables
         df_irf = pd.concat([df_irf, df_irf_obs], axis=1)
 
         return df_irf
 
     def states(self, smoothed=True):
```

### Comparing `dsgepy-0.1/dsgepy/pycsminwel.py` & `dsgepy-1.0/dsgepy/pycsminwel.py`

 * *Files identical despite different names*

### Comparing `dsgepy-0.1/dsgepy.egg-info/PKG-INFO` & `dsgepy-1.0/dsgepy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,96 @@
 Metadata-Version: 2.1
 Name: dsgepy
-Version: 0.1
+Version: 1.0
 Summary: Solve and estimate linearized DSGE models
 Author: Gustavo Amarante
 Author-email: developer@dsgepy.com
 Keywords: dsge,macroeconomics
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: scipy
+Requires-Dist: tqdm
+Requires-Dist: sympy
+Requires-Dist: numpy
+Requires-Dist: matplotlib
 
 
 # dsgepy
-This is a Python library to calibrate, estimate and analyze linearized DSGE models. The interface is inpired by the 
-dynare interface which allows for symbolic declarations of the variables and equations. The implemented bayesian 
-estimation method uses markov chain monte carlo (MCMC) to simulate the posterior distributions of the parameters. This 
-library is an effort to bring the DSGE toolset into the open-source world in a full python implementation, which allows 
-to embrace the advantages of this programming language when working with DSGEs.
+This is a Python library to specify, calibrate, solve, simulate, estimate and 
+analyze linearized DSGE models. The specification interface is inpired by 
+dynare, which allows for symbolic declarations of parameters, variables and 
+equations. Once a model is calbrated or estimated, it is solved using Sims 
+(2002) methodology. 
+Simulated trajectories can be generated from a calibrated model. Estimation 
+uses bayesian methods, specifically markov chain monte carlo (MCMC), to 
+simulate the posterior distributions of the parameters. Analysis tools include 
+impulse-response functions, historical decompostion and extraction of latent 
+variables.
+
+This library is an effort to bring the DSGE toolset into the open-source world 
+in a full python implementation, which allows to embrace the advantages of this 
+programming language when working with DSGEs.
 
 ---
 # Installation
 You can install this development version using:
 ```
 pip install dsgepy
 ```
 
-### Kalman Filter
-Computing the likelihood of models involve using the kalman filter. `pykalman` is available for python, but some 
-adjustments to the original library are needed to use with this library. So **in order for `dsgepy` to work you need 
-the corrected version of `pykalman`, available [here](https://github.com/gusamarante/pykalman). Make sure to clone this 
-version and add it to the interpreter befor using `dsgepy`**. The corrections here correct the way `pykalman` handles 
-masked numpy arrays and deals with ill-estimated covariance matrices. 
-
 ---
 # Example
 A full example on how to use this library with a small New Keynesian model is available in 
 [this Jupyter notebook](https://github.com/gusamarante/pydsge/blob/master/Example/example_snkm.ipynb). The model used 
-in the example is descibred briefly by the following equations: 
+in the example is descibred briefly by the following equations:
 
 <img src="http://latex.codecogs.com/gif.latex?\tilde{y}_{t}=E_{t}\left(\tilde{y}_{t+1}\right)-\frac{1}{\sigma}\left[\hat{i}_{t}-E_{t}\left(\pi_{t+1}\right)\right]+\psi_{ya}^{n}\left(\rho_{a}-1\right)a_{t}" />
 
 <img src="http://latex.codecogs.com/gif.latex?\pi_{t}=\beta E_{t}\left(\pi_{t+1}\right)+\kappa\tilde{y}_{t}+\sigma_{\pi}\varepsilon_{t}^{\pi}" />
 
 <img src="http://latex.codecogs.com/gif.latex?\hat{i}_{t}=\phi_{\pi}\pi_{t}+\phi_{y}\tilde{y}_{t}+v_{t}" />
 
 <img src="http://latex.codecogs.com/gif.latex?a_{t}=\rho_{a}a_{t-1}+\sigma_{a}\varepsilon_{t}^{a}" />
 
 <img src="http://latex.codecogs.com/gif.latex?v_{t}=\rho_{v}v_{t-1}+\sigma_{v}\varepsilon_{t}^{v}" />
 
 
 # Model Especification
 For now, the model equations have to be linearized around its steady-state. 
-Soon, there will be a functionality that allows for non-linearized declaration 
-of the equilibrium conditions.
+Soon, there will be a functionality that allows for declaration with 
+non-linearized equilibrium conditions.
 
 # Model Solution
 The solution method used is based on the implementation of Christopher A. Sims' `gensys` function. You can find the 
 author's original matlab code [here](https://dge.repec.org/codes/sims/linre3a/). The paper explaining the solution 
 method is [this one](https://dge.repec.org/codes/sims/linre3a/LINRE3A.pdf).
 
 # Model Estimation
 The models are estimated using Bayesian methdos, specifically, by simulating the posterior distribution using MCMC 
-sampling. Simulations are typically long, so there is a functionality that allows you to stop a simulation and continue 
+sampling. This process is slow, so there is a functionality that allows you to stop a simulation and continue 
 it later from where it stoped.
 
 # Analysis
 There are functionalities for computing Impulse-Response funcions for both state variables and observed variables. 
 Historical decomposition is also available, but only when the number of exogenous shocks matches the number of 
 observed variables.
 
 ---
 # Drawbacks
-Since there is symbolic declaration of variables and equations, methdos involving them are slow, so the MCMC methods 
-typically take a long time to run. Although there is room for improvement for the efficiency of these estimation
-algorithms.
+Since there is symbolic declaration of variables and equations, methdos 
+involving them are slow. Also, MCMC methods for macroeconomic models require 
+many iterations to achieve convergence. Clearly, there is room for improvement 
+on the efficiency of these estimation algorithms. Contributions are welcome.
+Speaking of contributions...
 
 ---
 # Contributing
 If you would like to contribute to this repository, plese check the 
 [contributing guidelines](https://github.com/gusamarante/pydsge/blob/master/CONTRIBUTING.md) here. A 
 [list of feature suggestions](https://github.com/gusamarante/pydsge/projects) is available on the projects page of this
 repository.
 
 ---
 # More Information and Help
-If you need more information and help, specially about contributing, you can contact Gustavo Amarante on 
-developer@dsgepy.com
+If you need more information and help, specially about contributing, you can 
+contact Gustavo Amarante on developer@dsgepy.com
```

### Comparing `dsgepy-0.1/setup.py` & `dsgepy-1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1'
+VERSION = '1.0'
 DESCRIPTION = 'Solve and estimate linearized DSGE models'
 
 # Setting up
 setup(name="dsgepy",
       version=VERSION,
       author="Gustavo Amarante",
       author_email="developer@dsgepy.com",
```

