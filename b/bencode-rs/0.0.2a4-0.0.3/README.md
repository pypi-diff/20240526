# Comparing `tmp/bencode_rs-0.0.2a4.tar.gz` & `tmp/bencode_rs-0.0.3.tar.gz`

## Comparing `bencode_rs-0.0.2a4.tar` & `bencode_rs-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a4/Cargo.toml
--rw-r--r--   0     1001      127      120 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.coveragerc
--rw-r--r--   0     1001      127       13 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.gitattributes
--rw-r--r--   0     1001      127      124 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.github/renovate.json
--rw-r--r--   0     1001      127     3084 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.github/workflows/_build_wheels.yaml
--rw-r--r--   0     1001      127     1732 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.github/workflows/ci.yaml
--rw-r--r--   0     1001      127      450 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.github/workflows/release.yaml
--rw-r--r--   0     1001      127     4828 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.gitignore
--rw-r--r--   0     1001      127     1085 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/LICENSE
--rw-r--r--   0     1001      127      184 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/bencode_rs/__init__.py
--rw-r--r--   0     1001      127      188 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/bencode_rs/__init__.pyi
--rw-r--r--   0     1001      127      831 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/leak.py
--rw-r--r--   0     1001      127      300 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/readme.md
--rw-r--r--   0     1001      127      123 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/requirements.txt
--rw-r--r--   0     1001      127      301 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/rustfmt.toml
--rw-r--r--   0     1001      127     7998 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/src/decode.rs
--rw-r--r--   0     1001      127     5612 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/src/encode.rs
--rw-r--r--   0     1001      127      557 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/src/lib.rs
--rw-r--r--   0     1001      127     5713 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/tests/fixtures/56507.torrent.bin
--rw-r--r--   0     1001      127   376318 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin
--rw-r--r--   0     1001      127     4397 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/tests/test_1_encode.py
--rw-r--r--   0     1001      127     3498 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/tests/test_2_decode.py
--rw-r--r--   0     1001      127     8499 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/Cargo.lock
--rw-r--r--   0     1001      127      648 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/pyproject.toml
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a4/PKG-INFO
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 bencode_rs-0.0.3/Cargo.toml
+-rw-r--r--   0     1001      127      120 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/.coveragerc
+-rw-r--r--   0     1001      127       13 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/.gitattributes
+-rw-r--r--   0     1001      127      124 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/.github/renovate.json
+-rw-r--r--   0     1001      127     3084 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/.github/workflows/_build_wheels.yaml
+-rw-r--r--   0     1001      127     1732 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0     1001      127      450 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0     1001      127     4828 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/.gitignore
+-rw-r--r--   0     1001      127     1085 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/LICENSE
+-rw-r--r--   0     1001      127      184 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/bencode_rs/__init__.py
+-rw-r--r--   0     1001      127      188 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/bencode_rs/__init__.pyi
+-rw-r--r--   0     1001      127      831 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/leak.py
+-rw-r--r--   0     1001      127      300 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/readme.md
+-rw-r--r--   0     1001      127      123 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/requirements.txt
+-rw-r--r--   0     1001      127      301 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/rustfmt.toml
+-rw-r--r--   0     1001      127     8392 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/src/decode.rs
+-rw-r--r--   0     1001      127     6004 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/src/encode.rs
+-rw-r--r--   0     1001      127      578 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/src/lib.rs
+-rw-r--r--   0     1001      127     5713 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/tests/fixtures/56507.torrent.bin
+-rw-r--r--   0     1001      127   376318 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin
+-rw-r--r--   0     1001      127     4397 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/tests/test_1_encode.py
+-rw-r--r--   0     1001      127     3498 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/tests/test_2_decode.py
+-rw-r--r--   0     1001      127     8704 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/Cargo.lock
+-rw-r--r--   0     1001      127      712 2024-05-26 16:01:01.000000 bencode_rs-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      830 1970-01-01 00:00:00.000000 bencode_rs-0.0.3/PKG-INFO
```

### Comparing `bencode_rs-0.0.2a4/Cargo.toml` & `bencode_rs-0.0.3/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "bencode"
 crate-type = ["cdylib"]
 
 [dependencies]
 bytes = "1.6.0"
+syncpool = '0.1.6'
 itoa = "1.0.11"
 # pyo3 = { version = "0.21.1", features = ["extension-module", 'abi3'] }
 pyo3 = { version = "0.21.2", features = ['abi3-py38'] }
 smallvec = "1.13.2"
 
 # "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
 # features = ["abi3-py38"]
