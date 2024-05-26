# Comparing `tmp/varorm-0.1.1.tar.gz` & `tmp/varorm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varorm-0.1.1.tar", last modified: Sat May 25 09:04:00 2024, max compression
+gzip compressed data, was "varorm-0.1.2.tar", last modified: Sun May 26 12:13:19 2024, max compression
```

## Comparing `varorm-0.1.1.tar` & `varorm-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-25 09:04:00.387408 varorm-0.1.1/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)    11357 2024-04-17 21:33:54.000000 varorm-0.1.1/LICENSE
--rw-rw-r--   0 sidq      (1000) sidq      (1000)    15419 2024-05-25 09:04:00.387408 varorm-0.1.1/PKG-INFO
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     2016 2024-05-25 09:03:38.000000 varorm-0.1.1/README.md
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       38 2024-05-25 09:04:00.387408 varorm-0.1.1/setup.cfg
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      763 2024-05-25 08:56:07.000000 varorm-0.1.1/setup.py
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-25 09:04:00.383408 varorm-0.1.1/varorm/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)        0 2024-05-01 22:41:17.000000 varorm-0.1.1/varorm/__init__.py
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-25 09:04:00.387408 varorm-0.1.1/varorm/dj/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       21 2024-05-02 12:59:57.000000 varorm-0.1.1/varorm/dj/__init__.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     1261 2024-05-25 08:44:46.000000 varorm-0.1.1/varorm/dj/admin.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      171 2024-05-02 22:23:24.000000 varorm-0.1.1/varorm/dj/apps.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       15 2024-05-02 22:21:47.000000 varorm-0.1.1/varorm/dj/globals.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      917 2024-05-03 12:03:42.000000 varorm-0.1.1/varorm/dj/loader.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     2729 2024-05-25 08:51:23.000000 varorm-0.1.1/varorm/dj/utils.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      852 2024-05-25 08:54:32.000000 varorm-0.1.1/varorm/dj/views.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      178 2024-05-03 21:41:53.000000 varorm-0.1.1/varorm/exceptions.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     2989 2024-05-03 22:25:12.000000 varorm-0.1.1/varorm/fields.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     2355 2024-05-25 09:01:20.000000 varorm-0.1.1/varorm/models.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     2975 2024-05-03 21:38:32.000000 varorm-0.1.1/varorm/storage.py
--rw-rw-r--   0 sidq      (1000) sidq      (1000)     1923 2024-05-03 22:26:15.000000 varorm-0.1.1/varorm/widgets.py
-drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-25 09:04:00.387408 varorm-0.1.1/varorm.egg-info/
--rw-rw-r--   0 sidq      (1000) sidq      (1000)    15419 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/PKG-INFO
--rw-rw-r--   0 sidq      (1000) sidq      (1000)      419 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/SOURCES.txt
--rw-rw-r--   0 sidq      (1000) sidq      (1000)        1 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/dependency_links.txt
--rw-rw-r--   0 sidq      (1000) sidq      (1000)       47 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/pbr.json
--rw-rw-r--   0 sidq      (1000) sidq      (1000)        7 2024-05-25 09:04:00.000000 varorm-0.1.1/varorm.egg-info/top_level.txt
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-26 12:13:19.049617 varorm-0.1.2/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)    11357 2024-04-17 21:33:54.000000 varorm-0.1.2/LICENSE
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)    15451 2024-05-26 12:13:19.045617 varorm-0.1.2/PKG-INFO
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2048 2024-05-26 12:12:42.000000 varorm-0.1.2/README.md
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       38 2024-05-26 12:13:19.049617 varorm-0.1.2/setup.cfg
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      763 2024-05-26 12:12:13.000000 varorm-0.1.2/setup.py
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-26 12:13:19.013617 varorm-0.1.2/varorm/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)        0 2024-05-01 22:41:17.000000 varorm-0.1.2/varorm/__init__.py
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-26 12:13:19.045617 varorm-0.1.2/varorm/dj/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       21 2024-05-02 12:59:57.000000 varorm-0.1.2/varorm/dj/__init__.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     1261 2024-05-25 08:44:46.000000 varorm-0.1.2/varorm/dj/admin.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      171 2024-05-02 22:23:24.000000 varorm-0.1.2/varorm/dj/apps.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       15 2024-05-02 22:21:47.000000 varorm-0.1.2/varorm/dj/globals.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      917 2024-05-03 12:03:42.000000 varorm-0.1.2/varorm/dj/loader.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2729 2024-05-25 08:51:23.000000 varorm-0.1.2/varorm/dj/utils.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      852 2024-05-25 08:54:32.000000 varorm-0.1.2/varorm/dj/views.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      178 2024-05-03 21:41:53.000000 varorm-0.1.2/varorm/exceptions.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2989 2024-05-03 22:25:12.000000 varorm-0.1.2/varorm/fields.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     2355 2024-05-25 09:01:20.000000 varorm-0.1.2/varorm/models.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     3793 2024-05-26 12:11:20.000000 varorm-0.1.2/varorm/storage.py
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)     1923 2024-05-03 22:26:15.000000 varorm-0.1.2/varorm/widgets.py
+drwxrwxr-x   0 sidq      (1000) sidq      (1000)        0 2024-05-26 12:13:19.033617 varorm-0.1.2/varorm.egg-info/
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)    15451 2024-05-26 12:13:18.000000 varorm-0.1.2/varorm.egg-info/PKG-INFO
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)      419 2024-05-26 12:13:18.000000 varorm-0.1.2/varorm.egg-info/SOURCES.txt
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)        1 2024-05-26 12:13:18.000000 varorm-0.1.2/varorm.egg-info/dependency_links.txt
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)       47 2024-05-26 12:13:18.000000 varorm-0.1.2/varorm.egg-info/pbr.json
+-rw-rw-r--   0 sidq      (1000) sidq      (1000)        7 2024-05-26 12:13:18.000000 varorm-0.1.2/varorm.egg-info/top_level.txt
```

### Comparing `varorm-0.1.1/LICENSE` & `varorm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `varorm-0.1.1/PKG-INFO` & `varorm-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varorm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Variable orm with django admin support
 Author: Sidq
 Author-email: abba.dmytro@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -214,14 +214,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## varorm - variables orm with django admin support
 
 #### v0.1 - Basic models and Django admin support
 #### v0.1.1 - Add groups access to variables and verbose_name for django admin, setup key on init of model
+#### v0.1.2 - Add MongoStorage 
 
 #### TODO - refactor django widgets, better type-hints
 ## Documentation
 
 ```python3
 from varorm.models import Model
 from varorm import fields
