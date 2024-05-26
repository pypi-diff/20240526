# Comparing `tmp/streamlit-islands-0.0.1.tar.gz` & `tmp/streamlit-islands-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-islands-0.0.1.tar", last modified: Sat May 25 08:53:27 2024, max compression
+gzip compressed data, was "streamlit-islands-0.0.2.tar", last modified: Sun May 26 12:32:32 2024, max compression
```

## Comparing `streamlit-islands-0.0.1.tar` & `streamlit-islands-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-25 08:53:27.434384 streamlit-islands-0.0.1/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     1067 2024-03-04 22:49:07.000000 streamlit-islands-0.0.1/LICENSE.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-25 08:53:27.434384 streamlit-islands-0.0.1/PKG-INFO
--rw-r--r--   0 anasb     (1000) anasb     (1000)      782 2024-05-25 07:35:48.000000 streamlit-islands-0.0.1/README.md
--rw-r--r--   0 anasb     (1000) anasb     (1000)       38 2024-05-25 08:53:27.434384 streamlit-islands-0.0.1/setup.cfg
--rw-r--r--   0 anasb     (1000) anasb     (1000)      845 2024-05-25 05:51:53.000000 streamlit-islands-0.0.1/setup.py
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-25 08:53:27.434384 streamlit-islands-0.0.1/streamlit_islands/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     2719 2024-05-25 07:38:00.000000 streamlit-islands-0.0.1/streamlit_islands/__init__.py
--rw-r--r--   0 anasb     (1000) anasb     (1000)    11875 2024-03-04 22:49:07.000000 streamlit-islands-0.0.1/streamlit_islands/demo.py
--rw-r--r--   0 anasb     (1000) anasb     (1000)        0 2024-05-25 05:53:34.000000 streamlit-islands-0.0.1/streamlit_islands/test.py
-drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-25 08:53:27.434384 streamlit-islands-0.0.1/streamlit_islands.egg-info/
--rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-25 08:53:27.000000 streamlit-islands-0.0.1/streamlit_islands.egg-info/PKG-INFO
--rw-r--r--   0 anasb     (1000) anasb     (1000)      316 2024-05-25 08:53:27.000000 streamlit-islands-0.0.1/streamlit_islands.egg-info/SOURCES.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)        1 2024-05-25 08:53:27.000000 streamlit-islands-0.0.1/streamlit_islands.egg-info/dependency_links.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-05-25 08:53:27.000000 streamlit-islands-0.0.1/streamlit_islands.egg-info/requires.txt
--rw-r--r--   0 anasb     (1000) anasb     (1000)       18 2024-05-25 08:53:27.000000 streamlit-islands-0.0.1/streamlit_islands.egg-info/top_level.txt
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     1067 2024-03-04 22:49:07.000000 streamlit-islands-0.0.2/LICENSE.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      634 2024-05-26 12:09:33.000000 streamlit-islands-0.0.2/README.md
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       38 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/setup.cfg
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      845 2024-05-26 12:31:46.000000 streamlit-islands-0.0.2/setup.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/streamlit_islands/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     4453 2024-05-26 12:27:57.000000 streamlit-islands-0.0.2/streamlit_islands/__init__.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      325 2024-05-26 12:30:40.000000 streamlit-islands-0.0.2/streamlit_islands/demo.py
+-rw-r--r--   0 anasb     (1000) anasb     (1000)        0 2024-05-25 05:53:34.000000 streamlit-islands-0.0.2/streamlit_islands/test.py
+drwxr-xr-x   0 anasb     (1000) anasb     (1000)        0 2024-05-26 12:32:32.184482 streamlit-islands-0.0.2/streamlit_islands.egg-info/
+-rw-r--r--   0 anasb     (1000) anasb     (1000)     2326 2024-05-26 12:32:31.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/PKG-INFO
+-rw-r--r--   0 anasb     (1000) anasb     (1000)      316 2024-05-26 12:32:32.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/SOURCES.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)        1 2024-05-26 12:32:31.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/dependency_links.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       16 2024-05-26 12:32:32.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/requires.txt
+-rw-r--r--   0 anasb     (1000) anasb     (1000)       18 2024-05-26 12:32:32.000000 streamlit-islands-0.0.2/streamlit_islands.egg-info/top_level.txt
```

### Comparing `streamlit-islands-0.0.1/LICENSE.txt` & `streamlit-islands-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-islands-0.0.1/PKG-INFO` & `streamlit-islands-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-islands
-Version: 0.0.1
+Version: 0.0.2
 Summary: Separate static content from dynamic content in Streamlit
 Home-page: https://github.com/bouzidanas/streamlit-islands
 Author: Anas Bouzid
 Author-email: anasbouzid@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `streamlit-islands-0.0.1/README.md` & `streamlit-islands-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 streamlit-islands  [![Version](https://img.shields.io/pypi/v/streamlit-islands)](https://pypi.org/project/streamlit-islands/#history) 
 [![PyPi - Downloads](https://img.shields.io/pypi/dm/streamlit-islands)](https://pypi.org/project/streamlit-islands/#files)[![Component Demo](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://islands-demo.streamlit.app/)
 ============
 
-Fix the vertical position of Streamlit containers relative to viewport instead of page
-
 ## Installation
 Install [streamlit-islands](https://pypi.org/project/streamlit-islands/) with pip:
 ```bash
 pip install streamlit-islands
 ```
 
-## Usage
-
 ## License
 This project is licensed under the [MIT License](LICENSE.txt)
 
-[hello]: # (arg 1, {
-    arg: "sell",
-    arg_alt: "buy"}, {arg 3}
-    )
+[say_hello]: # ("bob")
```

