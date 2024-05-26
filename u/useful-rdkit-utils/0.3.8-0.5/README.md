# Comparing `tmp/useful_rdkit_utils-0.3.8.tar.gz` & `tmp/useful_rdkit_utils-0.5.tar.gz`

## Comparing `useful_rdkit_utils-0.3.8.tar` & `useful_rdkit_utils-0.5.tar`

### file list

```diff
@@ -1,36 +1,70 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/.gitattributes
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/.lgtm.yml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/.readthedocs.yaml
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/MANIFEST.in
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/requirements.txt
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/.github/workflows/CI.yaml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/docs/Makefile
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/docs/source/conf.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/docs/source/index.rst
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/docs/source/installation.rst
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/docs/source/usage.rst
--rw-r--r--   0        0        0  1255975 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/notebooks/demo_REOS.ipynb
--rw-r--r--   0        0        0   251617 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/notebooks/demo_ring_systems.ipynb
--rw-r--r--   0        0        0   457681 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/notebooks/demo_useful_rdkit_utils.ipynb
--rw-r--r--   0        0        0    15105 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/notebooks/explore_functional_group_filters.ipynb
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/tests/test.smi
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/tests/test_reos.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/tests/test_ring_systems.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/tests/test_useful_rdkit_utils.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/useful_rdkit_utils/__init__.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/useful_rdkit_utils/pandas_utils.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/useful_rdkit_utils/reos.py
--rwxr-xr-x   0        0        0    10306 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/useful_rdkit_utils/ring_systems.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/useful_rdkit_utils/seaborn_utils.py
--rw-r--r--   0        0        0    12485 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/useful_rdkit_utils/useful_rdkit_utils.py
--rw-r--r--   0        0        0  1097792 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/useful_rdkit_utils/data/ring_systems/chembl_ring_systems.parquet
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/LICENSE
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.gitattributes
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.lgtm.yml
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/MANIFEST.in
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/requirements.txt
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/ring_freq_test.csv
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/ring_test.csv
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.github/workflows/CI.yaml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/.gitignore
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/misc.xml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/modules.xml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/useful_rdkit_utils.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/vcs.xml
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0  3405081 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/data/chembl_ring_systems.csv
+-rw-r--r--   0        0        0    40140 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/data/hia_hou.tab
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/data/test.smi
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/Makefile
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/conf.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/descriptors.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/geometry.rst
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/index.rst
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/installation.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/jupyter.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/misc_utils.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/pandas.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/reactions.rst
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/reos.rst
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/ring_systems.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/seaborn.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/stats.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/docs/source/units.rst
+-rw-r--r--   0        0        0    33382 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/bootstrap_AUC.ipynb
+-rw-r--r--   0        0        0   342969 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/demo_REOS.ipynb
+-rw-r--r--   0        0        0    54099 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/demo_descriptors.ipynb
+-rw-r--r--   0        0        0   461614 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/demo_ring_systems.ipynb
+-rw-r--r--   0        0        0   457681 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/demo_useful_rdkit_utils.ipynb
+-rw-r--r--   0        0        0    15105 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/explore_functional_group_filters.ipynb
+-rw-r--r--   0        0        0   590968 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/notebooks/zinc_sample.smi
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/__init__.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/ring_freq_test.csv
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/ring_test.csv
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/test.smi
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/test_reos.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/test_ring_systems.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/tests/test_useful_rdkit_utils.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/__init__.py
+-rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/descriptors.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/geometry.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/jupyter_utils.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/misc_utils.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/reactions.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/reos.py
+-rwxr-xr-x   0        0        0    11513 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/ring_systems.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/seaborn_utils.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/split_utils.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/stat_utils.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/units.py
+-rw-r--r--   0        0        0  1097792 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/useful_rdkit_utils/data/ring_systems/chembl_ring_systems.parquet
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/LICENSE
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/README.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/pyproject.toml
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 useful_rdkit_utils-0.5/PKG-INFO
```

### Comparing `useful_rdkit_utils-0.3.8/.readthedocs.yaml` & `useful_rdkit_utils-0.5/.readthedocs.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Required
 version: 2
 
 # Set the version of Python and other tools you might need
 build:
   os: ubuntu-20.04
   tools:
