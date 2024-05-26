# Comparing `tmp/genairr-0.1.2.tar.gz` & `tmp/genairr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genairr-0.1.2.tar", last modified: Sat May 25 10:11:00 2024, max compression
+gzip compressed data, was "genairr-0.1.3.tar", last modified: Sun May 26 12:10:02 2024, max compression
```

## Comparing `genairr-0.1.2.tar` & `genairr-0.1.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.591303 genairr-0.1.2/
--rw-rw-rw-   0        0        0       45 2024-05-25 10:08:45.000000 genairr-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0    24500 2024-05-25 10:11:00.590286 genairr-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    23320 2024-03-10 10:42:31.000000 genairr-0.1.2/README.md
--rw-rw-rw-   0        0        0       63 2024-03-11 07:57:09.000000 genairr-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 10:11:00.592286 genairr-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1688 2024-05-25 10:10:56.000000 genairr-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.457997 genairr-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.468536 genairr-0.1.2/src/GenAIRR/
--rw-rw-rw-   0        0        0      156 2024-03-07 11:37:33.000000 genairr-0.1.2/src/GenAIRR/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.478623 genairr-0.1.2/src/GenAIRR/alleles/
--rw-rw-rw-   0        0        0      120 2024-02-14 14:01:48.000000 genairr-0.1.2/src/GenAIRR/alleles/__init__.py
--rw-rw-rw-   0        0        0    12344 2024-03-31 06:06:28.000000 genairr-0.1.2/src/GenAIRR/alleles/allele.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.545319 genairr-0.1.2/src/GenAIRR/data/
--rw-rw-rw-   0        0        0   366369 2024-02-14 13:58:48.000000 genairr-0.1.2/src/GenAIRR/data/HH_S5F_60_META.pkl
--rw-rw-rw-   0        0        0   366378 2024-02-14 13:58:48.000000 genairr-0.1.2/src/GenAIRR/data/HH_S5F_META.pkl
--rw-rw-rw-   0        0        0   366369 2024-02-14 13:58:48.000000 genairr-0.1.2/src/GenAIRR/data/HH_S5F_Opposite_META.pkl
--rw-rw-rw-   0        0        0   366378 2024-02-14 13:58:48.000000 genairr-0.1.2/src/GenAIRR/data/HKL_S5F_META.pkl
--rw-rw-rw-   0        0        0  6375188 2024-02-29 08:18:48.000000 genairr-0.1.2/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V2.pkl
--rw-rw-rw-   0        0        0  6375243 2024-03-31 06:09:57.000000 genairr-0.1.2/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V3.pkl
--rw-rw-rw-   0        0        0   897136 2024-02-29 08:29:35.000000 genairr-0.1.2/src/GenAIRR/data/LightChain_KAPPA_DataConfigV2.pkl
--rw-rw-rw-   0        0        0   897188 2024-04-04 07:14:45.000000 genairr-0.1.2/src/GenAIRR/data/LightChain_KAPPA_DataConfigV3.pkl
--rw-rw-rw-   0        0        0  1258135 2024-02-29 08:24:14.000000 genairr-0.1.2/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV2.pkl
--rw-rw-rw-   0        0        0  1258187 2024-04-04 07:14:45.000000 genairr-0.1.2/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV3.pkl
--rw-rw-rw-   0        0        0      639 2024-05-22 15:26:12.000000 genairr-0.1.2/src/GenAIRR/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.548543 genairr-0.1.2/src/GenAIRR/generateDataConfig/
--rw-rw-rw-   0        0        0       82 2024-03-07 11:28:19.000000 genairr-0.1.2/src/GenAIRR/generateDataConfig/__init__.py
--rw-rw-rw-   0        0        0    42684 2024-03-24 09:12:04.000000 genairr-0.1.2/src/GenAIRR/generateDataConfig/make_dataconfig.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.556025 genairr-0.1.2/src/GenAIRR/mutation/
--rw-rw-rw-   0        0        0       95 2024-02-14 14:01:48.000000 genairr-0.1.2/src/GenAIRR/mutation/__init__.py
--rw-rw-rw-   0        0        0     1514 2024-02-29 15:28:44.000000 genairr-0.1.2/src/GenAIRR/mutation/config.py
--rw-rw-rw-   0        0        0     1081 2024-02-29 15:31:36.000000 genairr-0.1.2/src/GenAIRR/mutation/mutation_model.py
--rw-rw-rw-   0        0        0    18179 2024-03-31 06:06:28.000000 genairr-0.1.2/src/GenAIRR/mutation/s5f.py
--rw-rw-rw-   0        0        0     6789 2024-03-31 06:06:28.000000 genairr-0.1.2/src/GenAIRR/mutation/uniform.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.564286 genairr-0.1.2/src/GenAIRR/sequence/
--rw-rw-rw-   0        0        0      165 2024-03-06 08:37:25.000000 genairr-0.1.2/src/GenAIRR/sequence/__init__.py
--rw-rw-rw-   0        0        0     9859 2024-04-07 10:57:21.000000 genairr-0.1.2/src/GenAIRR/sequence/heavy_chain.py
--rw-rw-rw-   0        0        0     8878 2024-04-07 10:49:51.000000 genairr-0.1.2/src/GenAIRR/sequence/light_chain.py
--rw-rw-rw-   0        0        0     4948 2024-02-29 15:57:46.000000 genairr-0.1.2/src/GenAIRR/sequence/np_region.py
--rw-rw-rw-   0        0        0     4369 2024-03-06 08:37:25.000000 genairr-0.1.2/src/GenAIRR/sequence/sequence.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.571285 genairr-0.1.2/src/GenAIRR/simulation/
--rw-rw-rw-   0        0        0      339 2024-02-14 14:01:48.000000 genairr-0.1.2/src/GenAIRR/simulation/__init__.py
--rw-rw-rw-   0        0        0    21613 2024-05-22 15:09:43.000000 genairr-0.1.2/src/GenAIRR/simulation/heavy_chain_sequence_augmentor.py
--rw-rw-rw-   0        0        0    30282 2024-04-30 07:21:27.000000 genairr-0.1.2/src/GenAIRR/simulation/light_chain_sequence_augmentor.py
--rw-rw-rw-   0        0        0    36881 2024-04-18 15:01:19.000000 genairr-0.1.2/src/GenAIRR/simulation/sequence_augmentor_base.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.586285 genairr-0.1.2/src/GenAIRR/utilities/
--rw-rw-rw-   0        0        0     3286 2024-03-02 09:19:19.000000 genairr-0.1.2/src/GenAIRR/utilities/AlleleNComparer.py
--rw-rw-rw-   0        0        0      236 2024-02-29 09:29:41.000000 genairr-0.1.2/src/GenAIRR/utilities/__init__.py
--rw-rw-rw-   0        0        0    15686 2024-03-31 06:06:28.000000 genairr-0.1.2/src/GenAIRR/utilities/asc_utilities.py
--rw-rw-rw-   0        0        0     2288 2024-03-02 09:37:07.000000 genairr-0.1.2/src/GenAIRR/utilities/data_config.py
--rw-rw-rw-   0        0        0     3396 2024-03-31 06:06:28.000000 genairr-0.1.2/src/GenAIRR/utilities/data_utilities.py
--rw-rw-rw-   0        0        0      846 2024-03-02 09:38:08.000000 genairr-0.1.2/src/GenAIRR/utilities/file_utilities.py
--rw-rw-rw-   0        0        0     3335 2024-03-02 09:38:47.000000 genairr-0.1.2/src/GenAIRR/utilities/misc.py
--rw-rw-rw-   0        0        0     9495 2024-04-04 07:14:45.000000 genairr-0.1.2/src/GenAIRR/utilities/report.py
-drwxrwxrwx   0        0        0        0 2024-05-25 10:11:00.588285 genairr-0.1.2/src/GenAIRR.egg-info/
--rw-rw-rw-   0        0        0    24500 2024-05-25 10:10:59.000000 genairr-0.1.2/src/GenAIRR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1711 2024-05-25 10:11:00.000000 genairr-0.1.2/src/GenAIRR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 10:10:59.000000 genairr-0.1.2/src/GenAIRR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-25 10:10:59.000000 genairr-0.1.2/src/GenAIRR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-25 10:10:59.000000 genairr-0.1.2/src/GenAIRR.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:02.044559 genairr-0.1.3/
+-rw-rw-rw-   0        0        0       45 2024-05-25 10:08:45.000000 genairr-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    24500 2024-05-26 12:10:02.042306 genairr-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    23320 2024-03-10 10:42:31.000000 genairr-0.1.3/README.md
+-rw-rw-rw-   0        0        0       63 2024-03-11 07:57:09.000000 genairr-0.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 12:10:02.044559 genairr-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1688 2024-05-26 12:00:01.000000 genairr-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:01.874207 genairr-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:01.891855 genairr-0.1.3/src/GenAIRR/
+-rw-rw-rw-   0        0        0      156 2024-03-07 11:37:33.000000 genairr-0.1.3/src/GenAIRR/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:01.907823 genairr-0.1.3/src/GenAIRR/alleles/
+-rw-rw-rw-   0        0        0      120 2024-02-14 14:01:48.000000 genairr-0.1.3/src/GenAIRR/alleles/__init__.py
+-rw-rw-rw-   0        0        0    12336 2024-05-26 11:58:40.000000 genairr-0.1.3/src/GenAIRR/alleles/allele.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:01.982754 genairr-0.1.3/src/GenAIRR/data/
+-rw-rw-rw-   0        0        0   366369 2024-02-14 13:58:48.000000 genairr-0.1.3/src/GenAIRR/data/HH_S5F_60_META.pkl
+-rw-rw-rw-   0        0        0   366378 2024-02-14 13:58:48.000000 genairr-0.1.3/src/GenAIRR/data/HH_S5F_META.pkl
+-rw-rw-rw-   0        0        0   366369 2024-02-14 13:58:48.000000 genairr-0.1.3/src/GenAIRR/data/HH_S5F_Opposite_META.pkl
+-rw-rw-rw-   0        0        0   366378 2024-02-14 13:58:48.000000 genairr-0.1.3/src/GenAIRR/data/HKL_S5F_META.pkl
+-rw-rw-rw-   0        0        0  6375188 2024-02-29 08:18:48.000000 genairr-0.1.3/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V2.pkl
+-rw-rw-rw-   0        0        0  6375243 2024-03-31 06:09:57.000000 genairr-0.1.3/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V3.pkl
+-rw-rw-rw-   0        0        0   897136 2024-02-29 08:29:35.000000 genairr-0.1.3/src/GenAIRR/data/LightChain_KAPPA_DataConfigV2.pkl
+-rw-rw-rw-   0        0        0   897188 2024-04-04 07:14:45.000000 genairr-0.1.3/src/GenAIRR/data/LightChain_KAPPA_DataConfigV3.pkl
+-rw-rw-rw-   0        0        0  1258135 2024-02-29 08:24:14.000000 genairr-0.1.3/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV2.pkl
+-rw-rw-rw-   0        0        0  1258187 2024-04-04 07:14:45.000000 genairr-0.1.3/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV3.pkl
+-rw-rw-rw-   0        0        0      639 2024-05-22 15:26:12.000000 genairr-0.1.3/src/GenAIRR/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:01.987063 genairr-0.1.3/src/GenAIRR/generateDataConfig/
+-rw-rw-rw-   0        0        0       82 2024-03-07 11:28:19.000000 genairr-0.1.3/src/GenAIRR/generateDataConfig/__init__.py
+-rw-rw-rw-   0        0        0    42684 2024-03-24 09:12:04.000000 genairr-0.1.3/src/GenAIRR/generateDataConfig/make_dataconfig.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:01.997150 genairr-0.1.3/src/GenAIRR/mutation/
+-rw-rw-rw-   0        0        0       95 2024-02-14 14:01:48.000000 genairr-0.1.3/src/GenAIRR/mutation/__init__.py
+-rw-rw-rw-   0        0        0     1514 2024-02-29 15:28:44.000000 genairr-0.1.3/src/GenAIRR/mutation/config.py
+-rw-rw-rw-   0        0        0     1081 2024-02-29 15:31:36.000000 genairr-0.1.3/src/GenAIRR/mutation/mutation_model.py
+-rw-rw-rw-   0        0        0    18179 2024-03-31 06:06:28.000000 genairr-0.1.3/src/GenAIRR/mutation/s5f.py
+-rw-rw-rw-   0        0        0     6789 2024-03-31 06:06:28.000000 genairr-0.1.3/src/GenAIRR/mutation/uniform.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:02.008417 genairr-0.1.3/src/GenAIRR/sequence/
+-rw-rw-rw-   0        0        0      165 2024-03-06 08:37:25.000000 genairr-0.1.3/src/GenAIRR/sequence/__init__.py
+-rw-rw-rw-   0        0        0     9859 2024-04-07 10:57:21.000000 genairr-0.1.3/src/GenAIRR/sequence/heavy_chain.py
+-rw-rw-rw-   0        0        0     8640 2024-05-26 11:58:40.000000 genairr-0.1.3/src/GenAIRR/sequence/light_chain.py
+-rw-rw-rw-   0        0        0     4948 2024-02-29 15:57:46.000000 genairr-0.1.3/src/GenAIRR/sequence/np_region.py
+-rw-rw-rw-   0        0        0     4369 2024-03-06 08:37:25.000000 genairr-0.1.3/src/GenAIRR/sequence/sequence.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:02.019192 genairr-0.1.3/src/GenAIRR/simulation/
+-rw-rw-rw-   0        0        0      339 2024-02-14 14:01:48.000000 genairr-0.1.3/src/GenAIRR/simulation/__init__.py
+-rw-rw-rw-   0        0        0    21613 2024-05-22 15:09:43.000000 genairr-0.1.3/src/GenAIRR/simulation/heavy_chain_sequence_augmentor.py
+-rw-rw-rw-   0        0        0    30282 2024-04-30 07:21:27.000000 genairr-0.1.3/src/GenAIRR/simulation/light_chain_sequence_augmentor.py
+-rw-rw-rw-   0        0        0    36881 2024-04-18 15:01:19.000000 genairr-0.1.3/src/GenAIRR/simulation/sequence_augmentor_base.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:02.036657 genairr-0.1.3/src/GenAIRR/utilities/
+-rw-rw-rw-   0        0        0     3286 2024-03-02 09:19:19.000000 genairr-0.1.3/src/GenAIRR/utilities/AlleleNComparer.py
+-rw-rw-rw-   0        0        0      236 2024-02-29 09:29:41.000000 genairr-0.1.3/src/GenAIRR/utilities/__init__.py
+-rw-rw-rw-   0        0        0    15686 2024-03-31 06:06:28.000000 genairr-0.1.3/src/GenAIRR/utilities/asc_utilities.py
+-rw-rw-rw-   0        0        0     2288 2024-03-02 09:37:07.000000 genairr-0.1.3/src/GenAIRR/utilities/data_config.py
+-rw-rw-rw-   0        0        0     3396 2024-03-31 06:06:28.000000 genairr-0.1.3/src/GenAIRR/utilities/data_utilities.py
+-rw-rw-rw-   0        0        0      846 2024-03-02 09:38:08.000000 genairr-0.1.3/src/GenAIRR/utilities/file_utilities.py
+-rw-rw-rw-   0        0        0     3335 2024-03-02 09:38:47.000000 genairr-0.1.3/src/GenAIRR/utilities/misc.py
+-rw-rw-rw-   0        0        0     9495 2024-04-04 07:14:45.000000 genairr-0.1.3/src/GenAIRR/utilities/report.py
+drwxrwxrwx   0        0        0        0 2024-05-26 12:10:02.040060 genairr-0.1.3/src/GenAIRR.egg-info/
+-rw-rw-rw-   0        0        0    24500 2024-05-26 12:10:01.000000 genairr-0.1.3/src/GenAIRR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1711 2024-05-26 12:10:01.000000 genairr-0.1.3/src/GenAIRR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 12:10:01.000000 genairr-0.1.3/src/GenAIRR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-26 12:10:01.000000 genairr-0.1.3/src/GenAIRR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 12:10:01.000000 genairr-0.1.3/src/GenAIRR.egg-info/top_level.txt
```

### Comparing `genairr-0.1.2/PKG-INFO` & `genairr-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: GenAIRR
-Version: 0.1.2
+Version: 0.1.3
 Summary: An advanced immunoglobulin sequence simulation suite for benchmarking alignment models and sequence analysis.
 Home-page: https://github.com/MuteJester/GenAIRR
