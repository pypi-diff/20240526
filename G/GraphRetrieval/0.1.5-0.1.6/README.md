# Comparing `tmp/graphretrieval-0.1.5.tar.gz` & `tmp/graphretrieval-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphretrieval-0.1.5.tar", last modified: Mon May 20 10:09:37 2024, max compression
+gzip compressed data, was "graphretrieval-0.1.6.tar", last modified: Sun May 26 07:31:01 2024, max compression
```

## Comparing `graphretrieval-0.1.5.tar` & `graphretrieval-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:09:37.587110 graphretrieval-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:09:37.587110 graphretrieval-0.1.5/GraphRetrieval/
--rw-r--r--   0 runner    (1001) docker     (127)    25838 2024-05-20 10:09:33.000000 graphretrieval-0.1.5/GraphRetrieval/GraphRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-20 10:09:33.000000 graphretrieval-0.1.5/GraphRetrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:09:37.587110 graphretrieval-0.1.5/GraphRetrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-20 10:09:37.000000 graphretrieval-0.1.5/GraphRetrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-20 10:09:37.000000 graphretrieval-0.1.5/GraphRetrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:09:37.000000 graphretrieval-0.1.5/GraphRetrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-20 10:09:37.000000 graphretrieval-0.1.5/GraphRetrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 10:09:37.000000 graphretrieval-0.1.5/GraphRetrieval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-20 10:09:37.587110 graphretrieval-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-20 10:09:33.000000 graphretrieval-0.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:09:37.587110 graphretrieval-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-20 10:09:33.000000 graphretrieval-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/GraphRetrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)    24320 2024-05-26 07:30:56.000000 graphretrieval-0.1.6/GraphRetrieval/GraphRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-26 07:30:56.000000 graphretrieval-0.1.6/GraphRetrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/GraphRetrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 07:31:01.000000 graphretrieval-0.1.6/GraphRetrieval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-26 07:30:56.000000 graphretrieval-0.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:31:01.122630 graphretrieval-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-26 07:30:56.000000 graphretrieval-0.1.6/setup.py
```

### Comparing `graphretrieval-0.1.5/GraphRetrieval/GraphRetrieval.py` & `graphretrieval-0.1.6/GraphRetrieval/GraphRetrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 class GraphDocument(langchain_core.documents.base.Document):
     def __init__(self, page_content, metadata):
         super().__init__(page_content=page_content, metadata=metadata)
 
     def __repr__(self):
         return f"GraphDocument(page_content='{self.page_content}', metadata={self.metadata})"
     
-
 class GraphRAG():
     def __init__(self):
         self.graph = None
         self.documents = None
         self.embeddings = None
         self.embedding_model = "all-MiniLM-L6-v2"
         self.retrieval_model = "a_star"
@@ -83,25 +82,19 @@
         pre_documents = text_splitter.create_documents([text])
         documents = [GraphDocument(doc.page_content, doc.metadata) for doc in pre_documents]
 
         model = SentenceTransformer(self.embedding_model)
         embeddings = model.encode([doc.page_content for doc in documents])
         graph = nx.Graph()
 
-        def add_edges(i):
-            edges = []
+        for i in range(len(documents)):
             for j in range(i, len(documents)):
                 similarity = cosine_similarity([embeddings[i]], [embeddings[j]])
                 if similarity[0][0] > similarity_threshold:
-                    edges.append((i, j, similarity[0][0]))
-            return edges
-
-        edge_lists = Parallel(n_jobs=-1)(delayed(add_edges)(i) for i in range(len(documents)))
-        edges = [edge for edge_list in edge_lists for edge in edge_list]
-        graph.add_weighted_edges_from(edges)
+                    graph.add_edge(i, j, weight=similarity[0][0])
 
         self.graph = graph
         self.documents = documents
         self.embeddings = embeddings
 
         return graph, documents, embeddings
 
@@ -113,16 +106,17 @@
 
     def create_graphs_from_directory(self, directory_path, similarity_threshold=0):
         file_list = []
         overall_text = ""
         for file_name in os.listdir(directory_path):
             if file_name.endswith(".txt"):
                 file_path = os.path.join(directory_path, file_name)
