# Comparing `tmp/financial_datasets-0.1.8.tar.gz` & `tmp/financial_datasets-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financial_datasets-0.1.8.tar", max compression
+gzip compressed data, was "financial_datasets-0.1.9.tar", max compression
```

## Comparing `financial_datasets-0.1.8.tar` & `financial_datasets-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.8/LICENSE
--rw-r--r--   0        0        0     4090 2024-04-16 20:09:06.071968 financial_datasets-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.8/financial_datasets/__init__.py
--rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.8/financial_datasets/dataset.py
--rw-r--r--   0        0        0      598 2024-04-16 20:23:40.209155 financial_datasets-0.1.8/financial_datasets/filings.py
--rw-r--r--   0        0        0     9496 2024-04-16 20:09:06.083652 financial_datasets-0.1.8/financial_datasets/generator.py
--rw-r--r--   0        0        0     1457 2024-04-10 12:02:30.195140 financial_datasets-0.1.8/financial_datasets/prompts.py
--rw-r--r--   0        0        0      660 2024-04-16 20:24:53.919094 financial_datasets-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4983 1970-01-01 00:00:00.000000 financial_datasets-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-29 00:57:03.662287 financial_datasets-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4090 2024-04-16 20:09:06.071968 financial_datasets-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 00:57:47.261649 financial_datasets-0.1.9/financial_datasets/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-03 12:06:00.779549 financial_datasets-0.1.9/financial_datasets/dataset.py
+-rw-r--r--   0        0        0      598 2024-04-16 20:23:40.209155 financial_datasets-0.1.9/financial_datasets/filings.py
+-rw-r--r--   0        0        0     7003 2024-04-21 12:35:59.290852 financial_datasets-0.1.9/financial_datasets/generator.py
+-rw-r--r--   0        0        0     4016 2024-04-22 11:17:59.079006 financial_datasets-0.1.9/financial_datasets/parser.py
+-rw-r--r--   0        0        0     1457 2024-04-10 12:02:30.195140 financial_datasets-0.1.9/financial_datasets/prompts.py
+-rw-r--r--   0        0        0      659 2024-04-21 12:34:23.632329 financial_datasets-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 financial_datasets-0.1.9/PKG-INFO
```

### Comparing `financial_datasets-0.1.8/LICENSE` & `financial_datasets-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.8/README.md` & `financial_datasets-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.8/financial_datasets/filings.py` & `financial_datasets-0.1.9/financial_datasets/filings.py`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.8/financial_datasets/prompts.py` & `financial_datasets-0.1.9/financial_datasets/prompts.py`

 * *Files identical despite different names*

### Comparing `financial_datasets-0.1.8/pyproject.toml` & `financial_datasets-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financial-datasets"
-version = "0.1.8"
+version = "0.1.9"
 description = "Financial datasets for LLMs"
 authors = ["Virat Singh <virat@virat.ai>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "financial_datasets"}]
 
 [tool.poetry.dependencies]
@@ -14,15 +14,15 @@
 chromadb = "^0.4.24"
 tiktoken = "^0.6.0"
 anthropic = "^0.21.3"
 instructor = "^0.6.7"
 datasets = "^2.18.0"
 xmltodict = "^0.13.0"
 tqdm = "^4.66.2"
-edgartools = "^2.16.1"
+edgartools = "2.16.1"
 pypdf2 = "^3.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 twine = "^5.0.0"
 
 [build-system]
```

### Comparing `financial_datasets-0.1.8/PKG-INFO` & `financial_datasets-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: financial-datasets
-Version: 0.1.8
+Version: 0.1.9
 Summary: Financial datasets for LLMs
 License: MIT
 Author: Virat Singh
 Author-email: virat@virat.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: datasets (>=2.18.0,<3.0.0)
-Requires-Dist: edgartools (>=2.16.1,<3.0.0)
+Requires-Dist: edgartools (==2.16.1)
 Requires-Dist: instructor (>=0.6.7,<0.7.0)
 Requires-Dist: langchain (>=0.1.13,<0.2.0)
 Requires-Dist: openai (>=1.14.3,<2.0.0)
 Requires-Dist: pypdf2 (>=3.0.1,<4.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
```