```

### Comparing `bencode_rs-0.0.2a4/.github/workflows/_build_wheels.yaml` & `bencode_rs-0.0.3/.github/workflows/_build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a4/.github/workflows/ci.yaml` & `bencode_rs-0.0.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a4/.gitignore` & `bencode_rs-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a4/LICENSE` & `bencode_rs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a4/leak.py` & `bencode_rs-0.0.3/leak.py`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a4/src/decode.rs` & `bencode_rs-0.0.3/src/decode.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,110 @@
 use std::borrow::Cow;
-use std::collections::HashMap;
-use pyo3::ffi::{PyLong_FromString};
-use pyo3::prelude::*;
+
 use pyo3::{create_exception, PyResult, Python};
-use pyo3::exceptions::PyOverflowError;
-use pyo3::types::{PyBytes, PyDict, PyLong};
+use pyo3::exceptions::PyTypeError;
+use pyo3::ffi::PyLong_FromString;
+use pyo3::prelude::*;
+use pyo3::types::{PyBytes, PyDict};
 
 create_exception!(bencode_rs,BencodeDecodeError, pyo3::exceptions::PyException);
 
 type DecodeError = BencodeDecodeError;
 
 #[pyfunction]
-pub fn bdecode<'py>(py: Python<'py>, b: Bound<'py, PyBytes>) -> PyResult<Bound<'py, PyAny>> {
-    if b.len().unwrap() == 0 {
-        return Err(DecodeError::new_err("empty byte sequence"));
+#[pyo3(text_signature = "(b: Bytes, /)")]
+pub fn bdecode<'py>(py: Python<'py>, b: Py<PyAny>) -> PyResult<PyObject> {
+    let buf = match b.downcast_bound::<PyBytes>(py) {
+        Err(_) => {
+            return Err(PyTypeError::new_err("can only decode bytes"));
+        }
+        Ok(b) => b
+    };
+
+    if buf.len()? == 0 {
+        return Err(DecodeError::new_err("empty bytes"));
     }
 
     let mut ctx = Decoder {
-        bytes: b.as_bytes().to_vec(),
+        bytes: buf.as_bytes(),
         index: 0,
         py,
-        depth: 0,
+        // depth: 0,
     };
 
-    return Ok(ctx.decode_any()?.into_bound(py));
+    return Ok(ctx.decode_any()?);
 }
 
 
-pub type Object = PyObject;
-pub type DecodeResult = Result<Object, PyErr>;
-
 struct Decoder<'a> {
     // str_key: bool,
-    bytes: Vec<u8>,
+    bytes: &'a [u8],
     index: usize, // any torrent file larger than 4GiB?
     py: Python<'a>,
-    depth: usize,
 }
 
 impl<'a> Decoder<'a> {
     fn decode_any(&mut self) -> Result<PyObject, PyErr> {
         return match self.current_byte()? {
             b'i' => self.decode_int(),
-            b'0'..=b'9' => Ok(Cow::from(self.decode_bytes()?).into_py(self.py)),
-            b'l' => self.decode_list(),
+            b'0'..=b'9' => {
+                let bytes = self.decode_bytes()?;
+
+                return Ok(Cow::from(bytes).into_py(self.py));
+            }
+            b'l' => {
+                let list = self.decode_list()?;
+
+                return Ok(list.into_any());
+            }
             b'd' => self.decode_dict(),
             _ => return Err(DecodeError::new_err("invalid leading byte")),
         };
     }
 
+    fn decode_bytes(&mut self) -> Result<Vec<u8>, PyErr> {
+        let index_sep = match self.bytes[self.index..].iter().position(|&b| b == b':') {
+            Some(i) => i,
+            None => {
+                return Err(DecodeError::new_err(format!(
+                    "invalid bytes, missing length separator: index {}",
+                    self.index
+                )));
+            }
+        } + self.index;
+
+        if self.bytes[self.index] == b'0' && self.index + 1 != index_sep {
+            return Err(DecodeError::new_err(format!(
+                "invalid bytes length, leading '0' found at index {}",
+                self.index
+            )));
+        }
+
+        let mut len: usize = 0;
+        for c in self.bytes[self.index..index_sep].iter() {
+            len = len * 10 + (c - b'0') as usize;
+        }
+
+        let bytes_start: usize = index_sep + 1;
+        let bytes_end: usize = bytes_start + len - 1;
+
+        if bytes_end > self.bytes.len() - 1 {
+            return Err(DecodeError::new_err(format!(
+                "invalid bytes length, buffer overflow to {}: index {}, len {}",
+                bytes_end, self.index, len
+            )));
+        }
+
+        self.index = bytes_end + 1;
+
+        let str_buff: Vec<u8> = self.bytes[bytes_start..=bytes_end].to_vec();
+
+        return Ok(str_buff);
+    }
+
     fn decode_int(&mut self) -> Result<PyObject, PyErr> {
         let index_e = match self.bytes[self.index..].iter().position(|&b| b == b'e') {
             Some(i) => i,
             None => return Err(DecodeError::new_err("invalid int")),
         } + self.index;
 
         if index_e == self.index + 1 {
@@ -97,156 +149,120 @@
                 return Err(DecodeError::new_err(
                     format!("invalid int, '{}' found at {}", *c as char, self.index)
                 ));
             }
         }
 
         if sign < 0 {
-            // slow path to build PyLong with python
-            return self.decode_int_slow(index_e);
+            let mut val: i64 = 0;
+
+            for c_char in self.bytes[num_start..index_e].iter() {
+                let c = *c_char - b'0';
+                val = match val.checked_mul(10).and_then(|v| v.checked_add(c as i64)) {
+                    Some(v) => v,
+                    None => {
+                        return self.decode_int_slow(index_e);
+                    }
+                }
+            }
+
+            val = match val.checked_mul(-1) {
+                Some(v) => v,
+                None => {
+                    // slow path to build PyLong with python
+                    return self.decode_int_slow(index_e);
+                }
+            };
+
+            self.index = index_e + 1;
+            return Ok(val.into_py(self.py).into());
         }
 
-        let mut val: u128 = 0;
+        let mut val: u64 = 0;
 
         for c_char in self.bytes[num_start..index_e].iter() {
             let c = *c_char - b'0';
-            val = match val.checked_mul(10).and_then(|v| v.checked_add(c as u128)) {
+            val = match val.checked_mul(10).and_then(|v| v.checked_add(c as u64)) {
                 Some(v) => v,
                 None => {
                     return self.decode_int_slow(index_e);
                 }
             }
         }
 
         self.index = index_e + 1;
         return Ok(val.into_py(self.py).into());
     }
 
+    // support int may overflow i128/u128
     fn decode_int_slow(&mut self, index_e: usize) -> Result<PyObject, PyErr> {
         let s = self.bytes[self.index..index_e].to_vec();
 
         self.index = index_e + 1;
 
         let c_str = std::ffi::CString::new(s).unwrap();
+
         unsafe {
             let ptr = PyLong_FromString(c_str.as_ptr(), std::ptr::null_mut(), 10);
-
-            // panic!("not implemented");
             return Py::from_owned_ptr_or_err(self.py, ptr);
         };
     }
 
-    fn decode_bytes(&mut self) -> Result<Vec<u8>, PyErr> {
-        let index_sep = match self.bytes[self.index..].iter().position(|&b| b == b':') {
-            Some(i) => i,
-            None => {
-                return Err(DecodeError::new_err(format!(
-                    "invalid bytes, missing length separator: index {}",
-                    self.index
-                )));
-            }
-        } + self.index;
-
-        if self.bytes[self.index] == b'0' && self.index + 1 != index_sep {
-            return Err(DecodeError::new_err(format!(
-                "invalid bytes length, leading '0' found at index {}",
-                self.index
-            )));
-        }
-
-        let mut len: usize = 0;
-        for c in self.bytes[self.index..index_sep].iter() {
-            len = len * 10 + (c - b'0') as usize;
-        }
-
-        if index_sep + len >= self.bytes.len() {
-            return Err(DecodeError::new_err(format!(
-                "invalid bytes length, index out of range: index {}, len {}",
-                self.index, len
-            )));
-        }
-
-        let str_buff = self.bytes[index_sep + 1..index_sep + 1 + len].to_vec();
-
-        self.index = index_sep + len + 1;
-
-        // let o = PyBytes::new_bound(self.py, &str_buff);
-
-        return Ok(str_buff);
-    }
-
-    // fn check_depth(&mut self) -> Result<(), PyErr> {
-    //     if self.depth > 10000 {
-    //         return Err(DecodeError::new_err("object depth limit 10000 reached"));
-    //     }
-    //
-    //     return Ok(());
-    // }
-
-    fn decode_list(&mut self) -> DecodeResult {
-        // self.depth += 1;
-        // self.check_depth()?;
-
+    fn decode_list(&mut self) -> PyResult<PyObject> {
         self.index += 1;
-        let mut l = Vec::with_capacity(8);
+        let mut l = Vec::<PyObject>::with_capacity(16);
 
         loop {
             match self.bytes.get(self.index) {
                 None => {
                     return Err(DecodeError::new_err("unexpected end when parsing list".to_string()));
                 }
                 Some(b'e') => break,
                 Some(_) => {
                     l.push(self.decode_any()?);
                 }
             }
         }
 
-        // self.depth -= 1;
         self.index += 1;
-        return Ok(l.into_py(self.py));
+
+
+        Ok(l.into_py(self.py))
     }
 
-    fn decode_dict(&mut self) -> DecodeResult {
-        // self.depth += 1;
-        // self.check_depth()?;
+    fn decode_dict(&mut self) -> Result<PyObject, PyErr> {
         self.index += 1;
 
-        let mut map: HashMap<Cow<[u8]>, Object> = HashMap::with_capacity(8);
+        let d = PyDict::new_bound(self.py);
         let mut last_key: Option<Cow<[u8]>> = None;
         loop {
             match self.bytes.get(self.index) {
                 // unexpected data end
                 None => return Err(DecodeError::new_err("bytes end when decoding dict")),
                 // loop end
                 Some(b'e') => break,
                 Some(_) => {
                     let key = self.decode_bytes()?;
                     let value = self.decode_any()?;
-                    let ck = Cow::from(key.clone());
+
+                    let ck = Cow::from(key);
                     if let Some(lk) = last_key {
                         if lk > ck {
                             return Err(DecodeError::new_err(format!("dict key not sorted. index {}", self.index)));
                         } else if lk == ck {
                             return Err(DecodeError::new_err(format!("duplicated dict key found: index {}", self.index)));
                         }
                     }
-                    map.insert(ck.clone(), value);
+                    d.set_item(ck.clone().into_py(self.py), value.into_py(self.py))?;
+                    // map.insert(ck.clone(), value);
                     last_key = Some(ck);
                 }
             }
         }
 
-        let d = PyDict::new_bound(self.py);
-
-        for (k, v) in map.iter_mut() {
-            d.set_item(k.to_owned().into_py(self.py), v.to_owned())?;
-        }
-
-        // self.depth -= 1;
         self.index += 1;
         return Ok(d.into_py(self.py));
     }
 
     fn current_byte(&self) -> Result<u8, PyErr> {
         return match self.bytes.get(self.index) {
             None => {
```

