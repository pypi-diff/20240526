# Comparing `tmp/pluralkit-1.1.6.tar.gz` & `tmp/pluralkit-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluralkit-1.1.6.tar", last modified: Sun Feb 25 06:33:25 2024, max compression
+gzip compressed data, was "pluralkit-1.1.7.tar", last modified: Sat May 25 23:53:38 2024, max compression
```

## Comparing `pluralkit-1.1.6.tar` & `pluralkit-1.1.7.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.860952 pluralkit-1.1.6/
--rw-r--r--   0 mlandry    (501) staff       (20)     1068 2024-02-25 06:19:21.000000 pluralkit-1.1.6/LICENSE
--rw-r--r--   0 mlandry    (501) staff       (20)      267 2024-02-25 06:19:21.000000 pluralkit-1.1.6/MANIFEST.in
--rw-r--r--   0 mlandry    (501) staff       (20)     5419 2024-02-25 06:33:25.859984 pluralkit-1.1.6/PKG-INFO
--rw-r--r--   0 mlandry    (501) staff       (20)     3729 2024-02-25 06:19:21.000000 pluralkit-1.1.6/README.md
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.834698 pluralkit-1.1.6/docs/
--rw-r--r--   0 mlandry    (501) staff       (20)      634 2024-02-25 06:19:21.000000 pluralkit-1.1.6/docs/Makefile
--rw-r--r--   0 mlandry    (501) staff       (20)      652 2024-02-25 06:19:21.000000 pluralkit-1.1.6/docs/README.md
--rw-r--r--   0 mlandry    (501) staff       (20)     3312 2024-02-25 06:19:21.000000 pluralkit-1.1.6/docs/conf.py
--rw-r--r--   0 mlandry    (501) staff       (20)     1273 2024-02-25 06:19:21.000000 pluralkit-1.1.6/docs/index.rst
--rw-r--r--   0 mlandry    (501) staff       (20)      234 2024-02-25 06:19:21.000000 pluralkit-1.1.6/docs/requirements.txt
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.836115 pluralkit-1.1.6/docs/source/
--rw-r--r--   0 mlandry    (501) staff       (20)     3932 2024-02-25 06:19:21.000000 pluralkit-1.1.6/docs/source/changelog.rst
--rw-r--r--   0 mlandry    (501) staff       (20)    12092 2024-02-25 06:19:21.000000 pluralkit-1.1.6/docs/source/quickstart.rst
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.837629 pluralkit-1.1.6/docs/source/v1/
--rw-r--r--   0 mlandry    (501) staff       (20)     1761 2024-02-25 06:19:21.000000 pluralkit-1.1.6/docs/source/v1/api.rst
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.838612 pluralkit-1.1.6/docs/source/v2/
--rw-r--r--   0 mlandry    (501) staff       (20)     2943 2024-02-25 06:19:21.000000 pluralkit-1.1.6/docs/source/v2/api.rst
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.840504 pluralkit-1.1.6/pluralkit/
--rw-r--r--   0 mlandry    (501) staff       (20)      252 2024-02-25 06:19:21.000000 pluralkit-1.1.6/pluralkit/__init__.py
--rw-r--r--   0 mlandry    (501) staff       (20)      248 2024-02-25 06:32:01.000000 pluralkit-1.1.6/pluralkit/__version__.py
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.849522 pluralkit-1.1.6/pluralkit/v1/
--rw-r--r--   0 mlandry    (501) staff       (20)      217 2024-02-25 06:19:21.000000 pluralkit-1.1.6/pluralkit/v1/__init__.py
--rw-r--r--   0 mlandry    (501) staff       (20)    32468 2024-02-25 06:19:21.000000 pluralkit-1.1.6/pluralkit/v1/client.py
--rw-r--r--   0 mlandry    (501) staff       (20)     2824 2024-02-25 06:19:21.000000 pluralkit-1.1.6/pluralkit/v1/errors.py
--rw-r--r--   0 mlandry    (501) staff       (20)    38036 2024-02-25 06:19:21.000000 pluralkit-1.1.6/pluralkit/v1/models.py
--rw-r--r--   0 mlandry    (501) staff       (20)     4302 2024-02-25 06:19:21.000000 pluralkit-1.1.6/pluralkit/v1/utils.py
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.853196 pluralkit-1.1.6/pluralkit/v2/
--rw-r--r--   0 mlandry    (501) staff       (20)      666 2024-02-25 06:19:21.000000 pluralkit-1.1.6/pluralkit/v2/__init__.py
--rw-r--r--   0 mlandry    (501) staff       (20)    49625 2024-02-25 06:19:21.000000 pluralkit-1.1.6/pluralkit/v2/client.py
--rw-r--r--   0 mlandry    (501) staff       (20)     2821 2024-02-25 06:19:21.000000 pluralkit-1.1.6/pluralkit/v2/errors.py
--rw-r--r--   0 mlandry    (501) staff       (20)    39252 2024-02-25 06:31:17.000000 pluralkit-1.1.6/pluralkit/v2/models.py
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.857059 pluralkit-1.1.6/pluralkit.egg-info/
--rw-r--r--   0 mlandry    (501) staff       (20)     5419 2024-02-25 06:33:25.000000 pluralkit-1.1.6/pluralkit.egg-info/PKG-INFO
--rw-r--r--   0 mlandry    (501) staff       (20)      698 2024-02-25 06:33:25.000000 pluralkit-1.1.6/pluralkit.egg-info/SOURCES.txt
--rw-r--r--   0 mlandry    (501) staff       (20)        1 2024-02-25 06:33:25.000000 pluralkit-1.1.6/pluralkit.egg-info/dependency_links.txt
--rw-r--r--   0 mlandry    (501) staff       (20)      188 2024-02-25 06:33:25.000000 pluralkit-1.1.6/pluralkit.egg-info/requires.txt
--rw-r--r--   0 mlandry    (501) staff       (20)       10 2024-02-25 06:33:25.000000 pluralkit-1.1.6/pluralkit.egg-info/top_level.txt
--rw-r--r--   0 mlandry    (501) staff       (20)       38 2024-02-25 06:33:25.861166 pluralkit-1.1.6/setup.cfg
--rw-r--r--   0 mlandry    (501) staff       (20)     2217 2024-02-25 06:19:21.000000 pluralkit-1.1.6/setup.py
-drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-02-25 06:33:25.855937 pluralkit-1.1.6/tests/
--rw-r--r--   0 mlandry    (501) staff       (20)     6785 2024-02-25 06:19:21.000000 pluralkit-1.1.6/tests/test_member.py
--rw-r--r--   0 mlandry    (501) staff       (20)      503 2024-02-25 06:19:21.000000 pluralkit-1.1.6/tests/test_misc.py
--rw-r--r--   0 mlandry    (501) staff       (20)     2671 2024-02-25 06:19:21.000000 pluralkit-1.1.6/tests/test_system.py
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.354947 pluralkit-1.1.7/
+-rw-r--r--   0 mlandry    (501) staff       (20)     1068 2024-02-25 06:19:21.000000 pluralkit-1.1.7/LICENSE
+-rw-r--r--   0 mlandry    (501) staff       (20)      267 2024-02-25 06:19:21.000000 pluralkit-1.1.7/MANIFEST.in
+-rw-r--r--   0 mlandry    (501) staff       (20)     5419 2024-05-25 23:53:38.354391 pluralkit-1.1.7/PKG-INFO
+-rw-r--r--   0 mlandry    (501) staff       (20)     3729 2024-02-25 06:19:21.000000 pluralkit-1.1.7/README.md
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.338028 pluralkit-1.1.7/docs/
+-rw-r--r--   0 mlandry    (501) staff       (20)      634 2024-02-25 06:19:21.000000 pluralkit-1.1.7/docs/Makefile
+-rw-r--r--   0 mlandry    (501) staff       (20)      652 2024-02-25 06:19:21.000000 pluralkit-1.1.7/docs/README.md
+-rw-r--r--   0 mlandry    (501) staff       (20)     3312 2024-02-25 06:19:21.000000 pluralkit-1.1.7/docs/conf.py
+-rw-r--r--   0 mlandry    (501) staff       (20)     1273 2024-02-25 06:19:21.000000 pluralkit-1.1.7/docs/index.rst
+-rw-r--r--   0 mlandry    (501) staff       (20)      234 2024-02-25 06:19:21.000000 pluralkit-1.1.7/docs/requirements.txt
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.339411 pluralkit-1.1.7/docs/source/
+-rw-r--r--   0 mlandry    (501) staff       (20)     3932 2024-02-25 06:19:21.000000 pluralkit-1.1.7/docs/source/changelog.rst
+-rw-r--r--   0 mlandry    (501) staff       (20)    12092 2024-02-25 06:19:21.000000 pluralkit-1.1.7/docs/source/quickstart.rst
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.340197 pluralkit-1.1.7/docs/source/v1/
+-rw-r--r--   0 mlandry    (501) staff       (20)     1761 2024-02-25 06:19:21.000000 pluralkit-1.1.7/docs/source/v1/api.rst
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.340920 pluralkit-1.1.7/docs/source/v2/
+-rw-r--r--   0 mlandry    (501) staff       (20)     2943 2024-02-25 06:19:21.000000 pluralkit-1.1.7/docs/source/v2/api.rst
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.342245 pluralkit-1.1.7/pluralkit/
+-rw-r--r--   0 mlandry    (501) staff       (20)      252 2024-02-25 06:19:21.000000 pluralkit-1.1.7/pluralkit/__init__.py
+-rw-r--r--   0 mlandry    (501) staff       (20)      248 2024-05-25 23:48:53.000000 pluralkit-1.1.7/pluralkit/__version__.py
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.348377 pluralkit-1.1.7/pluralkit/v1/
+-rw-r--r--   0 mlandry    (501) staff       (20)      217 2024-02-25 06:19:21.000000 pluralkit-1.1.7/pluralkit/v1/__init__.py
+-rw-r--r--   0 mlandry    (501) staff       (20)    32468 2024-02-25 06:19:21.000000 pluralkit-1.1.7/pluralkit/v1/client.py
+-rw-r--r--   0 mlandry    (501) staff       (20)     2824 2024-02-25 06:19:21.000000 pluralkit-1.1.7/pluralkit/v1/errors.py
+-rw-r--r--   0 mlandry    (501) staff       (20)    38036 2024-02-25 06:19:21.000000 pluralkit-1.1.7/pluralkit/v1/models.py
+-rw-r--r--   0 mlandry    (501) staff       (20)     4302 2024-02-25 06:19:21.000000 pluralkit-1.1.7/pluralkit/v1/utils.py
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.350639 pluralkit-1.1.7/pluralkit/v2/
+-rw-r--r--   0 mlandry    (501) staff       (20)      666 2024-02-25 06:19:21.000000 pluralkit-1.1.7/pluralkit/v2/__init__.py
+-rw-r--r--   0 mlandry    (501) staff       (20)    49625 2024-02-25 06:19:21.000000 pluralkit-1.1.7/pluralkit/v2/client.py
+-rw-r--r--   0 mlandry    (501) staff       (20)     2821 2024-02-25 06:19:21.000000 pluralkit-1.1.7/pluralkit/v2/errors.py
+-rw-r--r--   0 mlandry    (501) staff       (20)    39980 2024-05-25 23:46:54.000000 pluralkit-1.1.7/pluralkit/v2/models.py
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.352602 pluralkit-1.1.7/pluralkit.egg-info/
+-rw-r--r--   0 mlandry    (501) staff       (20)     5419 2024-05-25 23:53:38.000000 pluralkit-1.1.7/pluralkit.egg-info/PKG-INFO
+-rw-r--r--   0 mlandry    (501) staff       (20)      717 2024-05-25 23:53:38.000000 pluralkit-1.1.7/pluralkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mlandry    (501) staff       (20)        1 2024-05-25 23:53:38.000000 pluralkit-1.1.7/pluralkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mlandry    (501) staff       (20)      188 2024-05-25 23:53:38.000000 pluralkit-1.1.7/pluralkit.egg-info/requires.txt
+-rw-r--r--   0 mlandry    (501) staff       (20)       10 2024-05-25 23:53:38.000000 pluralkit-1.1.7/pluralkit.egg-info/top_level.txt
+-rw-r--r--   0 mlandry    (501) staff       (20)      209 2024-02-25 06:38:51.000000 pluralkit-1.1.7/pypi_api_token.txt
+-rw-r--r--   0 mlandry    (501) staff       (20)       38 2024-05-25 23:53:38.355067 pluralkit-1.1.7/setup.cfg
+-rw-r--r--   0 mlandry    (501) staff       (20)     2217 2024-02-25 06:19:21.000000 pluralkit-1.1.7/setup.py
+drwxr-xr-x   0 mlandry    (501) staff       (20)        0 2024-05-25 23:53:38.352088 pluralkit-1.1.7/tests/
+-rw-r--r--   0 mlandry    (501) staff       (20)     6785 2024-02-25 06:19:21.000000 pluralkit-1.1.7/tests/test_member.py
+-rw-r--r--   0 mlandry    (501) staff       (20)      503 2024-02-25 06:19:21.000000 pluralkit-1.1.7/tests/test_misc.py
+-rw-r--r--   0 mlandry    (501) staff       (20)     2671 2024-02-25 06:19:21.000000 pluralkit-1.1.7/tests/test_system.py
```

### Comparing `pluralkit-1.1.6/LICENSE` & `pluralkit-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/PKG-INFO` & `pluralkit-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralkit
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python wrapper for PluralKit's API.
 Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner
 Author-email: pkpy@mit.edu
 License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pluralkit Version: 1.1.6 Summary: Python wrapper
