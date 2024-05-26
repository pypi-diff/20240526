# Comparing `tmp/fractus-0.1.7.tar.gz` & `tmp/fractus-0.1.8.tar.gz`

## Comparing `fractus-0.1.7.tar` & `fractus-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 fractus-0.1.7/Cargo.toml
--rw-r--r--   0        0        0     1066 2024-02-24 21:01:23.000000 fractus-0.1.7/LICENSE
--rw-r--r--   0        0        0      818 2024-02-24 21:01:23.000000 fractus-0.1.7/README.md
--rw-r--r--   0        0        0       40 2024-02-24 21:01:23.000000 fractus-0.1.7/rustfmt.toml
--rw-r--r--   0        0        0     6668 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/md4.rs
--rw-r--r--   0        0        0     6557 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/md5.rs
--rw-r--r--   0        0        0      231 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/mod.rs
--rw-r--r--   0        0        0     1771 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/py.rs
--rw-r--r--   0        0        0     7868 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/ripemd128.rs
--rw-r--r--   0        0        0     8703 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/ripemd160.rs
--rw-r--r--   0        0        0     8540 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/ripemd256.rs
--rw-r--r--   0        0        0     9361 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/ripemd320.rs
--rw-r--r--   0        0        0     5873 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/sha0.rs
--rw-r--r--   0        0        0     5878 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/sha1.rs
--rw-r--r--   0        0        0     7786 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/sha2_256.rs
--rw-r--r--   0        0        0     9420 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/sha2_512.rs
--rw-r--r--   0        0        0    53318 2024-02-24 21:01:23.000000 fractus-0.1.7/src/hash/whirlpool.rs
--rw-r--r--   0        0        0      303 2024-02-24 21:01:23.000000 fractus-0.1.7/src/lib.rs
--rw-r--r--   0        0        0      182 2024-02-24 21:01:23.000000 fractus-0.1.7/src/py.rs
--rw-r--r--   0        0        0     7858 2024-02-24 21:01:23.000000 fractus-0.1.7/Cargo.lock
--rw-r--r--   0        0        0      256 2024-02-24 21:01:23.000000 fractus-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 fractus-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 fractus-0.1.8/Cargo.toml
+-rw-r--r--   0        0        0     1066 2024-05-26 12:07:59.000000 fractus-0.1.8/LICENSE
+-rw-r--r--   0        0        0      834 2024-05-26 12:07:59.000000 fractus-0.1.8/README.md
+-rw-r--r--   0        0        0       40 2024-05-26 12:07:59.000000 fractus-0.1.8/rustfmt.toml
+-rw-r--r--   0        0        0     6668 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/md4.rs
+-rw-r--r--   0        0        0     6614 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/md5.rs
+-rw-r--r--   0        0        0      249 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/mod.rs
+-rw-r--r--   0        0        0     1781 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/py.rs
+-rw-r--r--   0        0        0     7868 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/ripemd128.rs
+-rw-r--r--   0        0        0     8703 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/ripemd160.rs
+-rw-r--r--   0        0        0     8540 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/ripemd256.rs
+-rw-r--r--   0        0        0     9361 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/ripemd320.rs
+-rw-r--r--   0        0        0     5930 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/sha0.rs
+-rw-r--r--   0        0        0     5935 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/sha1.rs
+-rw-r--r--   0        0        0     6607 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/sha2_224.rs
+-rw-r--r--   0        0        0     7843 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/sha2_256.rs
+-rw-r--r--   0        0        0     9477 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/sha2_512.rs
+-rw-r--r--   0        0        0    53318 2024-05-26 12:07:59.000000 fractus-0.1.8/src/hash/whirlpool.rs
+-rw-r--r--   0        0        0      303 2024-05-26 12:07:59.000000 fractus-0.1.8/src/lib.rs
+-rw-r--r--   0        0        0      310 2024-05-26 12:07:59.000000 fractus-0.1.8/src/py.rs
+-rw-r--r--   0        0        0    11151 2024-05-26 12:08:08.000000 fractus-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0      257 2024-05-26 12:07:59.000000 fractus-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1256 1970-01-01 00:00:00.000000 fractus-0.1.8/PKG-INFO
```

### Comparing `fractus-0.1.7/LICENSE` & `fractus-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fractus-0.1.7/README.md` & `fractus-0.1.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -34,13 +34,14 @@
 ## Features
 ### Length Extension Attack
 - [x] MD4
 - [x] MD5
 - [x] SHA0
 - [x] SHA1
 - [x] SHA2_256
