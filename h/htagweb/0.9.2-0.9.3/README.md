# Comparing `tmp/htagweb-0.9.2.tar.gz` & `tmp/htagweb-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.9.2.tar", max compression
+gzip compressed data, was "htagweb-0.9.3.tar", max compression
```

## Comparing `htagweb-0.9.2.tar` & `htagweb-0.9.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1065 2023-09-15 06:22:19.572286 htagweb-0.9.2/LICENSE
--rw-r--r--   0        0        0     3404 2023-09-15 06:22:19.572286 htagweb-0.9.2/README.md
--rw-r--r--   0        0        0      537 2023-09-15 06:22:19.860286 htagweb-0.9.2/htagweb/__init__.py
--rw-r--r--   0        0        0      679 2023-09-15 06:22:19.572286 htagweb-0.9.2/htagweb/__main__.py
--rw-r--r--   0        0        0    12550 2023-09-15 06:22:19.572286 htagweb-0.9.2/htagweb/appserver.py
--rw-r--r--   0        0        0     2521 2023-09-15 06:22:19.572286 htagweb-0.9.2/htagweb/crypto.py
--rw-r--r--   0        0        0     2666 2023-09-15 06:22:19.572286 htagweb-0.9.2/htagweb/htagserver.py
--rw-r--r--   0        0        0      758 2023-09-15 06:22:19.572286 htagweb-0.9.2/htagweb/sessions/__init__.py
--rw-r--r--   0        0        0     1398 2023-09-15 06:22:19.572286 htagweb-0.9.2/htagweb/sessions/file.py
--rw-r--r--   0        0        0     1581 2023-09-15 06:22:19.572286 htagweb-0.9.2/htagweb/sessions/memory.py
--rw-r--r--   0        0        0      485 2023-09-15 06:22:19.572286 htagweb-0.9.2/htagweb/sessions/shm.py
--rw-r--r--   0        0        0     7910 2023-09-15 06:22:19.572286 htagweb-0.9.2/htagweb/usot.py
--rw-r--r--   0        0        0     1106 2023-09-15 06:22:19.860286 htagweb-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 htagweb-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-09-26 16:48:06.319270 htagweb-0.9.3/LICENSE
+-rw-r--r--   0        0        0     3404 2023-09-26 16:48:06.319270 htagweb-0.9.3/README.md
+-rw-r--r--   0        0        0      537 2023-09-26 16:48:06.615275 htagweb-0.9.3/htagweb/__init__.py
+-rw-r--r--   0        0        0      679 2023-09-26 16:48:06.319270 htagweb-0.9.3/htagweb/__main__.py
+-rw-r--r--   0        0        0    12550 2023-09-26 16:48:06.319270 htagweb-0.9.3/htagweb/appserver.py
+-rw-r--r--   0        0        0     2521 2023-09-26 16:48:06.319270 htagweb-0.9.3/htagweb/crypto.py
+-rw-r--r--   0        0        0     2666 2023-09-26 16:48:06.319270 htagweb-0.9.3/htagweb/htagserver.py
+-rw-r--r--   0        0        0      758 2023-09-26 16:48:06.319270 htagweb-0.9.3/htagweb/sessions/__init__.py
+-rw-r--r--   0        0        0     1765 2023-09-26 16:48:06.319270 htagweb-0.9.3/htagweb/sessions/file.py
+-rw-r--r--   0        0        0     1828 2023-09-26 16:48:06.319270 htagweb-0.9.3/htagweb/sessions/memory.py
+-rw-r--r--   0        0        0      485 2023-09-26 16:48:06.319270 htagweb-0.9.3/htagweb/sessions/shm.py
+-rw-r--r--   0        0        0     7910 2023-09-26 16:48:06.319270 htagweb-0.9.3/htagweb/usot.py
+-rw-r--r--   0        0        0     1106 2023-09-26 16:48:06.615275 htagweb-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 htagweb-0.9.3/PKG-INFO
```

### Comparing `htagweb-0.9.2/LICENSE` & `htagweb-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.9.2/README.md` & `htagweb-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `htagweb-0.9.2/htagweb/__init__.py` & `htagweb-0.9.3/htagweb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 
 from .appserver import AppServer  # a completly different beast, but compatible with ^^
 from .htagserver import HtagServer  # a completly different beast.
 from .usot import Usot
 
 __all__= ["AppServer"]
 
-__version__ = "0.9.2" # auto updated
+__version__ = "0.9.3" # auto updated
```

