# Comparing `tmp/scatcluster-0.0.6.tar.gz` & `tmp/scatcluster-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.6.tar", last modified: Sun Apr 28 16:13:51 2024, max compression
+gzip compressed data, was "scatcluster-0.0.60.tar", last modified: Sun May 26 18:34:08 2024, max compression
```

## Comparing `scatcluster-0.0.6.tar` & `scatcluster-0.0.60.tar`

### file list

```diff
@@ -1,12 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:13:51.415429 scatcluster-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-28 16:13:49.000000 scatcluster-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 16:13:49.000000 scatcluster-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 16:13:51.415429 scatcluster-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:13:51.415429 scatcluster-0.0.6/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:13:51.000000 scatcluster-0.0.6/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:13:51.415429 scatcluster-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-28 16:13:50.000000 scatcluster-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:34:08.399744 scatcluster-0.0.60/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-26 18:34:05.000000 scatcluster-0.0.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 18:34:05.000000 scatcluster-0.0.60/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 18:34:08.399744 scatcluster-0.0.60/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:34:08.391744 scatcluster-0.0.60/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:34:08.395744 scatcluster-0.0.60/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21387 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:34:08.395744 scatcluster-0.0.60/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16558 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24715 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-05-26 18:34:05.000000 scatcluster-0.0.60/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 18:34:08.395744 scatcluster-0.0.60/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-26 18:34:08.000000 scatcluster-0.0.60/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-26 18:34:08.000000 scatcluster-0.0.60/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 18:34:08.000000 scatcluster-0.0.60/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-26 18:34:08.000000 scatcluster-0.0.60/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 18:34:08.000000 scatcluster-0.0.60/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 18:34:08.399744 scatcluster-0.0.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-26 18:34:05.000000 scatcluster-0.0.60/setup.py
```

### Comparing `scatcluster-0.0.6/LICENSE` & `scatcluster-0.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.6/setup.py` & `scatcluster-0.0.60/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Setup script for ScatCluster
+"""
 from setuptools import find_packages, setup
 
 NAME = 'scatcluster'
 DESCRIPTION = 'A workflow for clustering continuous time series with a deep scattering network.'
 URL = 'https://github.com/INGV/ScatCluster'
 AUTHOR = 'christopher.zerafa@ingv.it'
 REQUIRES_PYTHON = '>=3.8.0'
@@ -15,32 +18,32 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.6',
+    version='0.0.60',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
-    packages=find_packages('.'),
-    package_data={NAME: ['py.typed']},
+    packages=find_packages(where='.'),
+    package_data={NAME: ['scatcluster/*.py']},
     include_package_data=True,
     install_requires=REQUIRED,
     extras_require={'gpu': [*REQUIRED, *REQUIRED_GPU]},
-    license='Apache',
+    license='MIT',
     classifiers=[
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Natural Language :: English',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
```

