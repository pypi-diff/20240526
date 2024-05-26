# Comparing `tmp/hypt-0.0.1.tar.gz` & `tmp/hypt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypt-0.0.1.tar", last modified: Thu May 23 17:10:37 2024, max compression
+gzip compressed data, was "hypt-0.1.0.tar", last modified: Sun May 26 08:34:15 2024, max compression
```

## Comparing `hypt-0.0.1.tar` & `hypt-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,24 @@
-drwxrwxr-x   0 ajoo      (1000) ajoo      (1000)        0 2024-05-23 17:10:37.361392 hypt-0.0.1/
--rw-rw-r--   0 ajoo      (1000) ajoo      (1000)     1068 2024-05-23 17:01:09.000000 hypt-0.0.1/LICENSE
--rw-r--r--   0 ajoo      (1000) ajoo      (1000)      199 2024-05-23 17:10:37.361392 hypt-0.0.1/PKG-INFO
--rw-rw-r--   0 ajoo      (1000) ajoo      (1000)       46 2024-05-23 17:01:09.000000 hypt-0.0.1/README.md
--rw-rw-r--   0 ajoo      (1000) ajoo      (1000)       38 2024-05-23 17:10:37.361392 hypt-0.0.1/setup.cfg
--rw-rw-r--   0 ajoo      (1000) ajoo      (1000)      299 2024-05-23 17:03:44.000000 hypt-0.0.1/setup.py
-drwxrwxr-x   0 ajoo      (1000) ajoo      (1000)        0 2024-05-23 17:10:37.361392 hypt-0.0.1/src/
-drwxrwxr-x   0 ajoo      (1000) ajoo      (1000)        0 2024-05-23 17:10:37.361392 hypt-0.0.1/src/hypt/
--rw-rw-r--   0 ajoo      (1000) ajoo      (1000)        0 2024-05-23 17:04:09.000000 hypt-0.0.1/src/hypt/__init__.py
-drwxrwxr-x   0 ajoo      (1000) ajoo      (1000)        0 2024-05-23 17:10:37.361392 hypt-0.0.1/src/hypt.egg-info/
--rw-r--r--   0 ajoo      (1000) ajoo      (1000)      199 2024-05-23 17:10:37.000000 hypt-0.0.1/src/hypt.egg-info/PKG-INFO
--rw-rw-r--   0 ajoo      (1000) ajoo      (1000)      206 2024-05-23 17:10:37.000000 hypt-0.0.1/src/hypt.egg-info/SOURCES.txt
--rw-rw-r--   0 ajoo      (1000) ajoo      (1000)        1 2024-05-23 17:10:37.000000 hypt-0.0.1/src/hypt.egg-info/dependency_links.txt
--rw-rw-r--   0 ajoo      (1000) ajoo      (1000)        6 2024-05-23 17:10:37.000000 hypt-0.0.1/src/hypt.egg-info/requires.txt
--rw-rw-r--   0 ajoo      (1000) ajoo      (1000)        5 2024-05-23 17:10:37.000000 hypt-0.0.1/src/hypt.egg-info/top_level.txt
+drwxrwxr-x   0 ajoo      (1000) ajoo      (1000)        0 2024-05-26 08:34:15.247002 hypt-0.1.0/
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)     1068 2024-05-23 17:01:09.000000 hypt-0.1.0/LICENSE
+-rw-r--r--   0 ajoo      (1000) ajoo      (1000)      199 2024-05-26 08:34:15.247002 hypt-0.1.0/PKG-INFO
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)     3683 2024-05-26 08:18:15.000000 hypt-0.1.0/README.md
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)       38 2024-05-26 08:34:15.247002 hypt-0.1.0/setup.cfg
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)      300 2024-05-26 08:06:48.000000 hypt-0.1.0/setup.py
+drwxrwxr-x   0 ajoo      (1000) ajoo      (1000)        0 2024-05-26 08:34:15.247002 hypt-0.1.0/src/
+drwxrwxr-x   0 ajoo      (1000) ajoo      (1000)        0 2024-05-26 08:34:15.247002 hypt-0.1.0/src/hypt/
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)       79 2024-05-25 17:19:33.000000 hypt-0.1.0/src/hypt/__init__.py
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)     9749 2024-05-25 21:58:19.000000 hypt-0.1.0/src/hypt/distributions.py
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)     4189 2024-05-23 17:29:26.000000 hypt-0.1.0/src/hypt/line_search.py
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)       32 2024-05-23 18:15:18.000000 hypt-0.1.0/src/hypt/param_dict.py
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)       33 2024-05-25 17:05:11.000000 hypt-0.1.0/src/hypt/random.py
+-rwxrwxrwx   0 ajoo      (1000) ajoo      (1000)     2835 2024-05-25 17:15:08.000000 hypt-0.1.0/src/hypt/static.py
+drwxrwxr-x   0 ajoo      (1000) ajoo      (1000)        0 2024-05-26 08:34:15.247002 hypt-0.1.0/src/hypt.egg-info/
+-rw-r--r--   0 ajoo      (1000) ajoo      (1000)      199 2024-05-26 08:34:15.000000 hypt-0.1.0/src/hypt.egg-info/PKG-INFO
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)      385 2024-05-26 08:34:15.000000 hypt-0.1.0/src/hypt.egg-info/SOURCES.txt
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)        1 2024-05-26 08:34:15.000000 hypt-0.1.0/src/hypt.egg-info/dependency_links.txt
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)        6 2024-05-26 08:34:15.000000 hypt-0.1.0/src/hypt.egg-info/requires.txt
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)        5 2024-05-26 08:34:15.000000 hypt-0.1.0/src/hypt.egg-info/top_level.txt
+drwxrwxr-x   0 ajoo      (1000) ajoo      (1000)        0 2024-05-26 08:34:15.247002 hypt-0.1.0/tests/
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)     1324 2024-05-25 22:36:04.000000 hypt-0.1.0/tests/test_ch.py
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)      461 2024-05-25 21:39:57.000000 hypt-0.1.0/tests/test_parallel.py
+-rw-rw-r--   0 ajoo      (1000) ajoo      (1000)      565 2024-05-25 17:18:05.000000 hypt-0.1.0/tests/test_random_search.py
```

### Comparing `hypt-0.0.1/LICENSE` & `hypt-0.1.0/LICENSE`

 * *Files identical despite different names*

