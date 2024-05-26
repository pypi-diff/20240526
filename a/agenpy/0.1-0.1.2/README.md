# Comparing `tmp/agenpy-0.1.tar.gz` & `tmp/agenpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agenpy-0.1.tar", last modified: Sun Apr 28 15:38:52 2024, max compression
+gzip compressed data, was "agenpy-0.1.2.tar", last modified: Sun May 26 18:33:24 2024, max compression
```

## Comparing `agenpy-0.1.tar` & `agenpy-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 15:38:52.622040 agenpy-0.1/
--rw-rw-rw-   0        0        0    11556 2024-04-28 15:27:41.000000 agenpy-0.1/LICENSE
--rw-rw-rw-   0        0        0      492 2024-04-28 15:38:52.618043 agenpy-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      166 2024-04-28 15:27:00.000000 agenpy-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 15:38:52.579412 agenpy-0.1/agenpy/
--rw-rw-rw-   0        0        0        0 2024-04-28 15:29:48.000000 agenpy-0.1/agenpy/agenpy.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:38:52.615044 agenpy-0.1/agenpy.egg-info/
--rw-rw-rw-   0        0        0      492 2024-04-28 15:38:52.000000 agenpy-0.1/agenpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2024-04-28 15:38:52.000000 agenpy-0.1/agenpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 15:38:52.000000 agenpy-0.1/agenpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 15:38:52.000000 agenpy-0.1/agenpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 15:38:52.622040 agenpy-0.1/setup.cfg
--rw-rw-rw-   0        0        0      562 2024-04-28 15:34:46.000000 agenpy-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:33:24.645161 agenpy-0.1.2/
+-rw-rw-rw-   0        0        0    11556 2024-04-28 15:27:41.000000 agenpy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3541 2024-05-26 18:33:24.644161 agenpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3112 2024-05-26 18:30:00.000000 agenpy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 18:33:24.642162 agenpy-0.1.2/agenpy.egg-info/
+-rw-rw-rw-   0        0        0     3541 2024-05-26 18:33:24.000000 agenpy-0.1.2/agenpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2024-05-26 18:33:24.000000 agenpy-0.1.2/agenpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:33:24.000000 agenpy-0.1.2/agenpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-26 18:33:24.000000 agenpy-0.1.2/agenpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:33:24.000000 agenpy-0.1.2/agenpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 18:33:24.646160 agenpy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-05-26 18:33:17.000000 agenpy-0.1.2/setup.py
```

### Comparing `agenpy-0.1/LICENSE` & `agenpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agenpy-0.1/setup.py` & `agenpy-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setup(
    name='agenpy',
-   version='0.1',
+   version='0.1.2',
    description='A python package for setting up agentic behavior for LLMs. Includes optimization for large training data, and adherence to applied interactional policies.',
    license="Apache-2.0",
    long_description=long_description,
+   long_description_content_type='text/markdown',
    author='Octran Technologies',
    author_email='contact@octran.tech',
-   packages=['agenpy'],  #same as name
-   install_requires=[], #external packages as dependencies
+   packages=find_packages(), #same as name
+   install_requires=["openai>=1.30"], #external packages as dependencies
+   python_requires=">=3.8",
 )
```

