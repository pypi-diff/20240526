# Comparing `tmp/socialdataanalysis-0.2.tar.gz` & `tmp/socialdataanalysis-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialdataanalysis-0.2.tar", last modified: Wed May 22 20:16:09 2024, max compression
+gzip compressed data, was "socialdataanalysis-0.3.tar", last modified: Sat May 25 23:55:28 2024, max compression
```

## Comparing `socialdataanalysis-0.2.tar` & `socialdataanalysis-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:16:09.158135 socialdataanalysis-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 20:15:55.000000 socialdataanalysis-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-22 20:16:09.158135 socialdataanalysis-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 20:15:55.000000 socialdataanalysis-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:16:09.158135 socialdataanalysis-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-22 20:15:55.000000 socialdataanalysis-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:16:09.154135 socialdataanalysis-0.2/socialdataanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:15:55.000000 socialdataanalysis-0.2/socialdataanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66512 2024-05-22 20:15:55.000000 socialdataanalysis-0.2/socialdataanalysis/funcoes_personalizadas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:16:09.158135 socialdataanalysis-0.2/socialdataanalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-22 20:16:09.000000 socialdataanalysis-0.2/socialdataanalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-22 20:16:09.000000 socialdataanalysis-0.2/socialdataanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:16:09.000000 socialdataanalysis-0.2/socialdataanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 20:16:09.000000 socialdataanalysis-0.2/socialdataanalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 20:16:09.000000 socialdataanalysis-0.2/socialdataanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:55:28.776494 socialdataanalysis-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-25 23:55:20.000000 socialdataanalysis-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-25 23:55:28.776494 socialdataanalysis-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-25 23:55:20.000000 socialdataanalysis-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:55:28.776494 socialdataanalysis-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-25 23:55:20.000000 socialdataanalysis-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:55:28.776494 socialdataanalysis-0.3/socialdataanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:55:20.000000 socialdataanalysis-0.3/socialdataanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66512 2024-05-25 23:55:20.000000 socialdataanalysis-0.3/socialdataanalysis/association.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:55:28.776494 socialdataanalysis-0.3/socialdataanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-25 23:55:28.000000 socialdataanalysis-0.3/socialdataanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-25 23:55:28.000000 socialdataanalysis-0.3/socialdataanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:55:28.000000 socialdataanalysis-0.3/socialdataanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-25 23:55:28.000000 socialdataanalysis-0.3/socialdataanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 23:55:28.000000 socialdataanalysis-0.3/socialdataanalysis.egg-info/top_level.txt
```

### Comparing `socialdataanalysis-0.2/LICENSE` & `socialdataanalysis-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.2/PKG-INFO` & `socialdataanalysis-0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.2
+Version: 0.3
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `socialdataanalysis-0.2/socialdataanalysis/funcoes_personalizadas.py` & `socialdataanalysis-0.3/socialdataanalysis/association.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.2/socialdataanalysis.egg-info/PKG-INFO` & `socialdataanalysis-0.3/socialdataanalysis.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.2
+Version: 0.3
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

