# Comparing `tmp/pyathena-3.8.2.tar.gz` & `tmp/pyathena-3.8.3.tar.gz`

## Comparing `pyathena-3.8.2.tar` & `pyathena-3.8.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/__init__.py
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/async_cursor.py
--rw-r--r--   0        0        0    23825 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/common.py
--rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/connection.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/converter.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/cursor.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/error.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/formatter.py
--rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/py.typed
--rw-r--r--   0        0        0    23041 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/result_set.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/arrow/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    43497 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13467 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0    10297 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/pandas/util.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/spark/__init__.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/spark/async_cursor.py
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/spark/common.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/spark/cursor.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    42007 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pyathena-3.8.2/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pyathena-3.8.2/LICENSE
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pyathena-3.8.2/README.rst
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pyathena-3.8.2/pyproject.toml
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pyathena-3.8.2/PKG-INFO
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/__init__.py
+-rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    23825 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/common.py
+-rw-r--r--   0        0        0    13290 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/connection.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/converter.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/cursor.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/error.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/formatter.py
+-rw-r--r--   0        0        0    22930 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/py.typed
+-rw-r--r--   0        0        0    23041 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/result_set.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     6854 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/arrow/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    44469 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13467 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0    10297 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/pandas/util.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/spark/__init__.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/spark/async_cursor.py
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/spark/common.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/spark/cursor.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    42007 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pyathena-3.8.3/.gitignore
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pyathena-3.8.3/LICENSE
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 pyathena-3.8.3/README.rst
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pyathena-3.8.3/pyproject.toml
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 pyathena-3.8.3/PKG-INFO
```

### Comparing `pyathena-3.8.2/pyathena/__init__.py` & `pyathena-3.8.3/pyathena/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection, ConnectionCursor
     from pyathena.cursor import Cursor
 
-__version__ = "3.8.2"
+__version__ = "3.8.3"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.8.2/pyathena/async_cursor.py` & `pyathena-3.8.3/pyathena/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/common.py` & `pyathena-3.8.3/pyathena/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/connection.py` & `pyathena-3.8.3/pyathena/connection.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/converter.py` & `pyathena-3.8.3/pyathena/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/cursor.py` & `pyathena-3.8.3/pyathena/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/error.py` & `pyathena-3.8.3/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/formatter.py` & `pyathena-3.8.3/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/model.py` & `pyathena-3.8.3/pyathena/model.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/result_set.py` & `pyathena-3.8.3/pyathena/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/util.py` & `pyathena-3.8.3/pyathena/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/arrow/async_cursor.py` & `pyathena-3.8.3/pyathena/arrow/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/arrow/converter.py` & `pyathena-3.8.3/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/arrow/cursor.py` & `pyathena-3.8.3/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/arrow/result_set.py` & `pyathena-3.8.3/pyathena/arrow/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/arrow/util.py` & `pyathena-3.8.3/pyathena/arrow/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/fastparquet/util.py` & `pyathena-3.8.3/pyathena/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/filesystem/s3.py` & `pyathena-3.8.3/pyathena/filesystem/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,22 +211,17 @@
             self.dircache[path] = file
         else:
             file = self.dircache[path]
         return file
 
     def _ls_buckets(self, refresh: bool = False) -> List[S3Object]:
         if "" not in self.dircache or refresh:
-            try:
-                response = self._call(
-                    self._client.list_buckets,
-                )
-            except botocore.exceptions.ClientError as e:
-                # if e.response["Error"]["Code"] in ["AccessDenied", "403"]:
-                #     return []
-                raise
+            response = self._call(
+                self._client.list_buckets,
+            )
             buckets = [
                 S3Object(
                     init={
                         "ContentLength": 0,
                         "ContentType": None,
                         "StorageClass": S3StorageClass.S3_STORAGE_CLASS_BUCKET,
                         "ETag": None,
@@ -548,14 +543,16 @@
         return object_.to_dict()
 
     def cp_file(self, path1: str, path2: str, **kwargs):
         bucket1, key1, version_id1 = self.parse_path(path1)
         bucket2, key2, version_id2 = self.parse_path(path2)
         if version_id2:
             raise ValueError("Cannot copy to a versioned file.")
+        if not key1 or not key2:
+            raise ValueError("Cannot copy buckets.")
 
         info1 = self.info(path1)
         size1 = info1.get("size", 0)
         if size1 <= self.MULTIPART_UPLOAD_MAX_PART_SIZE:
             self._copy_object(
                 bucket1=bucket1,
                 key1=key1,
@@ -660,37 +657,43 @@
                 parts.append(
                     {
                         "ETag": result.etag,
                         "PartNumber": result.part_number,
                     }
                 )
 
-        parts.sort(key=lambda x: x["PartNumber"])
+        parts.sort(key=lambda x: x["PartNumber"])  # type: ignore
         self._complete_multipart_upload(
             bucket=bucket2,
             key=key2,
             upload_id=cast(str, multipart_upload.upload_id),
             parts=parts,
         )
 
     def cat_file(
         self, path: str, start: Optional[int] = None, end: Optional[int] = None, **kwargs
     ) -> bytes:
         bucket, key, version_id = self.parse_path(path)
         if start is not None or end is not None:
             size = self.info(path).get("size", 0)
             if start is None:
-                start = 0
+                range_start = 0
             elif start < 0:
-                start = size + start
+                range_start = size + start
+            else:
+                range_start = start
+
             if end is None:
-                end = size
+                range_end = size
             elif end < 0:
-                end = size + end
-            ranges = (start, end)
+                range_end = size + end
+            else:
+                range_end = end
+
+            ranges = (range_start, range_end)
         else:
             ranges = None
 
         return self._get_object(
             bucket=bucket,
             key=cast(str, key),
             ranges=ranges,
@@ -1080,25 +1083,46 @@
 
         if not self.multipart_upload:
             raise RuntimeError("Multipart upload is not initialized.")
 
         part_number = len(self.multipart_upload_parts)
         self.buffer.seek(0)
         while data := self.buffer.read(self.blocksize):
-            part_number += 1
-            self.multipart_upload_parts.append(
-                self._executor.submit(
-                    self.fs._upload_part,
-                    bucket=self.bucket,
-                    key=self.key,
-                    upload_id=cast(str, self.multipart_upload.upload_id),
-                    part_number=part_number,
-                    body=data,
+            # The last part of a multipart request should be adjusted
+            # to be larger than the minimum part size.
+            next_data = self.buffer.read(self.blocksize)
+            next_data_size = len(next_data)
+            if 0 < next_data_size < self.fs.MULTIPART_UPLOAD_MIN_PART_SIZE:
+                upload_data = data + next_data
+                upload_data_size = len(upload_data)
+                if upload_data_size < self.fs.MULTIPART_UPLOAD_MAX_PART_SIZE:
+                    uploads = [upload_data]
+                else:
+                    split_size = upload_data_size // 2
+                    uploads = [upload_data[:split_size], upload_data[split_size:]]
+            else:
+                uploads = [data]
+                if next_data:
+                    uploads.append(next_data)
+
+            for upload in uploads:
+                part_number += 1
+                self.multipart_upload_parts.append(
+                    self._executor.submit(
+                        self.fs._upload_part,
+                        bucket=self.bucket,
+                        key=self.key,
+                        upload_id=cast(str, self.multipart_upload.upload_id),
+                        part_number=part_number,
+                        body=upload,
+                    )
                 )
-            )
+
+            if not next_data:
+                break
 
         if self.autocommit and final:
             self.commit()
         return True
 
     def commit(self) -> None:
         if self.tell() == 0:
```

### Comparing `pyathena-3.8.2/pyathena/filesystem/s3_object.py` & `pyathena-3.8.3/pyathena/filesystem/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/pandas/async_cursor.py` & `pyathena-3.8.3/pyathena/pandas/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/pandas/converter.py` & `pyathena-3.8.3/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/pandas/cursor.py` & `pyathena-3.8.3/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/pandas/result_set.py` & `pyathena-3.8.3/pyathena/pandas/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/pandas/util.py` & `pyathena-3.8.3/pyathena/pandas/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/spark/async_cursor.py` & `pyathena-3.8.3/pyathena/spark/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/spark/common.py` & `pyathena-3.8.3/pyathena/spark/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/spark/cursor.py` & `pyathena-3.8.3/pyathena/spark/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/sqlalchemy/arrow.py` & `pyathena-3.8.3/pyathena/sqlalchemy/arrow.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/sqlalchemy/base.py` & `pyathena-3.8.3/pyathena/sqlalchemy/base.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/sqlalchemy/pandas.py` & `pyathena-3.8.3/pyathena/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/sqlalchemy/requirements.py` & `pyathena-3.8.3/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyathena/sqlalchemy/types.py` & `pyathena-3.8.3/pyathena/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/LICENSE` & `pyathena-3.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/README.rst` & `pyathena-3.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/pyproject.toml` & `pyathena-3.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyathena-3.8.2/PKG-INFO` & `pyathena-3.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: PyAthena
-Version: 3.8.2
+Version: 3.8.3
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Project-URL: homepage, https://github.com/laughingman7743/PyAthena/
 Project-URL: repository, https://github.com/laughingman7743/PyAthena/
 Author-email: laughingman7743 <laughingman7743@gmail.com>
 License: Copyright 2017 laughingman7743
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