+- [x] SHA2_224
 - [x] SHA2_512
 - [x] Ripemd128
 - [x] Ripemd160
 - [x] Ripemd256
 - [x] Ripemd320
-- [x] Whirlpool
+- [x] Whirlpool
```

### Comparing `fractus-0.1.7/src/hash/md4.rs` & `fractus-0.1.8/src/hash/md4.rs`

 * *Files identical despite different names*

### Comparing `fractus-0.1.7/src/hash/md5.rs` & `fractus-0.1.8/src/hash/md5.rs`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
                 self.transform();
                 offset = 0;
             }
         }
     }
 
     fn transform(&mut self) {
+        // Credit https://github.com/printfn/extendhash/
         let [mut a, mut b, mut c, mut d] = self.state;
         for i in 0..64 {
             let (e, j) = match i {
                 0..=15 => ((b & c) | (!b & d), i),
                 16..=31 => ((d & b) | (!d & c), (5 * i + 1) % 16),
                 32..=47 => (b ^ c ^ d, (3 * i + 5) % 16),
                 _ => (c ^ (b | !d), (7 * i) % 16),
```

### Comparing `fractus-0.1.7/src/hash/py.rs` & `fractus-0.1.8/src/hash/py.rs`

 * *Files 5% similar despite different names*

```diff
@@ -42,10 +42,10 @@
             )*
             Ok(())
         }
     };
 }
 
 make_py_func!(
-    md4, md5, ripemd128, ripemd160, ripemd256, ripemd320, sha0, sha1, sha2_256, sha2_512, whirlpool
+    md4, md5, ripemd128, ripemd160, ripemd256, ripemd320, sha0, sha1, sha2_224, sha2_256, sha2_512, whirlpool
 );
```

### Comparing `fractus-0.1.7/src/hash/ripemd128.rs` & `fractus-0.1.8/src/hash/ripemd128.rs`

 * *Files identical despite different names*

### Comparing `fractus-0.1.7/src/hash/ripemd160.rs` & `fractus-0.1.8/src/hash/ripemd160.rs`

 * *Files identical despite different names*

### Comparing `fractus-0.1.7/src/hash/ripemd256.rs` & `fractus-0.1.8/src/hash/ripemd256.rs`

 * *Files identical despite different names*

### Comparing `fractus-0.1.7/src/hash/ripemd320.rs` & `fractus-0.1.8/src/hash/ripemd320.rs`

 * *Files identical despite different names*

