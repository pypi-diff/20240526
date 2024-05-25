# Comparing `tmp/mddatasetbuilder-1.3.8.tar.gz` & `tmp/mddatasetbuilder-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mddatasetbuilder-1.3.8.tar", last modified: Fri Sep  8 17:23:56 2023, max compression
+gzip compressed data, was "mddatasetbuilder-1.3.9.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `mddatasetbuilder-1.3.8.tar` & `mddatasetbuilder-1.3.9.tar`

### file list

```diff
@@ -1,42 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:23:56.893178 mddatasetbuilder-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:23:56.885177 mddatasetbuilder-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:23:56.885177 mddatasetbuilder-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14517 2023-09-08 17:23:56.893178 mddatasetbuilder-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:23:56.889178 mddatasetbuilder-1.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:23:56.889178 mddatasetbuilder-1.3.8/mddatasetbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-09-08 17:23:56.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/c_stack.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/c_stack.h
--rw-r--r--   0 runner    (1001) docker     (127)    26117 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/datasetbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/deepmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    11361 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/dps.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/qmcalc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/mddatasetbuilder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:23:56.889178 mddatasetbuilder-1.3.8/mddatasetbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14517 2023-09-08 17:23:56.000000 mddatasetbuilder-1.3.8/mddatasetbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-09-08 17:23:56.000000 mddatasetbuilder-1.3.8/mddatasetbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 17:23:56.000000 mddatasetbuilder-1.3.8/mddatasetbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-09-08 17:23:56.000000 mddatasetbuilder-1.3.8/mddatasetbuilder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-09-08 17:23:56.000000 mddatasetbuilder-1.3.8/mddatasetbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-08 17:23:56.000000 mddatasetbuilder-1.3.8/mddatasetbuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 17:23:56.893178 mddatasetbuilder-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 17:23:56.889178 mddatasetbuilder-1.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/tests/test_bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/tests/test_datasetbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-09-08 17:23:43.000000 mddatasetbuilder-1.3.8/tox.ini
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/.git_archival.txt
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/.gitattributes
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/.github/workflows/push.yml
+-rw-r--r--   0        0        0      529 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/.github/workflows/pyright.yml
+-rw-r--r--   0        0        0     1998 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1216 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/.gitignore
+-rw-r--r--   0        0        0     1178 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1116 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/CITATION.cff
+-rw-r--r--   0        0        0     1015 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/CMakeLists.txt
+-rw-r--r--   0        0        0     7652 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/LICENSE
+-rw-r--r--   0        0        0      152 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/codecov.yml
+-rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/docs/CNAME
+-rw-r--r--   0        0        0     3879 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/docs/README.md
+-rw-r--r--   0        0        0      144 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/__init__.py
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/__main__.py
+-rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/_logger.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/_version.py
+-rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/c_stack.cpp
+-rw-r--r--   0        0        0      187 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/c_stack.h
+-rw-r--r--   0        0        0    27008 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/datasetbuilder.py
+-rw-r--r--   0        0        0     4807 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/deepmd.py
+-rw-r--r--   0        0        0    12729 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/detect.py
+-rw-r--r--   0        0        0       56 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/dps.pyi
+-rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/dps.pyx
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/py.typed
+-rw-r--r--   0        0        0     1012 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/qmcalc.py
+-rw-r--r--   0        0        0     6498 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/mddatasetbuilder/utils.py
+-rw-r--r--   0        0        0     3133 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0       13 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/tests/__init__.py
+-rw-r--r--   0        0        0      962 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/tests/test.json
+-rw-r--r--   0        0        0      897 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/tests/test_bond.py
+-rw-r--r--   0        0        0      205 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/tests/test_cli.py
+-rw-r--r--   0        0        0     4363 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/tests/test_datasetbuilder.py
+-rw-r--r--   0        0        0      481 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/tox.ini
+-rw-r--r--   0        0        0    14546 2022-11-09 12:37:21.000000 mddatasetbuilder-1.3.9/PKG-INFO
```

