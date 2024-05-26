# Comparing `tmp/pydatastreams-1.1.0.tar.gz` & `tmp/pydatastreams-1.2.0.tar.gz`

## Comparing `pydatastreams-1.1.0.tar` & `pydatastreams-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/datastream/__about__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/datastream/__init__.py
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/datastream/base.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/datastream/deserializing.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/datastream/serializing.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/README.md
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 pydatastreams-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/__about__.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/__init__.py
+-rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/base.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/deserializing.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/serializing.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/datastream/twoway.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/README.md
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 pydatastreams-1.2.0/PKG-INFO
```

### Comparing `pydatastreams-1.1.0/datastream/base.py` & `pydatastreams-1.2.0/datastream/base.py`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.1.0/datastream/deserializing.py` & `pydatastreams-1.2.0/datastream/deserializing.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 class DeserializingStream(BaseStream):
     def __init__(
         self, buffer: bytes | typing.IO[bytes], byteorder: int = ByteOrder.NATIVE_ENDIAN
     ):
         if not isinstance(buffer, io.BytesIO):
             if isinstance(buffer, io.IOBase):
-                buffer = io.BytesIO(buffer.getvalue())
+                buffer = io.BytesIO(buffer.getvalue()) # type: ignore
             else:
-                buffer = io.BytesIO(buffer)
+                buffer = io.BytesIO(buffer) # type: ignore
 
         super().__init__(buffer, byteorder)
 
     def read_format(self, fmt: str) -> typing.Any:
         return struct.unpack(self._byteorder + fmt, self.read(struct.calcsize(fmt)))[0]
 
     def read_int64(self) -> int:
@@ -61,77 +61,83 @@
         read.
         
         Returns:
             int: The decoded unsigned integer.
         """
         return self.read_uleb128_safe(-1)
 
-    def read_uleb128_safe(self, max_bytes = 16) -> int:
+    def read_uleb128_safe(self, max_bytes: int = 16) -> int:
         """
         Reads an unsigned LEB128 (Little-Endian Base 128) encoded integer from the data
         stream.
 
         Args:
             max_bytes (int, optional): The maximum number of bytes to read before
                 stopping. Defaults to 16.
 
         Returns:
             int: The decoded unsigned integer.
         """
+        if max_bytes == 0:
+            return 0
+        
         decoded = self.read_uint8()
 
         if decoded < 0x7F:
             return decoded
 
         decoded &= 0x7F
         shift_mod = 1
 
         while max_bytes != 0 and (current_byte := self.read_uint8()) & 0x80:
             decoded += (current_byte & 0x7F) << shift_mod * 7
             shift_mod += 1
             max_bytes -= 1
 
-        return decoded + (current_byte << shift_mod * 7)
+        return decoded + (current_byte << shift_mod * 7) # type: ignore
     
     def read_sleb128(self) -> int:
         """
         Reads a signed LEB128 (Little-Endian Base 128) encoded integer from the data
         stream. Keep in mind that this method does not perform any bounds checking, so
         it is possible to read an arbitrarily large integer if a malformed sequence is
         read.
 
         Returns:
             int: The decoded signed integer.
         """
         return self.read_sleb128_safe(-1)
     
-    def read_sleb128_safe(self, stop_after = 5) -> int:
+    def read_sleb128_safe(self, stop_after: int = 5) -> int:
         """
         Reads a signed LEB128 (Little-Endian Base 128) encoded integer from the data
         stream.
 
         Args:
             stop_after (int, optional): The maximum number of bytes to read before
                 stopping. Defaults to 5.
 
         Returns:
             int: The decoded signed integer.
         """
+        if stop_after == 0:
+            return 0
+
         decoded = self.read_uint8()
         shift_mod = 1
 
         if decoded < 0x7F:
             return decoded
         
         decoded &= 0x7F
 
         while stop_after != 0 and (current_byte := self.read_uint8()) & 0x80:
             decoded += (current_byte & 0x7F) << shift_mod * 7
             shift_mod += 1
             stop_after -= 1
         
-        decoded += (current_byte << shift_mod * 7)
+        decoded += (current_byte << shift_mod * 7) # type: ignore
 
-        if current_byte & 0x40:
+        if current_byte & 0x40: # type: ignore
             decoded |= -(1 << (shift_mod * 7) + 7)
 
         return decoded
```

