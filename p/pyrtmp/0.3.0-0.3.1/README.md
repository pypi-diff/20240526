# Comparing `tmp/pyrtmp-0.3.0.tar.gz` & `tmp/pyrtmp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtmp-0.3.0.tar", last modified: Sun Dec 10 11:03:23 2023, max compression
+gzip compressed data, was "pyrtmp-0.3.1.tar", last modified: Sun May 26 07:11:44 2024, max compression
```

## Comparing `pyrtmp-0.3.0.tar` & `pyrtmp-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2023-12-10 11:03:23.027670 pyrtmp-0.3.0/
--rw-r--r--   0 eittipat   (501) staff       (20)     1066 2023-12-09 04:32:59.000000 pyrtmp-0.3.0/LICENSE.txt
--rw-r--r--   0 eittipat   (501) staff       (20)     5464 2023-12-10 11:03:23.027615 pyrtmp-0.3.0/PKG-INFO
--rw-r--r--   0 eittipat   (501) staff       (20)     4787 2023-12-10 10:57:01.000000 pyrtmp-0.3.0/README.md
-drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2023-12-10 11:03:23.023078 pyrtmp-0.3.0/pyrtmp/
--rw-r--r--   0 eittipat   (501) staff       (20)     2358 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/__init__.py
-drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2023-12-10 11:03:23.024393 pyrtmp-0.3.0/pyrtmp/amf/
--rw-r--r--   0 eittipat   (501) staff       (20)        0 2023-12-09 04:32:59.000000 pyrtmp-0.3.0/pyrtmp/amf/__init__.py
--rw-r--r--   0 eittipat   (501) staff       (20)     5577 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/amf/serializers.py
--rw-r--r--   0 eittipat   (501) staff       (20)      177 2023-12-10 04:55:45.000000 pyrtmp-0.3.0/pyrtmp/amf/types.py
--rw-r--r--   0 eittipat   (501) staff       (20)     2894 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/flv.py
-drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2023-12-10 11:03:23.026404 pyrtmp-0.3.0/pyrtmp/messages/
--rw-r--r--   0 eittipat   (501) staff       (20)     5835 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/messages/__init__.py
--rw-r--r--   0 eittipat   (501) staff       (20)       76 2023-12-09 04:32:59.000000 pyrtmp-0.3.0/pyrtmp/messages/aggregate.py
--rw-r--r--   0 eittipat   (501) staff       (20)      378 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/messages/audio.py
--rw-r--r--   0 eittipat   (501) staff       (20)     9605 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/messages/command.py
--rw-r--r--   0 eittipat   (501) staff       (20)     1304 2023-12-09 04:32:59.000000 pyrtmp-0.3.0/pyrtmp/messages/data.py
--rw-r--r--   0 eittipat   (501) staff       (20)     1649 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/messages/factory.py
--rw-r--r--   0 eittipat   (501) staff       (20)     2012 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/messages/handshake.py
--rw-r--r--   0 eittipat   (501) staff       (20)     3640 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/messages/protocol_control.py
--rw-r--r--   0 eittipat   (501) staff       (20)       80 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/messages/shared_object.py
--rw-r--r--   0 eittipat   (501) staff       (20)     6439 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/messages/user_control.py
--rw-r--r--   0 eittipat   (501) staff       (20)      379 2023-12-09 04:32:59.000000 pyrtmp-0.3.0/pyrtmp/messages/video.py
--rw-r--r--   0 eittipat   (501) staff       (20)     8522 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/rtmp.py
--rw-r--r--   0 eittipat   (501) staff       (20)     7338 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/pyrtmp/session_manager.py
-drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2023-12-10 11:03:23.023816 pyrtmp-0.3.0/pyrtmp.egg-info/
--rw-r--r--   0 eittipat   (501) staff       (20)     5464 2023-12-10 11:03:23.000000 pyrtmp-0.3.0/pyrtmp.egg-info/PKG-INFO
--rw-r--r--   0 eittipat   (501) staff       (20)      764 2023-12-10 11:03:23.000000 pyrtmp-0.3.0/pyrtmp.egg-info/SOURCES.txt
--rw-r--r--   0 eittipat   (501) staff       (20)        1 2023-12-10 11:03:23.000000 pyrtmp-0.3.0/pyrtmp.egg-info/dependency_links.txt
--rw-r--r--   0 eittipat   (501) staff       (20)       13 2023-12-10 11:03:23.000000 pyrtmp-0.3.0/pyrtmp.egg-info/requires.txt
--rw-r--r--   0 eittipat   (501) staff       (20)       13 2023-12-10 11:03:23.000000 pyrtmp-0.3.0/pyrtmp.egg-info/top_level.txt
--rw-r--r--   0 eittipat   (501) staff       (20)      131 2023-12-10 11:03:23.027837 pyrtmp-0.3.0/setup.cfg
--rw-r--r--   0 eittipat   (501) staff       (20)      809 2023-12-10 10:53:54.000000 pyrtmp-0.3.0/setup.py
-drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2023-12-10 11:03:23.027357 pyrtmp-0.3.0/tests/
--rw-r--r--   0 eittipat   (501) staff       (20)     1060 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/tests/__init__.py
--rw-r--r--   0 eittipat   (501) staff       (20)     2574 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/tests/test_demo_ffmpeg.py
--rw-r--r--   0 eittipat   (501) staff       (20)     2581 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/tests/test_demo_flvdump.py
--rw-r--r--   0 eittipat   (501) staff       (20)     2377 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/tests/test_demo_rtmpt.py
--rw-r--r--   0 eittipat   (501) staff       (20)     4534 2023-12-10 10:44:54.000000 pyrtmp-0.3.0/tests/test_pyrtmp.py
+drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2024-05-26 07:11:44.038280 pyrtmp-0.3.1/
+-rw-r--r--   0 eittipat   (501) staff       (20)     1066 2023-12-09 04:32:59.000000 pyrtmp-0.3.1/LICENSE.txt
+-rw-r--r--   0 eittipat   (501) staff       (20)     5471 2024-05-26 07:11:44.038177 pyrtmp-0.3.1/PKG-INFO
+-rw-r--r--   0 eittipat   (501) staff       (20)     4787 2023-12-10 10:57:01.000000 pyrtmp-0.3.1/README.md
+drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2024-05-26 07:11:44.033521 pyrtmp-0.3.1/pyrtmp/
+-rw-r--r--   0 eittipat   (501) staff       (20)     2441 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/__init__.py
+drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2024-05-26 07:11:44.035042 pyrtmp-0.3.1/pyrtmp/amf/
+-rw-r--r--   0 eittipat   (501) staff       (20)        0 2023-12-09 04:32:59.000000 pyrtmp-0.3.1/pyrtmp/amf/__init__.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     5547 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/amf/serializers.py
+-rw-r--r--   0 eittipat   (501) staff       (20)      175 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/amf/types.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     2862 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/flv.py
+drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2024-05-26 07:11:44.036945 pyrtmp-0.3.1/pyrtmp/messages/
+-rw-r--r--   0 eittipat   (501) staff       (20)     5790 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/__init__.py
+-rw-r--r--   0 eittipat   (501) staff       (20)       76 2023-12-09 04:32:59.000000 pyrtmp-0.3.1/pyrtmp/messages/aggregate.py
+-rw-r--r--   0 eittipat   (501) staff       (20)      378 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/audio.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     9597 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/command.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     1303 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/data.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     1659 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/factory.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     2090 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/handshake.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     3646 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/protocol_control.py
+-rw-r--r--   0 eittipat   (501) staff       (20)       79 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/shared_object.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     6431 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/user_control.py
+-rw-r--r--   0 eittipat   (501) staff       (20)      378 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/messages/video.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     8962 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/rtmp.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     7437 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/pyrtmp/session_manager.py
+drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2024-05-26 07:11:44.034529 pyrtmp-0.3.1/pyrtmp.egg-info/
+-rw-r--r--   0 eittipat   (501) staff       (20)     5471 2024-05-26 07:11:44.000000 pyrtmp-0.3.1/pyrtmp.egg-info/PKG-INFO
+-rw-r--r--   0 eittipat   (501) staff       (20)      764 2024-05-26 07:11:44.000000 pyrtmp-0.3.1/pyrtmp.egg-info/SOURCES.txt
+-rw-r--r--   0 eittipat   (501) staff       (20)        1 2024-05-26 07:11:44.000000 pyrtmp-0.3.1/pyrtmp.egg-info/dependency_links.txt
+-rw-r--r--   0 eittipat   (501) staff       (20)       20 2024-05-26 07:11:44.000000 pyrtmp-0.3.1/pyrtmp.egg-info/requires.txt
+-rw-r--r--   0 eittipat   (501) staff       (20)       13 2024-05-26 07:11:44.000000 pyrtmp-0.3.1/pyrtmp.egg-info/top_level.txt
+-rw-r--r--   0 eittipat   (501) staff       (20)      131 2024-05-26 07:11:44.038465 pyrtmp-0.3.1/setup.cfg
+-rw-r--r--   0 eittipat   (501) staff       (20)      803 2024-05-26 07:00:26.000000 pyrtmp-0.3.1/setup.py
+drwxr-xr-x   0 eittipat   (501) staff       (20)        0 2024-05-26 07:11:44.037747 pyrtmp-0.3.1/tests/
+-rw-r--r--   0 eittipat   (501) staff       (20)     1065 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/tests/__init__.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     2573 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/tests/test_demo_ffmpeg.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     2580 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/tests/test_demo_flvdump.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     2376 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/tests/test_demo_rtmpt.py
+-rw-r--r--   0 eittipat   (501) staff       (20)     4576 2024-05-26 06:41:43.000000 pyrtmp-0.3.1/tests/test_pyrtmp.py
```

### Comparing `pyrtmp-0.3.0/LICENSE.txt` & `pyrtmp-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrtmp-0.3.0/PKG-INFO` & `pyrtmp-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtmp
-Version: 0.3.0
+Version: 0.3.1
 Summary: PyRTMP: Pure Python RTMP server
 Home-page: https://github.com/Eittipat/pyrtmp.git
 Download-URL: https://github.com/Eittipat/pyrtmp/releases/tag/v0.3.0
 Author: Eittipat.K
 Author-email: iammop@gmail.com
 License: MIT
 Keywords: RTMP,RTMPT,asyncio
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: bitstring>=4
+Requires-Dist: bitstring<4.2,>=4.1
 
 # PyRTMP: Pure Python RTMP server
 ![coverage](https://github.com/Eittipat/pyrtmp/blob/master/coverage.svg)
 ## Features
 
 - ✅ Pure Python
 - ✅ Easy to customize
```

### Comparing `pyrtmp-0.3.0/README.md` & `pyrtmp-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrtmp-0.3.0/pyrtmp/__init__.py` & `pyrtmp-0.3.1/pyrtmp/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import os
 from asyncio import StreamReader, WriteTransport
+from collections.abc import Mapping
 from io import BytesIO
-from typing import Any, List, Optional, Mapping
+from typing import Any
+
 from bitstring import BitStream
+from bitstring.bits import Bits
 from bitstring.utils import tokenparser
 
 
 def random_byte_array(size: int) -> bytes:
     return os.urandom(size)
 
 
 class StreamClosedException(Exception):
     pass
 
 
 class BitStreamReader:
-
     def __init__(self, reader: StreamReader) -> None:
         self.reader = reader
         self.buffer = BitStream()
         self.total_bytes = 0
         super().__init__()
 
-    async def read(self, fmt):
+    async def read(self, fmt) -> int | float | str | Bits | bool | bytes | None:
         _, token = tokenparser(fmt)
         assert len(token) == 1
         name, length, _ = token[0]
         assert length is not None
 
         bit_needed = int(length) - (self.buffer.length - self.buffer.pos)
         while bit_needed > 0:
@@ -45,31 +47,30 @@
     def _append(self, data: bytes) -> None:
         pos = self.buffer.pos
         self.buffer.append(data)
         self.buffer.pos = pos
 
 
 class BufferedWriteTransport(WriteTransport):
-
-    def __init__(self, buffer: BytesIO, extra: Optional[Mapping[Any, Any]] = ...) -> None:
+    def __init__(self, buffer: BytesIO, extra: Mapping[Any, Any] | None = ...) -> None:
         self._buffer = buffer
         self._closing = False
         self._closed = False
         super().__init__(extra)
 
-    def set_write_buffer_limits(self, high: Optional[int] = ..., low: Optional[int] = ...) -> None:
+    def set_write_buffer_limits(self, high: int | None = ..., low: int | None = ...) -> None:
         raise NotImplementedError
 
     def get_write_buffer_size(self) -> int:
         raise NotImplementedError
 
     def write(self, data: Any) -> None:
         self._buffer.write(data)
 
-    def writelines(self, list_of_data: List[Any]) -> None:
+    def writelines(self, list_of_data: list[Any]) -> None:
         raise NotImplementedError
 
     def write_eof(self) -> None:
         raise NotImplementedError
 
     def can_write_eof(self) -> bool:
         return False
```

### Comparing `pyrtmp-0.3.0/pyrtmp/amf/serializers.py` & `pyrtmp-0.3.1/pyrtmp/amf/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from typing import Any, Dict, List
+from typing import Any
 
-from bitstring import BitStream, BitArray
+from bitstring import BitArray, BitStream
 
 from pyrtmp.amf.types import AMF0
 
 
 class AMF0Serializer:
-
     @classmethod
     def create_object(cls, data: BitStream, value):
         if isinstance(value, str):
             cls.write_string_object(data, value)
         elif isinstance(value, bool):
             cls.write_boolean_object(data, value)
         elif isinstance(value, float):
             cls.write_number_object(data, value)
         elif isinstance(value, int):
             cls.write_number_object(data, value)
-        elif isinstance(value, Dict):
+        elif isinstance(value, dict):
             cls.write_object_object(data, value)
-        elif isinstance(value, List):
+        elif isinstance(value, list):
             cls.write_array_object(data, value)
         elif value is None:
             cls.write_null_object(data)
         else:
             raise NotImplementedError
 
     @classmethod
@@ -51,45 +50,44 @@
     @classmethod
     def write_null_object(cls, data: BitStream):
         pos = data.pos
         data.append(BitArray(uint=AMF0.NULL, length=8))
         data.pos = pos
 
     @classmethod
-    def write_object_object(cls, data: BitStream, value: Dict):
+    def write_object_object(cls, data: BitStream, value: dict):
         pos = data.pos
         data.append(BitArray(uint=AMF0.OBJECT, length=8))
         for k, v in value.items():
             data.append(BitArray(uint=len(k), length=16))
             data.append(BitArray(bytes=k.encode(), length=len(k) * 8))
             cls.create_object(data, v)
         data.append(BitArray(uint=AMF0.OBJECT_END, length=24))
         data.pos = pos
 
     @classmethod
-    def write_array_object(cls, data: BitStream, value: List):
+    def write_array_object(cls, data: BitStream, value: list):
         pos = data.pos
         data.append(BitArray(uint=AMF0.ARRAY, length=8))
         data.append(BitArray(uint=len(value), length=32))
         for item in value:
             for key in item:
                 property_key = key.encode()
                 data.append(BitArray(uint=len(property_key), length=16))
                 data.append(BitArray(bytes=property_key, length=len(property_key) * 8))
                 cls.create_object(data, item[key])
         data.append(BitArray(uint=AMF0.OBJECT_END, length=24))
         data.pos = pos
 
 
 class AMF0Deserializer:
-
     @classmethod
     def from_stream(cls, data: BitStream) -> Any:
         # determine object type
-        obj_type = data.peek('uint:8')
+        obj_type = data.peek("uint:8")
         if obj_type == AMF0.STRING:
             return cls.to_string_object(data)
         if obj_type == AMF0.NUMBER:
             return cls.to_number_object(data)
         if obj_type == AMF0.OBJECT:
             return cls.to_object_object(data)
         if obj_type == AMF0.NULL:
@@ -98,61 +96,61 @@
             return cls.to_array_object(data)
         if obj_type == AMF0.BOOLEAN:
             return cls.to_boolean_object(data)
         raise NotImplementedError
 
     @classmethod
     def to_boolean_object(cls, data: BitStream):
-        obj_type = data.read('uint:8')
+        obj_type = data.read("uint:8")
         assert obj_type == AMF0.BOOLEAN
-        value = data.read('uint:8')
+        value = data.read("uint:8")
         return False if value == 0 else True
 
     @classmethod
     def to_string_object(cls, data: BitStream):
-        obj_type = data.read('uint:8')
+        obj_type = data.read("uint:8")
         assert obj_type == AMF0.STRING
-        obj_length = data.read('uint:16')
-        return data.read(f'bytes:{obj_length}').decode()
+        obj_length = data.read("uint:16")
+        return data.read(f"bytes:{obj_length}").decode()
 
     @classmethod
     def to_number_object(cls, data: BitStream):
-        obj_type = data.read('uint:8')
+        obj_type = data.read("uint:8")
         assert obj_type == AMF0.NUMBER
-        return data.read('float:64')
+        return data.read("float:64")
 
     @classmethod
     def to_null_object(cls, data: BitStream):
-        obj_type = data.read('uint:8')
+        obj_type = data.read("uint:8")
         assert obj_type == AMF0.NULL
         return None
 
     @classmethod
     def to_object_object(cls, data: BitStream):
-        obj_type = data.read('uint:8')
+        obj_type = data.read("uint:8")
         assert obj_type == AMF0.OBJECT
         obj = {}
-        ending = "0000{:02x}".format(int(AMF0.OBJECT_END))
-        while data.peek('bytes:3').hex() != ending:
+        ending = f"0000{int(AMF0.OBJECT_END):02x}"
+        while data.peek("bytes:3").hex() != ending:
             # read property name
-            size = data.read('uint:16')
-            property_name = data.read(f'bytes:{size}').decode()
+            size = data.read("uint:16")
+            property_name = data.read(f"bytes:{size}").decode()
             # read object value (AMF0)
             property_value = cls.from_stream(data)
             obj[property_name] = property_value
         return obj
 
     @classmethod
     def to_array_object(cls, data: BitStream):
-        obj_type = data.read('uint:8')
+        obj_type = data.read("uint:8")
         assert obj_type == AMF0.ARRAY
         arr = []
-        count = data.read('uint:32')
-        ending = "0000{:02x}".format(int(AMF0.OBJECT_END))
-        while data.peek('bytes:3').hex() != ending:
-            size = data.read('uint:16')
-            property_name = data.read(f'bytes:{size}').decode()
+        count = data.read("uint:32")
+        ending = f"0000{int(AMF0.OBJECT_END):02x}"
+        while data.peek("bytes:3").hex() != ending:
+            size = data.read("uint:16")
+            property_name = data.read(f"bytes:{size}").decode()
             # read object value (AMF0)
             property_value = cls.from_stream(data)
             arr.append({property_name: property_value})
         assert len(arr) == count
         return arr
```

### Comparing `pyrtmp-0.3.0/pyrtmp/flv.py` & `pyrtmp-0.3.1/pyrtmp/flv.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 import enum
-from typing import BinaryIO
 
-from bitstring import BitStream, BitArray
+from bitstring import BitArray, BitStream
 
 
 class FLVTag:
-
     def __init__(self, stream: BitStream) -> None:
-        self.tag_type = stream.read('uint:8')
-        self.data_size = stream.read('uint:24')
-        self.timestamp = stream.read('bytes:3')
-        self.timestamp_ext = stream.read('bytes:1')
-        self.stream_id = stream.read('uint:24')
+        self.tag_type = stream.read("uint:8")
+        self.data_size = stream.read("uint:24")
+        self.timestamp = stream.read("bytes:3")
+        self.timestamp_ext = stream.read("bytes:1")
+        self.stream_id = stream.read("uint:24")
         super().__init__()
 
     @property
     def total_timestamp(self) -> int:
         return BitArray(self.timestamp_ext + self.timestamp).int
 
 
 class RawAudio:
-
     def __init__(self, stream: BitStream) -> None:
-        format = stream.read('uint:4')
+        format = stream.read("uint:4")
         assert format == 3
-        sampling = stream.read('uint:2')
+        sampling = stream.read("uint:2")
         assert sampling == 2
-        size = stream.read('uint:1')
+        size = stream.read("uint:1")
         assert size == 1
-        channel = stream.read('uint:1')
+        channel = stream.read("uint:1")
         assert channel == 0
-        self.bytes = stream.read('bytes')
+        self.bytes = stream.read("bytes")
 
         # new
         input = BitStream(self.bytes)
         self.pcm = []
         while input.pos < input.length:
-            self.pcm.append(input.read('intle:16'))
+            self.pcm.append(input.read("intle:16"))
 
 
 class FLVMediaType(int, enum.Enum):
     AUDIO = 8
     VIDEO = 9
     OBJECT = 18
 
 
 class FLVWriter:
-
     def __init__(self) -> None:
         self.prev_tag_size = 0
         super().__init__()
 
     def write_header(self) -> bytes:
         stream = BitStream()
-        stream.append(b'FLV')
+        stream.append(b"FLV")
         stream.append(BitStream(uint=1, length=8))
         stream.append(BitStream(uint=5, length=8))
         stream.append(BitStream(uint=9, length=32))
         stream.append(BitStream(uint=self.prev_tag_size, length=32))
         return stream.bytes
 
     def write(self, timestamp: int, payload: bytes, media_type: FLVMediaType) -> bytes:
@@ -80,17 +76,16 @@
         stream.append(payload)
         # prev tag size
         stream.append(BitArray(uint=self.prev_tag_size, length=32))
         return stream.bytes
 
 
 class FLVFileWriter:
-
     def __init__(self, output: str) -> None:
-        self.buffer = open(output, 'wb')
+        self.buffer = open(output, "wb")
         self.writer = FLVWriter()
         self.buffer.write(self.writer.write_header())
         super().__init__()
 
     def write(self, timestamp: int, payload: bytes, media_type: FLVMediaType):
         self.buffer.write(self.writer.write(timestamp, payload, media_type))
         self.buffer.flush()
```

### Comparing `pyrtmp-0.3.0/pyrtmp/messages/__init__.py` & `pyrtmp-0.3.1/pyrtmp/messages/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
-from typing import Iterable
-from bitstring import BitStream, BitArray
 
 import logging
+from collections.abc import Iterable
+
+from bitstring import BitArray, BitStream
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class BaseChunk:
     chunk_type: int
@@ -14,22 +15,22 @@
     timestamp: int
     msg_length: int
     msg_type_id: int
     msg_stream_id: int
     payload: bytes
 
     def __init__(
-            self,
-            chunk_type: int,
-            chunk_id: int,
-            timestamp: int,
-            msg_length: int,
-            msg_type_id: int,
-            msg_stream_id: int,
-            payload: bytes,
+        self,
+        chunk_type: int,
+        chunk_id: int,
+        timestamp: int,
+        msg_length: int,
+        msg_type_id: int,
+        msg_stream_id: int,
+        payload: bytes,
     ) -> None:
         self.chunk_type = chunk_type
         self.chunk_id = chunk_id
         self.timestamp = timestamp
         self.msg_length = msg_length
         self.msg_type_id = msg_type_id
         self.msg_stream_id = msg_stream_id
@@ -45,28 +46,28 @@
         buffer += f"msg_type_id: {self.msg_type_id},"
         buffer += f"msg_stream_id: {self.msg_stream_id},"
         buffer += f"payload: {len(self.payload)})"
         return buffer
 
 
 class RawChunk(BaseChunk):
-    raw_chunk_number: int = 0,
-    is_eof: bool = False,
+    raw_chunk_number: int = (0,)
+    is_eof: bool = (False,)
 
     def __init__(
-            self,
-            chunk_type: int,
-            chunk_id: int,
-            timestamp: int,
-            msg_length: int,
-            msg_type_id: int,
-            msg_stream_id: int,
-            payload: bytes,
-            raw_chunk_number: int = 0,
-            is_eof: bool = False,
+        self,
+        chunk_type: int,
+        chunk_id: int,
+        timestamp: int,
+        msg_length: int,
+        msg_type_id: int,
+        msg_stream_id: int,
+        payload: bytes,
+        raw_chunk_number: int = 0,
+        is_eof: bool = False,
     ) -> None:
         super().__init__(
             chunk_type=chunk_type,
             chunk_id=chunk_id,
             timestamp=timestamp,
             msg_length=msg_length,
             msg_type_id=msg_type_id,
@@ -121,15 +122,14 @@
 
         stream.append(self.payload)
 
         return stream.bytes
 
 
 class Chunk(BaseChunk):
-
     def print_debug(self):
         logger.debug(f"======{self.__class__}======")
         for key in self.__dict__.keys():
             if key.startswith("_"):
                 continue
 
             value = self.__dict__[key]
@@ -161,13 +161,14 @@
                 chunk_id=self.chunk_id,
                 timestamp=timedelta,
                 msg_length=self.msg_length,
                 msg_type_id=self.msg_type_id,
                 msg_stream_id=self.msg_stream_id,
                 payload=payload[:bytes_length],
                 raw_chunk_number=chunk_number,
-                is_eof=is_eof)
+                is_eof=is_eof,
+            )
             chunks.append(raw_chunk)
             chunk_number += 1
             chunk_type = 3  # next raw chunk always 3
             payload = payload[bytes_length:]
         return chunks