-                temp_text = open(file_path, 'r').read()
-                overall_text = overall_text + "\n" + temp_text
+                with open(file_path, 'r') as file:
+                    temp_text = file.read()
+                overall_text += "\n" + temp_text
                 file_list.append((temp_text, file_name))
 
         self.graph, self.documents, self.embeddings = self.constructGraph(overall_text, similarity_threshold=similarity_threshold)
         print("Graph created Successfully!")
 
         return file_list
 
@@ -134,107 +128,95 @@
         similar_nodes = []
         for neighbor in graph.neighbors(current_node):
             neighbor_embedding = self.embeddings[neighbor]
             neighbor_similarity = cosine_similarity([query_embedding], [neighbor_embedding])[0][0]
             similar_nodes.append((neighbor, neighbor_similarity))
         return similar_nodes
 
-    def a_star_search_parallel(self, graph, documents, embeddings, query_text, k=5):
+    def a_star_search(self, graph, documents, embeddings, query_text, k=5):
         model = SentenceTransformer(self.embedding_model)
         query_embedding = model.encode([query_text])[0]
 
         pq = [(0, None, 0)]
         visited = set()
         similar_nodes = []
 
         while pq and len(similar_nodes) < k:
             _, current_node, similarity_so_far = heapq.heappop(pq)
 
             if current_node is not None:
                 similar_nodes.append((current_node, similarity_so_far))
 
-            compute_similarity_partial = delayed(self.compute_similarity)
-            results = Parallel(n_jobs=-1)(compute_similarity_partial(neighbor, graph, documents, query_embedding) for neighbor in (graph.neighbors(current_node) if current_node is not None else range(len(documents)-1)))
-
-            for result in results:
-                for neighbor, neighbor_similarity in result:
-                    if neighbor not in visited:
-                        priority = -neighbor_similarity
-                        heapq.heappush(pq, (priority, neighbor, similarity_so_far + neighbor_similarity))
-                        visited.add(neighbor)
+            neighbors = graph.neighbors(current_node) if current_node is not None else range(len(documents))
+            for neighbor in neighbors:
+                if neighbor not in visited:
+                    neighbor_embedding = embeddings[neighbor]
+                    neighbor_similarity = cosine_similarity([query_embedding], [neighbor_embedding])[0][0]
+                    priority = -neighbor_similarity
+                    heapq.heappush(pq, (priority, neighbor, similarity_so_far + neighbor_similarity))
+                    visited.add(neighbor)
 
         return similar_nodes
 
-    def nearest_neighbors_parallel(self, query_text, k=5):
-        model = SentenceTransformer('all-MiniLM-L6-v2')
+    def nearest_neighbors(self, query_text, k=5):
+        model = SentenceTransformer(self.embedding_model)
         query_embedding = model.encode([query_text])[0]
         similarities = cosine_similarity([query_embedding], self.embeddings)
         sorted_indices = sorted(range(len(similarities[0])), key=lambda x: -similarities[0][x])[:k]
-        similar_indices = Parallel(n_jobs=-1)(delayed(self._get_similarity)(i, similarities, sorted_indices) for i in range(k))
-        return similar_indices
+        return [(idx, similarities[0][idx]) for idx in sorted_indices]
 
-    def _get_similarity(self, i, similarities, sorted_indices):
-        idx = sorted_indices[i]
-        return idx, similarities[0][idx]
-
-    def nearest_neighbors_sklearn_parallel(self, embeddings, query_text, k=5):
-        model = SentenceTransformer('all-MiniLM-L6-v2')
+    def nearest_neighbors_sklearn(self, embeddings, query_text, k=5):
+        model = SentenceTransformer(self.embedding_model)
         query_embedding = model.encode([query_text])[0]
 
         nn_model = NearestNeighbors(n_neighbors=k, metric='cosine')
         nn_model.fit(embeddings)
 
         distances, indices = nn_model.kneighbors([query_embedding])
 
-        similar_indices = Parallel(n_jobs=-1)(delayed(self._get_similarity_sklearn)(i, distances, indices) for i in range(k))
-        return similar_indices
-
-    def _get_similarity_sklearn(self, i, distances, indices):
-        idx = indices[0][i]
-        return idx, 1 - distances[0][i]
+        return [(indices[0][i], 1 - distances[0][i]) for i in range(k)]
 
