# Comparing `tmp/qspace-0.0.6.tar.gz` & `tmp/qspace-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qspace-0.0.6.tar", last modified: Sun May 26 05:55:51 2024, max compression
+gzip compressed data, was "qspace-0.0.7.tar", last modified: Sun May 26 06:01:19 2024, max compression
```

## Comparing `qspace-0.0.6.tar` & `qspace-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:55:51.676396 qspace-0.0.6/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 03:19:23.000000 qspace-0.0.6/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)    12098 2024-05-26 05:55:51.676396 qspace-0.0.6/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11009 2024-05-26 02:29:01.000000 qspace-0.0.6/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 05:55:51.676396 qspace-0.0.6/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-05-26 05:55:49.000000 qspace-0.0.6/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:55:51.672396 qspace-0.0.6/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:55:51.676396 qspace-0.0.6/src/qspace.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)    12098 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      232 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       33 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       95 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 06:01:19.572395 qspace-0.0.7/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 03:19:23.000000 qspace-0.0.7/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12098 2024-05-26 06:01:19.572395 qspace-0.0.7/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11009 2024-05-26 02:29:01.000000 qspace-0.0.7/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 06:01:19.572395 qspace-0.0.7/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-05-26 06:01:17.000000 qspace-0.0.7/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 06:01:19.568395 qspace-0.0.7/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 06:01:19.572395 qspace-0.0.7/src/qspace.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12098 2024-05-26 06:01:19.000000 qspace-0.0.7/src/qspace.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      232 2024-05-26 06:01:19.000000 qspace-0.0.7/src/qspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 06:01:19.000000 qspace-0.0.7/src/qspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       33 2024-05-26 06:01:19.000000 qspace-0.0.7/src/qspace.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       95 2024-05-26 06:01:19.000000 qspace-0.0.7/src/qspace.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 06:01:19.000000 qspace-0.0.7/src/qspace.egg-info/top_level.txt
```

### Comparing `qspace-0.0.6/LICENSE` & `qspace-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qspace-0.0.6/PKG-INFO` & `qspace-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qspace
-Version: 0.0.6
+Version: 0.0.7
 Summary: Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions.
 Home-page: 
 Author: rUv
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

### Comparing `qspace-0.0.6/README.md` & `qspace-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `qspace-0.0.6/setup.py` & `qspace-0.0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='qspace',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(where='src'),  # Specify src directory
     package_dir={'': 'src'},  # Define the root package directory
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
```

### Comparing `qspace-0.0.6/src/qspace.egg-info/PKG-INFO` & `qspace-0.0.7/src/qspace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qspace
-Version: 0.0.6
+Version: 0.0.7
 Summary: Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions.
 Home-page: 
 Author: rUv
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

