# Comparing `tmp/ytsnippet-0.1.tar.gz` & `tmp/ytsnippet-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytsnippet-0.1.tar", last modified: Sun May 26 15:50:44 2024, max compression
+gzip compressed data, was "ytsnippet-0.2.tar", last modified: Sun May 26 16:38:43 2024, max compression
```

## Comparing `ytsnippet-0.1.tar` & `ytsnippet-0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 15:50:44.881730 ytsnippet-0.1/
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      437 2024-05-26 15:50:44.881522 ytsnippet-0.1/PKG-INFO
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 15:45:27.000000 ytsnippet-0.1/README.md
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       38 2024-05-26 15:50:44.881770 ytsnippet-0.1/setup.cfg
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      740 2024-05-26 15:46:46.000000 ytsnippet-0.1/setup.py
-drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 15:50:44.880551 ytsnippet-0.1/ytsnippet/
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 15:44:51.000000 ytsnippet-0.1/ytsnippet/__init__.py
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)     1562 2024-05-26 15:48:37.000000 ytsnippet-0.1/ytsnippet/cli.py
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      329 2024-05-26 15:46:34.000000 ytsnippet-0.1/ytsnippet/database.py
-drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 15:50:44.881347 ytsnippet-0.1/ytsnippet.egg-info/
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      437 2024-05-26 15:50:44.000000 ytsnippet-0.1/ytsnippet.egg-info/PKG-INFO
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      279 2024-05-26 15:50:44.000000 ytsnippet-0.1/ytsnippet.egg-info/SOURCES.txt
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        1 2024-05-26 15:50:44.000000 ytsnippet-0.1/ytsnippet.egg-info/dependency_links.txt
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       49 2024-05-26 15:50:44.000000 ytsnippet-0.1/ytsnippet.egg-info/entry_points.txt
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       15 2024-05-26 15:50:44.000000 ytsnippet-0.1/ytsnippet.egg-info/requires.txt
--rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       10 2024-05-26 15:50:44.000000 ytsnippet-0.1/ytsnippet.egg-info/top_level.txt
+drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:38:43.905421 ytsnippet-0.2/
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      567 2024-05-26 16:38:43.905213 ytsnippet-0.2/PKG-INFO
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      121 2024-05-26 16:29:24.000000 ytsnippet-0.2/README.md
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       38 2024-05-26 16:38:43.905458 ytsnippet-0.2/setup.cfg
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      748 2024-05-26 16:38:35.000000 ytsnippet-0.2/setup.py
+drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:38:43.903745 ytsnippet-0.2/tests/
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:25:31.000000 ytsnippet-0.2/tests/test_manager.py
+drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:38:43.904101 ytsnippet-0.2/ytsnippet/
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 15:44:51.000000 ytsnippet-0.2/ytsnippet/__init__.py
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)     3537 2024-05-26 16:29:37.000000 ytsnippet-0.2/ytsnippet/cli.py
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)     1658 2024-05-26 16:26:12.000000 ytsnippet-0.2/ytsnippet/database.py
+drwxr-xr-x   0 yokoyamatakumi   (501) staff       (20)        0 2024-05-26 16:38:43.904959 ytsnippet-0.2/ytsnippet.egg-info/
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      567 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/PKG-INFO
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)      301 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/SOURCES.txt
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)        1 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/dependency_links.txt
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       49 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/entry_points.txt
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       15 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/requires.txt
+-rw-r--r--   0 yokoyamatakumi   (501) staff       (20)       10 2024-05-26 16:38:43.000000 ytsnippet-0.2/ytsnippet.egg-info/top_level.txt
```

### Comparing `ytsnippet-0.1/setup.py` & `ytsnippet-0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ytsnippet',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'ytsnippet=ytsnippet.cli:main',
         ],
     },
     install_requires=['prompt_toolkit'],
     author='Your Name',
-    author_email='your.email@example.com',
+    author_email='s2222038@stu.musashino-u.ac.jp',
     description='A simple code snippet manager',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/ytsnippet',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