+Metadata-Version: 2.1 Name: pluralkit Version: 1.1.7 Summary: Python wrapper
 for PluralKit's API. Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner Author-email: pkpy@mit.edu License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
 Classifier: Development Status :: 3 - Alpha Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `pluralkit-1.1.6/README.md` & `pluralkit-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/docs/Makefile` & `pluralkit-1.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/docs/README.md` & `pluralkit-1.1.7/docs/README.md`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/docs/conf.py` & `pluralkit-1.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/docs/index.rst` & `pluralkit-1.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/docs/source/changelog.rst` & `pluralkit-1.1.7/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/docs/source/quickstart.rst` & `pluralkit-1.1.7/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/docs/source/v1/api.rst` & `pluralkit-1.1.7/docs/source/v1/api.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/docs/source/v2/api.rst` & `pluralkit-1.1.7/docs/source/v2/api.rst`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/pluralkit/v1/client.py` & `pluralkit-1.1.7/pluralkit/v1/client.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/pluralkit/v1/errors.py` & `pluralkit-1.1.7/pluralkit/v1/errors.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/pluralkit/v1/models.py` & `pluralkit-1.1.7/pluralkit/v1/models.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/pluralkit/v1/utils.py` & `pluralkit-1.1.7/pluralkit/v1/utils.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/pluralkit/v2/__init__.py` & `pluralkit-1.1.7/pluralkit/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/pluralkit/v2/client.py` & `pluralkit-1.1.7/pluralkit/v2/client.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/pluralkit/v2/errors.py` & `pluralkit-1.1.7/pluralkit/v2/errors.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/pluralkit/v2/models.py` & `pluralkit-1.1.7/pluralkit/v2/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,27 @@
 
 class PluralKitId(Model):
     """Base class for PluralKit IDs.
     """
     uuid: Optional[str]
     id: Optional[str]
 
+    _six_character_allowed = "abcefghjknoprstuvwxyz"
+    _six_character_pattern = re.compile(
+        f"^([{_six_character_allowed}]{{3}}-?[{_six_character_allowed}]{{3}})$",
+        re.IGNORECASE,
+    )
+
     __slots__ = ["uuid", "id"]
 
-    def _check_id(self, id):
-        return len(id) == 5 and all(c in ALPHABET for c in id)
+    def _check_id(self, id: str) -> bool:
+        # 5-character IDs
+        if len(id) == 5 and all(c in ALPHABET for c in id): return True
+        # 6-character IDs
+        return bool(self._six_character_pattern.match(id))
 
     def _check_uuid(self, uuid):
         pattern = r"[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}"
         result = re.match(pattern, uuid)
         return bool(result)
 
     def __init__(self, id=None, uuid=None):
@@ -117,23 +126,29 @@
             raise ValueError(f"{self.CONTEXT} ID object must include at least one of: id, uuid")
 
         # accept any order/combination of inputs
         object.__setattr__(self, "id", None)
         object.__setattr__(self, "uuid", None)
         if id is not None:
             if self._check_id(id):
+                if len(id) >= 6:
+                    id = id.lower()
+                    id = f"{id[:3]}-{id[-3:]}"
                 object.__setattr__(self, "id", id)
             elif self._check_uuid(id):
                 object.__setattr__(self, "uuid", id)
             else:
                 raise ValueError(f"Malformed id given: {id!r}")
         if uuid is not None:
             if self._check_uuid(uuid):
                 object.__setattr__(self, "uuid", uuid)
             elif self._check_id(uuid):
+                if len(uuid) >= 6:
+                    uuid = uuid.lower()
+                    uuid = f"{uuid[:3]}-{uuid[-3:]}"
                 object.__setattr__(self, "id", uuid)
             else:
                 raise ValueError(f"Malformed uuid given: {uuid!r}")
 
     def __setattr__(self, name, value):
         msg = f"cannot assign to field {name!r}"
         raise AttributeError(msg)
@@ -142,15 +157,20 @@
         return f"{self.uuid}" if self.uuid is not None else f"{self.id}"
 
     def __repr__(self):
         attrs = f"{self.id!r}"
         if self.uuid is not None: attrs += f", {self.uuid!r}"
         return f"{self.__class__.__name__}({attrs})"
 
-    json = __str__
+    def json(self) -> str:
+        return (
+            f"{self.uuid}"
+            if self.uuid is not None
+            else f"{self.id.replace('-', '')}"
+        )
 
 class MemberId(PluralKitId):
     """Member IDs.
     """
     CONTEXT = "Member"
 
 class SystemId(PluralKitId):
```

