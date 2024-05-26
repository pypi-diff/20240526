# Comparing `tmp/dreamai-2.0.6.tar.gz` & `tmp/dreamai-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-2.0.6.tar", max compression
+gzip compressed data, was "dreamai-2.0.7.tar", max compression
```

## Comparing `dreamai-2.0.6.tar` & `dreamai-2.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.6/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.6/dreamai/__init__.py
--rw-r--r--   0        0        0     3765 2024-05-26 03:29:34.217009 dreamai-2.0.6/dreamai/ai.py
--rw-r--r--   0        0        0     6127 2024-05-11 13:59:15.167712 dreamai-2.0.6/dreamai/chroma.py
--rw-r--r--   0        0        0     1897 2024-05-08 13:31:52.980653 dreamai-2.0.6/dreamai/pdf.py
--rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0.6/dreamai/templates.py
--rw-r--r--   0        0        0    12777 2024-05-01 13:37:33.386393 dreamai-2.0.6/dreamai/utils.py
--rw-r--r--   0        0        0     1578 2024-05-26 11:19:43.950898 dreamai-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 dreamai-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.7/dreamai/__init__.py
+-rw-r--r--   0        0        0     3765 2024-05-26 03:29:34.217009 dreamai-2.0.7/dreamai/ai.py
+-rw-r--r--   0        0        0     6127 2024-05-11 13:59:15.167712 dreamai-2.0.7/dreamai/chroma.py
+-rw-r--r--   0        0        0     1897 2024-05-08 13:31:52.980653 dreamai-2.0.7/dreamai/pdf.py
+-rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0.7/dreamai/templates.py
+-rw-r--r--   0        0        0    12777 2024-05-01 13:37:33.386393 dreamai-2.0.7/dreamai/utils.py
+-rw-r--r--   0        0        0     1504 2024-05-26 12:19:08.556516 dreamai-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 dreamai-2.0.7/PKG-INFO
```

### Comparing `dreamai-2.0.6/dreamai/ai.py` & `dreamai-2.0.7/dreamai/ai.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.6/dreamai/chroma.py` & `dreamai-2.0.7/dreamai/chroma.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.6/dreamai/pdf.py` & `dreamai-2.0.7/dreamai/pdf.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.6/dreamai/templates.py` & `dreamai-2.0.7/dreamai/templates.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.6/dreamai/utils.py` & `dreamai-2.0.7/dreamai/utils.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0.6/pyproject.toml` & `dreamai-2.0.7/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dreamai"
-version = "2.0.6"
+version = "2.0.7"
 description = "🔂"
 authors = ["Hamza Farhan <thehamza96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 python-dotenv = "^1.0.1"
@@ -12,52 +12,49 @@
 openai = "^1.16.1"
 tiktoken = "^0.6.0"
 instructor = "^1.0.0"
 langchain = "^0.1.14"
 fastapi = "^0.110.1"
 demoji = "^1.1.0"
 litellm = "^1.34.22"
-dspy-ai = "^2.4.0"
 pypdf = "^4.1.0"
 chromadb = "^0.4.24"
 sentence-transformers = "^2.6.1"
 anthropic = "^0.23.0"
-modal = "^0.62.43"
 install = "^1.3.5"
 scikit-image = "^0.23.1"
 ultralytics = "^8.1.47"
 supervision = "^0.19.0"
-moviepy = "^1.0.3"
-youtube-transcript-api = "^0.6.2"
 scrapy = "^2.11.1"
 crochet = "^2.1.1"
-graphviz = "^0.20.3"
 streamlit = "^1.33.0"
 playwright = "^1.43.0"
 aiohttp = "^3.9.5"
-feedparser = "^6.0.11"
 accelerate = "^0.29.3"
-pyannote-audio = "^3.1.1"
 cython = "^3.0.10"
 logfire = "^0.28.0"
-streamlit-agraph = "^0.0.45"
-networkx = "^3.3"
-pygraphviz = "^1.13"
 hvplot = "^0.10.0"
 watchfiles = "^0.21.0"
 pygments = "^2.18.0"
 jupyter-bokeh = "^4.0.4"
 dash = "^2.17.0"
 dash-bootstrap-components = "^1.6.0"
 fastui = "^0.6.0"
 python-multipart = "^0.0.9"
 dash-cytoscape = "^1.0.1"
 google-generativeai = "^0.5.4"
 
 [tool.poetry.group.dev.dependencies]
+moviepy = "^1.0.3"
+feedparser = "^6.0.11"
+modal = "^0.62.43"
+youtube-transcript-api = "^0.6.2"
+pygraphviz = "^1.13"
+networkx = "^3.3"
+graphviz = "^0.20.3"
 podcast-downloader = {git = "https://github.com/dplocki/podcast-downloader.git"}
 faster-whisper = {git = "https://github.com/SYSTRAN/faster-whisper.git"}
 notebook = "^7.1.2"
 ipython = "^8.23.0"
 ipywidgets = "^8.1.2"
 pytest = "^8.1.1"
 ruff = "^0.3.5"
```

