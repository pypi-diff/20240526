# Comparing `tmp/graphretrieval-0.1.6.tar.gz` & `tmp/graphretrieval-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphretrieval-0.1.6.tar", last modified: Sun May 26 07:31:01 2024, max compression
+gzip compressed data, was "graphretrieval-0.1.7.tar", last modified: Sun May 26 07:44:36 2024, max compression
```

## Comparing `graphretrieval-0.1.6.tar` & `graphretrieval-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/GraphRetrieval/
--rw-r--r--   0 runner    (1001) docker     (127)    24320 2024-05-26 07:30:56.000000 graphretrieval-0.1.6/GraphRetrieval/GraphRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-26 07:30:56.000000 graphretrieval-0.1.6/GraphRetrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/GraphRetrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-26 07:30:56.000000 graphretrieval-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-26 07:30:56.000000 graphretrieval-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:44:36.910138 graphretrieval-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:44:36.906138 graphretrieval-0.1.7/GraphRetrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)    24319 2024-05-26 07:44:32.000000 graphretrieval-0.1.7/GraphRetrieval/GraphRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-26 07:44:32.000000 graphretrieval-0.1.7/GraphRetrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:44:36.910138 graphretrieval-0.1.7/GraphRetrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 07:44:36.000000 graphretrieval-0.1.7/GraphRetrieval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-26 07:44:36.910138 graphretrieval-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-26 07:44:32.000000 graphretrieval-0.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:44:36.910138 graphretrieval-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-26 07:44:32.000000 graphretrieval-0.1.7/setup.py
```

### Comparing `graphretrieval-0.1.6/GraphRetrieval/GraphRetrieval.py` & `graphretrieval-0.1.7/GraphRetrieval/GraphRetrieval.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,23 +226,24 @@
         query: {query}
         """
         ans = self.query_openai(prompt_template.format(context=full_text, query=query))
 
         return ans
 
     def query_openai(self, query):
-        openai.api_key = "YOUR_OPENAI_API_KEY"
-        response = openai.ChatCompletion.create(
-            model="gpt-3.5-turbo",
+        client = OpenAI()
+        completion = client.chat.completions.create(
+            model="gpt-3.5-turbo-0125",
             messages=[
                 {"role": "system", "content": "You are a helpful assistant"},
                 {"role": "user", "content": query}
-            ]
+            ],
+            n=1
         )
-        return response['choices'][0]['message']['content']
+        return(completion.choices[0].message.content)
 
     def save_db(self, file_path):
         with open(file_path, 'wb') as file:
             pickle.dump((self.graph, self.documents, self.embeddings), file)
             print("saved!")
 
     def load_db(self, file_path):
```

### Comparing `graphretrieval-0.1.6/GraphRetrieval.egg-info/PKG-INFO` & `graphretrieval-0.1.7/GraphRetrieval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.6
+Version: 0.1.7
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
```

### Comparing `graphretrieval-0.1.6/PKG-INFO` & `graphretrieval-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.6
+Version: 0.1.7
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
```

### Comparing `graphretrieval-0.1.6/README.rst` & `graphretrieval-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `graphretrieval-0.1.6/setup.py` & `graphretrieval-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 This `README.md` provides an overview of the GraphRetrieval library, installation instructions, and example usage scenarios, with the specified changes to the file path and environment variables sections.
 """
 
 setup(
     name='GraphRetrieval',
-    version='0.1.6',
+    version='0.1.7',
     description='Graph retrieval',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='JVNK',
     author_email='jaya11vibhav@gmail.com',
     url='https://github.com/jayavibhavnk/GraphRetrieval',
     packages=find_packages(),
```

