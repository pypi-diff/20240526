# Comparing `tmp/hpke-0.2.0.tar.gz` & `tmp/hpke-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpke-0.2.0.tar", max compression
+gzip compressed data, was "hpke-0.3.0.tar", max compression
```

## Comparing `hpke-0.2.0.tar` & `hpke-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11357 2022-04-09 08:54:19.710434 hpke-0.2.0/LICENSE
--rw-r--r--   0        0        0      894 2022-04-09 15:24:01.205221 hpke-0.2.0/README.md
--rw-r--r--   0        0        0    32768 2022-04-09 15:52:39.050289 hpke-0.2.0/hpke/.hpke.py.swp
--rw-r--r--   0        0        0       20 2021-08-08 20:10:13.624740 hpke-0.2.0/hpke/__init__.py
--rw-r--r--   0        0        0       22 2022-04-09 12:18:19.753425 hpke-0.2.0/hpke/__init__.py,cover
--rw-r--r--   0        0        0    19225 2022-04-09 15:55:21.592179 hpke-0.2.0/hpke/hpke.py
--rw-r--r--   0        0        0    14664 2022-04-09 12:20:06.296371 hpke-0.2.0/hpke/hpke.py,cover
--rw-r--r--   0        0        0      560 2022-04-09 15:58:39.965533 hpke-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1562 2022-04-09 15:59:42.436470 hpke-0.2.0/setup.py
--rw-r--r--   0        0        0     1474 2022-04-09 15:59:42.436651 hpke-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-04-09 08:54:19.710434 hpke-0.3.0/LICENSE
+-rw-r--r--   0        0        0      942 2022-04-10 07:38:33.849815 hpke-0.3.0/README.md
+-rw-r--r--   0        0        0       20 2021-08-08 20:10:13.624740 hpke-0.3.0/hpke/__init__.py
+-rw-r--r--   0        0        0       22 2022-04-09 12:18:19.753425 hpke-0.3.0/hpke/__init__.py,cover
+-rw-r--r--   0        0        0    19225 2022-04-09 15:55:21.592179 hpke-0.3.0/hpke/hpke.py
+-rw-r--r--   0        0        0    14664 2022-04-09 12:20:06.296371 hpke-0.3.0/hpke/hpke.py,cover
+-rw-r--r--   0        0        0      557 2024-05-26 08:59:09.423515 hpke-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1605 2024-05-26 09:00:33.229647 hpke-0.3.0/setup.py
+-rw-r--r--   0        0        0     1567 2024-05-26 09:00:33.229820 hpke-0.3.0/PKG-INFO
```

### Comparing `hpke-0.2.0/LICENSE` & `hpke-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hpke-0.2.0/README.md` & `hpke-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # hpke.py
 
 ![CI status](https://github.com/ctz/hpke-py/actions/workflows/ci.yaml/badge.svg)
+![PyPI version](https://shields.io/pypi/v/hpke)
 
 This is an implementation of [RFC9180](https://datatracker.ietf.org/doc/rfc9180/) in python3, using
 [cryptography.io](https://cryptography.io) for the underlying cryptography.
 
 ## Features
 
  - Modes
```

### Comparing `hpke-0.2.0/hpke/hpke.py` & `hpke-0.3.0/hpke/hpke.py`

 * *Files identical despite different names*

### Comparing `hpke-0.2.0/hpke/hpke.py,cover` & `hpke-0.3.0/hpke/hpke.py,cover`

 * *Files identical despite different names*

### Comparing `hpke-0.2.0/pyproject.toml` & `hpke-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "hpke"
-version = "0.2.0"
+version = "0.3.0"
 description = "HPKE implementation"
 authors = ["Joseph Birr-Pixton <jpixton@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/ctz/hpke-py"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-cryptography = "^3.4.7"
+cryptography = "^42"
 
 [tool.poetry.dev-dependencies]
 coverage = {version = "^5.5", extras = ["toml"]}
 pylint = "^2.10.2"
 pytest = "^6.2.4"
 pytest-cov = "^2.12.1"
 black = "^22.3.0"
```

### Comparing `hpke-0.2.0/setup.py` & `hpke-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['hpke']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['cryptography>=3.4.7,<4.0.0']
+['cryptography>=42,<43']
 
 setup_kwargs = {
     'name': 'hpke',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'HPKE implementation',
-    'long_description': '# hpke.py\n\n![CI status](https://github.com/ctz/hpke-py/actions/workflows/ci.yaml/badge.svg)\n\nThis is an implementation of [RFC9180](https://datatracker.ietf.org/doc/rfc9180/) in python3, using\n[cryptography.io](https://cryptography.io) for the underlying cryptography.\n\n## Features\n\n - Modes\n   - [x] mode_base\n   - [ ] mode_psk\n   - [x] mode_auth\n   - [ ] mode_auth_psk\n - AEADs\n   - [x] AES-128-GCM\n   - [x] AES-256-GCM\n   - [x] ChaCha20Poly1305\n   - [x] Export only\n - KEMs\n   - [x] DHKEM(P-256, HKDF-SHA256)\n   - [ ] DHKEM(P-384, HKDF-SHA384)\n   - [x] DHKEM(P-521, HKDF-SHA512)\n   - [ ] DHKEM(X25519, HKDF-SHA256)\n   - [ ] DHKEM(X448, HKDF-SHA512)\n - KDFs\n   - [x] HKDF-SHA256\n   - [x] HKDF-SHA384\n   - [x] HKDF-SHA512\n\n## Author\nJoseph Birr-Pixton <jpixton@gmail.com>\n\n## License\nhpke.py is licensed under the Apache License, Version 2.0. See\n[LICENSE](LICENSE) for the full license text.\n',
+    'long_description': '# hpke.py\n\n![CI status](https://github.com/ctz/hpke-py/actions/workflows/ci.yaml/badge.svg)\n![PyPI version](https://shields.io/pypi/v/hpke)\n\nThis is an implementation of [RFC9180](https://datatracker.ietf.org/doc/rfc9180/) in python3, using\n[cryptography.io](https://cryptography.io) for the underlying cryptography.\n\n## Features\n\n - Modes\n   - [x] mode_base\n   - [ ] mode_psk\n   - [x] mode_auth\n   - [ ] mode_auth_psk\n - AEADs\n   - [x] AES-128-GCM\n   - [x] AES-256-GCM\n   - [x] ChaCha20Poly1305\n   - [x] Export only\n - KEMs\n   - [x] DHKEM(P-256, HKDF-SHA256)\n   - [ ] DHKEM(P-384, HKDF-SHA384)\n   - [x] DHKEM(P-521, HKDF-SHA512)\n   - [ ] DHKEM(X25519, HKDF-SHA256)\n   - [ ] DHKEM(X448, HKDF-SHA512)\n - KDFs\n   - [x] HKDF-SHA256\n   - [x] HKDF-SHA384\n   - [x] HKDF-SHA512\n\n## Author\nJoseph Birr-Pixton <jpixton@gmail.com>\n\n## License\nhpke.py is licensed under the Apache License, Version 2.0. See\n[LICENSE](LICENSE) for the full license text.\n',
     'author': 'Joseph Birr-Pixton',
     'author_email': 'jpixton@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ctz/hpke-py',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `hpke-0.2.0/PKG-INFO` & `hpke-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: hpke
-Version: 0.2.0
+Version: 0.3.0
 Summary: HPKE implementation
 Home-page: https://github.com/ctz/hpke-py
 License: Apache-2.0
 Author: Joseph Birr-Pixton
 Author-email: jpixton@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: cryptography (>=3.4.7,<4.0.0)
+Requires-Dist: cryptography (>=42,<43)
 Project-URL: Repository, https://github.com/ctz/hpke-py
 Description-Content-Type: text/markdown
 
 # hpke.py
 
 ![CI status](https://github.com/ctz/hpke-py/actions/workflows/ci.yaml/badge.svg)
+![PyPI version](https://shields.io/pypi/v/hpke)
 
 This is an implementation of [RFC9180](https://datatracker.ietf.org/doc/rfc9180/) in python3, using
 [cryptography.io](https://cryptography.io) for the underlying cryptography.
 
 ## Features
 
  - Modes
```

