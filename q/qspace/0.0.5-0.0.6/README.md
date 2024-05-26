# Comparing `tmp/qspace-0.0.5.tar.gz` & `tmp/qspace-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qspace-0.0.5.tar", last modified: Sun May 26 05:48:56 2024, max compression
+gzip compressed data, was "qspace-0.0.6.tar", last modified: Sun May 26 05:55:51 2024, max compression
```

## Comparing `qspace-0.0.5.tar` & `qspace-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:48:56.536397 qspace-0.0.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 03:19:23.000000 qspace-0.0.5/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)    12014 2024-05-26 05:48:56.536397 qspace-0.0.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11009 2024-05-26 02:29:01.000000 qspace-0.0.5/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:48:56.536397 qspace-0.0.5/qspace.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)    12014 2024-05-26 05:48:56.000000 qspace-0.0.5/qspace.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      208 2024-05-26 05:48:56.000000 qspace-0.0.5/qspace.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 05:48:56.000000 qspace-0.0.5/qspace.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       43 2024-05-26 05:48:56.000000 qspace-0.0.5/qspace.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 05:48:56.000000 qspace-0.0.5/qspace.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 05:48:56.000000 qspace-0.0.5/qspace.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 05:48:56.536397 qspace-0.0.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1417 2024-05-26 05:48:44.000000 qspace-0.0.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:55:51.676396 qspace-0.0.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 03:19:23.000000 qspace-0.0.6/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12098 2024-05-26 05:55:51.676396 qspace-0.0.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11009 2024-05-26 02:29:01.000000 qspace-0.0.6/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 05:55:51.676396 qspace-0.0.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1598 2024-05-26 05:55:49.000000 qspace-0.0.6/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:55:51.672396 qspace-0.0.6/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:55:51.676396 qspace-0.0.6/src/qspace.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12098 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      232 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       33 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       95 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 05:55:51.000000 qspace-0.0.6/src/qspace.egg-info/top_level.txt
```

### Comparing `qspace-0.0.5/LICENSE` & `qspace-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qspace-0.0.5/PKG-INFO` & `qspace-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: qspace
-Version: 0.0.5
+Version: 0.0.6
 Summary: Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions.
 Home-page: 
 Author: rUv
-Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -20,14 +19,18 @@
 Requires-Dist: twine
 Requires-Dist: setuptools
 Requires-Dist: wheel
 Requires-Dist: flake8
 Requires-Dist: black
 Requires-Dist: pytest
 Requires-Dist: pip-upgrader
+Requires-Dist: asyncclick
+Requires-Dist: azure-quantum
+Requires-Dist: qsharp
+Requires-Dist: pyyaml
 
 ```                                    
  _____ _____ _____ _____ _____ _____ 
 |     |   __|  _  |  _  |     |   __|
 |  |  |__   |   __|     |   --|   __|
 |__  _|_____|__|  |__|__|_____|_____|
    |__|
```

### Comparing `qspace-0.0.5/README.md` & `qspace-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `qspace-0.0.5/qspace.egg-info/PKG-INFO` & `qspace-0.0.6/src/qspace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: qspace
-Version: 0.0.5
+Version: 0.0.6
 Summary: Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions.
 Home-page: 
 Author: rUv
-Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -20,14 +19,18 @@
 Requires-Dist: twine
 Requires-Dist: setuptools
 Requires-Dist: wheel
 Requires-Dist: flake8
 Requires-Dist: black
 Requires-Dist: pytest
 Requires-Dist: pip-upgrader
+Requires-Dist: asyncclick
+Requires-Dist: azure-quantum
+Requires-Dist: qsharp
+Requires-Dist: pyyaml
 
 ```                                    
  _____ _____ _____ _____ _____ _____ 
 |     |   __|  _  |  _  |     |   __|
 |  |  |__   |   __|     |   --|   __|
 |__  _|_____|__|  |__|__|_____|_____|
    |__|
```

### Comparing `qspace-0.0.5/setup.py` & `qspace-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-
 from setuptools import setup, find_packages
 from pathlib import Path
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='qspace',
-    version='0.0.5',
-    packages=find_packages(),
+    version='0.0.6',
+    packages=find_packages(where='src'),  # Specify src directory
+    package_dir={'': 'src'},  # Define the root package directory
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
         'black',
         'pytest',
         'pip-upgrader',
+        'asyncclick',
+        'azure-quantum',
+        'qsharp',
+        'pyyaml',
     ],
     entry_points={
         'console_scripts': [
-            'qspace=qspace.cli:main',
+            'qspace=q:cli',  # Update to point to q.cli
         ],
     },
     author='rUv',
-    author_email='',
     description='Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     license='Apache License 2.0',
     classifiers=[
         'Development Status :: 3 - Alpha',
```

