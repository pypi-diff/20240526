# Comparing `tmp/bxa-4.1.2.tar.gz` & `tmp/bxa-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bxa-4.1.2.tar", last modified: Mon Mar  4 20:40:08 2024, max compression
+gzip compressed data, was "bxa-4.1.3.tar", last modified: Sun May 26 18:26:15 2024, max compression
```

## Comparing `bxa-4.1.2.tar` & `bxa-4.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-04 20:40:08.934889 bxa-4.1.2/
--rw-r--r--   0 user      (1000) user      (1000)    35149 2021-05-10 10:26:12.000000 bxa-4.1.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)       72 2021-05-10 10:26:12.000000 bxa-4.1.2/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     7883 2024-03-04 20:40:08.934889 bxa-4.1.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     6892 2021-05-10 10:26:12.000000 bxa-4.1.2/README.rst
--rw-r--r--   0 user      (1000) user      (1000)     5426 2021-05-10 10:26:46.000000 bxa-4.1.2/addspec.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-04 20:40:08.902889 bxa-4.1.2/bxa/
--rw-r--r--   0 user      (1000) user      (1000)      269 2024-03-04 20:40:03.000000 bxa-4.1.2/bxa/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-04 20:40:08.906889 bxa-4.1.2/bxa/sherpa/
--rw-r--r--   0 user      (1000) user      (1000)      921 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-04 20:40:08.934889 bxa-4.1.2/bxa/sherpa/background/
--rw-r--r--   0 user      (1000) user      (1000)        0 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)   431614 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/chandra_1024.json
--rw-r--r--   0 user      (1000) user      (1000)   267761 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/erosita_1024.json
--rw-r--r--   0 user      (1000) user      (1000)    16677 2021-08-31 11:06:48.000000 bxa-4.1.2/bxa/sherpa/background/fitters.py
--rw-r--r--   0 user      (1000) user      (1000)     1788 2021-08-31 11:22:07.000000 bxa-4.1.2/bxa/sherpa/background/kde.py
--rw-r--r--   0 user      (1000) user      (1000)    16911 2021-08-31 11:06:48.000000 bxa-4.1.2/bxa/sherpa/background/models.py
--rw-r--r--   0 user      (1000) user      (1000)  1253996 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/nustar_4096.json
--rw-r--r--   0 user      (1000) user      (1000)    13251 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/pca.py
--rw-r--r--   0 user      (1000) user      (1000)  1161850 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/suzaku_4096.json
--rw-r--r--   0 user      (1000) user      (1000)   318648 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/swift_xrt_1024.json
--rw-r--r--   0 user      (1000) user      (1000)    20063 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/xmm.py
--rw-r--r--   0 user      (1000) user      (1000)  2882995 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/xmm_2400.json
--rw-r--r--   0 user      (1000) user      (1000)  3558683 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/xmm_4096.json
--rw-r--r--   0 user      (1000) user      (1000)   927873 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/xmm_epn_1024.json
--rw-r--r--   0 user      (1000) user      (1000)  1658222 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/xmm_epn_4096.json
--rw-r--r--   0 user      (1000) user      (1000)    78814 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/xrte_hexa_256.json
--rw-r--r--   0 user      (1000) user      (1000)    78972 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/xrte_hexb_256.json
--rw-r--r--   0 user      (1000) user      (1000)    62879 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/background/xrte_pca_128.json
--rw-r--r--   0 user      (1000) user      (1000)     2202 2021-08-31 11:06:48.000000 bxa-4.1.2/bxa/sherpa/cachedmodel.py
--rw-r--r--   0 user      (1000) user      (1000)      944 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/galabs.py
--rw-r--r--   0 user      (1000) user      (1000)    19866 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/invgauss.py
--rw-r--r--   0 user      (1000) user      (1000)     4086 2021-09-15 15:07:36.000000 bxa-4.1.2/bxa/sherpa/priors.py
--rw-r--r--   0 user      (1000) user      (1000)     2820 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/qq.py
--rw-r--r--   0 user      (1000) user      (1000)     5416 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/sherpa/rebinnedmodel.py
--rw-r--r--   0 user      (1000) user      (1000)     7586 2022-11-09 21:53:07.000000 bxa-4.1.2/bxa/sherpa/solver.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-04 20:40:08.934889 bxa-4.1.2/bxa/xspec/
--rw-r--r--   0 user      (1000) user      (1000)      802 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/xspec/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     7854 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/xspec/gof.py
--rw-r--r--   0 user      (1000) user      (1000)     3141 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/xspec/priors.py
--rw-r--r--   0 user      (1000) user      (1000)     4993 2021-05-10 10:26:12.000000 bxa-4.1.2/bxa/xspec/qq.py
--rw-r--r--   0 user      (1000) user      (1000)     4444 2023-10-21 13:54:45.000000 bxa-4.1.2/bxa/xspec/sinning.py
--rw-r--r--   0 user      (1000) user      (1000)    17839 2023-04-20 12:09:47.000000 bxa-4.1.2/bxa/xspec/solver.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-03-04 20:40:08.902889 bxa-4.1.2/bxa.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     7883 2024-03-04 20:40:08.000000 bxa-4.1.2/bxa.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1178 2024-03-04 20:40:08.000000 bxa-4.1.2/bxa.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-03-04 20:40:08.000000 bxa-4.1.2/bxa.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       52 2024-03-04 20:40:08.000000 bxa-4.1.2/bxa.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-03-04 20:40:08.000000 bxa-4.1.2/bxa.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)     2632 2021-05-10 10:26:12.000000 bxa-4.1.2/fixkeywords.py
--rw-r--r--   0 user      (1000) user      (1000)     1808 2021-05-10 10:26:12.000000 bxa-4.1.2/gal.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-03-04 20:40:08.934889 bxa-4.1.2/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1893 2024-03-04 20:40:03.000000 bxa-4.1.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-26 18:26:15.235810 bxa-4.1.3/
+-rw-r--r--   0 user      (1000) user      (1000)    35149 2021-05-10 10:26:12.000000 bxa-4.1.3/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)       72 2021-05-10 10:26:12.000000 bxa-4.1.3/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     7726 2024-05-26 18:26:15.235810 bxa-4.1.3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     6892 2021-05-10 10:26:12.000000 bxa-4.1.3/README.rst
+-rw-r--r--   0 user      (1000) user      (1000)     5426 2021-05-10 10:26:46.000000 bxa-4.1.3/addspec.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-26 18:26:15.230810 bxa-4.1.3/bxa/
+-rw-rw-r--   0 user      (1000) user      (1000)      269 2024-05-26 18:25:14.000000 bxa-4.1.3/bxa/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-26 18:26:15.230810 bxa-4.1.3/bxa/sherpa/
+-rw-r--r--   0 user      (1000) user      (1000)      921 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-26 18:26:15.234810 bxa-4.1.3/bxa/sherpa/background/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)   431614 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/chandra_1024.json
+-rw-r--r--   0 user      (1000) user      (1000)   267761 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/erosita_1024.json
+-rw-r--r--   0 user      (1000) user      (1000)    16677 2021-08-31 11:06:48.000000 bxa-4.1.3/bxa/sherpa/background/fitters.py
+-rw-r--r--   0 user      (1000) user      (1000)     1788 2021-08-31 11:22:07.000000 bxa-4.1.3/bxa/sherpa/background/kde.py
+-rw-r--r--   0 user      (1000) user      (1000)    16911 2021-08-31 11:06:48.000000 bxa-4.1.3/bxa/sherpa/background/models.py
+-rw-r--r--   0 user      (1000) user      (1000)  1253996 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/nustar_4096.json
+-rw-rw-r--   0 user      (1000) user      (1000)    13447 2024-05-26 16:28:54.000000 bxa-4.1.3/bxa/sherpa/background/pca.py
+-rw-r--r--   0 user      (1000) user      (1000)  1161850 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/suzaku_4096.json
+-rw-r--r--   0 user      (1000) user      (1000)   318648 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/swift_xrt_1024.json
+-rw-r--r--   0 user      (1000) user      (1000)    20063 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/xmm.py
+-rw-r--r--   0 user      (1000) user      (1000)  2882995 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/xmm_2400.json
+-rw-r--r--   0 user      (1000) user      (1000)  3558683 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/xmm_4096.json
+-rw-r--r--   0 user      (1000) user      (1000)   927873 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/xmm_epn_1024.json
+-rw-r--r--   0 user      (1000) user      (1000)  1658222 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/xmm_epn_4096.json
+-rw-r--r--   0 user      (1000) user      (1000)    78814 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/xrte_hexa_256.json
+-rw-r--r--   0 user      (1000) user      (1000)    78972 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/xrte_hexb_256.json
+-rw-r--r--   0 user      (1000) user      (1000)    62879 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/background/xrte_pca_128.json
+-rw-r--r--   0 user      (1000) user      (1000)     2202 2021-08-31 11:06:48.000000 bxa-4.1.3/bxa/sherpa/cachedmodel.py
+-rw-r--r--   0 user      (1000) user      (1000)      944 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/galabs.py
+-rw-r--r--   0 user      (1000) user      (1000)    19866 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/invgauss.py
+-rw-r--r--   0 user      (1000) user      (1000)     4086 2021-09-15 15:07:36.000000 bxa-4.1.3/bxa/sherpa/priors.py
+-rw-r--r--   0 user      (1000) user      (1000)     2820 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/qq.py
+-rw-r--r--   0 user      (1000) user      (1000)     5416 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/sherpa/rebinnedmodel.py
+-rw-r--r--   0 user      (1000) user      (1000)     7586 2022-11-09 21:53:07.000000 bxa-4.1.3/bxa/sherpa/solver.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-26 18:26:15.235810 bxa-4.1.3/bxa/xspec/
+-rw-r--r--   0 user      (1000) user      (1000)      802 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/xspec/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     7854 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/xspec/gof.py
+-rw-r--r--   0 user      (1000) user      (1000)     3141 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/xspec/priors.py
+-rw-r--r--   0 user      (1000) user      (1000)     4993 2021-05-10 10:26:12.000000 bxa-4.1.3/bxa/xspec/qq.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4457 2024-05-26 17:42:02.000000 bxa-4.1.3/bxa/xspec/sinning.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17839 2024-04-25 19:32:15.000000 bxa-4.1.3/bxa/xspec/solver.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-26 18:26:15.230810 bxa-4.1.3/bxa.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     7726 2024-05-26 18:26:15.000000 bxa-4.1.3/bxa.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1178 2024-05-26 18:26:15.000000 bxa-4.1.3/bxa.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-26 18:26:15.000000 bxa-4.1.3/bxa.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       52 2024-05-26 18:26:15.000000 bxa-4.1.3/bxa.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2024-05-26 18:26:15.000000 bxa-4.1.3/bxa.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)     2632 2021-05-10 10:26:12.000000 bxa-4.1.3/fixkeywords.py
+-rw-r--r--   0 user      (1000) user      (1000)     1808 2021-05-10 10:26:12.000000 bxa-4.1.3/gal.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-26 18:26:15.235810 bxa-4.1.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1893 2024-05-26 18:25:14.000000 bxa-4.1.3/setup.py
```

### Comparing `bxa-4.1.2/LICENSE` & `bxa-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/PKG-INFO` & `bxa-4.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxa
-Version: 4.1.2
+Version: 4.1.3
 Summary: Bayesian X-ray spectral analysis
 Home-page: https://github.com/JohannesBuchner/BXA/
 Author: Johannes Buchner
 Author-email: johannes.buchner.acad@gmx.com
 License: GNU General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -14,21 +14,14 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
