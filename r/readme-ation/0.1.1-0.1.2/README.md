# Comparing `tmp/readme_ation-0.1.1.tar.gz` & `tmp/readme-ation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_ation-0.1.1.tar", last modified: Sat May 25 08:50:09 2024, max compression
+gzip compressed data, was "readme-ation-0.1.2.tar", last modified: Sat May 25 21:48:09 2024, max compression
```

## Comparing `readme_ation-0.1.1.tar` & `readme-ation-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-25 08:50:09.943984 readme_ation-0.1.1/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 readme_ation-0.1.1/LICENSE
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      428 2024-05-25 08:50:09.943404 readme_ation-0.1.1/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       27 2024-05-25 07:22:55.000000 readme_ation-0.1.1/README.md
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     4473 2024-05-25 08:21:41.000000 readme_ation-0.1.1/main.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 readme_ation-0.1.1/pyproject.toml
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-25 08:50:09.942830 readme_ation-0.1.1/readme_ation.egg-info/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      428 2024-05-25 08:50:09.000000 readme_ation-0.1.1/readme_ation.egg-info/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      193 2024-05-25 08:50:09.000000 readme_ation-0.1.1/readme_ation.egg-info/SOURCES.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-05-25 08:50:09.000000 readme_ation-0.1.1/readme_ation.egg-info/dependency_links.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        5 2024-05-25 08:50:09.000000 readme_ation-0.1.1/readme_ation.egg-info/top_level.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-05-25 08:50:09.944109 readme_ation-0.1.1/setup.cfg
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      833 2024-05-25 08:49:00.000000 readme_ation-0.1.1/setup.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-25 21:48:09.048075 readme-ation-0.1.2/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 readme-ation-0.1.2/LICENSE
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      428 2024-05-25 21:48:09.047358 readme-ation-0.1.2/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       27 2024-05-25 07:22:55.000000 readme-ation-0.1.2/README.md
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 readme-ation-0.1.2/pyproject.toml
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-25 21:48:09.046457 readme-ation-0.1.2/readme_ation.egg-info/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      428 2024-05-25 21:48:08.000000 readme-ation-0.1.2/readme_ation.egg-info/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      197 2024-05-25 21:48:09.000000 readme-ation-0.1.2/readme_ation.egg-info/SOURCES.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-05-25 21:48:08.000000 readme-ation-0.1.2/readme_ation.egg-info/dependency_links.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        9 2024-05-25 21:48:08.000000 readme-ation-0.1.2/readme_ation.egg-info/top_level.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-05-25 21:48:09.048270 readme-ation-0.1.2/setup.cfg
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      865 2024-05-25 19:35:43.000000 readme-ation-0.1.2/setup.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     4473 2024-05-25 08:21:41.000000 readme-ation-0.1.2/versions.py
```

### Comparing `readme_ation-0.1.1/LICENSE` & `readme-ation-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `readme_ation-0.1.1/main.py` & `readme-ation-0.1.2/versions.py`

 * *Files identical despite different names*

### Comparing `readme_ation-0.1.1/setup.py` & `readme-ation-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="readme-ation",
-    version="0.1.1",
-        py_modules=['main'],
+    version="0.1.2",
+    # packages=find_packages(),
+    py_modules=['versions'],
     install_requires=[
         # List dependencies here, e.g. 'requests>=2.25.1'
     ],
     entry_points={
         # 'console_scripts': [
         #     'main = main:log_versions_to_readme_on_successful_exit',  # Assuming you have a main function in my_script.py
         # ],
```