-Download-URL: https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.2.tar.gz
+Download-URL: https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.3.tar.gz
 Author: Thomas Konstantinovsky & Ayelet Peres
 Author-email: thomaskon90@gmail.com
 Project-URL: Bug Tracker, https://github.com/MuteJester/GenAIRR/issues
 Keywords: immunogenetics,sequence simulation,bioinformatics,alignment benchmarking
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `genairr-0.1.2/README.md` & `genairr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/setup.py` & `genairr-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='GenAIRR',
-    version='0.1.2',
+    version='0.1.3',
     author='Thomas Konstantinovsky & Ayelet Peres',
     author_email='thomaskon90@gmail.com',
     description='An advanced immunoglobulin sequence simulation suite for benchmarking alignment models and sequence analysis.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/MuteJester/GenAIRR',
-    download_url='https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.2.tar.gz',
+    download_url='https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.3.tar.gz',
     project_urls={
         "Bug Tracker": "https://github.com/MuteJester/GenAIRR/issues"
     },
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     package_data={'GenAIRR': ['data/*.pkl', 'data/*.json']},  # Include any additional data files
     include_package_data=True,  # Include everything in source control
```

### Comparing `genairr-0.1.2/src/GenAIRR/alleles/allele.py` & `genairr-0.1.3/src/GenAIRR/alleles/allele.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,16 +260,16 @@
         self.anchor = None
         self.frame = None
         for frame in range(3):
             motif = re.compile('(ttt|ttc|tgg)(ggt|ggc|gga|ggg)[a-z]{3}(ggt|ggc|gga|ggg)')
             match = motif.search(self.ungapped_seq[frame:])
             if match:
                 if match.span()[0] % 3 == 0:
