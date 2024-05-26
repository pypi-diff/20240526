# Comparing `tmp/pipackager-0.4.3.tar.gz` & `tmp/pipackager-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipackager-0.4.3.tar", last modified: Sun May 26 02:52:30 2024, max compression
+gzip compressed data, was "pipackager-0.4.4.tar", last modified: Sun May 26 03:12:21 2024, max compression
```

## Comparing `pipackager-0.4.3.tar` & `pipackager-0.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:52:30.732677 pipackager-0.4.3/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.4.3/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 02:52:30.732677 pipackager-0.4.3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.4.3/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:52:30.728677 pipackager-0.4.3/pipackager/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.4.3/pipackager/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14989 2024-05-26 02:50:33.000000 pipackager-0.4.3/pipackager/cli.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:52:30.732677 pipackager-0.4.3/pipackager.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 02:52:30.000000 pipackager-0.4.3/pipackager.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-26 02:52:30.000000 pipackager-0.4.3/pipackager.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:52:30.000000 pipackager-0.4.3/pipackager.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-26 02:52:30.000000 pipackager-0.4.3/pipackager.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 02:52:30.000000 pipackager-0.4.3/pipackager.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-26 02:52:30.000000 pipackager-0.4.3/pipackager.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 02:52:30.732677 pipackager-0.4.3/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1510 2024-05-26 02:52:26.000000 pipackager-0.4.3/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:52:30.732677 pipackager-0.4.3/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.4.3/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.4.3/tests/test_pipackager.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:12:21.176669 pipackager-0.4.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.4.4/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 03:12:21.176669 pipackager-0.4.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.4.4/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:12:21.172669 pipackager-0.4.4/pipackager/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.4.4/pipackager/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14989 2024-05-26 02:50:33.000000 pipackager-0.4.4/pipackager/cli.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:12:21.176669 pipackager-0.4.4/pipackager.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 03:12:21.176669 pipackager-0.4.4/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1510 2024-05-26 03:12:16.000000 pipackager-0.4.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:12:21.176669 pipackager-0.4.4/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.4.4/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.4.4/tests/test_pipackager.py
```

### Comparing `pipackager-0.4.3/LICENSE` & `pipackager-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.3/PKG-INFO` & `pipackager-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.4.3
+Version: 0.4.4
 Summary: A tool to manage your PyPI package.
 Home-page: https://github.com/yourusername/pipackager
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pipackager-0.4.3/README.md` & `pipackager-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.3/pipackager/cli.py` & `pipackager-0.4.4/pipackager/cli.py`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.3/pipackager.egg-info/PKG-INFO` & `pipackager-0.4.4/pipackager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.4.3
+Version: 0.4.4
 Summary: A tool to manage your PyPI package.
 Home-page: https://github.com/yourusername/pipackager
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pipackager-0.4.3/setup.py` & `pipackager-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pipackager",
-    version="0.4.3",
+    version="0.4.4",
     packages=find_packages(),
     install_requires=[
         "twine",
         "setuptools",
         "wheel",
         "flake8",
         "black",
```

