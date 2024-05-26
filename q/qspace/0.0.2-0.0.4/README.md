# Comparing `tmp/qspace-0.0.2.tar.gz` & `tmp/qspace-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qspace-0.0.2.tar", last modified: Sun May 26 02:29:22 2024, max compression
+gzip compressed data, was "qspace-0.0.4.tar", last modified: Sun May 26 03:14:05 2024, max compression
```

## Comparing `qspace-0.0.2.tar` & `qspace-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:29:22.463728 qspace-0.0.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 03:19:23.000000 qspace-0.0.2/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)    12014 2024-05-26 02:29:22.459728 qspace-0.0.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11009 2024-05-26 02:29:01.000000 qspace-0.0.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:29:22.459728 qspace-0.0.2/qspace.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)    12014 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      208 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       43 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:29:22.000000 qspace-0.0.2/qspace.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 02:29:22.463728 qspace-0.0.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1417 2024-05-26 02:29:11.000000 qspace-0.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:05.079787 qspace-0.0.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 03:19:23.000000 qspace-0.0.4/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12014 2024-05-26 03:14:05.079787 qspace-0.0.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11009 2024-05-26 02:29:01.000000 qspace-0.0.4/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:05.079787 qspace-0.0.4/qspace.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    12014 2024-05-26 03:14:04.000000 qspace-0.0.4/qspace.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      208 2024-05-26 03:14:05.000000 qspace-0.0.4/qspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 03:14:04.000000 qspace-0.0.4/qspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       43 2024-05-26 03:14:04.000000 qspace-0.0.4/qspace.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 03:14:04.000000 qspace-0.0.4/qspace.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 03:14:04.000000 qspace-0.0.4/qspace.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 03:14:05.079787 qspace-0.0.4/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1417 2024-05-26 03:13:59.000000 qspace-0.0.4/setup.py
```

### Comparing `qspace-0.0.2/LICENSE` & `qspace-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qspace-0.0.2/PKG-INFO` & `qspace-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qspace
-Version: 0.0.2
+Version: 0.0.4
 Summary: Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions.
 Home-page: 
 Author: rUv
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qspace-0.0.2/README.md` & `qspace-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qspace-0.0.2/qspace.egg-info/PKG-INFO` & `qspace-0.0.4/qspace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qspace
-Version: 0.0.2
+Version: 0.0.4
 Summary: Q-Space, a cutting-edge deployment wizard designed to simplify the process of setting up and managing quantum computing applications using Azure Quantum and Azure Functions.
 Home-page: 
 Author: rUv
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `qspace-0.0.2/setup.py` & `qspace-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='qspace',
-    version='0.0.2',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
         'black',
```

