# Comparing `tmp/streamlit-islands-0.0.4.tar.gz` & `tmp/streamlit-islands-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-islands-0.0.4.tar", last modified: Sun May 26 12:54:18 2024, max compression
+gzip compressed data, was "streamlit-islands-0.0.5.tar", last modified: Sun May 26 13:00:51 2024, max compression
```

## Comparing `streamlit-islands-0.0.4.tar` & `streamlit-islands-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:54:18.144353 streamlit-islands-0.0.4/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     1067 2024-03-04 22:49:07.000000 streamlit-islands-0.0.4/LICENSE.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-26 12:54:18.144353 streamlit-islands-0.0.4/PKG-INFO
--rw-r--r--   0 anasb     (1000) anasb     (1000)      634 2024-05-26 12:09:33.000000 streamlit-islands-0.0.4/README.md
--rw-r--r--   0 anasb     (1000) anasb     (1000)       38 2024-05-26 12:54:18.144353 streamlit-islands-0.0.4/setup.cfg
--rw-r--r--   0 anasb     (1000) anasb     (1000)      845 2024-05-26 12:54:13.000000 streamlit-islands-0.0.4/setup.py
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:54:18.144353 streamlit-islands-0.0.4/streamlit_islands/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     4591 2024-05-26 12:48:43.000000 streamlit-islands-0.0.4/streamlit_islands/__init__.py
--rw-r--r--   0 anasb     (1000) anasb     (1000)      325 2024-05-26 12:30:40.000000 streamlit-islands-0.0.4/streamlit_islands/demo.py
--rw-r--r--   0 anasb     (1000) anasb     (1000)        0 2024-05-25 05:53:34.000000 streamlit-islands-0.0.4/streamlit_islands/test.py
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:54:18.144353 streamlit-islands-0.0.4/streamlit_islands.egg-info/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-26 12:54:17.000000 streamlit-islands-0.0.4/streamlit_islands.egg-info/PKG-INFO
--rw-r--r--   0 anasb     (1000) anasb     (1000)      329 2024-05-26 12:54:18.000000 streamlit-islands-0.0.4/streamlit_islands.egg-info/SOURCES.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)        1 2024-05-26 12:54:17.000000 streamlit-islands-0.0.4/streamlit_islands.egg-info/dependency_links.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-05-26 12:54:18.000000 streamlit-islands-0.0.4/streamlit_islands.egg-info/requires.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)       18 2024-05-26 12:54:18.000000 streamlit-islands-0.0.4/streamlit_islands.egg-info/top_level.txt
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:54:18.144353 streamlit-islands-0.0.4/test/
--rw-r--r--   0 anasb     (1000) anasb     (1000)      441 2024-05-26 12:52:00.000000 streamlit-islands-0.0.4/test/test.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 13:00:50.994314 streamlit-islands-0.0.5/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     1067 2024-03-04 22:49:07.000000 streamlit-islands-0.0.5/LICENSE.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      979 2024-05-26 13:00:50.994314 streamlit-islands-0.0.5/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      634 2024-05-26 12:09:33.000000 streamlit-islands-0.0.5/README.md
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       38 2024-05-26 13:00:50.994314 streamlit-islands-0.0.5/setup.cfg
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      845 2024-05-26 13:00:39.000000 streamlit-islands-0.0.5/setup.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 13:00:50.994314 streamlit-islands-0.0.5/streamlit_islands/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     4591 2024-05-26 12:48:43.000000 streamlit-islands-0.0.5/streamlit_islands/__init__.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      325 2024-05-26 12:30:40.000000 streamlit-islands-0.0.5/streamlit_islands/demo.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)        0 2024-05-25 05:53:34.000000 streamlit-islands-0.0.5/streamlit_islands/test.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 13:00:50.994314 streamlit-islands-0.0.5/streamlit_islands.egg-info/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      979 2024-05-26 13:00:50.000000 streamlit-islands-0.0.5/streamlit_islands.egg-info/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      329 2024-05-26 13:00:50.000000 streamlit-islands-0.0.5/streamlit_islands.egg-info/SOURCES.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)        1 2024-05-26 13:00:50.000000 streamlit-islands-0.0.5/streamlit_islands.egg-info/dependency_links.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-05-26 13:00:50.000000 streamlit-islands-0.0.5/streamlit_islands.egg-info/requires.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       18 2024-05-26 13:00:50.000000 streamlit-islands-0.0.5/streamlit_islands.egg-info/top_level.txt
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 13:00:50.994314 streamlit-islands-0.0.5/test/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      441 2024-05-26 12:52:00.000000 streamlit-islands-0.0.5/test/test.py
```

### Comparing `streamlit-islands-0.0.4/LICENSE.txt` & `streamlit-islands-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-islands-0.0.4/README.md` & `streamlit-islands-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-islands-0.0.4/setup.py` & `streamlit-islands-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "PROJECT.md").read_text()
 
 setup(
     name='streamlit-islands',
-    version='0.0.4',
+    version='0.0.5',
     author='Anas Bouzid',
     author_email='anasbouzid@gmail.com',
     description='Separate static content from dynamic content in Streamlit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/bouzidanas/streamlit-islands",
     packages=find_packages(),
```

### Comparing `streamlit-islands-0.0.4/streamlit_islands/__init__.py` & `streamlit-islands-0.0.5/streamlit_islands/__init__.py`

 * *Files identical despite different names*