-    python: "3.9"
+    python: "3.11"
     # You can also specify other tool versions:
     # nodejs: "16"
     # rust: "1.55"
     # golang: "1.17"
 
 # Build documentation in the docs/ directory with Sphinx
 sphinx:
@@ -22,8 +22,8 @@
 # If using Sphinx, optionally build your docs in additional formats such as PDF
 # formats:
 #    - pdf
 
 # Optionally declare the Python requirements required to build your docs
 python:
    install:
-   - requirements: requirements.txt
+   - requirements: requirements.txt
```

### Comparing `useful_rdkit_utils-0.3.8/CHANGELOG.md` & `useful_rdkit_utils-0.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/CODE_OF_CONDUCT.md` & `useful_rdkit_utils-0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/.github/CONTRIBUTING.md` & `useful_rdkit_utils-0.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/.github/workflows/CI.yaml` & `useful_rdkit_utils-0.5/.github/workflows/CI.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 jobs:
   test:
     name: Test on ${{ matrix.os }}, Python ${{ matrix.python-version }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [macOS-latest, ubuntu-latest, windows-latest]
-        python-version: [3.7, 3.8, 3.9]
+        python-version: [3.11]
 
     steps:
     - uses: actions/checkout@v1
 
     - name: Additional info about the build
       shell: bash
       run: |
@@ -56,15 +56,15 @@
 
 
     - name: Run tests
 
       shell: bash
 
       run: |
-        pytest -v --cov=useful_rdkit_utils --cov-report=xml --color=yes useful_rdkit_utils/tests/
+        pytest -v --cov=useful_rdkit_utils --cov-report=xml --color=yes tests/
 
     - name: CodeCov
       uses: codecov/codecov-action@v1
       with:
         file: ./coverage.xml
         flags: unittests
         name: codecov-${{ matrix.os }}-py${{ matrix.python-version }}
```

### Comparing `useful_rdkit_utils-0.3.8/docs/Makefile` & `useful_rdkit_utils-0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/docs/source/conf.py` & `useful_rdkit_utils-0.5/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'useful_rdkit_utils'
 copyright = f'{date.today().year}, Pat Walters'
 author = 'Pat Walters'
 
 # The full version, including alpha/beta/rc tags.
-release = '0.1.6'
+release = '0.5.0'
 
 # The short X.Y version.
 parsed_version = re.match(
     '(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?',
     release,
 )
 version = parsed_version.expand('\g<major>.\g<minor>.\g<patch>')
@@ -86,15 +86,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -221,16 +221,18 @@
 # epub_exclude_files = ['search.html']
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {
-    'https://docs.python.org/3/': None,
-}
+#intersphinx_mapping = {
+#    'https://docs.python.org/3/': None,
+#}
+
+intersphinx_mapping = {'python': ('https://docs.python.org/3', None)}
 
 autoclass_content = 'both'
 
 # Don't sort alphabetically, explained at:
 # https://stackoverflow.com/questions/37209921/python-how-not-to-sort-sphinx-output-in-alphabetical-order
 autodoc_member_order = 'bysource'
```

### Comparing `useful_rdkit_utils-0.3.8/docs/source/installation.rst` & `useful_rdkit_utils-0.5/docs/source/installation.rst`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     $ pip install useful_rdkit_utils[viz,cli,jupyter]
 
 The most recent code and data can be installed directly from GitHub with:
 
 .. code-block:: shell
 
-    $ pip install git+https://github.com//useful_rdkit_utils.git
+    $ pip install git+https://github.com/PatWalters/useful_rdkit_utils.git
 
 To install in development mode, use the following:
 
 .. code-block:: shell
 
     $ git clone git+https://github.com//useful_rdkit_utils.git
     $ cd useful_rdkit_utils
```

### Comparing `useful_rdkit_utils-0.3.8/notebooks/demo_useful_rdkit_utils.ipynb` & `useful_rdkit_utils-0.5/notebooks/demo_useful_rdkit_utils.ipynb`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/notebooks/explore_functional_group_filters.ipynb` & `useful_rdkit_utils-0.5/notebooks/explore_functional_group_filters.ipynb`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/tests/test.smi` & `useful_rdkit_utils-0.5/data/test.smi`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/tests/test_ring_systems.py` & `useful_rdkit_utils-0.5/tests/test_ring_systems.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/tests/test_useful_rdkit_utils.py` & `useful_rdkit_utils-0.5/tests/test_useful_rdkit_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from io import StringIO
 import pandas as pd
 
 
 def generate_3D_mol():
     mol_block = """
-  Mrv2004 12282122453D          
+  Mrv2004 12282122453D
 
   6  6  0  0  0  0            999 V2000
    -0.0237   -1.2344   -1.9689 C   0  0  0  0  0  0  0  0  0  0  0  0
     0.1104   -1.0717   -0.4320 C   0  0  0  0  0  0  0  0  0  0  0  0
    -1.1007   -0.3176    0.1775 C   0  0  0  0  0  0  0  0  0  0  0  0
    -1.3506    1.0411   -0.5283 C   0  0  0  0  0  0  0  0  0  0  0  0
    -1.4847    0.8784   -2.0653 C   0  0  0  0  0  0  0  0  0  0  0  0
@@ -121,15 +121,15 @@
 Cn1c(=O)c2[nH]cnc2n(C)c1=O.NCC(=O)[O-].[Na+] 674529
 C[N+](C)(C)CCO.Cn1c(=O)c2[n-]cnc2n(C)c1=O 674385"""
     ifs = StringIO(buff)
     df = pd.read_csv(ifs, sep=" ", names=["SMILES", "Name"])
     df["mol"] = df.SMILES.apply(Chem.MolFromSmiles)
     df["fp"] = df.mol.apply(uru.mol2morgan_fp)
     clusters = uru.taylor_butina_clustering(df.fp.values)
-    assert str(clusters) == "[6 0 0 0 5 4 3 1 1 2]"
+    assert str(clusters) == "[6, 0, 0, 0, 5, 4, 3, 1, 1, 2]"
 
 
 def test_label_atoms():
     mol = Chem.MolFromSmiles("c1ccccc1")
     uru.label_atoms(mol, range(0, mol.GetNumAtoms()))
     atom_labels = [atm.GetProp("atomNote") for atm in mol.GetAtoms()]
     assert str(atom_labels) == "['0', '1', '2', '3', '4', '5']"
```

### Comparing `useful_rdkit_utils-0.3.8/useful_rdkit_utils/pandas_utils.py` & `useful_rdkit_utils-0.5/useful_rdkit_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/useful_rdkit_utils/reos.py` & `useful_rdkit_utils-0.5/useful_rdkit_utils/reos.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 import sys
-from pathlib import Path
+from typing import List, Optional
 
 import pandas as pd
 import pystow
 from rdkit import Chem
+from tqdm.auto import tqdm
+from rdkit.Chem.rdchem import Mol
+
 
 
 class REOS:
     """REOS - Rapid Elimination Of Swill\n
     Walters, Ajay, Murcko, "Recognizing molecules with druglike properties"\n
     Curr. Opin. Chem. Bio., 3 (1999), 384-387\n
     https://doi.org/10.1016/S1367-5931(99)80058-1
     """
 
-    def __init__(self, active_rules=None):
+    def __init__(self, active_rules: Optional[List[str]] = None) -> None:
+        """
+        Initialize the REOS class.
+
+        :param active_rules: List of active rules. If None, the default rule 'Glaxo' is used.
+        :type active_rules: Optional[List[str]]
+        :default active_rules: None
+        """
         self.output_smarts = False
         if active_rules is None:
             active_rules = ['Glaxo']
         url = 'https://raw.githubusercontent.com/PatWalters/rd_filters/master/rd_filters/data/alert_collection.csv'
         self.rule_path = pystow.ensure('useful_rdkit_utils', 'data', url=url)
+        self.active_rule_df = None
         self.rule_df = pd.read_csv(self.rule_path)
         self.read_rules(self.rule_path, active_rules)
 
     def set_output_smarts(self, output_smarts):
         """Determine whether SMARTS are returned
         :param output_smarts: True or False
         :return: None
@@ -59,41 +70,63 @@
                 available_rules = sorted(list(self.rule_df["rule_set_name"].unique()))
                 raise ValueError(f"Supplied rules: {active_rules} not available. Please select from {available_rules}")
 
         else:
             print("Error reading rules, please fix the SMARTS errors reported above", file=sys.stderr)
             sys.exit(1)
         if active_rules is not None:
-            self.active_rule_df = self.rule_df.query("rule_set_name in @active_rules")
+            self.active_rule_df = self.rule_df.query("rule_set_name in @active_rules").copy()
         else:
-            self.active_rule_df = self.rule_df
+            self.active_rule_df = self.rule_df.copy()
 
     def set_active_rule_sets(self, active_rules=None):
         """Set the active rule set(s)
 
         :param active_rules: list of active rule sets
         :return: None
         """
         assert active_rules
         self.active_rule_df = self.rule_df.query("rule_set_name in @active_rules")
 
+    def set_min_priority(self, min_priority: int) -> None:
+        """Set the minimum priority for rules to be included in the active rule set.
+
+        :param min_priority: The minimum priority for rules to be included.
+        :return: None
+        """
+        # reset active_rule_df
+        self.active_rule_df = self.rule_df.query("rule_set_name in @active_rules").copy()
+        # filter to only include rules with priority greater than or equal to min_priority
+        self.active_rule_df = self.active_rule_df.query("priority >= @min_priority")
+
     def get_available_rule_sets(self):
         """Get the available rule sets in rule_df
 
         :return: a list of available rule sets
         """
         return self.rule_df.rule_set_name.unique()
 
     def get_active_rule_sets(self):
         """Get the active rule sets in active_rule_df
 
         :return: a list of active rule sets
         """
         return self.active_rule_df.rule_set_name.unique()
 
+    def drop_rule(self, description: str) -> None:
+        """Drops a rule from the active rule set based on its description.
+
+        :param: description: The description of the rule to be dropped.
+        :return: None
+        """
+        num_rules_before = len(self.active_rule_df)
+        self.active_rule_df = self.active_rule_df.query("description != @description")
+        num_rules_after = len(self.active_rule_df)
+        print(f"Dropped {num_rules_before - num_rules_after} rule(s)")
+
     def get_rule_file_location(self):
         """Get the path to the rules file as a Path
 
         :return: Path for rules file
         """
         return self.rule_path
 
@@ -124,7 +157,37 @@
         :return: process_mol result or None if the SMILES can't be parsed
         """
         mol = Chem.MolFromSmiles(smiles)
         if mol is None:
             print(f"Error parsing SMILES {smiles}")
             return None
         return self.process_mol(mol)
+
+    def pandas_smiles(self, smiles_list: List[str]) -> pd.DataFrame:
+        """Process a list of SMILES strings
+
+        :param smiles_list: list of SMILES strings
+        :return: a pandas DataFrame with the results
+        """
+        results = []
+        for smiles in tqdm(smiles_list):
+            results.append(self.process_smiles(smiles))
+        if self.output_smarts:
+            column_names = ['rule_set_name', 'description', 'smarts']
+        else:
+            column_names = ['rule_set_name', 'description']
+        return pd.DataFrame(results, columns=column_names)
+
+    def pandas_mols(self, mol_list: List[Mol]) -> pd.DataFrame:
+        """Process a list of RDKit molecules
+
+        :param mol_list: list of RDKit molecules
+        :return: a pandas DataFrame with the results
+        """
+        results = []
+        for mol in tqdm(mol_list):
+            results.append(self.process_mol(mol))
+        if self.output_smarts:
+            column_names = ['rule_set_name', 'description', 'smarts']
+        else:
+            column_names = ['rule_set_name', 'description']
+        return pd.DataFrame(results, columns=column_names)
```

### Comparing `useful_rdkit_utils-0.3.8/useful_rdkit_utils/ring_systems.py` & `useful_rdkit_utils-0.5/useful_rdkit_utils/ring_systems.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python
+import itertools
+import sys
 from dataclasses import dataclass
+from importlib import resources
+from operator import itemgetter
 from pathlib import Path
 
+import click
+import pandas as pd
+import pystow
 from rdkit import Chem
 from rdkit.Chem.rdMolDescriptors import CalcNumRings
-import pandas as pd
 from tqdm.auto import tqdm
-import pystow
-import sys
-import click
-from operator import itemgetter
-from importlib import resources
+
 
 class RingSystemFinder:
     """A class to identify ring systems """
 
     def __init__(self):
         """Initialize susbstructure search objects to identify key functionality
         """
@@ -168,19 +170,19 @@
     def _read_file(cls, path: Path | str | None = None) -> pd.DataFrame:
         """
         Initialize the lookup table
         :param path: csv file with ring smiles and frequency
         """
         if path is None:
             with (
-                resources.files("useful_rdkit_utils")
-                .joinpath("data")
-                .joinpath("ring_systems")
-                .joinpath("chembl_ring_systems.parquet")
-                .open("rb")
+                    resources.files("useful_rdkit_utils")
+                            .joinpath("data")
+                            .joinpath("ring_systems")
+                            .joinpath("chembl_ring_systems.parquet")
+                            .open("rb")
             ) as f:
                 return pd.read_parquet(f)
         if isinstance(path, str) and path.startswith("https://"):
             path = pystow.ensure('useful_rdkit_utils', 'data', url=path)
         path = Path(path)
         if any(path.name.endswith(".csv" + c) for c in ["", ".gz", ".br", ".xz", ".zst"]):
             return pd.read_csv(path)
@@ -227,26 +229,27 @@
 def test_ring_system_lookup(input_filename, output_filename):
     """Test for RingSystemLookup
     :param input_filename: input smiles file
     :param output_filename: output csv file
     :return: None
     """
     df = pd.read_csv(input_filename, sep=" ", names=["SMILES", "Name"])
-    ring_system_lookup = RingSystemLookup()
+    ring_system_lookup = RingSystemLookup.default()
     min_freq_list = []
     for smi in tqdm(df.SMILES):
         freq_list = ring_system_lookup.process_smiles(smi)
         min_freq_list.append(get_min_ring_frequency(freq_list))
     df['min_ring'] = [x[0] for x in min_freq_list]
     df['min_freq'] = [x[1] for x in min_freq_list]
     df.to_csv(output_filename, index=False)
 
 
 def get_min_ring_frequency(ring_list):
     """Get minimum frequency from RingSystemLookup.process_smiles
+
     :param ring_list: output from RingSystemLookup.process_smiles
     :return: [ring_with minimum frequency, minimum frequency], acyclic molecules return ["",-1]
     """
     ring_list.sort(key=itemgetter(1))
     if len(ring_list):
         return ring_list[0]
     else:
@@ -264,9 +267,51 @@
         sys.exit(0)
     if mode == "build":
         create_ring_dictionary(infile, outfile)
     if mode == "search":
         test_ring_system_lookup(infile, outfile)
 
 
+# ----------- Ring stats
+def get_spiro_atoms(mol):
+    """Get atoms that are part of a spiro fusion
+
+    :param mol: input RDKit molecule
+    :return: a list of atom numbers for atoms that are the centers of spiro fusions
+    """
+    info = mol.GetRingInfo()
+    ring_sets = [set(x) for x in info.AtomRings()]
+    spiro_atoms = []
+    for i, j in itertools.combinations(ring_sets, 2):
+        i_and_j = (i.intersection(j))
+        if len(i_and_j) == 1:
+            spiro_atoms += list(i_and_j)
+    return spiro_atoms
+
+
+def max_ring_size(mol):
+    """Get the size of the largest ring in a molecule
+
+    :param mol: input_molecule
+    :return: size of the largest ring or 0 for an acyclic molecule
+    """
+    ri = mol.GetRingInfo()
+    atom_rings = ri.AtomRings()
+    if len(atom_rings) == 0:
+        return 0
+    else:
+        return max([len(x) for x in ri.AtomRings()])
+
+
+def ring_stats(mol):
+    """Get some simple statistics for rings
+
+    :param mol: RDKit molecule
+    :return: number of rings, maximum ring size
+    """
+    max_size = max_ring_size(mol)
+    num_rings = CalcNumRings(mol)
+    return num_rings, max_size
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `useful_rdkit_utils-0.3.8/useful_rdkit_utils/data/ring_systems/chembl_ring_systems.parquet` & `useful_rdkit_utils-0.5/useful_rdkit_utils/data/ring_systems/chembl_ring_systems.parquet`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/.gitignore` & `useful_rdkit_utils-0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/LICENSE` & `useful_rdkit_utils-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `useful_rdkit_utils-0.3.8/README.md` & `useful_rdkit_utils-0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,21 +27,21 @@
 
 
 
 ### Demos
 The notebooks directory contains Jupyter notebooks that show how to use some of the functions in this collection.
 
 ### Contributing
-I'm very open to PRs with corrections and/or contributions. 
+I'm very open to PRs with corrections and/or contributions.
 
 ### Copyright
 
-Copyright (c) 2021, Pat Walters
+Copyright (c) 2021-2024, Pat Walters
 
 ### License
 
 The code in this package is licensed under the MIT License.
 
 ### Acknowledgements
- 
-Project based on the 
+
+Project based on the
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.6.
```

### Comparing `useful_rdkit_utils-0.3.8/pyproject.toml` & `useful_rdkit_utils-0.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="useful_rdkit_utils"
-version = "0.3.8"
+dynamic=["version"]
 authors = [
   { name="Pat Walters", email="wpwalters@gmail.com" },
 ]
 description = "A collection of useful RDKit functions"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
      'numpy',	
      'rdkit',
      'pandas',
      'pystow',
+     'pyarrow',
+     'seaborn',
+     'scipy',
+     'tqdm',
+     'scikit-learn',
+     'dataclasses',
+     'py3dmol',
+     'click'
 ]
 