-Requires-Dist: ultranest
-Requires-Dist: numpy
-Requires-Dist: tqdm
-Requires-Dist: corner
-Requires-Dist: h5py
-Requires-Dist: matplotlib
-Requires-Dist: astropy
 
 About Bayesian X-ray Analysis (BXA)
 ------------------------------------
 
 BXA connects the X-ray spectral analysis environments Xspec/Sherpa
 to the nested sampling algorithm UltraNest 
 for **Bayesian Parameter Estimation** and **Model comparison**.
```

### Comparing `bxa-4.1.2/README.rst` & `bxa-4.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/addspec.py` & `bxa-4.1.3/addspec.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/__init__.py` & `bxa-4.1.3/bxa/sherpa/__init__.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/chandra_1024.json` & `bxa-4.1.3/bxa/sherpa/background/chandra_1024.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/erosita_1024.json` & `bxa-4.1.3/bxa/sherpa/background/erosita_1024.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/fitters.py` & `bxa-4.1.3/bxa/sherpa/background/fitters.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/kde.py` & `bxa-4.1.3/bxa/sherpa/background/kde.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/models.py` & `bxa-4.1.3/bxa/sherpa/background/models.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/nustar_4096.json` & `bxa-4.1.3/bxa/sherpa/background/nustar_4096.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/pca.py` & `bxa-4.1.3/bxa/sherpa/background/pca.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 if 'MAKESPHINXDOC' not in os.environ:
 	import sherpa.astro.ui as ui
 	from sherpa.stats import Cash, CStat
 	from sherpa.models.parameter import Parameter
 	from sherpa.models import ArithmeticModel, CompositeModel
 	from sherpa.astro.ui import *
