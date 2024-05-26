# Comparing `tmp/dreamai-2.0.4.tar.gz` & `tmp/dreamai-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-2.0.4.tar", max compression
+gzip compressed data, was "dreamai-2.0.6.tar", max compression
```

## Comparing `dreamai-2.0.4.tar` & `dreamai-2.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.4/dreamai/__init__.py
--rw-r--r--   0        0        0     3087 2024-04-04 19:47:26.432580 dreamai-2.0.4/dreamai/ai.py
--rw-r--r--   0        0        0     5999 2024-04-08 16:29:05.217116 dreamai-2.0.4/dreamai/chroma.py
--rw-r--r--   0        0        0     1881 2024-04-04 18:10:25.180688 dreamai-2.0.4/dreamai/pdf.py
--rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0.4/dreamai/templates.py
--rw-r--r--   0        0        0     5693 2024-04-03 18:34:42.550727 dreamai-2.0.4/dreamai/utils.py
--rw-r--r--   0        0        0      797 2024-04-09 15:05:57.386874 dreamai-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 dreamai-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.6/dreamai/__init__.py
+-rw-r--r--   0        0        0     3765 2024-05-26 03:29:34.217009 dreamai-2.0.6/dreamai/ai.py
+-rw-r--r--   0        0        0     6127 2024-05-11 13:59:15.167712 dreamai-2.0.6/dreamai/chroma.py
+-rw-r--r--   0        0        0     1897 2024-05-08 13:31:52.980653 dreamai-2.0.6/dreamai/pdf.py
+-rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0.6/dreamai/templates.py
+-rw-r--r--   0        0        0    12777 2024-05-01 13:37:33.386393 dreamai-2.0.6/dreamai/utils.py
+-rw-r--r--   0        0        0     1578 2024-05-26 11:19:43.950898 dreamai-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 dreamai-2.0.6/PKG-INFO
```

### Comparing `dreamai-2.0.4/dreamai/chroma.py` & `dreamai-2.0.6/dreamai/chroma.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 from typing import Callable
 from uuid import uuid4
 
 import chromadb
 import torch
 from chromadb import Collection as ChromaCollection
+from chromadb.api.types import Include, QueryResult, GetResult
 from chromadb.utils.embedding_functions import SentenceTransformerEmbeddingFunction
 from langchain_core.documents import Document as LCDocument
 from sentence_transformers import CrossEncoder
 from termcolor import colored
 
 CHROMA_EMBEDDING_MODEL = "multi-qa-mpnet-base-cos-v1"
 CHROMA_DIR = "chroma_dir"
@@ -32,15 +33,16 @@
         except Exception as e:
             print(colored(f"Error deleting collection named {name}: {e}", "red"))
             pass
     embedding_function = SentenceTransformerEmbeddingFunction(
         model_name=embedding_model, device=device
     )
     collection = chroma_client.get_or_create_collection(
-        name, embedding_function=embedding_function
+        name,
+        embedding_function=embedding_function,  # type: ignore
     )
     return collection
 
 
 def json_files_to_collection(
     flist: list[str | Path], chroma_collection: ChromaCollection
 ):
@@ -56,15 +58,15 @@
                     "level": data["level"],
                     "type": data["type"],
                     "prev_id": "",
                     "next_id": "",
                 }
             )
             docs.append(json.dumps(data))
-    print(colored(f"Adding {i} files to collection", "cyan"))
+    # print(colored(f"Adding {i} files to collection", "cyan"))
     chroma_collection.add(ids=ids, documents=docs, metadatas=metas)
 
 
 def id_from_lc_doc(doc: LCDocument, doc_idx=None, **kwargs) -> str | None:
     try:
         file_name = doc.metadata.get("filename", doc.metadata.get("source"))
         doc_id = file_name or ""
@@ -79,15 +81,15 @@
         return None
 
 
 def lc_docs_to_chroma_docs(
     docs: list[LCDocument],
     id_fn: Callable = id_from_lc_doc,
     add_links: bool = True,
-) -> tuple[list[str], list[str], list[dict]]:
+) -> dict:
     chroma_ids = []
     chroma_docs = []
     chroma_metadatas = []
     for i, doc in enumerate(docs):
         chroma_ids.append(id_fn(doc=doc, doc_idx=i) or f"id_{i}")
         chroma_docs.append(doc.page_content)
     for i, doc in enumerate(docs):
@@ -107,16 +109,16 @@
     id: str,
     collection: ChromaCollection,
     direction: str = "prev",
     n_steps: int = 2,
 ) -> list:
     ids = []
     for _ in range(n_steps):
-        metadata = collection.get(ids=[id])["metadatas"][0]
-        id = metadata.get(f"{direction}_id", "")
+        metadata = collection.get(ids=[id])["metadatas"][0]  # type: ignore
+        id = metadata.get(f"{direction}_id", "")  # type: ignore
         if not id:
             break
         ids.append(id)
     return ids
 
 
 def traverse_ids(
@@ -143,36 +145,37 @@
         )
         res_ids.append(prev_ids[::-1] + [id] + next_ids)
     return res_ids
 
 
 def rerank_chroma_results(
     query_text: str,
-    results: dict,
+    results: QueryResult,
     cross_encoder_model: str = CROSS_ENCODER_MODEL,
 ) -> dict:
     device = "cuda" if torch.cuda.is_available() else "cpu"
     cross_encoder = CrossEncoder(cross_encoder_model, device=device)
-    pairs = [[query_text, doc] for doc in results["documents"][0]]
+    pairs = [[query_text, doc] for doc in results["documents"][0]]  # type: ignore
     scores = cross_encoder.predict(pairs)
-    scores_idx = sorted(range(len(scores)), key=lambda i: scores[i], reverse=True)
-    results = {k: [[v[0][i] for i in scores_idx]] for k, v in results.items() if v}
-    return results
+    scores_idx = sorted(
+        range(len(scores)), key=lambda i: scores[i].item(), reverse=True
+    )
+    return {k: [[v[0][i] for i in scores_idx]] for k, v in results.items() if v}  # type: ignore
 
 
 def query_collection(
     query_text: str,
     collection: ChromaCollection,
     n_results: int = 10,
     rerank_results: bool = False,
     n_prev_links: int = 2,
     n_next_links: int = 2,
-    include: list[str] = ["metadatas", "documents"],
+    include: Include = ["metadatas", "documents"],
     reranker_model: str = CROSS_ENCODER_MODEL,
-) -> tuple[list[dict], list[str]]:
+) -> tuple[list[GetResult], list[str]]:
     query_res = collection.query(
         query_texts=query_text, n_results=n_results, include=include
     )
     if rerank_results:
         query_res = rerank_chroma_results(
             query_text=query_text,
             results=query_res,
```

### Comparing `dreamai-2.0.4/dreamai/pdf.py` & `dreamai-2.0.6/dreamai/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from chromadb import Collection as ChromaCollection
 from langchain.text_splitter import RecursiveCharacterTextSplitter
-from langchain_community.document_loaders import PyPDFLoader
+from langchain_community.document_loaders import PyPDFLoader  # type: ignore
 from langchain_core.documents import Document as LCDocument
 
 from .chroma import (
     CHROMA_DEVICE,
     CHROMA_DIR,
     CHROMA_EMBEDDING_MODEL,
     chroma_collection,
```

### Comparing `dreamai-2.0.4/dreamai/templates.py` & `dreamai-2.0.6/dreamai/templates.py`

 * *Files identical despite different names*

