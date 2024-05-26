# Comparing `tmp/contact-notes-local-0.0.8.tar.gz` & `tmp/contact-notes-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-notes-local-0.0.8.tar", last modified: Wed Feb  7 16:29:38 2024, max compression
+gzip compressed data, was "contact-notes-local-0.0.9.tar", last modified: Wed Feb  7 16:36:27 2024, max compression
```

## Comparing `contact-notes-local-0.0.8.tar` & `contact-notes-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 16:29:38.831520 contact-notes-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-07 16:29:38.831520 contact-notes-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-07 16:29:03.000000 contact-notes-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 16:29:38.827520 contact-notes-local-0.0.8/contact_notes_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 16:29:38.831520 contact-notes-local-0.0.8/contact_notes_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 16:29:03.000000 contact-notes-local-0.0.8/contact_notes_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-02-07 16:29:03.000000 contact-notes-local-0.0.8/contact_notes_local/src/contact_notes_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-07 16:29:03.000000 contact-notes-local-0.0.8/contact_notes_local/src/contact_notes_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 16:29:38.831520 contact-notes-local-0.0.8/contact_notes_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-07 16:29:38.000000 contact-notes-local-0.0.8/contact_notes_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-07 16:29:38.000000 contact-notes-local-0.0.8/contact_notes_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 16:29:38.000000 contact-notes-local-0.0.8/contact_notes_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-07 16:29:38.000000 contact-notes-local-0.0.8/contact_notes_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-07 16:29:38.000000 contact-notes-local-0.0.8/contact_notes_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-07 16:29:03.000000 contact-notes-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 16:29:38.831520 contact-notes-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-02-07 16:29:03.000000 contact-notes-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 16:36:27.740981 contact-notes-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-07 16:36:27.740981 contact-notes-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-07 16:35:58.000000 contact-notes-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 16:36:27.736981 contact-notes-local-0.0.9/contact_notes_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 16:36:27.740981 contact-notes-local-0.0.9/contact_notes_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 16:35:58.000000 contact-notes-local-0.0.9/contact_notes_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-02-07 16:35:58.000000 contact-notes-local-0.0.9/contact_notes_local/src/contact_notes_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-07 16:35:58.000000 contact-notes-local-0.0.9/contact_notes_local/src/contact_notes_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 16:36:27.740981 contact-notes-local-0.0.9/contact_notes_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-07 16:36:27.000000 contact-notes-local-0.0.9/contact_notes_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-07 16:36:27.000000 contact-notes-local-0.0.9/contact_notes_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 16:36:27.000000 contact-notes-local-0.0.9/contact_notes_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-07 16:36:27.000000 contact-notes-local-0.0.9/contact_notes_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-07 16:36:27.000000 contact-notes-local-0.0.9/contact_notes_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-07 16:35:58.000000 contact-notes-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 16:36:27.740981 contact-notes-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-02-07 16:35:58.000000 contact-notes-local-0.0.9/setup.py
```

### Comparing `contact-notes-local-0.0.8/PKG-INFO` & `contact-notes-local-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-notes-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-notes-local Python
 Home-page: https://github.com/circles-zone/contact-note-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-notes-local-0.0.8/contact_notes_local/src/contact_notes_local.py` & `contact-notes-local-0.0.9/contact_notes_local/src/contact_notes_local.py`

 * *Files identical despite different names*

### Comparing `contact-notes-local-0.0.8/contact_notes_local/src/contact_notes_local_constants.py` & `contact-notes-local-0.0.9/contact_notes_local/src/contact_notes_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact-notes-local-0.0.8/contact_notes_local.egg-info/PKG-INFO` & `contact-notes-local-0.0.9/contact_notes_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-notes-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-notes-local Python
 Home-page: https://github.com/circles-zone/contact-note-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-notes-local-0.0.8/setup.py` & `contact-notes-local-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "contact-notes-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # update only the minor version each time # https://pypi.org/project/contact-notes-local/
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/contact-notes-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-notes-local Python",
     long_description="PyPI Package for Circles contact-notes-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/contact-note-local-python-package",  # https://pypi.org/project/contact-notes-local/
     packages=[package_dir],
```

