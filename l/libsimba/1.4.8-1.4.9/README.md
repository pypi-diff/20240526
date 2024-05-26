# Comparing `tmp/libsimba-1.4.8.tar.gz` & `tmp/libsimba-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsimba-1.4.8.tar", max compression
+gzip compressed data, was "libsimba-1.4.9.tar", max compression
```

## Comparing `libsimba-1.4.8.tar` & `libsimba-1.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1099 2023-03-19 19:21:39.908933 libsimba-1.4.8/LICENSE
--rw-r--r--   0        0        0     6148 2022-08-29 12:51:26.796404 libsimba-1.4.8/libsimba/.DS_Store
--rw-r--r--   0        0        0     1529 2024-03-07 08:24:18.582108 libsimba-1.4.8/libsimba/__init__.py
--rw-r--r--   0        0        0     1988 2024-03-09 09:43:42.012788 libsimba-1.4.8/libsimba/auth/__init__.py
--rw-r--r--   0        0        0    10547 2023-09-29 17:13:22.513991 libsimba-1.4.8/libsimba/auth/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1294 2024-03-09 09:43:44.166035 libsimba-1.4.8/libsimba/auth/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1425 2024-03-09 09:47:07.552095 libsimba-1.4.8/libsimba/auth/__pycache__/apikey.cpython-39.pyc
--rw-r--r--   0        0        0    10004 2024-03-07 10:02:50.833460 libsimba-1.4.8/libsimba/auth/__pycache__/client_credentials.cpython-39.pyc
--rw-r--r--   0        0        0     1381 2024-03-07 10:07:58.051055 libsimba-1.4.8/libsimba/auth/apikey.py
--rw-r--r--   0        0        0    14155 2024-03-07 08:45:04.006800 libsimba-1.4.8/libsimba/auth/client_credentials.py
--rw-r--r--   0        0        0     5439 2024-03-26 18:47:23.415429 libsimba-1.4.8/libsimba/config.py
--rw-r--r--   0        0        0     2385 2024-01-17 14:57:32.079102 libsimba-1.4.8/libsimba/exceptions.py
--rw-r--r--   0        0        0      420 2023-03-04 13:47:45.339901 libsimba-1.4.8/libsimba/logging.conf
--rw-r--r--   0        0        0     9513 2024-01-17 14:57:32.087024 libsimba-1.4.8/libsimba/param_checking.py
--rw-r--r--   0        0        0     9058 2024-04-25 16:28:25.416143 libsimba-1.4.8/libsimba/schemas.py
--rw-r--r--   0        0        0    43473 2024-04-09 12:05:30.382336 libsimba-1.4.8/libsimba/simba.py
--rw-r--r--   0        0        0    11155 2024-01-17 14:57:32.080878 libsimba-1.4.8/libsimba/simba_contract.py
--rw-r--r--   0        0        0    11044 2024-01-17 14:57:32.075698 libsimba-1.4.8/libsimba/simba_contract_sync.py
--rw-r--r--   0        0        0    32398 2024-03-26 18:52:17.461357 libsimba-1.4.8/libsimba/simba_request.py
--rw-r--r--   0        0        0    89029 2024-04-25 16:35:42.644353 libsimba-1.4.8/libsimba/simba_sync.py
--rw-r--r--   0        0        0    12737 2024-04-09 11:43:57.877966 libsimba-1.4.8/libsimba/utils.py
--rw-r--r--   0        0        0     2180 2024-01-17 14:57:32.077507 libsimba-1.4.8/libsimba/wallet.py
--rw-r--r--   0        0        0     1489 2024-04-25 16:36:27.597471 libsimba-1.4.8/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 libsimba-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-03-19 19:21:39.908933 libsimba-1.4.9/LICENSE
+-rw-r--r--   0        0        0     6148 2022-08-29 12:51:26.796404 libsimba-1.4.9/libsimba/.DS_Store
+-rw-r--r--   0        0        0     1529 2024-03-07 08:24:18.582108 libsimba-1.4.9/libsimba/__init__.py
+-rw-r--r--   0        0        0     1988 2024-03-09 09:43:42.012788 libsimba-1.4.9/libsimba/auth/__init__.py
+-rw-r--r--   0        0        0    10547 2023-09-29 17:13:22.513991 libsimba-1.4.9/libsimba/auth/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1294 2024-03-09 09:43:44.166035 libsimba-1.4.9/libsimba/auth/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1425 2024-03-09 09:47:07.552095 libsimba-1.4.9/libsimba/auth/__pycache__/apikey.cpython-39.pyc
+-rw-r--r--   0        0        0    10004 2024-03-07 10:02:50.833460 libsimba-1.4.9/libsimba/auth/__pycache__/client_credentials.cpython-39.pyc
+-rw-r--r--   0        0        0     1381 2024-03-07 10:07:58.051055 libsimba-1.4.9/libsimba/auth/apikey.py
+-rw-r--r--   0        0        0    14155 2024-03-07 08:45:04.006800 libsimba-1.4.9/libsimba/auth/client_credentials.py
+-rw-r--r--   0        0        0     5439 2024-03-26 18:47:23.415429 libsimba-1.4.9/libsimba/config.py
+-rw-r--r--   0        0        0     2385 2024-01-17 14:57:32.079102 libsimba-1.4.9/libsimba/exceptions.py
+-rw-r--r--   0        0        0      420 2023-03-04 13:47:45.339901 libsimba-1.4.9/libsimba/logging.conf
+-rw-r--r--   0        0        0     9513 2024-01-17 14:57:32.087024 libsimba-1.4.9/libsimba/param_checking.py
+-rw-r--r--   0        0        0     9058 2024-04-25 16:28:25.416143 libsimba-1.4.9/libsimba/schemas.py
+-rw-r--r--   0        0        0    43479 2024-04-25 16:48:40.794997 libsimba-1.4.9/libsimba/simba.py
+-rw-r--r--   0        0        0    11155 2024-01-17 14:57:32.080878 libsimba-1.4.9/libsimba/simba_contract.py
+-rw-r--r--   0        0        0    11044 2024-01-17 14:57:32.075698 libsimba-1.4.9/libsimba/simba_contract_sync.py
+-rw-r--r--   0        0        0    32398 2024-03-26 18:52:17.461357 libsimba-1.4.9/libsimba/simba_request.py
+-rw-r--r--   0        0        0    89029 2024-04-25 16:35:42.644353 libsimba-1.4.9/libsimba/simba_sync.py
+-rw-r--r--   0        0        0    12737 2024-04-09 11:43:57.877966 libsimba-1.4.9/libsimba/utils.py
+-rw-r--r--   0        0        0     2180 2024-01-17 14:57:32.077507 libsimba-1.4.9/libsimba/wallet.py
+-rw-r--r--   0        0        0     1489 2024-04-25 16:49:11.319417 libsimba-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 libsimba-1.4.9/PKG-INFO
```

### Comparing `libsimba-1.4.8/LICENSE` & `libsimba-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/.DS_Store` & `libsimba-1.4.9/libsimba/.DS_Store`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/__init__.py` & `libsimba-1.4.9/libsimba/__init__.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/auth/__init__.py` & `libsimba-1.4.9/libsimba/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/auth/__pycache__/__init__.cpython-311.pyc` & `libsimba-1.4.9/libsimba/auth/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/auth/__pycache__/__init__.cpython-39.pyc` & `libsimba-1.4.9/libsimba/auth/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/auth/__pycache__/apikey.cpython-39.pyc` & `libsimba-1.4.9/libsimba/auth/__pycache__/apikey.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/auth/__pycache__/client_credentials.cpython-39.pyc` & `libsimba-1.4.9/libsimba/auth/__pycache__/client_credentials.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/auth/apikey.py` & `libsimba-1.4.9/libsimba/auth/apikey.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/auth/client_credentials.py` & `libsimba-1.4.9/libsimba/auth/client_credentials.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/config.py` & `libsimba-1.4.9/libsimba/config.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/exceptions.py` & `libsimba-1.4.9/libsimba/exceptions.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/param_checking.py` & `libsimba-1.4.9/libsimba/param_checking.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/schemas.py` & `libsimba-1.4.9/libsimba/schemas.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/simba.py` & `libsimba-1.4.9/libsimba/simba.py`

 * *Files 0% similar despite different names*