-    def greedy_bfs_search_parallel(self, query_text, k=5):
+    def greedy_bfs_search(self, query_text, k=5):
         model = SentenceTransformer(self.embedding_model)
         query_embedding = model.encode([query_text])[0]
 
         pq = PriorityQueue()
         pq.put((0, None, 0))
         visited = set()
         similar_nodes = []
 
         while not pq.empty() and len(similar_nodes) < k:
             _, current_node, similarity_so_far = pq.get()
 
             if current_node is not None:
                 similar_nodes.append((current_node, similarity_so_far))
 
-            compute_similarity_partial = delayed(self.compute_similarity)
-            results = Parallel(n_jobs=-1)(compute_similarity_partial(neighbor, self.graph, self.documents, query_embedding) for neighbor in (self.graph.neighbors(current_node) if current_node is not None else range(len(self.documents)-1)))
-
-            for result in results:
-                for neighbor, neighbor_similarity in result:
-                    if neighbor not in visited:
-                        priority = -neighbor_similarity
-                        pq.put((priority, neighbor, similarity_so_far + neighbor_similarity))
-                        visited.add(neighbor)
+            neighbors = self.graph.neighbors(current_node) if current_node is not None else range(len(self.documents))
+            for neighbor in neighbors:
+                if neighbor not in visited:
+                    neighbor_embedding = self.embeddings[neighbor]
+                    neighbor_similarity = cosine_similarity([query_embedding], [neighbor_embedding])[0][0]
+                    priority = -neighbor_similarity
+                    pq.put((priority, neighbor, similarity_so_far + neighbor_similarity))
+                    visited.add(neighbor)
 
         return similar_nodes
 
-    def similarity_search(self, query, retrieval_model="a_star", k = 5):
-        retrieval_model=self.retrieval_model
+    def similarity_search(self, query, retrieval_model="a_star", k=5):
+        retrieval_model = self.retrieval_model
         similar_nodes = []
 
         if retrieval_model == "a_star":
-            similar_indices = [index for index, _ in self.a_star_search_parallel(self.graph, self.documents, self.embeddings, query, k)]
+            similar_indices = [index for index, _ in self.a_star_search(self.graph, self.documents, self.embeddings, query, k)]
         elif retrieval_model == "nearest_neighbors":
-            similar_indices = [index for index, _ in self.nearest_neighbors_parallel(query, k)]
+            similar_indices = [index for index, _ in self.nearest_neighbors(query, k)]
         elif retrieval_model == "nearest_neighbors1":
-            similar_indices = [index for index, _ in self.nearest_neighbors_sklearn_parallel(self.embeddings, query, k)]
+            similar_indices = [index for index, _ in self.nearest_neighbors_sklearn(self.embeddings, query, k)]
         elif retrieval_model == "greedy":
-            similar_indices = [index for index, _ in self.greedy_bfs_search_parallel(query, k)]
+            similar_indices = [index for index, _ in self.greedy_bfs_search(query, k)]
 
         return [self.documents[index] for index in similar_indices]
 
     def queryLLM(self, query):
         similar_documents = self.similarity_search(query)
         full_text = "\n".join([doc.page_content for doc in similar_documents])
 
