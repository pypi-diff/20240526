# Comparing `tmp/dicio_py-1.0.tar.gz` & `tmp/dicio_py-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicio_py-1.0.tar", last modified: Sun May 26 14:45:12 2024, max compression
+gzip compressed data, was "dicio_py-1.1.tar", last modified: Sun May 26 15:05:52 2024, max compression
```

## Comparing `dicio_py-1.0.tar` & `dicio_py-1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:45:12.428502 dicio_py-1.0/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.0/LICENSE
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1596 2024-05-26 14:45:12.428502 dicio_py-1.0/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.0/README.md
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:45:12.428502 dicio_py-1.0/dicio_py.egg-info/
--rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1596 2024-05-26 14:45:12.000000 dicio_py-1.0/dicio_py.egg-info/PKG-INFO
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      170 2024-05-26 14:45:12.000000 dicio_py-1.0/dicio_py.egg-info/SOURCES.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-26 14:45:12.000000 dicio_py-1.0/dicio_py.egg-info/dependency_links.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        4 2024-05-26 14:45:12.000000 dicio_py-1.0/dicio_py.egg-info/top_level.txt
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-26 14:45:12.428502 dicio_py-1.0/setup.cfg
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      605 2024-05-26 14:27:32.000000 dicio_py-1.0/setup.py
-drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:45:12.428502 dicio_py-1.0/src/
--rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.0/src/__init__.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 15:05:52.509818 dicio_py-1.1/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)    35149 2024-05-26 14:04:54.000000 dicio_py-1.1/LICENSE
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1619 2024-05-26 15:05:52.505818 dicio_py-1.1/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)     1236 2024-05-26 14:43:55.000000 dicio_py-1.1/README.md
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 15:05:52.501818 dicio_py-1.1/dicio_py.egg-info/
+-rw-r--r--   0 jeiel     (1000) jeiel     (1000)     1619 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/PKG-INFO
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      205 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        1 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       43 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/entry_points.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        4 2024-05-26 15:05:52.000000 dicio_py-1.1/dicio_py.egg-info/top_level.txt
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)       38 2024-05-26 15:05:52.509818 dicio_py-1.1/setup.cfg
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)      738 2024-05-26 15:05:18.000000 dicio_py-1.1/setup.py
+drwxrwxr-x   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 15:05:52.501818 dicio_py-1.1/src/
+-rw-rw-r--   0 jeiel     (1000) jeiel     (1000)        0 2024-05-26 14:28:37.000000 dicio_py-1.1/src/__init__.py
```

### Comparing `dicio_py-1.0/LICENSE` & `dicio_py-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicio_py-1.0/PKG-INFO` & `dicio_py-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.0
+Version: 1.1
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dicio-py
 Um dicionário com interface de terminal (Dessa vez feito em Python para ser multiplataforma)
 
 > Este script faz um web scraping no site: https://www.dicio.com.br/ e formata o retorno em um agradável texto em terminal.
```

### Comparing `dicio_py-1.0/README.md` & `dicio_py-1.1/README.md`

 * *Files identical despite different names*

### Comparing `dicio_py-1.0/dicio_py.egg-info/PKG-INFO` & `dicio_py-1.1/dicio_py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: dicio-py
-Version: 1.0
+Version: 1.1
 Summary: Dicionário via CLI
 Home-page: https://github.com/Jetrom17/dicio-py
 Author: Jetrom17
 Author-email: Jeiel@duck.com
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dicio-py
 Um dicionário com interface de terminal (Dessa vez feito em Python para ser multiplataforma)
 
 > Este script faz um web scraping no site: https://www.dicio.com.br/ e formata o retorno em um agradável texto em terminal.
```