-                    self.anchor = match.span()[0] + frame - 1 # correct for the end of the cdr3
-                    self.frame = frame - 1 # retain the frame of the J
+                    self.anchor = match.span()[0] + frame # correct for the end of the cdr3
+                    self.frame = frame # retain the frame of the J
                     
 
     def _get_trim_length(self, trim_dicts):
         """Determines the trim lengths for the J allele's sequence based on provided trimming dictionaries.
 
         Args:
             trim_dicts (dict): A dictionary specifying trimming lengths for different allele types.
```

### Comparing `genairr-0.1.2/src/GenAIRR/data/HH_S5F_60_META.pkl` & `genairr-0.1.3/src/GenAIRR/data/HH_S5F_60_META.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/HH_S5F_META.pkl` & `genairr-0.1.3/src/GenAIRR/data/HH_S5F_META.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/HH_S5F_Opposite_META.pkl` & `genairr-0.1.3/src/GenAIRR/data/HH_S5F_Opposite_META.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/HKL_S5F_META.pkl` & `genairr-0.1.3/src/GenAIRR/data/HKL_S5F_META.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V2.pkl` & `genairr-0.1.3/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V2.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V3.pkl` & `genairr-0.1.3/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V3.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/LightChain_KAPPA_DataConfigV2.pkl` & `genairr-0.1.3/src/GenAIRR/data/LightChain_KAPPA_DataConfigV2.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/LightChain_KAPPA_DataConfigV3.pkl` & `genairr-0.1.3/src/GenAIRR/data/LightChain_KAPPA_DataConfigV3.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV2.pkl` & `genairr-0.1.3/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV2.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV3.pkl` & `genairr-0.1.3/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV3.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/data/__init__.py` & `genairr-0.1.3/src/GenAIRR/data/__init__.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/generateDataConfig/make_dataconfig.py` & `genairr-0.1.3/src/GenAIRR/generateDataConfig/make_dataconfig.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/mutation/config.py` & `genairr-0.1.3/src/GenAIRR/mutation/config.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/mutation/mutation_model.py` & `genairr-0.1.3/src/GenAIRR/mutation/mutation_model.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/mutation/s5f.py` & `genairr-0.1.3/src/GenAIRR/mutation/s5f.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/mutation/uniform.py` & `genairr-0.1.3/src/GenAIRR/mutation/uniform.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/sequence/heavy_chain.py` & `genairr-0.1.3/src/GenAIRR/sequence/heavy_chain.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/sequence/light_chain.py` & `genairr-0.1.3/src/GenAIRR/sequence/light_chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,18 +62,15 @@
         # log trims
         self.v_trim_5 = v_trim_5
         self.v_trim_3 = v_trim_3
         self.j_trim_5 = j_trim_5
         self.j_trim_3 = j_trim_3
 
         self.ungapped_seq = nuc_seq.upper()
-
         self.junction_length = self.get_junction_length()
-        self.junction_start = self.v_allele.anchor
-        self.junction_end = self.v_allele.anchor + self.junction_length
 
         self.junction = self.ungapped_seq[self.v_allele.anchor:
                                           self.v_allele.anchor + self.junction_length].upper()
 
         self.update_metadata()
         self._is_functional(self.ungapped_seq)
 
@@ -88,16 +85,14 @@
         self.j_seq_end = self.j_seq_start + self.j_allele.ungapped_len - self.j_trim_5
         self.v_germline_start = 0
         self.v_germline_end = self.v_allele.ungapped_len - self.v_trim_3
         self.j_germline_start = self.j_trim_5
         self.j_germline_end = self.j_allele.ungapped_len - self.j_trim_3
         self.junction_start = self.v_allele.anchor
         self.junction_end = self.v_allele.anchor + self.junction_length
-        self.junction = self.ungapped_seq[self.junction_start:
-                                          (self.junction_end+1)].upper()
         
     def _is_functional(self, sequence):
         """
        Evaluates whether the light chain sequence is functional based on the presence of in-frame junctions
        without stop codons and specific amino acid motifs at the junction boundaries.
 
        Args:
@@ -142,17 +137,17 @@
         """
         Calculates the length of the junction region in the light chain sequence, taking into account
         the trimmed V and J segments and the NP1 region.
 
         Returns:
             int: The total length of the junction region, including CDR3 and flanking conserved regions.
         """
-
-        junction_length = self.v_seq_end - (self.v_allele.anchor - 1) - self.v_trim_3 + self.NP1_length + \
-                          (self.j_allele.anchor + 2) - self.j_trim_5
+                                  
+        junction_length = self.v_allele.length - (self.v_allele.anchor - 1) - self.v_trim_3 + \
+            self.NP1_length  + (self.j_allele.anchor + 2) - self.j_trim_5
         return junction_length
 
     def check_stops(self, seq):
         """
         Checks the given sequence for the presence of stop codons.
 
         Args:
```

### Comparing `genairr-0.1.2/src/GenAIRR/sequence/np_region.py` & `genairr-0.1.3/src/GenAIRR/sequence/np_region.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/sequence/sequence.py` & `genairr-0.1.3/src/GenAIRR/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/simulation/heavy_chain_sequence_augmentor.py` & `genairr-0.1.3/src/GenAIRR/simulation/heavy_chain_sequence_augmentor.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/simulation/light_chain_sequence_augmentor.py` & `genairr-0.1.3/src/GenAIRR/simulation/light_chain_sequence_augmentor.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/simulation/sequence_augmentor_base.py` & `genairr-0.1.3/src/GenAIRR/simulation/sequence_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/utilities/AlleleNComparer.py` & `genairr-0.1.3/src/GenAIRR/utilities/AlleleNComparer.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/utilities/asc_utilities.py` & `genairr-0.1.3/src/GenAIRR/utilities/asc_utilities.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/utilities/data_config.py` & `genairr-0.1.3/src/GenAIRR/utilities/data_config.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/utilities/data_utilities.py` & `genairr-0.1.3/src/GenAIRR/utilities/data_utilities.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/utilities/file_utilities.py` & `genairr-0.1.3/src/GenAIRR/utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/utilities/misc.py` & `genairr-0.1.3/src/GenAIRR/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR/utilities/report.py` & `genairr-0.1.3/src/GenAIRR/utilities/report.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.2/src/GenAIRR.egg-info/PKG-INFO` & `genairr-0.1.3/src/GenAIRR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: GenAIRR
-Version: 0.1.2
+Version: 0.1.3
 Summary: An advanced immunoglobulin sequence simulation suite for benchmarking alignment models and sequence analysis.
 Home-page: https://github.com/MuteJester/GenAIRR
-Download-URL: https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.2.tar.gz
+Download-URL: https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.3.tar.gz
 Author: Thomas Konstantinovsky & Ayelet Peres
 Author-email: thomaskon90@gmail.com
 Project-URL: Bug Tracker, https://github.com/MuteJester/GenAIRR/issues
 Keywords: immunogenetics,sequence simulation,bioinformatics,alignment benchmarking
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `genairr-0.1.2/src/GenAIRR.egg-info/SOURCES.txt` & `genairr-0.1.3/src/GenAIRR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

