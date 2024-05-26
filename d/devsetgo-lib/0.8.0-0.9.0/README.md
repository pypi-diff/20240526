# Comparing `tmp/devsetgo_lib-0.8.0.tar.gz` & `tmp/devsetgo_lib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devsetgo_lib-0.8.0.tar", last modified: Sun Mar 13 02:07:54 2022, max compression
+gzip compressed data, was "devsetgo_lib-0.9.0.tar", last modified: Sun Dec  4 21:55:33 2022, max compression
```

## Comparing `devsetgo_lib-0.8.0.tar` & `devsetgo_lib-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-13 02:07:54.676305 devsetgo_lib-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-03-13 02:07:45.000000 devsetgo_lib-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-03-13 02:07:54.676305 devsetgo_lib-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-03-13 02:07:45.000000 devsetgo_lib-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-13 02:07:54.676305 devsetgo_lib-0.8.0/devsetgo_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-03-13 02:07:54.000000 devsetgo_lib-0.8.0/devsetgo_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-03-13 02:07:54.000000 devsetgo_lib-0.8.0/devsetgo_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-13 02:07:54.000000 devsetgo_lib-0.8.0/devsetgo_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-13 02:07:54.000000 devsetgo_lib-0.8.0/devsetgo_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-03-13 02:07:54.000000 devsetgo_lib-0.8.0/devsetgo_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-13 02:07:54.676305 devsetgo_lib-0.8.0/dsg_lib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-13 02:07:45.000000 devsetgo_lib-0.8.0/dsg_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-03-13 02:07:45.000000 devsetgo_lib-0.8.0/dsg_lib/calendar_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11107 2022-03-13 02:07:45.000000 devsetgo_lib-0.8.0/dsg_lib/file_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-03-13 02:07:45.000000 devsetgo_lib-0.8.0/dsg_lib/folder_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5346 2022-03-13 02:07:45.000000 devsetgo_lib-0.8.0/dsg_lib/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-03-13 02:07:45.000000 devsetgo_lib-0.8.0/dsg_lib/patterns.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-03-13 02:07:54.676305 devsetgo_lib-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-03-13 02:07:45.000000 devsetgo_lib-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:55:33.948248 devsetgo_lib-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-04 21:55:25.000000 devsetgo_lib-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2022-12-04 21:55:33.948248 devsetgo_lib-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2022-12-04 21:55:25.000000 devsetgo_lib-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:55:33.948248 devsetgo_lib-0.9.0/devsetgo_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2022-12-04 21:55:33.000000 devsetgo_lib-0.9.0/devsetgo_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2022-12-04 21:55:33.000000 devsetgo_lib-0.9.0/devsetgo_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 21:55:33.000000 devsetgo_lib-0.9.0/devsetgo_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-04 21:55:33.000000 devsetgo_lib-0.9.0/devsetgo_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-04 21:55:33.000000 devsetgo_lib-0.9.0/devsetgo_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:55:33.948248 devsetgo_lib-0.9.0/dsg_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 21:55:25.000000 devsetgo_lib-0.9.0/dsg_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2022-12-04 21:55:25.000000 devsetgo_lib-0.9.0/dsg_lib/calendar_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2022-12-04 21:55:25.000000 devsetgo_lib-0.9.0/dsg_lib/file_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2022-12-04 21:55:25.000000 devsetgo_lib-0.9.0/dsg_lib/folder_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2022-12-04 21:55:25.000000 devsetgo_lib-0.9.0/dsg_lib/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2022-12-04 21:55:25.000000 devsetgo_lib-0.9.0/dsg_lib/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2022-12-04 21:55:33.948248 devsetgo_lib-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2022-12-04 21:55:25.000000 devsetgo_lib-0.9.0/setup.py
```

### Comparing `devsetgo_lib-0.8.0/LICENSE` & `devsetgo_lib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devsetgo_lib-0.8.0/PKG-INFO` & `devsetgo_lib-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: devsetgo_lib
-Version: 0.8.0
+Version: 0.9.0
 Summary: Common functions for applications
 Home-page: https://github.com/devsetgo/dev_com_lib
 Author: Mike Ryan
 Author-email: mikeryan56@gmail.com
 License: MIT
 Project-URL: Documentation, https://devsetgo.github.io/devsetgo_lib/
 Project-URL: Source, https://github.com/devsetgo/devsetgo_lib
 Keywords: file,folder,loguru,logging,CSV,JSON,Text,Regex
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -23,14 +22,15 @@
 Python:
 
 [![PyPI version fury.io](https://badge.fury.io/py/devsetgo-lib.svg)](https://pypi.python.org/pypi/devsetgo-lib/)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 
 CI/CD Pipeline:
 [![Actions Status](https://github.com/devsetgo/dsg_lib./workflows/PythonPackage/badge.svg)](https://github.com/devsetgo/dsg_lib./actions)
 
 SonarCloud:
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=devsetgo_devsetgo_lib&metric=coverage)](https://sonarcloud.io/dashboard?id=devsetgo_devsetgo_lib)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=devsetgo_devsetgo_lib&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=devsetgo_devsetgo_lib)
@@ -64,8 +64,7 @@
     - Get Month
 
 - Patterns
     - Patter Between
 
 - Logging
     - logging configuration and interceptor
-
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: devsetgo_lib Version: 0.8.0 Summary: Common
+Metadata-Version: 2.1 Name: devsetgo_lib Version: 0.9.0 Summary: Common
 functions for applications Home-page: https://github.com/devsetgo/dev_com_lib
 Author: Mike Ryan Author-email: mikeryan56@gmail.com License: MIT Project-URL:
 Documentation, https://devsetgo.github.io/devsetgo_lib/ Project-URL: Source,
 https://github.com/devsetgo/devsetgo_lib Keywords:
-file,folder,loguru,logging,CSV,JSON,Text,Regex Platform: UNKNOWN Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Operating
-System :: POSIX Classifier: Operating System :: MacOS :: MacOS X Classifier:
-Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Python: [![PyPI version
-fury.io](https://badge.fury.io/py/devsetgo-lib.svg)](https://pypi.python.org/
-pypi/devsetgo-lib/) _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_!_[_P_y_t_h_o_n_ _3_._7_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._7_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-
-_3_7_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._8_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/
-_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_8_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._9_]_(_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._9_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/
-_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_9_0_/_)_ _C_I_/_C_D_ _P_i_p_e_l_i_n_e_:_ _[_!_[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
-_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_w_o_r_k_f_l_o_w_s_/_P_y_t_h_o_n_P_a_c_k_a_g_e_/_b_a_d_g_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
-_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_a_c_t_i_o_n_s_)_ _S_o_n_a_r_C_l_o_u_d_:_ _[_!_[_C_o_v_e_r_a_g_e_]_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/
-_p_r_o_j_e_c_t___b_a_d_g_e_s_/_m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_c_o_v_e_r_a_g_e_)_]_(_h_t_t_p_s_:_/_/
-_s_o_n_a_r_c_l_o_u_d_._i_o_/_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_M_a_i_n_t_a_i_n_a_b_i_l_i_t_y_ _R_a_t_i_n_g_]
-_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
+file,folder,loguru,logging,CSV,JSON,Text,Regex Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: Microsoft :: Windows Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE Python: [![PyPI version fury.io](https://
+badge.fury.io/py/devsetgo-lib.svg)](https://pypi.python.org/pypi/devsetgo-lib/
+) _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_!_[_P_y_t_h_o_n_ _3_._7_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._7_-
+_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_7_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._8_]
+_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/
+_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_8_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._9_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_p_y_t_h_o_n_-_3_._9_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_9_0_/_)_ _[_!
+_[_P_y_t_h_o_n_ _3_._1_0_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._1_0_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/
+_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_1_0_0_/_)_ _C_I_/_C_D_ _P_i_p_e_l_i_n_e_:_ _[_!_[_A_c_t_i_o_n_s
+_S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_w_o_r_k_f_l_o_w_s_/_P_y_t_h_o_n_P_a_c_k_a_g_e_/
+_b_a_d_g_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_a_c_t_i_o_n_s_)_ _S_o_n_a_r_C_l_o_u_d_:_ _[_!
+_[_C_o_v_e_r_a_g_e_]_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
+_m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_c_o_v_e_r_a_g_e_)_]_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/
+_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_M_a_i_n_t_a_i_n_a_b_i_l_i_t_y_ _R_a_t_i_n_g_]_(_h_t_t_p_s_:_/_/
+_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
 _m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_s_q_a_l_e___r_a_t_i_n_g_)_]_(_h_t_t_p_s_:_/_/
 _s_o_n_a_r_c_l_o_u_d_._i_o_/_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_Q_u_a_l_i_t_y_ _G_a_t_e_ _S_t_a_t_u_s_]
 _(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
 _m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_a_l_e_r_t___s_t_a_t_u_s_)_]_(_h_t_t_p_s_:_/_/
 _s_o_n_a_r_c_l_o_u_d_._i_o_/_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_R_e_l_i_a_b_i_l_i_t_y_ _R_a_t_i_n_g_]_(_h_t_t_p_s_:
 _/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
 _m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_r_e_l_i_a_b_i_l_i_t_y___r_a_t_i_n_g_)_]_(_h_t_t_p_s_:_/_/
```

### Comparing `devsetgo_lib-0.8.0/README.md` & `devsetgo_lib-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Python:
 
 [![PyPI version fury.io](https://badge.fury.io/py/devsetgo-lib.svg)](https://pypi.python.org/pypi/devsetgo-lib/)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 
 CI/CD Pipeline:
 [![Actions Status](https://github.com/devsetgo/dsg_lib./workflows/PythonPackage/badge.svg)](https://github.com/devsetgo/dsg_lib./actions)
 
 SonarCloud:
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=devsetgo_devsetgo_lib&metric=coverage)](https://sonarcloud.io/dashboard?id=devsetgo_devsetgo_lib)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=devsetgo_devsetgo_lib&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=devsetgo_devsetgo_lib)
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
 Python: [![PyPI version fury.io](https://badge.fury.io/py/devsetgo-lib.svg)]
 (https://pypi.python.org/pypi/devsetgo-lib/) _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_!_[_P_y_t_h_o_n_ _3_._7_]
 _(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._7_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/
 _d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_7_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._8_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
 _p_y_t_h_o_n_-_3_._8_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_8_0_/_)_ _[_!
 _[_P_y_t_h_o_n_ _3_._9_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._9_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/
-_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_9_0_/_)_ _C_I_/_C_D_ _P_i_p_e_l_i_n_e_:_ _[_!_[_A_c_t_i_o_n_s
-_S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_w_o_r_k_f_l_o_w_s_/_P_y_t_h_o_n_P_a_c_k_a_g_e_/
-_b_a_d_g_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_a_c_t_i_o_n_s_)_ _S_o_n_a_r_C_l_o_u_d_:_ _[_!
-_[_C_o_v_e_r_a_g_e_]_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
-_m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_c_o_v_e_r_a_g_e_)_]_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/
-_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_M_a_i_n_t_a_i_n_a_b_i_l_i_t_y_ _R_a_t_i_n_g_]_(_h_t_t_p_s_:_/_/
-_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
+_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_9_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._1_0_]_(_h_t_t_p_s_:_/_/
+_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._1_0_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/
+_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_1_0_0_/_)_ _C_I_/_C_D_ _P_i_p_e_l_i_n_e_:_ _[_!_[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
+_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_w_o_r_k_f_l_o_w_s_/_P_y_t_h_o_n_P_a_c_k_a_g_e_/_b_a_d_g_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
+_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_a_c_t_i_o_n_s_)_ _S_o_n_a_r_C_l_o_u_d_:_ _[_!_[_C_o_v_e_r_a_g_e_]_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/
+_p_r_o_j_e_c_t___b_a_d_g_e_s_/_m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_c_o_v_e_r_a_g_e_)_]_(_h_t_t_p_s_:_/_/
+_s_o_n_a_r_c_l_o_u_d_._i_o_/_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_M_a_i_n_t_a_i_n_a_b_i_l_i_t_y_ _R_a_t_i_n_g_]
+_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
 _m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_s_q_a_l_e___r_a_t_i_n_g_)_]_(_h_t_t_p_s_:_/_/
 _s_o_n_a_r_c_l_o_u_d_._i_o_/_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_Q_u_a_l_i_t_y_ _G_a_t_e_ _S_t_a_t_u_s_]
 _(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
 _m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_a_l_e_r_t___s_t_a_t_u_s_)_]_(_h_t_t_p_s_:_/_/
 _s_o_n_a_r_c_l_o_u_d_._i_o_/_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_R_e_l_i_a_b_i_l_i_t_y_ _R_a_t_i_n_g_]_(_h_t_t_p_s_:
 _/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
 _m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_r_e_l_i_a_b_i_l_i_t_y___r_a_t_i_n_g_)_]_(_h_t_t_p_s_:_/_/
```

### Comparing `devsetgo_lib-0.8.0/devsetgo_lib.egg-info/PKG-INFO` & `devsetgo_lib-0.9.0/devsetgo_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: devsetgo-lib
-Version: 0.8.0
+Version: 0.9.0
 Summary: Common functions for applications
 Home-page: https://github.com/devsetgo/dev_com_lib
 Author: Mike Ryan
 Author-email: mikeryan56@gmail.com
 License: MIT
 Project-URL: Documentation, https://devsetgo.github.io/devsetgo_lib/
 Project-URL: Source, https://github.com/devsetgo/devsetgo_lib
 Keywords: file,folder,loguru,logging,CSV,JSON,Text,Regex
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.8
@@ -23,14 +22,15 @@
 Python:
 
 [![PyPI version fury.io](https://badge.fury.io/py/devsetgo-lib.svg)](https://pypi.python.org/pypi/devsetgo-lib/)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 
 CI/CD Pipeline:
 [![Actions Status](https://github.com/devsetgo/dsg_lib./workflows/PythonPackage/badge.svg)](https://github.com/devsetgo/dsg_lib./actions)
 
 SonarCloud:
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=devsetgo_devsetgo_lib&metric=coverage)](https://sonarcloud.io/dashboard?id=devsetgo_devsetgo_lib)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=devsetgo_devsetgo_lib&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=devsetgo_devsetgo_lib)
@@ -64,8 +64,7 @@
     - Get Month
 
 - Patterns
     - Patter Between
 
 - Logging
     - logging configuration and interceptor
-
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: devsetgo-lib Version: 0.8.0 Summary: Common
+Metadata-Version: 2.1 Name: devsetgo-lib Version: 0.9.0 Summary: Common
 functions for applications Home-page: https://github.com/devsetgo/dev_com_lib
 Author: Mike Ryan Author-email: mikeryan56@gmail.com License: MIT Project-URL:
 Documentation, https://devsetgo.github.io/devsetgo_lib/ Project-URL: Source,
 https://github.com/devsetgo/devsetgo_lib Keywords:
-file,folder,loguru,logging,CSV,JSON,Text,Regex Platform: UNKNOWN Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Operating
-System :: POSIX Classifier: Operating System :: MacOS :: MacOS X Classifier:
-Operating System :: Microsoft :: Windows Requires-Python: >=3.8 Description-
-Content-Type: text/markdown License-File: LICENSE Python: [![PyPI version
-fury.io](https://badge.fury.io/py/devsetgo-lib.svg)](https://pypi.python.org/
-pypi/devsetgo-lib/) _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_!_[_P_y_t_h_o_n_ _3_._7_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._7_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-
-_3_7_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._8_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/
-_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_8_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._9_]_(_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._9_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/
-_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_9_0_/_)_ _C_I_/_C_D_ _P_i_p_e_l_i_n_e_:_ _[_!_[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
-_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_w_o_r_k_f_l_o_w_s_/_P_y_t_h_o_n_P_a_c_k_a_g_e_/_b_a_d_g_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
-_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_a_c_t_i_o_n_s_)_ _S_o_n_a_r_C_l_o_u_d_:_ _[_!_[_C_o_v_e_r_a_g_e_]_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/
-_p_r_o_j_e_c_t___b_a_d_g_e_s_/_m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_c_o_v_e_r_a_g_e_)_]_(_h_t_t_p_s_:_/_/
-_s_o_n_a_r_c_l_o_u_d_._i_o_/_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_M_a_i_n_t_a_i_n_a_b_i_l_i_t_y_ _R_a_t_i_n_g_]
-_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
+file,folder,loguru,logging,CSV,JSON,Text,Regex Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
+:: Microsoft :: Windows Requires-Python: >=3.8 Description-Content-Type: text/
+markdown License-File: LICENSE Python: [![PyPI version fury.io](https://
+badge.fury.io/py/devsetgo-lib.svg)](https://pypi.python.org/pypi/devsetgo-lib/
+) _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_!_[_P_y_t_h_o_n_ _3_._7_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._7_-
+_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_7_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._8_]
+_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/
+_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_8_0_/_)_ _[_!_[_P_y_t_h_o_n_ _3_._9_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_p_y_t_h_o_n_-_3_._9_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_9_0_/_)_ _[_!
+_[_P_y_t_h_o_n_ _3_._1_0_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._1_0_-_b_l_u_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/
+_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/_r_e_l_e_a_s_e_/_p_y_t_h_o_n_-_3_1_0_0_/_)_ _C_I_/_C_D_ _P_i_p_e_l_i_n_e_:_ _[_!_[_A_c_t_i_o_n_s
+_S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_w_o_r_k_f_l_o_w_s_/_P_y_t_h_o_n_P_a_c_k_a_g_e_/
+_b_a_d_g_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_e_v_s_e_t_g_o_/_d_s_g___l_i_b_._/_a_c_t_i_o_n_s_)_ _S_o_n_a_r_C_l_o_u_d_:_ _[_!
+_[_C_o_v_e_r_a_g_e_]_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
+_m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_c_o_v_e_r_a_g_e_)_]_(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/
+_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_M_a_i_n_t_a_i_n_a_b_i_l_i_t_y_ _R_a_t_i_n_g_]_(_h_t_t_p_s_:_/_/
+_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
 _m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_s_q_a_l_e___r_a_t_i_n_g_)_]_(_h_t_t_p_s_:_/_/
 _s_o_n_a_r_c_l_o_u_d_._i_o_/_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_Q_u_a_l_i_t_y_ _G_a_t_e_ _S_t_a_t_u_s_]
 _(_h_t_t_p_s_:_/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
 _m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_a_l_e_r_t___s_t_a_t_u_s_)_]_(_h_t_t_p_s_:_/_/
 _s_o_n_a_r_c_l_o_u_d_._i_o_/_d_a_s_h_b_o_a_r_d_?_i_d_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_)_ _[_!_[_R_e_l_i_a_b_i_l_i_t_y_ _R_a_t_i_n_g_]_(_h_t_t_p_s_:
 _/_/_s_o_n_a_r_c_l_o_u_d_._i_o_/_a_p_i_/_p_r_o_j_e_c_t___b_a_d_g_e_s_/
 _m_e_a_s_u_r_e_?_p_r_o_j_e_c_t_=_d_e_v_s_e_t_g_o___d_e_v_s_e_t_g_o___l_i_b_&_m_e_t_r_i_c_=_r_e_l_i_a_b_i_l_i_t_y___r_a_t_i_n_g_)_]_(_h_t_t_p_s_:_/_/
```

### Comparing `devsetgo_lib-0.8.0/dsg_lib/file_functions.py` & `devsetgo_lib-0.9.0/dsg_lib/file_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,30 +159,65 @@
     # open/create file
     with open(file_save, "w+", encoding="utf-8", newline="") as write_file:
         # write data to file
         file_writer = csv.writer(
             write_file,
             delimiter=delimiter,
             quotechar=quotechar,
-            quoting=csv.QUOTE_MINIMAL,
         )
         for row in data:
             file_writer.writerow(row)
 
     logging.info(f"File Create: {file_name}")
     return "complete"
 
 
 # CSV Open file
 # pass file name and optional delimiter (default is ',')
 # Output is dictionary/json
 # expectation is for file to be quote minimal and skipping initial spaces is
 # a good thing
 # modify as needed
-def open_csv(file_name: str, delimit: str = None) -> list:
+def open_csv(
+    file_name: str,
+    delimit: str = None,
+    quote_level: str = None,
+    skip_initial_space: bool = True,
+) -> list:
+
+    quote_level_list: list = ["none", "minimal", "all"]
+    # TODO: figure out how non-numeric is supposed to work
+    # Python documentation as needed https://docs.python.org/3/library/csv.html
+
+    if quote_level is None:
+        quoting = csv.QUOTE_MINIMAL
+
+    elif quote_level.lower() not in quote_level_list:
+        error = f"quote_level '{quote_level}' is not valid type - {quote_level_list}"
+        logging.error(error)
+        raise ValueError(error)
+
+    elif quote_level.lower() in quote_level_list:
+
+        if quote_level.lower() == "none":
+            quoting = csv.QUOTE_NONE
+
+        # elif quote_level.lower() == "non-numeric":
+        #     quoting = csv.QUOTE_NONNUMERIC
+
+        elif quote_level.lower() == "minimal":
+            quoting = csv.QUOTE_MINIMAL
+
+        elif quote_level.lower() == "all":
+            quoting = csv.QUOTE_ALL
+
+        else:  # pragma: no cover
+            error = f"quote_level '{quote_level}' has caused an unhandled, undefined, or unknown error"  # pragma: no cover
+            logging.error(error)  # pragma: no cover
+            raise ValueError(error)  # pragma: no cover
 
     # set delimiter if none
     if delimit is None:
         delimit = ","
 
     # check if file name is a string
     if isinstance(file_name, str) is False:
@@ -205,16 +240,16 @@
     # open file
     data = []
     with open(file_save) as read_file:
         # load file into data variable
         csv_data = csv.DictReader(
             read_file,
             delimiter=delimit,
-            quoting=csv.QUOTE_MINIMAL,
-            skipinitialspace=True,
+            quoting=quoting,
+            skipinitialspace=skip_initial_space,
         )
 
         # convert list to JSON object
         title = csv_data.fieldnames
         # iterate through each row to create dictionary/json object
         for row in csv_data:
             data.extend([{title[i]: row[title[i]] for i in range(len(title))}])
@@ -226,15 +261,15 @@
 # create sample csv file
 def create_sample_files(file_name: str, sample_size: int):
 
     first_name: list = [
         "Daniel",
         "Catherine",
         "Valerie",
-        "Mike",
+        "Michael",
         "Kristina",
         "Linda",
         "Olive",
         "Mollie",
         "Nadia",
         "Elisha",
         "Lorraine",
@@ -247,24 +282,27 @@
     ]
 
     csv_data = []
     count = 0
     for _ in range(sample_size):
         r_int: int = random.randint(0, len(first_name) - 1)
         if count == 0:
-            sample_list: List[str] = ["name", "birth_date"]
+            sample_list: List[str] = ["name", "birth_date", "number"]
         else:
             sample_list: List[str] = [
                 first_name[r_int],
                 str(__gen_datetime()),
+                count,
             ]  # type: ignore
 
         count += 1
         csv_data.append(sample_list)
+        logging.info(sample_list)
 
+    print(csv_data)
     csv_file = f"{file_name}.csv"
     save_csv(csv_file, csv_data)
 
     json_data = []
     for _ in range(sample_size):
         r_int = random.randint(0, len(first_name) - 1)
         sample_dict: dict = {
@@ -274,15 +312,15 @@
         json_data.append(sample_dict)
     json_file = f"{file_name}.json"
     save_json(json_file, json_data)
 
 
 def __gen_datetime(min_year: int = None, max_year: int = None):
     if min_year is None:
-        min_year = 1900
+        min_year = 1905
     if max_year is None:
         max_year = datetime.now().year
     # generate a datetime in format yyyy-mm-dd hh:mm:ss.000000
     year: int = random.randint(min_year, max_year)
     month: int = random.randint(1, 12)
     day: int = random.randint(1, 28)
     hour: int = random.randint(0, 12)
```

### Comparing `devsetgo_lib-0.8.0/dsg_lib/folder_functions.py` & `devsetgo_lib-0.9.0/dsg_lib/folder_functions.py`

 * *Files identical despite different names*

### Comparing `devsetgo_lib-0.8.0/dsg_lib/logging_config.py` & `devsetgo_lib-0.9.0/dsg_lib/logging_config.py`

 * *Files identical despite different names*

### Comparing `devsetgo_lib-0.8.0/dsg_lib/patterns.py` & `devsetgo_lib-0.9.0/dsg_lib/patterns.py`

 * *Files identical despite different names*

### Comparing `devsetgo_lib-0.8.0/setup.cfg` & `devsetgo_lib-0.9.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [bumpversion]
-current_version = 0.8.0
+current_version = 0.9.0
 commit = True
-tag = False
+tag = True
 
 [bumpversion:file:setup.py]
 
 [metadata]
 description-file = README.md
 
 [flake8]
@@ -18,19 +18,20 @@
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 line_length = 88
 
 [coverage:run]
-source = app/*
+source = /
 omit = setup.py, _venv/*,tests/*,examples/*,
 
 [coverage:report]
 exclude_lines = 
+	pragma: no cover
 	if __name__
 	def main
 	pragma: no cover
 
 [tool:pytest]
 norecursedirs = /tests
 testpaths = tests
```

### Comparing `devsetgo_lib-0.8.0/setup.py` & `devsetgo_lib-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="devsetgo_lib",
-    version="0.8.0",
+    version="0.9.0",
     description="Common functions for applications",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/devsetgo/dev_com_lib",
     project_urls={
         "Documentation": "https://devsetgo.github.io/devsetgo_lib/",
         "Source": "https://github.com/devsetgo/devsetgo_lib",
```

