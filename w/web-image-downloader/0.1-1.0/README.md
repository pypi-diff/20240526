# Comparing `tmp/web_image_downloader-0.1.tar.gz` & `tmp/web_image_downloader-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_image_downloader-0.1.tar", last modified: Sun May 26 17:44:09 2024, max compression
+gzip compressed data, was "web_image_downloader-1.0.tar", last modified: Sun May 26 18:43:28 2024, max compression
```

## Comparing `web_image_downloader-0.1.tar` & `web_image_downloader-1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-26 17:44:09.459096 web_image_downloader-0.1/
--rw-r--r--   0 arif      (1000) arif      (1000)      979 2024-05-26 17:44:09.459096 web_image_downloader-0.1/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)      474 2024-05-26 17:42:19.000000 web_image_downloader-0.1/README.md
--rw-rw-r--   0 arif      (1000) arif      (1000)       38 2024-05-26 17:44:09.459096 web_image_downloader-0.1/setup.cfg
--rw-rw-r--   0 arif      (1000) arif      (1000)      842 2024-05-26 17:43:40.000000 web_image_downloader-0.1/setup.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-26 17:44:09.459096 web_image_downloader-0.1/web_image_downloader/
--rw-rw-r--   0 arif      (1000) arif      (1000)        0 2024-05-26 17:38:52.000000 web_image_downloader-0.1/web_image_downloader/__init__.py
--rw-rw-r--   0 arif      (1000) arif      (1000)      899 2024-05-26 17:40:38.000000 web_image_downloader-0.1/web_image_downloader/downloader.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-26 17:44:09.459096 web_image_downloader-0.1/web_image_downloader.egg-info/
--rw-r--r--   0 arif      (1000) arif      (1000)      979 2024-05-26 17:44:09.000000 web_image_downloader-0.1/web_image_downloader.egg-info/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)      352 2024-05-26 17:44:09.000000 web_image_downloader-0.1/web_image_downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)        1 2024-05-26 17:44:09.000000 web_image_downloader-0.1/web_image_downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       73 2024-05-26 17:44:09.000000 web_image_downloader-0.1/web_image_downloader.egg-info/entry_points.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       22 2024-05-26 17:44:09.000000 web_image_downloader-0.1/web_image_downloader.egg-info/requires.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       21 2024-05-26 17:44:09.000000 web_image_downloader-0.1/web_image_downloader.egg-info/top_level.txt
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-26 18:43:28.499636 web_image_downloader-1.0/
+-rw-r--r--   0 arif      (1000) arif      (1000)     1120 2024-05-26 18:43:28.499636 web_image_downloader-1.0/PKG-INFO
+-rw-rw-r--   0 arif      (1000) arif      (1000)      474 2024-05-26 17:42:19.000000 web_image_downloader-1.0/README.md
+-rw-rw-r--   0 arif      (1000) arif      (1000)       38 2024-05-26 18:43:28.499636 web_image_downloader-1.0/setup.cfg
+-rw-rw-r--   0 arif      (1000) arif      (1000)     1102 2024-05-26 18:43:17.000000 web_image_downloader-1.0/setup.py
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-26 18:43:28.495636 web_image_downloader-1.0/web_image_downloader/
+-rw-rw-r--   0 arif      (1000) arif      (1000)        0 2024-05-26 17:38:52.000000 web_image_downloader-1.0/web_image_downloader/__init__.py
+-rw-rw-r--   0 arif      (1000) arif      (1000)      899 2024-05-26 17:40:38.000000 web_image_downloader-1.0/web_image_downloader/downloader.py
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-26 18:43:28.499636 web_image_downloader-1.0/web_image_downloader.egg-info/
+-rw-r--r--   0 arif      (1000) arif      (1000)     1120 2024-05-26 18:43:28.000000 web_image_downloader-1.0/web_image_downloader.egg-info/PKG-INFO
+-rw-rw-r--   0 arif      (1000) arif      (1000)      352 2024-05-26 18:43:28.000000 web_image_downloader-1.0/web_image_downloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       55 2024-05-26 18:43:28.000000 web_image_downloader-1.0/web_image_downloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       73 2024-05-26 18:43:28.000000 web_image_downloader-1.0/web_image_downloader.egg-info/entry_points.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       22 2024-05-26 18:43:28.000000 web_image_downloader-1.0/web_image_downloader.egg-info/requires.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       21 2024-05-26 18:43:28.000000 web_image_downloader-1.0/web_image_downloader.egg-info/top_level.txt
```

### Comparing `web_image_downloader-0.1/PKG-INFO` & `web_image_downloader-1.0/web_image_downloader.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: web_image_downloader
-Version: 0.1
+Name: web-image-downloader
+Version: 1.0
 Summary: A package to download images from the web using web_assets_downloader.
 Home-page: https://github.com/arif-x/web-image-downloader
 Author: Ariffudin
 Author-email: sudo.ariffudin@gmail.com
+Project-URL: Source, https://github.com/arif-x/web-image-downloader
+Project-URL: Source Code, https://github.com/arif-x/web-image-downloader
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: web-assets-downloader
```

### Comparing `web_image_downloader-0.1/setup.py` & `web_image_downloader-1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='web_image_downloader',
-    version='0.1',
+    version='1.0',
     packages=find_packages(),
     install_requires=[
         'web-assets-downloader'
     ],
     entry_points={
         'console_scripts': [
             'download_images=web_image_downloader.downloader:main'
@@ -20,8 +20,15 @@
     url='https://github.com/arif-x/web-image-downloader',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
+    dependency_links=[
+        'git+https://github.com/arif-x/web-image-downloader.git'
+    ],
+    project_urls={
+        'Source': 'https://github.com/arif-x/web-image-downloader',
+        'Source Code': 'https://github.com/arif-x/web-image-downloader'
+    }
 )
```

### Comparing `web_image_downloader-0.1/web_image_downloader/downloader.py` & `web_image_downloader-1.0/web_image_downloader/downloader.py`

 * *Files identical despite different names*

