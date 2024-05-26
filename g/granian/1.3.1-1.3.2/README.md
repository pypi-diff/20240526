# Comparing `tmp/granian-1.3.1.tar.gz` & `tmp/granian-1.3.2.tar.gz`

## Comparing `granian-1.3.1.tar` & `granian-1.3.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 granian-1.3.1/Cargo.toml
--rw-r--r--   0     1001      127     1486 2024-05-01 22:25:47.000000 granian-1.3.1/LICENSE
--rw-r--r--   0     1001      127    10387 2024-05-01 22:25:47.000000 granian-1.3.1/README.md
--rw-r--r--   0     1001      127       87 2024-05-01 22:25:47.000000 granian-1.3.1/granian/__init__.py
--rw-r--r--   0     1001      127       50 2024-05-01 22:25:47.000000 granian-1.3.1/granian/__main__.py
--rw-r--r--   0     1001      127      276 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_futures.py
--rw-r--r--   0     1001      127     3043 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_granian.pyi
--rw-r--r--   0     1001      127      143 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_imports.py
--rw-r--r--   0     1001      127     1677 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_internal.py
--rw-r--r--   0     1001      127     2935 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_loops.py
--rw-r--r--   0     1001      127       93 2024-05-01 22:25:47.000000 granian-1.3.1/granian/_types.py
--rw-r--r--   0     1001      127     3895 2024-05-01 22:25:47.000000 granian-1.3.1/granian/asgi.py
--rw-r--r--   0     1001      127     9221 2024-05-01 22:25:47.000000 granian-1.3.1/granian/cli.py
--rw-r--r--   0     1001      127      379 2024-05-01 22:25:47.000000 granian-1.3.1/granian/constants.py
--rw-r--r--   0     1001      127      615 2024-05-01 22:25:47.000000 granian-1.3.1/granian/http.py
--rw-r--r--   0     1001      127     1480 2024-05-01 22:25:47.000000 granian-1.3.1/granian/log.py
--rw-r--r--   0     1001      127      144 2024-05-01 22:25:47.000000 granian-1.3.1/granian/net.py
--rw-r--r--   0     1001      127        0 2024-05-01 22:25:47.000000 granian-1.3.1/granian/py.typed
--rw-r--r--   0     1001      127      769 2024-05-01 22:25:47.000000 granian-1.3.1/granian/rsgi.py
--rw-r--r--   0     1001      127    19087 2024-05-01 22:25:47.000000 granian-1.3.1/granian/server.py
--rw-r--r--   0     1001      127     1354 2024-05-01 22:25:47.000000 granian-1.3.1/granian/wsgi.py
--rw-r--r--   0     1001      127    12724 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/callbacks.rs
--rw-r--r--   0     1001      127     2031 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/errors.rs
--rw-r--r--   0     1001      127     6352 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/http.rs
--rw-r--r--   0     1001      127    22320 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/io.rs
--rw-r--r--   0     1001      127      302 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/mod.rs
--rw-r--r--   0     1001      127     4839 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/serve.rs
--rw-r--r--   0     1001      127      259 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/types.rs
--rw-r--r--   0     1001      127     4679 2024-05-01 22:25:47.000000 granian-1.3.1/src/asgi/utils.rs
--rw-r--r--   0     1001      127     1030 2024-05-01 22:25:47.000000 granian-1.3.1/src/asyncio.rs
--rw-r--r--   0     1001      127    13845 2024-05-01 22:25:47.000000 granian-1.3.1/src/callbacks.rs
--rw-r--r--   0     1001      127     2900 2024-05-01 22:25:47.000000 granian-1.3.1/src/conversion.rs
--rw-r--r--   0     1001      127     1345 2024-05-01 22:25:47.000000 granian-1.3.1/src/http.rs
--rw-r--r--   0     1001      127     1298 2024-05-01 22:25:47.000000 granian-1.3.1/src/io.rs
--rw-r--r--   0     1001      127      964 2024-05-01 22:25:47.000000 granian-1.3.1/src/lib.rs
--rw-r--r--   0     1001      127     9737 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/callbacks.rs
--rw-r--r--   0     1001      127      564 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/errors.rs
--rw-r--r--   0     1001      127     5970 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/http.rs
--rw-r--r--   0     1001      127    13340 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/io.rs
--rw-r--r--   0     1001      127      742 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/mod.rs
--rw-r--r--   0     1001      127     4839 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/serve.rs
--rw-r--r--   0     1001      127     8849 2024-05-01 22:25:47.000000 granian-1.3.1/src/rsgi/types.rs
--rw-r--r--   0     1001      127    11181 2024-05-01 22:25:47.000000 granian-1.3.1/src/runtime.rs
--rw-r--r--   0     1001      127     2298 2024-05-01 22:25:47.000000 granian-1.3.1/src/tcp.rs
--rw-r--r--   0     1001      127     1111 2024-05-01 22:25:47.000000 granian-1.3.1/src/tls.rs
--rw-r--r--   0     1001      127     1272 2024-05-01 22:25:47.000000 granian-1.3.1/src/utils.rs
--rw-r--r--   0     1001      127    37312 2024-05-01 22:25:47.000000 granian-1.3.1/src/workers.rs
--rw-r--r--   0     1001      127     4007 2024-05-01 22:25:47.000000 granian-1.3.1/src/ws.rs
--rw-r--r--   0     1001      127     4690 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/callbacks.rs
--rw-r--r--   0     1001      127     1557 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/http.rs
--rw-r--r--   0     1001      127       58 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/mod.rs
--rw-r--r--   0     1001      127     2455 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/serve.rs
--rw-r--r--   0     1001      127     6339 2024-05-01 22:25:47.000000 granian-1.3.1/src/wsgi/types.rs
--rw-r--r--   0     1001      127     4104 2024-05-01 22:25:47.000000 granian-1.3.1/tests/apps/asgi.py
--rw-r--r--   0     1001      127     3140 2024-05-01 22:25:47.000000 granian-1.3.1/tests/apps/rsgi.py
--rw-r--r--   0     1001      127     1123 2024-05-01 22:25:47.000000 granian-1.3.1/tests/apps/wsgi.py
--rw-r--r--   0     1001      127     2434 2024-05-01 22:25:47.000000 granian-1.3.1/tests/conftest.py
--rw-r--r--   0     1001      127       95 2024-05-01 22:25:47.000000 granian-1.3.1/tests/fixtures/media.png
--rw-r--r--   0     1001      127     1139 2024-05-01 22:25:47.000000 granian-1.3.1/tests/fixtures/tls/cert.pem
--rw-r--r--   0     1001      127     1704 2024-05-01 22:25:47.000000 granian-1.3.1/tests/fixtures/tls/key.pem
--rw-r--r--   0     1001      127     2791 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_asgi.py
--rw-r--r--   0     1001      127     1750 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_https.py
--rw-r--r--   0     1001      127     2756 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_rsgi.py
--rw-r--r--   0     1001      127     2611 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_ws.py
--rw-r--r--   0     1001      127     2300 2024-05-01 22:25:47.000000 granian-1.3.1/tests/test_wsgi.py
--rw-r--r--   0     1001      127    33752 2024-05-01 22:25:47.000000 granian-1.3.1/Cargo.lock
--rw-r--r--   0     1001      127     2907 2024-05-01 22:25:47.000000 granian-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    12565 1970-01-01 00:00:00.000000 granian-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 granian-1.3.2/Cargo.toml
+-rw-r--r--   0     1001      127     1486 2024-05-21 18:10:41.000000 granian-1.3.2/LICENSE
+-rw-r--r--   0     1001      127    10387 2024-05-21 18:10:41.000000 granian-1.3.2/README.md
+-rw-r--r--   0     1001      127       87 2024-05-21 18:10:41.000000 granian-1.3.2/granian/__init__.py
+-rw-r--r--   0     1001      127       50 2024-05-21 18:10:41.000000 granian-1.3.2/granian/__main__.py
+-rw-r--r--   0     1001      127      276 2024-05-21 18:10:41.000000 granian-1.3.2/granian/_futures.py
+-rw-r--r--   0     1001      127     3043 2024-05-21 18:10:41.000000 granian-1.3.2/granian/_granian.pyi
+-rw-r--r--   0     1001      127      143 2024-05-21 18:10:41.000000 granian-1.3.2/granian/_imports.py
+-rw-r--r--   0     1001      127     1677 2024-05-21 18:10:41.000000 granian-1.3.2/granian/_internal.py
+-rw-r--r--   0     1001      127     2935 2024-05-21 18:10:41.000000 granian-1.3.2/granian/_loops.py
+-rw-r--r--   0     1001      127       93 2024-05-21 18:10:41.000000 granian-1.3.2/granian/_types.py
+-rw-r--r--   0     1001      127     3895 2024-05-21 18:10:41.000000 granian-1.3.2/granian/asgi.py
+-rw-r--r--   0     1001      127     9221 2024-05-21 18:10:41.000000 granian-1.3.2/granian/cli.py
+-rw-r--r--   0     1001      127      379 2024-05-21 18:10:41.000000 granian-1.3.2/granian/constants.py
+-rw-r--r--   0     1001      127      615 2024-05-21 18:10:41.000000 granian-1.3.2/granian/http.py
+-rw-r--r--   0     1001      127     1480 2024-05-21 18:10:41.000000 granian-1.3.2/granian/log.py
+-rw-r--r--   0     1001      127      144 2024-05-21 18:10:41.000000 granian-1.3.2/granian/net.py
+-rw-r--r--   0     1001      127        0 2024-05-21 18:10:41.000000 granian-1.3.2/granian/py.typed
+-rw-r--r--   0     1001      127      769 2024-05-21 18:10:41.000000 granian-1.3.2/granian/rsgi.py
+-rw-r--r--   0     1001      127    19087 2024-05-21 18:10:41.000000 granian-1.3.2/granian/server.py
+-rw-r--r--   0     1001      127     1354 2024-05-21 18:10:41.000000 granian-1.3.2/granian/wsgi.py
+-rw-r--r--   0     1001      127    12724 2024-05-21 18:10:41.000000 granian-1.3.2/src/asgi/callbacks.rs
+-rw-r--r--   0     1001      127     2031 2024-05-21 18:10:41.000000 granian-1.3.2/src/asgi/errors.rs
+-rw-r--r--   0     1001      127     6352 2024-05-21 18:10:41.000000 granian-1.3.2/src/asgi/http.rs
+-rw-r--r--   0     1001      127    22320 2024-05-21 18:10:41.000000 granian-1.3.2/src/asgi/io.rs
+-rw-r--r--   0     1001      127      302 2024-05-21 18:10:41.000000 granian-1.3.2/src/asgi/mod.rs
+-rw-r--r--   0     1001      127     4839 2024-05-21 18:10:41.000000 granian-1.3.2/src/asgi/serve.rs
+-rw-r--r--   0     1001      127      259 2024-05-21 18:10:41.000000 granian-1.3.2/src/asgi/types.rs
+-rw-r--r--   0     1001      127     4679 2024-05-21 18:10:41.000000 granian-1.3.2/src/asgi/utils.rs
+-rw-r--r--   0     1001      127     1030 2024-05-21 18:10:41.000000 granian-1.3.2/src/asyncio.rs
+-rw-r--r--   0     1001      127    13845 2024-05-21 18:10:41.000000 granian-1.3.2/src/callbacks.rs
+-rw-r--r--   0     1001      127     2900 2024-05-21 18:10:41.000000 granian-1.3.2/src/conversion.rs
+-rw-r--r--   0     1001      127     1345 2024-05-21 18:10:41.000000 granian-1.3.2/src/http.rs
+-rw-r--r--   0     1001      127     1298 2024-05-21 18:10:41.000000 granian-1.3.2/src/io.rs
+-rw-r--r--   0     1001      127      964 2024-05-21 18:10:41.000000 granian-1.3.2/src/lib.rs
+-rw-r--r--   0     1001      127     9737 2024-05-21 18:10:41.000000 granian-1.3.2/src/rsgi/callbacks.rs
+-rw-r--r--   0     1001      127      564 2024-05-21 18:10:41.000000 granian-1.3.2/src/rsgi/errors.rs
+-rw-r--r--   0     1001      127     5970 2024-05-21 18:10:41.000000 granian-1.3.2/src/rsgi/http.rs
+-rw-r--r--   0     1001      127    13340 2024-05-21 18:10:41.000000 granian-1.3.2/src/rsgi/io.rs
+-rw-r--r--   0     1001      127      742 2024-05-21 18:10:41.000000 granian-1.3.2/src/rsgi/mod.rs
+-rw-r--r--   0     1001      127     4839 2024-05-21 18:10:41.000000 granian-1.3.2/src/rsgi/serve.rs
+-rw-r--r--   0     1001      127     8849 2024-05-21 18:10:41.000000 granian-1.3.2/src/rsgi/types.rs
+-rw-r--r--   0     1001      127    11253 2024-05-21 18:10:41.000000 granian-1.3.2/src/runtime.rs
+-rw-r--r--   0     1001      127     2298 2024-05-21 18:10:41.000000 granian-1.3.2/src/tcp.rs
+-rw-r--r--   0     1001      127     1111 2024-05-21 18:10:41.000000 granian-1.3.2/src/tls.rs
+-rw-r--r--   0     1001      127     1272 2024-05-21 18:10:41.000000 granian-1.3.2/src/utils.rs
+-rw-r--r--   0     1001      127    37182 2024-05-21 18:10:41.000000 granian-1.3.2/src/workers.rs
+-rw-r--r--   0     1001      127     4007 2024-05-21 18:10:41.000000 granian-1.3.2/src/ws.rs
+-rw-r--r--   0     1001      127     4863 2024-05-21 18:10:41.000000 granian-1.3.2/src/wsgi/callbacks.rs
+-rw-r--r--   0     1001      127     1557 2024-05-21 18:10:41.000000 granian-1.3.2/src/wsgi/http.rs
+-rw-r--r--   0     1001      127       58 2024-05-21 18:10:41.000000 granian-1.3.2/src/wsgi/mod.rs
+-rw-r--r--   0     1001      127     2455 2024-05-21 18:10:41.000000 granian-1.3.2/src/wsgi/serve.rs
+-rw-r--r--   0     1001      127     6339 2024-05-21 18:10:41.000000 granian-1.3.2/src/wsgi/types.rs
+-rw-r--r--   0     1001      127     4104 2024-05-21 18:10:41.000000 granian-1.3.2/tests/apps/asgi.py
+-rw-r--r--   0     1001      127     3140 2024-05-21 18:10:41.000000 granian-1.3.2/tests/apps/rsgi.py
+-rw-r--r--   0     1001      127     1123 2024-05-21 18:10:41.000000 granian-1.3.2/tests/apps/wsgi.py
+-rw-r--r--   0     1001      127     2434 2024-05-21 18:10:41.000000 granian-1.3.2/tests/conftest.py
+-rw-r--r--   0     1001      127       95 2024-05-21 18:10:41.000000 granian-1.3.2/tests/fixtures/media.png
+-rw-r--r--   0     1001      127     1139 2024-05-21 18:10:41.000000 granian-1.3.2/tests/fixtures/tls/cert.pem
+-rw-r--r--   0     1001      127     1704 2024-05-21 18:10:41.000000 granian-1.3.2/tests/fixtures/tls/key.pem
+-rw-r--r--   0     1001      127     2791 2024-05-21 18:10:41.000000 granian-1.3.2/tests/test_asgi.py
+-rw-r--r--   0     1001      127     1750 2024-05-21 18:10:41.000000 granian-1.3.2/tests/test_https.py
+-rw-r--r--   0     1001      127     2756 2024-05-21 18:10:41.000000 granian-1.3.2/tests/test_rsgi.py
+-rw-r--r--   0     1001      127     2611 2024-05-21 18:10:41.000000 granian-1.3.2/tests/test_ws.py
+-rw-r--r--   0     1001      127     2423 2024-05-21 18:10:41.000000 granian-1.3.2/tests/test_wsgi.py
+-rw-r--r--   0     1001      127    34181 2024-05-21 18:10:41.000000 granian-1.3.2/Cargo.lock
+-rw-r--r--   0     1001      127     2907 2024-05-21 18:10:41.000000 granian-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    12565 1970-01-01 00:00:00.000000 granian-1.3.2/PKG-INFO
```

### Comparing `granian-1.3.1/Cargo.toml` & `granian-1.3.2/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "granian"
-version = "1.3.1"
+version = "1.3.2"
 description = "A Rust HTTP server for Python applications"
 authors = ["Giovanni Barillari <g@baro.dev>"]
 license = "BSD-3-Clause"
 edition = "2021"
 
 keywords = ["web", "asyncio"]
 