```

### Comparing `pyrtmp-0.3.0/pyrtmp/messages/command.py` & `pyrtmp-0.3.1/pyrtmp/messages/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from pyrtmp.messages import Chunk
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class CommandMessage(Chunk):
-
     def __init__(self, command_name: str, **kwargs):
         super().__init__(**kwargs)
         self.command_name = command_name
 
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
@@ -56,21 +55,20 @@
             command_name=signature,
             **chunk.__dict__,
         )
         return instance
 
 
 class NCConnect(NetConnectionCommand):
-
     def __init__(
-            self,
-            transaction_id: int,
-            command_object: dict,
-            optional_user_arguments: dict | None,
-            **kwargs,
+        self,
+        transaction_id: int,
+        command_object: dict,
+        optional_user_arguments: dict | None,
+        **kwargs,
     ):
         super().__init__(**kwargs)
         self.transaction_id = transaction_id
         self.command_object = command_object
         self.optional_user_arguments = optional_user_arguments
 
     @classmethod
@@ -93,24 +91,30 @@
 
     def create_response(self) -> Chunk:
         data = BitStream()
 
         # payload
         AMF0Serializer.create_object(data, "_result")
         AMF0Serializer.create_object(data, 1)
-        AMF0Serializer.create_object(data, {
-            "fmsVer": "FMS/3,0,123",
-            "capabilities": 31,
-        })
-        AMF0Serializer.create_object(data, {
-            "level": "status",
-            "code": "NetConnection.Connect.Success",
-            "description": "Connection succeeds",
-            "objectEncoding": 0,
-        })
+        AMF0Serializer.create_object(
+            data,
+            {
+                "fmsVer": "FMS/3,0,123",
+                "capabilities": 31,
+            },
+        )
+        AMF0Serializer.create_object(
+            data,
+            {
+                "level": "status",
+                "code": "NetConnection.Connect.Success",
+                "description": "Connection succeeds",
+                "objectEncoding": 0,
+            },
+        )
 
         return Chunk(
             chunk_type=0,
             chunk_id=self.chunk_id,
             timestamp=0,
             msg_length=len(data.bytes),
             msg_type_id=0x14,
@@ -124,15 +128,14 @@
 
 
 class NCClose(NetConnectionCommand):
     pass
 
 
 class NCCreateStream(NetConnectionCommand):
-
     def __init__(self, transaction_id: int, command_object: dict, **kwargs):
         super().__init__(**kwargs)
         self.transaction_id = transaction_id
         self.command_object = command_object
 
     @classmethod
     def from_chunk(cls, chunk: Chunk):
@@ -204,21 +207,20 @@
 
 
 class NSPlay2(NetConnectionCommand):
     pass
 
 
 class NSDeleteStream(NetConnectionCommand):
-
     def __init__(
-            self,
-            stream_id: int,
-            transaction_id: int,
-            command_object: dict,
-            **kwargs,
+        self,
+        stream_id: int,
+        transaction_id: int,
+        command_object: dict,
+        **kwargs,
     ):
         super().__init__(**kwargs)
         self.stream_id = stream_id
         self.transaction_id = transaction_id
         self.command_object = command_object
 
     @classmethod
@@ -234,20 +236,19 @@
             command_object=command_object,
             stream_id=stream_id,
             **chunk.__dict__,
         )
 
 
 class NSCloseStream(NetConnectionCommand):
