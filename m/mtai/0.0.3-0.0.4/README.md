# Comparing `tmp/mtai-0.0.3.tar.gz` & `tmp/mtai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mtai-0.0.3.tar", last modified: Thu May 23 19:36:32 2024, max compression
+gzip compressed data, was "mtai-0.0.4.tar", last modified: Sun May 26 10:24:45 2024, max compression
```

## Comparing `mtai-0.0.3.tar` & `mtai-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:36:32.543308 mtai-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 19:36:08.000000 mtai-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-23 19:36:32.539308 mtai-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-23 19:36:08.000000 mtai-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:36:32.539308 mtai-0.0.3/mtai/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 19:36:08.000000 mtai-0.0.3/mtai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-23 19:36:08.000000 mtai-0.0.3/mtai/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 19:36:08.000000 mtai-0.0.3/mtai/mt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-23 19:36:08.000000 mtai-0.0.3/mtai/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:36:32.539308 mtai-0.0.3/mtai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-23 19:36:32.000000 mtai-0.0.3/mtai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-23 19:36:32.000000 mtai-0.0.3/mtai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:36:32.000000 mtai-0.0.3/mtai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 19:36:32.000000 mtai-0.0.3/mtai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 19:36:32.000000 mtai-0.0.3/mtai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:36:32.543308 mtai-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-23 19:36:08.000000 mtai-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:24:45.440832 mtai-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-26 10:24:19.000000 mtai-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-26 10:24:45.440832 mtai-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-26 10:24:19.000000 mtai-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:24:45.440832 mtai-0.0.4/mtai/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/mt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-26 10:24:19.000000 mtai-0.0.4/mtai/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:24:45.440832 mtai-0.0.4/mtai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-26 10:24:45.000000 mtai-0.0.4/mtai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 10:24:45.440832 mtai-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-26 10:24:19.000000 mtai-0.0.4/setup.py
```

### Comparing `mtai-0.0.3/LICENSE` & `mtai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mtai-0.0.3/PKG-INFO` & `mtai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtai
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library to consume meditranscribe ai API
 Home-page: https://github.com/mediatranscribe/mt-ai-python
 Author: KtechHub
 Author-email: pypi@ktechhub.com
 License: MIT
 Keywords: mtai mediatranscribe mtaiapi python library
 Classifier: Intended Audience :: Developers
```

### Comparing `mtai-0.0.3/README.md` & `mtai-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mtai-0.0.3/mtai/base.py` & `mtai-0.0.4/mtai/base.py`

 * *Files identical despite different names*

### Comparing `mtai-0.0.3/mtai/tags.py` & `mtai-0.0.4/mtai/tags.py`

 * *Files identical despite different names*

### Comparing `mtai-0.0.3/mtai.egg-info/PKG-INFO` & `mtai-0.0.4/mtai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtai
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python library to consume meditranscribe ai API
 Home-page: https://github.com/mediatranscribe/mt-ai-python
 Author: KtechHub
 Author-email: pypi@ktechhub.com
 License: MIT
 Keywords: mtai mediatranscribe mtaiapi python library
 Classifier: Intended Audience :: Developers
```

### Comparing `mtai-0.0.3/setup.py` & `mtai-0.0.4/setup.py`

 * *Files identical despite different names*