@@ -32,14 +32,15 @@
 
 [dependencies]
 anyhow = "=1.0"
 futures = "0.3"
 http-body-util = { version = "=0.1" }
 hyper = { version = "=1.3", features = ["http1", "http2", "server"] }
 hyper-util = { version = "=0.1", features = ["server-auto", "tokio"] }
+itertools = "0.13"
 log = "0.4"
 percent-encoding = "=2.3"
 pin-project = "1.1"
 pyo3 = { version = "=0.21", features = ["anyhow", "extension-module", "generate-import-lib"] }
 pyo3-log = "=0.10"
 rustls-pemfile = "2.1"
 socket2 = { version = "0.5", features = ["all"] }
```

### Comparing `granian-1.3.1/LICENSE` & `granian-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/README.md` & `granian-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/_granian.pyi` & `granian-1.3.2/granian/_granian.pyi`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/_internal.py` & `granian-1.3.2/granian/_internal.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/_loops.py` & `granian-1.3.2/granian/_loops.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/asgi.py` & `granian-1.3.2/granian/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/cli.py` & `granian-1.3.2/granian/cli.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/http.py` & `granian-1.3.2/granian/http.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/log.py` & `granian-1.3.2/granian/log.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/rsgi.py` & `granian-1.3.2/granian/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/server.py` & `granian-1.3.2/granian/server.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/granian/wsgi.py` & `granian-1.3.2/granian/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/asgi/callbacks.rs` & `granian-1.3.2/src/asgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/asgi/errors.rs` & `granian-1.3.2/src/asgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/asgi/http.rs` & `granian-1.3.2/src/asgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/asgi/io.rs` & `granian-1.3.2/src/asgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/asgi/serve.rs` & `granian-1.3.2/src/asgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/asgi/utils.rs` & `granian-1.3.2/src/asgi/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/asyncio.rs` & `granian-1.3.2/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/callbacks.rs` & `granian-1.3.2/src/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/conversion.rs` & `granian-1.3.2/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/http.rs` & `granian-1.3.2/src/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/io.rs` & `granian-1.3.2/src/io.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/lib.rs` & `granian-1.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/rsgi/callbacks.rs` & `granian-1.3.2/src/rsgi/callbacks.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/rsgi/errors.rs` & `granian-1.3.2/src/rsgi/errors.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/rsgi/http.rs` & `granian-1.3.2/src/rsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/rsgi/io.rs` & `granian-1.3.2/src/rsgi/io.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/rsgi/mod.rs` & `granian-1.3.2/src/rsgi/mod.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/rsgi/serve.rs` & `granian-1.3.2/src/rsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/rsgi/types.rs` & `granian-1.3.2/src/rsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/runtime.rs` & `granian-1.3.2/src/runtime.rs`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
     pub fn context<'p>(&self, py: Python<'p>) -> Bound<'p, PyAny> {
         self.context.clone().into_bound(py)
     }
 }
 
 pub trait JoinError {
+    #[allow(dead_code)]
     fn is_panic(&self) -> bool;
 }
 
 pub trait Runtime: Send + 'static {
     type JoinError: JoinError + Send;
     type JoinHandle: Future<Output = Result<(), Self::JoinError>> + Send;
 