-
     def __init__(
-            self,
-            transaction_id: int,
-            command_object: dict,
-            **kwargs,
+        self,
+        transaction_id: int,
+        command_object: dict,
+        **kwargs,
     ):
         super().__init__(**kwargs)
         self.transaction_id = transaction_id
         self.command_object = command_object
 
     @classmethod
     def from_chunk(cls, chunk: Chunk):
@@ -268,22 +269,21 @@
 
 
 class NSReceiveVideo(NetConnectionCommand):
     pass
 
 
 class NSPublish(NetConnectionCommand):
-
     def __init__(
-            self,
-            transaction_id: int,
-            command_object: dict,
-            publishing_name: str,
-            publishing_type: str,
-            **kwargs,
+        self,
+        transaction_id: int,
+        command_object: dict,
+        publishing_name: str,
+        publishing_type: str,
+        **kwargs,
     ):
         super().__init__(**kwargs)
         self.transaction_id = transaction_id
         self.command_object = command_object
         self.publishing_name = publishing_name
         self.publishing_type = publishing_type
 
@@ -307,19 +307,17 @@
     def create_response(self) -> Chunk:
         data = BitStream()
 
         # payload
         AMF0Serializer.create_object(data, "onStatus")
         AMF0Serializer.create_object(data, 0)
         AMF0Serializer.create_object(data, None)