-	from sherpa.astro.instrument import RSPModelNoPHA, RMFModelNoPHA
+	from sherpa.astro.instrument import RSPModelNoPHA, RMFModelNoPHA, create_delta_rmf, create_arf
 else:
 	# mock objects when sherpa doc is built
 	ArithmeticModel = object
 	class CompositeModel(object):
 		pass
 	RSPModelNoPHA, RMFModelNoPHA = object, object
 
@@ -99,21 +99,19 @@
 	def calc(self, p, x, xhi=None, *args, **kwargs):
 		src = self.model.calc(p, self.xlo, self.xhi)
 		assert numpy.isfinite(src).all(), src
 		return src
 
 
 def get_identity_response(i):
-	n = get_bkg(i).counts.size
 	rmf = get_rmf(i)
-	try:
-		arf = get_arf(i)
-		return lambda model: IdentityResponse(n, model, arf=arf, rmf=rmf)
-	except:
-		return lambda model: IdentityRMF(n, model, rmf=rmf)
+	delta_rmf = create_delta_rmf(rmf.e_min, rmf.e_max, offset=1, e_min=rmf.e_min, e_max=rmf.e_max, ethresh=rmf.ethresh)
+	flat_arf = create_arf(rmf.e_min, rmf.e_max, ethresh=rmf.ethresh)
+
+	return lambda model: RSPModelNoPHA(flat_arf, delta_rmf, model)
 
 
 
 logf = logging.getLogger('bxa.Fitter')
 logf.setLevel(logging.INFO)
 
 # Model