### Comparing `fractus-0.1.7/src/hash/sha0.rs` & `fractus-0.1.8/src/hash/sha0.rs`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                 self.transform();
                 offset = 0;
             }
         }
     }
 
     fn transform(&mut self) {
+        // Credit https://github.com/printfn/extendhash/
         let mut w = [0u32; 80];
         for i in 0..80 {
             if i < 16 {
                 w[i] = self.block[i];
             } else {
                 w[i] = w[i - 3] ^ w[i - 8] ^ w[i - 14] ^ w[i - 16];
             }
```

### Comparing `fractus-0.1.7/src/hash/sha1.rs` & `fractus-0.1.8/src/hash/sha1.rs`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                 self.transform();
                 offset = 0;
             }
         }
     }
 
     fn transform(&mut self) {
+        // Credit https://github.com/printfn/extendhash/
         let mut w = [0u32; 80];
         for i in 0..80 {
             if i < 16 {
                 w[i] = self.block[i];
             } else {
                 w[i] = (w[i - 3] ^ w[i - 8] ^ w[i - 14] ^ w[i - 16]).rotate_left(1);
             }
```

### Comparing `fractus-0.1.7/src/hash/sha2_256.rs` & `fractus-0.1.8/src/hash/sha2_256.rs`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,17 @@
                 self.transform();
                 offset = 0;
             }
         }
     }
 
     fn transform(&mut self) {
-        let mut w = [0u32; 80];
-        for i in 0..80 {
+        // Credit https://github.com/printfn/extendhash/
+        let mut w = [0u32; 64];
+        for i in 0..64 {
             if i < 16 {
                 w[i] = self.block[i];
             } else {
                 let s1 = w[i - 2].rotate_right(17) ^ w[i - 2].rotate_right(19) ^ (w[i - 2] >> 10);
                 let s0 = w[i - 15].rotate_right(7) ^ w[i - 15].rotate_right(18) ^ (w[i - 15] >> 3);
                 w[i] = s1
                     .wrapping_add(w[i - 7])
```

### Comparing `fractus-0.1.7/src/hash/sha2_512.rs` & `fractus-0.1.8/src/hash/sha2_512.rs`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
                 self.transform();
                 offset = 0;
             }
         }
     }
 
     fn transform(&mut self) {
+        // Credit https://github.com/printfn/extendhash/
         let mut w = [0u64; 80];
         for i in 0..80 {
             if i < 16 {
                 w[i] = self.block[i];
             } else {
                 let s1 = w[i - 2].rotate_right(19) ^ w[i - 2].rotate_right(61) ^ (w[i - 2] >> 6);
                 let s0 = w[i - 15].rotate_right(1) ^ w[i - 15].rotate_right(8) ^ (w[i - 15] >> 7);
```

### Comparing `fractus-0.1.7/src/hash/whirlpool.rs` & `fractus-0.1.8/src/hash/whirlpool.rs`

 * *Files identical despite different names*

### Comparing `fractus-0.1.7/Cargo.lock` & `fractus-0.1.8/Cargo.lock`

 * *Files 16% similar despite different names*

```diff
@@ -11,23 +11,46 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
+
+[[package]]
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
+name = "ctrlc"
+version = "3.4.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "672465ae37dc1bc6380a6547a8883d5dd397b0f1faaad4f265726cc7042a5345"
+dependencies = [
+ "nix",
+ "windows-sys",
+]
+
+[[package]]
 name = "fractus"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
+ "ctrlc",
  "pyo3",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -61,14 +84,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "nix"
+version = "0.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab2156c4fce2f8df6c499cc1c763e4394b7482525bf2a9701c9d79d215f519e4"
+dependencies = [
+ "bitflags 2.5.0",
+ "cfg-if",
+ "cfg_aliases",
+ "libc",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
@@ -86,15 +121,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
@@ -182,15 +217,15 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
@@ -227,62 +262,135 @@
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `fractus-0.1.7/PKG-INFO` & `fractus-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fractus
-Version: 0.1.7
+Version: 0.1.8
 Requires-Dist: cffi >=1.16.0
 License-File: LICENSE
 Summary: Cryptographic attack library for Rust and Python
 Keywords: crypto,attack
 Author: GlacierSG <iamglaciersg@gmail.com>
 Author-email: GlacierSG <iamglaciersg@gmail.com>
 License: MIT
@@ -47,13 +47,15 @@
 ## Features
 ### Length Extension Attack
 - [x] MD4
 - [x] MD5
 - [x] SHA0
 - [x] SHA1
 - [x] SHA2_256
+- [x] SHA2_224
 - [x] SHA2_512
 - [x] Ripemd128
 - [x] Ripemd160
 - [x] Ripemd256
 - [x] Ripemd320
 - [x] Whirlpool
+
```

