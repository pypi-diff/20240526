# Comparing `tmp/kvalchemy-0.0.7.tar.gz` & `tmp/kvalchemy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvalchemy-0.0.7.tar", last modified: Sat May 18 20:50:22 2024, max compression
+gzip compressed data, was "kvalchemy-0.0.8.tar", last modified: Sat May 25 23:51:49 2024, max compression
```

## Comparing `kvalchemy-0.0.7.tar` & `kvalchemy-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:22.280685 kvalchemy-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-18 20:50:22.280685 kvalchemy-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:22.276685 kvalchemy-0.0.7/kvalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/kvalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/kvalchemy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/kvalchemy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/kvalchemy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/kvalchemy/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/kvalchemy/values.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:22.280685 kvalchemy-0.0.7/kvalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-18 20:50:22.000000 kvalchemy-0.0.7/kvalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-18 20:50:22.000000 kvalchemy-0.0.7/kvalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:50:22.000000 kvalchemy-0.0.7/kvalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 20:50:22.000000 kvalchemy-0.0.7/kvalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-18 20:50:22.000000 kvalchemy-0.0.7/kvalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:50:22.280685 kvalchemy-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:50:22.280685 kvalchemy-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8669 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-18 20:50:14.000000 kvalchemy-0.0.7/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:51:49.859967 kvalchemy-0.0.8/kvalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/kvalchemy/values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/kvalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 23:51:49.000000 kvalchemy-0.0.8/kvalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:51:49.863967 kvalchemy-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-25 23:51:39.000000 kvalchemy-0.0.8/tests/test_time.py
```

### Comparing `kvalchemy-0.0.7/LICENSE.md` & `kvalchemy-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.7/PKG-INFO` & `kvalchemy-0.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.7
+Version: 0.0.8
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,19 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: backoff
 Requires-Dist: sqlalchemy
+Provides-Extra: dev
+Requires-Dist: PyMySQL[rsa]; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # KVAlchemy
 
 KVAlchemy is a SQLAlchemy-based key-vault store. It has the ability to get/set values based off a string key, an optional string tag, and an optional expiration time. Additionally it has a built-in ability to memoize function results to the store.
 
 ## Example
```

### Comparing `kvalchemy-0.0.7/README.md` & `kvalchemy-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.7/kvalchemy/client.py` & `kvalchemy-0.0.8/kvalchemy/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 """
 Home to the KVAlchemy client.
 """
 import contextlib
 import logging
 from typing import Any, Callable, Iterable, Union
 
+import backoff
 from sqlalchemy import create_engine
+from sqlalchemy.exc import IntegrityError
 from sqlalchemy.orm import Session, scoped_session, sessionmaker
 
 from kvalchemy.models import KEY_MAX_LENGTH, TAG_MAX_LENGTH, Base, KVStore, ValueMixIn
 from kvalchemy.proxy import Proxy
 from kvalchemy.time import ExpirationType, to_expire
 from kvalchemy.values import ENOVAL
 
 log = logging.getLogger(__name__)
 
-MEMOIZE_TAG = "__memoize__"
+
+retry_integrity_errors = backoff.on_exception(
+    backoff.constant, IntegrityError, interval=0.1, max_time=30
+)
 
 
 class KVAlchemy:
     """
     Client for working with the key-value store.
     """
 