-        AMF0Serializer.create_object(data, {
-            "level": "status",
-            "code": "NetStream.Publish.Start",
-            "description": "Start publishing"
-        })
+        AMF0Serializer.create_object(
+            data, {"level": "status", "code": "NetStream.Publish.Start", "description": "Start publishing"}
+        )
 
         return Chunk(
             chunk_type=0,
             chunk_id=3,
             timestamp=0,
             msg_length=len(data.bytes),
             msg_type_id=0x14,
```

### Comparing `pyrtmp-0.3.0/pyrtmp/messages/data.py` & `pyrtmp-0.3.1/pyrtmp/messages/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         logger.warning(f"Unknown data message '{signature}', use default parser")
         instance = cls(**chunk.__dict__)
         instance.command_name = signature
         return instance
 
 
 class MetaDataMessage(DataMessage):
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         instance = cls(**chunk.__dict__)
         data = BitStream(instance.payload)
         instance.command_name = AMF0Deserializer.from_stream(data)
         instance.event = AMF0Deserializer.from_stream(data)
         instance.meta = AMF0Deserializer.from_stream(data)
```

### Comparing `pyrtmp-0.3.0/pyrtmp/messages/factory.py` & `pyrtmp-0.3.1/pyrtmp/messages/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from pyrtmp.messages import Chunk
 from pyrtmp.messages.audio import AudioMessage
 from pyrtmp.messages.command import CommandMessage
 from pyrtmp.messages.data import DataMessage
 from pyrtmp.messages.protocol_control import (
-    SetChunkSize, AbortMessage, Acknowledgement,
-    WindowAcknowledgementSize, SetPeerBandwidth,
+    AbortMessage,
+    Acknowledgement,
+    SetChunkSize,
+    SetPeerBandwidth,
+    WindowAcknowledgementSize,
 )
 from pyrtmp.messages.user_control import UserControlMessage
 from pyrtmp.messages.video import VideoMessage
 
 
 class MessageFactory:
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
-
         # protocol control message
         if chunk.msg_type_id == 0x01:
             return SetChunkSize.from_chunk(chunk)
         if chunk.msg_type_id == 0x02:
             return AbortMessage.from_chunk(chunk)
         if chunk.msg_type_id == 0x03:
             return Acknowledgement.from_chunk(chunk)
```

### Comparing `pyrtmp-0.3.0/pyrtmp/messages/handshake.py` & `pyrtmp-0.3.1/pyrtmp/messages/handshake.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,65 @@
-from bitstring import BitStream, BitArray
+from __future__ import annotations
+
+from bitstring import BitArray, BitStream
 
 from pyrtmp import BitStreamReader
 
 
 class C0:
-
     def __init__(self, protocol_version: int) -> None:
         self.protocol_version = protocol_version
         super().__init__()
 
     @classmethod
-    async def from_stream(cls, stream: BitStreamReader):
-        protocol_version = await stream.read('uint:8')
+    async def from_stream(cls, stream: BitStreamReader) -> C0:
+        protocol_version = await stream.read("uint:8")
         return cls(protocol_version=protocol_version)
 
-    def to_bytes(self):
+    def to_bytes(self) -> bytes:
         stream = BitStream()
         stream.append(BitArray(uint=self.protocol_version, length=8))
         return stream.bytes
 
 
 class C1:
-
     def __init__(self, time: int, zero: int, random: bytes) -> None:
         self.time = time
         self.zero = zero
         self.random = random
         super().__init__()
 
     @classmethod
-    async def from_stream(cls, stream: BitStreamReader):
-        time = await stream.read('uint:32')
-        zero = await stream.read('uint:32')
-        rand = await stream.read('bytes:1528')
+    async def from_stream(cls, stream: BitStreamReader) -> C1:
+        time = await stream.read("uint:32")
+        zero = await stream.read("uint:32")
+        rand = await stream.read("bytes:1528")
         return cls(time=time, zero=zero, random=rand)
 
-    def to_bytes(self):
+    def to_bytes(self) -> bytes:
         stream = BitStream()
         stream.append(BitArray(uint=self.time, length=32))
         stream.append(BitArray(uint=self.zero, length=32))
         stream.append(BitArray(bytes=self.random, length=1528 * 8))
         return stream.bytes
 
 
 class C2:
-
     def __init__(self, time1: int, time2: int, random: bytes) -> None:
         self.time1 = time1
         self.time2 = time2
         self.random = random
         super().__init__()
 
     @classmethod
-    async def from_stream(cls, stream: BitStreamReader):
-        time1 = await stream.read('uint:32')
-        time2 = await stream.read('uint:32')
-        rand = await stream.read('bytes:1528')
+    async def from_stream(cls, stream: BitStreamReader) -> C2:
+        time1 = await stream.read("uint:32")
+        time2 = await stream.read("uint:32")
+        rand = await stream.read("bytes:1528")
         return cls(time1=time1, time2=time2, random=rand)
 
-    def to_bytes(self):
+    def to_bytes(self) -> bytes:
         stream = BitStream()
         stream.append(BitArray(uint=self.time1, length=32))
         stream.append(BitArray(uint=self.time2, length=32))
         stream.append(BitArray(bytes=self.random, length=1528 * 8))
         return stream.bytes
```

### Comparing `pyrtmp-0.3.0/pyrtmp/messages/protocol_control.py` & `pyrtmp-0.3.1/pyrtmp/messages/protocol_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from bitstring import BitStream, BitArray
+from bitstring import BitArray, BitStream
+
 from pyrtmp.messages import Chunk
 
 
 class ProtocolControlMessage(Chunk):
     pass
 
 
 class SetChunkSize(ProtocolControlMessage):
-
     def __init__(self, chunk_size: int):
         assert 1 <= chunk_size <= 2147483647
         payload = BitStream()
         payload.append(BitArray(uint=chunk_size, length=32))
         super().__init__(
             chunk_id=2,
             chunk_type=0,
@@ -22,20 +22,19 @@
             payload=payload.bytes,
         )
         self.chunk_size = chunk_size
 
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
-        instance = cls(chunk_size=data.read('uint:32'))
+        instance = cls(chunk_size=data.read("uint:32"))
         return instance
 
 
 class AbortMessage(ProtocolControlMessage):
-
     def __init__(self, chunk_stream_id: int):
         payload = BitStream()
         payload.append(BitArray(uint=chunk_stream_id, length=32))
         super().__init__(
             chunk_id=2,
             chunk_type=0,
             timestamp=0,
@@ -45,20 +44,19 @@
             payload=payload.bytes,
         )
         self.chunk_stream_id = chunk_stream_id
 
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
-        instance = cls(chunk_stream_id=data.read('uint:32'))
+        instance = cls(chunk_stream_id=data.read("uint:32"))
         return instance
 
 
 class Acknowledgement(ProtocolControlMessage):
-
     def __init__(self, seq_number: int):
         payload = BitStream()
         payload.append(BitArray(uint=seq_number, length=32))
         super().__init__(
             chunk_id=2,
             chunk_type=0,
             timestamp=0,
@@ -68,42 +66,41 @@
             payload=payload.bytes,
         )
         self.seq_number = seq_number
 
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
-        instance = cls(seq_number=data.read('uint:32'))
+        instance = cls(seq_number=data.read("uint:32"))
         return instance
 
 
 class WindowAcknowledgementSize(ProtocolControlMessage):
-
     def __init__(self, ack_window_size: int):
         payload = BitStream()
         payload.append(BitArray(uint=ack_window_size, length=32))
         super().__init__(
             chunk_id=2,
             chunk_type=0,
             timestamp=0,
             msg_length=len(payload.bytes),
             msg_type_id=0x05,
             msg_stream_id=0,
-            payload=payload.bytes)
+            payload=payload.bytes,
+        )
         self.ack_window_size = ack_window_size
 
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
-        instance = cls(ack_window_size=data.read('uint:32'))
+        instance = cls(ack_window_size=data.read("uint:32"))
         return instance
 
 
 class SetPeerBandwidth(ProtocolControlMessage):