### Comparing `mddatasetbuilder-1.3.8/.github/workflows/release.yml` & `mddatasetbuilder-1.3.9/.github/workflows/release.yml`

 * *Files 12% similar despite different names*

```diff
@@ -14,63 +14,63 @@
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         include:
           # linux-64
           - os: ubuntu-latest
-            python: 37
-            platform_id: manylinux_x86_64
-          # macos-x86-64
-          - os: macos-latest
-            python: 37
-            platform_id: macosx_x86_64
-          - os: macos-latest
             python: 38
+            platform_id: manylinux_x86_64
+          # macosx_universal2
+          - os: macos-14
+            python: 39
             platform_id: macosx_universal2
           # win-64
           - os: windows-2019
-            python: 37
+            python: 38
             platform_id: win_amd64
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.14.1
+        uses: pypa/cibuildwheel@v2.18
         env:
           CIBW_ARCHS: all
           CIBW_BUILD: cp${{ matrix.python }}-${{ matrix.platform_id }}
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
+          name: cibw-wheels-cp${{ matrix.python }}-${{ matrix.platform_id }}-${{ strategy.job-index }}
           path: ./wheelhouse/*.whl
 
   build_sdist:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: '3.10'
       - run: python -m pip install build
       - name: Build sdist
         run: python -m build --sdist
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
+          name: cibw-sdist
           path: dist/*.tar.gz
 
   upload_pypi:
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
     permissions:
         # IMPORTANT: this permission is mandatory for trusted publishing
         id-token: write
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
-          name: artifact
+          pattern: cibw-*
           path: dist
+          merge-multiple: true
 
       - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `mddatasetbuilder-1.3.8/.gitignore` & `mddatasetbuilder-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mddatasetbuilder-1.3.8/.pre-commit-config.yaml` & `mddatasetbuilder-1.3.9/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
     # there are many log files in tests
     # TODO: seperate py files and log files
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-json
     -   id: check-added-large-files
     -   id: check-merge-conflict
     -   id: check-symlinks
     -   id: check-toml
 # Python
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.287
+    rev: v0.4.4
     hooks:
     - id: ruff
       args: ["--fix"]
--   repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 23.7.0
-    hooks:
-    -   id: black-jupyter
+    - id: ruff-format
 # numpydoc
 -   repo: https://github.com/Carreau/velin
     rev: 0.0.12
     hooks:
     - id: velin
       args: ["--write"]
 # C++
 -   repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v16.0.6
+    rev: v18.1.5
     hooks:
     -   id: clang-format
 # Cython
 -   repo: https://github.com/MarcoGorelli/cython-lint
-    rev: v0.15.0
+    rev: v0.16.2
     hooks:
     -   id: cython-lint
     -   id: double-quote-cython-strings
+# CMake
+-   repo: https://github.com/cheshirekow/cmake-format-precommit
+    rev: v0.6.13
+    hooks:
+      - id: cmake-format
```

### Comparing `mddatasetbuilder-1.3.8/CITATION.cff` & `mddatasetbuilder-1.3.9/CITATION.cff`

 * *Files identical despite different names*

### Comparing `mddatasetbuilder-1.3.8/LICENSE` & `mddatasetbuilder-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mddatasetbuilder-1.3.8/PKG-INFO` & `mddatasetbuilder-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: mddatasetbuilder
-Version: 1.3.8
+Version: 1.3.9
 Summary: A script to generate molecular dynamics (MD) datasets for machine learning from given LAMMPS trajectories automatically.
