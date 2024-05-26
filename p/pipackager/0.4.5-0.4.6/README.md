# Comparing `tmp/pipackager-0.4.5.tar.gz` & `tmp/pipackager-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipackager-0.4.5.tar", last modified: Sun May 26 03:14:57 2024, max compression
+gzip compressed data, was "pipackager-0.4.6.tar", last modified: Sun May 26 05:05:34 2024, max compression
```

## Comparing `pipackager-0.4.5.tar` & `pipackager-0.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:57.828668 pipackager-0.4.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.4.5/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4550 2024-05-26 03:14:57.828668 pipackager-0.4.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.4.5/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:57.824668 pipackager-0.4.5/pipackager/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.4.5/pipackager/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14989 2024-05-26 02:50:33.000000 pipackager-0.4.5/pipackager/cli.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:57.828668 pipackager-0.4.5/pipackager.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4550 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 03:14:57.828668 pipackager-0.4.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1498 2024-05-26 03:14:52.000000 pipackager-0.4.5/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:57.828668 pipackager-0.4.5/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.4.5/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.4.5/tests/test_pipackager.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:05:34.167940 pipackager-0.4.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.4.6/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4550 2024-05-26 05:05:34.167940 pipackager-0.4.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.4.6/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:05:34.163939 pipackager-0.4.6/pipackager/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.4.6/pipackager/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15186 2024-05-26 05:04:53.000000 pipackager-0.4.6/pipackager/cli.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:05:34.167940 pipackager-0.4.6/pipackager.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4550 2024-05-26 05:05:34.000000 pipackager-0.4.6/pipackager.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-26 05:05:34.000000 pipackager-0.4.6/pipackager.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 05:05:34.000000 pipackager-0.4.6/pipackager.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-26 05:05:34.000000 pipackager-0.4.6/pipackager.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 05:05:34.000000 pipackager-0.4.6/pipackager.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-26 05:05:34.000000 pipackager-0.4.6/pipackager.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 05:05:34.167940 pipackager-0.4.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1498 2024-05-26 05:05:29.000000 pipackager-0.4.6/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 05:05:34.167940 pipackager-0.4.6/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.4.6/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.4.6/tests/test_pipackager.py
```

### Comparing `pipackager-0.4.5/LICENSE` & `pipackager-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.5/PKG-INFO` & `pipackager-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.4.5
+Version: 0.4.6
 Summary: A tool to manage your PyPI package.
 Home-page: https://github.com/ruvnet/pipackager
 Author: rUv
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pipackager-0.4.5/README.md` & `pipackager-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.5/pipackager/cli.py` & `pipackager-0.4.6/pipackager/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,26 @@
 def create_setup_py():
     name = input("Enter the package name: ")
     version = input("Enter the package version (e.g., 0.1.0): ")
     author = input("Enter the author's name: ")
     author_email = input("Enter the author's email: ")
     description = input("Enter the package description: ")
     url = input("Enter the package URL: ")
+    entry_point = input("Enter the entry point for console scripts (leave blank if not applicable): ")
+
+    if entry_point:
+        entry_points = f"""
+    entry_points={{
+        'console_scripts': [
+            '{entry_point}',
+        ],
+    }},
+"""
+    else:
+        entry_points = ""
 
     setup_contents = f"""
 from setuptools import setup, find_packages
 from pathlib import Path
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
@@ -111,20 +123,15 @@
         'setuptools',
         'wheel',
         'flake8',
         'black',
         'pytest',
         'pip-upgrader',
     ],
-    entry_points={{
-        'console_scripts': [
-            '{name}={name}.cli:main',
-        ],
-    }},
-    author='{author}',
+{entry_points}    author='{author}',
     author_email='{author_email}',
     description='{description}',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='{url}',
     license='Apache License 2.0',
     classifiers=[
```

### Comparing `pipackager-0.4.5/pipackager.egg-info/PKG-INFO` & `pipackager-0.4.6/pipackager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.4.5
+Version: 0.4.6
 Summary: A tool to manage your PyPI package.
 Home-page: https://github.com/ruvnet/pipackager
 Author: rUv
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pipackager-0.4.5/setup.py` & `pipackager-0.4.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pipackager",
-    version="0.4.5",
+    version="0.4.6",
     packages=find_packages(),
     install_requires=[
         "twine",
         "setuptools",
         "wheel",
         "flake8",
         "black",
```

