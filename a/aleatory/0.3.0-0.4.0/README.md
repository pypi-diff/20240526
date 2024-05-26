# Comparing `tmp/aleatory-0.3.0.tar.gz` & `tmp/aleatory-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dialidsantiago/Git/aleatory/dist/.tmp-x2_i0bwl/aleatory-0.3.0.tar", last modified: Fri Apr 19 20:10:55 2024, max compression
+gzip compressed data, was "/Users/dialidsantiago/Git/aleatory/dist/.tmp-yiekrx3o/aleatory-0.4.0.tar", last modified: Sun May 26 07:56:27 2024, max compression
```

## Comparing `aleatory-0.3.0.tar` & `aleatory-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,54 @@
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.770718 aleatory-0.3.0/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1090 2024-04-19 18:45:58.000000 aleatory-0.3.0/LICENSE
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     4101 2024-04-19 20:10:55.769810 aleatory-0.3.0/PKG-INFO
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     3186 2024-04-19 18:45:32.000000 aleatory-0.3.0/README.md
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.716492 aleatory-0.3.0/aleatory/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.3.0/aleatory/__init__.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.721969 aleatory-0.3.0/aleatory/processes/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      756 2024-04-12 13:11:57.000000 aleatory-0.3.0/aleatory/processes/__init__.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.743036 aleatory-0.3.0/aleatory/processes/analytical/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.3.0/aleatory/processes/analytical/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     6191 2024-01-08 21:57:15.000000 aleatory-0.3.0/aleatory/processes/analytical/bes.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5094 2024-01-08 21:57:20.000000 aleatory-0.3.0/aleatory/processes/analytical/besq.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     6085 2024-04-19 19:37:07.000000 aleatory-0.3.0/aleatory/processes/analytical/brownian_bridge.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     2643 2024-04-19 18:36:09.000000 aleatory-0.3.0/aleatory/processes/analytical/brownian_excursion.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     4335 2024-04-19 19:37:27.000000 aleatory-0.3.0/aleatory/processes/analytical/brownian_meander.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5740 2024-04-19 15:25:01.000000 aleatory-0.3.0/aleatory/processes/analytical/brownian_motion.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     2064 2024-04-08 15:35:51.000000 aleatory-0.3.0/aleatory/processes/analytical/gaussian.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5062 2022-12-25 17:41:15.000000 aleatory-0.3.0/aleatory/processes/analytical/geometric_brownian.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     6430 2024-04-12 14:05:19.000000 aleatory-0.3.0/aleatory/processes/base.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.753609 aleatory-0.3.0/aleatory/processes/euler_maruyama/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5260 2023-04-29 10:54:19.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/cev_process.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5400 2023-06-10 09:19:44.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/cir_process.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1638 2022-12-25 18:20:27.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     3312 2023-11-12 09:39:52.000000 aleatory-0.3.0/aleatory/processes/euler_maruyama/vasicek.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.757083 aleatory-0.3.0/aleatory/stats/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      427 2024-01-14 14:32:19.000000 aleatory-0.3.0/aleatory/stats/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     4174 2024-01-14 14:26:45.000000 aleatory-0.3.0/aleatory/stats/non_central_chi.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.759317 aleatory-0.3.0/aleatory/utils/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.3.0/aleatory/utils/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)    10659 2024-04-19 18:15:19.000000 aleatory-0.3.0/aleatory/utils/utils.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.768791 aleatory-0.3.0/aleatory.egg-info/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     4101 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/PKG-INFO
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1159 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/SOURCES.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        1 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/dependency_links.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      100 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/requires.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        9 2024-04-19 20:10:55.000000 aleatory-0.3.0/aleatory.egg-info/top_level.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1008 2024-04-19 18:44:34.000000 aleatory-0.3.0/pyproject.toml
--rw-r--r--   0 dialidsantiago   (501) staff       (20)       38 2024-04-19 20:10:55.770917 aleatory-0.3.0/setup.cfg
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-04-19 20:10:55.767421 aleatory-0.3.0/tests/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     4683 2024-01-08 22:41:25.000000 aleatory-0.3.0/tests/test_bes.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     6644 2024-04-19 19:54:54.000000 aleatory-0.3.0/tests/test_charts.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      656 2024-01-11 14:27:54.000000 aleatory-0.3.0/tests/test_marginal_functions.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1616 2024-01-11 16:02:20.000000 aleatory-0.3.0/tests/test_ncx.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      258 2022-12-25 12:07:25.000000 aleatory-0.3.0/tests/test_transormation_em.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.364956 aleatory-0.4.0/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1091 2024-05-26 07:46:05.000000 aleatory-0.4.0/LICENSE
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4252 2024-05-26 07:56:27.363795 aleatory-0.4.0/PKG-INFO
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     3337 2024-05-26 07:53:08.000000 aleatory-0.4.0/README.md
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.321261 aleatory-0.4.0/aleatory/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.4.0/aleatory/__init__.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.328578 aleatory-0.4.0/aleatory/processes/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      887 2024-05-19 20:44:09.000000 aleatory-0.4.0/aleatory/processes/__init__.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.337587 aleatory-0.4.0/aleatory/processes/analytical/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.4.0/aleatory/processes/analytical/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     6242 2024-05-26 07:22:15.000000 aleatory-0.4.0/aleatory/processes/analytical/bes.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5341 2024-05-19 07:45:51.000000 aleatory-0.4.0/aleatory/processes/analytical/besq.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     6055 2024-05-26 07:12:10.000000 aleatory-0.4.0/aleatory/processes/analytical/brownian_bridge.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     2620 2024-05-26 07:13:13.000000 aleatory-0.4.0/aleatory/processes/analytical/brownian_excursion.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4685 2024-05-26 07:17:09.000000 aleatory-0.4.0/aleatory/processes/analytical/brownian_meander.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     7040 2024-05-26 07:20:50.000000 aleatory-0.4.0/aleatory/processes/analytical/brownian_motion.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     2064 2024-04-08 15:35:51.000000 aleatory-0.4.0/aleatory/processes/analytical/gaussian.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5158 2024-05-19 07:24:40.000000 aleatory-0.4.0/aleatory/processes/analytical/geometric_brownian.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1113 2024-05-19 07:00:40.000000 aleatory-0.4.0/aleatory/processes/base.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5917 2024-05-26 07:08:56.000000 aleatory-0.4.0/aleatory/processes/base_analytical.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1166 2024-05-19 07:00:40.000000 aleatory-0.4.0/aleatory/processes/base_eu.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.345425 aleatory-0.4.0/aleatory/processes/euler_maruyama/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.4.0/aleatory/processes/euler_maruyama/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     2584 2024-05-19 12:17:48.000000 aleatory-0.4.0/aleatory/processes/euler_maruyama/cev_process.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5403 2024-05-19 17:30:12.000000 aleatory-0.4.0/aleatory/processes/euler_maruyama/cir_process.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     2901 2024-05-26 07:25:58.000000 aleatory-0.4.0/aleatory/processes/euler_maruyama/ckls_process.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4949 2024-05-25 22:58:16.000000 aleatory-0.4.0/aleatory/processes/euler_maruyama/ckls_process_generic.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1638 2022-12-25 18:20:27.000000 aleatory-0.4.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     3612 2024-05-19 07:05:19.000000 aleatory-0.4.0/aleatory/processes/euler_maruyama/vasicek.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.347778 aleatory-0.4.0/aleatory/processes/jump/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2024-05-18 13:52:20.000000 aleatory-0.4.0/aleatory/processes/jump/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     7898 2024-05-26 07:18:08.000000 aleatory-0.4.0/aleatory/processes/jump/poisson.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.350270 aleatory-0.4.0/aleatory/stats/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      427 2024-01-14 14:32:19.000000 aleatory-0.4.0/aleatory/stats/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4174 2024-01-14 14:26:45.000000 aleatory-0.4.0/aleatory/stats/non_central_chi.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.352514 aleatory-0.4.0/aleatory/utils/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.4.0/aleatory/utils/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)    10693 2024-04-24 23:03:36.000000 aleatory-0.4.0/aleatory/utils/utils.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.362991 aleatory-0.4.0/aleatory.egg-info/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4252 2024-05-26 07:56:27.000000 aleatory-0.4.0/aleatory.egg-info/PKG-INFO
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1442 2024-05-26 07:56:27.000000 aleatory-0.4.0/aleatory.egg-info/SOURCES.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        1 2024-05-26 07:56:27.000000 aleatory-0.4.0/aleatory.egg-info/dependency_links.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      100 2024-05-26 07:56:27.000000 aleatory-0.4.0/aleatory.egg-info/requires.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        9 2024-05-26 07:56:27.000000 aleatory-0.4.0/aleatory.egg-info/top_level.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1008 2024-05-26 07:45:17.000000 aleatory-0.4.0/pyproject.toml
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)       38 2024-05-26 07:56:27.365098 aleatory-0.4.0/setup.cfg
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2024-05-26 07:56:27.362269 aleatory-0.4.0/tests/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4683 2024-01-08 22:41:25.000000 aleatory-0.4.0/tests/test_bes.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1745 2024-05-19 20:43:30.000000 aleatory-0.4.0/tests/test_bm.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     6888 2024-05-19 12:22:33.000000 aleatory-0.4.0/tests/test_charts.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     3275 2024-05-20 21:19:41.000000 aleatory-0.4.0/tests/test_ckls.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      654 2024-05-19 12:22:33.000000 aleatory-0.4.0/tests/test_marginal_functions.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1616 2024-01-11 16:02:20.000000 aleatory-0.4.0/tests/test_ncx.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      258 2022-12-25 12:07:25.000000 aleatory-0.4.0/tests/test_transormation_em.py
```

### Comparing `aleatory-0.3.0/LICENSE` & `aleatory-0.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022-2024 Dialid Santiago (Quant Girl)
+Copyright (c) 2022-2024 Dialid Santiago (@Quant_Girl)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `aleatory-0.3.0/PKG-INFO` & `aleatory-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,10 @@
-Metadata-Version: 2.1
-Name: aleatory
-Version: 0.3.0
-Summary: Stochastic Processes Simulation and Visualisation
-Author-email: Dialid Santiago <d.santiago@outlook.com>
-Project-URL: Homepage, https://github.com/quantgirluk/aleatory
-Project-URL: Bug Tracker, https://github.com/quantgirluk/aleatory/issues
-Project-URL: Documentation, https://aleatory.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: numpy>=1.23.5
-Requires-Dist: scipy>=1.9.3
-Requires-Dist: matplotlib>=3.6.2
-Requires-Dist: statsmodels>=0.13.5
-Requires-Dist: parameterized>=0.8.1
-
 # *aleatory*
 
 [![PyPI version fury.io](https://badge.fury.io/py/aleatory.svg)](https://pypi.org/project/aleatory/) [![Downloads](https://static.pepy.tech/personalized-badge/aleatory?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/aleatory)
-
 ![example workflow](https://github.com/quantgirluk/aleatory/actions/workflows/python-package.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/aleatory/badge/?version=latest)](https://aleatory.readthedocs.io/en/latest/?badge=latest)
 
 - [Git Homepage](https://github.com/quantgirluk/aleatory)
 - [Pip Repository](https://pypi.org/project/aleatory/)
 - [Documentation](https://aleatory.readthedocs.io/en/latest/)
 
 ## Overview
@@ -41,27 +17,29 @@
 - create visualisations to illustrate the processes properties and behaviour
 
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/vasicek_process_drawn.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
 </p>
 
-Currently, `aleatory` supports the following processes:
+Currently, `aleatory` supports the following 13 processes:
 
 - Brownian Motion
 - Brownian Bridge
 - Brownian Excursion
 - Brownian Meander
-- Geometric Brownian Motion
-- Ornstein–Uhlenbeck
-- Vasicek
-- Cox–Ingersoll–Ross
-- Constant Elasticity
-- Bessel Process
-- Squared Bessel Processs
+- Geometric Brownian Motion (GBM) process
+- Ornstein–Uhlenbeck (OU) process
+- Vasicek process
+- Cox–Ingersoll–Ross (CIR) process
+- Constant Elasticity Variance (CEV) process
+- Chan-Karolyi-Longstaff-Sanders (CKLS) process
+- Bessel (BES) process
+- Squared Bessel (BESQ) process
+- Poisson process
 
 ## Installation
 
 Aleatory is available on [pypi](https://pypi.python.org/pypi) and can be
 installed as follows
 
 ```
