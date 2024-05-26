# Comparing `tmp/msfabricpysdkcore-0.0.8.tar.gz` & `tmp/msfabricpysdkcore-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfabricpysdkcore-0.0.8.tar", last modified: Thu Apr 18 12:10:12 2024, max compression
+gzip compressed data, was "msfabricpysdkcore-0.0.9.tar", last modified: Thu Apr 18 12:17:36 2024, max compression
```

## Comparing `msfabricpysdkcore-0.0.8.tar` & `msfabricpysdkcore-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 12:10:12.436507 msfabricpysdkcore-0.0.8/
--rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    16383 2024-04-18 12:10:12.431981 msfabricpysdkcore-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    15865 2024-04-17 08:55:42.000000 msfabricpysdkcore-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 12:10:12.210181 msfabricpysdkcore-0.0.8/msfabricpysdkcore/
--rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/__init__.py
--rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/admin_item.py
--rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/admin_workspace.py
--rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/adminapi.py
--rw-rw-rw-   0        0        0     2436 2024-04-18 10:49:14.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/auth.py
--rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/capacity.py
--rw-rw-rw-   0        0        0     1197 2024-04-18 10:46:00.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/client.py
--rw-rw-rw-   0        0        0    32048 2024-04-16 15:03:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/coreapi.py
--rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/domain.py
--rw-rw-rw-   0        0        0    11570 2024-04-16 14:02:36.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/item.py
--rw-rw-rw-   0        0        0     2745 2024-04-11 11:55:54.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/job_instance.py
--rw-rw-rw-   0        0        0     3928 2024-04-11 11:55:24.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/lakehouse.py
--rw-rw-rw-   0        0        0     2848 2024-04-11 16:24:05.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/long_running_operation.py
--rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/onelakeshortcut.py
--rw-rw-rw-   0        0        0     3834 2024-04-15 14:15:34.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/otheritems.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:10:12.424012 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/
--rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/__init__.py
--rw-rw-rw-   0        0        0     2048 2024-04-17 14:16:01.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_admin_apis.py
--rw-rw-rw-   0        0        0     4635 2024-04-17 14:16:20.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_domains.py
--rw-rw-rw-   0        0        0     2399 2024-04-17 14:16:25.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_git.py
--rw-rw-rw-   0        0        0    21185 2024-04-17 14:45:21.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
--rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_jobs.py
--rw-rw-rw-   0        0        0     2391 2024-04-17 14:16:33.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_shortcuts.py
--rw-rw-rw-   0        0        0     6549 2024-04-17 14:16:38.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_workspaces_capacities.py
--rw-rw-rw-   0        0        0    48660 2024-04-16 15:03:00.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore/workspace.py
-drwxrwxrwx   0        0        0        0 2024-04-18 12:10:12.429980 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/
--rw-rw-rw-   0        0        0    16383 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-18 12:10:12.000000 msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      564 2024-04-18 12:07:11.000000 msfabricpysdkcore-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 12:10:12.436507 msfabricpysdkcore-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-18 12:07:06.000000 msfabricpysdkcore-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:17:36.159878 msfabricpysdkcore-0.0.9/
+-rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    16443 2024-04-18 12:17:36.154677 msfabricpysdkcore-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    15925 2024-04-18 12:17:10.000000 msfabricpysdkcore-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 12:17:35.993778 msfabricpysdkcore-0.0.9/msfabricpysdkcore/
+-rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/__init__.py
+-rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/admin_item.py
+-rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/admin_workspace.py
+-rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/adminapi.py
+-rw-rw-rw-   0        0        0     2430 2024-04-18 12:15:22.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/auth.py
+-rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/capacity.py
+-rw-rw-rw-   0        0        0     1197 2024-04-18 10:46:00.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/client.py
+-rw-rw-rw-   0        0        0    32048 2024-04-16 15:03:12.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/coreapi.py
+-rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/domain.py
+-rw-rw-rw-   0        0        0    11570 2024-04-16 14:02:36.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/item.py
+-rw-rw-rw-   0        0        0     2745 2024-04-11 11:55:54.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/job_instance.py
+-rw-rw-rw-   0        0        0     3928 2024-04-11 11:55:24.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/lakehouse.py
+-rw-rw-rw-   0        0        0     2848 2024-04-11 16:24:05.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/long_running_operation.py
+-rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/onelakeshortcut.py
+-rw-rw-rw-   0        0        0     3834 2024-04-15 14:15:34.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/otheritems.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:17:36.144132 msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/__init__.py
+-rw-rw-rw-   0        0        0     2048 2024-04-17 14:16:01.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_admin_apis.py
+-rw-rw-rw-   0        0        0     4635 2024-04-17 14:16:20.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_domains.py
+-rw-rw-rw-   0        0        0     2399 2024-04-17 14:16:25.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_git.py
+-rw-rw-rw-   0        0        0    21185 2024-04-17 14:45:21.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
+-rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_jobs.py
+-rw-rw-rw-   0        0        0     2391 2024-04-17 14:16:33.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_shortcuts.py
+-rw-rw-rw-   0        0        0     6549 2024-04-17 14:16:38.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_workspaces_capacities.py
+-rw-rw-rw-   0        0        0    48660 2024-04-16 15:03:00.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore/workspace.py
+drwxrwxrwx   0        0        0        0 2024-04-18 12:17:36.147146 msfabricpysdkcore-0.0.9/msfabricpysdkcore.egg-info/
+-rw-rw-rw-   0        0        0    16443 2024-04-18 12:17:35.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2024-04-18 12:17:35.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 12:17:35.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-18 12:17:35.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-18 12:17:35.000000 msfabricpysdkcore-0.0.9/msfabricpysdkcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      564 2024-04-18 12:16:25.000000 msfabricpysdkcore-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 12:17:36.159878 msfabricpysdkcore-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-18 12:16:46.000000 msfabricpysdkcore-0.0.9/setup.py
```

### Comparing `msfabricpysdkcore-0.0.8/LICENSE` & `msfabricpysdkcore-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/PKG-INFO` & `msfabricpysdkcore-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -20,15 +20,15 @@
 ![Python hugging a F](assets/fabricpythontransparent.png)
 
 The Microsoft Fabric REST APIs are documented [here](https://docs.microsoft.com/en-us/rest/api/fabric/).
 They are designed to automate your Fabric processes.
 
 This SDK helps to interact with the Fabric APIs in a more Pythonic way.
 Additionally it brings some extra features like:
-- Authentication is handled for you (currently Azure CLI Authentication  and Service Principal Authentication are supported)
+- Authentication is handled for you (currently Azure CLI Authentication and Service Principal Authentication are supported, as well as Synapse Spark Authentication in Fabric Notebooks)
 - Waiting for completion of long running operations
 - Retry logic when hitting the API rate limits
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
 - Do bulk operations (see [Usage Patterns](usage_patterns.md))
 - Pagination support
```

### Comparing `msfabricpysdkcore-0.0.8/README.md` & `msfabricpysdkcore-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![Python hugging a F](assets/fabricpythontransparent.png)
 
 The Microsoft Fabric REST APIs are documented [here](https://docs.microsoft.com/en-us/rest/api/fabric/).
 They are designed to automate your Fabric processes.
 
 This SDK helps to interact with the Fabric APIs in a more Pythonic way.
 Additionally it brings some extra features like:
-- Authentication is handled for you (currently Azure CLI Authentication  and Service Principal Authentication are supported)
+- Authentication is handled for you (currently Azure CLI Authentication and Service Principal Authentication are supported, as well as Synapse Spark Authentication in Fabric Notebooks)
 - Waiting for completion of long running operations
 - Retry logic when hitting the API rate limits
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
 - Do bulk operations (see [Usage Patterns](usage_patterns.md))
 - Pagination support
```

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/admin_item.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/admin_item.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/admin_workspace.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/admin_workspace.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/adminapi.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/adminapi.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/auth.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,10 +68,10 @@
     def __init__(self):
         mssparkutils.credentials.getToken("pbi")
         print("Using Synapse Spark Utils for authentication")
 
     def get_token(self):
         """Get token from Azure AD"""
         token = mssparkutils.credentials.getToken("pbi")
-        return token.token
+        return token
```

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/capacity.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/capacity.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/client.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/client.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/coreapi.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/coreapi.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/domain.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/domain.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/item.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/item.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/job_instance.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/job_instance.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/lakehouse.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/lakehouse.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/long_running_operation.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/long_running_operation.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/onelakeshortcut.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/onelakeshortcut.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/otheritems.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/otheritems.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_admin_apis.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_admin_apis.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_domains.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_domains.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_git.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_items_incl_lakehouse.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_items_incl_lakehouse.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_jobs.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_shortcuts.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/tests/test_workspaces_capacities.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/tests/test_workspaces_capacities.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore/workspace.py` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore/workspace.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/PKG-INFO` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -20,15 +20,15 @@
 ![Python hugging a F](assets/fabricpythontransparent.png)
 
 The Microsoft Fabric REST APIs are documented [here](https://docs.microsoft.com/en-us/rest/api/fabric/).
 They are designed to automate your Fabric processes.
 
 This SDK helps to interact with the Fabric APIs in a more Pythonic way.
 Additionally it brings some extra features like:
-- Authentication is handled for you (currently Azure CLI Authentication  and Service Principal Authentication are supported)
+- Authentication is handled for you (currently Azure CLI Authentication and Service Principal Authentication are supported, as well as Synapse Spark Authentication in Fabric Notebooks)
 - Waiting for completion of long running operations
 - Retry logic when hitting the API rate limits
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
 - Do bulk operations (see [Usage Patterns](usage_patterns.md))
 - Pagination support
```

### Comparing `msfabricpysdkcore-0.0.8/msfabricpysdkcore.egg-info/SOURCES.txt` & `msfabricpysdkcore-0.0.9/msfabricpysdkcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.8/pyproject.toml` & `msfabricpysdkcore-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msfabricpysdkcore"
-version = "0.0.8"
+version = "0.0.9"
 dynamic = ["dependencies"]
 authors = [
   { name="Andreas Rederer"},
 ]
 description = "A Python SDK for Microsoft Fabric"
 readme = "README.md"
 requires-python = ">=3.10"
```

