# Comparing `tmp/crx_utils-1.0.0.tar.gz` & `tmp/crx_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crx_utils-1.0.0.tar", last modified: Sun May 26 10:36:46 2024, max compression
+gzip compressed data, was "crx_utils-1.1.0.tar", last modified: Sun May 26 10:49:06 2024, max compression
```

## Comparing `crx_utils-1.0.0.tar` & `crx_utils-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 10:36:46.258062 crx_utils-1.0.0/
--rw-rw-rw-   0        0        0       85 2024-05-26 10:32:30.000000 crx_utils-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      419 2024-05-26 10:36:46.257063 crx_utils-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 10:36:46.243062 crx_utils-1.0.0/crx/
--rw-rw-rw-   0        0        0      783 2024-05-26 00:13:51.000000 crx_utils-1.0.0/crx/Cogs.py
--rw-rw-rw-   0        0        0     1356 2024-05-26 00:54:31.000000 crx_utils-1.0.0/crx/Embed.py
--rw-rw-rw-   0        0        0     1154 2024-05-26 00:55:36.000000 crx_utils-1.0.0/crx/Loguru.py
--rw-rw-rw-   0        0        0     1507 2024-05-26 09:43:03.000000 crx_utils-1.0.0/crx/Reader.py
--rw-rw-rw-   0        0        0      754 2024-05-26 00:55:46.000000 crx_utils-1.0.0/crx/Tortoise.py
--rw-rw-rw-   0        0        0      238 2024-05-26 00:55:12.000000 crx_utils-1.0.0/crx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:36:46.257063 crx_utils-1.0.0/crx_utils.egg-info/
--rw-rw-rw-   0        0        0      419 2024-05-26 10:36:46.000000 crx_utils-1.0.0/crx_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-05-26 10:36:46.000000 crx_utils-1.0.0/crx_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 10:36:46.000000 crx_utils-1.0.0/crx_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2024-05-26 10:36:46.000000 crx_utils-1.0.0/crx_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-26 10:36:46.000000 crx_utils-1.0.0/crx_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      109 2024-05-26 10:36:41.000000 crx_utils-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-26 10:36:46.258062 crx_utils-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      568 2024-05-26 10:27:24.000000 crx_utils-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:49:06.470324 crx_utils-1.1.0/
+-rw-rw-rw-   0        0        0       85 2024-05-26 10:32:30.000000 crx_utils-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      419 2024-05-26 10:49:06.469325 crx_utils-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 10:49:06.456325 crx_utils-1.1.0/crx/
+-rw-rw-rw-   0        0        0      783 2024-05-26 00:13:51.000000 crx_utils-1.1.0/crx/Cogs.py
+-rw-rw-rw-   0        0        0     1356 2024-05-26 00:54:31.000000 crx_utils-1.1.0/crx/Embed.py
+-rw-rw-rw-   0        0        0     1154 2024-05-26 00:55:36.000000 crx_utils-1.1.0/crx/Loguru.py
+-rw-rw-rw-   0        0        0     1507 2024-05-26 09:43:03.000000 crx_utils-1.1.0/crx/Reader.py
+-rw-rw-rw-   0        0        0      754 2024-05-26 00:55:46.000000 crx_utils-1.1.0/crx/Tortoise.py
+-rw-rw-rw-   0        0        0      238 2024-05-26 00:55:12.000000 crx_utils-1.1.0/crx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:49:06.469325 crx_utils-1.1.0/crx_utils.egg-info/
+-rw-rw-rw-   0        0        0      419 2024-05-26 10:49:06.000000 crx_utils-1.1.0/crx_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-26 10:49:06.000000 crx_utils-1.1.0/crx_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:49:06.000000 crx_utils-1.1.0/crx_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-05-26 10:49:06.000000 crx_utils-1.1.0/crx_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-26 10:49:06.000000 crx_utils-1.1.0/crx_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      109 2024-05-26 10:36:41.000000 crx_utils-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:49:06.470324 crx_utils-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      560 2024-05-26 10:47:22.000000 crx_utils-1.1.0/setup.py
```

### Comparing `crx_utils-1.0.0/crx/Cogs.py` & `crx_utils-1.1.0/crx/Cogs.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.0.0/crx/Embed.py` & `crx_utils-1.1.0/crx/Embed.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.0.0/crx/Loguru.py` & `crx_utils-1.1.0/crx/Loguru.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.0.0/crx/Reader.py` & `crx_utils-1.1.0/crx/Reader.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.0.0/crx/Tortoise.py` & `crx_utils-1.1.0/crx/Tortoise.py`

 * *Files identical despite different names*

### Comparing `crx_utils-1.0.0/setup.py` & `crx_utils-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="crx-utils",
-    version="1.0.0",
+    version="1.1.0",
     description="A collection of functions for creating Discord bots, works with nextcord.",
     url="https://discord.gg/EEp67FWQDP",
     author="CRX-DEV",
     author_email="cherniq66@gmail.com",
     license="MIT License",
-    
-
     packages=find_packages(include=['crx', 'crx.*']),
     install_requires=[
         "tortoise-orm==0.21.0",
         "nextcord==2.6.0",
         "aiofiles==23.2.1",
         "fastenv==0.5.0",
         "loguru==0.7.2",
```

