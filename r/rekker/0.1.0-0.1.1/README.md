# Comparing `tmp/rekker-0.1.0.tar.gz` & `tmp/rekker-0.1.1.tar.gz`

## Comparing `rekker-0.1.0.tar` & `rekker-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 rekker-0.1.0/Cargo.toml
--rw-r--r--   0        0        0     1066 2024-05-13 17:48:22.000000 rekker-0.1.0/LICENSE
--rw-r--r--   0        0        0      288 2024-05-13 17:48:22.000000 rekker-0.1.0/README.md
--rw-r--r--   0        0        0     2008 2024-05-13 17:48:22.000000 rekker-0.1.0/src/http1.rs
--rw-r--r--   0        0        0      201 2024-05-13 17:48:22.000000 rekker-0.1.0/src/lib.rs
--rw-r--r--   0        0        0     9354 2024-05-13 17:48:22.000000 rekker-0.1.0/src/literal.rs
--rw-r--r--   0        0        0       99 2024-05-13 17:48:22.000000 rekker-0.1.0/src/pipe/mod.rs
--rw-r--r--   0        0        0      680 2024-05-13 17:48:22.000000 rekker-0.1.0/src/pipe/pipe.rs
--rw-r--r--   0        0        0     1966 2024-05-13 17:48:22.000000 rekker-0.1.0/src/pipe/py.rs
--rw-r--r--   0        0        0     8647 2024-05-13 17:48:22.000000 rekker-0.1.0/src/pipe/tcp.rs
--rw-r--r--   0        0        0     1356 2024-05-13 17:48:22.000000 rekker-0.1.0/src/pipe/tls.rs
--rw-r--r--   0        0        0      212 2024-05-13 17:48:22.000000 rekker-0.1.0/src/pipe/udp.rs
--rw-r--r--   0        0        0      184 2024-05-13 17:48:22.000000 rekker-0.1.0/src/py.rs
--rw-r--r--   0        0        0    21023 2024-05-13 17:48:22.000000 rekker-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      387 2024-05-13 17:48:22.000000 rekker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      875 1970-01-01 00:00:00.000000 rekker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 rekker-0.1.1/Cargo.toml
+-rw-r--r--   0        0        0     1066 2024-05-26 12:08:46.000000 rekker-0.1.1/LICENSE
+-rw-r--r--   0        0        0      469 2024-05-26 12:08:46.000000 rekker-0.1.1/README.md
+-rw-r--r--   0        0        0      197 2024-05-26 12:08:46.000000 rekker-0.1.1/src/lib.rs
+-rw-r--r--   0        0        0    10174 2024-05-26 12:08:46.000000 rekker-0.1.1/src/literal.rs
+-rw-r--r--   0        0        0       99 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/mod.rs
+-rw-r--r--   0        0        0      680 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/pipe.rs
+-rw-r--r--   0        0        0     1966 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/py.rs
+-rw-r--r--   0        0        0     7659 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/tcp.rs
+-rw-r--r--   0        0        0     1356 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/tls.rs
+-rw-r--r--   0        0        0      212 2024-05-26 12:08:46.000000 rekker-0.1.1/src/pipe/udp.rs
+-rw-r--r--   0        0        0      312 2024-05-26 12:08:46.000000 rekker-0.1.1/src/py.rs
+-rw-r--r--   0        0        0     2389 2024-05-26 12:08:46.000000 rekker-0.1.1/src/req.rs
+-rw-r--r--   0        0        0    21723 2024-05-26 12:08:55.000000 rekker-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      387 2024-05-26 12:08:46.000000 rekker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 rekker-0.1.1/PKG-INFO
```

### Comparing `rekker-0.1.0/Cargo.toml` & `rekker-0.1.1/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 name = "rekker"
 description = "Attack library written for rust and python"
 authors = ["GlacierSG <iamglaciersg@gmail.com>"]
 repository = "https://github.com/GlacierSG/rekker"
 readme = "README.md"
 keywords = ["tcp","attack"]
 license = "MIT"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 pyo3 = { version = "0.21.2", features = ["extension-module"], optional = true}
 colored = "2.1.0"
 rustls = "0.23.5"
 webpki-roots = "0.26.1"