+[tool.hatch.version]
+path = "useful_rdkit_utils/__init__.py"
+
+[project.optional-dependencies]
+tests = ['pytest']
+viz = ['py3DMol', 'seaborn']
+cli = ['click']
+
 [project.urls]
 "Homepage" = "https://github.com/PatWalters/useful_rdkit_utils"
 "Bug Tracker" = "https://github.com/PatWalters/useful_rdkit_utils/issues"
```

### Comparing `useful_rdkit_utils-0.3.8/PKG-INFO` & `useful_rdkit_utils-0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,38 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: useful_rdkit_utils
-Version: 0.3.8
+Version: 0.5
 Summary: A collection of useful RDKit functions
 Project-URL: Homepage, https://github.com/PatWalters/useful_rdkit_utils
 Project-URL: Bug Tracker, https://github.com/PatWalters/useful_rdkit_utils/issues
 Author-email: Pat Walters <wpwalters@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.11
+Requires-Dist: click
+Requires-Dist: dataclasses
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: py3dmol
+Requires-Dist: pyarrow
 Requires-Dist: pystow
 Requires-Dist: rdkit
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: seaborn
+Requires-Dist: tqdm
+Provides-Extra: cli
+Requires-Dist: click; extra == 'cli'
+Provides-Extra: tests
+Requires-Dist: pytest; extra == 'tests'
+Provides-Extra: viz
+Requires-Dist: py3dmol; extra == 'viz'
+Requires-Dist: seaborn; extra == 'viz'
 Description-Content-Type: text/markdown
 
 useful_rdkit_utils
 ==============================
 [//]: # (Badges)
 [![GitHub Actions Build Status](https://github.com/PatWalters/useful_rdkit_utils/workflows/CI/badge.svg)](https://github.com/PatWalters/useful_rdkit_utils/actions?query=workflow%3ACI)
 
@@ -45,21 +60,21 @@
 
 
 
 ### Demos
 The notebooks directory contains Jupyter notebooks that show how to use some of the functions in this collection.
 
 ### Contributing
-I'm very open to PRs with corrections and/or contributions. 
+I'm very open to PRs with corrections and/or contributions.
 
 ### Copyright
 
-Copyright (c) 2021, Pat Walters
+Copyright (c) 2021-2024, Pat Walters
 
 ### License
 
 The code in this package is licensed under the MIT License.
 
 ### Acknowledgements
- 
-Project based on the 
+
+Project based on the
 [Computational Molecular Science Python Cookiecutter](https://github.com/molssi/cookiecutter-cms) version 1.6.
```

