# Comparing `tmp/pipackager-0.4.1.tar.gz` & `tmp/pipackager-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipackager-0.4.1.tar", last modified: Sun May 26 02:16:32 2024, max compression
+gzip compressed data, was "pipackager-0.4.2.tar", last modified: Sun May 26 02:18:48 2024, max compression
```

## Comparing `pipackager-0.4.1.tar` & `pipackager-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:16:32.516690 pipackager-0.4.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.4.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 02:16:32.516690 pipackager-0.4.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.4.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:16:32.512690 pipackager-0.4.1/pipackager/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.4.1/pipackager/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14941 2024-05-26 02:15:14.000000 pipackager-0.4.1/pipackager/cli.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:16:32.516690 pipackager-0.4.1/pipackager.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 02:16:32.000000 pipackager-0.4.1/pipackager.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-26 02:16:32.000000 pipackager-0.4.1/pipackager.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:16:32.000000 pipackager-0.4.1/pipackager.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-26 02:16:32.000000 pipackager-0.4.1/pipackager.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 02:16:32.000000 pipackager-0.4.1/pipackager.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-26 02:16:32.000000 pipackager-0.4.1/pipackager.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 02:16:32.516690 pipackager-0.4.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1511 2024-05-26 02:15:52.000000 pipackager-0.4.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:16:32.516690 pipackager-0.4.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.4.1/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.4.1/tests/test_pipackager.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:18:48.072689 pipackager-0.4.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.4.2/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 02:18:48.072689 pipackager-0.4.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.4.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:18:48.056690 pipackager-0.4.2/pipackager/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.4.2/pipackager/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14990 2024-05-26 02:18:15.000000 pipackager-0.4.2/pipackager/cli.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:18:48.060690 pipackager-0.4.2/pipackager.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 02:18:47.000000 pipackager-0.4.2/pipackager.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-26 02:18:48.000000 pipackager-0.4.2/pipackager.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:18:47.000000 pipackager-0.4.2/pipackager.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-26 02:18:47.000000 pipackager-0.4.2/pipackager.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 02:18:47.000000 pipackager-0.4.2/pipackager.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-26 02:18:47.000000 pipackager-0.4.2/pipackager.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 02:18:48.072689 pipackager-0.4.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1511 2024-05-26 02:18:42.000000 pipackager-0.4.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:18:48.072689 pipackager-0.4.2/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.4.2/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.4.2/tests/test_pipackager.py
```

### Comparing `pipackager-0.4.1/LICENSE` & `pipackager-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.1/PKG-INFO` & `pipackager-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.4.1
+Version: 0.4.2
 Summary: A tool to manage your PyPI package.
 Home-page: https://github.com/yourusername/pipackager
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pipackager-0.4.1/README.md` & `pipackager-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.1/pipackager/cli.py` & `pipackager-0.4.2/pipackager/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import subprocess
 import sys
 
 def show_menu():
     clear()
     print("***********************************")
     print("*        PyPI Package Manager     *")
+    print("*              by rUv             *")
     print("***********************************")
     print("1. Initial Setup")
     print("2. Clean old distributions")
     print("3. Build new distributions")
     print("4. Upload distributions to PyPI")
     print("5. Increment version number (patch)")
     print("6. Increment version number (minor)")
```

### Comparing `pipackager-0.4.1/pipackager.egg-info/PKG-INFO` & `pipackager-0.4.2/pipackager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.4.1
+Version: 0.4.2
 Summary: A tool to manage your PyPI package.
 Home-page: https://github.com/yourusername/pipackager
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pipackager-0.4.1/setup.py` & `pipackager-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pipackager",
-    version="0.4.1",
+    version="0.4.2",
     packages=find_packages(),
     install_requires=[
         "twine",
         "setuptools",
         "wheel",
         "flake8",
         "black",
```

