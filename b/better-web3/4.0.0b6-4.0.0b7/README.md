# Comparing `tmp/better_web3-4.0.0b6.tar.gz` & `tmp/better_web3-4.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-4.0.0b6.tar", max compression
+gzip compressed data, was "better_web3-4.0.0b7.tar", max compression
```

## Comparing `better_web3-4.0.0b6.tar` & `better_web3-4.0.0b7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b6/better_web3/__init__.py
--rw-r--r--   0        0        0     1706 2024-05-25 06:30:15.222893 better_web3-4.0.0b6/better_web3/caip_2.py
--rw-r--r--   0        0        0    11093 2024-05-25 07:08:34.914763 better_web3-4.0.0b6/better_web3/chain.py
--rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b6/better_web3/contract.py
--rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b6/better_web3/models.py
--rw-r--r--   0        0        0      137 2024-05-25 06:19:06.436481 better_web3-4.0.0b6/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b6/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      286 2024-05-25 06:27:06.720178 better_web3-4.0.0b6/better_web3/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b6/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0      885 2024-05-25 06:27:06.721182 better_web3-4.0.0b6/better_web3/utils/__pycache__/eth.cpython-312.pyc
--rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b6/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0      707 2024-05-25 06:27:06.721687 better_web3-4.0.0b6/better_web3/utils/__pycache__/other.cpython-312.pyc
--rw-r--r--   0        0        0      434 2024-05-25 06:19:06.433481 better_web3-4.0.0b6/better_web3/utils/eth.py
--rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b6/better_web3/utils/other.py
--rw-r--r--   0        0        0      521 2024-05-25 07:09:09.142412 better_web3-4.0.0b6/pyproject.toml
--rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b6/README.md
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b7/better_web3/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-25 06:30:15.222893 better_web3-4.0.0b7/better_web3/caip_2.py
+-rw-r--r--   0        0        0    11063 2024-05-25 08:31:44.153820 better_web3-4.0.0b7/better_web3/chain.py
+-rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b7/better_web3/contract.py
+-rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b7/better_web3/models.py
+-rw-r--r--   0        0        0      137 2024-05-25 06:19:06.436481 better_web3-4.0.0b7/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b7/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      286 2024-05-25 06:27:06.720178 better_web3-4.0.0b7/better_web3/utils/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b7/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0      885 2024-05-25 06:27:06.721182 better_web3-4.0.0b7/better_web3/utils/__pycache__/eth.cpython-312.pyc
+-rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b7/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0      707 2024-05-25 06:27:06.721687 better_web3-4.0.0b7/better_web3/utils/__pycache__/other.cpython-312.pyc
+-rw-r--r--   0        0        0      434 2024-05-25 06:19:06.433481 better_web3-4.0.0b7/better_web3/utils/eth.py
+-rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b7/better_web3/utils/other.py
+-rw-r--r--   0        0        0      521 2024-05-25 08:32:06.323804 better_web3-4.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b7/README.md
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b7/PKG-INFO
```

### Comparing `better_web3-4.0.0b6/better_web3/caip_2.py` & `better_web3-4.0.0b7/better_web3/caip_2.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b6/better_web3/chain.py` & `better_web3-4.0.0b7/better_web3/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,15 @@
     ) -> dict[str: str]:  # dict[explorer_name: url]
         if not self.explorers:
             raise ValueError("No explorers")
 
         if isinstance(tx_hash, HexBytes):
             tx_hash = tx_hash.hex()
 
-        urls = {}
-        for explorer in self.explorers:
-            urls[explorer.name] = tx_url(explorer.url, tx_hash)
+        return {explorer.name: tx_url(explorer.url, tx_hash) for explorer in self.explorers}
 
     async def is_eip1559_supported(self) -> bool:
         """
         :return: True if EIP1559 is supported by the node, False otherwise
         """
         last_block = await self.eth.get_block("latest")
         return True if "baseFeePerGas" in last_block else False
@@ -219,15 +217,15 @@
         tx_params = await self._build_tx_base_params(gas, tx_params=tx_params)
         tx_params = await self._build_tx_fee_params(
             gas_price, max_fee_per_gas, max_priority_fee_per_gas, tx_params=tx_params)
         return await contract_function.build_transaction(tx_params)
 
     async def sign_and_send_tx(self, account: LocalAccount, tx: TxParams) -> HexStr:
         signed_tx = account.sign_transaction(tx)
-        tx_hash = await self.eth.send_raw_transaction(signed_tx.rawTransaction)
+        tx_hash = await self.eth.send_raw_transaction(signed_tx.raw_transaction)
         return HexStr(tx_hash.hex())
 
     async def execute_fn(
             self,
             account: LocalAccount,
             fn: AsyncContractFunction,
             **kwargs,
```

### Comparing `better_web3-4.0.0b6/better_web3/models.py` & `better_web3-4.0.0b7/better_web3/models.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b6/better_web3/utils/__pycache__/__init__.cpython-311.pyc` & `better_web3-4.0.0b7/better_web3/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b6/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-4.0.0b7/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b6/better_web3/utils/__pycache__/eth.cpython-312.pyc` & `better_web3-4.0.0b7/better_web3/utils/__pycache__/eth.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b6/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-4.0.0b7/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b6/better_web3/utils/__pycache__/other.cpython-312.pyc` & `better_web3-4.0.0b7/better_web3/utils/__pycache__/other.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b6/pyproject.toml` & `better_web3-4.0.0b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "better-web3"
-version = "4.0.0.b6"
+version = "4.0.0.b7"
 description = "Web3 stuff"
 authors = ["Alen <alen.kimov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/alenkimov/better_web3"
 packages = [{include = "better_web3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `better_web3-4.0.0b6/README.md` & `better_web3-4.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b6/PKG-INFO` & `better_web3-4.0.0b7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 4.0.0b6
+Version: 4.0.0b7
 Summary: Web3 stuff
 Home-page: https://github.com/alenkimov/better_web3
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