### Comparing `bencode_rs-0.0.2a4/src/encode.rs` & `bencode_rs-0.0.3/src/encode.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,79 @@
-use std::borrow::Cow;
 use std::collections::HashSet;
 
-use bytes::{BufMut, Bytes, BytesMut};
+use bytes::{BufMut, BytesMut};
+use pyo3::{create_exception, exceptions::PyTypeError, prelude::*, types::{PyBool, PyBytes, PyDict, PyInt, PyList, PyString, PyTuple}};
 use pyo3::exceptions::PyValueError;
-use pyo3::{create_exception, exceptions::PyTypeError, ffi::Py_TYPE, prelude::*, types::{PyBool, PyBytes, PyDict, PyInt, PyList, PyString, PyTuple, PyType}};
 use smallvec::SmallVec;
+use syncpool::SyncPool;
 
 create_exception!(bencode_rs, BencodeEncodeError, pyo3::exceptions::PyException);
 
-type EncodeError = BencodeEncodeError;
+pub const MIB: usize = 1_048_576;
 
-struct Context<'py> {
-    buf: BytesMut,
-    seen: HashSet<usize>,
-    py: Python<'py>,
+pub fn init() {
+    unsafe {
+        CONTEXT_POOL.replace(SyncPool::with_builder(Context::initializer));
+    }
 }
 
 #[pyfunction]
 #[pyo3(text_signature = "(v: Any, /)")]
