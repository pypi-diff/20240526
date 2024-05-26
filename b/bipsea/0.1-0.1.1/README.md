# Comparing `tmp/bipsea-0.1.tar.gz` & `tmp/bipsea-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipsea-0.1.tar", last modified: Sun May 26 12:14:29 2024, max compression
+gzip compressed data, was "bipsea-0.1.1.tar", last modified: Sun May 26 13:24:02 2024, max compression
```

## Comparing `bipsea-0.1.tar` & `bipsea-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 12:14:29.341127 bipsea-0.1/
--rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.1/LICENSE.md
--rw-r--r--   0 akarve     (501) staff       (20)      675 2024-05-26 12:14:29.340913 bipsea-0.1/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)     8922 2024-05-26 11:53:50.000000 bipsea-0.1/README.md
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 12:14:29.340717 bipsea-0.1/bipsea.egg-info/
--rw-r--r--   0 akarve     (501) staff       (20)      675 2024-05-26 12:14:29.000000 bipsea-0.1/bipsea.egg-info/PKG-INFO
--rw-r--r--   0 akarve     (501) staff       (20)      289 2024-05-26 12:14:29.000000 bipsea-0.1/bipsea.egg-info/SOURCES.txt
--rw-r--r--   0 akarve     (501) staff       (20)        1 2024-05-26 12:14:29.000000 bipsea-0.1/bipsea.egg-info/dependency_links.txt
--rw-r--r--   0 akarve     (501) staff       (20)       38 2024-05-26 12:14:29.000000 bipsea-0.1/bipsea.egg-info/entry_points.txt
--rw-r--r--   0 akarve     (501) staff       (20)       26 2024-05-26 12:14:29.000000 bipsea-0.1/bipsea.egg-info/requires.txt
--rw-r--r--   0 akarve     (501) staff       (20)        1 2024-05-26 12:14:29.000000 bipsea-0.1/bipsea.egg-info/top_level.txt
--rw-r--r--   0 akarve     (501) staff       (20)       38 2024-05-26 12:14:29.341177 bipsea-0.1/setup.cfg
--rw-r--r--   0 akarve     (501) staff       (20)     1063 2024-05-26 11:57:12.000000 bipsea-0.1/setup.py
-drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 12:14:29.340546 bipsea-0.1/tests/
--rw-r--r--   0 akarve     (501) staff       (20)     1296 2024-05-26 11:53:50.000000 bipsea-0.1/tests/test_bip32.py
--rw-r--r--   0 akarve     (501) staff       (20)     2161 2024-05-26 11:53:50.000000 bipsea-0.1/tests/test_bip39.py
--rw-r--r--   0 akarve     (501) staff       (20)     3687 2024-05-26 11:53:50.000000 bipsea-0.1/tests/test_bip85.py
--rw-r--r--   0 akarve     (501) staff       (20)     6533 2024-05-26 11:53:50.000000 bipsea-0.1/tests/test_cli.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.422500 bipsea-0.1.1/
+-rw-r--r--   0 akarve     (501) staff       (20)    11356 2024-05-26 11:53:50.000000 bipsea-0.1.1/LICENSE.md
+-rw-r--r--   0 akarve     (501) staff       (20)      676 2024-05-26 13:24:02.422308 bipsea-0.1.1/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)     8922 2024-05-26 11:53:50.000000 bipsea-0.1.1/README.md
+-rw-r--r--   0 akarve     (501) staff       (20)       38 2024-05-26 13:24:02.422539 bipsea-0.1.1/setup.cfg
+-rw-r--r--   0 akarve     (501) staff       (20)     1057 2024-05-26 13:21:53.000000 bipsea-0.1.1/setup.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.419278 bipsea-0.1.1/src/
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.420626 bipsea-0.1.1/src/bipsea/
+-rw-r--r--   0 akarve     (501) staff       (20)        0 2024-05-26 11:53:50.000000 bipsea-0.1.1/src/bipsea/__init__.py
+-rw-r--r--   0 akarve     (501) staff       (20)     8116 2024-05-26 12:50:48.000000 bipsea-0.1.1/src/bipsea/bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3669 2024-05-26 12:51:31.000000 bipsea-0.1.1/src/bipsea/bip32types.py
+-rw-r--r--   0 akarve     (501) staff       (20)     5797 2024-05-26 12:53:56.000000 bipsea-0.1.1/src/bipsea/bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     7814 2024-05-26 12:54:02.000000 bipsea-0.1.1/src/bipsea/bipsea.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3853 2024-05-26 12:54:08.000000 bipsea-0.1.1/src/bipsea/seedwords.py
+-rw-r--r--   0 akarve     (501) staff       (20)      864 2024-05-26 13:18:45.000000 bipsea-0.1.1/src/bipsea/util.py
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.422088 bipsea-0.1.1/src/bipsea.egg-info/
+-rw-r--r--   0 akarve     (501) staff       (20)      676 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/PKG-INFO
+-rw-r--r--   0 akarve     (501) staff       (20)      465 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/SOURCES.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        1 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/dependency_links.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       45 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/entry_points.txt
+-rw-r--r--   0 akarve     (501) staff       (20)       26 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/requires.txt
+-rw-r--r--   0 akarve     (501) staff       (20)        7 2024-05-26 13:24:02.000000 bipsea-0.1.1/src/bipsea.egg-info/top_level.txt
+drwxr-xr-x   0 akarve     (501) staff       (20)        0 2024-05-26 13:24:02.421906 bipsea-0.1.1/tests/
+-rw-r--r--   0 akarve     (501) staff       (20)     1324 2024-05-26 13:11:18.000000 bipsea-0.1.1/tests/test_bip32.py
+-rw-r--r--   0 akarve     (501) staff       (20)     2182 2024-05-26 13:11:18.000000 bipsea-0.1.1/tests/test_bip39.py
+-rw-r--r--   0 akarve     (501) staff       (20)     3708 2024-05-26 13:11:18.000000 bipsea-0.1.1/tests/test_bip85.py
+-rw-r--r--   0 akarve     (501) staff       (20)     6535 2024-05-26 13:11:18.000000 bipsea-0.1.1/tests/test_cli.py
```

### Comparing `bipsea-0.1/LICENSE.md` & `bipsea-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.1/PKG-INFO` & `bipsea-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.1
+Version: 0.1.1
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
-Keywords: Bitcoin BIP85  BIP32 cryptography
+Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.md
```

### Comparing `bipsea-0.1/README.md` & `bipsea-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bipsea-0.1/bipsea.egg-info/PKG-INFO` & `bipsea-0.1.1/src/bipsea.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bipsea
-Version: 0.1
+Version: 0.1.1
 Summary: Python implementation of BIP 85 (and BIP 32)
 Author: Aneesh Karve
 Author-email: bonded_metals_0u@icloud.com
 Project-URL: Source, https://github.com/akarve/bipsea
