# Comparing `tmp/pipackager-0.4.4.tar.gz` & `tmp/pipackager-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipackager-0.4.4.tar", last modified: Sun May 26 03:12:21 2024, max compression
+gzip compressed data, was "pipackager-0.4.5.tar", last modified: Sun May 26 03:14:57 2024, max compression
```

## Comparing `pipackager-0.4.4.tar` & `pipackager-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:12:21.176669 pipackager-0.4.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.4.4/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 03:12:21.176669 pipackager-0.4.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.4.4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:12:21.172669 pipackager-0.4.4/pipackager/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.4.4/pipackager/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14989 2024-05-26 02:50:33.000000 pipackager-0.4.4/pipackager/cli.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:12:21.176669 pipackager-0.4.4/pipackager.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-26 03:12:21.000000 pipackager-0.4.4/pipackager.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 03:12:21.176669 pipackager-0.4.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1510 2024-05-26 03:12:16.000000 pipackager-0.4.4/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:12:21.176669 pipackager-0.4.4/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.4.4/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.4.4/tests/test_pipackager.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:57.828668 pipackager-0.4.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.4.5/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4550 2024-05-26 03:14:57.828668 pipackager-0.4.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.4.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:57.824668 pipackager-0.4.5/pipackager/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.4.5/pipackager/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14989 2024-05-26 02:50:33.000000 pipackager-0.4.5/pipackager/cli.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:57.828668 pipackager-0.4.5/pipackager.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4550 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-26 03:14:57.000000 pipackager-0.4.5/pipackager.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 03:14:57.828668 pipackager-0.4.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1498 2024-05-26 03:14:52.000000 pipackager-0.4.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 03:14:57.828668 pipackager-0.4.5/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.4.5/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.4.5/tests/test_pipackager.py
```

### Comparing `pipackager-0.4.4/LICENSE` & `pipackager-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.4/PKG-INFO` & `pipackager-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.4.4
+Version: 0.4.5
 Summary: A tool to manage your PyPI package.
-Home-page: https://github.com/yourusername/pipackager
-Author: Your Name
+Home-page: https://github.com/ruvnet/pipackager
+Author: rUv
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pipackager-0.4.4/README.md` & `pipackager-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.4/pipackager/cli.py` & `pipackager-0.4.5/pipackager/cli.py`

 * *Files identical despite different names*

### Comparing `pipackager-0.4.4/pipackager.egg-info/PKG-INFO` & `pipackager-0.4.5/pipackager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.4.4
+Version: 0.4.5
 Summary: A tool to manage your PyPI package.
-Home-page: https://github.com/yourusername/pipackager
-Author: Your Name
+Home-page: https://github.com/ruvnet/pipackager
+Author: rUv
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pipackager-0.4.4/setup.py` & `pipackager-0.4.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pipackager",
-    version="0.4.4",
+    version="0.4.5",
     packages=find_packages(),
     install_requires=[
         "twine",
         "setuptools",
         "wheel",
         "flake8",
         "black",
@@ -22,20 +22,20 @@
         "console_scripts": [
             "pipackager=pipackager.cli:main",
             # Ensure no duplicates like:
             # 'pipackager=pipackager.cli:main',
             # 'another_command=another.module:main_function',
         ],
     },
-    author="Your Name",
+    author="rUv",
     author_email="your-email@example.com",
     description="A tool to manage your PyPI package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/yourusername/pipackager",
+    url="https://github.com/ruvnet/pipackager",
     license="Apache License 2.0",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
```

