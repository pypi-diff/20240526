# Comparing `tmp/python_ydotool-1.0.4.tar.gz` & `tmp/python_ydotool-1.0.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ydotool-1.0.4.tar", last modified: Sun May 26 17:18:26 2024, max compression
+gzip compressed data, was "python_ydotool-1.0.4.post1.tar", last modified: Sun May 26 17:34:28 2024, max compression
```

## Comparing `python_ydotool-1.0.4.tar` & `python_ydotool-1.0.4.post1.tar`

### file list

```diff
@@ -1,20 +1,29 @@
-drwxr-xr-x   0 antares   (1000) users      (100)        0 2024-05-26 17:18:26.006329 python_ydotool-1.0.4/
--rw-r--r--   0 antares   (1000) users      (100)    34523 2024-05-25 15:45:23.000000 python_ydotool-1.0.4/LICENSE
--rw-r--r--   0 antares   (1000) users      (100)     3646 2024-05-26 17:18:26.006329 python_ydotool-1.0.4/PKG-INFO
--rw-r--r--   0 antares   (1000) users      (100)     3289 2024-05-26 17:17:59.000000 python_ydotool-1.0.4/README.md
-drwxr-xr-x   0 antares   (1000) users      (100)        0 2024-05-26 17:18:26.006329 python_ydotool-1.0.4/pydotool/
--rw-r--r--   0 antares   (1000) users      (100)      246 2024-05-26 15:26:06.000000 python_ydotool-1.0.4/pydotool/__init__.py
--rw-r--r--   0 antares   (1000) users      (100)      464 2024-05-26 15:26:06.000000 python_ydotool-1.0.4/pydotool/_sequence.py
--rw-r--r--   0 antares   (1000) users      (100)     2011 2024-05-26 15:26:06.000000 python_ydotool-1.0.4/pydotool/ascii_2_keycode.py
--rw-r--r--   0 antares   (1000) users      (100)     2695 2024-05-26 16:59:59.000000 python_ydotool-1.0.4/pydotool/click.py
--rw-r--r--   0 antares   (1000) users      (100)    15034 2024-05-26 15:26:06.000000 python_ydotool-1.0.4/pydotool/input_event_code.py
--rw-r--r--   0 antares   (1000) users      (100)     2080 2024-05-26 16:59:59.000000 python_ydotool-1.0.4/pydotool/key.py
--rw-r--r--   0 antares   (1000) users      (100)      610 2024-05-26 15:26:06.000000 python_ydotool-1.0.4/pydotool/mousemove.py
--rw-r--r--   0 antares   (1000) users      (100)     1412 2024-05-26 15:26:06.000000 python_ydotool-1.0.4/pydotool/typetool.py
-drwxr-xr-x   0 antares   (1000) users      (100)        0 2024-05-26 17:18:26.006329 python_ydotool-1.0.4/python_ydotool.egg-info/
--rw-r--r--   0 antares   (1000) users      (100)     3646 2024-05-26 17:18:25.000000 python_ydotool-1.0.4/python_ydotool.egg-info/PKG-INFO
--rw-r--r--   0 antares   (1000) users      (100)      355 2024-05-26 17:18:25.000000 python_ydotool-1.0.4/python_ydotool.egg-info/SOURCES.txt
--rw-r--r--   0 antares   (1000) users      (100)        1 2024-05-26 17:18:25.000000 python_ydotool-1.0.4/python_ydotool.egg-info/dependency_links.txt
--rw-r--r--   0 antares   (1000) users      (100)       19 2024-05-26 17:18:25.000000 python_ydotool-1.0.4/python_ydotool.egg-info/top_level.txt
--rw-r--r--   0 antares   (1000) users      (100)       38 2024-05-26 17:18:26.006329 python_ydotool-1.0.4/setup.cfg
--rw-r--r--   0 antares   (1000) users      (100)     2386 2024-05-26 17:17:59.000000 python_ydotool-1.0.4/setup.py
+drwxr-xr-x   0 antares   (1000) users      (100)        0 2024-05-26 17:34:28.882366 python_ydotool-1.0.4.post1/
+-rw-r--r--   0 antares   (1000) users      (100)     1401 2024-05-26 17:34:15.000000 python_ydotool-1.0.4.post1/CMakeLists.txt
+-rw-r--r--   0 antares   (1000) users      (100)    34523 2024-05-25 15:45:23.000000 python_ydotool-1.0.4.post1/LICENSE
+-rw-r--r--   0 antares   (1000) users      (100)       67 2024-05-26 17:32:50.000000 python_ydotool-1.0.4.post1/MANIFEST.in
+-rw-r--r--   0 antares   (1000) users      (100)     3652 2024-05-26 17:34:28.881366 python_ydotool-1.0.4.post1/PKG-INFO
+-rw-r--r--   0 antares   (1000) users      (100)     3289 2024-05-26 17:17:59.000000 python_ydotool-1.0.4.post1/README.md
+drwxr-xr-x   0 antares   (1000) users      (100)        0 2024-05-26 17:34:28.881366 python_ydotool-1.0.4.post1/pydotool/
+-rw-r--r--   0 antares   (1000) users      (100)      246 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/pydotool/__init__.py
+-rw-r--r--   0 antares   (1000) users      (100)      464 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/pydotool/_sequence.py
+-rw-r--r--   0 antares   (1000) users      (100)     2011 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/pydotool/ascii_2_keycode.py
+-rw-r--r--   0 antares   (1000) users      (100)     2695 2024-05-26 16:59:59.000000 python_ydotool-1.0.4.post1/pydotool/click.py
+-rw-r--r--   0 antares   (1000) users      (100)    15034 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/pydotool/input_event_code.py
+-rw-r--r--   0 antares   (1000) users      (100)     2080 2024-05-26 16:59:59.000000 python_ydotool-1.0.4.post1/pydotool/key.py
+-rw-r--r--   0 antares   (1000) users      (100)      610 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/pydotool/mousemove.py
+-rw-r--r--   0 antares   (1000) users      (100)     1412 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/pydotool/typetool.py
+drwxr-xr-x   0 antares   (1000) users      (100)        0 2024-05-26 17:34:28.881366 python_ydotool-1.0.4.post1/python_ydotool.egg-info/
+-rw-r--r--   0 antares   (1000) users      (100)     3652 2024-05-26 17:34:28.000000 python_ydotool-1.0.4.post1/python_ydotool.egg-info/PKG-INFO
+-rw-r--r--   0 antares   (1000) users      (100)      480 2024-05-26 17:34:28.000000 python_ydotool-1.0.4.post1/python_ydotool.egg-info/SOURCES.txt
+-rw-r--r--   0 antares   (1000) users      (100)        1 2024-05-26 17:34:28.000000 python_ydotool-1.0.4.post1/python_ydotool.egg-info/dependency_links.txt
+-rw-r--r--   0 antares   (1000) users      (100)       19 2024-05-26 17:34:28.000000 python_ydotool-1.0.4.post1/python_ydotool.egg-info/top_level.txt
+-rw-r--r--   0 antares   (1000) users      (100)       38 2024-05-26 17:34:28.882366 python_ydotool-1.0.4.post1/setup.cfg
+-rw-r--r--   0 antares   (1000) users      (100)     2502 2024-05-26 17:31:50.000000 python_ydotool-1.0.4.post1/setup.py
+-rw-r--r--   0 antares   (1000) users      (100)       12 2024-05-26 17:29:39.000000 python_ydotool-1.0.4.post1/version
+drwxr-xr-x   0 antares   (1000) users      (100)        0 2024-05-26 17:34:28.881366 python_ydotool-1.0.4.post1/ydotool/
+-rw-r--r--   0 antares   (1000) users      (100)    34523 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/ydotool/LICENSE
+-rw-r--r--   0 antares   (1000) users      (100)     4245 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/ydotool/pydotool.c
+-rw-r--r--   0 antares   (1000) users      (100)      143 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/ydotool/pydotool.h
+-rw-r--r--   0 antares   (1000) users      (100)     2110 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/ydotool/ydotool.c
+-rw-r--r--   0 antares   (1000) users      (100)     2206 2024-05-26 15:26:06.000000 python_ydotool-1.0.4.post1/ydotool/ydotool.h
```

### Comparing `python_ydotool-1.0.4/LICENSE` & `python_ydotool-1.0.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ydotool-1.0.4/PKG-INFO` & `python_ydotool-1.0.4.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ydotool
-Version: 1.0.4
+Version: 1.0.4.post1
 Summary: ydotool client implemented in Python
 Home-page: https://github.com/Antares0982/pydotool
 Project-URL: Bug Tracker, https://github.com/Antares0982/pydotool/issues
 Project-URL: Source Code, https://github.com/Antares0982/pydotool
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python_ydotool-1.0.4/README.md` & `python_ydotool-1.0.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `python_ydotool-1.0.4/pydotool/ascii_2_keycode.py` & `python_ydotool-1.0.4.post1/pydotool/ascii_2_keycode.py`

 * *Files identical despite different names*