### Comparing `pydatastreams-1.1.0/datastream/serializing.py` & `pydatastreams-1.2.0/datastream/serializing.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         Returns the bytes written to the stream.
 
         Returns:
             bytes: The bytes written to the stream.
         """
         return self._backing_stream.getvalue()
 
-    def __bytes__(self) -> bytes:
+    def __bytes__(self) -> bytes: # type: ignore
         return self.bytes()
 
     def write_format(self, fmt: str, value: typing.Any):
         self.write(struct.pack(self._byteorder + fmt, value))
 
     def write_int64(self, value: int):
         self.write_format("q", value)
```

### Comparing `pydatastreams-1.1.0/.gitignore` & `pydatastreams-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.1.0/LICENSE.txt` & `pydatastreams-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.1.0/README.md` & `pydatastreams-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 serialized = stream.bytes()
 
 # this also works
 serialized = bytes(stream)
 ```
 
+Note: This library also contains a stream for both serializing and deserializing data. This stream is called [`TwoWayStream`](datastream/twoway.py#L9).
+
 The stream classes support serializing/deserializing the standard data types:
 | Data Type | Description | [Serializer](datastream/serializing.py#L8) | [Deserializer](datastream/deserializing.py#L8)
 | --- | --- | ---| --- |
 | `int8_t` | Signed 8-bit number | [`write_int8(value: int)`](datastream/serializing.py#L52) | [`read_int8() -> int`](datastream/deserializing.py#L41) |
 | `uint8_t` | Unsigned 8-bit number | [`write_uint8(value: int)`](datastream/serializing.py#L55) | [`read_uint8() -> int`](datastream/deserializing.py#L44) |
 | `int16_t` | Signed 16-bit number | [`write_int16(value: int)`](datastream/serializing.py#L46) | [`read_int16() -> int`](datastream/deserializing.py#L35) |
 | `uint16_t` | Unsigned 16-bit number | [`write_uint16(value: int)`](datastream/serializing.py#L49) | [`read_uint16() -> int`](datastream/deserializing.py#L38) |
```

### Comparing `pydatastreams-1.1.0/pyproject.toml` & `pydatastreams-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydatastreams-1.1.0/PKG-INFO` & `pydatastreams-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydatastreams
-Version: 1.1.0
+Version: 1.2.0
 Summary: A simple and easy to use library for reading and writing data streams.
 Project-URL: Homepage, https://github.com/yntha/datastream
 Project-URL: Repository, https://github.com/yntha/datastream.git
 Project-URL: Issues, https://github.com/yntha/datastream/issues
 Author-email: yntha <bguznvjk@gmail.com>
 License-File: LICENSE.txt
 Keywords: binary,data,file,io,stream
@@ -45,14 +45,16 @@
 
 serialized = stream.bytes()
 
 # this also works
 serialized = bytes(stream)
 ```
 
+Note: This library also contains a stream for both serializing and deserializing data. This stream is called [`TwoWayStream`](datastream/twoway.py#L9).
+
 The stream classes support serializing/deserializing the standard data types:
 | Data Type | Description | [Serializer](datastream/serializing.py#L8) | [Deserializer](datastream/deserializing.py#L8)
 | --- | --- | ---| --- |
 | `int8_t` | Signed 8-bit number | [`write_int8(value: int)`](datastream/serializing.py#L52) | [`read_int8() -> int`](datastream/deserializing.py#L41) |
 | `uint8_t` | Unsigned 8-bit number | [`write_uint8(value: int)`](datastream/serializing.py#L55) | [`read_uint8() -> int`](datastream/deserializing.py#L44) |
 | `int16_t` | Signed 16-bit number | [`write_int16(value: int)`](datastream/serializing.py#L46) | [`read_int16() -> int`](datastream/deserializing.py#L35) |
 | `uint16_t` | Unsigned 16-bit number | [`write_uint16(value: int)`](datastream/serializing.py#L49) | [`read_uint16() -> int`](datastream/deserializing.py#L38) |
```

