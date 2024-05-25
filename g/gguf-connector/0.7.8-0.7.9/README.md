# Comparing `tmp/gguf_connector-0.7.8.tar.gz` & `tmp/gguf_connector-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gguf_connector-0.7.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gguf_connector-0.7.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gguf_connector-0.7.8.tar` & `gguf_connector-0.7.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 gguf_connector-0.7.8/LICENSE
--rw-r--r--   0        0        0     3361 2024-02-18 08:44:33.171007 gguf_connector-0.7.8/README.md
--rw-r--r--   0        0        0      628 2024-02-14 23:15:25.918476 gguf_connector-0.7.8/pyproject.toml
--rw-r--r--   0        0        0     1415 2024-02-18 08:44:15.671467 gguf_connector-0.7.8/src/gguf_connector/__init__.py
--rw-r--r--   0        0        0     1840 2024-01-30 01:31:08.777941 gguf_connector-0.7.8/src/gguf_connector/c.py
--rw-r--r--   0        0        0    16203 2024-02-17 01:02:43.963670 gguf_connector-0.7.8/src/gguf_connector/const.py
--rw-r--r--   0        0        0     3804 2024-02-13 01:19:56.303546 gguf_connector-0.7.8/src/gguf_connector/cp.py
--rw-r--r--   0        0        0     1859 2024-02-10 00:57:25.529668 gguf_connector-0.7.8/src/gguf_connector/cpp.py
--rw-r--r--   0        0        0     2560 2024-02-18 08:44:08.020982 gguf_connector-0.7.8/src/gguf_connector/data.json
--rw-r--r--   0        0        0     1107 2024-01-25 22:42:23.643191 gguf_connector-0.7.8/src/gguf_connector/g.py
--rw-r--r--   0        0        0     1160 2024-01-25 22:42:36.329688 gguf_connector-0.7.8/src/gguf_connector/gpp.py
--rw-r--r--   0        0        0      742 2024-01-08 04:10:18.194979 gguf_connector-0.7.8/src/gguf_connector/logo.png
--rw-r--r--   0        0        0     2209 2024-02-06 01:28:14.547133 gguf_connector-0.7.8/src/gguf_connector/m.py
--rw-r--r--   0        0        0      794 2024-01-30 01:29:40.229066 gguf_connector-0.7.8/src/gguf_connector/menu.py
--rw-r--r--   0        0        0     3802 2024-02-13 01:20:02.166806 gguf_connector-0.7.8/src/gguf_connector/pp.py
--rw-r--r--   0        0        0     1709 2024-02-17 02:02:07.805031 gguf_connector-0.7.8/src/gguf_connector/r.py
--rw-r--r--   0        0        0     9507 2024-02-18 00:08:52.652959 gguf_connector-0.7.8/src/gguf_connector/reader.py
--rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 gguf_connector-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1095 2024-01-21 23:59:42.278418 gguf_connector-0.7.9/LICENSE
+-rw-r--r--   0        0        0     3361 2024-02-19 03:51:33.999706 gguf_connector-0.7.9/README.md
+-rw-r--r--   0        0        0      628 2024-02-14 23:15:25.918476 gguf_connector-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     1415 2024-02-19 03:50:53.986771 gguf_connector-0.7.9/src/gguf_connector/__init__.py
+-rw-r--r--   0        0        0     1840 2024-01-30 01:31:08.777941 gguf_connector-0.7.9/src/gguf_connector/c.py
+-rw-r--r--   0        0        0    16203 2024-02-17 01:02:43.963670 gguf_connector-0.7.9/src/gguf_connector/const.py
+-rw-r--r--   0        0        0     3804 2024-02-13 01:19:56.303546 gguf_connector-0.7.9/src/gguf_connector/cp.py
+-rw-r--r--   0        0        0     1859 2024-02-10 00:57:25.529668 gguf_connector-0.7.9/src/gguf_connector/cpp.py
+-rw-r--r--   0        0        0     2560 2024-02-19 03:50:30.421974 gguf_connector-0.7.9/src/gguf_connector/data.json
+-rw-r--r--   0        0        0     1107 2024-01-25 22:42:23.643191 gguf_connector-0.7.9/src/gguf_connector/g.py
+-rw-r--r--   0        0        0     1160 2024-01-25 22:42:36.329688 gguf_connector-0.7.9/src/gguf_connector/gpp.py
+-rw-r--r--   0        0        0      742 2024-01-08 04:10:18.194979 gguf_connector-0.7.9/src/gguf_connector/logo.png
+-rw-r--r--   0        0        0     2209 2024-02-06 01:28:14.547133 gguf_connector-0.7.9/src/gguf_connector/m.py
+-rw-r--r--   0        0        0      794 2024-01-30 01:29:40.229066 gguf_connector-0.7.9/src/gguf_connector/menu.py
+-rw-r--r--   0        0        0     3802 2024-02-13 01:20:02.166806 gguf_connector-0.7.9/src/gguf_connector/pp.py
+-rw-r--r--   0        0        0     1709 2024-02-17 02:02:07.805031 gguf_connector-0.7.9/src/gguf_connector/r.py
+-rw-r--r--   0        0        0     9507 2024-02-18 00:08:52.652959 gguf_connector-0.7.9/src/gguf_connector/reader.py
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 gguf_connector-0.7.9/PKG-INFO
```

### Comparing `gguf_connector-0.7.8/LICENSE` & `gguf_connector-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/README.md` & `gguf_connector-0.7.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## GGUF connector
 
 GGUF (GPT-Generated Unified Format) is a successor of GGML (GPT-Generated Model Language), it was released on August 21, 2023; by the way, GPT stands for Generative Pre-trained Transformer.
 
 [<img src="https://raw.githubusercontent.com/calcuis/gguf-connector/master/gguf.gif" width="128" height="128">](https://github.com/calcuis/gguf-connector)
-[![Static Badge](https://img.shields.io/badge/version-0.7.8-green?logo=github)](https://github.com/calcuis/gguf-connector/releases)
+[![Static Badge](https://img.shields.io/badge/version-0.7.9-green?logo=github)](https://github.com/calcuis/gguf-connector/releases)
 [![Static Badge](https://img.shields.io/badge/pack-0.1.3-green?logo=microsoft)](https://github.com/calcuis/chatgpt-model-selector/releases)
 
 This package is a simple graphical user interface (GUI) application that uses the ctransformers or llama.cpp to interact with a chat model for generating responses.
 
 Install the connector via pip (once only):
 ```
 pip install gguf-connector
```

### Comparing `gguf_connector-0.7.8/pyproject.toml` & `gguf_connector-0.7.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/__init__.py` & `gguf_connector-0.7.9/src/gguf_connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # !/usr/bin/env python3
 
-__version__="0.7.8"
+__version__="0.7.9"
 
 def __init__():
     import argparse
     parser = argparse.ArgumentParser()
     parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__)
     subparsers = parser.add_subparsers(title="subcommands", dest="subcommand", help="choose a subcommand:")
     subparsers.add_parser('cpp', help='[cpp] connector cpp')
```

### Comparing `gguf_connector-0.7.8/src/gguf_connector/c.py` & `gguf_connector-0.7.9/src/gguf_connector/c.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/const.py` & `gguf_connector-0.7.9/src/gguf_connector/const.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/cp.py` & `gguf_connector-0.7.9/src/gguf_connector/cp.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/cpp.py` & `gguf_connector-0.7.9/src/gguf_connector/cpp.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/data.json` & `gguf_connector-0.7.9/src/gguf_connector/data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.859375%*

 * *Differences: {'0': "{'name': ' chat.gguf     [1.9GB; for general purpose]'}",*

 * * '1': "{'name': ' code.gguf     [3.3GB; for coding assistance]'}",*

 * * '2': "{'name': ' medi.gguf     [3.3GB; for medical/health advice]'}",*

 * * '3': "{'name': ' law.gguf      [3.3GB; for law/legal opinion]'}",*

 * * '4': "{'name': ' finance.gguf  [3.3GB; for wealth/financial plan]'}",*

 * * '5': "{'name': ' coder.gguf    [1.4GB; for simple coding issue]'}",*

 * * '6': "{'name': ' phi2.gguf     [1.4GB; for technical problem]'}",*

 * * '7': "{'name': ' lam2.gguf     [3. […]*

```diff
@@ -1,42 +1,42 @@
 [
     {
-        "name": "chat.gguf      [1.9GB; for general purpose]",
+        "name": " chat.gguf     [1.9GB; for general purpose]",
         "url": "https://huggingface.co/calcuis/chat/resolve/main/chat.gguf"
     },
     {
-        "name": "code.gguf      [3.3GB; for coding assistance]",
+        "name": " code.gguf     [3.3GB; for coding assistance]",
         "url": "https://huggingface.co/calcuis/code_mini/resolve/main/code.gguf"
     },
     {
-        "name": "medi.gguf      [3.3GB; for medical/health advice]",
+        "name": " medi.gguf     [3.3GB; for medical/health advice]",
         "url": "https://huggingface.co/calcuis/medi_mini/resolve/main/medi.gguf"
     },
     {
-        "name": "law.gguf       [3.3GB; for law/legal opinion]",
+        "name": " law.gguf      [3.3GB; for law/legal opinion]",
         "url": "https://huggingface.co/calcuis/law_mini/resolve/main/law.gguf"
     },
     {
-        "name": "finance.gguf   [3.3GB; for wealth/financial plan]",
+        "name": " finance.gguf  [3.3GB; for wealth/financial plan]",
         "url": "https://huggingface.co/calcuis/gguf/resolve/main/finance.gguf"
     },
     {
-        "name": "coder.gguf     [1.4GB; for simple coding issue]",
+        "name": " coder.gguf    [1.4GB; for simple coding issue]",
         "url": "https://huggingface.co/calcuis/gguf/resolve/main/coder.gguf"
     },
     {
-        "name": "phi2.gguf      [1.4GB; for technical problem]",
+        "name": " phi2.gguf     [1.4GB; for technical problem]",
         "url": "https://huggingface.co/calcuis/phi2_mini/resolve/main/phi2.gguf"
     },
     {
-        "name": "lam2.gguf      [3.3GB; for long/detailed response]",
+        "name": " lam2.gguf     [3.3GB; for long/detailed response]",
         "url": "https://huggingface.co/calcuis/lam2_mini/resolve/main/lam2.gguf"
     },
     {
-        "name": "tiny2.gguf     [783MB; for fast/rapid response]",
+        "name": " tiny2.gguf    [783MB; for fast/rapid response]",
         "url": "https://huggingface.co/calcuis/gguf/resolve/main/tiny2.gguf"
     },
     {
         "name": "stable.gguf   [1.7GB; for code review]",
         "url": "https://huggingface.co/calcuis/gguf/resolve/main/stable.gguf"
     },
     {
```

### Comparing `gguf_connector-0.7.8/src/gguf_connector/g.py` & `gguf_connector-0.7.9/src/gguf_connector/g.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/gpp.py` & `gguf_connector-0.7.9/src/gguf_connector/gpp.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/logo.png` & `gguf_connector-0.7.9/src/gguf_connector/logo.png`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/m.py` & `gguf_connector-0.7.9/src/gguf_connector/m.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/menu.py` & `gguf_connector-0.7.9/src/gguf_connector/menu.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/pp.py` & `gguf_connector-0.7.9/src/gguf_connector/pp.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/r.py` & `gguf_connector-0.7.9/src/gguf_connector/r.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/src/gguf_connector/reader.py` & `gguf_connector-0.7.9/src/gguf_connector/reader.py`

 * *Files identical despite different names*

### Comparing `gguf_connector-0.7.8/PKG-INFO` & `gguf_connector-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gguf-connector
-Version: 0.7.8
+Version: 0.7.9
 Summary: GGUF connector(s) with GUI
 Author-email: calcuis <calculatics@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: llama-cpp-python
 Requires-Dist: ctransformers
 Requires-Dist: pypdf
@@ -12,15 +12,15 @@
 Project-URL: Issues, https://github.com/calcuis/gguf-connector/issues
 
 ## GGUF connector
 
 GGUF (GPT-Generated Unified Format) is a successor of GGML (GPT-Generated Model Language), it was released on August 21, 2023; by the way, GPT stands for Generative Pre-trained Transformer.
 
 [<img src="https://raw.githubusercontent.com/calcuis/gguf-connector/master/gguf.gif" width="128" height="128">](https://github.com/calcuis/gguf-connector)
-[![Static Badge](https://img.shields.io/badge/version-0.7.8-green?logo=github)](https://github.com/calcuis/gguf-connector/releases)
+[![Static Badge](https://img.shields.io/badge/version-0.7.9-green?logo=github)](https://github.com/calcuis/gguf-connector/releases)
 [![Static Badge](https://img.shields.io/badge/pack-0.1.3-green?logo=microsoft)](https://github.com/calcuis/chatgpt-model-selector/releases)
 
 This package is a simple graphical user interface (GUI) application that uses the ctransformers or llama.cpp to interact with a chat model for generating responses.
 
 Install the connector via pip (once only):
 ```
 pip install gguf-connector
```

