# Comparing `tmp/openrouter_selector-0.0.1.tar.gz` & `tmp/openrouter_selector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrouter_selector-0.0.1.tar", last modified: Sun May 26 16:23:54 2024, max compression
+gzip compressed data, was "openrouter_selector-0.0.2.tar", last modified: Sun May 26 16:51:12 2024, max compression
```

## Comparing `openrouter_selector-0.0.1.tar` & `openrouter_selector-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hirosekento   (501) staff       (20)        0 2024-05-26 16:23:54.721401 openrouter_selector-0.0.1/
--rw-r--r--   0 hirosekento   (501) staff       (20)     1061 2024-05-26 15:00:06.000000 openrouter_selector-0.0.1/LICENSE
--rw-r--r--   0 hirosekento   (501) staff       (20)      554 2024-05-26 16:23:54.721044 openrouter_selector-0.0.1/PKG-INFO
--rw-r--r--   0 hirosekento   (501) staff       (20)       78 2024-05-26 15:07:58.000000 openrouter_selector-0.0.1/README.md
--rw-r--r--   0 hirosekento   (501) staff       (20)      477 2024-05-26 16:23:43.000000 openrouter_selector-0.0.1/pyproject.toml
--rw-r--r--   0 hirosekento   (501) staff       (20)       38 2024-05-26 16:23:54.721542 openrouter_selector-0.0.1/setup.cfg
-drwxr-xr-x   0 hirosekento   (501) staff       (20)        0 2024-05-26 16:23:54.717835 openrouter_selector-0.0.1/src/
-drwxr-xr-x   0 hirosekento   (501) staff       (20)        0 2024-05-26 16:23:54.719269 openrouter_selector-0.0.1/src/openrouter_selector/
--rw-r--r--   0 hirosekento   (501) staff       (20)      638 2024-05-26 16:08:01.000000 openrouter_selector-0.0.1/src/openrouter_selector/selector.py
--rw-r--r--   0 hirosekento   (501) staff       (20)       54 2024-05-26 16:08:00.000000 openrouter_selector-0.0.1/src/openrouter_selector/＿init＿.py
-drwxr-xr-x   0 hirosekento   (501) staff       (20)        0 2024-05-26 16:23:54.720679 openrouter_selector-0.0.1/src/openrouter_selector.egg-info/
--rw-r--r--   0 hirosekento   (501) staff       (20)      554 2024-05-26 16:23:54.000000 openrouter_selector-0.0.1/src/openrouter_selector.egg-info/PKG-INFO
--rw-r--r--   0 hirosekento   (501) staff       (20)      340 2024-05-26 16:23:54.000000 openrouter_selector-0.0.1/src/openrouter_selector.egg-info/SOURCES.txt
--rw-r--r--   0 hirosekento   (501) staff       (20)        1 2024-05-26 16:23:54.000000 openrouter_selector-0.0.1/src/openrouter_selector.egg-info/dependency_links.txt
--rw-r--r--   0 hirosekento   (501) staff       (20)       15 2024-05-26 16:23:54.000000 openrouter_selector-0.0.1/src/openrouter_selector.egg-info/requires.txt
--rw-r--r--   0 hirosekento   (501) staff       (20)       20 2024-05-26 16:23:54.000000 openrouter_selector-0.0.1/src/openrouter_selector.egg-info/top_level.txt
+drwxr-xr-x   0 hirosekento   (501) staff       (20)        0 2024-05-26 16:51:12.705923 openrouter_selector-0.0.2/
+-rw-r--r--   0 hirosekento   (501) staff       (20)     1061 2024-05-26 15:00:06.000000 openrouter_selector-0.0.2/LICENSE
+-rw-r--r--   0 hirosekento   (501) staff       (20)      999 2024-05-26 16:51:12.705549 openrouter_selector-0.0.2/PKG-INFO
+-rw-r--r--   0 hirosekento   (501) staff       (20)      547 2024-05-26 16:47:23.000000 openrouter_selector-0.0.2/README.md
+-rw-r--r--   0 hirosekento   (501) staff       (20)      450 2024-05-26 16:50:08.000000 openrouter_selector-0.0.2/pyproject.toml
+-rw-r--r--   0 hirosekento   (501) staff       (20)       38 2024-05-26 16:51:12.705991 openrouter_selector-0.0.2/setup.cfg
+drwxr-xr-x   0 hirosekento   (501) staff       (20)        0 2024-05-26 16:51:12.701617 openrouter_selector-0.0.2/src/
+drwxr-xr-x   0 hirosekento   (501) staff       (20)        0 2024-05-26 16:51:12.703256 openrouter_selector-0.0.2/src/openrouter_selector/
+-rw-r--r--   0 hirosekento   (501) staff       (20)      638 2024-05-26 16:47:11.000000 openrouter_selector-0.0.2/src/openrouter_selector/selector.py
+-rw-r--r--   0 hirosekento   (501) staff       (20)       54 2024-05-26 16:08:00.000000 openrouter_selector-0.0.2/src/openrouter_selector/＿init＿.py
+drwxr-xr-x   0 hirosekento   (501) staff       (20)        0 2024-05-26 16:51:12.705166 openrouter_selector-0.0.2/src/openrouter_selector.egg-info/
+-rw-r--r--   0 hirosekento   (501) staff       (20)      999 2024-05-26 16:51:12.000000 openrouter_selector-0.0.2/src/openrouter_selector.egg-info/PKG-INFO
+-rw-r--r--   0 hirosekento   (501) staff       (20)      340 2024-05-26 16:51:12.000000 openrouter_selector-0.0.2/src/openrouter_selector.egg-info/SOURCES.txt
+-rw-r--r--   0 hirosekento   (501) staff       (20)        1 2024-05-26 16:51:12.000000 openrouter_selector-0.0.2/src/openrouter_selector.egg-info/dependency_links.txt
+-rw-r--r--   0 hirosekento   (501) staff       (20)       15 2024-05-26 16:51:12.000000 openrouter_selector-0.0.2/src/openrouter_selector.egg-info/requires.txt
+-rw-r--r--   0 hirosekento   (501) staff       (20)       20 2024-05-26 16:51:12.000000 openrouter_selector-0.0.2/src/openrouter_selector.egg-info/top_level.txt
```

### Comparing `openrouter_selector-0.0.1/LICENSE` & `openrouter_selector-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openrouter_selector-0.0.1/src/openrouter_selector/selector.py` & `openrouter_selector-0.0.2/src/openrouter_selector/selector.py`

 * *Files identical despite different names*