-
     def __init__(self, ack_window_size: int, limit_type: int):
         payload = BitStream()
         payload.append(BitArray(uint=ack_window_size, length=32))
         payload.append(BitArray(uint=limit_type, length=8))
         super().__init__(
             chunk_id=2,
             chunk_type=0,
@@ -116,11 +113,11 @@
         self.ack_window_size = ack_window_size
         self.limit_type = limit_type
 
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
         instance = cls(
-            ack_window_size=data.read('uint:32'),
-            limit_type=data.read('uint:8'),
+            ack_window_size=data.read("uint:32"),
+            limit_type=data.read("uint:8"),
         )
         return instance
```

### Comparing `pyrtmp-0.3.0/pyrtmp/messages/user_control.py` & `pyrtmp-0.3.1/pyrtmp/messages/user_control.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 import logging
 
-from bitstring import BitStream, BitArray
+from bitstring import BitArray, BitStream
 
 from pyrtmp.messages import Chunk
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class UserControlMessage(Chunk):
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
-        signature = data.read('uint:16')
+        signature = data.read("uint:16")
         if signature == 0:
             return StreamBegin.from_chunk(chunk)
         logger.warning(f"Unknown CommandMessage '{signature}', use default parser")
         instance = cls(**chunk.__dict__)
         instance.event_type = signature
         return instance
 
 
 class StreamBegin(UserControlMessage):
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
         instance = cls(**chunk.__dict__)
-        instance.event_type = data.read('uint:16')
-        instance.stream_id = data.read('uint:32')
+        instance.event_type = data.read("uint:16")
+        instance.stream_id = data.read("uint:32")
         return instance
 
     def __init__(self, stream_id: int) -> bytes:
         payload = BitStream()
         payload.append(BitArray(uint=0, length=16))
         payload.append(BitArray(uint=stream_id, length=32))
         super().__init__(
@@ -46,21 +44,20 @@
             payload=payload.bytes,
         )
         self.event_type = 0
         self.stream_id = stream_id
 
 
 class StreamEOF(UserControlMessage):
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
         instance = cls(**chunk.__dict__)
-        instance.event_type = data.read('uint:16')
-        instance.stream_id = data.read('uint:32')
+        instance.event_type = data.read("uint:16")
+        instance.stream_id = data.read("uint:32")
         return instance
 
     def __init__(self, stream_id: int) -> bytes:
         payload = BitStream()
         payload.append(BitArray(uint=1, length=16))
         payload.append(BitArray(uint=stream_id, length=32))
         super().__init__(
@@ -73,21 +70,20 @@
             payload=payload.bytes,
         )
         self.event_type = 1
         self.stream_id = stream_id
 
 
 class StreamDry(UserControlMessage):
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
         instance = cls(**chunk.__dict__)
-        instance.event_type = data.read('uint:16')
-        instance.stream_id = data.read('uint:32')
+        instance.event_type = data.read("uint:16")
+        instance.stream_id = data.read("uint:32")
         return instance
 
     def __init__(self, stream_id: int) -> bytes:
         payload = BitStream()
         payload.append(BitArray(uint=2, length=16))
         payload.append(BitArray(uint=stream_id, length=32))
         super().__init__(
@@ -100,22 +96,21 @@
             payload=payload.bytes,
         )
         self.event_type = 2
         self.stream_id = stream_id
 
 
 class SetBufferLength(UserControlMessage):
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
         instance = cls(**chunk.__dict__)
-        instance.event_type = data.read('uint:16')
-        instance.stream_id = data.read('uint:32')
-        instance.milliseconds = data.read('uint:32')
+        instance.event_type = data.read("uint:16")
+        instance.stream_id = data.read("uint:32")
+        instance.milliseconds = data.read("uint:32")
         return instance
 
     def __init__(self, stream_id: int, milliseconds: int) -> bytes:
         payload = BitStream()
         payload.append(BitArray(uint=3, length=16))
         payload.append(BitArray(uint=stream_id, length=32))
         payload.append(BitArray(uint=milliseconds, length=32))
@@ -130,21 +125,20 @@
         )
         self.event_type = 3
         self.stream_id = stream_id
         self.milliseconds = milliseconds
 
 
 class StreamIsRecorded(UserControlMessage):
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
         instance = cls(**chunk.__dict__)
-        instance.event_type = data.read('uint:16')
-        instance.stream_id = data.read('uint:32')
+        instance.event_type = data.read("uint:16")
+        instance.stream_id = data.read("uint:32")
         return instance
 
     def __init__(self, stream_id: int) -> bytes:
         payload = BitStream()
         payload.append(BitArray(uint=4, length=16))
         payload.append(BitArray(uint=stream_id, length=32))
         super().__init__(
@@ -157,21 +151,20 @@
             payload=payload.bytes,
         )
         self.event_type = 4
         self.stream_id = stream_id
 
 
 class PingRequest(UserControlMessage):
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
         instance = cls(**chunk.__dict__)
-        instance.event_type = data.read('uint:16')
-        instance.timestamp = data.read('uint:32')
+        instance.event_type = data.read("uint:16")
+        instance.timestamp = data.read("uint:32")
         return instance
 
     def __init__(self, timestamp: int) -> bytes:
         payload = BitStream()
         payload.append(BitArray(uint=6, length=16))
         payload.append(BitArray(uint=timestamp, length=32))
         super().__init__(
@@ -184,21 +177,20 @@
             payload=payload.bytes,
         )
         self.event_type = 6
         self.timestamp = timestamp
 
 
 class PingResponse(UserControlMessage):
-
     @classmethod
     def from_chunk(cls, chunk: Chunk):
         data = BitStream(chunk.payload)
         instance = cls(**chunk.__dict__)
