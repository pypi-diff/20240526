# Comparing `tmp/scatcluster-0.0.59.tar.gz` & `tmp/scatcluster-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.59.tar", last modified: Sun May 26 07:16:07 2024, max compression
+gzip compressed data, was "scatcluster-0.0.6.tar", last modified: Sun Apr 28 16:13:51 2024, max compression
```

## Comparing `scatcluster-0.0.59.tar` & `scatcluster-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:16:07.176192 scatcluster-0.0.59/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-26 07:16:01.000000 scatcluster-0.0.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 07:16:01.000000 scatcluster-0.0.59/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 07:16:07.176192 scatcluster-0.0.59/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:16:07.172192 scatcluster-0.0.59/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:16:07.172192 scatcluster-0.0.59/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:16:07.172192 scatcluster-0.0.59/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16558 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    20212 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-26 07:16:01.000000 scatcluster-0.0.59/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:16:07.172192 scatcluster-0.0.59/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 07:16:07.000000 scatcluster-0.0.59/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-26 07:16:07.000000 scatcluster-0.0.59/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:16:07.000000 scatcluster-0.0.59/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-26 07:16:07.000000 scatcluster-0.0.59/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 07:16:07.000000 scatcluster-0.0.59/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:16:07.176192 scatcluster-0.0.59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-26 07:16:01.000000 scatcluster-0.0.59/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:13:51.415429 scatcluster-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-28 16:13:49.000000 scatcluster-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 16:13:49.000000 scatcluster-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 16:13:51.415429 scatcluster-0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:13:51.415429 scatcluster-0.0.6/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:13:51.415429 scatcluster-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-28 16:13:50.000000 scatcluster-0.0.6/setup.py
```

### Comparing `scatcluster-0.0.59/LICENSE` & `scatcluster-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.59/setup.py` & `scatcluster-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-"""
-Setup script for ScatCluster
-"""
 from setuptools import find_packages, setup
 
 NAME = 'scatcluster'
 DESCRIPTION = 'A workflow for clustering continuous time series with a deep scattering network.'
 URL = 'https://github.com/INGV/ScatCluster'
 AUTHOR = 'christopher.zerafa@ingv.it'
 REQUIRES_PYTHON = '>=3.8.0'
@@ -18,32 +15,32 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.59',
+    version='0.0.6',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages(where='.'),
-    package_data={NAME: ['scatcluster/*.py']},
+    packages=find_packages('.'),
+    package_data={NAME: ['py.typed']},
     include_package_data=True,
     install_requires=REQUIRED,
     extras_require={'gpu': [*REQUIRED, *REQUIRED_GPU]},
-    license='MIT',
+    license='Apache',
     classifiers=[
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Natural Language :: English',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
```