@@ -72,21 +77,27 @@
         If delete_expired is True, any expired keys will be deleted before exiting the block.
             Note that delete_expired only applies if commit is True.
         """
         with self._session() as session:
             yield session
 
             if commit:
+                # End the user's session via commit.
+                session.commit()
+
                 if delete_expired:
+                    # Now we're starting a new transaction to delete expired keys.
                     session.query(KVStore).filter(
                         ~KVStore.non_expired_filter()
                     ).delete()
 
-                session.commit()
+                    # commit the delete transaction
+                    session.commit()
 
+    @retry_integrity_errors
     def get(
         self,
         key: str,
         default: Any = ENOVAL,
         tag: str = "",
         return_expiration: bool = False,
     ) -> Any:
@@ -113,28 +124,30 @@
                 raise KeyError(f"key: {key}, tag: {tag}")
 
             if return_expiration:
                 return result.value, getattr(result, "expire", None)
 
             return result.value
 
+    @retry_integrity_errors
     def set(
         self, key: str, value: Any, tag: str = "", expire: ExpirationType = None
     ) -> None:
         """
         Sets the given key/tag combo to the value provided.
 
         If expire is provided, it must be something that can be processed by
         the to_expire function in kvalchemy.time.
         """
         with self.session() as session:
             session.merge(
                 KVStore(key=key, value=value, tag=tag, expire=to_expire(expire))
             )
 
+    @retry_integrity_errors
     def delete(self, key: str, tag: str = "") -> None:
         """
         Deletes the given key/tag combo from the store.
         """
         with self.session() as session:
             query = (
                 session.query(KVStore)
@@ -162,27 +175,29 @@
             else:
                 value = default
 
         self.delete(key, tag)
 
         return value
 
+    @retry_integrity_errors
     def clear(self) -> None:
         """
         Clears all key-value pairs from the store.
         """
         with self.session() as session:
             session.query(KVStore).delete()
 
     def get_proxy(self, key: str, default: Any = ENOVAL, tag: str = "") -> Proxy:
         """
         Returns a Proxy object for the given key, tag, default.
         """
         return Proxy(self, key, default, tag)
 
+    @retry_integrity_errors
     def delete_tag(self, tag: str) -> int:
         """
         Deletes all keys under a given tag.
 
         Returns the number of keys deleted.
         """
         with self.session() as session:
```

### Comparing `kvalchemy-0.0.7/kvalchemy/models.py` & `kvalchemy-0.0.8/kvalchemy/models.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.7/kvalchemy/proxy.py` & `kvalchemy-0.0.8/kvalchemy/proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.7/kvalchemy/time.py` & `kvalchemy-0.0.8/kvalchemy/time.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.7/kvalchemy.egg-info/PKG-INFO` & `kvalchemy-0.0.8/kvalchemy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvalchemy
-Version: 0.0.7
+Version: 0.0.8
 Summary: A SQLAlchemy based Key-Value store.
 Author-email: csm10495 <csm10495@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/csm10495/kvalchemy
 Project-URL: repository, https://github.com/csm10495/kvalchemy
 Project-URL: documentation, https://csm10495.github.io/kvalchemy
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,19 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: backoff
 Requires-Dist: sqlalchemy
+Provides-Extra: dev
+Requires-Dist: PyMySQL[rsa]; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 # KVAlchemy
 
 KVAlchemy is a SQLAlchemy-based key-vault store. It has the ability to get/set values based off a string key, an optional string tag, and an optional expiration time. Additionally it has a built-in ability to memoize function results to the store.
 
 ## Example
```

### Comparing `kvalchemy-0.0.7/pyproject.toml` & `kvalchemy-0.0.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -9,33 +9,39 @@
     "Natural Language :: English",
     "Operating System :: POSIX",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">=3.8"
-dependencies = ['sqlalchemy']
+dependencies = ["backoff", 'sqlalchemy']
 
 [project.urls]
 homepage = "https://github.com/csm10495/kvalchemy"
 repository = "https://github.com/csm10495/kvalchemy"
 documentation  = "https://csm10495.github.io/kvalchemy"
 
+[project.optional-dependencies]
+dev = [
+    "PyMySQL[rsa]",
+    "pytest"
+]
+
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [tool.setuptools]
 packages = ["kvalchemy"]
 include-package-data = true
 
 [tool.setuptools.dynamic]
 version = {attr = "kvalchemy.__version__"}
 
 [tool.pytest.ini_options]
 pythonpath = [
-  "."
+    "."
 ]
 
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
```

### Comparing `kvalchemy-0.0.7/tests/test_client.py` & `kvalchemy-0.0.8/tests/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+from concurrent.futures import ThreadPoolExecutor
 from datetime import datetime, timedelta
 from unittest.mock import patch
 from uuid import UUID, uuid4
 
 import pytest
 
 from kvalchemy import KVAlchemy
@@ -69,14 +70,35 @@
 
     with kvalchemy.session() as session:
         result = session.query(KVStore).filter_by(key="key", tag="").one()
         assert result.value == "value"
         assert session.query(KVStore).count() == 1
 
 
+def test_session_access_thrash(kvalchemy):
+    if "sqlite" in kvalchemy.url:
+        pytest.skip("sqlite backend doesn't support multiple accesses at once")
+
+    kva = KVAlchemy(kvalchemy.url)
+
+    def thrash(kva):
+        for i in range(10):
+            kva.set("key", i)
+
+    futures = []
+    with ThreadPoolExecutor() as executor:
+        for _ in range(100):
+            futures.append(executor.submit(thrash, kva))
+
+        for f in futures:
+            f.result()
+
+    assert kva.get("key") == 9
+
+
 def test_session_commit_false(kvalchemy, kvstore):
     with kvalchemy.session(commit=False) as session:
         session.add(kvstore)
 
     with kvalchemy.session() as session:
         result = session.query(KVStore).filter_by(key="key", tag="").one_or_none()
         assert result is None
@@ -126,15 +148,15 @@
     kvalchemy.set("key", "value3")
     assert kvalchemy.get("key") == "value3"
     assert kvalchemy.get("key", tag="tag") == "value2"
 
 
 def test_set_get_with_expire(kvalchemy):
     kvalchemy.set("key", "value", expire=0)
-    time.sleep(0.1)
+    time.sleep(0.5)
     assert kvalchemy.get("key", "default") == "default"
 
     kvalchemy.set("key", "value", expire=datetime(9999, 2, 2))
     assert kvalchemy.get("key", return_expiration=True) == (
         "value",
         datetime(9999, 2, 2),
     )
@@ -274,22 +296,22 @@
     ret_val = False
     assert x() == True
     x.cache_clear()
     assert x() == False
 
     ret_val = True
 
-    @kvalchemy.memoize(expire=0.001)
+    @kvalchemy.memoize(expire=0.0001)
     def y():
         global ret_val
         return ret_val
 
     assert y() == True
     ret_val = False
-    time.sleep(0.1)
+    time.sleep(0.5)
     assert y() == False
 
 
 def test_memoize_expire_if(kvalchemy):
     @kvalchemy.memoize(expire_if=True)
     def x():
         return uuid4()
```

### Comparing `kvalchemy-0.0.7/tests/test_proxy.py` & `kvalchemy-0.0.8/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `kvalchemy-0.0.7/tests/test_time.py` & `kvalchemy-0.0.8/tests/test_time.py`

 * *Files identical despite different names*