### Comparing `pluralkit-1.1.6/pluralkit.egg-info/PKG-INFO` & `pluralkit-1.1.7/pluralkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralkit
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python wrapper for PluralKit's API.
 Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner
 Author-email: pkpy@mit.edu
 License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pluralkit Version: 1.1.6 Summary: Python wrapper
+Metadata-Version: 2.1 Name: pluralkit Version: 1.1.7 Summary: Python wrapper
 for PluralKit's API. Home-page: https://github.com/almonds0166/pluralkit.py
 Author: Madison Landry, Alyx Warner Author-email: pkpy@mit.edu License: MIT
 Project-URL: Documentation, https://pluralkit.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/almonds0166/pluralkit.py/issues
 Classifier: Development Status :: 3 - Alpha Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `pluralkit-1.1.6/pluralkit.egg-info/SOURCES.txt` & `pluralkit-1.1.7/pluralkit.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pypi_api_token.txt
 setup.py
 docs/Makefile
 docs/README.md
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/source/changelog.rst
```

### Comparing `pluralkit-1.1.6/setup.py` & `pluralkit-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/tests/test_member.py` & `pluralkit-1.1.7/tests/test_member.py`

 * *Files identical despite different names*

### Comparing `pluralkit-1.1.6/tests/test_system.py` & `pluralkit-1.1.7/tests/test_system.py`

 * *Files identical despite different names*