@@ -246,15 +244,15 @@
 			for s in get_stat_info():
 				if self.id in s.ids and len(s.bkg_ids) > 0:
 					print('get_stat_info returned: ids=%s bkg_ids=%s' % (s.ids, s.bkg_ids))
 
 		assert len(ss) == 1
 		return ss[0].statval
 
-	def fit(self):
+	def fit(self, max_lines=10):
 		# try a PCA decomposition of this spectrum
 		logf.info('fitting background of ID=%s using PCA method' % (self.id))
 		initial = self.decompose()
 		logf.info('fit: initial PCA decomposition: %s' % (initial))
 		id = self.id
 		set_method('neldermead')
 		bkgmodel = PCAModel('pca%s' % id, data=self.pca)
@@ -343,49 +341,49 @@
 
 		print('Final choice: %d parameters, aic=%.2f' % (last_nparams, last_aic))
 		# reset to the last good solution
 		for p, v in zip(bkgmodel.pars, last_final):
 			p.val = v
 
 		last_model = convbkgmodel
-		for i in range(10):
+		for i in range(1, max_lines + 1):
 			print()
-			print('Adding Gaussian#%d' % (i+1))
+			print('Adding Gaussian#%d' % (i))
 			# find largest discrepancy
 			set_analysis(id, "ener", "rate")
 			m = get_bkg_fit_plot(id)
 			y = m.dataplot.y.cumsum()
 			z = m.modelplot.y.cumsum()
 			diff_rate = numpy.abs(y - z)
 			set_analysis(id, "ener", "counts")
 			m = get_bkg_fit_plot(id)
 			x = m.dataplot.x
 			y = m.dataplot.y.cumsum()
 			z = m.modelplot.y.cumsum()
 			diff = numpy.abs(y - z)
