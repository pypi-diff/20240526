# Comparing `tmp/better_web3-4.0.0b7.tar.gz` & `tmp/better_web3-4.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-4.0.0b7.tar", max compression
+gzip compressed data, was "better_web3-4.0.0b8.tar", max compression
```

## Comparing `better_web3-4.0.0b7.tar` & `better_web3-4.0.0b8.tar`

### file list

```diff
@@ -1,17 +1,9 @@
--rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b7/better_web3/__init__.py
--rw-r--r--   0        0        0     1706 2024-05-25 06:30:15.222893 better_web3-4.0.0b7/better_web3/caip_2.py
--rw-r--r--   0        0        0    11063 2024-05-25 08:31:44.153820 better_web3-4.0.0b7/better_web3/chain.py
--rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b7/better_web3/contract.py
--rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b7/better_web3/models.py
--rw-r--r--   0        0        0      137 2024-05-25 06:19:06.436481 better_web3-4.0.0b7/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b7/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      286 2024-05-25 06:27:06.720178 better_web3-4.0.0b7/better_web3/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b7/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0      885 2024-05-25 06:27:06.721182 better_web3-4.0.0b7/better_web3/utils/__pycache__/eth.cpython-312.pyc
--rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b7/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0      707 2024-05-25 06:27:06.721687 better_web3-4.0.0b7/better_web3/utils/__pycache__/other.cpython-312.pyc
--rw-r--r--   0        0        0      434 2024-05-25 06:19:06.433481 better_web3-4.0.0b7/better_web3/utils/eth.py
--rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b7/better_web3/utils/other.py
--rw-r--r--   0        0        0      521 2024-05-25 08:32:06.323804 better_web3-4.0.0b7/pyproject.toml
--rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b7/README.md
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0      236 2024-05-26 06:57:16.536588 better_web3-4.0.0b8/better_web3/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-25 06:30:15.222893 better_web3-4.0.0b8/better_web3/caip_2.py
+-rw-r--r--   0        0        0    11063 2024-05-25 08:31:44.153820 better_web3-4.0.0b8/better_web3/chain.py
+-rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b8/better_web3/contract.py
+-rw-r--r--   0        0        0     1057 2024-05-26 06:51:13.939678 better_web3-4.0.0b8/better_web3/models.py
+-rw-r--r--   0        0        0      343 2024-05-26 06:57:16.529867 better_web3-4.0.0b8/better_web3/utils.py
+-rw-r--r--   0        0        0      521 2024-05-26 06:57:28.235630 better_web3-4.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b8/README.md
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b8/PKG-INFO
```

### Comparing `better_web3-4.0.0b7/better_web3/caip_2.py` & `better_web3-4.0.0b8/better_web3/caip_2.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b7/better_web3/chain.py` & `better_web3-4.0.0b8/better_web3/chain.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b7/better_web3/models.py` & `better_web3-4.0.0b8/better_web3/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from pydantic import BaseModel, Field
+from eth_typing import HexStr
 
 
 class Explorer(BaseModel):
     name: str
     url: str
     standard: str
     # icon: str | None = None
 
+    def tx_url(self, tx_hash: HexStr | str):
+        return f"{self.url}/tx/0x{tx_hash}"
+
 
 class NativeCurrency(BaseModel):
     name: str = "Ether"
     symbol: str = "ETH"
     decimals: int = 18
```

### Comparing `better_web3-4.0.0b7/pyproject.toml` & `better_web3-4.0.0b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "better-web3"
-version = "4.0.0.b7"
+version = "4.0.0.b8"
 description = "Web3 stuff"
 authors = ["Alen <alen.kimov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/alenkimov/better_web3"
 packages = [{include = "better_web3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `better_web3-4.0.0b7/README.md` & `better_web3-4.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b7/PKG-INFO` & `better_web3-4.0.0b8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 4.0.0b7
+Version: 4.0.0b8
 Summary: Web3 stuff
 Home-page: https://github.com/alenkimov/better_web3
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