@@ -74,15 +52,15 @@
 
 - ``numpy``  for random number generation
 - ``scipy`` and ``statsmodels`` for support for a number of one-dimensional distributions.
 - ``matplotlib`` for creating visualisations
 
 ## Compatibility
 
-Aleatory is tested on Python versions 3.8, 3.9, and 3.10
+Aleatory is tested on Python versions 3.8, 3.9, 3.10, and 3.11
 
 ## Quick-Start
 
 Aleatory allows you to create fancy visualisations from different stochastic processes in an easy and concise way.
 
 For example, the following code
 
@@ -99,15 +77,15 @@
 <p align="center">
 <img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
 </p>
 
 For more examples visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
 
 
-⭐️ **If you like this project, please give it a star!** ⭐️
+**If you like this project, please give it a star!** ⭐️
 
 ## Thanks for Visiting! ✨
 
 Connect with me via:
 
 - 🦜 [Twitter](https://twitter.com/Quant_Girl)
 - 👩🏽‍💼 [Linkedin](https://www.linkedin.com/in/dialidsantiago/)
```

### Comparing `aleatory-0.3.0/aleatory/processes/__init__.py` & `aleatory-0.4.0/aleatory/processes/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from aleatory.processes.euler_maruyama.vasicek import Vasicek
 from aleatory.processes.euler_maruyama.ornstein_uhlenbeck import OUProcess
 from aleatory.processes.euler_maruyama.cir_process import CIRProcess
-from aleatory.processes.euler_maruyama.cev_process import CEVProcess
+
 from aleatory.processes.analytical.geometric_brownian import GBM
 from aleatory.processes.analytical.brownian_motion import BrownianMotion
 from aleatory.processes.analytical.bes import BESProcess
 from aleatory.processes.analytical.besq import BESQProcess
 from aleatory.processes.analytical.brownian_bridge import BrownianBridge
 from aleatory.processes.analytical.brownian_excursion import BrownianExcursion
 from aleatory.processes.analytical.brownian_meander import BrownianMeander
+from aleatory.processes.euler_maruyama.ckls_process import CKLSProcess
+from aleatory.processes.euler_maruyama.cev_process import CEVProcess
+from aleatory.processes.jump.poisson import PoissonProcess
```

### Comparing `aleatory-0.3.0/aleatory/processes/analytical/bes.py` & `aleatory-0.4.0/aleatory/processes/analytical/bes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from functools import partial
 from multiprocessing import Pool
 
 import numpy as np
 from scipy.special import eval_genlaguerre
 
 from aleatory.processes.analytical.brownian_motion import BrownianMotion
-from aleatory.processes.base import SPExplicit
+from aleatory.processes.base_analytical import SPAnalytical
 from aleatory.stats import ncx
 from aleatory.utils.utils import check_positive_integer, get_times, sample_bessel_global
 
 
 def _sample_bessel_global(T, initial, dim, n):
     path = sample_bessel_global(T=T, initial=initial, dim=dim, n=n)
     return path
 
 
-class BESProcess(SPExplicit):
+class BESProcess(SPAnalytical):
     r"""Bessel process
 
     .. image:: _static/bes_process_drawn.png
 
 
     A Bessel process :math:`BES^{n}_{0},` for :math:`n\geq 2` integer is a continuous stochastic process
     :math:`\{X(t) : t \geq  0\}` characterised as the Euclidian norm of an :math:`n`-dimensional
@@ -113,17 +113,17 @@
         else:
             return _sample_bessel_global(self.T, self.initial, self.dim, n)
 
     def simulate(self, n, N):
         """
         Simulate paths/trajectories from the instanced stochastic process.
 
-        param n: number of steps in each path
-        param N: number of paths to simulate
-        return: list with N paths (each one is a numpy array of size n)
+        :param int n: number of steps in each path
+        :param int N: number of paths to simulate
+        :return: list with N paths (each one is a numpy array of size n)
         """
         self.n = n
         self.N = N
         self.times = get_times(self.T, n)
 
         if isinstance(self.dim, int) and self.initial == 0:
 
@@ -139,17 +139,14 @@
             results = pool.map(func, [n] * N)
             pool.close()
             pool.join()
 
             self.paths = results
             return self.paths
 
-    def get_marginal(self, t):
-        marginal = ncx(df=self.dim, nc=self.initial / np.sqrt(t), scale=np.sqrt(t))
-        return marginal
 
     def _process_expectation(self, times=None):
         # TODO: Add the case when times is zero, at the moment this fails because nc required division by t
         if times is None:
             times = self.times
 
         alpha = (self.dim / 2.0) - 1.0
@@ -161,29 +158,32 @@
         else:
             nc = (self.initial ** 2) / times[1:]
             expectations = np.sqrt(times[1:]) * math.sqrt(math.pi / 2.0) * eval_genlaguerre(0.5, alpha,
                                                                                             (-1.0 / 2.0) * nc)
             expectations = np.insert(expectations, 0, self.initial)
         return expectations
 
-    def marginal_expectation(self, times=None):
-        expectations = self._process_expectation(times=times)
-        return expectations
-
     def _process_variance(self, times=None):
         if times is None:
             times = self.times
         expectations = self._process_expectation(times)
         variances = self.dim * times + self.initial ** 2 - expectations ** 2
         return variances
 
-    def marginal_variance(self, times):
+    def _process_stds(self, times=None):
+        if times is None:
+            times = self.times
         variances = self._process_variance(times=times)
-        return variances
-
-    def _process_stds(self):
-        stds = np.sqrt(self._process_variance())
+        stds = np.sqrt(variances)
         return stds
 
-    def process_stds(self):
-        stds = self._process_stds()
-        return stds
+    def get_marginal(self, t):
+        marginal = ncx(df=self.dim, nc=self.initial / np.sqrt(t), scale=np.sqrt(t))
+        return marginal
+
+    def marginal_expectation(self, times=None):
+        expectations = self._process_expectation(times=times)
+        return expectations
+
+    def marginal_variance(self, times):
+        variances = self._process_variance(times=times)
+        return variances
```

### Comparing `aleatory-0.3.0/aleatory/processes/analytical/besq.py` & `aleatory-0.4.0/aleatory/processes/analytical/besq.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from functools import partial
 from multiprocessing import Pool
 
 import numpy as np
 from scipy.stats import ncx2
 
 from aleatory.processes.analytical.brownian_motion import BrownianMotion
-from aleatory.processes.base import SPExplicit
+from aleatory.processes.base_analytical import SPAnalytical
 from aleatory.utils.utils import get_times, check_positive_integer, sample_besselq_global
 
 
 def _sample_besselq_global(T, initial, dim, n):
     path = sample_besselq_global(T=T, initial=initial, dim=dim, n=n)
 
     return path
 
 
-class BESQProcess(SPExplicit):
+class BESQProcess(SPAnalytical):
     r"""Squared Bessel process
 
     .. image:: _static/besq_process_drawn.png
 
 
     A squared Bessel process :math:`BESQ^{n}_{0}`, for :math:`n` integer is a continuous stochastic process
     :math:`\{X(t) : t \geq  0\}` which is characterised as the squared Euclidian norm of an :math:`n`-dimensional
@@ -126,39 +126,46 @@
             results = pool.map(func, [n] * N)
             pool.close()
             pool.join()
 
             self.paths = results
             return self.paths
 
-    def get_marginal(self, t):
-        marginal = ncx2(df=self.dim, nc=self.initial / t, scale=t)
-        return marginal
-
     def _process_expectation(self, times=None):
         if times is None:
             times = self.times
         expectations = self.initial + self.dim * np.array(times)
         return expectations
 
-    def marginal_expectation(self, times=None):
-        expectations = self._process_expectation(times=times)
-        return expectations
-
     def _process_variance(self, times=None):
         if times is None:
             times = self.times
-        variances = 2.0 * (self.dim + 2.0*self.initial/times) * times**2
+        variances = 2.0 * (self.dim + 2.0 * self.initial / times) * times ** 2
 
         return variances
 
-    def marginal_variance(self, times):
+    def _process_stds(self, times=None):
+        if times is None:
+            times = self.times
         variances = self._process_variance(times=times)
-        return variances
-
-    def _process_stds(self):
-        stds = np.sqrt(self._process_variance())
+        stds = np.sqrt(variances)
         return stds
 
-    def process_stds(self):
-        stds = self._process_stds()
-        return stds
+    # def _process_stds(self):
+    #     stds = np.sqrt(self._process_variance())
+    #     return stds
+    #
+    # def process_stds(self):
+    #     stds = self._process_stds()
+    #     return stds
+
+    def get_marginal(self, t):
+        marginal = ncx2(df=self.dim, nc=self.initial / t, scale=t)
+        return marginal
+
+    def marginal_expectation(self, times=None):
+        expectations = self._process_expectation(times=times)
+        return expectations
+
+    def marginal_variance(self, times):
+        variances = self._process_variance(times=times)
+        return variances
```

### Comparing `aleatory-0.3.0/aleatory/processes/analytical/brownian_bridge.py` & `aleatory-0.4.0/aleatory/processes/analytical/brownian_bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
     .. math::
 
         B_t = (W_t | W_T = 0), \ \ \ \   t\in (0,T].
 
     More generally, a Brownian Bridge is  subject to the conditions :math:`W(0) = a` and :math:`W(T) = b`.
 
-    Parameters
-        :param float initial: initial condition
-        :param float end: end condition
-        :param float T: the right hand endpoint of the time interval :math:`[0,T]`
+
+    :param float initial: initial condition
+    :param float end: end condition
+    :param float T: the right hand endpoint of the time interval :math:`[0,T]`
         for the process
-        :param numpy.random.Generator rng: a custom random number generator
+    :param numpy.random.Generator rng: a custom random number generator
 
     """
     def __init__(self, initial=0.0, end=0.0, T=1.0, rng=None):
         """
         Parameters
         :param float initial: initial condition
         :param float end: end condition
```

### Comparing `aleatory-0.3.0/aleatory/processes/analytical/brownian_excursion.py` & `aleatory-0.4.0/aleatory/processes/analytical/brownian_excursion.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,17 @@
 
     .. image:: _static/brownian_excursion_drawn.png
 
     A Brownian excursion process, is a Wiener process (or Brownian motion) conditioned
     to be positive and to take the value 0 at time 1. Alternatively, it can be defined as a Brownian
     Bridge process conditioned to be positive.
 
-    Parameters
-        :param float T: the right hand endpoint of the time interval :math:`[0,T]`
+    :param float T: the right hand endpoint of the time interval :math:`[0,T]`
         for the process
-        :param numpy.random.Generator rng: a custom random number generator
+    :param numpy.random.Generator rng: a custom random number generator
 
     """
     def __init__(self, T=1.0, rng=None):
         super().__init__(T=T, rng=rng)
         self.name = "Brownian Excursion"
         self.description = "Brownian Excursion"
         self._brownian_bridge = BrownianBridge(initial=0.0, end=0.0, T=T, rng=rng)
```

### Comparing `aleatory-0.3.0/aleatory/processes/analytical/brownian_meander.py` & `aleatory-0.4.0/aleatory/processes/analytical/brownian_meander.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,19 @@
 
     i.e. the last time before t = 1 when :math:`W_t` visits zero. Then the
     Brownian Meander is defined as follows
 
     .. math::
         W_t^{+} = \frac{1}{\sqrt{1-\tau}} |W(\tau  + t (1-\tau))|, \ \ \ \   t\in (0,1].
 
-
-    Parameters
+    :param float T: the right hand endpoint of the time interval :math:`[0,T]`
+        for the process
+    :param bool fixed_end: flag to indicate if the process has a fixed end point. Defaults to `False`
+    :param float end: end point for the Meander, in the case of `fixed_end` equal `True`
+    :param numpy.random.Generator rng: a custom random number generator
 
     """
 
     def __init__(self, T=1.0, fixed_end=False, end=None, rng=None):
         super().__init__(T=T, rng=rng)
         self.name = "Tied Brownian Meander" if fixed_end else "Brownian Meander"
         self.fixed_end = fixed_end
```

### Comparing `aleatory-0.3.0/aleatory/processes/analytical/brownian_motion.py` & `aleatory-0.4.0/aleatory/processes/analytical/brownian_motion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 """Brownian Motion"""
 import numpy as np
 from scipy.stats import norm
 
-from aleatory.processes.base import SPExplicit
+from aleatory.processes.base_analytical import SPAnalytical
 from aleatory.processes.analytical.gaussian import GaussianIncrements
 from aleatory.utils.utils import check_positive_number, check_numeric, get_times
 
 
-class BrownianMotion(SPExplicit):
+class BrownianMotion(SPAnalytical):
     r"""Brownian motion
 
     .. image:: _static/brownian_motion_drawn.png
 
 
     A standard Brownian motion    :math:`\{W_t : t \geq 0\}` is defined by the following properties:
 
     1. Starts at zero, i.e. :math:`W(0) = 0`
     2. Independent increments
     3. :math:`W(t) - W(s)` follows a Gaussian distribution :math:`N(0, t-s)`
     4. Almost surely continuous
 
-    A more general version of a Brownian motion, is the Drifted Brownian Motion which  is defined
+    A more general version of a Brownian motion, is the Arithmetic Brownian Motion which  is defined
     by the following SDE
 
     .. math::
 
         dX_t = \mu dt + \sigma dW_t \ \ \ \   t\in (0,T]
 
 
     with initial condition :math:`X_0 = x_0\in\mathbb{R}`, where
 
     - :math:`\mu` is the drift
     - :math:`\sigma>0` is the volatility
-    - :math:`W_t` is a standard Brownian Motion.
+    - :math:`W_t` is a standard Brownian Motion
 
     Clearly, the solution to this equation can be written as
 
     .. math::
 
         X_t = x_0 +  \mu t + \sigma W_t \ \ \ \ t \in [0,T]
 
     and each :math:`X_t \sim N(\mu t, \sigma^2 t)`.
 
-    Parameters:
 
-    :param float drift: the parameter :math:`\mu` in the above SDE
-    :param float scale: the parameter :math:`\sigma>0` in the above SDE
-    :param float initial: the initial condition :math:`x_0` in the above SDE
-    :param float T: the right hand endpoint of the time interval :math:`[0,T]`
-        for the process
-    :param numpy.random.Generator rng: a custom random number generator
+    :parameter float drift: the parameter :math:`\mu` in the above SDE
+    :parameter float scale: the parameter :math:`\sigma>0` in the above SDE
+    :parameter float initial: the initial condition :math:`x_0` in the above SDE
+    :parameter float T: the right hand endpoint of the time interval :math:`[0,T]` for the process
+    :parameter numpy.random.Generator rng: a custom random number generator
 
     """
 
-    def __init__(self, drift=0.0, scale=1.0, T=1.0, rng=None):
+    def __init__(self, drift=0.0, scale=1.0, initial=0.0, T=1.0, rng=None):
         super().__init__(T=T, rng=rng, initial=0.0)
         self.drift = drift
         self.scale = scale
-        self.name = "Brownian Motion" if drift == 0.0 else "Brownian Motion with Drift"
+        self.initial = initial
+        standard_condition = drift == 0.0 and scale == 1.0 and initial == 0.0
+        self.name = "Brownian Motion" if standard_condition else "Arithmetic Brownian Motion"
         self.n = None
         self.times = None
         self.gaussian_increments = GaussianIncrements(T=self.T, rng=self.rng)
 
     @property
     def drift(self):
         return self._drift
@@ -76,102 +76,128 @@
         return self._scale
 
     @scale.setter
     def scale(self, value):
         check_positive_number(value, "Scale")
         self._scale = value
 
+    @property
+    def initial(self):
+        return self._initial
+
+    @initial.setter
+    def initial(self, value):
+        self._initial = value
+
     def _sample_brownian_motion(self, n):
         self.n = n
         self.times = get_times(self.T, self.n)
-        bm = np.cumsum(self.scale * self.gaussian_increments.sample(n - 1))
-        bm = np.insert(bm, 0, [0])
-        if self.drift == 0:
-            return bm
-        else:
-            return self.times * self.drift + bm
+        # increments = np.random.normal(scale=np.sqrt(self.T/self.n), size=self.n)
+        increments = np.cumsum(self.gaussian_increments.sample(n - 1))
+        increments = np.insert(increments, 0, [0])
+
+        path = np.full(n, self.initial) + self.drift * self.times + self.scale * increments
+        # bm = np.cumsum(self.scale *self.gaussian_increments.sample(n - 1))
+        # bm = np.insert(bm, 0, [0])
+        # if self.drift == 0:
+        #     return bm
+        # else:
+        # return self.initial + self.drift+self.times + bm
+        return path
+
+    def __str__(self):
+
+        return "Brownian Motion with drift={drift}, and scale={scale} on [0, {T}].".format(
+            T=str(self.T), drift=str(self.drift), scale=str(self.scale),
+            initial=str(self.initial))
 
     def sample(self, n):
         """
         Generates a discrete time sample from a Brownian Motion instance.
 
-        :param n: the number of steps
+        :param int n: the number of steps
         :return: numpy array
         """
         return self._sample_brownian_motion(n)
 
     def _sample_brownian_motion_at(self, times):
+        if times[0] != 0:
+            times = np.insert(times, 0, [0])
         self.times = times
-        bm = np.cumsum(self.scale * self.gaussian_increments.sample_at(times))
 
-        if times[0] != 0:
-            bm = np.insert(bm, 0, [0])
+        increments = np.cumsum(self.gaussian_increments.sample_at(times))
+        # increments = np.insert(increments, 0, [0])
+
+        path = np.full(len(self.times), self.initial) + self.drift * self.times + self.scale * increments
+        # bm = np.cumsum(self.scale * self.gaussian_increments.sample_at(times))
 
-        if self.drift != 0:
-            bm += [self.drift * t for t in times]
+        #
+        # if self.drift != 0:
+        #     bm += [self.drift * t for t in times]
 
-        return bm
+        return path
 
     def sample_at(self, times):
         """
         Generates a sample from a Brownian motion at the specified times.
 
         :param times: the times which define the sample
         :return: numpy array
         """
         return self._sample_brownian_motion_at(times)
 
     def _process_expectation(self, times=None):
         if times is None:
             times = self.times
-        return self.drift * times
-
-    def marginal_expectation(self, times=None):
-        expectations = self._process_expectation(times=times)
-        return expectations
+        return self.initial + self.drift * times
 
     def _process_variance(self, times=None):
         if times is None:
             times = self.times
         return (self.scale ** 2) * times
 
-    def marginal_variance(self, times):
-        variances = self._process_variance(times=times)
-        return variances
-
-    def _process_stds(self):
-        return self.scale * np.sqrt(self.times)
+    def _process_stds(self, times=None):
+        if times is None:
+            times = self.times
+        return self.scale * np.sqrt(times)
 
     def process_stds(self):
         stds = self._process_stds()
         return stds
 
     def get_marginal(self, t):
-        marginal = norm(loc=self.drift * t, scale=self.scale * np.sqrt(t))
+        marginal = norm(loc=self.initial + self.drift * t, scale=self.scale * np.sqrt(t))
         return marginal
 
+    def marginal_expectation(self, times=None):
+        expectations = self._process_expectation(times=times)
+        return expectations
+
+    def marginal_variance(self, times):
+        variances = self._process_variance(times=times)
+        return variances
+
     def draw(self, n, N, marginal=True, envelope=False, type='3sigma', title=None, **fig_kw):
         """
         Simulates and plots paths/trajectories from the instanced stochastic process.
 
         Produces different kind of visualisation illustrating the following elements:
 
         - times versus process values as lines
         - the expectation of the process across time
         - histogram showing the empirical marginal distribution :math:`X_T` (optional when ``marginal = True``)
         - probability density function of the marginal distribution :math:`X_T` (optional when ``marginal = True``)
         - envelope of confidence intervals across time (optional when ``envelope = True``)
 
-
-        :param n: number of steps in each path
-        :param N: number of paths to simulate
-        :param marginal: bool, default: True
-        :param envelope: bool, default: False
-        :param type: string, default: '3sigma'
-        :param title: string to customise plot title
+        :param int n: number of steps in each path
+        :param int N: number of paths to simulate
+        :param bool marginal:  defaults to True
+        :param bool envelope:   defaults to False
+        :param str type:   defaults to  '3sigma'
+        :param str title:  to be used to customise plot title. If not passed, the title defaults to the name of the process.
         :return:
         """
 
         if type == '3sigma':
             return self._draw_3sigmastyle(n=n, N=N, marginal=marginal, envelope=envelope, title=title, **fig_kw)
         elif type == 'qq':
             return self._draw_qqstyle(n, N, marginal=marginal, envelope=envelope, title=title, **fig_kw)
```

### Comparing `aleatory-0.3.0/aleatory/processes/analytical/gaussian.py` & `aleatory-0.4.0/aleatory/processes/analytical/gaussian.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.3.0/aleatory/processes/analytical/geometric_brownian.py` & `aleatory-0.4.0/aleatory/processes/analytical/geometric_brownian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Geometric Brownian Motion
 """
 import numpy as np
 from scipy.stats import lognorm
 
-from aleatory.processes.base import SPExplicit
+from aleatory.processes.base_analytical import SPAnalytical
 from aleatory.processes.analytical.brownian_motion import BrownianMotion
 from aleatory.utils.utils import check_positive_number, check_numeric, get_times, check_positive_integer
 
 
-class GBM(SPExplicit):
+class GBM(SPAnalytical):
     r"""Geometric Brownian Motion
 
     .. image:: _static/geometric_brownian_motion_drawn.png
 
 
     A Geometric Brownian Motion :math:`\{X(t) : t \geq  0\}` is characterised by
     the following SDE.
@@ -122,33 +122,37 @@
         return self._sample_geometric_brownian_motion_at(times)
 
     def _process_expectation(self, times=None):
         if times is None:
             times = self.times
         return self.initial * np.exp(self.drift * times)
 
-    def marginal_expectation(self, times=None):
-        expectations = self._process_expectation(times=times)
-        return expectations
 
     def _process_variance(self, times=None):
         if times is None:
             times = self.times
         variances = (self.initial ** 2) * np.exp(2 * self.drift * times) * (
                 np.exp(times * self.volatility ** 2) - 1)
         return variances
 
-    def marginal_variance(self, times=None):
+    def _process_stds(self, times=None):
+        if times is None:
+            times = self.times
         variances = self._process_variance(times=times)
-        return variances
-
-    def _process_stds(self):
-        variances = self.marginal_variance()
         stds = np.sqrt(variances)
         return stds
 
+
     def get_marginal(self, t):
         mu_x = np.log(self.initial) + (self.drift - 0.5 * self.volatility ** 2) * t
         sigma_x = self.volatility * np.sqrt(t)
         marginal = lognorm(s=sigma_x, scale=np.exp(mu_x))
 
         return marginal
+
+    def marginal_expectation(self, times=None):
+        expectations = self._process_expectation(times=times)
+        return expectations
+
+    def marginal_variance(self, times=None):
+        variances = self._process_variance(times=times)
+        return variances
```

### Comparing `aleatory-0.3.0/aleatory/processes/base.py` & `aleatory-0.4.0/aleatory/processes/base_analytical.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,110 +1,108 @@
-from abc import ABC
 from abc import abstractmethod
 
 import numpy as np
 
-from aleatory.utils.utils import check_positive_number
-from aleatory.utils.utils import plot_paths, draw_paths, check_positive_integer, get_times
+from aleatory.processes.base import StochasticProcess
+from aleatory.utils.utils import plot_paths, draw_paths
 
 
-class BaseProcess(ABC):
-    def __init__(self, rng=None):
-        self.rng = rng
-
-    @property
-    def rng(self):
-        if self._rng is None:
-            return np.random.default_rng()
-        return self._rng
-
-    @rng.setter
-    def rng(self, value):
-        if value is None:
-            self._rng = None
-        elif isinstance(value, (np.random.RandomState, np.random.Generator)):
-            self._rng = value
-        else:
-            raise TypeError("rng must be of type `numpy.random.Generator`")
-
-
-class StochasticProcess(BaseProcess, ABC):
-    """
-    Base class for all one-factor stochastic processes classes.
-    All processes of this type are defined on a finite interval $[0,T]$.
-    """
-
-    def __init__(self, T=1.0, rng=None):
-        super().__init__(rng=rng)
-        self.T = T
-
-    @property
-    def T(self):
-        """End time of the process."""
-        return self._T
-
-    @T.setter
-    def T(self, value):
-        check_positive_number(value, "Time end")
-        self._T = float(value)
-
-
-class SPExplicit(StochasticProcess):
+class SPAnalytical(StochasticProcess):
 
     def __init__(self, initial=0.0, name=None, T=1.0, rng=None):
         super().__init__(T=T, rng=rng)
         self.initial = initial
         self.name = name
         self.n = None
         self.times = None
         self.N = None
         self.paths = None
+        self._empirical_marginals = None
 
     @abstractmethod
     def sample(self, n):  # pragma: no cover
         pass
 
     def simulate(self, n, N):
         """
         Simulate paths/trajectories from the instanced stochastic process.
 
-        :param n: number of steps in each path
-        :param N: number of paths to simulate
+        :param int n: number of steps in each path
+        :param int N: number of paths to simulate
         :return: list with N paths (each one is a numpy array of size n)
         """
         self.n = n
         self.N = N
         self.paths = [self.sample(n) for _ in range(N)]
         return self.paths
 
-    @abstractmethod
-    def get_marginal(self, t):
-        pass
+    def _get_empirical_marginal_samples(self):
+        if self.paths is None:
+            self.simulate(self.n, self.N)
+
+        empirical_marginal_samples = np.array(self.paths).transpose()
+        return empirical_marginal_samples
+
+    def estimate_expectations(self):
+        if self._empirical_marginals is None:
+            self._empirical_marginals = self._get_empirical_marginal_samples()
+        empirical_means = [np.mean(m) for m in self._empirical_marginals]
+        return empirical_means
+
+    def estimate_variances(self):
+        if self._empirical_marginals is None:
+            self._empirical_marginals = self._get_empirical_marginal_samples()
+        empirical_vars = [np.var(m) for m in self._empirical_marginals]
+        return empirical_vars
+
+    def estimate_stds(self):
+        variances = self.estimate_variances()
+        stds = [np.sqrt(var) for var in variances]
+        return stds
+
+    def estimate_quantiles(self, q):
+        if self._empirical_marginals is None:
+            self._empirical_marginals = self._get_empirical_marginal_samples()
+        empirical_quantiles = [np.quantile(m, q) for m in self._empirical_marginals]
+        return empirical_quantiles
 
-    @abstractmethod
     def _process_expectation(self):
-        pass
+        return self.estimate_expectations()
+
+    def process_expectation(self):
+        return self._process_expectation()
+
 
-    @abstractmethod
     def _process_variance(self):
-        pass
+        return self.estimate_variances()
+
+    def process_variance(self):
+        return self._process_variance()
 
-    @abstractmethod
     def _process_stds(self):
+        stds = np.sqrt(self.process_variance())
+        return stds
+
+    def process_stds(self):
+        stds = self._process_stds()
+        return stds
+
+    def get_marginal(self, t):
         pass
 
     def plot(self, n, N, title=None, **fig_kw):
         """
         Simulates and plots paths/trajectories from the instanced stochastic process.
         Simple plot of times versus process values as lines and/or markers.
 
-        :param n: number of steps in each path
-        :param N: number of paths to simulate
-        :param title: string to customise plot title
+        :parameter int n: number of steps in each path
+        :parameter int N: number of paths to simulate
+        :parameter str title: string to customise plot title
         :return:
+
         """
         self.simulate(n, N)
         if title:
             figure = plot_paths(self.times, self.paths, title=title, **fig_kw)
         else:
             figure = plot_paths(self.times, self.paths, title=self.name, **fig_kw)
         return figure
@@ -154,53 +152,15 @@
         Visualisation shows
         - times versus process values as lines
         - the expectation of the process across time
         - histogram showing the empirical marginal distribution :math:`X_T`
         - probability density function of the marginal distribution :math:`X_T`
         - envelope of confidence intervals
 
-        :param n: number of steps in each path
-        :param N: number of paths to simulate
-        :param marginal: bool, default: True
-        :param envelope: bool, default: False
-        :param title: string optional default to None
+        :param int n: number of steps in each path
+        :param int N: number of paths to simulate
+        :param bool marginal: defaults to True
+        :param bool envelope: defaults to False
+        :param str title: string optional default to the name of the process
         :return:
         """
         return self._draw_qqstyle(n, N, marginal=marginal, envelope=envelope, title=title, **fig_kw)
-
-
-class SPEulerMaruyama(SPExplicit):
-    def __int__(self, f=None, g=None, initial=0.0, T=1.0, rng=None):
-        super().__init__(T=T, rng=rng, initial=initial)
-        self.f = f
-        self.g = g
-        self.n = None
-        self.dt = None
-        self.times = None
-        self.name = None
-
-    def _sample_em_process(self, n, log=False):
-        check_positive_integer(n)
-        self.n = n
-        self.dt = 1.0 * self.T / self.n
-        self.times = get_times(self.T, self.n)
-        dws = self.rng.normal(scale=np.sqrt(self.dt), size=self.n)
-
-        if log:
-            origin = np.log(self.initial)
-        else:
-            origin = self.initial
-
-        path = [origin]
-        previous = origin
-
-        for (t, dw) in zip(self.times[1:], dws[1:]):
-            previous += self.f(previous, t) * self.dt + self.g(previous, t) * dw
-            path.append(previous)
-
-        if log:
-            return np.exp(path)
-
-        return path
-
-    def sample(self, n):
-        return self._sample_em_process(n)
```

### Comparing `aleatory-0.3.0/aleatory/processes/euler_maruyama/cev_process.py` & `aleatory-0.4.0/aleatory/processes/euler_maruyama/cir_process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,166 +1,168 @@
-"""
-Constant Elasticity Variance Process
-"""
-from aleatory.processes.base import SPEulerMaruyama
+from aleatory.processes.base_eu import SPEulerMaruyama
 import numpy as np
-from aleatory.utils.utils import draw_paths
+from scipy.stats import ncx2
 
 
-class CEVProcess(SPEulerMaruyama):
+class CIRProcess(SPEulerMaruyama):
     r"""
-    CEV or constant elasticity of variance process
+    Cox–Ingersoll–Ross Process
 
-    .. image:: _static/cev_process_drawn.png
+    .. image:: _static/cir_process_drawn.png
 
-
-    A CEV process  :math:`X = \{X : t \geq  0\}` is characterised by the following
+    A Cox–Ingersoll–Ross process :math:`X = \{X : t \geq  0\}` is characterised by the following
     Stochastic Differential Equation
 
     .. math::
 
-      dX_t = \mu X_t dt + \sigma X_t^{\gamma} dW_t, \ \ \ \ \forall t\in (0,T],
+      dX_t = \theta(\mu - X_t) dt + \sigma \sqrt{X_t} dW_t, \ \ \ \ \forall t\in (0,T],
 
     with initial condition :math:`X_0 = x_0`, where
 
-    - :math:`\mu` is the drift
-    - :math:`\sigma>0` is the scale of the volatility
-    - :math:`\gamma\geq 0` is the elasticity term
+    - :math:`\theta` is the rate of mean reversion
+    - :math:`\mu` is the long term mean value.
+    - :math:`\sigma>0` is the instantaneous volatility
     - :math:`W_t` is a standard Brownian Motion.
 
 
+    Each :math:`X_t` follows a non-central chi-square distribution.
+
+
+    :param float theta: the parameter :math:`\theta` in the above SDE
     :param float mu: the parameter :math:`\mu` in the above SDE
     :param float sigma: the parameter :math:`\sigma>0` in the above SDE
-    :param float gamma: the parameter :math:`\gamma` in the above SDE
     :param float initial: the initial condition :math:`x_0` in the above SDE
     :param float T: the right hand endpoint of the time interval :math:`[0,T]`
         for the process
     :param numpy.random.Generator rng: a custom random number generator
+
     """
 
-    def __init__(self, gamma=1.5, mu=0.5, sigma=0.1, initial=1.0, T=1.0, rng=None):
-        super().__init__(T=T, rng=rng)
-        self.gamma = gamma
+    def __init__(self, theta=1.0, mu=2.0, sigma=0.5, initial=5.0, T=1.0, rng=None):
+        super().__init__(T=T, rng=rng, initial=initial)
+        self.theta = theta
         self.mu = mu
         self.sigma = sigma
-        self.initial = initial
         self.n = 1.0
         self.dt = 1.0 * self.T / self.n
         self.times = np.arange(0.0, self.T + self.dt, self.dt)
-        self.name = "CEV Process"
-        self.paths = None
-        self._marginals = None
+        self.name = "CIR Process"
 
         def f(x, _):
-            return self.mu - 0.5 * (self.sigma ** 2) * np.exp(2.0 * (self.gamma - 1.0) * x)
-            # return self.mu * x
+            # return self.theta * (self.mu - x)
+            return np.exp(-x) * (self.theta * (self.mu - np.exp(x)) - 0.5 * self.sigma ** 2)
 
         def g(x, _):
-            return self.sigma * np.exp((self.gamma - 1.0) * x)
-            # return self.sigma * (x ** self.gamma)
+            # return self.sigma * np.sqrt(x)
+            return self.sigma * np.exp(-0.5 * x)
 
         self.f = f
         self.g = g
 
     @property
+    def theta(self):
+        return self._theta
+
+    @theta.setter
+    def theta(self, value):
+        if value < 0:
+            raise ValueError("theta must be positive")
+        self._theta = value
+
+    @property
     def sigma(self):
         return self._sigma
 
     @sigma.setter
     def sigma(self, value):
-        if value < 0:
-            raise ValueError("sigma cannot be negative")
+        if value <= 0:
+            raise ValueError("sigma has to be positive")
+        if 2 * self.theta * self.mu <= value ** 2:
+            raise ValueError("Condition 2*theta*mu >= sigma**2 must be satisfied")
         self._sigma = value
 
-    @property
-    def gamma(self):
-        return self._gamma
+    def __str__(self):
+        return "Cox–Ingersoll–Ross process with parameters {speed}, {mean}, and {volatility} on [0, {T}].".format(
+            T=str(self.T), speed=str(self.theta), mean=str(self.mu), volatility=str(self.sigma))
 
-    @gamma.setter
-    def gamma(self, value):
-        if value < 0:
-            raise ValueError("gamma cannot be negative")
-        self._gamma = value
+    def _process_expectation(self, times=None):
+        if times is None:
+            times = self.times
+        expectations = self.initial * np.exp((-1.0) * self.theta * times) + self.mu * (
+                np.ones(len(times)) - np.exp((-1.0) * self.theta * times))
+        return expectations
 
-    def __str__(self):
-        return "CEV process with parameters {gamma}, {drift}, and {volatility} on [0, {T}].".format(
-            T=str(self.T), gamma=str(self.gamma), drift=str(self.mu), volatility=str(self.sigma))
+    def marginal_expectation(self, times=None):
+        expectations = self._process_expectation(times=times)
+        return expectations
 
-    def _get_empirical_marginal_samples(self):
-        if self.paths is None:
-            self.simulate(self.n, self.N)
+    def _process_variance(self, times=None):
+        if times is None:
+            times = self.times
+        variances = (self.sigma ** 2 / self.theta) * self.initial * (
+                np.exp(-1.0 * self.theta * times) - np.exp(-2.0 * self.theta * times)) + (
+                            self.mu * self.sigma ** 2 / (2 * self.theta)) * (
+                            (np.ones(len(times)) - np.exp(-1.0 * self.theta * times)) ** 2)
+        return variances
 
-        empirical_marginal_samples = np.array(self.paths).transpose()
-        return empirical_marginal_samples
+    def _process_degrees_of_freedom(self):
+        df = 4.0 * self.theta * self.mu / (self.sigma ** 2)
 
-    def get_marginal(self, t):
-        pass
+        return df
 
-    def estimate_expectations(self):
-        if self._marginals is None:
-            self._marginals = self._get_empirical_marginal_samples()
-
-        empirical_means = [np.mean(m) for m in self._marginals]
-        return empirical_means
-
-    def estimate_variances(self):
-        if self._marginals is None:
-            self._marginals = self._get_empirical_marginal_samples()
-        empirical_vars = [np.var(m) for m in self._marginals]
-        return empirical_vars
-
-    def estimate_stds(self):
-        variances = self.estimate_variances()
-        stds = [np.sqrt(var) for var in variances]
-        return stds
+    def marginal_df(self):
+
+        return self._process_degrees_of_freedom()
+
+    def _process_nc_parameter(self, times=None):
+        if times is None:
+            times = self.times
+        c = 2.0 * self.theta / ((1.0 - np.exp(-1.0 * self.theta * times)) * self.sigma ** 2)
+        ncs = 2.0 * c * self.initial * np.exp(-1.0 * self.theta * times)
 
-    def estimate_quantiles(self, q):
-        if self._marginals is None:
-            self._marginals = self._get_empirical_marginal_samples()
-        empirical_quantiles = [np.quantile(m, q) for m in self._marginals]
-        return empirical_quantiles
-
-    def _process_expectation(self):
-        return self.estimate_expectations()
+        return ncs
 
-    def process_expectation(self):
-        return self._process_expectation()
+    def marginal_nc_parameter(self, times=None):
+        ncs = self._process_nc_parameter(times=times)
 
-    def _process_variance(self):
-        return self.estimate_variances()
+        return ncs
 
-    def process_variance(self):
-        return self._process_variance()
+    def _process_scales(self, times=None):
+        if times is None:
+            times = self.times
+        c = 2.0 * self.theta / ((1.0 - np.exp(-1.0 * self.theta * times)) * self.sigma ** 2)
+        scales = 1.0 / (2.0 * c)
+
+        return scales
+
+    def marginal_scale(self, times=None):
+        scales = self._process_scales(times=times)
+
+        return scales
+
+    def marginal_variance(self, times=None):
+        variances = self._process_variance(times=times)
+        return variances
 
     def _process_stds(self):
-        stds = np.sqrt(self.process_variance())
+        stds = np.sqrt(self._process_variance())
         return stds
 
     def process_stds(self):
         stds = self._process_stds()
         return stds
 
-    def draw(self, n, N, marginal=True, envelope=False, title=None, **fig_kw):
-        self.simulate(n, N)
-        expectations = self.estimate_expectations()
-
-        if envelope:
-            lower = self.estimate_quantiles(0.005)
-            upper = self.estimate_quantiles(0.995)
-        else:
-            lower = None
-            upper = None
-
-        chart_title = title if title else self.name
-
-        if marginal:
-            fig = draw_paths(times=self.times, paths=self.paths, N=N, title=chart_title, KDE=True, marginal=marginal,
-                             expectations=expectations, envelope=envelope, lower=lower, upper=upper,
-                             **fig_kw)
-        else:
-            fig = draw_paths(times=self.times, paths=self.paths, N=N, title=chart_title,
-                             expectations=expectations, marginal=marginal, **fig_kw)
+    def get_marginal(self, t):
+        a = self.theta
+        b = self.mu
+        sigma = self.sigma
+
+        c = 2.0 * a / ((1.0 - np.exp(-1.0 * a * t)) * sigma ** 2)
+        df = 4.0 * a * b / sigma ** 2
+        nc = 2.0 * c * self.initial * np.exp(-1.0 * a * t)
+        scale = 1.0 / (2 * c)
+        marginal = ncx2(df, nc, scale=scale)
 
-        return fig
+        return marginal
 
     def sample(self, n):
         return self._sample_em_process(n, log=True)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aleatory-0.3.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py` & `aleatory-0.4.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.3.0/aleatory/processes/euler_maruyama/vasicek.py` & `aleatory-0.4.0/aleatory/processes/euler_maruyama/vasicek.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Vasicek Process
 """
-from aleatory.processes.base import SPEulerMaruyama
+from aleatory.processes.base_eu import SPEulerMaruyama
 import numpy as np
 from scipy.stats import norm
 
 
 class Vasicek(SPEulerMaruyama):
     r"""
     Vasicek Process
@@ -18,15 +18,15 @@
 
     .. math::
 
       dX_t = \theta(\mu - X_t) dt + \sigma dW_t, \ \ \ \ \forall t\in (0,T],
 
     with initial condition :math:`X_0 = x_0`, where
 
-    - :math:`\theta` is the speed of reversion
+    - :math:`\theta>0` is the speed of reversion
     - :math:`\mu` is the long term mean value.
     - :math:`\sigma>0` is the instantaneous volatility
     - :math:`W_t` is a standard Brownian Motion.
 
 
     Each :math:`X_t` follows a normal distribution.
 
@@ -56,29 +56,40 @@
 
         def g(x, _):
             return self.sigma
 
         self.f = f
         self.g = g
 
+    @property
+    def theta(self):
+        return self._theta
+
+    @theta.setter
+    def theta(self, value):
+        if value < 0:
+            raise ValueError("theta parameter must be positive")
+        self._theta = value
+
     def __str__(self):
-        return "Vasicek process with parameters {speed}, {mean}, and {volatility} on [0, {T}].".format(
-            T=str(self.T), speed=str(self.theta), mean=str(self.mu), volatility=str(self.sigma))
+        return "Vasicek process with parameters theta={speed}, mu={mean}, sigma={volatility}, initial={initial} on [0, {T}].".format(
+            T=str(self.T), speed=str(self.theta), mean=str(self.mu), volatility=str(self.sigma),
+            initial=str(self.initial))
 
     def _process_expectation(self, times=None):
         if times is None:
             times = self.times
         return self.initial * np.exp((-1.0) * self.theta * times) + self.mu * (
                 np.ones(len(times)) - np.exp((-1.0) * self.theta * times))
 
     def marginal_expectation(self, times=None):
         expectations = self._process_expectation(times=times)
         return expectations
 
-    def _process_variance(self,times=None):
+    def _process_variance(self, times=None):
         if times is None:
             times = self.times
         variances = (self.sigma ** 2) * (1.0 / (2.0 * self.theta)) * (
                 np.ones(len(times)) - np.exp(-2.0 * self.theta * times))
         return variances
 
     def marginal_variance(self, times=None):
```

### Comparing `aleatory-0.3.0/aleatory/stats/non_central_chi.py` & `aleatory-0.4.0/aleatory/stats/non_central_chi.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.3.0/aleatory/utils/utils.py` & `aleatory-0.4.0/aleatory/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,23 +103,25 @@
             colors = [col[b] for b in my_bins]
 
             if KDE:
                 kde = sm.nonparametric.KDEUnivariate(last_points)
                 kde.fit()  # Estimate the densities
                 ax2.plot(kde.density, kde.support, '--', lw=1.75, alpha=0.6, label='$X_T$  KDE', zorder=10)
                 ax2.axhline(y=np.mean(last_points), linestyle='--', lw=1.75, label=r'$\overline{X_T}$')
+                ax2.legend()
             elif marginal and marginalT:
                 marginaldist = marginalT
                 x = np.linspace(marginaldist.ppf(0.001), marginaldist.ppf(0.999), 100)
                 ax2.plot(marginaldist.pdf(x), x, '-', lw=1.75, alpha=0.6, label='$X_T$ pdf')
                 ax2.axhline(y=marginaldist.mean(), linestyle='--', lw=1.75, label='$E[X_T]$')
+                ax2.legend()
 
             plt.setp(ax2.get_yticklabels(), visible=False)
             ax2.set_title('$X_T$')
-            ax2.legend()
+
 
             for i in range(N):
                 ax1.plot(times, paths[i], '-', lw=1.0, color=cm(colors[i]))
 
             if expectations is not None:
                 ax1.plot(times, expectations, '--', lw=1.75, label='$E[X_t]$')
                 ax1.legend()
```

### Comparing `aleatory-0.3.0/aleatory.egg-info/PKG-INFO` & `aleatory-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleatory
-Version: 0.3.0
+Version: 0.4.0
 Summary: Stochastic Processes Simulation and Visualisation
 Author-email: Dialid Santiago <d.santiago@outlook.com>
 Project-URL: Homepage, https://github.com/quantgirluk/aleatory
 Project-URL: Bug Tracker, https://github.com/quantgirluk/aleatory/issues
 Project-URL: Documentation, https://aleatory.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,14 @@
 Requires-Dist: matplotlib>=3.6.2
 Requires-Dist: statsmodels>=0.13.5
 Requires-Dist: parameterized>=0.8.1
 
 # *aleatory*
 
 [![PyPI version fury.io](https://badge.fury.io/py/aleatory.svg)](https://pypi.org/project/aleatory/) [![Downloads](https://static.pepy.tech/personalized-badge/aleatory?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/aleatory)
-
 ![example workflow](https://github.com/quantgirluk/aleatory/actions/workflows/python-package.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/aleatory/badge/?version=latest)](https://aleatory.readthedocs.io/en/latest/?badge=latest)
 
 - [Git Homepage](https://github.com/quantgirluk/aleatory)
 - [Pip Repository](https://pypi.org/project/aleatory/)
 - [Documentation](https://aleatory.readthedocs.io/en/latest/)
 
 ## Overview
@@ -41,27 +40,29 @@
 - create visualisations to illustrate the processes properties and behaviour
 
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/vasicek_process_drawn.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
 </p>
 
-Currently, `aleatory` supports the following processes:
+Currently, `aleatory` supports the following 13 processes:
 
 - Brownian Motion
 - Brownian Bridge
 - Brownian Excursion
 - Brownian Meander
-- Geometric Brownian Motion
-- Ornstein–Uhlenbeck
-- Vasicek
-- Cox–Ingersoll–Ross
-- Constant Elasticity
-- Bessel Process
-- Squared Bessel Processs
+- Geometric Brownian Motion (GBM) process
+- Ornstein–Uhlenbeck (OU) process
+- Vasicek process
+- Cox–Ingersoll–Ross (CIR) process
+- Constant Elasticity Variance (CEV) process
+- Chan-Karolyi-Longstaff-Sanders (CKLS) process
+- Bessel (BES) process
+- Squared Bessel (BESQ) process
+- Poisson process
 
 ## Installation
 
 Aleatory is available on [pypi](https://pypi.python.org/pypi) and can be
 installed as follows
 
 ```
@@ -74,15 +75,15 @@
 
 - ``numpy``  for random number generation
 - ``scipy`` and ``statsmodels`` for support for a number of one-dimensional distributions.
 - ``matplotlib`` for creating visualisations
 
 ## Compatibility
 
-Aleatory is tested on Python versions 3.8, 3.9, and 3.10
+Aleatory is tested on Python versions 3.8, 3.9, 3.10, and 3.11
 
 ## Quick-Start
 
 Aleatory allows you to create fancy visualisations from different stochastic processes in an easy and concise way.
 
 For example, the following code
 
@@ -99,15 +100,15 @@
 <p align="center">
 <img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"   style="display:block;float:none;margin-left:auto;margin-right:auto;width:80%">
 </p>
 
 For more examples visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
 
 
-⭐️ **If you like this project, please give it a star!** ⭐️
+**If you like this project, please give it a star!** ⭐️
 
 ## Thanks for Visiting! ✨
 
 Connect with me via:
 
 - 🦜 [Twitter](https://twitter.com/Quant_Girl)
 - 👩🏽‍💼 [Linkedin](https://www.linkedin.com/in/dialidsantiago/)
```

### Comparing `aleatory-0.3.0/aleatory.egg-info/SOURCES.txt` & `aleatory-0.4.0/aleatory.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,30 +5,38 @@
 aleatory.egg-info/PKG-INFO
 aleatory.egg-info/SOURCES.txt
 aleatory.egg-info/dependency_links.txt
 aleatory.egg-info/requires.txt
 aleatory.egg-info/top_level.txt
 aleatory/processes/__init__.py
 aleatory/processes/base.py
+aleatory/processes/base_analytical.py
+aleatory/processes/base_eu.py
 aleatory/processes/analytical/__init__.py
 aleatory/processes/analytical/bes.py
 aleatory/processes/analytical/besq.py
 aleatory/processes/analytical/brownian_bridge.py
 aleatory/processes/analytical/brownian_excursion.py
 aleatory/processes/analytical/brownian_meander.py
 aleatory/processes/analytical/brownian_motion.py
 aleatory/processes/analytical/gaussian.py
 aleatory/processes/analytical/geometric_brownian.py
 aleatory/processes/euler_maruyama/__init__.py
 aleatory/processes/euler_maruyama/cev_process.py
 aleatory/processes/euler_maruyama/cir_process.py
+aleatory/processes/euler_maruyama/ckls_process.py
+aleatory/processes/euler_maruyama/ckls_process_generic.py
 aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py
 aleatory/processes/euler_maruyama/vasicek.py
+aleatory/processes/jump/__init__.py
+aleatory/processes/jump/poisson.py
 aleatory/stats/__init__.py
 aleatory/stats/non_central_chi.py
 aleatory/utils/__init__.py
 aleatory/utils/utils.py
 tests/test_bes.py
+tests/test_bm.py
 tests/test_charts.py
+tests/test_ckls.py
 tests/test_marginal_functions.py
 tests/test_ncx.py
 tests/test_transormation_em.py
```

### Comparing `aleatory-0.3.0/pyproject.toml` & `aleatory-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aleatory"
-version = "0.3.0"
+version = "0.4.0"
 authors = [{ name = "Dialid Santiago", email = "d.santiago@outlook.com" }, ]
 description = "Stochastic Processes Simulation and Visualisation"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["pandas>=1.5.2",
                 "numpy>=1.23.5",
                 "scipy>=1.9.3",
```

### Comparing `aleatory-0.3.0/tests/test_bes.py` & `aleatory-0.4.0/tests/test_bes.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.3.0/tests/test_charts.py` & `aleatory-0.4.0/tests/test_charts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import matplotlib.figure
 import numpy as np
 
 from aleatory.processes import (BrownianMotion, GBM, Vasicek, OUProcess, CIRProcess, CEVProcess, BESProcess,
-                                BESQProcess, BrownianBridge, BrownianExcursion, BrownianMeander)
+                                BESQProcess, BrownianBridge, BrownianExcursion, BrownianMeander,
+                                CKLSProcess)
 
 SAVE = False
 SAVE_PATH = '../docs/source/_static/'
 
 
 def test_sample(n=100):
     process = BrownianMotion()
@@ -36,14 +37,15 @@
 
     for v1, v2 in zip(sim1[0], sim2[0]):
         assert v1 == v2
 
 
 def test_figures_examples():
     bm = BrownianMotion()
+    bm_arithmetic = BrownianMotion(initial=1.0, drift=1.0, scale=2.5)
     bridge = BrownianBridge(initial=1.0, end=2.0)
     excursion = BrownianExcursion()
     meander = BrownianMeander()
     meander_end = BrownianMeander(fixed_end=True, end=2.0)
     meander_end_automatic = BrownianMeander(fixed_end=True)
     bmd = BrownianMotion(drift=-1.0, scale=0.5)
     gbm = GBM()
@@ -51,22 +53,26 @@
     ouprocess = OUProcess()
     cirprocess = CIRProcess()
     cev = CEVProcess()
     bes = BESProcess(dim=10)
     bes_float = BESProcess(dim=4.5)
     besq = BESQProcess(dim=10)
     besq_float = BESQProcess(dim=3.5)
+    ckls = CKLSProcess()
 
-    processes = [bridge, excursion, meander, meander_end, meander_end_automatic]
+    # processes = [cirprocess]
+    # processes = [bridge, excursion, meander, meander_end, meander_end_automatic]
+    # processes = [cirprocess, cev]
     # processes = [bm, bmd, bridge, excursion, meander, gbm, vasicek, ouprocess, cirprocess, cev, bes, besq, bes_float, besq_float]
-    # [bm, besq_float, bes_float]
+    # processes = [bm, besq_float, bes_float]
     # processes = [gbm, vasicek, ouprocess, cirprocess, cev, bes, besq]
     # processes = [bes_float, besq_float]
     # processes = [bm, bmd, bridge, excursion, meander, meander_end]
     # [bm, bmd, gbm,  cirprocess, cev, bes, besq, bes_float, besq_float]
+    processes = [ckls]
     style = "https://raw.githubusercontent.com/quantgirluk/matplotlib-stylesheets/main/quant-pastel-light.mplstyle"
     # with plt.style.context(style):
     for process in processes:
         process.plot(n=100, N=5, figsize=(9.5, 6), dpi=200)
         # process.plot(n=100, N=5, title='My favourite figure', figsize=(9.5, 6), dpi=200)  # figure_with_title
         #
         name = process.name.replace(" ", "_").lower()
```

### Comparing `aleatory-0.3.0/tests/test_marginal_functions.py` & `aleatory-0.4.0/tests/test_marginal_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,9 +16,7 @@
             assert m == drift * t
 
         for v, t in zip(variances, grid_times):
             assert v == (scale ** 2) * t
 
         for m, t in zip(means, process.times):
             assert m == drift * t
-
-
```

### Comparing `aleatory-0.3.0/tests/test_ncx.py` & `aleatory-0.4.0/tests/test_ncx.py`

 * *Files identical despite different names*

