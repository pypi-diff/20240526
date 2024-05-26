# Comparing `tmp/clipboardhist-1.0.4.tar.gz` & `tmp/clipboardhist-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipboardhist-1.0.4.tar", last modified: Fri May 24 20:55:30 2024, max compression
+gzip compressed data, was "clipboardhist-1.0.5.tar", last modified: Sun May 26 14:51:38 2024, max compression
```

## Comparing `clipboardhist-1.0.4.tar` & `clipboardhist-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-24 20:55:30.998283 clipboardhist-1.0.4/
--rw-r--r--   0 shiro      (501) staff       (20)     1068 2024-05-24 17:25:54.000000 clipboardhist-1.0.4/LICENSE
--rw-r--r--   0 shiro      (501) staff       (20)     1014 2024-05-24 20:55:30.998108 clipboardhist-1.0.4/PKG-INFO
--rw-r--r--   0 shiro      (501) staff       (20)      554 2024-05-24 19:22:55.000000 clipboardhist-1.0.4/README.md
-drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-24 20:55:30.996922 clipboardhist-1.0.4/clipboardhist/
--rw-r--r--   0 shiro      (501) staff       (20)      228 2024-05-24 20:35:38.000000 clipboardhist-1.0.4/clipboardhist/__init__.py
--rw-r--r--   0 shiro      (501) staff       (20)     2064 2024-05-24 18:57:22.000000 clipboardhist-1.0.4/clipboardhist/clipboardhist.py
-drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-24 20:55:30.997861 clipboardhist-1.0.4/clipboardhist.egg-info/
--rw-r--r--   0 shiro      (501) staff       (20)     1014 2024-05-24 20:55:30.000000 clipboardhist-1.0.4/clipboardhist.egg-info/PKG-INFO
--rw-r--r--   0 shiro      (501) staff       (20)      267 2024-05-24 20:55:30.000000 clipboardhist-1.0.4/clipboardhist.egg-info/SOURCES.txt
--rw-r--r--   0 shiro      (501) staff       (20)        1 2024-05-24 20:55:30.000000 clipboardhist-1.0.4/clipboardhist.egg-info/dependency_links.txt
--rw-r--r--   0 shiro      (501) staff       (20)       10 2024-05-24 20:55:30.000000 clipboardhist-1.0.4/clipboardhist.egg-info/requires.txt
--rw-r--r--   0 shiro      (501) staff       (20)       14 2024-05-24 20:55:30.000000 clipboardhist-1.0.4/clipboardhist.egg-info/top_level.txt
--rw-r--r--   0 shiro      (501) staff       (20)       38 2024-05-24 20:55:30.998339 clipboardhist-1.0.4/setup.cfg
--rw-r--r--   0 shiro      (501) staff       (20)      748 2024-05-24 20:55:14.000000 clipboardhist-1.0.4/setup.py
+drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-26 14:51:38.858051 clipboardhist-1.0.5/
+-rw-r--r--   0 shiro      (501) staff       (20)     1068 2024-05-24 17:25:54.000000 clipboardhist-1.0.5/LICENSE
+-rw-r--r--   0 shiro      (501) staff       (20)     1014 2024-05-26 14:51:38.857875 clipboardhist-1.0.5/PKG-INFO
+-rw-r--r--   0 shiro      (501) staff       (20)      554 2024-05-24 19:22:55.000000 clipboardhist-1.0.5/README.md
+drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-26 14:51:38.856504 clipboardhist-1.0.5/clipboardhist/
+-rw-r--r--   0 shiro      (501) staff       (20)      228 2024-05-26 14:51:23.000000 clipboardhist-1.0.5/clipboardhist/__init__.py
+-rw-r--r--   0 shiro      (501) staff       (20)     2064 2024-05-24 18:57:22.000000 clipboardhist-1.0.5/clipboardhist/clipboardhist.py
+drwxr-xr-x   0 shiro      (501) staff       (20)        0 2024-05-26 14:51:38.857624 clipboardhist-1.0.5/clipboardhist.egg-info/
+-rw-r--r--   0 shiro      (501) staff       (20)     1014 2024-05-26 14:51:38.000000 clipboardhist-1.0.5/clipboardhist.egg-info/PKG-INFO
+-rw-r--r--   0 shiro      (501) staff       (20)      267 2024-05-26 14:51:38.000000 clipboardhist-1.0.5/clipboardhist.egg-info/SOURCES.txt
+-rw-r--r--   0 shiro      (501) staff       (20)        1 2024-05-26 14:51:38.000000 clipboardhist-1.0.5/clipboardhist.egg-info/dependency_links.txt
+-rw-r--r--   0 shiro      (501) staff       (20)       10 2024-05-26 14:51:38.000000 clipboardhist-1.0.5/clipboardhist.egg-info/requires.txt
+-rw-r--r--   0 shiro      (501) staff       (20)       14 2024-05-26 14:51:38.000000 clipboardhist-1.0.5/clipboardhist.egg-info/top_level.txt
+-rw-r--r--   0 shiro      (501) staff       (20)       38 2024-05-26 14:51:38.858121 clipboardhist-1.0.5/setup.cfg
+-rw-r--r--   0 shiro      (501) staff       (20)      748 2024-05-26 14:51:28.000000 clipboardhist-1.0.5/setup.py
```

### Comparing `clipboardhist-1.0.4/LICENSE` & `clipboardhist-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clipboardhist-1.0.4/PKG-INFO` & `clipboardhist-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipboardhist
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple tool for managing clipboard history.
 Home-page: https://github.com/h1l2o/clipboardhist
 Author: HIRO TAKAGI
 Author-email: s2222103@stu.musashino-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clipboardhist-1.0.4/README.md` & `clipboardhist-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `clipboardhist-1.0.4/clipboardhist/clipboardhist.py` & `clipboardhist-1.0.5/clipboardhist/clipboardhist.py`

 * *Files identical despite different names*

### Comparing `clipboardhist-1.0.4/clipboardhist.egg-info/PKG-INFO` & `clipboardhist-1.0.5/clipboardhist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipboardhist
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple tool for managing clipboard history.
 Home-page: https://github.com/h1l2o/clipboardhist
 Author: HIRO TAKAGI
 Author-email: s2222103@stu.musashino-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clipboardhist-1.0.4/setup.py` & `clipboardhist-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='clipboardhist',
-    version='1.0.4',
+    version='1.0.5',
     description='A simple tool for managing clipboard history.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='HIRO TAKAGI',
     author_email='s2222103@stu.musashino-u.ac.jp',
     url='https://github.com/h1l2o/clipboardhist',
     packages=find_packages(),
```