-pub fn bencode<'py>(py: Python<'py>, v: Bound<'py, PyAny>) -> PyResult<Cow<'py, [u8]>> {
-    let mut ctx = Context {
-        buf: BytesMut::with_capacity(4096),
-        seen: HashSet::with_capacity(100),
-        py,
-    };
+pub fn bencode<'py>(py: Python<'py>, v: Bound<'py, PyAny>) -> PyResult<Bound<'py, PyBytes>> {
+    let mut ctx = get_ctx();
+    // let mut ctx = Context::initializer();
+
+    encode_any(&mut ctx, py, v)?;
+
+    let r = PyBytes::new_bound(py, ctx.buf.as_ref());
+
+    release_ctx(ctx);
+
+    return Ok(r);
+}
+
+type EncodeError = BencodeEncodeError;
+
+static mut CONTEXT_POOL: Option<SyncPool<Context>> = None;
+
+fn get_ctx() -> Box<Context> {
+    unsafe {
+        CONTEXT_POOL.as_mut().unwrap().get()
+    }
+}
+
+fn release_ctx(mut ctx: Box<Context>) -> () {
+    // do not store large buffers
+    // who encode torrent >= 100 MiB normally?
+    if ctx.buf.capacity() > 100 * MIB {
+        return;
+    }
+    ctx.buf.clear();
+    ctx.seen.clear();
+    unsafe {
+        CONTEXT_POOL.as_mut().unwrap().put(ctx);
+    }
+}
+
 
-    encode_any(&mut ctx, v)?;
+struct Context {
+    buf: BytesMut,
+    seen: HashSet<usize>,
+}
 
-    return Ok(ctx.buf.to_vec().into());
+impl Context {
+    fn initializer() -> Self {
+        Self {
+            buf: BytesMut::with_capacity(4096),
+            seen: HashSet::with_capacity(100),
+        }
+    }
 }
 
-fn encode_any<'py>(ctx: &mut Context, value: Bound<'py, PyAny>) -> PyResult<()> {
+fn encode_any<'py>(ctx: &mut Context, py: Python<'py>, value: Bound<'py, PyAny>) -> PyResult<()> {
     if let Ok(s) = value.downcast::<PyString>() {
         let str = s.to_string();
         let mut buffer = itoa::Buffer::new();
         ctx.buf.put(buffer.format(str.len()).as_bytes());
         ctx.buf.put_u8(b':');
         ctx.buf.put(str.as_bytes());
 
@@ -83,15 +122,15 @@
             ));
         }
 
         ctx.seen.insert(ptr);
         ctx.buf.put_u8(b'l');
 
         for x in seq {
-            encode_any(ctx, x)?;
+            encode_any(ctx, py, x)?;
         }
 
         ctx.buf.put_u8(b'e');
         ctx.seen.remove(&ptr);
 
         return Ok(());
     }
