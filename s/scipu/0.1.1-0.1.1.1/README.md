# Comparing `tmp/scipu-0.1.1.tar.gz` & `tmp/scipu-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipu-0.1.1.tar", last modified: Sun May 26 13:00:09 2024, max compression
+gzip compressed data, was "scipu-0.1.1.1.tar", last modified: Sun May 26 13:03:50 2024, max compression
```

## Comparing `scipu-0.1.1.tar` & `scipu-0.1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 13:00:09.936678 scipu-0.1.1/
--rw-rw-rw-   0        0        0       38 2024-05-26 12:40:51.000000 scipu-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       18 2024-05-26 10:39:36.000000 scipu-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      389 2024-05-26 13:00:09.936678 scipu-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       31 2024-05-26 10:39:32.000000 scipu-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 13:00:09.928704 scipu-0.1.1/scipu/
--rw-rw-rw-   0        0        0       28 2024-05-26 12:55:43.000000 scipu-0.1.1/scipu/__init__.py
--rw-rw-rw-   0        0        0     5598 2024-05-26 11:31:26.000000 scipu-0.1.1/scipu/package.py
-drwxrwxrwx   0        0        0        0 2024-05-26 13:00:09.936678 scipu-0.1.1/scipu.egg-info/
--rw-rw-rw-   0        0        0      389 2024-05-26 13:00:09.000000 scipu-0.1.1/scipu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-05-26 13:00:09.000000 scipu-0.1.1/scipu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 13:00:09.000000 scipu-0.1.1/scipu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-26 13:00:09.000000 scipu-0.1.1/scipu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-05-26 13:00:09.937675 scipu-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      572 2024-05-26 12:55:25.000000 scipu-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:03:50.183155 scipu-0.1.1.1/
+-rw-rw-rw-   0        0        0       38 2024-05-26 12:40:51.000000 scipu-0.1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       18 2024-05-26 10:39:36.000000 scipu-0.1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      391 2024-05-26 13:03:50.183155 scipu-0.1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2024-05-26 10:39:32.000000 scipu-0.1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 13:03:50.177179 scipu-0.1.1.1/scipu/
+-rw-rw-rw-   0        0        0       23 2024-05-26 13:02:28.000000 scipu-0.1.1.1/scipu/__init__.py
+-rw-rw-rw-   0        0        0     5598 2024-05-26 11:31:26.000000 scipu-0.1.1.1/scipu/package.py
+drwxrwxrwx   0        0        0        0 2024-05-26 13:03:50.182158 scipu-0.1.1.1/scipu.egg-info/
+-rw-rw-rw-   0        0        0      391 2024-05-26 13:03:50.000000 scipu-0.1.1.1/scipu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-05-26 13:03:50.000000 scipu-0.1.1.1/scipu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 13:03:50.000000 scipu-0.1.1.1/scipu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-26 13:03:50.000000 scipu-0.1.1.1/scipu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-05-26 13:03:50.184152 scipu-0.1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      574 2024-05-26 13:03:34.000000 scipu-0.1.1.1/setup.py
```

### Comparing `scipu-0.1.1/scipu/package.py` & `scipu-0.1.1.1/scipu/package.py`

 * *Files identical despite different names*

### Comparing `scipu-0.1.1/setup.py` & `scipu-0.1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   with open('README.md', 'r') as f:
     return f.read()
 
 
 
 setup(
     name='scipu',
-    version='0.1.1',
+    version='0.1.1.1',
     packages=find_packages(),
     description='A simple TVIMS library',
     author='Ackrome',
     author_email='ivansergeyevicht@gmail.com',
     url='https://github.com/Ackrome/scipu',
     classifiers=[
         'Programming Language :: Python :: 3',
```

