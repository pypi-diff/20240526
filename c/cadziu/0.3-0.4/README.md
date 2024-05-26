# Comparing `tmp/cadziu-0.3.tar.gz` & `tmp/cadziu-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadziu-0.3.tar", last modified: Sun May 26 12:29:45 2024, max compression
+gzip compressed data, was "cadziu-0.4.tar", last modified: Sun May 26 12:33:16 2024, max compression
```

## Comparing `cadziu-0.3.tar` & `cadziu-0.4.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:29:45.291055 cadziu-0.3/
--rw-r--r--   0 adam      (1001) adam      (1002)      502 2024-05-26 12:29:45.291055 cadziu-0.3/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-26 12:11:59.000000 cadziu-0.3/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:29:45.287055 cadziu-0.3/cadziu.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)      502 2024-05-26 12:29:45.000000 cadziu-0.3/cadziu.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      200 2024-05-26 12:29:45.000000 cadziu-0.3/cadziu.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 12:29:45.000000 cadziu-0.3/cadziu.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       41 2024-05-26 12:29:45.000000 cadziu-0.3/cadziu.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       23 2024-05-26 12:29:45.000000 cadziu-0.3/cadziu.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 12:29:45.000000 cadziu-0.3/cadziu.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 12:29:45.291055 cadziu-0.3/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)      802 2024-05-26 12:29:37.000000 cadziu-0.3/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:33:16.859789 cadziu-0.4/
+-rw-r--r--   0 adam      (1001) adam      (1002)      502 2024-05-26 12:33:16.855789 cadziu-0.4/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-26 12:11:59.000000 cadziu-0.4/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:33:16.843789 cadziu-0.4/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-26 12:32:11.000000 cadziu-0.4/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1839 2024-05-26 12:32:42.000000 cadziu-0.4/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2175 2024-05-26 12:32:50.000000 cadziu-0.4/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:33:16.851789 cadziu-0.4/cadziu.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)      502 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      241 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       41 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       23 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 12:33:16.859789 cadziu-0.4/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)      802 2024-05-26 12:32:29.000000 cadziu-0.4/setup.py
```

### Comparing `cadziu-0.3/setup.py` & `cadziu-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cadziu',
-    version='0.3',
+    version='0.4',
     author='Your Name',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadziu',
     packages=find_packages(),
```

