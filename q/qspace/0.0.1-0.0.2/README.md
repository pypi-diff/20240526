# Comparing `tmp/qspace-0.0.1.tar.gz` & `tmp/qspace-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qspace-0.0.1.tar", last modified: Sun May 26 02:23:21 2024, max compression
+gzip compressed data, was "qspace-0.0.2.tar", last modified: Sun May 26 02:29:22 2024, max compression
```

## Comparing `qspace-0.0.1.tar` & `qspace-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:23:21.375720 qspace-0.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 03:19:23.000000 qspace-0.0.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)    11716 2024-05-26 02:23:21.375720 qspace-0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10711 2024-05-25 03:53:50.000000 qspace-0.0.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:23:21.375720 qspace-0.0.1/qspace.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)    11716 2024-05-26 02:23:21.000000 qspace-0.0.1/qspace.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      208 2024-05-26 02:23:21.000000 qspace-0.0.1/qspace.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:23:21.000000 qspace-0.0.1/qspace.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       43 2024-05-26 02:23:21.000000 qspace-0.0.1/qspace.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 02:23:21.000000 qspace-0.0.1/qspace.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:23:21.000000 qspace-0.0.1/qspace.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 02:23:21.375720 qspace-0.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1417 2024-05-26 02:23:08.000000 qspace-0.0.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:29:22.463728 qspace-0.0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 03:19:23.000000 qspace-0.0.2/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12014 2024-05-26 02:29:22.459728 qspace-0.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11009 2024-05-26 02:29:01.000000 qspace-0.0.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:29:22.459728 qspace-0.0.2/qspace.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12014 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      208 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       43 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 02:29:22.463728 qspace-0.0.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1417 2024-05-26 02:29:11.000000 qspace-0.0.2/setup.py
```

### Comparing `qspace-0.0.1/LICENSE` & `qspace-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qspace-0.0.1/PKG-INFO` & `qspace-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qspace
-Version: 0.0.1
+Version: 0.0.2
 Summary: Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions.
 Home-page: 
 Author: rUv
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -38,14 +38,32 @@
 # Quantum Deployment Wizard
 ### Deploy every possibility, for everything, everywhere, all at once.
 
 ## Introduction
 
 Welcome to Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions. Whether you're a beginner or an advanced user, Q-Space provides a user-friendly interface to deploy, configure, and optimize quantum applications seamlessly.
 
+# Installation and Setup
+
+To get started with Q-Space, follow these steps:
+
+## Step 1: Install Q-Space
+
+Use the following pip command to install Q-Space:
+
+```sh
+pip install qspace
+```
+## Step 2: Run Q-Space
+After installing, you can start the Q-Space Deployment Wizard by running:
+
+```
+qspace
+```
+
 ## Brief Technical Introduction
 
 Q-Space leverages the power of Azure Quantum, a cloud-based quantum computing service, and Azure Functions, a serverless compute service, to create a robust framework for quantum computing. This combination allows users to run quantum algorithms, perform resource estimations, and manage quantum jobs efficiently.
 ## Features
 
 - 🚀 **Easy Mode**: Step-by-step guidance for setting up and deploying quantum applications.
 - 🔧 **Advanced Mode**: Granular control over each step of the deployment process.
```

### Comparing `qspace-0.0.1/README.md` & `qspace-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,32 @@
 # Quantum Deployment Wizard
 ### Deploy every possibility, for everything, everywhere, all at once.
 
 ## Introduction
 
 Welcome to Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions. Whether you're a beginner or an advanced user, Q-Space provides a user-friendly interface to deploy, configure, and optimize quantum applications seamlessly.
 
+# Installation and Setup
+
+To get started with Q-Space, follow these steps:
+
+## Step 1: Install Q-Space
+
+Use the following pip command to install Q-Space:
+
+```sh
+pip install qspace
+```
+## Step 2: Run Q-Space
+After installing, you can start the Q-Space Deployment Wizard by running:
+
+```
+qspace
+```
+
 ## Brief Technical Introduction
 
 Q-Space leverages the power of Azure Quantum, a cloud-based quantum computing service, and Azure Functions, a serverless compute service, to create a robust framework for quantum computing. This combination allows users to run quantum algorithms, perform resource estimations, and manage quantum jobs efficiently.
 ## Features
 
 - 🚀 **Easy Mode**: Step-by-step guidance for setting up and deploying quantum applications.
 - 🔧 **Advanced Mode**: Granular control over each step of the deployment process.
```

### Comparing `qspace-0.0.1/qspace.egg-info/PKG-INFO` & `qspace-0.0.2/qspace.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qspace
-Version: 0.0.1
+Version: 0.0.2
 Summary: Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions.
 Home-page: 
 Author: rUv
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -38,14 +38,32 @@
 # Quantum Deployment Wizard
 ### Deploy every possibility, for everything, everywhere, all at once.
 
 ## Introduction
 
 Welcome to Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions. Whether you're a beginner or an advanced user, Q-Space provides a user-friendly interface to deploy, configure, and optimize quantum applications seamlessly.
 
+# Installation and Setup
+
+To get started with Q-Space, follow these steps:
+
+## Step 1: Install Q-Space
+
+Use the following pip command to install Q-Space:
+
+```sh
+pip install qspace
+```
+## Step 2: Run Q-Space
+After installing, you can start the Q-Space Deployment Wizard by running:
+
+```
+qspace
+```
+
 ## Brief Technical Introduction
 
 Q-Space leverages the power of Azure Quantum, a cloud-based quantum computing service, and Azure Functions, a serverless compute service, to create a robust framework for quantum computing. This combination allows users to run quantum algorithms, perform resource estimations, and manage quantum jobs efficiently.
 ## Features
 
 - 🚀 **Easy Mode**: Step-by-step guidance for setting up and deploying quantum applications.
 - 🔧 **Advanced Mode**: Granular control over each step of the deployment process.
```

### Comparing `qspace-0.0.1/setup.py` & `qspace-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='qspace',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
         'black',
```

