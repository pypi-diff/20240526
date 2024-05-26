# Comparing `tmp/mongo-api-client-0.1.tar.gz` & `tmp/mongo-api-client-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo-api-client-0.1.tar", last modified: Sat May 25 16:34:58 2024, max compression
+gzip compressed data, was "mongo-api-client-0.2.tar", last modified: Sat May 25 16:49:03 2024, max compression
```

## Comparing `mongo-api-client-0.1.tar` & `mongo-api-client-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 16:34:58.589096 mongo-api-client-0.1/
--rw-rw-rw-   0        0        0     4157 2024-05-25 16:34:58.588096 mongo-api-client-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3652 2024-05-25 16:33:00.000000 mongo-api-client-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 16:34:58.584097 mongo-api-client-0.1/mongo_api_client/
--rw-rw-rw-   0        0        0    13501 2024-05-25 16:13:38.000000 mongo-api-client-0.1/mongo_api_client/MongoApiClient.py
--rw-rw-rw-   0        0        0       42 2024-05-25 16:30:42.000000 mongo-api-client-0.1/mongo_api_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 16:34:58.588096 mongo-api-client-0.1/mongo_api_client.egg-info/
--rw-rw-rw-   0        0        0     4157 2024-05-25 16:34:58.000000 mongo-api-client-0.1/mongo_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-05-25 16:34:58.000000 mongo-api-client-0.1/mongo_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 16:34:58.000000 mongo-api-client-0.1/mongo_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 16:34:58.000000 mongo-api-client-0.1/mongo_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-25 16:34:58.000000 mongo-api-client-0.1/mongo_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 16:34:58.589096 mongo-api-client-0.1/setup.cfg
--rw-rw-rw-   0        0        0      740 2024-05-25 16:30:25.000000 mongo-api-client-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:49:03.700364 mongo-api-client-0.2/
+-rw-rw-rw-   0        0        0     4159 2024-05-25 16:49:03.699365 mongo-api-client-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3654 2024-05-25 16:44:52.000000 mongo-api-client-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 16:49:03.695363 mongo-api-client-0.2/mongo_api_client/
+-rw-rw-rw-   0        0        0    13501 2024-05-25 16:13:38.000000 mongo-api-client-0.2/mongo_api_client/MongoApiClient.py
+-rw-rw-rw-   0        0        0       42 2024-05-25 16:30:42.000000 mongo-api-client-0.2/mongo_api_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 16:49:03.698365 mongo-api-client-0.2/mongo_api_client.egg-info/
+-rw-rw-rw-   0        0        0     4159 2024-05-25 16:49:03.000000 mongo-api-client-0.2/mongo_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-25 16:49:03.000000 mongo-api-client-0.2/mongo_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 16:49:03.000000 mongo-api-client-0.2/mongo_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 16:49:03.000000 mongo-api-client-0.2/mongo_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-25 16:49:03.000000 mongo-api-client-0.2/mongo_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 16:49:03.700364 mongo-api-client-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      740 2024-05-25 16:47:02.000000 mongo-api-client-0.2/setup.py
```

### Comparing `mongo-api-client-0.1/PKG-INFO` & `mongo-api-client-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-api-client
-Version: 0.1
+Version: 0.2
 Summary: Provides a fluent syntax for interacting with a MongoDB API Instance
 Home-page: https://github.com/alexanderthegreat96/mongo-api-python-client
 Author: Alexandru Lupaescu
 Author-email: alexandrulupaescu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,15 @@
     - "like": Similar to (using the MongoDB $regex operator)
 - Sorting: You can specify the sorting order as "asc" (ascending) or  - "desc" (descending) using the sort_by() method.
 
 ## Usage
 Here's an example of how to use MongoApiClient to interact with MongoDB:
 
 ```python
-from MongoApiClient import MongoApiClient
+from mongo_api_client import MongoApiClient
 
 # Initialize MongoApiClient with connection details
 database = MongoApiClient(
     server_ip= "your-server-ip", 
     server_port=9875, 
     scheme= "http")
 ```
```

### Comparing `mongo-api-client-0.1/README.md` & `mongo-api-client-0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     - "like": Similar to (using the MongoDB $regex operator)
 - Sorting: You can specify the sorting order as "asc" (ascending) or  - "desc" (descending) using the sort_by() method.
 
 ## Usage
 Here's an example of how to use MongoApiClient to interact with MongoDB:
 
 ```python
-from MongoApiClient import MongoApiClient
+from mongo_api_client import MongoApiClient
 
 # Initialize MongoApiClient with connection details
 database = MongoApiClient(
     server_ip= "your-server-ip", 
     server_port=9875, 
     scheme= "http")
 ```
```

### Comparing `mongo-api-client-0.1/mongo_api_client/MongoApiClient.py` & `mongo-api-client-0.2/mongo_api_client/MongoApiClient.py`

 * *Files identical despite different names*

### Comparing `mongo-api-client-0.1/mongo_api_client.egg-info/PKG-INFO` & `mongo-api-client-0.2/mongo_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-api-client
-Version: 0.1
+Version: 0.2
 Summary: Provides a fluent syntax for interacting with a MongoDB API Instance
 Home-page: https://github.com/alexanderthegreat96/mongo-api-python-client
 Author: Alexandru Lupaescu
 Author-email: alexandrulupaescu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,15 +37,15 @@
     - "like": Similar to (using the MongoDB $regex operator)
 - Sorting: You can specify the sorting order as "asc" (ascending) or  - "desc" (descending) using the sort_by() method.
 
 ## Usage
 Here's an example of how to use MongoApiClient to interact with MongoDB:
 
 ```python
-from MongoApiClient import MongoApiClient
+from mongo_api_client import MongoApiClient
 
 # Initialize MongoApiClient with connection details
 database = MongoApiClient(
     server_ip= "your-server-ip", 
     server_port=9875, 
     scheme= "http")
 ```
```

### Comparing `mongo-api-client-0.1/setup.py` & `mongo-api-client-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mongo-api-client',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         "requests"
     ],
     author='Alexandru Lupaescu',
     author_email='alexandrulupaescu@gmail.com',
     description='Provides a fluent syntax for interacting with a MongoDB API Instance',
```