### Comparing `streamlit-islands-0.0.1/setup.py` & `streamlit-islands-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "PROJECT.md").read_text()
 
 setup(
     name='streamlit-islands',
-    version='0.0.1',
+    version='0.0.2',
     author='Anas Bouzid',
     author_email='anasbouzid@gmail.com',
     description='Separate static content from dynamic content in Streamlit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/bouzidanas/streamlit-islands",
     packages=find_packages(),
```

### Comparing `streamlit-islands-0.0.1/streamlit_islands/__init__.py` & `streamlit-islands-0.0.2/streamlit_islands/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,97 @@
 import streamlit as st
 import streamlit.components.v1 as components
 import os.path
+import inspect
+from ast import literal_eval
 
-def load_md(markdown_file_name, **kwargs):
+def load_md(markdown_file_name):
     # if file name starts with the result of os.path.join("..", ""), then the path is relative to the parent directory
     parent_dir_prefix = os.path.join("..", "")
     current_dir_prefix = os.path.join(".", "")
     directory_symbol = os.path.join(" ", " ").strip()
     if markdown_file_name.startswith(parent_dir_prefix):
         markdown_file = os.path.join(os.path.split(os.path.dirname(__file__))[0], markdown_file_name.replace(parent_dir_prefix, ""))
     elif markdown_file_name.startswith(current_dir_prefix) or directory_symbol not in markdown_file_name:
         markdown_file = os.path.join(os.path.dirname(__file__), markdown_file_name.replace(current_dir_prefix, ""))
     else:
         markdown_file = markdown_file_name
 
-    st.write(markdown_file)
     with open(markdown_file, "r") as f:
         md = f.read()
-    return process_md(md, **kwargs)
+    return process_md(md)
 
-def process_md(md, **kwargs):
+def process_md(md):
     # Split the markdown into static and dynamic content
     # The dynamic content will be substituted in place of text
     # having the following format: \n[name]: # (list of arguments)\n
     # where 'name' is the name of a function that will generate the dynamic content
     # and the 'list of arguments' is a list of arguments that will be passed to this function
     static_content = []
     dynamic_content = []
     temp_content = []
     temp_call_name = ""
     temp_call_args = ""
     in_dynamic_content = False
+
     for line in md.split("\n"):
         if not in_dynamic_content and line.strip().startswith("[") and "]: # (" in line:
             temp_call_name = line.split("]: # (")[0][1:]
             temp_call_args = line.split("]: # (")[1][:-1]
             if line.strip().endswith(")"):
                 in_dynamic_content = False
                 dynamic_content.append([temp_call_name, temp_call_args])
             else:
                 temp_call_args += line.split("]: # (")[1][-1]
                 in_dynamic_content = True
-            static_content.append("\n".join(temp_content))
+
+            if len(static_content) > 0:
+                for index in range(len(temp_content)):
+                    if temp_content[index].strip() == "":
+                        static_content.append("\n".join(temp_content[index:]))
+                        break
+            else:
+                static_content.append("\n".join(temp_content))
+            temp_content = []
         elif in_dynamic_content and line.strip().endswith(")"):
             temp_call_args += line[:-1].strip()
             dynamic_content.append([temp_call_name, temp_call_args])
             in_dynamic_content = False
         elif in_dynamic_content:
             temp_call_args += line.strip()
         else:
             temp_content.append(line)
 
-    return static_content, dynamic_content
-           
-
-content1 = load_md("test.md")
-content2 = load_md("../README.md")
-
-st.markdown(content1[0][0])
+    # Make sure to add the last bit of static content        
+    if len(temp_content) > 0:
+        for index in range(len(temp_content)):
+            if temp_content[index].strip() == "":
+                static_content.append("\n".join(temp_content[index:]))
+                break
 
-st.write("---")
-
-st.markdown(content2[0][0])
-
-st.write("---")
-
-st.write(content1[1])
+    return static_content, dynamic_content
 
-st.write(content2[1])
+def call_local_function(function_name, arguments, function):
+    try:
+        function(*literal_eval(arguments))
+    except Exception as e:
+        st.error("**ERROR!** An exception occurred while calling the function <" + function_name + "> with arguments: " + str(arguments) + " (see exception below)")
+        st.exception(e)
+
+def load_content(markdown_file_name, use_write=False, **kwargs):
+    static_content, dynamic_content = load_md(markdown_file_name)
+
+    for index in range(len(static_content)):
+        if use_write:
+            st.write(static_content[index], **kwargs)
+        else:
+            st.markdown(static_content[index], **kwargs)
+        if len(dynamic_content) > index:
+            caller_globals = dict(inspect.getmembers(inspect.stack()[1][0]))["f_locals"]
+            function_name = dynamic_content[index][0]
+            function_args = "[" + dynamic_content[index][1] + "]"
+            if function_name in caller_globals and callable(caller_globals[function_name]):
+                call_local_function(function_name, function_args, caller_globals[function_name])
+            else:
+                st.error('**ERROR!** `streamlit-islands` could not find a function called `<' + function_name + ">` in the streamlit script. Make sure the function is defined above the call to `load_content`.")
 
+    return static_content, dynamic_content
```

### Comparing `streamlit-islands-0.0.1/streamlit_islands.egg-info/PKG-INFO` & `streamlit-islands-0.0.2/streamlit_islands.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-islands
-Version: 0.0.1
+Version: 0.0.2
 Summary: Separate static content from dynamic content in Streamlit
 Home-page: https://github.com/bouzidanas/streamlit-islands
 Author: Anas Bouzid
 Author-email: anasbouzid@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

