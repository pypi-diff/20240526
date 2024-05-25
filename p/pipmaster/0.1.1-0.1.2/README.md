# Comparing `tmp/pipmaster-0.1.1.tar.gz` & `tmp/pipmaster-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipmaster-0.1.1.tar", last modified: Sun Apr 14 20:31:31 2024, max compression
+gzip compressed data, was "pipmaster-0.1.2.tar", last modified: Sat May 25 22:02:06 2024, max compression
```

## Comparing `pipmaster-0.1.1.tar` & `pipmaster-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 20:31:31.391986 pipmaster-0.1.1/
--rw-rw-rw-   0        0        0    11558 2024-04-14 11:47:19.000000 pipmaster-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2452 2024-04-14 20:31:31.390988 pipmaster-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1590 2024-04-14 20:31:10.000000 pipmaster-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 20:31:31.373975 pipmaster-0.1.1/pipmaster/
--rw-rw-rw-   0        0        0     1941 2024-04-14 12:02:07.000000 pipmaster-0.1.1/pipmaster/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 20:31:31.390988 pipmaster-0.1.1/pipmaster.egg-info/
--rw-rw-rw-   0        0        0     2452 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-14 20:31:31.000000 pipmaster-0.1.1/pipmaster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 20:31:31.392986 pipmaster-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1201 2024-04-14 20:31:25.000000 pipmaster-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:02:06.670513 pipmaster-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 20:19:07.000000 pipmaster-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6112 2024-05-25 22:02:06.669511 pipmaster-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5250 2024-05-25 20:34:54.000000 pipmaster-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 22:02:06.640772 pipmaster-0.1.2/pipmaster/
+-rw-rw-rw-   0        0        0     8065 2024-05-25 20:24:48.000000 pipmaster-0.1.2/pipmaster/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:02:06.668511 pipmaster-0.1.2/pipmaster.egg-info/
+-rw-rw-rw-   0        0        0     6112 2024-05-25 22:02:06.000000 pipmaster-0.1.2/pipmaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-25 22:02:06.000000 pipmaster-0.1.2/pipmaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 22:02:06.000000 pipmaster-0.1.2/pipmaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-25 22:02:06.000000 pipmaster-0.1.2/pipmaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 22:02:06.000000 pipmaster-0.1.2/pipmaster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 22:02:06.670513 pipmaster-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2024-05-25 20:19:37.000000 pipmaster-0.1.2/setup.py
```

### Comparing `pipmaster-0.1.1/LICENSE` & `pipmaster-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipmaster-0.1.1/setup.py` & `pipmaster-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().splitlines()
 
 setup(
     name="pipmaster",
-    version="0.1.1",
+    version="0.1.2",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A simple and versatile Python package manager for automating installation and verification across platforms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/pymanage",
     packages=find_packages(),
```