### Comparing `htagweb-0.9.2/htagweb/__main__.py` & `htagweb-0.9.3/htagweb/__main__.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.9.2/htagweb/appserver.py` & `htagweb-0.9.3/htagweb/appserver.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.9.2/htagweb/crypto.py` & `htagweb-0.9.3/htagweb/crypto.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.9.2/htagweb/htagserver.py` & `htagweb-0.9.3/htagweb/htagserver.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.9.2/htagweb/sessions/__init__.py` & `htagweb-0.9.3/htagweb/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.9.2/htagweb/sessions/file.py` & `htagweb-0.9.3/htagweb/sessions/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,29 +22,44 @@
 
         if os.path.isfile(self._file):
             with open(self._file,"rb+") as fid:
                 self._d=pickle.load(fid)
         else:
             self._d={}
 
+    def __len__(self):
+        return len(self._d.keys())
+
+    def __contains__(self,key):
+        return key in self._d.keys()
+
     def items(self):
         return self._d.items()
 
     def get(self,k:str,default=None):
         return self._d.get(k,default)
 
     def __getitem__(self,k:str):
         return self._d[k]
 
+    def __delitem__(self,k:str):
+        """ save session """
+        del self._d[k]
+
+        with open(self._file,"wb+") as fid:
+            pickle.dump(self._d,fid, protocol=4)
+
     def __setitem__(self,k:str,v):
+        """ save session """
         self._d[k]=v
 
         with open(self._file,"wb+") as fid:
             pickle.dump(self._d,fid, protocol=4)
 
     def clear(self):
+        """ save session """
         self._d.clear()
         if os.path.isfile(self._file):
             os.unlink(self._file)
 
 async def create(uid,persistent=False) -> FileDict:
     return FileDict(uid,persistent)
```

### Comparing `htagweb-0.9.2/htagweb/sessions/memory.py` & `htagweb-0.9.3/htagweb/sessions/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,37 @@
 
 
 class ServerMemDict: # proxy between app and ServerUnique
     def __init__(self,uid,dico:dict):
         self._uid=uid
         self._dico=dico
 
+    def __len__(self):
+        return len(self._dico.keys())
+
+    def __contains__(self,key):
+        return key in self._dico.keys()
+
     def items(self):
         return self._dico.items()
 
     def get(self,k:str,default=None):       # could be inplemented in SessionMem
         return self._dico.get(k,default)
 
     def __getitem__(self,k:str):            # could be inplemented in SessionMem
         return self._dico[k]
 
     def __setitem__(self,k:str,v):          # could be inplemented in SessionMem
         self._dico[k]=v
         PX.clientsync.set( self._uid, self._dico)
 
+    def __delitem__(self,k:str):
+        del self._dico[k]
+        PX.clientsync.set( self._uid, self._dico)
+
     def clear(self):
         self._dico.clear()
         PX.clientsync.set( self._uid, {})
 
     def __repr__(self):
         return f"<SessionMem {self._dico}>"
 
@@ -41,14 +51,16 @@
     def get(self,uid:str) -> ServerMemDict:
         if uid not in self.SESSIONS:
             self.SESSIONS[uid] = {}
         return ServerMemDict( uid, self.SESSIONS[uid] )
     def set(self,uid:str,dico):
         self.SESSIONS[uid] = dico
 
+
+
 PX=Usot( SessionMemory, port=19999 )
 
 def startServer():
     PX.start()
 
 async def create(uid) -> ServerMemDict:
     return PX.clientsync.get( uid )
```

### Comparing `htagweb-0.9.2/htagweb/usot.py` & `htagweb-0.9.3/htagweb/usot.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.9.2/pyproject.toml` & `htagweb-0.9.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.9.2" # auto-updated
+version = "0.9.3" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
@@ -15,15 +15,15 @@
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: Apache Software License",
 ]
 
 [tool.poetry.dependencies]
 # https://python-poetry.org/docs/dependency-specification/
 python = "^3.7"
-htag = ">= 0.9.44"
+htag = ">= 0.41.0"
 starlette = ">= 0.21.0"
 pycryptodomex = ">= 3.0.0"
 uvicorn = {version = ">=0.22,<1.0", extras = ["standard"]}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
```

### Comparing `htagweb-0.9.2/PKG-INFO` & `htagweb-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.9.2
+Version: 0.9.3
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: htag (>=0.9.44)
+Requires-Dist: htag (>=0.41.0)
 Requires-Dist: pycryptodomex (>=3.0.0)
 Requires-Dist: starlette (>=0.21.0)
 Requires-Dist: uvicorn[standard] (>=0.22,<1.0)
 Project-URL: Documentation, https://github.com/manatlan/htagweb
 Project-URL: Repository, https://github.com/manatlan/htagweb
 Description-Content-Type: text/markdown
```