### Comparing `python_ydotool-1.0.4/pydotool/click.py` & `python_ydotool-1.0.4.post1/pydotool/click.py`

 * *Files identical despite different names*

### Comparing `python_ydotool-1.0.4/pydotool/input_event_code.py` & `python_ydotool-1.0.4.post1/pydotool/input_event_code.py`

 * *Files identical despite different names*

### Comparing `python_ydotool-1.0.4/pydotool/key.py` & `python_ydotool-1.0.4.post1/pydotool/key.py`

 * *Files identical despite different names*

### Comparing `python_ydotool-1.0.4/pydotool/mousemove.py` & `python_ydotool-1.0.4.post1/pydotool/mousemove.py`

 * *Files identical despite different names*

### Comparing `python_ydotool-1.0.4/pydotool/typetool.py` & `python_ydotool-1.0.4.post1/pydotool/typetool.py`

 * *Files identical despite different names*

### Comparing `python_ydotool-1.0.4/python_ydotool.egg-info/PKG-INFO` & `python_ydotool-1.0.4.post1/python_ydotool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ydotool
-Version: 1.0.4
+Version: 1.0.4.post1
 Summary: ydotool client implemented in Python
 Home-page: https://github.com/Antares0982/pydotool
 Project-URL: Bug Tracker, https://github.com/Antares0982/pydotool/issues
 Project-URL: Source Code, https://github.com/Antares0982/pydotool
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python_ydotool-1.0.4/setup.py` & `python_ydotool-1.0.4.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,24 +47,28 @@
             extdir = os.path.abspath(os.path.dirname(ext_fullpath))
             os.rename(os.path.join(extdir, f'{ext.name}.so'), ext_fullpath)
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+with open("version", "r") as version_file:
+    version = version_file.read().strip()
+
 setup(
     name='python-ydotool',
-    version="v1.0.4",
+    version=version,
     ext_modules=[
         CMakeExtension(name='_pydotool'),
     ],
     url='https://github.com/Antares0982/pydotool',
     project_urls={
         'Bug Tracker': 'https://github.com/Antares0982/pydotool/issues',
         'Source Code': 'https://github.com/Antares0982/pydotool',
     },
+    include_package_data=True,
     description='ydotool client implemented in Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     cmdclass={'build_ext': cmake_build_ext},
     packages=['pydotool'],  # List your Python packages
 )
```