@@ -104,15 +143,15 @@
             ));
         }
 
         ctx.seen.insert(ptr);
         ctx.buf.put_u8(b'l');
 
         for x in seq {
-            encode_any(ctx, x)?;
+            encode_any(ctx, py, x)?;
         }
 
         ctx.buf.put_u8(b'e');
         ctx.seen.remove(&ptr);
 
         return Ok(());
     }
@@ -123,72 +162,60 @@
             let repr = value.repr().unwrap().to_string();
             return Err(PyValueError::new_err(format!(
                 "circular reference found: {repr}"
             )));
         }
         ctx.seen.insert(ptr);
 
-        _encode_dict(ctx, dict)?;
+        encode_dict(ctx, py, dict)?;
 
         ctx.seen.remove(&ptr);
         return Ok(());
     }
 
     let typ = value.get_type();
     let name = typ.name()?;
 
     return Err(PyTypeError::new_err(format!("Unsupported type '{name}'")));
 }
 
-fn _encode_bytes(v: Cow<[u8]>, buf: &mut BytesMut) -> PyResult<()> {
-    let mut buffer = itoa::Buffer::new();
-
-    buf.put(buffer.format(v.len()).as_bytes());
-    buf.put_u8(b':');
-    buf.put(Bytes::from(v.to_vec()));
-
-    return Ok(());
-}
-
 #[inline]
 fn _encode_str<'py>(v: String, buf: &mut BytesMut) -> PyResult<()> {
     let mut buffer = itoa::Buffer::new();
 
     buf.put(buffer.format(v.len()).as_bytes());
     buf.put_u8(b':');
     buf.put(v.as_bytes());
 
     return Ok(());
 }
 
