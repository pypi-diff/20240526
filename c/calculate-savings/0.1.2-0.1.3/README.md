# Comparing `tmp/calculate_savings-0.1.2.tar.gz` & `tmp/calculate_savings-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculate_savings-0.1.2.tar", last modified: Sat May 25 11:28:22 2024, max compression
+gzip compressed data, was "calculate_savings-0.1.3.tar", last modified: Sun May 26 12:48:05 2024, max compression
```

## Comparing `calculate_savings-0.1.2.tar` & `calculate_savings-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-25 11:28:22.339226 calculate_savings-0.1.2/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       23 2024-05-21 13:12:43.000000 calculate_savings-0.1.2/MANIFEST.in
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      992 2024-05-25 11:28:22.339029 calculate_savings-0.1.2/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      429 2024-05-25 11:27:47.000000 calculate_savings-0.1.2/README.md
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-25 11:28:22.339267 calculate_savings-0.1.2/setup.cfg
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     1094 2024-05-25 11:28:07.000000 calculate_savings-0.1.2/setup.py
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-25 11:28:22.324535 calculate_savings-0.1.2/src/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     6148 2024-05-21 13:35:14.000000 calculate_savings-0.1.2/src/.DS_Store
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-25 11:28:22.338798 calculate_savings-0.1.2/src/calculate_savings.egg-info/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      992 2024-05-25 11:28:22.000000 calculate_savings-0.1.2/src/calculate_savings.egg-info/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      329 2024-05-25 11:28:22.000000 calculate_savings-0.1.2/src/calculate_savings.egg-info/SOURCES.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-25 11:28:22.000000 calculate_savings-0.1.2/src/calculate_savings.egg-info/dependency_links.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       61 2024-05-25 11:28:22.000000 calculate_savings-0.1.2/src/calculate_savings.egg-info/entry_points.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-25 11:28:22.000000 calculate_savings-0.1.2/src/calculate_savings.egg-info/top_level.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     4747 2024-05-25 11:19:57.000000 calculate_savings-0.1.2/src/calculate_savings.py
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-25 11:28:22.325198 calculate_savings-0.1.2/src/data/
--rw-r--r--   0 takenakayuuki   (501) staff       (20) 19188118 2024-05-21 05:28:42.000000 calculate_savings-0.1.2/src/data/hon-maikin-k-jissu.csv
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-26 12:48:04.999641 calculate_savings-0.1.3/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       23 2024-05-21 13:12:43.000000 calculate_savings-0.1.3/MANIFEST.in
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     1228 2024-05-26 12:48:04.999439 calculate_savings-0.1.3/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      666 2024-05-26 12:46:41.000000 calculate_savings-0.1.3/README.md
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-26 12:48:04.999678 calculate_savings-0.1.3/setup.cfg
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     1094 2024-05-26 12:47:37.000000 calculate_savings-0.1.3/setup.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-26 12:48:04.983550 calculate_savings-0.1.3/src/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     6148 2024-05-21 13:35:14.000000 calculate_savings-0.1.3/src/.DS_Store
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-26 12:48:04.999164 calculate_savings-0.1.3/src/calculate_savings.egg-info/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     1228 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      329 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/SOURCES.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/dependency_links.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       61 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/entry_points.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/top_level.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     4747 2024-05-25 11:19:57.000000 calculate_savings-0.1.3/src/calculate_savings.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-26 12:48:04.984221 calculate_savings-0.1.3/src/data/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20) 19188118 2024-05-21 05:28:42.000000 calculate_savings-0.1.3/src/data/hon-maikin-k-jissu.csv
```

### Comparing `calculate_savings-0.1.2/setup.py` & `calculate_savings-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="calculate_savings",
-    version="0.1.2",
+    version="0.1.3",
     author="YukiTakenaka",
     author_email="s2222024@stu.musashino-u.ac.jp",
     description="How much can you save in 10 years by predicting your salary?",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/takenakayuuki0901/calculate_savings.git",
     project_urls={
```

### Comparing `calculate_savings-0.1.2/src/.DS_Store` & `calculate_savings-0.1.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `calculate_savings-0.1.2/src/calculate_savings.py` & `calculate_savings-0.1.3/src/calculate_savings.py`

 * *Files identical despite different names*

### Comparing `calculate_savings-0.1.2/src/data/hon-maikin-k-jissu.csv` & `calculate_savings-0.1.3/src/data/hon-maikin-k-jissu.csv`

 * *Files identical despite different names*