@@ -82,20 +83,22 @@
     where
         F: Future<Output = R> + Send + 'static;
 
     fn get_task_locals() -> Option<TaskLocals>;
 }
 
 pub trait SpawnLocalExt: Runtime {
+    #[allow(dead_code)]
     fn spawn_local<F>(&self, fut: F) -> Self::JoinHandle
     where
         F: Future<Output = ()> + 'static;
 }
 
 pub trait LocalContextExt: Runtime {
+    #[allow(dead_code)]
     fn scope_local<F, R>(&self, locals: TaskLocals, fut: F) -> Pin<Box<dyn Future<Output = R>>>
     where
         F: Future<Output = R> + 'static;
 }
 
 pub(crate) struct RuntimeWrapper {
     rt: tokio::runtime::Runtime,
```

### Comparing `granian-1.3.1/src/tcp.rs` & `granian-1.3.2/src/tcp.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/tls.rs` & `granian-1.3.2/src/tls.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/utils.rs` & `granian-1.3.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/workers.rs` & `granian-1.3.2/src/workers.rs`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,14 @@
         let tcp_listener = tokio::net::TcpListener::from_std($tcp_listener).unwrap();
         let local_addr = tcp_listener.local_addr().unwrap();
         let mut accept_loop = true;
 
         while accept_loop {
             tokio::select! {
                 Ok((stream, remote_addr)) = tcp_listener.accept() => {
-                    #[allow(clippy::redundant_closure_call)]
                     $inner(local_addr, remote_addr, stream)
                 },
                 _ = $quit_signal => {
                     accept_loop = false;
                 }
             }
         }
@@ -199,15 +198,14 @@
         let mut accept_loop = true;
 
         while accept_loop {
             tokio::select! {
                 accept = tls_listener.accept() => {
                     match accept {
                         Ok((stream, remote_addr)) => {
-                            #[allow(clippy::redundant_closure_call)]
                             $inner(local_addr, remote_addr, stream)
                         },
                         Err(err) => {
                             log::info!("TLS handshake failed with {:?}", err);
                         }
                     }
                 },
```

### Comparing `granian-1.3.1/src/ws.rs` & `granian-1.3.2/src/ws.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/wsgi/callbacks.rs` & `granian-1.3.2/src/wsgi/callbacks.rs`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 use http_body_util::BodyExt;
 use hyper::{
     body::{self, Bytes},
     header,
     http::{request, uri::Authority},
     Version,
 };
+use itertools::Itertools;
 use percent_encoding::percent_decode_str;
 use pyo3::{
     prelude::*,
     types::{IntoPyDict, PyDict},
 };
 use std::borrow::Cow;
 use std::net::SocketAddr;
@@ -47,23 +48,28 @@
         _ => "HTTP/1",
     };
     let server = (server_addr.ip().to_string(), server_addr.port().to_string());
     let client = client_addr.to_string();
     let content_type = parts.headers.remove(header::CONTENT_TYPE);
     let content_len = parts.headers.remove(header::CONTENT_LENGTH);
     let mut headers = Vec::with_capacity(parts.headers.len());