```diff
@@ -1103,15 +1103,15 @@
                 )
             if network:
                 params.add_filter(
                     FieldFilter(field="networks", op=FilterOp.EQ, value=network)
                 )
         return await SimbaRequest(
             endpoint=Path.ADMIN_ACCOUNTS,
-            query_params=params,
+            query_params=params.query,
             login=login,
         ).retrieve(config=config, headers=headers or {})
 
     async def get_org_accounts(
         self,
         org: str,
         nickname: Optional[str] = None,
```

### Comparing `libsimba-1.4.8/libsimba/simba_contract.py` & `libsimba-1.4.9/libsimba/simba_contract.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/simba_contract_sync.py` & `libsimba-1.4.9/libsimba/simba_contract_sync.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/simba_request.py` & `libsimba-1.4.9/libsimba/simba_request.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/simba_sync.py` & `libsimba-1.4.9/libsimba/simba_sync.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/utils.py` & `libsimba-1.4.9/libsimba/utils.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/libsimba/wallet.py` & `libsimba-1.4.9/libsimba/wallet.py`

 * *Files identical despite different names*

### Comparing `libsimba-1.4.8/pyproject.toml` & `libsimba-1.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsimba"
-version = "1.4.8"
+version = "1.4.9"
 description = "libsimba is a library simplifying the use of SIMBAChain Blocks APIs."
 authors = [
     "SIMBA Chain Inc."
 ]
 
 packages = [
     { include = "libsimba" }
```