```

### Comparing `varorm-0.1.1/README.md` & `varorm-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ## varorm - variables orm with django admin support
 
 #### v0.1 - Basic models and Django admin support
 #### v0.1.1 - Add groups access to variables and verbose_name for django admin, setup key on init of model
+#### v0.1.2 - Add MongoStorage 
 
 #### TODO - refactor django widgets, better type-hints
 ## Documentation
 
 ```python3
 from varorm.models import Model
 from varorm import fields
```

### Comparing `varorm-0.1.1/setup.py` & `varorm-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   'GitHub': 'https://github.com/sidqdev/varorm',
   'Telegram': 'https://t.me/sidqdev'
 }
 
 
 setup(
     name='varorm',
-    version='0.1.1',
+    version='0.1.2',
     author='Sidq',
     author_email='abba.dmytro@gmail.com',
     description='Variable orm with django admin support',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     license=license,
```

### Comparing `varorm-0.1.1/varorm/dj/admin.py` & `varorm-0.1.2/varorm/dj/admin.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.1/varorm/dj/loader.py` & `varorm-0.1.2/varorm/dj/loader.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.1/varorm/dj/utils.py` & `varorm-0.1.2/varorm/dj/utils.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.1/varorm/dj/views.py` & `varorm-0.1.2/varorm/dj/views.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.1/varorm/fields.py` & `varorm-0.1.2/varorm/fields.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.1/varorm/models.py` & `varorm-0.1.2/varorm/models.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.1/varorm/storage.py` & `varorm-0.1.2/varorm/storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -97,7 +97,34 @@
             return val.decode()
         
         return val
         
     def hset(self, key: str, hkey: str, value: Any):
         return self._connection.hset(key, hkey, value)
     
+
+class MongoStorage(BaseStorage):
+    def __init__(self, url: str = None, db_name: str = 'default', **kwargs) -> None:
+        import pymongo
+        if url is not None:
+            client = pymongo.MongoClient(url)
+        else:
+            client = pymongo.MongoClient(**kwargs)
+
+        self._db = client[db_name]
+
+    def hget(self, key: str, hkey: str) -> Any:
+        try:
+            val = self._db[key].find_one({"key": hkey})
+            assert val is not None
+        except:
+            raise VarDoesNotExistException
+
+        val = val['value']
+        if isinstance(val, bytes):
+            return val.decode()
+        
+        return val
+        
+    def hset(self, key: str, hkey: str, value: Any):
+        return self._db[key].replace_one({"key": hkey}, {"key": hkey, "value": value}, upsert=True)
+
```

### Comparing `varorm-0.1.1/varorm/widgets.py` & `varorm-0.1.2/varorm/widgets.py`

 * *Files identical despite different names*

### Comparing `varorm-0.1.1/varorm.egg-info/PKG-INFO` & `varorm-0.1.2/varorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varorm
-Version: 0.1.1
+Version: 0.1.2
 Summary: Variable orm with django admin support
 Author: Sidq
 Author-email: abba.dmytro@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -214,14 +214,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## varorm - variables orm with django admin support
 
 #### v0.1 - Basic models and Django admin support
 #### v0.1.1 - Add groups access to variables and verbose_name for django admin, setup key on init of model
+#### v0.1.2 - Add MongoStorage 
 
 #### TODO - refactor django widgets, better type-hints
 ## Documentation
 
 ```python3
 from varorm.models import Model
 from varorm import fields
```

