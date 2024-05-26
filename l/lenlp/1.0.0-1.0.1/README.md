# Comparing `tmp/lenlp-1.0.0.tar.gz` & `tmp/lenlp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenlp-1.0.0.tar", last modified: Sun May 26 00:45:33 2024, max compression
+gzip compressed data, was "lenlp-1.0.1.tar", last modified: Sun May 26 01:37:25 2024, max compression
```

## Comparing `lenlp-1.0.0.tar` & `lenlp-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-26 00:45:33.625884 lenlp-1.0.0/
--rw-r--r--   0 raphael    (502) staff       (20)      479 2024-05-25 23:39:02.000000 lenlp-1.0.0/Cargo.toml
--rw-r--r--   0 raphael    (502) staff       (20)       46 2024-05-25 21:19:28.000000 lenlp-1.0.0/MANIFEST.in
--rw-r--r--   0 raphael    (502) staff       (20)      791 2024-05-26 00:45:33.625671 lenlp-1.0.0/PKG-INFO
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-26 00:45:33.622676 lenlp-1.0.0/lenlp/
--rw-r--r--   0 raphael    (502) staff       (20)       90 2024-05-25 23:40:24.000000 lenlp-1.0.0/lenlp/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)       63 2024-05-25 23:38:57.000000 lenlp-1.0.0/lenlp/__version__.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-26 00:45:33.623584 lenlp-1.0.0/lenlp/analyzer/
--rw-r--r--   0 raphael    (502) staff       (20)       59 2024-05-25 23:41:55.000000 lenlp-1.0.0/lenlp/analyzer/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     1921 2024-05-25 23:41:56.000000 lenlp-1.0.0/lenlp/analyzer/analyze.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-26 00:45:33.623855 lenlp-1.0.0/lenlp/counter/
--rw-r--r--   0 raphael    (502) staff       (20)       46 2024-05-25 23:16:39.000000 lenlp-1.0.0/lenlp/counter/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     3909 2024-05-25 23:22:57.000000 lenlp-1.0.0/lenlp/counter/count.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-26 00:45:33.624118 lenlp-1.0.0/lenlp/flash/
--rw-r--r--   0 raphael    (502) staff       (20)       59 2024-05-24 12:15:01.000000 lenlp-1.0.0/lenlp/flash/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     1414 2024-05-25 21:01:20.000000 lenlp-1.0.0/lenlp/flash/flash_text.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-26 00:45:33.624443 lenlp-1.0.0/lenlp/normalizer/
--rw-r--r--   0 raphael    (502) staff       (20)       58 2024-05-25 23:23:17.000000 lenlp-1.0.0/lenlp/normalizer/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)      493 2024-05-25 23:22:55.000000 lenlp-1.0.0/lenlp/normalizer/normalize.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-26 00:45:33.624982 lenlp-1.0.0/lenlp/sparse/
--rw-r--r--   0 raphael    (502) staff       (20)      204 2024-05-25 13:12:31.000000 lenlp-1.0.0/lenlp/sparse/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     3749 2024-05-25 21:01:08.000000 lenlp-1.0.0/lenlp/sparse/bm25_vectorizer.py
--rw-r--r--   0 raphael    (502) staff       (20)     3649 2024-05-25 21:01:26.000000 lenlp-1.0.0/lenlp/sparse/count_vectorizer.py
--rw-r--r--   0 raphael    (502) staff       (20)     3864 2024-05-25 21:01:23.000000 lenlp-1.0.0/lenlp/sparse/tfidf_vectorizer.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-26 00:45:33.625134 lenlp-1.0.0/lenlp.egg-info/
--rw-r--r--   0 raphael    (502) staff       (20)      791 2024-05-26 00:45:33.000000 lenlp-1.0.0/lenlp.egg-info/PKG-INFO
--rw-r--r--   0 raphael    (502) staff       (20)      548 2024-05-26 00:45:33.000000 lenlp-1.0.0/lenlp.egg-info/SOURCES.txt
--rw-r--r--   0 raphael    (502) staff       (20)        1 2024-05-26 00:45:33.000000 lenlp-1.0.0/lenlp.egg-info/dependency_links.txt
--rw-r--r--   0 raphael    (502) staff       (20)      135 2024-05-26 00:45:33.000000 lenlp-1.0.0/lenlp.egg-info/requires.txt
--rw-r--r--   0 raphael    (502) staff       (20)        6 2024-05-26 00:45:33.000000 lenlp-1.0.0/lenlp.egg-info/top_level.txt
--rw-r--r--   0 raphael    (502) staff       (20)       38 2024-05-26 00:45:33.625939 lenlp-1.0.0/setup.cfg
--rw-r--r--   0 raphael    (502) staff       (20)     1027 2024-05-26 00:39:26.000000 lenlp-1.0.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.709364 lenlp-1.0.1/
+-rw-r--r--   0 runner     (501) staff       (20)      479 2024-05-26 01:35:47.000000 lenlp-1.0.1/Cargo.toml
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-26 01:35:47.000000 lenlp-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)      447 2024-05-26 01:37:25.709189 lenlp-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.705540 lenlp-1.0.1/lenlp/
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/__version__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.706565 lenlp-1.0.1/lenlp/analyzer/
+-rw-r--r--   0 runner     (501) staff       (20)       59 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/analyzer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1921 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/analyzer/analyze.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.707027 lenlp-1.0.1/lenlp/counter/
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/counter/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3909 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/counter/count.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.707454 lenlp-1.0.1/lenlp/flash/
+-rw-r--r--   0 runner     (501) staff       (20)       59 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/flash/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1414 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/flash/flash_text.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.707992 lenlp-1.0.1/lenlp/normalizer/
+-rw-r--r--   0 runner     (501) staff       (20)       58 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/normalizer/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      493 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/normalizer/normalize.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.708897 lenlp-1.0.1/lenlp/sparse/
+-rw-r--r--   0 runner     (501) staff       (20)      204 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/sparse/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3749 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/sparse/bm25_vectorizer.py
+-rw-r--r--   0 runner     (501) staff       (20)     3649 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/sparse/count_vectorizer.py
+-rw-r--r--   0 runner     (501) staff       (20)     3864 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/sparse/tfidf_vectorizer.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.706189 lenlp-1.0.1/lenlp.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      447 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      548 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      135 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-26 01:37:25.709437 lenlp-1.0.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1027 2024-05-26 01:35:47.000000 lenlp-1.0.1/setup.py
```

### Comparing `lenlp-1.0.0/lenlp/analyzer/analyze.py` & `lenlp-1.0.1/lenlp/analyzer/analyze.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.0/lenlp/counter/count.py` & `lenlp-1.0.1/lenlp/counter/count.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.0/lenlp/flash/flash_text.py` & `lenlp-1.0.1/lenlp/flash/flash_text.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.0/lenlp/sparse/bm25_vectorizer.py` & `lenlp-1.0.1/lenlp/sparse/bm25_vectorizer.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.0/lenlp/sparse/count_vectorizer.py` & `lenlp-1.0.1/lenlp/sparse/count_vectorizer.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.0/lenlp/sparse/tfidf_vectorizer.py` & `lenlp-1.0.1/lenlp/sparse/tfidf_vectorizer.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.0/lenlp.egg-info/SOURCES.txt` & `lenlp-1.0.1/lenlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.0/setup.py` & `lenlp-1.0.1/setup.py`

 * *Files identical despite different names*

