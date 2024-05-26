# Comparing `tmp/bencode_rs-0.0.2a3.tar.gz` & `tmp/bencode_rs-0.0.2a4.tar.gz`

## Comparing `bencode_rs-0.0.2a3.tar` & `bencode_rs-0.0.2a4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a3/Cargo.toml
--rw-r--r--   0     1001      127      120 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/.coveragerc
--rw-r--r--   0     1001      127       13 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/.gitattributes
--rw-r--r--   0     1001      127      124 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/.github/renovate.json
--rw-r--r--   0     1001      127     3345 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/.github/workflows/_build_wheels.yaml
--rw-r--r--   0     1001      127      643 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/.github/workflows/build.yaml
--rw-r--r--   0     1001      127      538 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/.github/workflows/release.yaml
--rw-r--r--   0     1001      127      921 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/.github/workflows/tests.yaml
--rw-r--r--   0     1001      127     4828 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/.gitignore
--rw-r--r--   0     1001      127     1085 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/LICENSE
--rw-r--r--   0     1001      127     1081 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/bench.py
--rw-r--r--   0     1001      127      184 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/bencode_rs/__init__.py
--rw-r--r--   0     1001      127      188 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/bencode_rs/__init__.pyi
--rw-r--r--   0     1001      127      831 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/leak.py
--rw-r--r--   0     1001      127      300 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/readme.md
--rw-r--r--   0     1001      127      301 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/rustfmt.toml
--rw-r--r--   0     1001      127     7905 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/src/decode.rs
--rw-r--r--   0     1001      127     5612 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/src/encode.rs
--rw-r--r--   0     1001      127      557 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/src/lib.rs
--rw-r--r--   0     1001      127     5713 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/tests/fixtures/56507.torrent.bin
--rw-r--r--   0     1001      127   376318 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin
--rw-r--r--   0     1001      127     4397 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/tests/test_1_encode.py
--rw-r--r--   0     1001      127     3419 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/tests/test_2_decode.py
--rw-r--r--   0     1001      127     8499 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/Cargo.lock
--rw-r--r--   0     1001      127      802 2024-05-25 19:15:17.000000 bencode_rs-0.0.2a3/pyproject.toml
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a3/PKG-INFO
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a4/Cargo.toml
+-rw-r--r--   0     1001      127      120 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.coveragerc
+-rw-r--r--   0     1001      127       13 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.gitattributes
+-rw-r--r--   0     1001      127      124 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.github/renovate.json
+-rw-r--r--   0     1001      127     3084 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.github/workflows/_build_wheels.yaml
+-rw-r--r--   0     1001      127     1732 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.github/workflows/ci.yaml
+-rw-r--r--   0     1001      127      450 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.github/workflows/release.yaml
+-rw-r--r--   0     1001      127     4828 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/.gitignore
+-rw-r--r--   0     1001      127     1085 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/LICENSE
+-rw-r--r--   0     1001      127      184 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/bencode_rs/__init__.py
+-rw-r--r--   0     1001      127      188 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/bencode_rs/__init__.pyi
+-rw-r--r--   0     1001      127      831 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/leak.py
+-rw-r--r--   0     1001      127      300 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/readme.md
+-rw-r--r--   0     1001      127      123 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/requirements.txt
+-rw-r--r--   0     1001      127      301 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/rustfmt.toml
+-rw-r--r--   0     1001      127     7998 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/src/decode.rs
+-rw-r--r--   0     1001      127     5612 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/src/encode.rs
+-rw-r--r--   0     1001      127      557 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/src/lib.rs
+-rw-r--r--   0     1001      127     5713 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/tests/fixtures/56507.torrent.bin
+-rw-r--r--   0     1001      127   376318 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin
+-rw-r--r--   0     1001      127     4397 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/tests/test_1_encode.py
+-rw-r--r--   0     1001      127     3498 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/tests/test_2_decode.py
+-rw-r--r--   0     1001      127     8499 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/Cargo.lock
+-rw-r--r--   0     1001      127      648 2024-05-26 10:05:56.000000 bencode_rs-0.0.2a4/pyproject.toml
+-rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a4/PKG-INFO
```

### Comparing `bencode_rs-0.0.2a3/Cargo.toml` & `bencode_rs-0.0.2a4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/.github/workflows/_build_wheels.yaml` & `bencode_rs-0.0.2a4/.github/workflows/_build_wheels.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -112,19 +112,7 @@
     needs: [ "linux", "windows", "macos", "sdist" ]
     steps:
       - name: Merge Artifacts
         uses: actions/upload-artifact/merge@v4
         with:
           name: wheel
           pattern: wheels-*