-Author-email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
+Keywords: dataset,molecular dynamics
+Home-page: https://github.com/tongzhugroup/mddatasetbuilder
+Author-Email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -164,48 +166,45 @@
         General Public License ever published by the Free Software Foundation.
         
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
-        
-Project-URL: homepage, https://github.com/tongzhugroup/mddatasetbuilder
-Project-URL: documentation, https://mddatasetbuilder.njzjz.win/
-Project-URL: repository, https://github.com/tongzhugroup/mddatasetbuilder
-Keywords: dataset,molecular dynamics
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
+Project-URL: Homepage, https://github.com/tongzhugroup/mddatasetbuilder
+Project-URL: Documentation, https://mddatasetbuilder.njzjz.win/
+Project-URL: Repository, https://github.com/tongzhugroup/mddatasetbuilder
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: ase
 Requires-Dist: gaussianrunner>=1.0.20
 Requires-Dist: tqdm>=4.9.0
 Requires-Dist: coloredlogs
 Requires-Dist: lz4
 Requires-Dist: dpdata>=0.1.2
 Requires-Dist: openbabel-wheel>=3.1.0.0
-Provides-Extra: test
 Requires-Dist: requests; extra == "test"
 Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: pytest-cov<4; extra == "test"
 Requires-Dist: cython; extra == "test"
 Requires-Dist: fakegaussian>=0.0.3; extra == "test"
