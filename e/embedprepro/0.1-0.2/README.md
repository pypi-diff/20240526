# Comparing `tmp/embedprepro-0.1.tar.gz` & `tmp/embedprepro-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedprepro-0.1.tar", last modified: Sun May 26 13:38:42 2024, max compression
+gzip compressed data, was "embedprepro-0.2.tar", last modified: Sun May 26 15:29:49 2024, max compression
```

## Comparing `embedprepro-0.1.tar` & `embedprepro-0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-26 13:38:42.811947 embedprepro-0.1/
--rw-r--r--   0 eier       (501) staff       (20)       53 2024-05-26 13:38:42.811357 embedprepro-0.1/PKG-INFO
-drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-26 13:38:42.804772 embedprepro-0.1/embedprepro.egg-info/
--rw-r--r--   0 eier       (501) staff       (20)       53 2024-05-26 13:38:42.000000 embedprepro-0.1/embedprepro.egg-info/PKG-INFO
--rw-r--r--   0 eier       (501) staff       (20)      425 2024-05-26 13:38:42.000000 embedprepro-0.1/embedprepro.egg-info/SOURCES.txt
--rw-r--r--   0 eier       (501) staff       (20)        1 2024-05-26 13:38:42.000000 embedprepro-0.1/embedprepro.egg-info/dependency_links.txt
--rw-r--r--   0 eier       (501) staff       (20)       54 2024-05-26 13:38:42.000000 embedprepro-0.1/embedprepro.egg-info/entry_points.txt
--rw-r--r--   0 eier       (501) staff       (20)      769 2024-05-26 13:38:42.000000 embedprepro-0.1/embedprepro.egg-info/requires.txt
--rw-r--r--   0 eier       (501) staff       (20)       14 2024-05-26 13:38:42.000000 embedprepro-0.1/embedprepro.egg-info/top_level.txt
-drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-26 13:38:42.810141 embedprepro-0.1/preprocessing/
--rw-r--r--   0 eier       (501) staff       (20)        0 2024-05-25 20:53:37.000000 embedprepro-0.1/preprocessing/__init__.py
--rw-r--r--   0 eier       (501) staff       (20)     8560 2024-05-25 22:54:06.000000 embedprepro-0.1/preprocessing/agglomerative_clustering.py
--rw-r--r--   0 eier       (501) staff       (20)     6168 2024-05-26 12:50:08.000000 embedprepro-0.1/preprocessing/cli.py
--rw-r--r--   0 eier       (501) staff       (20)     8067 2024-05-25 23:33:31.000000 embedprepro-0.1/preprocessing/dimensionality_reduction.py
--rw-r--r--   0 eier       (501) staff       (20)     2028 2024-05-25 13:21:15.000000 embedprepro-0.1/preprocessing/embedding_service.py
--rw-r--r--   0 eier       (501) staff       (20)     3509 2024-05-26 12:37:01.000000 embedprepro-0.1/preprocessing/visualization_service.py
--rw-r--r--   0 eier       (501) staff       (20)       38 2024-05-26 13:38:42.812169 embedprepro-0.1/setup.cfg
--rw-r--r--   0 eier       (501) staff       (20)     1535 2024-05-26 13:38:22.000000 embedprepro-0.1/setup.py
+drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-26 15:29:49.363268 embedprepro-0.2/
+-rw-r--r--   0 eier       (501) staff       (20)     5473 2024-05-26 15:29:49.362603 embedprepro-0.2/PKG-INFO
+-rw-r--r--   0 eier       (501) staff       (20)     5379 2024-05-26 15:22:25.000000 embedprepro-0.2/README.md
+drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-26 15:29:49.353047 embedprepro-0.2/embedprepro.egg-info/
+-rw-r--r--   0 eier       (501) staff       (20)     5473 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/PKG-INFO
+-rw-r--r--   0 eier       (501) staff       (20)      435 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/SOURCES.txt
+-rw-r--r--   0 eier       (501) staff       (20)        1 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/dependency_links.txt
+-rw-r--r--   0 eier       (501) staff       (20)       54 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/entry_points.txt
+-rw-r--r--   0 eier       (501) staff       (20)      769 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/requires.txt
+-rw-r--r--   0 eier       (501) staff       (20)       14 2024-05-26 15:29:49.000000 embedprepro-0.2/embedprepro.egg-info/top_level.txt
+drwxr-xr-x   0 eier       (501) staff       (20)        0 2024-05-26 15:29:49.361388 embedprepro-0.2/preprocessing/
+-rw-r--r--   0 eier       (501) staff       (20)        0 2024-05-25 20:53:37.000000 embedprepro-0.2/preprocessing/__init__.py
+-rw-r--r--   0 eier       (501) staff       (20)     8560 2024-05-25 22:54:06.000000 embedprepro-0.2/preprocessing/agglomerative_clustering.py
+-rw-r--r--   0 eier       (501) staff       (20)     6168 2024-05-26 12:50:08.000000 embedprepro-0.2/preprocessing/cli.py
+-rw-r--r--   0 eier       (501) staff       (20)     8067 2024-05-25 23:33:31.000000 embedprepro-0.2/preprocessing/dimensionality_reduction.py
+-rw-r--r--   0 eier       (501) staff       (20)     2028 2024-05-25 13:21:15.000000 embedprepro-0.2/preprocessing/embedding_service.py
+-rw-r--r--   0 eier       (501) staff       (20)     3509 2024-05-26 12:37:01.000000 embedprepro-0.2/preprocessing/visualization_service.py
+-rw-r--r--   0 eier       (501) staff       (20)       38 2024-05-26 15:29:49.363479 embedprepro-0.2/setup.cfg
+-rw-r--r--   0 eier       (501) staff       (20)     1633 2024-05-26 15:29:00.000000 embedprepro-0.2/setup.py
```

### Comparing `embedprepro-0.1/embedprepro.egg-info/requires.txt` & `embedprepro-0.2/embedprepro.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `embedprepro-0.1/preprocessing/agglomerative_clustering.py` & `embedprepro-0.2/preprocessing/agglomerative_clustering.py`

 * *Files identical despite different names*

### Comparing `embedprepro-0.1/preprocessing/cli.py` & `embedprepro-0.2/preprocessing/cli.py`

 * *Files identical despite different names*

### Comparing `embedprepro-0.1/preprocessing/dimensionality_reduction.py` & `embedprepro-0.2/preprocessing/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `embedprepro-0.1/preprocessing/embedding_service.py` & `embedprepro-0.2/preprocessing/embedding_service.py`

 * *Files identical despite different names*

### Comparing `embedprepro-0.1/preprocessing/visualization_service.py` & `embedprepro-0.2/preprocessing/visualization_service.py`

 * *Files identical despite different names*

### Comparing `embedprepro-0.1/setup.py` & `embedprepro-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='embedprepro',
-    version='0.1',
+    version='0.2',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         "certifi==2024.2.2",
         "charset-normalizer==3.3.2",
         "click==8.1.7",
         "contourpy==1.2.1",
         "cycler==0.12.1",
```

