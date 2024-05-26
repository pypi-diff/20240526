# Comparing `tmp/shmessy-1.3.4.tar.gz` & `tmp/shmessy-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shmessy-1.3.4.tar", max compression
+gzip compressed data, was "shmessy-1.3.5.tar", max compression
```

## Comparing `shmessy-1.3.4.tar` & `shmessy-1.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1073 2024-05-23 07:25:38.222913 shmessy-1.3.4/LICENSE
--rw-r--r--   0        0        0     5669 2024-05-23 07:25:38.222913 shmessy-1.3.4/README.md
--rw-r--r--   0        0        0      863 2024-05-23 07:26:07.218920 shmessy-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     5701 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/__init__.py
--rw-r--r--   0        0        0     2023 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/exceptions.py
--rw-r--r--   0        0        0      395 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/schema.py
--rw-r--r--   0        0        0        0 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/__init__.py
--rw-r--r--   0        0        0     1037 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/base.py
--rw-r--r--   0        0        0     2226 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/boolean.py
--rw-r--r--   0        0        0     2532 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/date.py
--rw-r--r--   0        0        0     3084 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/datetime_.py
--rw-r--r--   0        0        0     1016 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/email.py
--rw-r--r--   0        0        0     1550 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/float.py
--rw-r--r--   0        0        0     1256 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/integer.py
--rw-r--r--   0        0        0     1272 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/ipv4_address.py
--rw-r--r--   0        0        0      991 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/string.py
--rw-r--r--   0        0        0     3188 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types/unix_timestamp.py
--rw-r--r--   0        0        0     7381 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/types_handler.py
--rw-r--r--   0        0        0     1848 2024-05-23 07:25:38.226913 shmessy-1.3.4/src/shmessy/utils.py
--rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 shmessy-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-26 06:23:04.957457 shmessy-1.3.5/LICENSE
+-rw-r--r--   0        0        0     5669 2024-05-26 06:23:04.957457 shmessy-1.3.5/README.md
+-rw-r--r--   0        0        0      863 2024-05-26 06:23:37.377555 shmessy-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     5701 2024-05-26 06:23:04.957457 shmessy-1.3.5/src/shmessy/__init__.py
+-rw-r--r--   0        0        0     2023 2024-05-26 06:23:04.957457 shmessy-1.3.5/src/shmessy/exceptions.py
+-rw-r--r--   0        0        0      395 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/schema.py
+-rw-r--r--   0        0        0        0 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/__init__.py
+-rw-r--r--   0        0        0     1037 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/base.py
+-rw-r--r--   0        0        0     2226 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/boolean.py
+-rw-r--r--   0        0        0     2532 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/date.py
+-rw-r--r--   0        0        0     3128 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/datetime_.py
+-rw-r--r--   0        0        0     1016 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/email.py
+-rw-r--r--   0        0        0     1550 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/float.py
+-rw-r--r--   0        0        0     1256 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/integer.py
+-rw-r--r--   0        0        0     1272 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/ipv4_address.py
+-rw-r--r--   0        0        0      991 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/string.py
+-rw-r--r--   0        0        0     3188 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types/unix_timestamp.py
+-rw-r--r--   0        0        0     7381 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/types_handler.py
+-rw-r--r--   0        0        0     1848 2024-05-26 06:23:04.961457 shmessy-1.3.5/src/shmessy/utils.py
+-rw-r--r--   0        0        0     6353 1970-01-01 00:00:00.000000 shmessy-1.3.5/PKG-INFO
```

### Comparing `shmessy-1.3.4/LICENSE` & `shmessy-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/README.md` & `shmessy-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/pyproject.toml` & `shmessy-1.3.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shmessy"
-version = "v1.3.4"
+version = "v1.3.5"
 description = "If your data is messy - Use Shmessy!"
 readme = "README.md"
 authors = ["Ohad Mata <ohadmata@gmail.com>"]
 homepage = "https://github.com/ohadmata/shmessy"
 repository = "https://github.com/ohadmata/shmessy"
 packages = [
     { include = "shmessy", from = "src" },
```

### Comparing `shmessy-1.3.4/src/shmessy/__init__.py` & `shmessy-1.3.5/src/shmessy/__init__.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/exceptions.py` & `shmessy-1.3.5/src/shmessy/exceptions.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types/base.py` & `shmessy-1.3.5/src/shmessy/types/base.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types/boolean.py` & `shmessy-1.3.5/src/shmessy/types/boolean.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types/date.py` & `shmessy-1.3.5/src/shmessy/types/date.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types/datetime_.py` & `shmessy-1.3.5/src/shmessy/types/datetime_.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         "%Y-%m-%dT%H:%M:%S.%f",  # 2022-12-30T00:00:00.000
         "%Y-%m-%d %H:%M:%S.%fZ",  # 2022-12-30 00:00:00.000Z
         "%Y-%m-%d %H:%M:%S.%f",  # 2022-12-30 00:00:00.000
         "%Y-%m-%dT%H:%M:%S.%fZ",  # 2022-12-30T00:00:00.000Z
         "%Y-%m-%dT%H:%M:%S",  # 2022-12-30T00:00:00
         "%d/%m/%Y %H:%M",  # 30/12/2022 00:00
         "%m/%d/%Y %H:%M",  # 12/30/2022 00:00
+        "%d/%m/%y %H:%M",  # 12/30/22 00:00
         "%Y-%m-%d %H:%M",  # 2020-09-24 11:57
         "%Y-%m-%d %H:%M:%S %Z",  # 2020-09-24 11:57:27 UTC
         "%Y-%m-%d %H:%M:%S %z",  # 2022-12-30 11:57:27 +00:00"
     ]
 
     def validate(self, data: ndarray) -> Optional[InferredField]:
         if data.dtype.type == np.dtype("datetime64"):
```

### Comparing `shmessy-1.3.4/src/shmessy/types/email.py` & `shmessy-1.3.5/src/shmessy/types/email.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types/float.py` & `shmessy-1.3.5/src/shmessy/types/float.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types/integer.py` & `shmessy-1.3.5/src/shmessy/types/integer.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types/ipv4_address.py` & `shmessy-1.3.5/src/shmessy/types/ipv4_address.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types/string.py` & `shmessy-1.3.5/src/shmessy/types/string.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types/unix_timestamp.py` & `shmessy-1.3.5/src/shmessy/types/unix_timestamp.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/types_handler.py` & `shmessy-1.3.5/src/shmessy/types_handler.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/src/shmessy/utils.py` & `shmessy-1.3.5/src/shmessy/utils.py`

 * *Files identical despite different names*

### Comparing `shmessy-1.3.4/PKG-INFO` & `shmessy-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shmessy
-Version: 1.3.4
+Version: 1.3.5
 Summary: If your data is messy - Use Shmessy!
 Home-page: https://github.com/ohadmata/shmessy
 Author: Ohad Mata
 Author-email: ohadmata@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