-			i = numpy.argmax(diff)
+			imax = numpy.argmax(diff)
 			energies = x
-			e = x[i]
-			print('largest remaining discrepancy at %.3fkeV[%d], need %d counts' % (x[i], i, diff[i]))
-			#e = x[i]
-			power = diff_rate[i]
+			e = x[imax]
+			print('largest remaining discrepancy at %.3fkeV[%d], need %d counts' % (x[imax], imax, diff[imax]))
+			power = diff_rate[imax]
+			# power = diff[imax]
 			# lets try to inject a gaussian there
 
 			g = xsgaussian('g_%d_%d' % (id, i))
 			print('placing gaussian at %.2fkeV, with power %s' % (e, power))
 			# we work in energy bins, not energy
 			g.LineE.min = energies[0]
 			g.LineE.max = energies[-1]
 			g.LineE.val = e
-			if i > len(diff) - 2:
-				i = len(diff) - 2
-			if i < 2:
-				i = 2
-			g.Sigma = (x[i + 1] - x[i - 1])
-			g.Sigma.min = (x[i + 1] - x[i - 1])/3
+			if imax > len(diff) - 2:
+				imax = len(diff) - 2
+			if imax < 2:
+				imax = 2
+			g.Sigma = (x[imax + 1] - x[imax - 1])
+			g.Sigma.min = (x[imax + 1] - x[imax - 1])/3
 			g.Sigma.max = x[-1] - x[0]
 			g.norm.min = power * 1e-6
 			g.norm.val = power
 			convbkgmodel2 = response(g)
 			next_model = last_model + convbkgmodel2
 			set_bkg_full_model(self.id, next_model)
 			fit_bkg(id=self.id)
@@ -401,23 +399,23 @@
 			else:
 				print('not significant, rejecting')
 				set_bkg_full_model(self.id, last_model)
 				for p, v in zip(last_model.pars, last_final):
 					p.val = v
 				break
 
-def auto_background(id):
+def auto_background(id, max_lines=10):
 	"""Automatically fits background *id* based on PCA-based templates,
 	and additional gaussian lines as needed by AIC."""
 	bkgmodel = PCAFitter(id)
 	log_sherpa = logging.getLogger('sherpa.astro.ui.utils')
 	prev_level = log_sherpa.level
 	try:
 		log_sherpa.setLevel(logging.WARN)
-		bkgmodel.fit()
+		bkgmodel.fit(max_lines)
 	finally:
 		log_sherpa.setLevel(prev_level)
 	m = get_bkg_fit_plot(id)
 	numpy.savetxt('test_bkg.txt', numpy.transpose([m.dataplot.x, m.dataplot.y, m.modelplot.x, m.modelplot.y]))
 	return get_bkg_model(id)