+ctrlc = "3.4.4"
 
 [lib]
 crate-type = ["cdylib", "lib"]
```

### Comparing `rekker-0.1.0/LICENSE` & `rekker-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rekker-0.1.0/src/http1.rs` & `rekker-0.1.1/src/req.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,91 @@
+use crate::literal::to_lit_colored;
+use colored::*;
 
-pub struct Http1 {
+pub struct Req {
     pub method: Vec<u8>,
     pub path: Vec<u8>,
     pub headers: Vec<(Vec<u8>, Vec<u8>)>,
     pub body_raw: Vec<u8>,
-    pub separator: Vec<u8>,
     pub proxied: bool,
     pub host: Vec<u8>,
+    pub tls: bool,
 }
 
-impl Http1 {
-    pub fn new() -> Http1 {
-        Http1 {
+impl Req {
+    pub fn new() -> Req {
+        Req {
             method: b"GET".to_vec(),
             path: b"/".to_vec(),
             headers: vec![],
             body_raw: b"".to_vec(),
-            separator: b"\r\n".to_vec(),
             host: b"".to_vec(),
             proxied: false,
+            tls: false,
         }
     }
 
     pub fn url(mut self, value: impl AsRef<[u8]>) -> Self {
         let value = value.as_ref();
 
+        let mut t = 0;
+        if value.len() >= 8 && &value[..8] == b"https://" {
+            self.tls = true;
+            t = 8;
+        }
+        else if value.len() >= 7 && &value[..7] == b"http://" {
+            self.tls = false;
+            t = 7;
+        }
+
         let mut l = value.len();
-        for i in 0..value.len() {
+        for i in t..value.len() {
             if value[i] == 47 {
                 l = i;
                 break;
             }
         }
         self.host = value[..l].to_vec();
         self.path = value[l..].to_vec();
-        self.headers.insert(0, (b"Host".to_vec(), value[..l].to_vec()));
+        if l-t > 1 {
+            self = self.header(b"Host", &value[t..l].to_vec());
+        }
         self
     }
 
     pub fn header(mut self, header: impl AsRef<[u8]>, value: impl AsRef<[u8]>) -> Self {
         self.headers.push((header.as_ref().to_vec(), value.as_ref().to_vec()));
         self
     }
 
     pub fn body(mut self, body: impl AsRef<[u8]>) -> Self {
         let body = body.as_ref();
         self.body_raw = body.to_vec();
-        self.header(b"Content-length", body.len().to_string())
+        self
     }
 
-    pub fn raw(&self) -> Vec<u8> {
-        let mut out = self.method.to_vec();
-        out.extend(b" ");
+    pub fn pretty(&self) -> String {
+        fn colored(b: &[u8]) -> String {
+            to_lit_colored(b, |x| x.into(), |x| x.yellow())
+        }
+        let mut out = colored(&self.method);
+        out.push_str(" ");
         if self.proxied {
-            out.extend(&self.host);
+            out.push_str(&colored(&self.host));
         }
-        out.extend(&self.path);
-        out.extend(b" HTTP/1.1");
-        out.extend(&self.separator);
+        out.push_str(&colored(&self.path));
+        out.push_str(" HTTP/1.1\n");
         for (header, value) in &self.headers {
-            out.extend(header);
-            out.extend(b": ");
-            out.extend(value);
-            out.extend(&self.separator);
+            out.push_str(&colored(&header));
+            out.push_str(": ");
+            out.push_str(&colored(&value));
+            out.push_str("\n");
         }
-        out.extend(&self.separator);
-        out.extend(&self.body_raw);
+        out.push_str("\n");
+        out.push_str(&colored(&self.body_raw));
         out
     }
 
     pub fn proxy(mut self) -> Self {
         self.proxied = true;
         self
     }
```

### Comparing `rekker-0.1.0/src/literal.rs` & `rekker-0.1.1/src/literal.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+use colored::*;
+
+pub fn to_lit_colored(bytes: impl AsRef<[u8]>, normal_fn: fn(&str) -> ColoredString, byte_fn: fn(&str) -> ColoredString) -> String {
+    let bytes = bytes.as_ref();
+    let mut lit = String::new();
+    for byte in bytes {
+        if *byte == 9  { lit.push_str(&format!("{}", byte_fn("\\t"))); }
+        else if *byte == 10 { lit.push_str(&format!("{}", byte_fn("\\n"))); }
+        else if *byte == 13 { lit.push_str(&format!("{}", byte_fn("\\r"))); }
+        else if *byte == 92 { lit.push_str(&format!("{}", byte_fn("\\\\"))); }
+        else if *byte >= 32 && *byte <= 126 {
+            lit.push_str(&format!("{}", normal_fn(&String::from_utf8(vec![*byte]).unwrap())));
+        }
+        else {
+            lit.push_str(&format!("{}", byte_fn(&format!("\\x{:02x}", byte))));
+        }
+    }
+    lit
+}
+
 pub fn from_lit(input: impl AsRef<[u8]>) -> Result<Vec<u8>, String> {
     let mut result = Vec::new();
     let bytes = input.as_ref();
     let mut i = 0;
 
     while i < bytes.len() {
         if bytes[i] == b'\\' {
```

### Comparing `rekker-0.1.0/src/pipe/pipe.rs` & `rekker-0.1.1/src/pipe/pipe.rs`

 * *Files identical despite different names*

### Comparing `rekker-0.1.0/src/pipe/py.rs` & `rekker-0.1.1/src/pipe/py.rs`

 * *Files identical despite different names*

### Comparing `rekker-0.1.0/src/pipe/tls.rs` & `rekker-0.1.1/src/pipe/tls.rs`

 * *Files identical despite different names*

### Comparing `rekker-0.1.0/Cargo.lock` & `rekker-0.1.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,20 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cfg_aliases"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
+
+[[package]]
 name = "clang-sys"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67523a3b4be3ce1989d607a828d036249522dd9c1c8de7f4dd2dae43a37369d1"
 dependencies = [
  "glob",
  "libc",
@@ -126,14 +132,24 @@
 checksum = "cbf2150cce219b664a8a70df7a1f933836724b503f8a413af9365b4dcc4d90b8"
 dependencies = [
  "lazy_static",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "ctrlc"
+version = "3.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "672465ae37dc1bc6380a6547a8883d5dd397b0f1faaad4f265726cc7042a5345"
+dependencies = [
+ "nix",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "dunce"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
 
 [[package]]
 name = "either"
@@ -287,14 +303,26 @@
 [[package]]
 name = "mirai-annotations"
 version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c9be0862c1b3f26a88803c4a49de6889c10e608b3ee9344e6ef5b45fb37ad3d1"
 
 [[package]]
+name = "nix"
+version = "0.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab2156c4fce2f8df6c499cc1c763e4394b7482525bf2a9701c9d79d215f519e4"
+dependencies = [
+ "bitflags",
+ "cfg-if",
+ "cfg_aliases",
+ "libc",
+]
+
+[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
@@ -468,17 +496,18 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rekker"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "colored",
+ "ctrlc",
  "pyo3",
  "rustls",
  "webpki-roots",
 ]
 
 [[package]]
 name = "ring"
```

### Comparing `rekker-0.1.0/PKG-INFO` & `rekker-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rekker
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Attack library written for rust and python
 Keywords: tcp,attack
 Author: GlacierSG <iamglaciersg@gmail.com>
@@ -13,17 +13,36 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/GlacierSG/rekker
 
 # Rekker
 
 Rekker is inspired by pwntools features for communicating with tcp sockets. 
-It is still in development and a lot of features do not exist or have not been tested properly.
+
+Rekker is still in development.
 
 ## Example
 ```python
 import rekker
-io = Tcp("localhost:1234")
+io = rekker.Tcp("localhost:1234")
+io.send(b"abc")
 io.sendline(b"abcd")
+io.sendlineafter(b"abc", b"cde")
+io.recv(123)
+io.recvn(123)
+io.recvline()
+io.recvuntil(b"abc")
+io.recvall()
 io.interactive()
+io.debug()
+io.close()
+```
+## Install
+### Rust
+```bash
+cargo add rekker
+```
+### Python
+```bash
+pip install rekker
 ```
```

