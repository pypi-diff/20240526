# Comparing `tmp/semantic_space-0.0.0.tar.gz` & `tmp/semantic_space-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_space-0.0.0.tar", max compression
+gzip compressed data, was "semantic_space-0.0.1.tar", max compression
```

## Comparing `semantic_space-0.0.0.tar` & `semantic_space-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2024-05-25 10:24:47.840448 semantic_space-0.0.0/LICENSE.txt
--rw-r--r--   0        0        0      605 2024-05-26 20:01:53.433898 semantic_space-0.0.0/README.md
--rw-r--r--   0        0        0      563 2024-05-26 20:03:55.108255 semantic_space-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-26 19:40:02.870876 semantic_space-0.0.0/semantic_space/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 09:58:35.728018 semantic_space-0.0.0/semantic_space/models/__init__.py
--rw-r--r--   0        0        0     6994 2024-05-26 19:28:39.850331 semantic_space-0.0.0/semantic_space/models/grams.py
--rw-r--r--   0        0        0        0 2024-05-25 09:57:09.699010 semantic_space-0.0.0/semantic_space/tools/__init__.py
--rw-r--r--   0        0        0     9221 2024-05-26 19:17:02.217015 semantic_space-0.0.0/semantic_space/tools/preprocessing.py
--rw-r--r--   0        0        0    15744 2024-05-26 15:32:00.201400 semantic_space-0.0.0/semantic_space/tools/tokens.py
--rw-r--r--   0        0        0        0 2024-05-25 10:39:29.284710 semantic_space-0.0.0/semantic_space/utils/__init__.py
--rw-r--r--   0        0        0      312 2024-05-26 19:28:39.853965 semantic_space-0.0.0/semantic_space/utils/exceptions.py
--rw-r--r--   0        0        0      984 2024-05-26 15:32:00.192645 semantic_space-0.0.0/semantic_space/utils/types.py
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 semantic_space-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-25 10:24:47.840448 semantic_space-0.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      613 2024-05-26 20:06:51.257200 semantic_space-0.0.1/README.md
+-rw-r--r--   0        0        0      563 2024-05-26 20:06:51.253686 semantic_space-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-26 19:40:02.870876 semantic_space-0.0.1/semantic_space/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 09:58:35.728018 semantic_space-0.0.1/semantic_space/models/__init__.py
+-rw-r--r--   0        0        0     6994 2024-05-26 19:28:39.850331 semantic_space-0.0.1/semantic_space/models/grams.py
+-rw-r--r--   0        0        0        0 2024-05-25 09:57:09.699010 semantic_space-0.0.1/semantic_space/tools/__init__.py
+-rw-r--r--   0        0        0     9221 2024-05-26 19:17:02.217015 semantic_space-0.0.1/semantic_space/tools/preprocessing.py
+-rw-r--r--   0        0        0    15744 2024-05-26 15:32:00.201400 semantic_space-0.0.1/semantic_space/tools/tokens.py
+-rw-r--r--   0        0        0        0 2024-05-25 10:39:29.284710 semantic_space-0.0.1/semantic_space/utils/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-26 19:28:39.853965 semantic_space-0.0.1/semantic_space/utils/exceptions.py
+-rw-r--r--   0        0        0      984 2024-05-26 15:32:00.192645 semantic_space-0.0.1/semantic_space/utils/types.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 semantic_space-0.0.1/PKG-INFO
```

### Comparing `semantic_space-0.0.0/LICENSE.txt` & `semantic_space-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semantic_space-0.0.0/README.md` & `semantic_space-0.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # sematnic-space
 
 A basic NLP library for modelization and tokenization.
 
-_pip install libnlp_
+_pip install semantic-space_
 
 ## Project Details
 
 This is a project where I collect the codes that I have written
 for NLP applications. I have modularized some of the code that
 I have used for [AhmetGPT](https://github.com/ahmeterdem1/ahmetgpt), and prepared
 a well-structured library for similar applications. The code may be buggy, haven't
```

### Comparing `semantic_space-0.0.0/pyproject.toml` & `semantic_space-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "semantic-space"
-version = "0.0.0"
+version = "0.0.1"
 description = "A basic NLP library for modelization and tokenization."
 authors = ["Ahmet Erdem <ahmetblk1035@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ahmeterdem1/semantic-space"
 keywords = ["NLP", "Natural Language Processing", "library"]
```

### Comparing `semantic_space-0.0.0/semantic_space/models/grams.py` & `semantic_space-0.0.1/semantic_space/models/grams.py`

 * *Files identical despite different names*

### Comparing `semantic_space-0.0.0/semantic_space/tools/preprocessing.py` & `semantic_space-0.0.1/semantic_space/tools/preprocessing.py`

 * *Files identical despite different names*

### Comparing `semantic_space-0.0.0/semantic_space/tools/tokens.py` & `semantic_space-0.0.1/semantic_space/tools/tokens.py`

 * *Files identical despite different names*

### Comparing `semantic_space-0.0.0/semantic_space/utils/types.py` & `semantic_space-0.0.1/semantic_space/utils/types.py`

 * *Files identical despite different names*

### Comparing `semantic_space-0.0.0/PKG-INFO` & `semantic_space-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-space
-Version: 0.0.0
+Version: 0.0.1
 Summary: A basic NLP library for modelization and tokenization.
 Home-page: https://github.com/ahmeterdem1/semantic-space
 License: MIT
 Keywords: NLP,Natural Language Processing,library
 Author: Ahmet Erdem
 Author-email: ahmetblk1035@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -19,15 +19,15 @@
 Project-URL: Repository, https://github.com/ahmeterdem1/semantic-space
 Description-Content-Type: text/markdown
 
 # sematnic-space
 
 A basic NLP library for modelization and tokenization.
 
-_pip install libnlp_
+_pip install semantic-space_
 
 ## Project Details
 
 This is a project where I collect the codes that I have written
 for NLP applications. I have modularized some of the code that
 I have used for [AhmetGPT](https://github.com/ahmeterdem1/ahmetgpt), and prepared
 a well-structured library for similar applications. The code may be buggy, haven't
```