-    for (key, val) in &parts.headers {
+    for key in parts.headers.keys() {
         headers.push((
             format!("HTTP_{}", key.as_str().replace('-', "_").to_uppercase()),
-            val.to_str().unwrap_or_default(),
+            parts
+                .headers
+                .get_all(key)
+                .iter()
+                .map(|v| v.to_str().unwrap_or_default())
+                .join(","),
         ));
     }
     if !parts.headers.contains_key(header::HOST) {
         let host = parts.uri.authority().map_or("", Authority::as_str);
-        headers.push(("HTTP_HOST".to_string(), host));
+        headers.push(("HTTP_HOST".to_string(), host.to_string()));
     }
 
     Python::with_gil(|py| {
         let environ = PyDict::new_bound(py);
         environ.set_item(pyo3::intern!(py, "SERVER_PROTOCOL"), version)?;
         environ.set_item(pyo3::intern!(py, "SERVER_NAME"), server.0)?;
         environ.set_item(pyo3::intern!(py, "SERVER_PORT"), server.1)?;
```

### Comparing `granian-1.3.1/src/wsgi/http.rs` & `granian-1.3.2/src/wsgi/http.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/wsgi/serve.rs` & `granian-1.3.2/src/wsgi/serve.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/src/wsgi/types.rs` & `granian-1.3.2/src/wsgi/types.rs`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/apps/asgi.py` & `granian-1.3.2/tests/apps/asgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/apps/rsgi.py` & `granian-1.3.2/tests/apps/rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/apps/wsgi.py` & `granian-1.3.2/tests/apps/wsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/conftest.py` & `granian-1.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/fixtures/tls/cert.pem` & `granian-1.3.2/tests/fixtures/tls/cert.pem`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/fixtures/tls/key.pem` & `granian-1.3.2/tests/fixtures/tls/key.pem`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/test_asgi.py` & `granian-1.3.2/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/test_https.py` & `granian-1.3.2/tests/test_https.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/test_rsgi.py` & `granian-1.3.2/tests/test_rsgi.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/test_ws.py` & `granian-1.3.2/tests/test_ws.py`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/tests/test_wsgi.py` & `granian-1.3.2/tests/test_wsgi.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 
 @pytest.mark.asyncio
 @pytest.mark.skipif(bool(os.getenv('PGO_RUN')), reason='PGO build')
 @pytest.mark.parametrize('threading_mode', ['runtime', 'workers'])
 async def test_scope(wsgi_server, threading_mode):
     payload = 'body_payload'
     async with wsgi_server(threading_mode) as port:
-        res = httpx.post(f'http://localhost:{port}/info?test=true', content=payload)
+        res = httpx.post(
+            f'http://localhost:{port}/info?test=true', content=payload, headers=[('test', 'val1'), ('test', 'val2')]
+        )
 
     assert res.status_code == 200
     assert res.headers['content-type'] == 'application/json'
 
     data = res.json()
     assert data['scheme'] == 'http'
     assert data['method'] == 'POST'
     assert data['path'] == '/info'
     assert data['query_string'] == 'test=true'
     assert data['headers']['HTTP_HOST'] == f'localhost:{port}'
     assert data['content_length'] == str(len(payload))
+    assert data['headers']['HTTP_TEST'] == 'val1,val2'
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize('threading_mode', ['runtime', 'workers'])
 async def test_body(wsgi_server, threading_mode):
     async with wsgi_server(threading_mode) as port:
         res = httpx.post(f'http://localhost:{port}/echo', content='test')
```

### Comparing `granian-1.3.1/Cargo.lock` & `granian-1.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -127,14 +127,20 @@
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
+name = "either"
+version = "1.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
+
+[[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "fnv"
@@ -265,21 +271,22 @@
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "granian"
-version = "1.3.1"
+version = "1.3.2"
 dependencies = [
  "anyhow",
  "futures",
  "http-body-util",
  "hyper",
  "hyper-util",
+ "itertools",
  "log",
  "mimalloc",
  "percent-encoding",
  "pin-project",
  "pyo3",
  "pyo3-log",
  "rustls-pemfile",
@@ -434,14 +441,23 @@
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
+name = "itertools"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "413ee7dfc52ee1a4949ceeb7dbc8a33f2d6c088194d9f922fb8318faf1f01186"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "libc"
```

### Comparing `granian-1.3.1/pyproject.toml` & `granian-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `granian-1.3.1/PKG-INFO` & `granian-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: granian
-Version: 1.3.1
+Version: 1.3.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

