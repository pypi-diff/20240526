# Comparing `tmp/pproject-0.0.3.tar.gz` & `tmp/pproject-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pproject-0.0.3.tar", last modified: Sat May 25 16:36:20 2024, max compression
+gzip compressed data, was "pproject-0.0.4.tar", last modified: Sun May 26 21:21:53 2024, max compression
```

## Comparing `pproject-0.0.3.tar` & `pproject-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-25 16:36:20.714820 pproject-0.0.3/
--rw-r--r--   0 sojirotachibana   (501) staff       (20)      444 2024-05-25 16:36:20.714638 pproject-0.0.3/PKG-INFO
--rw-r--r--   0 sojirotachibana   (501) staff       (20)        8 2024-05-25 16:29:51.000000 pproject-0.0.3/README.md
--rw-r--r--   0 sojirotachibana   (501) staff       (20)       38 2024-05-25 16:36:20.714852 pproject-0.0.3/setup.cfg
--rw-r--r--   0 sojirotachibana   (501) staff       (20)      883 2024-05-25 16:34:20.000000 pproject-0.0.3/setup.py
-drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-25 16:36:20.713761 pproject-0.0.3/src/
-drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-25 16:36:20.714460 pproject-0.0.3/src/pproject.egg-info/
--rw-r--r--   0 sojirotachibana   (501) staff       (20)      444 2024-05-25 16:36:20.000000 pproject-0.0.3/src/pproject.egg-info/PKG-INFO
--rw-r--r--   0 sojirotachibana   (501) staff       (20)      217 2024-05-25 16:36:20.000000 pproject-0.0.3/src/pproject.egg-info/SOURCES.txt
--rw-r--r--   0 sojirotachibana   (501) staff       (20)        1 2024-05-25 16:36:20.000000 pproject-0.0.3/src/pproject.egg-info/dependency_links.txt
--rw-r--r--   0 sojirotachibana   (501) staff       (20)       43 2024-05-25 16:36:20.000000 pproject-0.0.3/src/pproject.egg-info/entry_points.txt
--rw-r--r--   0 sojirotachibana   (501) staff       (20)        9 2024-05-25 16:36:20.000000 pproject-0.0.3/src/pproject.egg-info/top_level.txt
--rw-r--r--   0 sojirotachibana   (501) staff       (20)       29 2024-05-25 15:53:42.000000 pproject-0.0.3/src/pproject.py
+drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-26 21:21:53.080197 pproject-0.0.4/
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)      499 2024-05-26 21:21:53.080004 pproject-0.0.4/PKG-INFO
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)        8 2024-05-25 16:29:51.000000 pproject-0.0.4/README.md
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)       38 2024-05-26 21:21:53.080234 pproject-0.0.4/setup.cfg
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)      928 2024-05-26 21:20:35.000000 pproject-0.0.4/setup.py
+drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-26 21:21:53.078967 pproject-0.0.4/src/
+drwxr-xr-x   0 sojirotachibana   (501) staff       (20)        0 2024-05-26 21:21:53.079805 pproject-0.0.4/src/pproject.egg-info/
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)      499 2024-05-26 21:21:53.000000 pproject-0.0.4/src/pproject.egg-info/PKG-INFO
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)      217 2024-05-26 21:21:53.000000 pproject-0.0.4/src/pproject.egg-info/SOURCES.txt
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)        1 2024-05-26 21:21:53.000000 pproject-0.0.4/src/pproject.egg-info/dependency_links.txt
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)       43 2024-05-26 21:21:53.000000 pproject-0.0.4/src/pproject.egg-info/entry_points.txt
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)        9 2024-05-26 21:21:53.000000 pproject-0.0.4/src/pproject.egg-info/top_level.txt
+-rw-r--r--   0 sojirotachibana   (501) staff       (20)     1774 2024-05-26 21:19:19.000000 pproject-0.0.4/src/pproject.py
```

### Comparing `pproject-0.0.3/setup.py` & `pproject-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 with open("README.md","r",encoding="utf-8")as fh:
     long_description=fh.read()
 setuptools.setup(
     name="pproject",
-    version="0.0.3",
+    version="0.0.4",
     author="Sojiro4",
     author_email="s2122097@stu.musashino-u.ac.jp",
-    description="",
+    description="Predicted price change for iphone in XX years",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Sojiro4/pproject",
     project_urls={
     "Bug Tracker":"https://github.com/Sojiro4/pproject",
     },
     classifiers=[
```