-
-  check-dist:
-    name: Check dist
-    needs: [ merge-wheel-artifact ]
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/download-artifact@v4
-        with:
-          name: wheel
-          path: dist
-
-      - run: pipx run twine check --strict dist/*
```

### Comparing `bencode_rs-0.0.2a3/.gitignore` & `bencode_rs-0.0.2a4/.gitignore`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/LICENSE` & `bencode_rs-0.0.2a4/LICENSE`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/leak.py` & `bencode_rs-0.0.2a4/leak.py`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/src/decode.rs` & `bencode_rs-0.0.2a4/src/decode.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 use std::borrow::Cow;
 use std::collections::HashMap;
-use pyo3::ffi::PyLong_FromString;
+use pyo3::ffi::{PyLong_FromString};
 use pyo3::prelude::*;
 use pyo3::{create_exception, PyResult, Python};
-use pyo3::types::PyDict;
+use pyo3::exceptions::PyOverflowError;
+use pyo3::types::{PyBytes, PyDict, PyLong};
 
 create_exception!(bencode_rs,BencodeDecodeError, pyo3::exceptions::PyException);
 
 type DecodeError = BencodeDecodeError;
 
 #[pyfunction]
-#[pyo3(text_signature = "(b: bytes, /)")]
-pub fn bdecode(py: Python<'_>, b: Vec<u8>) -> PyResult<Bound<'_, PyAny>> {
-    if b.len() == 0 {
+pub fn bdecode<'py>(py: Python<'py>, b: Bound<'py, PyBytes>) -> PyResult<Bound<'py, PyAny>> {
+    if b.len().unwrap() == 0 {
         return Err(DecodeError::new_err("empty byte sequence"));
     }
 
     let mut ctx = Decoder {
-        bytes: b,
+        bytes: b.as_bytes().to_vec(),
         index: 0,
         py,
         depth: 0,
     };
 
     return Ok(ctx.decode_any()?.into_bound(py));
 }
@@ -35,25 +35,25 @@
     bytes: Vec<u8>,
     index: usize, // any torrent file larger than 4GiB?
     py: Python<'a>,
     depth: usize,
 }
 
 impl<'a> Decoder<'a> {
-    fn decode_any(&mut self) -> DecodeResult {
+    fn decode_any(&mut self) -> Result<PyObject, PyErr> {
         return match self.current_byte()? {
             b'i' => self.decode_int(),
             b'0'..=b'9' => Ok(Cow::from(self.decode_bytes()?).into_py(self.py)),
             b'l' => self.decode_list(),
             b'd' => self.decode_dict(),
             _ => return Err(DecodeError::new_err("invalid leading byte")),
         };
     }
 
-    fn decode_int(&mut self) -> DecodeResult {
+    fn decode_int(&mut self) -> Result<PyObject, PyErr> {
         let index_e = match self.bytes[self.index..].iter().position(|&b| b == b'e') {
             Some(i) => i,
             None => return Err(DecodeError::new_err("invalid int")),
         } + self.index;
 
         if index_e == self.index + 1 {
             return Err(DecodeError::new_err(format!(
@@ -96,35 +96,36 @@
             if !(b'0' <= *c && *c <= b'9') {
                 return Err(DecodeError::new_err(
                     format!("invalid int, '{}' found at {}", *c as char, self.index)
                 ));
             }
         }
 
-        if sign > 0 {
-            let mut val: u128 = 0;
+        if sign < 0 {
+            // slow path to build PyLong with python
+            return self.decode_int_slow(index_e);
+        }
 
-            for c_char in self.bytes[num_start..index_e].iter() {
-                let c = *c_char - b'0';
-                val = match val.checked_mul(10).and_then(|v| v.checked_add(c as u128)) {
-                    Some(v) => v,
-                    None => {
-                        return self.decode_int_slow(index_e);
-                    }
+        let mut val: u128 = 0;
+
+        for c_char in self.bytes[num_start..index_e].iter() {
+            let c = *c_char - b'0';
+            val = match val.checked_mul(10).and_then(|v| v.checked_add(c as u128)) {
+                Some(v) => v,
+                None => {
+                    return self.decode_int_slow(index_e);
                 }
             }
-
-            self.index = index_e + 1;
-            return Ok(val.into_py(self.py));
         }
 
-        return self.decode_int_slow(index_e);
+        self.index = index_e + 1;
+        return Ok(val.into_py(self.py).into());
     }
 
-    fn decode_int_slow(&mut self, index_e: usize) -> DecodeResult {
+    fn decode_int_slow(&mut self, index_e: usize) -> Result<PyObject, PyErr> {
         let s = self.bytes[self.index..index_e].to_vec();
 
         self.index = index_e + 1;
 
         let c_str = std::ffi::CString::new(s).unwrap();
         unsafe {
             let ptr = PyLong_FromString(c_str.as_ptr(), std::ptr::null_mut(), 10);
@@ -169,25 +170,25 @@
         self.index = index_sep + len + 1;
 
         // let o = PyBytes::new_bound(self.py, &str_buff);
 
         return Ok(str_buff);
     }
 
-    fn check_depth(&mut self) -> Result<(), PyErr> {
-        if self.depth > 10000 {
-            return Err(DecodeError::new_err("object depth limit 10000 reached"));
-        }
-
-        return Ok(());
-    }
+    // fn check_depth(&mut self) -> Result<(), PyErr> {
+    //     if self.depth > 10000 {
+    //         return Err(DecodeError::new_err("object depth limit 10000 reached"));
+    //     }
+    //
+    //     return Ok(());
+    // }
 
     fn decode_list(&mut self) -> DecodeResult {
-        self.depth += 1;
-        self.check_depth()?;
+        // self.depth += 1;
+        // self.check_depth()?;
 
         self.index += 1;
         let mut l = Vec::with_capacity(8);
 
         loop {
             match self.bytes.get(self.index) {
                 None => {
@@ -196,57 +197,56 @@
                 Some(b'e') => break,
                 Some(_) => {
                     l.push(self.decode_any()?);
                 }
             }
         }
 
-        self.depth -= 1;
+        // self.depth -= 1;
         self.index += 1;
         return Ok(l.into_py(self.py));
     }
 
     fn decode_dict(&mut self) -> DecodeResult {
-        self.depth += 1;
-        self.check_depth()?;
+        // self.depth += 1;
+        // self.check_depth()?;
         self.index += 1;
 
         let mut map: HashMap<Cow<[u8]>, Object> = HashMap::with_capacity(8);
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
                     let ck = Cow::from(key.clone());
-                    if !last_key.is_none() {
-                        let lk = last_key.unwrap();
+                    if let Some(lk) = last_key {
                         if lk > ck {
                             return Err(DecodeError::new_err(format!("dict key not sorted. index {}", self.index)));
                         } else if lk == ck {
                             return Err(DecodeError::new_err(format!("duplicated dict key found: index {}", self.index)));
                         }
                     }
-                    map.insert(ck.clone(), value.clone());
-                    last_key = Some(ck.clone());
+                    map.insert(ck.clone(), value);
+                    last_key = Some(ck);
                 }
             }
         }
 
         let d = PyDict::new_bound(self.py);
 
         for (k, v) in map.iter_mut() {
             d.set_item(k.to_owned().into_py(self.py), v.to_owned())?;
         }
 
-        self.depth -= 1;
+        // self.depth -= 1;
         self.index += 1;
         return Ok(d.into_py(self.py));
     }
 
     fn current_byte(&self) -> Result<u8, PyErr> {
         return match self.bytes.get(self.index) {
             None => {
```

### Comparing `bencode_rs-0.0.2a3/src/encode.rs` & `bencode_rs-0.0.2a4/src/encode.rs`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/src/lib.rs` & `bencode_rs-0.0.2a4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/tests/fixtures/56507.torrent.bin` & `bencode_rs-0.0.2a4/tests/fixtures/56507.torrent.bin`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin` & `bencode_rs-0.0.2a4/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/tests/test_1_encode.py` & `bencode_rs-0.0.2a4/tests/test_1_encode.py`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/tests/test_2_decode.py` & `bencode_rs-0.0.2a4/tests/test_2_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     ["raw", "expected"],
     [
         (b"i1e", 1),
         (b"i4927586304e", 4927586304),
         (b"0:", b""),
         (b"4:spam", b"spam"),
         (b"i-3e", -3),
+        (b"i-9223372036854775808e", -9223372036854775808),  # longlong int +1
         (b"i9223372036854775808e", 9223372036854775808),  # longlong int +1
         (b"i18446744073709551616e", 18446744073709551616),  # unsigned long long +1
         # long long int range -9223372036854775808, 9223372036854775807
         (b"i-9223372036854775808e", -9223372036854775808),
         (b"i9223372036854775808e", 9223372036854775808),
         (b"le", []),
         (b"l4:spam4:eggse", [b"spam", b"eggs"]),
```

### Comparing `bencode_rs-0.0.2a3/Cargo.lock` & `bencode_rs-0.0.2a4/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a3/pyproject.toml` & `bencode_rs-0.0.2a4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "bencode-rs"
-version = "0.0.2a3"
+version = "0.0.2a4"
 requires-python = ">=3.8,<4.0"
 description = "a bencode parser binding build with pyo3"
 readme = "readme.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Rust",
@@ -16,22 +16,13 @@
 ]
 keywords = [
     "bittorrent",
     "bencode",
     "p2p",
 ]
 
-[project.optional-dependencies]
-dev = [
-    # lint
-    "pre-commit",
-    # testing
-    "pytest",
-    "pytest-github-actions-annotate-failures==0.2.0",
-]
-
 [tool.maturin]
 features = ["pyo3/extension-module"]
 module-name = "bencode_rs._bencode"
 
 [tool.cibuildwheel]
 skip = ["pp*", "*-musllinux_i686"]
```

