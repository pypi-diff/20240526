# Comparing `tmp/readme-ation-0.1.2.tar.gz` & `tmp/readme_ation-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme-ation-0.1.2.tar", last modified: Sat May 25 21:48:09 2024, max compression
+gzip compressed data, was "readme_ation-0.1.4.tar", last modified: Sun May 26 05:37:27 2024, max compression
```

## Comparing `readme-ation-0.1.2.tar` & `readme_ation-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-25 21:48:09.048075 readme-ation-0.1.2/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 readme-ation-0.1.2/LICENSE
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      428 2024-05-25 21:48:09.047358 readme-ation-0.1.2/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       27 2024-05-25 07:22:55.000000 readme-ation-0.1.2/README.md
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 readme-ation-0.1.2/pyproject.toml
-drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-25 21:48:09.046457 readme-ation-0.1.2/readme_ation.egg-info/
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      428 2024-05-25 21:48:08.000000 readme-ation-0.1.2/readme_ation.egg-info/PKG-INFO
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      197 2024-05-25 21:48:09.000000 readme-ation-0.1.2/readme_ation.egg-info/SOURCES.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-05-25 21:48:08.000000 readme-ation-0.1.2/readme_ation.egg-info/dependency_links.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)        9 2024-05-25 21:48:08.000000 readme-ation-0.1.2/readme_ation.egg-info/top_level.txt
--rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-05-25 21:48:09.048270 readme-ation-0.1.2/setup.cfg
--rw-r--r--   0 charlesfeinn   (501) staff       (20)      865 2024-05-25 19:35:43.000000 readme-ation-0.1.2/setup.py
--rw-r--r--   0 charlesfeinn   (501) staff       (20)     4473 2024-05-25 08:21:41.000000 readme-ation-0.1.2/versions.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-26 05:37:27.512570 readme_ation-0.1.4/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     1070 2024-05-25 07:57:26.000000 readme_ation-0.1.4/LICENSE
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      428 2024-05-26 05:37:27.511946 readme_ation-0.1.4/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       27 2024-05-25 07:22:55.000000 readme_ation-0.1.4/README.md
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       94 2024-05-25 08:00:42.000000 readme_ation-0.1.4/pyproject.toml
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-26 05:37:27.509463 readme_ation-0.1.4/readme_ation/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        0 2024-05-26 05:19:56.000000 readme_ation-0.1.4/readme_ation/__init__.py
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)     4473 2024-05-25 08:21:41.000000 readme_ation-0.1.4/readme_ation/versions.py
+drwxr-xr-x   0 charlesfeinn   (501) staff       (20)        0 2024-05-26 05:37:27.511330 readme_ation-0.1.4/readme_ation.egg-info/
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      428 2024-05-26 05:37:27.000000 readme_ation-0.1.4/readme_ation.egg-info/PKG-INFO
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      235 2024-05-26 05:37:27.000000 readme_ation-0.1.4/readme_ation.egg-info/SOURCES.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)        1 2024-05-26 05:37:27.000000 readme_ation-0.1.4/readme_ation.egg-info/dependency_links.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       13 2024-05-26 05:37:27.000000 readme_ation-0.1.4/readme_ation.egg-info/top_level.txt
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)       38 2024-05-26 05:37:27.512873 readme_ation-0.1.4/setup.cfg
+-rw-r--r--   0 charlesfeinn   (501) staff       (20)      900 2024-05-26 05:34:48.000000 readme_ation-0.1.4/setup.py
```

### Comparing `readme-ation-0.1.2/LICENSE` & `readme_ation-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `readme-ation-0.1.2/setup.py` & `readme_ation-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="readme-ation",
-    version="0.1.2",
-    # packages=find_packages(),
-    py_modules=['versions'],
+    version="0.1.4",
+    packages=['readme_ation'],
+    # py_modules=['versions'],
     install_requires=[
         # List dependencies here, e.g. 'requests>=2.25.1'
     ],
     entry_points={
         # 'console_scripts': [
         #     'main = main:log_versions_to_readme_on_successful_exit',  # Assuming you have a main function in my_script.py
         # ],
     },
     author='Charles Feinn',
+    email='chuckfinca@gmail.com',
     description='A README.md generation tool',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/your-repo',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

### Comparing `readme-ation-0.1.2/versions.py` & `readme_ation-0.1.4/readme_ation/versions.py`

 * *Files identical despite different names*

