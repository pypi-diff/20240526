# Comparing `tmp/scatcluster-0.0.5.tar.gz` & `tmp/scatcluster-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.5.tar", last modified: Sun Apr 28 16:12:38 2024, max compression
+gzip compressed data, was "scatcluster-0.0.6.tar", last modified: Sun Apr 28 16:13:51 2024, max compression
```

## Comparing `scatcluster-0.0.5.tar` & `scatcluster-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:12:38.631622 scatcluster-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-28 16:12:35.000000 scatcluster-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-28 16:12:35.000000 scatcluster-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 16:12:38.631622 scatcluster-0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 16:12:38.631622 scatcluster-0.0.5/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-28 16:12:38.000000 scatcluster-0.0.5/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-28 16:12:38.000000 scatcluster-0.0.5/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:12:38.000000 scatcluster-0.0.5/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-28 16:12:38.000000 scatcluster-0.0.5/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 16:12:38.000000 scatcluster-0.0.5/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 16:12:38.631622 scatcluster-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-28 16:12:36.000000 scatcluster-0.0.5/setup.py
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

### Comparing `scatcluster-0.0.5/LICENSE` & `scatcluster-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.5/PKG-INFO` & `scatcluster-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.5
+Version: 0.0.6
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.5/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.6/scatcluster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.5
+Version: 0.0.6
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: Apache
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.5/setup.py` & `scatcluster-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.5',
+    version='0.0.6',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages('.'),
     package_data={NAME: ['py.typed']},
```