+Provides-Extra: test
+Description-Content-Type: text/markdown
 
 # MDDatasetBuilder
 
 [![DOI:10.1038/s41467-020-19497-z](https://img.shields.io/badge/DOI-10.1038%2Fs41467--020--19497--z-blue)](https://doi.org/10.1038/s41467-020-19497-z)
 [![Citations](https://citations.njzjz.win/10.1038/s41467-020-19497-z)](https://doi.org/10.1038/s41467-020-19497-z)
 [![python version](https://img.shields.io/pypi/pyversions/mddatasetbuilder.svg?logo=python&logoColor=white)](https://pypi.org/project/mddatasetbuilder)
 [![PyPI](https://img.shields.io/pypi/v/mddatasetbuilder.svg)](https://pypi.org/project/mddatasetbuilder)
```

### Comparing `mddatasetbuilder-1.3.8/docs/README.md` & `mddatasetbuilder-1.3.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `mddatasetbuilder-1.3.8/mddatasetbuilder/datasetbuilder.py` & `mddatasetbuilder-1.3.9/mddatasetbuilder/datasetbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,26 @@
 import gc
 import itertools
 import os
 import pickle
 import tempfile
 import time
 from collections import Counter, defaultdict
-from multiprocessing import cpu_count
+from typing import List, Optional
 
 import numpy as np
+from ase.atoms import Atoms
 from ase.data import atomic_numbers
 from ase.io import write as write_xyz
 from sklearn import preprocessing
 from sklearn.cluster import MiniBatchKMeans
 
 from ._logger import logger
-from .detect import Detect
+from ._version import version as __version__
+from .detect import Detect, DetectDump
 from .utils import (
     bytestolist,
     listtobytes,
     must_be_list,
     read_compressed_block,
     run_mp,
 )
@@ -94,15 +96,15 @@
         stepinterval=1,
         n_clusters=10000,
         n_each=1,
         qmkeywords="%nproc=4\n#force mn15/6-31g(d,p) Geom=PrintInputOrient",
         nproc=None,
         pbc=True,
         fragment=False,
-        errorfilename=None,
+        errorfilename: Optional[List[str]] = None,
         errorlimit=0.0,
         atom_pref=False,
     ):
         """Init the builder."""
         print(__doc__)
         print(f"Author:{__author__}  Email:{__email__}")
         atomname = np.array(atomname) if atomname else np.array(["C", "H", "O"])
@@ -121,15 +123,22 @@
             )
 
         self.dataset_dir = f"dataset_{dataset_name}"
         self.xyzfilename = dataset_name
         self.clusteratom = clusteratom if clusteratom else atomname
         self.atombondtype = []
         self.stepinterval = stepinterval
-        self.nproc = nproc if nproc else cpu_count()
+        if nproc:
+            self.nproc = nproc
+        else:
+            try:
+                self.nproc = len(os.sched_getaffinity(0))
+            except AttributeError:
+                # macos and windows
+                self.nproc = os.cpu_count()
         self.cutoff = cutoff
         self.n_clusters = n_clusters
         self.n_each = n_each
         self.writegjf = True
         self.gjfdir = f"{self.dataset_dir}_gjf"
         self.qmkeywords = must_be_list(qmkeywords)
         self.fragment = fragment
@@ -292,21 +301,23 @@
                     The eigenvalues of columb matrix.
                 symbols: collections.Counter
                     The elements of atoms.
         """
         step, lines = item
         results = []
         if step in self.dstep:
+            assert isinstance(self.crddetector, DetectDump)
             step_atoms, _ = self.crddetector.readcrd(lines)
             for atoma in self.dstep[step]:
                 # atom ID starts from 1
                 distances = step_atoms.get_distances(
                     atoma - 1, range(len(step_atoms)), mic=True
                 )
                 cutoffatoms = step_atoms[distances < self.cutoff]
+                assert isinstance(cutoffatoms, Atoms)
                 symbols = cutoffatoms.get_chemical_symbols()
                 results.append(
                     (
                         np.array([step, atoma]),
                         self._calcoulumbmatrix(cutoffatoms),
                         Counter(symbols),
                     )
@@ -354,15 +365,17 @@
         -------
         numpy.ndarray
             The selected index.
         """
         min_max_scaler = preprocessing.MinMaxScaler()
         X = np.array(min_max_scaler.fit_transform(X))
         clus = MiniBatchKMeans(
-            n_clusters=n_clusters, init_size=(min(3 * n_clusters, len(X))), n_init=3
+            n_clusters=n_clusters,
+            init_size=(min(3 * n_clusters, len(X))),
+            n_init=3,  # type: ignore
         )
         labels = clus.fit_predict(X)
         choosedidx = []
         for i in range(n_clusters):
             idx = np.where(labels == i)[0]
             if idx.size:
                 choosedidx.append(np.random.choice(idx, n_each))
@@ -467,14 +480,15 @@
         multiplicities = [
             self.detect_multiplicity(atoms_whole[atoms].get_chemical_symbols())
             for atoms in takenatomidindex
         ]
         multiplicity_whole = sum(multiplicities) - len(takenatomidindex) + 1
         multiplicity_whole_str = f"0 {multiplicity_whole}"
         title = "\nGenerated by MDDatasetMaker (Author: Jinzhe Zeng)\n"
+        connect = None
         if len(self.qmkeywords) > 1:
             connect = "\n--link1--\n"
             chk = [f"%chk={os.path.splitext(os.path.basename(gjffilename))[0]}.chk"]
         else:
             chk = []
         if len(takenatomidindex) == 1 or not self.fragment:
             buff.extend((*chk, self.qmkeywords[0], title, multiplicity_whole_str))
@@ -495,14 +509,15 @@
                         "{}(Fragment={}) {:.5f} {:.5f} {:.5f}".format(
                             atom.symbol, index, *atom.position
                         )
                         for atom in atoms_whole[atoms]
                     ]
                 )
         for kw in itertools.islice(self.qmkeywords, 1, None):
+            assert connect is not None
             buff.extend((connect, *chk, kw, title, f"0 {multiplicity_whole}", "\n"))
         buff.append("\n")
         with open(gjffilename, "w") as f:
             f.write("\n".join(buff))
 
     def _writestepxyzfile(self, item):
         """Write xyz files and GJF files in a timestep.
@@ -520,18 +535,20 @@
         results: int
             The number of written files.
         """
         step, lines = item
         results = 0
         if step in self.dstep:
             if len(lines) == 2:
+                assert isinstance(self.crddetector, DetectDump)
                 step_atoms, _ = self.crddetector.readcrd(lines[0])
-                molecules = self.bonddetector.readmolecule(lines[1])
+                molecules, _ = self.bonddetector.readmolecule(lines[1])
             else:
                 molecules, step_atoms = self.bonddetector.readmolecule(lines)
+            assert step_atoms is not None
             for atoma, trajatomfilename, itype, itotal in self.dstep[step]:
                 # update counter
                 folder = str(itotal // 1000).zfill(self.foldermaxlength)
                 atomtypenum = str(itype).zfill(self.maxlength)
                 # atom ID starts from 1
                 distances = step_atoms.get_distances(
                     atoma - 1, range(len(step_atoms)), mic=True
@@ -545,17 +562,18 @@
                     mol_atomid = np.array(mo)
                     if np.any(np.isin(mol_atomid, cutoffatomid)):
                         takenatomids.append(mol_atomid)
                         takenatomidindex.append(range(idsum, idsum + len(mol_atomid)))
                         idsum += len(mol_atomid)
                 idx = np.concatenate(takenatomids)
                 cutoffatoms = step_atoms[idx]
-                cutoffatoms[np.nonzero(idx == atoma - 1)[0][0]].tag = 1
+                assert isinstance(cutoffatoms, Atoms)
+                cutoffatoms[np.nonzero(idx == atoma - 1)[0][0]].tag = 1  # type: ignore
                 cutoffatoms.wrap(
-                    center=step_atoms[atoma - 1].position
+                    center=step_atoms[atoma - 1].position  # type: ignore
                     / cutoffatoms.get_cell_lengths_and_angles()[0:3],
                     pbc=cutoffatoms.get_pbc(),
                 )
                 write_xyz(
                     os.path.join(
                         self.dataset_dir,
                         folder,
@@ -622,14 +640,15 @@
         """Iterate over the model deviation file.
 
         Yields
         ------
         str
             the line of model deviation
         """
+        assert self.errorfilename is not None
         fns = must_be_list(self.errorfilename)
         for fn in fns:
             with open(fn) as f:
                 it = itertools.islice(f, 1, None)
                 yield from it
 
 
@@ -703,14 +722,19 @@
     parser.add_argument(
         "-e",
         "--errorlimit",
         help="Model deviation lower threshold. Atoms whose model deviation is less than the threshold will not be collected.",
         type=float,
         default=0.0,
     )
+    parser.add_argument(
+        "--version",
+        action="version",
+        version=f"MDDatasetBuilder {__version__}",
+    )
     args = parser.parse_args()
     DatasetBuilder(
         atomname=args.atomname,
         bondfilename=args.bondfile,
         dumpfilename=args.dumpfile,
         dataset_name=args.name,
         cutoff=args.cutoff,
```

### Comparing `mddatasetbuilder-1.3.8/mddatasetbuilder/deepmd.py` & `mddatasetbuilder-1.3.9/mddatasetbuilder/deepmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                     logfiles.append(os.path.join(root, logfile))
         multi_systems = dpdata.MultiSystems()
         with Pool() as pool:
             for system in pool.imap_unordered(
                 self._preparedeepmdforLOG, tqdm(logfiles, disable=None)
             ):
                 multi_systems.append(system)
-        multi_systems.to_deepmd_npy(self.deepmd_dir)
+        multi_systems.to_deepmd_npy(self.deepmd_dir)  # type: ignore
         for formula, system in multi_systems.systems.items():
             self.system_paths.append(os.path.join(self.deepmd_dir, formula))
             self.batch_size.append(
                 min(
                     max(32 // (system["coords"].shape[1]), 1), system["coords"].shape[0]
                 )
             )
```

### Comparing `mddatasetbuilder-1.3.8/mddatasetbuilder/detect.py` & `mddatasetbuilder-1.3.9/mddatasetbuilder/detect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """Detect from trajectory."""
+
 import pickle
 from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 from enum import Enum, auto
+from typing import List, Optional, Tuple, Union, cast
 
 import numpy as np
 from ase import Atom, Atoms
 from openbabel import openbabel
 
-from .dps import dps as connectmolecule
+from mddatasetbuilder.dps import dps as connectmolecule
 
 
 class Detect(metaclass=ABCMeta):
     """Detect structures from file(s)."""
 
     def __init__(self, filename, atomname, pbc, errorlimit=None, errorfilename=None):
         self.filename = filename
         self.atomname = atomname
         self.pbc = pbc
         self.errorlimit = errorlimit
         self.errorfilename = errorfilename
         self.steplinenum = self._readN()
 
     @abstractmethod
-    def _readN(self):
+    def _readN(self) -> int:
         pass
 
     @abstractmethod
-    def readatombondtype(self, item):
+    def readatombondtype(self, item) -> Tuple[dict, int]:
         """Read bond types of atoms such as C1111."""
         pass
 
     @abstractmethod
-    def readmolecule(self, lines):
+    def readmolecule(self, lines) -> Tuple[List[List[int]], Optional[Atoms]]:
         """Read molecules."""
         pass
 
     @staticmethod
     def gettype(inputtype):
         """Get the class for the input file type."""
         if inputtype == "bond":
@@ -49,14 +51,18 @@
 
 
 class DetectBond(Detect):
     """Detect from the LAMMPS bond file."""
 
     def _readN(self):
         """Read bondfile N, which should be at very beginning."""
+        N = None
+        atomtype = None
+        stepaindex = None
+        stepbindex = None
         # copy from reacnetgenerator on 2018-12-15
         with open(
             self.filename if isinstance(self.filename, str) else self.filename[0]
         ) as f:
             iscompleted = False
             for index, line in enumerate(f):
                 if line.startswith("#"):
@@ -67,15 +73,18 @@
                         else:
                             iscompleted = True
                             stepaindex = index
                         N = [int(s) for s in line.split() if s.isdigit()][0]
                         atomtype = np.zeros(N, dtype=int)
                 else:
                     s = line.split()
+                    assert atomtype is not None
                     atomtype[int(s[0]) - 1] = int(s[1])
+        if stepaindex is None or stepbindex is None or N is None or atomtype is None:
+            raise RuntimeError("The bond file is not completed")
         steplinenum = stepbindex - stepaindex
         self._N = N
         self.atomtype = atomtype
         self.atomnames = self.atomname[self.atomtype - 1]
         return steplinenum
 
     def readatombondtype(self, item):
@@ -105,70 +114,83 @@
                         for x in s[4 + int(s[2]) : 4 + 2 * int(s[2])]
                     )
                     d[pickle.dumps((self.atomnames[int(s[0]) - 1], atombond))].append(
                         int(s[0])
                     )
         return d, step
 
-    def readmolecule(self, lines):
+    def readmolecule(self, lines) -> Tuple[List[List[int]], Optional[Atoms]]:
         """Return molecules from lines.
 
         Parameters
         ----------
         lines : list of strs
             Lines of LAMMPS bond files.
 
         Returns
         -------
         molecules: list
             Indexes of atoms in molecules.
+        None
+            None
         """
         # copy from reacnetgenerator on 2018-12-15
-        bond = [None] * self._N
+        bond: List[Optional[List[int]]] = [None] * self._N
         for line in lines:
             if line:
                 if not line.startswith("#"):
                     s = line.split()
                     bond[int(s[0]) - 1] = [int(x) - 1 for x in s[3 : 3 + int(s[2])]]
-        molecules = connectmolecule(bond)
-        return molecules
+        bond_ = cast(List[List[int]], bond)
+        molecules = connectmolecule(bond_)
+        return molecules, None
 
 
 class DetectDump(Detect):
     """Detect from the dump file."""
 
     def _readN(self):
         # copy from reacnetgenerator on 2018-12-15
         iscompleted = False
+        N = None
+        atomtype = None
+        stepaindex = None
+        stepbindex = None
         with open(
             self.filename if isinstance(self.filename, str) else self.filename[0]
         ) as f:
+            linecontent = None
             for index, line in enumerate(f):
                 if line.startswith("ITEM:"):
                     linecontent = self.LineType.linecontent(line)
                     if linecontent == self.LineType.ATOMS:
                         keys = line.split()
                         self.id_idx = keys.index("id") - 2
                         self.tidx = keys.index("type") - 2
                         self.xidx = keys.index("x") - 2
                         self.yidx = keys.index("y") - 2
                         self.zidx = keys.index("z") - 2
                 else:
-                    if linecontent == self.LineType.NUMBER:
+                    if linecontent is None:
+                        raise RuntimeError("No ITEM: in the dump file")
+                    elif linecontent == self.LineType.NUMBER:
                         if iscompleted:
                             stepbindex = index
                             break
                         else:
                             iscompleted = True
                             stepaindex = index
                         N = int(line.split()[0])
                         atomtype = np.zeros(N, dtype=int)
                     elif linecontent == self.LineType.ATOMS:
                         s = line.split()
+                        assert atomtype is not None
                         atomtype[int(s[self.id_idx]) - 1] = int(s[self.tidx])
+        if stepaindex is None or stepbindex is None or N is None or atomtype is None:
+            raise RuntimeError("The dump file is not completed")
         steplinenum = stepbindex - stepaindex
         self._N = N
         self.atomtype = atomtype
         self.atomnames = self.atomname[self.atomtype - 1]
         return steplinenum
 
     def readatombondtype(self, item):
@@ -183,29 +205,31 @@
         -------
         dict
             dict of bond orders
         int
             the step index
         """
         (step, lines), needlerror = item
-        if needlerror:
-            trajline, errorline = lines
-            lerror = np.fromstring(errorline, dtype=float, sep=" ")[7:]
+        lerror: Optional[Union[np.ndarray, List[float]]] = None
         d = defaultdict(list)
         step_atoms, ids = self.readcrd(lines)
         if needlerror:
+            trajline, errorline = lines
+            lerror = np.fromstring(errorline, dtype=float, sep=" ")[7:]
             lerror = [x for (y, x) in sorted(zip(ids, lerror))]
         level = self._crd2bond(step_atoms, readlevel=True)
         for i, (n, l) in enumerate(zip(self.atomnames, level)):
-            if not needlerror or lerror[i] > self.errorlimit:
+            if lerror is None or (
+                self.errorlimit is not None and lerror[i] > self.errorlimit
+            ):
                 # Note that atom id starts from 1
                 d[pickle.dumps((n, sorted(l)))].append(i + 1)
         return d, step
 
-    def readmolecule(self, lines):
+    def readmolecule(self, lines) -> Tuple[List[List[int]], Optional[Atoms]]:
         """Return molecules from lines.
 
         Parameters
         ----------
         lines : list of strs
             Lines of LAMMPS bond files.
 
@@ -245,45 +269,48 @@
                 openbabel.vector3(cell[0][0], cell[0][1], cell[0][2]),
                 openbabel.vector3(cell[1][0], cell[1][1], cell[1][2]),
                 openbabel.vector3(cell[2][0], cell[2][1], cell[2][2]),
             )
             mol.CloneData(uc)
             mol.SetPeriodicMol()
         mol.ConnectTheDots()
-        if not readlevel:
-            bond = [[] for i in range(atomnumber)]
-        else:
+        # when readlevel is False, bond is used to store connected atoms
+        # otherwise, bondlevel is used to store bond orders
+        bond = [[] for i in range(atomnumber)]
+        if readlevel:
             mol.PerceiveBondOrders()
-            bondlevel = [[] for i in range(atomnumber)]
         mol.EndModify()
         for b in openbabel.OBMolBondIter(mol):
             s1 = b.GetBeginAtom().GetId()
             s2 = b.GetEndAtom().GetId()
             if not readlevel:
                 bond[s1].append(s2)
                 bond[s2].append(s1)
             else:
                 level = b.GetBondOrder()
-                bondlevel[s1].append(level)
-                bondlevel[s2].append(level)
-        return bondlevel if readlevel else bond
+                bond[s1].append(level)
+                bond[s2].append(level)
+        return bond
 
-    def readcrd(self, item):
+    def readcrd(self, item) -> Tuple[Atoms, List[int]]:
         """Only this function can read coordinates."""
         lines = item
         # box information
         ss = []
         step_atoms = []
         ids = []
+        linecontent = None
         for line in lines:
             if line:
                 if line.startswith("ITEM:"):
                     linecontent = self.LineType.linecontent(line)
                 else:
-                    if linecontent == self.LineType.ATOMS:
+                    if linecontent is None:
+                        raise RuntimeError("No ITEM: in the dump file")
+                    elif linecontent == self.LineType.ATOMS:
                         s = line.split()
                         ids.append(int(s[self.id_idx]))
                         step_atoms.append(
                             Atom(
                                 self.atomname[int(s[self.tidx]) - 1],
                                 (
                                     float(s[self.xidx]),
@@ -309,16 +336,16 @@
         yhi = ss[1][1] - max(0.0, yz)
         zlo = ss[2][0]
         zhi = ss[2][1]
         boxsize = np.array(
             [[xhi - xlo, 0.0, 0.0], [xy, yhi - ylo, 0.0], [xz, yz, zhi - zlo]]
         )
         # sort by ID
-        step_atoms = [x for (y, x) in sorted(zip(ids, step_atoms))]
-        step_atoms = Atoms(step_atoms, cell=boxsize, pbc=self.pbc)
+        step_atoms_ = [x for (y, x) in sorted(zip(ids, step_atoms))]
+        step_atoms = Atoms(step_atoms_, cell=boxsize, pbc=self.pbc)
         return step_atoms, ids
 
     class LineType(Enum):
         """Line type in the LAMMPS dump files."""
 
         TIMESTEP = auto()
         ATOMS = auto()
```

### Comparing `mddatasetbuilder-1.3.8/mddatasetbuilder/dps.pyx` & `mddatasetbuilder-1.3.9/mddatasetbuilder/dps.pyx`

 * *Files identical despite different names*

### Comparing `mddatasetbuilder-1.3.8/mddatasetbuilder/utils.py` & `mddatasetbuilder-1.3.9/mddatasetbuilder/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utils."""
+
 import itertools
 import pickle
 from multiprocessing import Pool, Semaphore
-from typing import BinaryIO, Union
+from typing import BinaryIO, List, TypeVar, Union, overload
 
 import lz4.frame
 from tqdm.auto import tqdm
 
 from ._logger import logger
 
 
@@ -187,15 +188,15 @@
         The compressed line.
 
     Returns
     -------
     object
         The decompressed object.
     """
-    return pickle.loads(decompress(x, isbytes=True))
+    return pickle.loads(decompress(x, isbytes=True))  # type: ignore
 
 
 def run_mp(nproc, **arg):
     """Process a file with multiple processors.
 
     Parameters
     ----------
@@ -226,15 +227,24 @@
         raise
     else:
         pool.close()
     finally:
         pool.join()
 
 
-def must_be_list(obj):
+T = TypeVar("T")
+
+
+@overload
+def must_be_list(obj: List[T]) -> List[T]: ...
+@overload
+def must_be_list(obj: T) -> List[T]: ...
+
+
+def must_be_list(obj: Union[T, List[T]]) -> List[T]:
     """Convert a object to a list if the object is not a list.
 
     Parameters
     ----------
     obj : Object
         The object to convert.
```

### Comparing `mddatasetbuilder-1.3.8/tests/test.json` & `mddatasetbuilder-1.3.9/tests/test.json`

 * *Files identical despite different names*

### Comparing `mddatasetbuilder-1.3.8/tests/test_bond.py` & `mddatasetbuilder-1.3.9/tests/test_bond.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test detecting bonds."""
+
 import numpy as np
 from ase import Atoms
 
 from mddatasetbuilder.detect import DetectDump
 
 
 def test_bond_pbc():
```

### Comparing `mddatasetbuilder-1.3.8/tests/test_datasetbuilder.py` & `mddatasetbuilder-1.3.9/tests/test_datasetbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Test."""
 
-
 import hashlib
 import json
 import math
 import os
 import tempfile
 from pathlib import Path
```

