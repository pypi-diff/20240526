# Comparing `tmp/aipkgs_notifications-1.0.1.tar.gz` & `tmp/aipkgs_notifications-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_notifications-1.0.1.tar", max compression
+gzip compressed data, was "aipkgs_notifications-1.0.2.tar", max compression
```

## Comparing `aipkgs_notifications-1.0.1.tar` & `aipkgs_notifications-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1058 2023-11-05 00:26:39.099971 aipkgs_notifications-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     3070 2023-12-11 22:43:30.104335 aipkgs_notifications-1.0.1/README.md
--rw-r--r--   0        0        0       51 2023-12-11 21:30:41.390034 aipkgs_notifications-1.0.1/aipkgs_notifications/__init__.py
--rw-r--r--   0        0        0      946 2023-11-25 23:01:16.403609 aipkgs_notifications-1.0.1/aipkgs_notifications/enums.py
--rw-r--r--   0        0        0     9396 2024-01-11 14:01:48.030045 aipkgs_notifications-1.0.1/aipkgs_notifications/ns.py
--rw-r--r--   0        0        0     5272 2024-01-23 17:29:09.843114 aipkgs_notifications-1.0.1/aipkgs_notifications/payload.py
--rw-r--r--   0        0        0     2122 2023-11-25 23:31:13.326810 aipkgs_notifications-1.0.1/aipkgs_notifications/response.py
--rw-r--r--   0        0        0      976 2023-11-02 20:50:24.863627 aipkgs_notifications-1.0.1/aipkgs_notifications/singleton.py
--rw-r--r--   0        0        0      122 2023-11-04 15:34:02.233847 aipkgs_notifications-1.0.1/aipkgs_notifications/utils.py
--rw-r--r--   0        0        0      662 2024-05-15 22:16:16.599556 aipkgs_notifications-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 aipkgs_notifications-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-11-05 00:26:39.099971 aipkgs_notifications-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     3070 2023-12-11 22:43:30.104335 aipkgs_notifications-1.0.2/README.md
+-rw-r--r--   0        0        0       51 2023-12-11 21:30:41.390034 aipkgs_notifications-1.0.2/aipkgs_notifications/__init__.py
+-rw-r--r--   0        0        0      946 2023-11-25 23:01:16.403609 aipkgs_notifications-1.0.2/aipkgs_notifications/enums.py
+-rw-r--r--   0        0        0     9396 2024-01-11 14:01:48.030045 aipkgs_notifications-1.0.2/aipkgs_notifications/ns.py
+-rw-r--r--   0        0        0     5272 2024-01-23 17:29:09.843114 aipkgs_notifications-1.0.2/aipkgs_notifications/payload.py
+-rw-r--r--   0        0        0     2122 2023-11-25 23:31:13.326810 aipkgs_notifications-1.0.2/aipkgs_notifications/response.py
+-rw-r--r--   0        0        0      976 2023-11-02 20:50:24.863627 aipkgs_notifications-1.0.2/aipkgs_notifications/singleton.py
+-rw-r--r--   0        0        0      122 2023-11-04 15:34:02.233847 aipkgs_notifications-1.0.2/aipkgs_notifications/utils.py
+-rw-r--r--   0        0        0      662 2024-05-26 16:10:23.556425 aipkgs_notifications-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 aipkgs_notifications-1.0.2/PKG-INFO
```

### Comparing `aipkgs_notifications-1.0.1/LICENSE.md` & `aipkgs_notifications-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-1.0.1/README.md` & `aipkgs_notifications-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-1.0.1/aipkgs_notifications/enums.py` & `aipkgs_notifications-1.0.2/aipkgs_notifications/enums.py`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-1.0.1/aipkgs_notifications/ns.py` & `aipkgs_notifications-1.0.2/aipkgs_notifications/ns.py`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-1.0.1/aipkgs_notifications/payload.py` & `aipkgs_notifications-1.0.2/aipkgs_notifications/payload.py`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-1.0.1/aipkgs_notifications/response.py` & `aipkgs_notifications-1.0.2/aipkgs_notifications/response.py`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-1.0.1/aipkgs_notifications/singleton.py` & `aipkgs_notifications-1.0.2/aipkgs_notifications/singleton.py`

 * *Files identical despite different names*

### Comparing `aipkgs_notifications-1.0.1/pyproject.toml` & `aipkgs_notifications-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aipkgs-notifications"
-version = "1.0.1"
+version = "1.0.2"
 description = "A simple package to send notifications to your devices using Firebase Cloud Messaging."
 authors = ["Alexy <alexy.ib@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/AlexyIbrahim/Notifications"
 repository = "https://github.com/AlexyIbrahim/Notifications"
 keywords = ["ai"]
```

### Comparing `aipkgs_notifications-1.0.1/PKG-INFO` & `aipkgs_notifications-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aipkgs-notifications
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple package to send notifications to your devices using Firebase Cloud Messaging.
 Home-page: https://github.com/AlexyIbrahim/Notifications
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.4,<4.0.0
```

