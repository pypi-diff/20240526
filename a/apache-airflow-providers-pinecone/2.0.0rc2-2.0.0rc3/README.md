# Comparing `tmp/apache_airflow_providers_pinecone-2.0.0rc2.tar.gz` & `tmp/apache_airflow_providers_pinecone-2.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_pinecone-2.0.0rc2.tar", last modified: Fri May 10 23:41:08 2024, max compression
+gzip compressed data, was "apache_airflow_providers_pinecone-2.0.0rc3.tar", last modified: Fri May 10 23:41:08 2024, max compression
```

## Comparing `apache_airflow_providers_pinecone-2.0.0rc2.tar` & `apache_airflow_providers_pinecone-2.0.0rc3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3087 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/README.rst
--rw-r--r--   0        0        0    13569 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/LICENSE
--rw-r--r--   0        0        0     1495 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/__init__.py
--rw-r--r--   0        0        0     2351 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/hooks/__init__.py
--rw-r--r--   0        0        0    14884 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/hooks/pinecone.py
--rw-r--r--   0        0        0      785 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/operators/__init__.py
--rw-r--r--   0        0        0     7564 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/operators/pinecone.py
--rw-r--r--   0        0        0     2985 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 apache_airflow_providers_pinecone-2.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     3087 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc3/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/LICENSE
+-rw-r--r--   0        0        0     1495 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/__init__.py
+-rw-r--r--   0        0        0     2351 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/hooks/__init__.py
+-rw-r--r--   0        0        0    14946 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/hooks/pinecone.py
+-rw-r--r--   0        0        0      785 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/operators/__init__.py
+-rw-r--r--   0        0        0     7608 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/operators/pinecone.py
+-rw-r--r--   0        0        0     2985 2024-05-10 23:41:08.000000 apache_airflow_providers_pinecone-2.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     4795 1970-01-01 00:00:00.000000 apache_airflow_providers_pinecone-2.0.0rc3/PKG-INFO
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/README.rst` & `apache_airflow_providers_pinecone-2.0.0rc3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pinecone``
 
-Release: ``2.0.0.rc2``
+Release: ``2.0.0.rc3``
 
 
 `Pinecone <https://docs.pinecone.io/docs/overview>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/LICENSE` & `apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/__init__.py` & `apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/get_provider_info.py` & `apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/hooks/__init__.py` & `apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/hooks/pinecone.py` & `apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/hooks/pinecone.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from typing import TYPE_CHECKING, Any
 
 from pinecone import Pinecone, PodSpec, ServerlessSpec
 
 from airflow.hooks.base import BaseHook
 
 if TYPE_CHECKING:
+    from pinecone import Vector
     from pinecone.core.client.model.sparse_values import SparseValues
     from pinecone.core.client.models import DescribeIndexStatsResponse, QueryResponse, UpsertResponse
 
     from airflow.models.connection import Connection
 
 
 class PineconeHook(BaseHook):
@@ -133,15 +134,15 @@
     def list_indexes(self) -> Any:
         """Retrieve a list of all indexes in your project."""
         return self.pinecone_client.list_indexes()
 
     def upsert(
         self,
         index_name: str,
-        vectors: list[Any],
+        vectors: list[Vector] | list[tuple] | list[dict],
         namespace: str = "",
         batch_size: int | None = None,
         show_progress: bool = True,
         **kwargs: Any,
     ) -> UpsertResponse:
         """
         Write vectors into a namespace.
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/operators/__init__.py` & `apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/airflow/providers/pinecone/operators/pinecone.py` & `apache_airflow_providers_pinecone-2.0.0rc3/airflow/providers/pinecone/operators/pinecone.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,42 +21,44 @@
 from typing import TYPE_CHECKING, Any, Sequence
 
 from airflow.models import BaseOperator
 from airflow.providers.pinecone.hooks.pinecone import PineconeHook
 from airflow.utils.context import Context
 
 if TYPE_CHECKING:
+    from pinecone import Vector
+
     from airflow.utils.context import Context
 
 
 class PineconeIngestOperator(BaseOperator):
     """
     Ingest vector embeddings into Pinecone.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:PineconeIngestOperator`
 
     :param conn_id: The connection id to use when connecting to Pinecone.
     :param index_name: Name of the Pinecone index.
-    :param input_vectors: Data to be ingested, in the form of a list of tuples where each tuple
-        contains (id, vector_embedding, metadata).
+    :param input_vectors: Data to be ingested, in the form of a list of vectors, list of tuples,
+        or list of dictionaries.
     :param namespace: The namespace to write to. If not specified, the default namespace is used.
     :param batch_size: The number of vectors to upsert in each batch.
     :param upsert_kwargs: .. seealso:: https://docs.pinecone.io/reference/upsert
     """
 
     template_fields: Sequence[str] = ("index_name", "input_vectors", "namespace")
 
     def __init__(
         self,
         *,
         conn_id: str = PineconeHook.default_conn_name,
         index_name: str,
-        input_vectors: list[tuple],
+        input_vectors: list[Vector] | list[tuple] | list[dict],
         namespace: str = "",
         batch_size: int | None = None,
         upsert_kwargs: dict | None = None,
         **kwargs: Any,
     ) -> None:
         self.upsert_kwargs = upsert_kwargs or {}
         super().__init__(**kwargs)
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/pyproject.toml` & `apache_airflow_providers_pinecone-2.0.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-pinecone"
-version = "2.0.0.rc2"
+version = "2.0.0.rc3"
 description = "Provider package apache-airflow-providers-pinecone for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
```

### Comparing `apache_airflow_providers_pinecone-2.0.0rc2/PKG-INFO` & `apache_airflow_providers_pinecone-2.0.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pinecone
-Version: 2.0.0rc2
+Version: 2.0.0rc3
 Summary: Provider package apache-airflow-providers-pinecone for Apache Airflow
 Keywords: airflow-provider,pinecone,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pinecone``
 
-Release: ``2.0.0.rc2``
+Release: ``2.0.0.rc3``
 
 
 `Pinecone <https://docs.pinecone.io/docs/overview>`__
 
 
 Provider package
 ----------------
```