-Keywords: Bitcoin BIP85  BIP32 cryptography
+Keywords: Bitcoin BIP85 BIP32 cryptography
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.md
```

### Comparing `bipsea-0.1/setup.py` & `bipsea-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from setuptools import find_packages, setup
 
-from util import __app_name__, __version__
-
 setup(
-    name=__app_name__,
-    version=__version__,
-    packages=find_packages(),
+    name="bipsea",
+    version="0.1.1",
+    package_dir={"": "src"},
+    packages=find_packages(where="src"),
     description="Python implementation of BIP 85 (and BIP 32)",
     author="Aneesh Karve",
     author_email="bonded_metals_0u@icloud.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    keywords="Bitcoin BIP85  BIP32 cryptography",
+    keywords="Bitcoin BIP85 BIP32 cryptography",
     install_requires=[
         "click",
         "base58",
         "ecdsa",
         "pytest",
     ],
     tests_require=[
@@ -31,11 +30,11 @@
         "requests",
     ],
     project_urls={
         "Source": "https://github.com/akarve/bipsea",
     },
     entry_points={
         "console_scripts": [
-            "bipsea=bipsea:cli",
+            "bipsea=bipsea.bipsea:cli",
         ],
     },
 )
```

### Comparing `bipsea-0.1/tests/test_bip32.py` & `bipsea-0.1.1/tests/test_bip32.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 import pytest
 from data.bip32_vectors import INVALID_KEYS, VECTORS
 
-from bip32 import to_master_key
-from bip32types import parse_ext_key
-from bip85 import derive
-from util import LOGGER, from_hex
+from bipsea.bip32 import to_master_key
+from bipsea.bip32types import parse_ext_key
+from bipsea.bip85 import derive
+from bipsea.util import LOGGER, from_hex
 
 logger = logging.getLogger(LOGGER)
 
 
 @pytest.mark.parametrize(
     "vector",
     VECTORS,
```

### Comparing `bipsea-0.1/tests/test_bip39.py` & `bipsea-0.1.1/tests/test_bip39.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import warnings
 from unicodedata import is_normalized
 
 import pytest
 import requests
 from data.bip39_vectors import VECTORS
 
-from bip32 import to_master_key
-from seedwords import DICT_HASH, N_MNEMONICS, entropy_to_words, to_master_seed
-from util import LOGGER, from_hex
+from bipsea.bip32 import to_master_key
+from bipsea.seedwords import DICT_HASH, N_MNEMONICS, entropy_to_words, to_master_seed
+from bipsea.util import LOGGER, from_hex
 
 logger = logging.getLogger(LOGGER)
 
 WORD_COUNTS = {12, 15, 18, 21, 24}
 
 
 @pytest.mark.parametrize(
```

### Comparing `bipsea-0.1/tests/test_bip85.py` & `bipsea-0.1.1/tests/test_bip85.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     HEX,
     PWD_BASE64,
     PWD_BASE85,
     WIF,
     XPRV,
 )
 
-from bip32types import parse_ext_key
-from bip85 import DRNG, apply_85, derive, to_entropy, to_hex_string
-from util import LOGGER, to_hex_string
+from bipsea.bip32types import parse_ext_key
+from bipsea.bip85 import DRNG, apply_85, derive, to_entropy, to_hex_string
+from bipsea.util import LOGGER, to_hex_string
 
 logger = logging.getLogger(LOGGER)
 
 
 @pytest.mark.parametrize(
     "vector",
     EXT_KEY_TO_ENTROPY,
```

### Comparing `bipsea-0.1/tests/test_cli.py` & `bipsea-0.1.1/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 import pytest
 from click.testing import CliRunner
+from data.bip39_vectors import VECTORS
+from data.bip85_vectors import BIP39, HEX, PWD_BASE64, PWD_BASE85, WIF
 
-from bipsea import N_WORDS_ALLOWED, cli
-from tests.data.bip39_vectors import VECTORS
-from tests.data.bip85_vectors import BIP39, HEX, PWD_BASE64, PWD_BASE85, WIF
-from util import LOGGER
+from bipsea.bipsea import N_WORDS_ALLOWED, cli
+from bipsea.util import LOGGER
 
 logger = logging.getLogger(LOGGER)
 
 
 @pytest.fixture
 def runner():
     return CliRunner()
```

