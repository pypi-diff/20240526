# Comparing `tmp/streamlit-islands-0.0.2.tar.gz` & `tmp/streamlit-islands-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-islands-0.0.2.tar", last modified: Sun May 26 12:32:32 2024, max compression
+gzip compressed data, was "streamlit-islands-0.0.3.tar", last modified: Sun May 26 12:44:44 2024, max compression
```

## Comparing `streamlit-islands-0.0.2.tar` & `streamlit-islands-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     1067 2024-03-04 22:49:07.000000 streamlit-islands-0.0.2/LICENSE.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/PKG-INFO
--rw-r--r--   0 anasb     (1000) anasb     (1000)      634 2024-05-26 12:09:33.000000 streamlit-islands-0.0.2/README.md
--rw-r--r--   0 anasb     (1000) anasb     (1000)       38 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/setup.cfg
--rw-r--r--   0 anasb     (1000) anasb     (1000)      845 2024-05-26 12:31:46.000000 streamlit-islands-0.0.2/setup.py
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/streamlit_islands/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     4453 2024-05-26 12:27:57.000000 streamlit-islands-0.0.2/streamlit_islands/__init__.py
--rw-r--r--   0 anasb     (1000) anasb     (1000)      325 2024-05-26 12:30:40.000000 streamlit-islands-0.0.2/streamlit_islands/demo.py
--rw-r--r--   0 anasb     (1000) anasb     (1000)        0 2024-05-25 05:53:34.000000 streamlit-islands-0.0.2/streamlit_islands/test.py
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/streamlit_islands.egg-info/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-26 12:32:31.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/PKG-INFO
--rw-r--r--   0 anasb     (1000) anasb     (1000)      316 2024-05-26 12:32:32.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/SOURCES.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)        1 2024-05-26 12:32:31.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/dependency_links.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-05-26 12:32:32.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/requires.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)       18 2024-05-26 12:32:32.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/top_level.txt
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:44:44.274410 streamlit-islands-0.0.3/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     1067 2024-03-04 22:49:07.000000 streamlit-islands-0.0.3/LICENSE.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-26 12:44:44.274410 streamlit-islands-0.0.3/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      634 2024-05-26 12:09:33.000000 streamlit-islands-0.0.3/README.md
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       38 2024-05-26 12:44:44.274410 streamlit-islands-0.0.3/setup.cfg
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      845 2024-05-26 12:44:41.000000 streamlit-islands-0.0.3/setup.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:44:44.274410 streamlit-islands-0.0.3/streamlit_islands/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     4589 2024-05-26 12:43:59.000000 streamlit-islands-0.0.3/streamlit_islands/__init__.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      325 2024-05-26 12:30:40.000000 streamlit-islands-0.0.3/streamlit_islands/demo.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)        0 2024-05-25 05:53:34.000000 streamlit-islands-0.0.3/streamlit_islands/test.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:44:44.274410 streamlit-islands-0.0.3/streamlit_islands.egg-info/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-26 12:44:43.000000 streamlit-islands-0.0.3/streamlit_islands.egg-info/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      329 2024-05-26 12:44:44.000000 streamlit-islands-0.0.3/streamlit_islands.egg-info/SOURCES.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)        1 2024-05-26 12:44:43.000000 streamlit-islands-0.0.3/streamlit_islands.egg-info/dependency_links.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-05-26 12:44:44.000000 streamlit-islands-0.0.3/streamlit_islands.egg-info/requires.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       18 2024-05-26 12:44:44.000000 streamlit-islands-0.0.3/streamlit_islands.egg-info/top_level.txt
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:44:44.274410 streamlit-islands-0.0.3/test/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      353 2024-05-26 12:36:51.000000 streamlit-islands-0.0.3/test/test.py
```

### Comparing `streamlit-islands-0.0.2/LICENSE.txt` & `streamlit-islands-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-islands-0.0.2/PKG-INFO` & `streamlit-islands-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-islands
-Version: 0.0.2
+Version: 0.0.3
 Summary: Separate static content from dynamic content in Streamlit
 Home-page: https://github.com/bouzidanas/streamlit-islands
 Author: Anas Bouzid
 Author-email: anasbouzid@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `streamlit-islands-0.0.2/README.md` & `streamlit-islands-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-islands-0.0.2/setup.py` & `streamlit-islands-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "PROJECT.md").read_text()
 
 setup(
     name='streamlit-islands',
-    version='0.0.2',
+    version='0.0.3',
     author='Anas Bouzid',
     author_email='anasbouzid@gmail.com',
     description='Separate static content from dynamic content in Streamlit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/bouzidanas/streamlit-islands",
     packages=find_packages(),
```

### Comparing `streamlit-islands-0.0.2/streamlit_islands/__init__.py` & `streamlit-islands-0.0.3/streamlit_islands/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import streamlit as st
 import streamlit.components.v1 as components
 import os.path
 import inspect
 from ast import literal_eval
 
 def load_md(markdown_file_name):
-    # if file name starts with the result of os.path.join("..", ""), then the path is relative to the parent directory
-    parent_dir_prefix = os.path.join("..", "")
-    current_dir_prefix = os.path.join(".", "")
-    directory_symbol = os.path.join(" ", " ").strip()
-    if markdown_file_name.startswith(parent_dir_prefix):
-        markdown_file = os.path.join(os.path.split(os.path.dirname(__file__))[0], markdown_file_name.replace(parent_dir_prefix, ""))
-    elif markdown_file_name.startswith(current_dir_prefix) or directory_symbol not in markdown_file_name:
-        markdown_file = os.path.join(os.path.dirname(__file__), markdown_file_name.replace(current_dir_prefix, ""))
-    else:
-        markdown_file = markdown_file_name
+    # # if file name starts with the result of os.path.join("..", ""), then the path is relative to the parent directory
+    # parent_dir_prefix = os.path.join("..", "")
+    # current_dir_prefix = os.path.join(".", "")
+    # directory_symbol = os.path.join(" ", " ").strip()
+    # if markdown_file_name.startswith(parent_dir_prefix):
+    #     markdown_file = os.path.join(os.path.split(os.path.dirname(__file__))[0], markdown_file_name.replace(parent_dir_prefix, ""))
+    # elif markdown_file_name.startswith(current_dir_prefix) or directory_symbol not in markdown_file_name:
+    #     markdown_file = os.path.join(os.path.dirname(__file__), markdown_file_name.replace(current_dir_prefix, ""))
+    # else:
+    #     markdown_file = markdown_file_name
+
+    # Until I can get the code above to work, I will use the following code
+    markdown_file = markdown_file_name
 
     with open(markdown_file, "r") as f:
         md = f.read()
     return process_md(md)
 
 def process_md(md):
     # Split the markdown into static and dynamic content
```

### Comparing `streamlit-islands-0.0.2/streamlit_islands.egg-info/PKG-INFO` & `streamlit-islands-0.0.3/streamlit_islands.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-islands
-Version: 0.0.2
+Version: 0.0.3
 Summary: Separate static content from dynamic content in Streamlit
 Home-page: https://github.com/bouzidanas/streamlit-islands
 Author: Anas Bouzid
 Author-email: anasbouzid@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

