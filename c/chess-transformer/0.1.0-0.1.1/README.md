# Comparing `tmp/chess_transformer-0.1.0.tar.gz` & `tmp/chess_transformer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess_transformer-0.1.0.tar", last modified: Sun May 26 18:24:48 2024, max compression
+gzip compressed data, was "chess_transformer-0.1.1.tar", last modified: Sun May 26 18:32:35 2024, max compression
```

## Comparing `chess_transformer-0.1.0.tar` & `chess_transformer-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:24:48.856927 chess_transformer-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      323 2024-05-26 18:24:48.856927 chess_transformer-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-26 16:42:39.000000 chess_transformer-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      523 2024-05-26 16:42:39.000000 chess_transformer-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-26 18:24:48.856927 chess_transformer-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:24:48.846927 chess_transformer-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:24:48.856927 chess_transformer-0.1.0/src/chess_transformer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-26 17:06:39.000000 chess_transformer-0.1.0/src/chess_transformer/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:24:48.856927 chess_transformer-0.1.0/src/chess_transformer/data/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      161 2024-05-26 18:20:18.000000 chess_transformer-0.1.0/src/chess_transformer/data/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      787 2024-05-26 18:16:42.000000 chess_transformer-0.1.0/src/chess_transformer/data/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1949 2024-05-26 18:20:06.000000 chess_transformer-0.1.0/src/chess_transformer/data/mask.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      768 2024-05-26 17:53:57.000000 chess_transformer-0.1.0/src/chess_transformer/data/random.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:24:48.856927 chess_transformer-0.1.0/src/chess_transformer/vocab/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      168 2024-05-26 18:05:22.000000 chess_transformer-0.1.0/src/chess_transformer/vocab/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)    12034 2024-05-26 16:57:10.000000 chess_transformer-0.1.0/src/chess_transformer/vocab/sans.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      822 2024-05-26 18:06:59.000000 chess_transformer-0.1.0/src/chess_transformer/vocab/vocab.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:24:48.856927 chess_transformer-0.1.0/src/chess_transformer.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      323 2024-05-26 18:24:48.000000 chess_transformer-0.1.0/src/chess_transformer.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      500 2024-05-26 18:24:48.000000 chess_transformer-0.1.0/src/chess_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-26 18:24:48.000000 chess_transformer-0.1.0/src/chess_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-26 18:24:48.000000 chess_transformer-0.1.0/src/chess_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:32:35.706928 chess_transformer-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      323 2024-05-26 18:32:35.706928 chess_transformer-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-26 16:42:39.000000 chess_transformer-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      523 2024-05-26 18:32:30.000000 chess_transformer-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-26 18:32:35.706928 chess_transformer-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:32:35.696928 chess_transformer-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:32:35.706928 chess_transformer-0.1.1/src/chess_transformer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-05-26 17:06:39.000000 chess_transformer-0.1.1/src/chess_transformer/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:32:35.706928 chess_transformer-0.1.1/src/chess_transformer/data/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      173 2024-05-26 18:29:19.000000 chess_transformer-0.1.1/src/chess_transformer/data/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      787 2024-05-26 18:16:42.000000 chess_transformer-0.1.1/src/chess_transformer/data/dataset.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2559 2024-05-26 18:29:11.000000 chess_transformer-0.1.1/src/chess_transformer/data/mask.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      768 2024-05-26 17:53:57.000000 chess_transformer-0.1.1/src/chess_transformer/data/random.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:32:35.706928 chess_transformer-0.1.1/src/chess_transformer/vocab/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      168 2024-05-26 18:05:22.000000 chess_transformer-0.1.1/src/chess_transformer/vocab/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)    12034 2024-05-26 16:57:10.000000 chess_transformer-0.1.1/src/chess_transformer/vocab/sans.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      822 2024-05-26 18:06:59.000000 chess_transformer-0.1.1/src/chess_transformer/vocab/vocab.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-26 18:32:35.706928 chess_transformer-0.1.1/src/chess_transformer.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      323 2024-05-26 18:32:35.000000 chess_transformer-0.1.1/src/chess_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      500 2024-05-26 18:32:35.000000 chess_transformer-0.1.1/src/chess_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-26 18:32:35.000000 chess_transformer-0.1.1/src/chess_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       18 2024-05-26 18:32:35.000000 chess_transformer-0.1.1/src/chess_transformer.egg-info/top_level.txt
```

### Comparing `chess_transformer-0.1.0/pyproject.toml` & `chess_transformer-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-transformer"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread goes smarter, baby"
 dependencies = [
   
 ]
```

### Comparing `chess_transformer-0.1.0/src/chess_transformer/data/dataset.py` & `chess_transformer-0.1.1/src/chess_transformer/data/dataset.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.0/src/chess_transformer/data/random.py` & `chess_transformer-0.1.1/src/chess_transformer/data/random.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.0/src/chess_transformer/vocab/sans.py` & `chess_transformer-0.1.1/src/chess_transformer/vocab/sans.py`

 * *Files identical despite different names*

### Comparing `chess_transformer-0.1.0/src/chess_transformer/vocab/vocab.py` & `chess_transformer-0.1.1/src/chess_transformer/vocab/vocab.py`

 * *Files identical despite different names*