-fn _encode_dict<'py>(ctx: &mut Context, v: &Bound<'py, PyDict>) -> PyResult<()> {
+fn encode_dict<'py>(ctx: &mut Context, py: Python<'py>, v: &Bound<'py, PyDict>) -> PyResult<()> {
     ctx.buf.put_u8(b'd');
 
     let mut sv: SmallVec<[(String, Bound<'_, PyAny>); 8]> = SmallVec::with_capacity(v.len());
 
     for item in v.items().iter() {
         let (key, value): (PyObject, Bound<'_, PyAny>) = item.extract()?;
 
-        if let Ok(d) = key.extract::<&PyString>(ctx.py) {
+        if let Ok(d) = key.extract::<&PyString>(py) {
             let bb = d.to_string();
             sv.push((bb, value));
-        } else if let Ok(d) = key.extract::<&PyBytes>(ctx.py) {
+            continue;
+        }
+
+        if let Ok(d) = key.extract::<&PyBytes>(py) {
             sv.push((String::from_utf8(d.as_bytes().into())?, value));
-        } else {
-            unsafe {
-                let typ = Py_TYPE(key.as_ptr());
+            continue;
+        }
 
-                let bb = PyType::from_borrowed_type_ptr(ctx.py, typ);
-                let name = bb.qualname()?;
+        let typ = value.get_type();
+        let name = typ.name()?;
 
-                return Err(PyTypeError::new_err(format!(
-                    "Unsupported type {name} as dict keys"
-                )));
-            }
-        }
+        return Err(PyTypeError::new_err(format!("Unsupported type '{name}' as dict key")));
     }
 
     sv.sort_unstable_by(|a, b| a.0.cmp(&b.0));
 
     let mut last_key: Option<String> = None;
     for (key, _) in sv.clone() {
         if let Some(lk) = last_key {
@@ -200,14 +227,14 @@
         }
 
         last_key = Some(key);
     }
 
     for (key, value) in sv {
         _encode_str(key, &mut ctx.buf)?;
-        encode_any(ctx, value.into_any())?;
+        encode_any(ctx, py, value.into_any())?;
     }
 
     ctx.buf.put_u8(b'e');
 
     return Ok(());
 }
```

### Comparing `bencode_rs-0.0.2a4/src/lib.rs` & `bencode_rs-0.0.3/src/lib.rs`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 mod decode;
 mod encode;
 
 use pyo3::prelude::*;
 
 #[pymodule]
 fn _bencode(py: Python<'_>, m: &Bound<'_, PyModule>) -> PyResult<()> {
+    encode::init();
+
     m.add_function(wrap_pyfunction!(encode::bencode, m)?)?;
     m.add_function(wrap_pyfunction!(decode::bdecode, m)?)?;
     m.add(
         "BencodeEncodeError",
         py.get_type_bound::<encode::BencodeEncodeError>(),
     )?;
     m.add(
```

### Comparing `bencode_rs-0.0.2a4/tests/fixtures/56507.torrent.bin` & `bencode_rs-0.0.3/tests/fixtures/56507.torrent.bin`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a4/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin` & `bencode_rs-0.0.3/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a4/tests/test_1_encode.py` & `bencode_rs-0.0.3/tests/test_1_encode.py`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a4/tests/test_2_decode.py` & `bencode_rs-0.0.3/tests/test_2_decode.py`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a4/Cargo.lock` & `bencode_rs-0.0.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 name = "bencode"
 version = "0.0.0"
 dependencies = [
  "bytes",
  "itoa",
  "pyo3",
  "smallvec",
+ "syncpool",
 ]
 
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
@@ -224,14 +225,20 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syncpool"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "276c1fc00f41ad03bdcf390e81f967adfdb9c828c0a967e1c92df8050471c6bd"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "unicode-ident"
```

### Comparing `bencode_rs-0.0.2a4/pyproject.toml` & `bencode_rs-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "bencode-rs"
-version = "0.0.2a4"
+version = "0.0.3"
 requires-python = ">=3.8,<4.0"
 description = "a bencode parser binding build with pyo3"
 readme = "readme.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Rust",
@@ -16,13 +16,16 @@
 ]
 keywords = [
     "bittorrent",
     "bencode",
     "p2p",
 ]
 
+[project.urls]
+Homepage = 'https://github.com/trim21/bencode-rs'
+
 [tool.maturin]
 features = ["pyo3/extension-module"]
 module-name = "bencode_rs._bencode"
 
 [tool.cibuildwheel]
 skip = ["pp*", "*-musllinux_i686"]
```

### Comparing `bencode_rs-0.0.2a4/PKG-INFO` & `bencode_rs-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: bencode-rs
-Version: 0.0.2a4
+Version: 0.0.3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 License-File: LICENSE
 Summary: a bencode parser binding build with pyo3
 Keywords: bittorrent,bencode,p2p
 Requires-Python: >=3.8, <4.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Homepage, https://github.com/trim21/bencode-rs
 
 # A bencode serialize/deserialize library writte in Rust
 
 ## install
 
 ```shell
 pip install bencode-rs
```