@@ -244,24 +226,23 @@
         query: {query}
         """
         ans = self.query_openai(prompt_template.format(context=full_text, query=query))
 
         return ans
 
     def query_openai(self, query):
-        client = OpenAI()
-        completion = client.chat.completions.create(
-            model="gpt-3.5-turbo-0125",
+        openai.api_key = "YOUR_OPENAI_API_KEY"
+        response = openai.ChatCompletion.create(
+            model="gpt-3.5-turbo",
             messages=[
                 {"role": "system", "content": "You are a helpful assistant"},
                 {"role": "user", "content": query}
-            ],
-            n=1
+            ]
         )
-        return(completion.choices[0].message.content)
+        return response['choices'][0]['message']['content']
 
     def save_db(self, file_path):
         with open(file_path, 'wb') as file:
             pickle.dump((self.graph, self.documents, self.embeddings), file)
             print("saved!")
 
     def load_db(self, file_path):
@@ -272,36 +253,31 @@
     def update_graph_with_new_text(self, new_text, similarity_threshold=0):
         new_documents = [GraphDocument(text, None) for text in new_text.split('\n\n')]
         model = SentenceTransformer(self.embedding_model)
         new_embeddings = model.encode([doc.page_content for doc in new_documents])
 
         if len(self.documents) > 0 and len(new_documents) > 0:
             similarity = cosine_similarity(self.embeddings, new_embeddings)
-            edges = [(i, j + len(self.documents), similarity[i][j]) for i in range(len(self.documents)) for j in range(len(new_documents))
-                    if similarity[i][j] > similarity_threshold]
-            self.graph.add_weighted_edges_from(edges)
+            for i in range(len(self.documents)):
+                for j in range(len(new_documents)):
+                    if similarity[i][j] > similarity_threshold:
+                        self.graph.add_edge(i, j + len(self.documents), weight=similarity[i][j])
 
-        def add_edges(i):
-            edges = []
+        for i in range(len(new_documents)):
             for j in range(i, len(new_documents)):
-                similarity = cosine_similarity([self.embeddings[i]], [new_embeddings[j]])
+                similarity = cosine_similarity([new_embeddings[i]], [new_embeddings[j]])
                 if similarity[0][0] > similarity_threshold:
-                    edges.append((i, j + len(self.documents), similarity[0][0]))
-            return edges
-
-        edge_lists = Parallel(n_jobs=-1)(delayed(add_edges)(i) for i in range(len(self.documents)))
-        edges = [edge for edge_list in edge_lists for edge in edge_list]
-        self.graph.add_weighted_edges_from(edges)
+                    self.graph.add_edge(i + len(self.documents), j + len(self.documents), weight=similarity[0][0])
 
         self.documents.extend(new_documents)
-        self.embeddings.extend(new_embeddings)
+        self.embeddings = np.vstack((self.embeddings, new_embeddings))
 
         return self.graph, self.documents, self.embeddings
 
-    def create_graph_from_pdf(self, pdf_file, similarity_threshold=0):
+    def create_graph_from_pdf(self, pdf_file, similarity_threshold=0, chunk_size = 1250, chunk_overlap = 100):
         with open(pdf_file, "rb") as f:
             pdf_reader = PyPDF2.PdfFileReader(f)
             num_pages = pdf_reader.numPages
             text = ""
             for page_num in range(num_pages):
                 text += pdf_reader.getPage(page_num).extractText()
         self.graph, self.documents, self.embeddings = self.constructGraph(text, similarity_threshold=similarity_threshold)
@@ -555,67 +531,59 @@
             documents = [GraphDocument(image, {"path": image}) for image in images]
         else:
             documents = [GraphDocument("Image Object", {"image": image}) for image in images]
         
         embeddings = [self.image_to_embedding(image) for image in images]
         graph = nx.Graph()
 
-        def add_edges(i):
-            edges = []
+        for i in range(len(documents)):
             for j in range(i, len(documents)):
                 similarity = cosine_similarity([embeddings[i]], [embeddings[j]])[0][0]
                 if similarity > similarity_threshold:
-                    edges.append((i, j, similarity))
-            return edges
-
-        edge_lists = Parallel(n_jobs=-1)(delayed(add_edges)(i) for i in range(len(documents)))
-        edges = [edge for edge_list in edge_lists for edge in edge_list]
-        graph.add_weighted_edges_from(edges)
+                    graph.add_edge(i, j, weight=similarity)
 
         self.graph = graph
         self.documents = documents
         self.embeddings = np.array(embeddings)
 
         return graph, documents, embeddings
 
-    def a_star_search_parallel(self, query_image_path, k=5):
+    def a_star_search(self, query_image_path, k=5):
         query_embedding = self.image_to_embedding(query_image_path)
         pq = [(0, None, 0)]
         visited = set()
         similar_nodes = []
 
         while pq and len(similar_nodes) < k:
             _, current_node, similarity_so_far = heapq.heappop(pq)
 
             if current_node is not None:
                 similar_nodes.append((current_node, similarity_so_far))
 
-            compute_similarity_partial = delayed(self.compute_similarity)
-            results = Parallel(n_jobs=-1)(compute_similarity_partial(neighbor, self.graph, query_embedding) for neighbor in (self.graph.neighbors(current_node) if current_node is not None else range(len(self.documents))))
-
-            for result in results:
-                for neighbor, neighbor_similarity in result:
-                    if neighbor not in visited:
-                        priority = -neighbor_similarity
-                        heapq.heappush(pq, (priority, neighbor, similarity_so_far + neighbor_similarity))
-                        visited.add(neighbor)
+            neighbors = self.graph.neighbors(current_node) if current_node is not None else range(len(self.documents))
+            for neighbor in neighbors:
+                if neighbor not in visited:
+                    neighbor_similarity = self.compute_similarity(neighbor, query_embedding)
+                    priority = -neighbor_similarity
+                    heapq.heappush(pq, (priority, neighbor, similarity_so_far + neighbor_similarity))
+                    visited.add(neighbor)
 
         return similar_nodes
 
-    def compute_similarity(self, neighbor, graph, query_embedding):
+    def compute_similarity(self, neighbor, query_embedding):
         neighbor_embedding = self.embeddings[neighbor]
         neighbor_similarity = cosine_similarity([query_embedding], [neighbor_embedding])[0][0]
-        return [(neighbor, neighbor_similarity)]
+        return neighbor_similarity
 
     def similarity_search(self, query_image_path, retrieval_model="a_star", k=5):
         retrieval_model=self.retrieval_model
         similar_nodes = []
 
         if retrieval_model == "a_star":
-            similar_indices = [index for index, _ in self.a_star_search_parallel(query_image_path, k)]
+            similar_indices = [index for index, _ in self.a_star_search(query_image_path, k)]
 
         return [self.documents[index] for index in similar_indices]
 
     def save_db(self, file_path):
         with open(file_path, 'wb') as file:
             pickle.dump((self.graph, self.documents, self.embeddings), file)
             print("saved!")
@@ -635,8 +603,9 @@
             raise ValueError("Either directory_path or images must be provided.")
         print("Graph created Successfully!")
         return self.documents
         
     def visualize_graph(self):
         pos = nx.spring_layout(self.graph)
         nx.draw(self.graph, pos, with_labels=True, node_color='skyblue', edge_color='gray', node_size=1000, font_size=10)
-        plt.show() ## use matplotlib
+        plt.show()
+
```

### Comparing `graphretrieval-0.1.5/GraphRetrieval.egg-info/PKG-INFO` & `graphretrieval-0.1.6/GraphRetrieval.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.5
+Version: 0.1.6
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
@@ -152,15 +152,15 @@
     print(doc.metadata["path"])
 ```
 
 ```python
 image_graph_rag.visualize_graph() # for graph visualization
 ```
 
-
+### Note: This is a new version without parallelization, use 0.1.5>= for parallelization.
 
 #### Contributing
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss what you would like to change.
 License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `graphretrieval-0.1.5/PKG-INFO` & `graphretrieval-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.5
+Version: 0.1.6
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
@@ -152,15 +152,15 @@
     print(doc.metadata["path"])
 ```
 
 ```python
 image_graph_rag.visualize_graph() # for graph visualization
 ```
 
-
+### Note: This is a new version without parallelization, use 0.1.5>= for parallelization.
 
 #### Contributing
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss what you would like to change.
 License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `graphretrieval-0.1.5/README.rst` & `graphretrieval-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `graphretrieval-0.1.5/setup.py` & `graphretrieval-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,29 +133,29 @@
     print(doc.metadata["path"])
 ```
 
 ```python
 image_graph_rag.visualize_graph() # for graph visualization
 ```
 
-
+### Note: This is a new version without parallelization, use 0.1.5>= for parallelization.
 
 #### Contributing
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss what you would like to change.
 License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 This `README.md` provides an overview of the GraphRetrieval library, installation instructions, and example usage scenarios, with the specified changes to the file path and environment variables sections.
 """
 
 setup(
     name='GraphRetrieval',
-    version='0.1.5',
+    version='0.1.6',
     description='Graph retrieval',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='JVNK',
     author_email='jaya11vibhav@gmail.com',
     url='https://github.com/jayavibhavnk/GraphRetrieval',
     packages=find_packages(),
```

