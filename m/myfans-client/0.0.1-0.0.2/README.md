# Comparing `tmp/myfans_client-0.0.1.tar.gz` & `tmp/myfans_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfans_client-0.0.1.tar", max compression
+gzip compressed data, was "myfans_client-0.0.2.tar", max compression
```

## Comparing `myfans_client-0.0.1.tar` & `myfans_client-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1067 2024-05-24 14:02:51.268759 myfans_client-0.0.1/LICENSE
--rw-r--r--   0        0        0       47 2024-05-24 14:02:51.268759 myfans_client-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-24 14:02:51.268759 myfans_client-0.0.1/myfans_client/__init__.py
--rw-r--r--   0        0        0     5807 2024-05-24 14:02:51.268759 myfans_client-0.0.1/myfans_client/client.py
--rw-r--r--   0        0        0       86 2024-05-24 14:02:51.268759 myfans_client-0.0.1/myfans_client/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-24 14:02:51.268759 myfans_client-0.0.1/myfans_client/models/__init__.py
--rw-r--r--   0        0        0      311 2024-05-24 14:02:51.268759 myfans_client-0.0.1/myfans_client/models/follow.py
--rw-r--r--   0        0        0      806 2024-05-24 14:03:11.408968 myfans_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 myfans_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-26 16:26:00.361578 myfans_client-0.0.2/LICENSE
+-rw-r--r--   0        0        0       47 2024-05-26 16:26:00.361578 myfans_client-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/__init__.py
+-rw-r--r--   0        0        0     6475 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/client.py
+-rw-r--r--   0        0        0       86 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/models/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/models/follow.py
+-rw-r--r--   0        0        0     1160 2024-05-26 16:26:00.361578 myfans_client-0.0.2/myfans_client/models/user.py
+-rw-r--r--   0        0        0      806 2024-05-26 16:26:16.921711 myfans_client-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 myfans_client-0.0.2/PKG-INFO
```

### Comparing `myfans_client-0.0.1/LICENSE` & `myfans_client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myfans_client-0.0.1/myfans_client/client.py` & `myfans_client-0.0.2/myfans_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 from typing import Generator
 
 import httpx
 
 from myfans_client.exceptions import MyFansException
 from myfans_client.models.follow import FollowUser
+from myfans_client.models.user import UserProfile
 
 # https://api.myfans.jp/api/v2/users/f6257cde-61cc-428f-834b-c95d138d21fb/followers?page=1
 # https://api.myfans.jp/api/v2/users/show_by_username?username=XXXX
 
 
 class MyFansClient:
     def __init__(self, email: str, password: str, base_url: str = 'https://api.myfans.jp', debug: bool = False):
@@ -158,14 +159,34 @@
 
         is_followed = self._post(
             f'api/v1/users/{user_id}/unfollow',
             headers=self.header,
         )
         return is_followed
 
+    def show_by_username(self, username: str) -> UserProfile:
+        """
+        GET https://api.myfans.jp/api/v2/users/show_by_username?username=USERNAME
+        """
+        res = self._get(
+            f'api/v2/users/show_by_username?username={username}',
+            headers=self.header,
+        )
+        return UserProfile(**res)
+
+    def get_users(self, user_code: str) -> UserProfile:
+        """
+        GET https://api.myfans.jp/api/v1/users/USER_CODE
+        """
+        res = self._get(
+            f'api/v1/users/{user_code}',
+            headers=self.header,
+        )
+        return UserProfile(**res)
+
     def _post(self, path: str, *arg, **kwargs):
         return self._request('POST', path, *arg, **kwargs)
 
     def _get(self, path: str, *arg, **kwargs):
         return self._request('GET', path, *arg, **kwargs)
 
     def _put(self, path: str, *arg, **kwargs):
```

### Comparing `myfans_client-0.0.1/pyproject.toml` & `myfans_client-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "myfans-client"
-version = "0.0.1"  # using poetry-dynamic-versioning
+version = "0.0.2"  # using poetry-dynamic-versioning
 description = ""
 authors = ["komanushi <155377273+komanushi@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/komanushi/myfans-client"
 repository = "https://github.com/komanushi/myfans-client"
 keywords = ["API"]
```

### Comparing `myfans_client-0.0.1/PKG-INFO` & `myfans_client-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfans-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Home-page: https://github.com/komanushi/myfans-client
 License: MIT
 Keywords: API
 Author: komanushi
 Author-email: 155377273+komanushi@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