```

### Comparing `bxa-4.1.2/bxa/sherpa/background/suzaku_4096.json` & `bxa-4.1.3/bxa/sherpa/background/suzaku_4096.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/swift_xrt_1024.json` & `bxa-4.1.3/bxa/sherpa/background/swift_xrt_1024.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/xmm.py` & `bxa-4.1.3/bxa/sherpa/background/xmm.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/xmm_2400.json` & `bxa-4.1.3/bxa/sherpa/background/xmm_2400.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/xmm_4096.json` & `bxa-4.1.3/bxa/sherpa/background/xmm_4096.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/xmm_epn_1024.json` & `bxa-4.1.3/bxa/sherpa/background/xmm_epn_1024.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/xmm_epn_4096.json` & `bxa-4.1.3/bxa/sherpa/background/xmm_epn_4096.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/xrte_hexa_256.json` & `bxa-4.1.3/bxa/sherpa/background/xrte_hexa_256.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/xrte_hexb_256.json` & `bxa-4.1.3/bxa/sherpa/background/xrte_hexb_256.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/background/xrte_pca_128.json` & `bxa-4.1.3/bxa/sherpa/background/xrte_pca_128.json`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/cachedmodel.py` & `bxa-4.1.3/bxa/sherpa/cachedmodel.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/galabs.py` & `bxa-4.1.3/bxa/sherpa/galabs.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/invgauss.py` & `bxa-4.1.3/bxa/sherpa/invgauss.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/priors.py` & `bxa-4.1.3/bxa/sherpa/priors.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/qq.py` & `bxa-4.1.3/bxa/sherpa/qq.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/rebinnedmodel.py` & `bxa-4.1.3/bxa/sherpa/rebinnedmodel.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/sherpa/solver.py` & `bxa-4.1.3/bxa/sherpa/solver.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/xspec/__init__.py` & `bxa-4.1.3/bxa/xspec/__init__.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/xspec/gof.py` & `bxa-4.1.3/bxa/xspec/gof.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/xspec/priors.py` & `bxa-4.1.3/bxa/xspec/priors.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/xspec/qq.py` & `bxa-4.1.3/bxa/xspec/qq.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa/xspec/sinning.py` & `bxa-4.1.3/bxa/xspec/sinning.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,22 +123,22 @@
 	# plot data
 	ymin = 1e300
 	ymax = 0
 	for (xloi, xhii, ydatai), gofpi in zip(grouped_data, data_gofp):
 		best_gof = -numpy.log10(gofpi + 1e-300)
 		# 1e3 and 1e6 correspond roughly to 3 sigma and 5 sigma
 		c = 'green' if best_gof < 2 else 'orange' if best_gof < 6. else 'red'
-		f = 1. / (xhii-xloi) #* deltax
+		f = 1. / (xhii - xloi)
 		y = ydatai * f
 		modelrange_low  = scipy.special.gammaincinv(ydatai + 1, 0.1) * f
 		modelrange_high = scipy.special.gammaincinv(ydatai + 1, 0.9) * f
-		marked_binned.append(
-			dict(x=(xloi+xhii)/2., xerr=(-xloi+xhii)/2.,
+		marked_binned.append(dict(
+			x=(xloi + xhii)/2., xerr=(xhii - xloi) / 2.,
 			y = y,
-			yerr = [[modelrange_high - y], [y - modelrange_low]],
+			yerr = [[max(0, modelrange_high - y)], [max(0, y - modelrange_low)]],
 			color=c)
 		)
 		ymin = min(ymin, modelrange_low)
 		ymax = max(ymax, modelrange_high)
 	
 	return dict(marked_binned = marked_binned, 
 		gof_avg=gof_avg, gof_total=gof_total, stats=stats,
```

### Comparing `bxa-4.1.2/bxa/xspec/solver.py` & `bxa-4.1.3/bxa/xspec/solver.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/bxa.egg-info/PKG-INFO` & `bxa-4.1.3/bxa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bxa
-Version: 4.1.2
+Version: 4.1.3
 Summary: Bayesian X-ray spectral analysis
 Home-page: https://github.com/JohannesBuchner/BXA/
 Author: Johannes Buchner
 Author-email: johannes.buchner.acad@gmx.com
 License: GNU General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -14,21 +14,14 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
-Requires-Dist: ultranest
-Requires-Dist: numpy
-Requires-Dist: tqdm
-Requires-Dist: corner
-Requires-Dist: h5py
-Requires-Dist: matplotlib
-Requires-Dist: astropy
 
 About Bayesian X-ray Analysis (BXA)
 ------------------------------------
 
 BXA connects the X-ray spectral analysis environments Xspec/Sherpa
 to the nested sampling algorithm UltraNest 
 for **Bayesian Parameter Estimation** and **Model comparison**.
```

### Comparing `bxa-4.1.2/bxa.egg-info/SOURCES.txt` & `bxa-4.1.3/bxa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/fixkeywords.py` & `bxa-4.1.3/fixkeywords.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/gal.py` & `bxa-4.1.3/gal.py`

 * *Files identical despite different names*

### Comparing `bxa-4.1.2/setup.py` & `bxa-4.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 except ImportError:
     sherpa_available = False
 
 if not sherpa_available and not xspec_available:
     warnings.warn("BXA is a plugin for xspec/sherpa, but neither xspec nor sherpa are installed in the current environment!")
 
 setup(name='bxa',
-    version='4.1.2',
+    version='4.1.3',
     author='Johannes Buchner',
     url='https://github.com/JohannesBuchner/BXA/',
     author_email='johannes.buchner.acad@gmx.com',
     description='Bayesian X-ray spectral analysis',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
```