-        instance.event_type = data.read('uint:16')
-        instance.timestamp = data.read('uint:32')
+        instance.event_type = data.read("uint:16")
+        instance.timestamp = data.read("uint:32")
         return instance
 
     def __init__(self, timestamp: int) -> bytes:
         payload = BitStream()
         payload.append(BitArray(uint=7, length=16))
         payload.append(BitArray(uint=timestamp, length=32))
         super().__init__(
```

### Comparing `pyrtmp-0.3.0/pyrtmp/rtmp.py` & `pyrtmp-0.3.1/pyrtmp/rtmp.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from __future__ import annotations
+
 import abc
 import asyncio
 import logging
 from asyncio import StreamReader, StreamWriter, events
+
 from pyrtmp import StreamClosedException
 from pyrtmp.messages import Chunk
 from pyrtmp.messages.audio import AudioMessage
-from pyrtmp.messages.command import NCConnect, NCCreateStream, NSPublish, NSCloseStream, NSDeleteStream
+from pyrtmp.messages.command import NCConnect, NCCreateStream, NSCloseStream, NSDeleteStream, NSPublish
 from pyrtmp.messages.data import MetaDataMessage
 from pyrtmp.messages.factory import MessageFactory
-from pyrtmp.messages.protocol_control import WindowAcknowledgementSize, SetChunkSize, SetPeerBandwidth
+from pyrtmp.messages.protocol_control import SetChunkSize, SetPeerBandwidth, WindowAcknowledgementSize
 from pyrtmp.messages.user_control import StreamBegin
 from pyrtmp.messages.video import VideoMessage
 from pyrtmp.session_manager import SessionManager
 
 logging.basicConfig(level=logging.DEBUG)
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 
 class BaseRTMPController(abc.ABC):
-
     async def client_callback(self, reader: StreamReader, writer: StreamWriter) -> None:
         raise NotImplementedError()
 
     async def on_handshake(self, session: SessionManager) -> None:
         raise NotImplementedError()
 
     async def on_nc_connect(self, session: SessionManager, message: NCConnect) -> None:
@@ -64,19 +65,18 @@
         raise NotImplementedError()
 
     async def cleanup(self, session: SessionManager) -> None:
         raise NotImplementedError()
 
 
 class SimpleRTMPController(BaseRTMPController):
-
     async def client_callback(self, reader: StreamReader, writer: StreamWriter) -> None:
         # create session per client
         session = SessionManager(reader=reader, writer=writer)
-        logger.debug(f'Client connected {session.peername}')
+        logger.debug(f"Client connected {session.peername}")
 
         try:
             # do handshake
             await self.on_handshake(session)
             logger.debug(f"Handshake! {session.peername}")
 
             # read chunks
@@ -103,124 +103,124 @@
                     await self.on_ns_close_stream(session, message)
                 elif isinstance(message, NSDeleteStream):
                     await self.on_ns_delete_stream(session, message)
                 else:
                     await self.on_unknown_message(session, message)
 
         except StreamClosedException as ex:
-            logger.debug(f'Client disconnected {session.peername}')
+            logger.debug(f"Client disconnected {session.peername}")
             await self.on_stream_closed(session, ex)
         except Exception as ex:
             logger.exception(ex)
         finally:
             await self.cleanup(session)
 
-    async def on_handshake(self, session) -> None:
+        writer.close()
+
+    async def on_handshake(self, session: SessionManager) -> None:
         await session.handshake()
 
-    async def on_nc_connect(self, session, message) -> None:
+    async def on_nc_connect(self, session: SessionManager, message: NCConnect) -> None:
         session.write_chunk_to_stream(WindowAcknowledgementSize(ack_window_size=5000000))
         session.write_chunk_to_stream(SetPeerBandwidth(ack_window_size=5000000, limit_type=2))
         session.write_chunk_to_stream(StreamBegin(stream_id=0))
         session.write_chunk_to_stream(SetChunkSize(chunk_size=8192))
         session.writer_chunk_size = 8192
         session.write_chunk_to_stream(message.create_response())
         await session.drain()
 
-    async def on_window_acknowledgement_size(self, session, message) -> None:
+    async def on_window_acknowledgement_size(self, session: SessionManager, message: WindowAcknowledgementSize) -> None:
         pass
 
-    async def on_nc_create_stream(self, session, message) -> None:
+    async def on_nc_create_stream(self, session: SessionManager, message: NCCreateStream) -> None:
         session.write_chunk_to_stream(message.create_response())
         await session.drain()
 
-    async def on_ns_publish(self, session, message) -> None:
+    async def on_ns_publish(self, session: SessionManager, message: NSPublish) -> None:
         session.write_chunk_to_stream(StreamBegin(stream_id=1))
         session.write_chunk_to_stream(message.create_response())
         await session.drain()
 
-    async def on_metadata(self, session, message) -> None:
+    async def on_metadata(self, session: SessionManager, message: MetaDataMessage) -> None:
         pass
 
-    async def on_set_chunk_size(self, session, message) -> None:
+    async def on_set_chunk_size(self, session: SessionManager, message: SetChunkSize) -> None:
         session.reader_chunk_size = message.chunk_size
 
-    async def on_video_message(self, session, message) -> None:
+    async def on_video_message(self, session: SessionManager, message: VideoMessage) -> None:
         pass
 
-    async def on_audio_message(self, session, message) -> None:
+    async def on_audio_message(self, session: SessionManager, message: AudioMessage) -> None:
         pass
 
-    async def on_ns_close_stream(self, session, message) -> None:
+    async def on_ns_close_stream(self, session: SessionManager, message: NSCloseStream) -> None:
         pass
 
-    async def on_ns_delete_stream(self, session, message) -> None:
+    async def on_ns_delete_stream(self, session: SessionManager, message: NSDeleteStream) -> None:
         pass
 
-    async def on_unknown_message(self, session, message) -> None:
+    async def on_unknown_message(self, session: SessionManager, message: Chunk) -> None:
         logger.warning(f"Unknown message {str(message)}")
 
     async def on_stream_closed(self, session: SessionManager, exception: StreamClosedException) -> None:
         pass
 
     async def cleanup(self, session: SessionManager) -> None:
-        logger.debug(f'Clean up {session.peername}')
+        logger.debug(f"Clean up {session.peername}")
 
 
 class RTMPProtocol(asyncio.StreamReaderProtocol):
-
     def __init__(self, controller: BaseRTMPController) -> None:
         self.callback = controller.client_callback
         self.loop = events.get_event_loop()
         super().__init__(
             StreamReader(loop=self.loop),
             self.callback,
             loop=self.loop,
         )
 
 
 class SimpleRTMPServer:
-
-    def __init__(self):
+    def __init__(self) -> None:
         self.server = None
         self.on_start = None
         self.on_stop = None
 
-    def _signal_on_start(self):
+    def _signal_on_start(self) -> None:
         if self.on_start:
             self.on_start()
 
-    def _signal_on_stop(self):
+    def _signal_on_stop(self) -> None:
         if self.on_stop:
             self.on_stop()
 
-    async def create(self, host: str, port: int):
+    async def create(self, host: str, port: int) -> None:
         loop = asyncio.get_event_loop()
         self.server = await loop.create_server(
             lambda: RTMPProtocol(controller=SimpleRTMPController()),
             host=host,
             port=port,
         )
 
-    async def start(self):
+    async def start(self) -> None:
         addr = self.server.sockets[0].getsockname()
         await self.server.start_serving()
         self._signal_on_start()
-        logger.info(f'Serving on {addr}')
+        logger.info(f"Serving on {addr}")
 
-    async def wait_closed(self):
+    async def wait_closed(self) -> None:
         await self.server.wait_closed()
 
-    async def stop(self):
+    async def stop(self) -> None:
         self.server.close()
         self._signal_on_stop()
 
 
-async def main():
+async def main() -> None:
     server = SimpleRTMPServer()
-    await server.create(host='0.0.0.0', port=1935)
+    await server.create(host="0.0.0.0", port=1935)
     await server.start()
     await server.wait_closed()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `pyrtmp-0.3.0/pyrtmp/session_manager.py` & `pyrtmp-0.3.1/pyrtmp/session_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from __future__ import annotations
-from typing import Generator
+
+from asyncio import StreamReader, StreamWriter
+from collections.abc import Generator
+
 from bitstring import BitStream
+
 from pyrtmp import BitStreamReader, random_byte_array
 from pyrtmp.messages import Chunk, RawChunk
 from pyrtmp.messages.handshake import C0, C1, C2
 
 
 class SessionManager:
-
     def __init__(
-            self,
-            reader,
-            writer,
-            reader_chunk_size=128,
-            writer_chunk_size=128) -> None:
+        self, reader: StreamReader, writer: StreamWriter, reader_chunk_size: int = 128, writer_chunk_size: int = 128
+    ) -> None:
         self.reader = reader
         self.writer = writer
         self.reader_chunk_size = reader_chunk_size
         self.writer_chunk_size = writer_chunk_size
         self.latest_chunks = {}
         self.fifo_reader = BitStreamReader(self.reader)
         self.previous_chunk_for_writing: RawChunk | None = None
         self.state = {}
         super().__init__()
 
     @property
-    def total_read_bytes(self):
+    def total_read_bytes(self) -> int:
         return self.fifo_reader.total_bytes
 
     @property
-    def peername(self):
-        a, b = self.writer.get_extra_info('peername')
+    def peername(self) -> str:
+        a, b = self.writer.get_extra_info("peername")
         return f"{a}:{b}"
 
-    def set_latest_chunk(self, chunk: RawChunk):
+    def set_latest_chunk(self, chunk: RawChunk) -> None:
         self.latest_chunks[str(chunk.chunk_id)] = chunk
         self.latest_chunks["latest"] = chunk
 
     def get_previous_chunk(self, chunk_id: int) -> RawChunk:
         return self.latest_chunks[str(chunk_id)]
 
-    async def handshake(self):
+    async def handshake(self) -> None:
         # read c0c1
         c0 = await C0.from_stream(self.fifo_reader)
         c1 = await C1.from_stream(self.fifo_reader)
         s0 = C0(protocol_version=c0.protocol_version)
         s1 = C1(time=0, zero=0, random=random_byte_array(1528))
         s2 = C2(time1=c1.time, time2=c1.time, random=c1.random)
         s0s1s2 = BitStream()
@@ -99,49 +99,49 @@
                         payload=payload.bytes,
                     )
 
     async def read_raw_chunk(self) -> RawChunk:
         stream = self.fifo_reader
         chunk_size = self.reader_chunk_size
 
-        fmt = await stream.read('uint:2')
-        cs_id = await stream.read('uint:6')
+        fmt = await stream.read("uint:2")
+        cs_id = await stream.read("uint:6")
         if cs_id == 0:
-            cs_id = await stream.read('uint:8') + 64
+            cs_id = await stream.read("uint:8") + 64
         elif cs_id == 1:
-            cs_id = await stream.read('uint:16') + 64
+            cs_id = await stream.read("uint:16") + 64
         elif cs_id == 2:
             pass
 
         assert fmt is not None and cs_id is not None
 
         if fmt == 0:
             # 11 bytes
-            timestamp = await stream.read('uint:24')
+            timestamp = await stream.read("uint:24")
             if timestamp >= 0xFFFFFF:
                 timestamp = 0xFFFFFF
-            msg_length = await stream.read('uint:24')
-            msg_type_id = await stream.read('uint:8')
-            msg_stream_id = await stream.read('uintle:32')
+            msg_length = await stream.read("uint:24")
+            msg_type_id = await stream.read("uint:8")
+            msg_stream_id = await stream.read("uintle:32")
             sequence = 0
         elif fmt == 1:
             # 7 bytes
             previous_chunk = self.get_previous_chunk(cs_id)
             assert previous_chunk is not None
-            delta = await stream.read('uint:24')
-            msg_length = await stream.read('uint:24')
-            msg_type_id = await stream.read('uint:8')
+            delta = await stream.read("uint:24")
+            msg_length = await stream.read("uint:24")
+            msg_type_id = await stream.read("uint:8")
             msg_stream_id = previous_chunk.msg_stream_id
             timestamp = previous_chunk.timestamp + delta
             sequence = 0 if previous_chunk.is_eof else previous_chunk.raw_chunk_number + 1
         elif fmt == 2:
             # 3 bytes
             previous_chunk = self.get_previous_chunk(cs_id)
             assert previous_chunk is not None
-            delta = await stream.read('uint:24')
+            delta = await stream.read("uint:24")
             timestamp = previous_chunk.timestamp + delta
             msg_length = previous_chunk.msg_length
             msg_type_id = previous_chunk.msg_type_id
             msg_stream_id = previous_chunk.msg_stream_id
             sequence = 0 if previous_chunk.is_eof else previous_chunk.raw_chunk_number + 1
         elif fmt == 3:
             # 0 bytes
@@ -153,21 +153,21 @@
             msg_type_id = previous_chunk.msg_type_id
             msg_stream_id = previous_chunk.msg_stream_id
             sequence = 0 if previous_chunk.is_eof else previous_chunk.raw_chunk_number + 1
         else:
             raise NotImplementedError
 
         if timestamp == 0xFFFFFF:
-            timestamp = await stream.read('uint:32')
+            timestamp = await stream.read("uint:32")
 
         # determine payload size
         total_read = chunk_size * sequence
         bytes_length = min(chunk_size, msg_length - total_read)
         is_eof = (msg_length - total_read - bytes_length) == 0
-        payload = await stream.read(f'bytes:{bytes_length}')
+        payload = await stream.read(f"bytes:{bytes_length}")
         instance = RawChunk(
             chunk_type=fmt,
             chunk_id=cs_id,
             timestamp=timestamp,
             msg_length=msg_length,
             msg_type_id=msg_type_id,
             msg_stream_id=msg_stream_id,
@@ -178,16 +178,16 @@
 
         # update latest chunk
         self.set_latest_chunk(instance)
 
         # return
         return instance
 
-    def write_chunk_to_stream(self, chunk: Chunk):
+    def write_chunk_to_stream(self, chunk: Chunk) -> None:
         chunks = chunk.to_raw_chunks(self.writer_chunk_size, self.previous_chunk_for_writing)
         for chunk in chunks:
             self.writer.write(chunk.to_bytes())
             self.previous_chunk_for_writing = chunk
 
-    async def drain(self):
+    async def drain(self) -> None:
         self.previous_chunk_for_writing = None
         await self.writer.drain()
```

### Comparing `pyrtmp-0.3.0/pyrtmp.egg-info/PKG-INFO` & `pyrtmp-0.3.1/pyrtmp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtmp
-Version: 0.3.0
+Version: 0.3.1
 Summary: PyRTMP: Pure Python RTMP server
 Home-page: https://github.com/Eittipat/pyrtmp.git
 Download-URL: https://github.com/Eittipat/pyrtmp/releases/tag/v0.3.0
 Author: Eittipat.K
 Author-email: iammop@gmail.com
 License: MIT
 Keywords: RTMP,RTMPT,asyncio
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: bitstring>=4
+Requires-Dist: bitstring<4.2,>=4.1
 
 # PyRTMP: Pure Python RTMP server
 ![coverage](https://github.com/Eittipat/pyrtmp/blob/master/coverage.svg)
 ## Features
 
 - ✅ Pure Python
 - ✅ Easy to customize
```

### Comparing `pyrtmp-0.3.0/pyrtmp.egg-info/SOURCES.txt` & `pyrtmp-0.3.1/pyrtmp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrtmp-0.3.0/tests/__init__.py` & `pyrtmp-0.3.1/tests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,27 +10,28 @@
         os.remove(path)
 
 
 async def invoke_command(command: str):
     proc = None
     try:
         proc = await asyncio.subprocess.create_subprocess_shell(
-            command, stdout=asyncio.subprocess.PIPE,
+            command,
+            stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
         )
         stdout, stderr = await proc.communicate()
         if proc.returncode > 0:
             logging.exception(stderr.decode())
             raise Exception("Non-zero returned")
 
         return stdout, stderr
     finally:
         if proc and proc.returncode is None:
             process = psutil.Process(proc.pid)
-            to_be_kill = [p for p in process.children(recursive=True)]
+            to_be_kill = list(process.children(recursive=True))
             to_be_kill.append(process)
             exception = None
             for p in to_be_kill:
                 try:
                     p.kill()
                 except Exception as ex:
                     exception = ex
```

### Comparing `pyrtmp-0.3.0/tests/test_demo_ffmpeg.py` & `pyrtmp-0.3.1/tests/test_demo_ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import unittest
 
 from example.demo_ffmpeg import SimpleServer
 from tests import invoke_command, remove_if_exist
 
 
 class TestFFMPEG(unittest.IsolatedAsyncioTestCase):
-
     async def asyncSetUp(self):
         _loop = asyncio.get_event_loop()
         _loop._close_loop = _loop.close
         _loop.close = lambda: ()
         asyncio.set_event_loop(_loop)
 
     async def test_single_ffmpeg(self):
@@ -20,15 +19,15 @@
             # given
             stream_name = "test_ffmpeg"
             command = "ffmpeg -i SampleVideo_1280x720_5mb.flv -c:v copy -c:a copy -f flv {}"
             target = os.path.join(tempdir, stream_name + ".flv")
             remove_if_exist(target)
 
             server = SimpleServer(tempdir)
-            await server.create(host='127.0.0.1', port=1935)
+            await server.create(host="127.0.0.1", port=1935)
             await server.start()
 
             task1 = invoke_command(command.format(f"rtmp://127.0.0.1:1935/test/{stream_name}"))
 
             # when
             await task1
             await asyncio.sleep(3)
@@ -41,15 +40,15 @@
             stdout, stderr = await invoke_command(f"ffprobe -i {target} -show_format | grep duration")
             self.assertEqual(stdout.decode().startswith("duration=26"), True)
 
     async def test_multiple_ffmpeg(self):
         with tempfile.TemporaryDirectory() as tempdir:
             # given
             server = SimpleServer(tempdir)
-            await server.create(host='127.0.0.1', port=1935)
+            await server.create(host="127.0.0.1", port=1935)
             await server.start()
 
             tasks = []
             for i in range(3):
                 stream_name = f"test_ffmpeg_{i}"
                 command = "ffmpeg -i SampleVideo_1280x720_5mb.flv -c:v copy -c:a copy -f flv {}"
                 target = os.path.join(tempdir, stream_name + ".flv")
```

### Comparing `pyrtmp-0.3.0/tests/test_demo_flvdump.py` & `pyrtmp-0.3.1/tests/test_demo_flvdump.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import unittest
 
 from example.demo_flvdump import SimpleServer
 from tests import invoke_command, remove_if_exist
 
 
 class TestFLVDump(unittest.IsolatedAsyncioTestCase):
-
     async def asyncSetUp(self):
         _loop = asyncio.get_event_loop()
         _loop._close_loop = _loop.close
         _loop.close = lambda: ()
         asyncio.set_event_loop(_loop)
 
     async def test_single_flvdump(self):
@@ -20,15 +19,15 @@
             # given
             command = "ffmpeg -i SampleVideo_1280x720_5mb.flv -c:v copy -c:a copy -f flv {}"
             stream_name = "test_flvdump"
             target = os.path.join(tempdir, stream_name + ".flv")
             remove_if_exist(target)
 
             server = SimpleServer(tempdir)
-            await server.create(host='127.0.0.1', port=1935)
+            await server.create(host="127.0.0.1", port=1935)
             await server.start()
 
             task1 = invoke_command(command.format(f"rtmp://127.0.0.1:1935/test/{stream_name}"))
 
             # when
             await task1
             await asyncio.sleep(3)
@@ -41,15 +40,15 @@
             stdout, stderr = await invoke_command(f"ffprobe -i {target} -show_format | grep duration")
             self.assertEqual(stdout.decode().startswith("duration=26"), True)
 
     async def test_multiple_flvdump(self):
         with tempfile.TemporaryDirectory() as tempdir:
             # given
             server = SimpleServer(tempdir)
-            await server.create(host='127.0.0.1', port=1935)
+            await server.create(host="127.0.0.1", port=1935)
             await server.start()
 
             tasks = []
             for i in range(3):
                 command = "ffmpeg -i SampleVideo_1280x720_5mb.flv -c:v copy -c:a copy -f flv {}"
                 stream_name = f"test_flvdump_{i}"
                 target = os.path.join(tempdir, stream_name + ".flv")
```

### Comparing `pyrtmp-0.3.0/tests/test_demo_rtmpt.py` & `pyrtmp-0.3.1/tests/test_demo_rtmpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import unittest
 
 from example.demo_rtmpt import serve_rtmpt
 from tests import invoke_command, remove_if_exist
 
 
 class TestRTMP(unittest.IsolatedAsyncioTestCase):
-
     async def test_single_rtmpt(self):
         with tempfile.TemporaryDirectory() as tempdir:
             # given
             filename = "SampleVideo_1280x720_5mb.flv"
             stream_path = "rtmpt://127.0.0.1:5000/test/test_rtmpt"
             target = os.path.join(tempdir, "test_rtmpt" + ".flv")
             remove_if_exist(target)
```

### Comparing `pyrtmp-0.3.0/tests/test_pyrtmp.py` & `pyrtmp-0.3.1/tests/test_pyrtmp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
 import unittest
-
 from asyncio import StreamReader
+
 from bitstring import BitArray, BitStream
+
 from pyrtmp import BitStreamReader
 from pyrtmp.amf.serializers import AMF0Serializer
 
 
 class MockStreamReader(StreamReader):
-
     def __init__(self):
         super().__init__()
         self.mock_data = None
 
     async def read(self, n=...):
         while self.mock_data is None:
             await asyncio.sleep(0.1)
@@ -21,15 +21,14 @@
         return data
 
     def set_mock_data(self, data: bytes):
         self.mock_data = data
 
 
 class TestBitStreamReader(unittest.IsolatedAsyncioTestCase):
-
     async def test_enough_data(self):
         # given
         mock_data = BitArray("0b1111111100000000100010001000000011011011").bytes
         mock_reader = MockStreamReader()
         mock_reader.set_mock_data(mock_data)
         stream = BitStreamReader(reader=mock_reader)
 
@@ -43,23 +42,23 @@
 
     async def test_not_enough_data(self):
         # given
         mock_reader = MockStreamReader()
         stream = BitStreamReader(reader=mock_reader)
 
         async def feed_data():
-            mock_reader.set_mock_data(b'\xff')
+            mock_reader.set_mock_data(b"\xff")
             await asyncio.sleep(0.5)
-            mock_reader.set_mock_data(b'\x00')
+            mock_reader.set_mock_data(b"\x00")
             await asyncio.sleep(0.5)
-            mock_reader.set_mock_data(b'\x88')
+            mock_reader.set_mock_data(b"\x88")
             await asyncio.sleep(0.5)
-            mock_reader.set_mock_data(b'\x80')
+            mock_reader.set_mock_data(b"\x80")
             await asyncio.sleep(0.5)
-            mock_reader.set_mock_data(b'\xdb')
+            mock_reader.set_mock_data(b"\xdb")
             print("feed_data done")
 
         task = asyncio.create_task(feed_data())
 
         # when
         uint8 = await stream.read("uint:8")
         int32 = await stream.read("int:32")
@@ -68,95 +67,104 @@
 
         # then
         self.assertEqual(uint8, 255)
         self.assertEqual(int32, 8945883)
 
 
 class AMF0SerializerTestCase(unittest.TestCase):
-
     def test_write_boolean_object(self):
         # given
         data = BitStream()
 
         # when
         AMF0Serializer.write_boolean_object(data, True)
 
         # then
         self.assertEqual(data.pos, 0)
         self.assertEqual(data.length, 8 + 8)
-        self.assertEqual(data.bytes, b'\x01\x01')
+        self.assertEqual(data.bytes, b"\x01\x01")
 
     def test_write_string_object(self):
         # given
         data = BitStream()
 
         # when
         AMF0Serializer.write_string_object(data, "hello world")
 
         # then
         self.assertEqual(data.pos, 0)
         self.assertEqual(data.length, 8 + 16 + len("hello world") * 8)
-        self.assertEqual(data.bytes, b'\x02\x00\x0bhello world')
+        self.assertEqual(data.bytes, b"\x02\x00\x0bhello world")
 
     def test_write_number_object(self):
         # given
         data = BitStream()
 
         # when
         AMF0Serializer.write_number_object(data, 3.1415)
 
         # then
         self.assertEqual(data.pos, 0)
         self.assertEqual(data.length, 72)
-        self.assertEqual(data.bytes, b'\x00@\t!\xca\xc0\x83\x12o')
+        self.assertEqual(data.bytes, b"\x00@\t!\xca\xc0\x83\x12o")
 
     def test_write_null_object(self):
         # given
         data = BitStream()
 
         # when
         AMF0Serializer.write_null_object(data)
 
         # then
         self.assertEqual(data.pos, 0)
         self.assertEqual(data.length, 8)
-        self.assertEqual(data.bytes, b'\x05')
+        self.assertEqual(data.bytes, b"\x05")
 
     def test_write_object_object(self):
         # given
         data = BitStream()
 
         # when
-        AMF0Serializer.write_object_object(data, {
-            "key1": "value1",
-            "key2": 2,
-            "key3": True,
-        })
+        AMF0Serializer.write_object_object(
+            data,
+            {
+                "key1": "value1",
+                "key2": 2,
+                "key3": True,
+            },
+        )
 
         # then
         self.assertEqual(data.pos, 0)
         self.assertEqual(data.length, 336)
-        self.assertEqual(data.bytes,
-                         b'\x03\x00\x04' +
-                         b'key1\x02\x00\x06value1\x00\x04' +
-                         b'key2\x00@\x00\x00\x00\x00\x00\x00\x00\x00\x04' +
-                         b'key3\x01\x01\x00\x00\t')
+        self.assertEqual(
+            data.bytes,
+            b"\x03\x00\x04"
+            + b"key1\x02\x00\x06value1\x00\x04"
+            + b"key2\x00@\x00\x00\x00\x00\x00\x00\x00\x00\x04"
+            + b"key3\x01\x01\x00\x00\t",
+        )
 
     def test_write_array_object(self):
         # given
         data = BitStream()
 
         # when
-        AMF0Serializer.write_array_object(data, [
-            {"key1": "value1"},
-            {"key2": 2},
-            {"key3": True},
-        ])
+        AMF0Serializer.write_array_object(
+            data,
+            [
+                {"key1": "value1"},
+                {"key2": 2},
+                {"key3": True},
+            ],
+        )
 
         # then
         self.assertEqual(data.pos, 0)
         self.assertEqual(data.length, 368)
-        self.assertEqual(data.bytes,
-                         b'\x08\x00\x00\x00\x03\x00\x04'
-                         + b'key1\x02\x00\x06value1\x00\x04'
-                         + b'key2\x00@\x00\x00\x00\x00\x00\x00\x00\x00\x04'
-                         + b'key3\x01\x01\x00\x00\t')
+        self.assertEqual(
+            data.bytes,
+            b"\x08\x00\x00\x00\x03\x00\x04"
+            + b"key1\x02\x00\x06value1\x00\x04"
+            + b"key2\x00@\x00\x00\x00\x00\x00\x00\x00\x00\x04"
+            + b"key3\x01\x01\x00\x00\t",
+        )
```

