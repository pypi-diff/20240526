# Comparing `tmp/dscontexai-0.0.1.tar.gz` & `tmp/dscontexai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscontexai-0.0.1.tar", last modified: Sun May 26 13:37:53 2024, max compression
+gzip compressed data, was "dscontexai-0.0.2.tar", last modified: Sun May 26 13:46:46 2024, max compression
```

## Comparing `dscontexai-0.0.1.tar` & `dscontexai-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:37:53.909228 dscontexai-0.0.1/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:37:53.905228 dscontexai-0.0.1/PKG-INFO
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:37:53.905228 dscontexai-0.0.1/dscontexai/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       96 2024-05-26 12:20:55.000000 dscontexai-0.0.1/dscontexai/__init__.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3601 2024-05-26 10:20:02.000000 dscontexai-0.0.1/dscontexai/generate_report.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10463 2024-05-26 09:55:24.000000 dscontexai-0.0.1/dscontexai/grammar.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)    10176 2024-05-26 09:38:15.000000 dscontexai-0.0.1/dscontexai/grammar_with_box_latex.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     3495 2024-05-26 09:49:20.000000 dscontexai-0.0.1/dscontexai/ploting.py
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1405 2024-05-26 05:49:34.000000 dscontexai-0.0.1/dscontexai/xgboost.py
-drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:37:53.905228 dscontexai-0.0.1/dscontexai.egg-info/
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:37:53.000000 dscontexai-0.0.1/dscontexai.egg-info/PKG-INFO
--rw-rw-r--   0 harisk    (1000) harisk    (1000)      333 2024-05-26 13:37:53.000000 dscontexai-0.0.1/dscontexai.egg-info/SOURCES.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 13:37:53.000000 dscontexai-0.0.1/dscontexai.egg-info/dependency_links.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     1059 2024-05-26 13:37:53.000000 dscontexai-0.0.1/dscontexai.egg-info/requires.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 13:37:53.000000 dscontexai-0.0.1/dscontexai.egg-info/top_level.txt
--rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 13:37:53.909228 dscontexai-0.0.1/setup.cfg
--rw-rw-r--   0 harisk    (1000) harisk    (1000)     2393 2024-05-26 13:37:17.000000 dscontexai-0.0.1/setup.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:46:46.526155 dscontexai-0.0.2/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:46:46.526155 dscontexai-0.0.2/PKG-INFO
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:46:46.526155 dscontexai-0.0.2/dscontexai/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      100 2024-05-26 13:46:04.000000 dscontexai-0.0.2/dscontexai/__init__.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3601 2024-05-26 10:20:02.000000 dscontexai-0.0.2/dscontexai/generate_report.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10463 2024-05-26 09:55:24.000000 dscontexai-0.0.2/dscontexai/grammar.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)    10176 2024-05-26 09:38:15.000000 dscontexai-0.0.2/dscontexai/grammar_with_box_latex.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     3495 2024-05-26 09:49:20.000000 dscontexai-0.0.2/dscontexai/ploting.py
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1405 2024-05-26 05:49:34.000000 dscontexai-0.0.2/dscontexai/xgboost.py
+drwxrwxr-x   0 harisk    (1000) harisk    (1000)        0 2024-05-26 13:46:46.526155 dscontexai-0.0.2/dscontexai.egg-info/
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      443 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/PKG-INFO
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)      333 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)        1 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     1059 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/requires.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       11 2024-05-26 13:46:46.000000 dscontexai-0.0.2/dscontexai.egg-info/top_level.txt
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)       38 2024-05-26 13:46:46.526155 dscontexai-0.0.2/setup.cfg
+-rw-rw-r--   0 harisk    (1000) harisk    (1000)     2393 2024-05-26 13:46:20.000000 dscontexai-0.0.2/setup.py
```

### Comparing `dscontexai-0.0.1/dscontexai/generate_report.py` & `dscontexai-0.0.2/dscontexai/generate_report.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.1/dscontexai/grammar.py` & `dscontexai-0.0.2/dscontexai/grammar.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.1/dscontexai/grammar_with_box_latex.py` & `dscontexai-0.0.2/dscontexai/grammar_with_box_latex.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.1/dscontexai/ploting.py` & `dscontexai-0.0.2/dscontexai/ploting.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.1/dscontexai/xgboost.py` & `dscontexai-0.0.2/dscontexai/xgboost.py`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.1/dscontexai.egg-info/requires.txt` & `dscontexai-0.0.2/dscontexai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dscontexai-0.0.1/setup.py` & `dscontexai-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "ConteXAI"
 LONG_DESCRIPTION = "xAI for everyone!"
 
 # Setting up
 setup(
     name="dscontexai",
     version=VERSION,
```

