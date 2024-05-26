# Comparing `tmp/graphretrieval-0.1.7.tar.gz` & `tmp/graphretrieval-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphretrieval-0.1.7.tar", last modified: Sun May 26 07:44:36 2024, max compression
+gzip compressed data, was "graphretrieval-0.1.8.tar", last modified: Sun May 26 08:06:41 2024, max compression
```

## Comparing `graphretrieval-0.1.7.tar` & `graphretrieval-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:44:36.910138 graphretrieval-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:44:36.906138 graphretrieval-0.1.7/GraphRetrieval/
--rw-r--r--   0 runner    (1001) docker     (127)    24319 2024-05-26 07:44:32.000000 graphretrieval-0.1.7/GraphRetrieval/GraphRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-26 07:44:32.000000 graphretrieval-0.1.7/GraphRetrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:44:36.910138 graphretrieval-0.1.7/GraphRetrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-26 07:44:36.910138 graphretrieval-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-26 07:44:32.000000 graphretrieval-0.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:44:36.910138 graphretrieval-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-26 07:44:32.000000 graphretrieval-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 08:06:41.378399 graphretrieval-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 08:06:41.374399 graphretrieval-0.1.8/GraphRetrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)    24315 2024-05-26 08:06:29.000000 graphretrieval-0.1.8/GraphRetrieval/GraphRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-26 08:06:29.000000 graphretrieval-0.1.8/GraphRetrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 08:06:41.374399 graphretrieval-0.1.8/GraphRetrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-26 08:06:41.000000 graphretrieval-0.1.8/GraphRetrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-26 08:06:41.000000 graphretrieval-0.1.8/GraphRetrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 08:06:41.000000 graphretrieval-0.1.8/GraphRetrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-26 08:06:41.000000 graphretrieval-0.1.8/GraphRetrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 08:06:41.000000 graphretrieval-0.1.8/GraphRetrieval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-26 08:06:41.378399 graphretrieval-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-26 08:06:29.000000 graphretrieval-0.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 08:06:41.378399 graphretrieval-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-26 08:06:29.000000 graphretrieval-0.1.8/setup.py
```

### Comparing `graphretrieval-0.1.7/GraphRetrieval/GraphRetrieval.py` & `graphretrieval-0.1.8/GraphRetrieval/GraphRetrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
         self.documents.extend(new_documents)
         self.embeddings = np.vstack((self.embeddings, new_embeddings))
 
         return self.graph, self.documents, self.embeddings
 
     def create_graph_from_pdf(self, pdf_file, similarity_threshold=0, chunk_size = 1250, chunk_overlap = 100):
         with open(pdf_file, "rb") as f:
-            pdf_reader = PyPDF2.PdfFileReader(f)
+            pdf_reader = PyPDF2.PdfReader(f)
             num_pages = pdf_reader.numPages
             text = ""
             for page_num in range(num_pages):
                 text += pdf_reader.getPage(page_num).extractText()
         self.graph, self.documents, self.embeddings = self.constructGraph(text, similarity_threshold=similarity_threshold)
         print("Graph created Successfully!")
```

### Comparing `graphretrieval-0.1.7/GraphRetrieval.egg-info/PKG-INFO` & `graphretrieval-0.1.8/GraphRetrieval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.7
+Version: 0.1.8
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
 Requires-Dist: langchain
 Requires-Dist: sentence_transformers
 Requires-Dist: langchain-community
 Requires-Dist: langchain-openai
 Requires-Dist: langchain-experimental
 Requires-Dist: neo4j
 Requires-Dist: tiktoken
-Requires-Dist: pypdf2
+Requires-Dist: pypdf2==3.0.0
 
 
 # GraphRetrieval
 
 GraphRetrieval is a Python library designed for advanced text retrieval and knowledge graph querying. It supports various models and techniques to enable efficient and accurate information retrieval from large text corpora and knowledge bases.
 
 ## Installation
```

### Comparing `graphretrieval-0.1.7/PKG-INFO` & `graphretrieval-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.7
+Version: 0.1.8
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
 Requires-Dist: langchain
 Requires-Dist: sentence_transformers
 Requires-Dist: langchain-community
 Requires-Dist: langchain-openai
 Requires-Dist: langchain-experimental
 Requires-Dist: neo4j
 Requires-Dist: tiktoken
-Requires-Dist: pypdf2
+Requires-Dist: pypdf2==3.0.0
 
 
 # GraphRetrieval
 
 GraphRetrieval is a Python library designed for advanced text retrieval and knowledge graph querying. It supports various models and techniques to enable efficient and accurate information retrieval from large text corpora and knowledge bases.
 
 ## Installation
```

### Comparing `graphretrieval-0.1.7/README.rst` & `graphretrieval-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `graphretrieval-0.1.7/setup.py` & `graphretrieval-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 This `README.md` provides an overview of the GraphRetrieval library, installation instructions, and example usage scenarios, with the specified changes to the file path and environment variables sections.
 """
 
 setup(
     name='GraphRetrieval',
-    version='0.1.7',
+    version='0.1.8',
     description='Graph retrieval',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='JVNK',
     author_email='jaya11vibhav@gmail.com',
     url='https://github.com/jayavibhavnk/GraphRetrieval',
     packages=find_packages(),
@@ -164,13 +164,13 @@
       'langchain',
       'sentence_transformers',
       'langchain-community', 
       'langchain-openai',
       'langchain-experimental',
       'neo4j',
       'tiktoken',
-      'pypdf2'
+      'pypdf2==3.0.0'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha'
     ],
 )
```

