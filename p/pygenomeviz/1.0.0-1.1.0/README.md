# Comparing `tmp/pygenomeviz-1.0.0.tar.gz` & `tmp/pygenomeviz-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenomeviz-1.0.0.tar", max compression
+gzip compressed data, was "pygenomeviz-1.1.0.tar", max compression
```

## Comparing `pygenomeviz-1.0.0.tar` & `pygenomeviz-1.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1062 2024-05-18 14:46:39.493759 pygenomeviz-1.0.0/LICENSE
--rw-r--r--   0        0        0    16412 2024-05-18 14:46:39.493759 pygenomeviz-1.0.0/README.md
--rw-r--r--   0        0        0     2525 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      614 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/__init__.py
--rw-r--r--   0        0        0      281 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/align/__init__.py
--rw-r--r--   0        0        0    13548 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/align/coord.py
--rw-r--r--   0        0        0      359 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/align/tool/__init__.py
--rw-r--r--   0        0        0     6227 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/align/tool/base.py
--rw-r--r--   0        0        0     5207 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/align/tool/blast.py
--rw-r--r--   0        0        0     5880 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/align/tool/mmseqs.py
--rw-r--r--   0        0        0     6130 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/align/tool/mummer.py
--rw-r--r--   0        0        0     4474 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/align/tool/pmauve.py
--rw-r--r--   0        0        0      334 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/exception.py
--rw-r--r--   0        0        0    26494 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/genomeviz.py
--rw-r--r--   0        0        0        0 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/gui/__init__.py
--rw-r--r--   0        0        0    16101 2024-05-18 14:46:39.613759 pygenomeviz-1.0.0/src/pygenomeviz/gui/app.py
--rw-r--r--   0        0        0  1422986 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/gui/assets/pgv_demo.gif
--rw-r--r--   0        0        0     1950 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/gui/config.py
--rw-r--r--   0        0        0     5508 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/gui/plot.py
--rw-r--r--   0        0        0     3551 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/gui/utils.py
--rw-r--r--   0        0        0     1687 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/logger.py
--rw-r--r--   0        0        0      127 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/parser/__init__.py
--rw-r--r--   0        0        0    15471 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/parser/genbank.py
--rw-r--r--   0        0        0    17012 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/parser/gff.py
--rw-r--r--   0        0        0    11554 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/patches.py
--rw-r--r--   0        0        0    15745 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/scripts/__init__.py
--rw-r--r--   0        0        0     6819 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/scripts/blast.py
--rw-r--r--   0        0        0     2856 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/scripts/download.py
--rw-r--r--   0        0        0     2566 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/scripts/gui.py
--rw-r--r--   0        0        0     6758 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/scripts/mmseqs.py
--rw-r--r--   0        0        0     6775 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/scripts/mummer.py
--rw-r--r--   0        0        0     5212 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/scripts/pmauve.py
--rw-r--r--   0        0        0       92 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/segment/__init__.py
--rw-r--r--   0        0        0    24508 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/segment/feature.py
--rw-r--r--   0        0        0      242 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/track/__init__.py
--rw-r--r--   0        0        0     3351 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/track/base.py
--rw-r--r--   0        0        0    31433 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/track/feature.py
--rw-r--r--   0        0        0     6766 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/track/link.py
--rw-r--r--   0        0        0      901 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/typing.py
--rw-r--r--   0        0        0      487 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/utils/__init__.py
--rw-r--r--   0        0        0     6360 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/utils/download.py
--rw-r--r--   0        0        0     6061 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/utils/helper.py
--rw-r--r--   0        0        0     1124 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/utils/plot.py
--rw-r--r--   0        0        0     2319 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/__init__.py
--rw-r--r--   0        0        0     7090 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     7074 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4618 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     7111 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4618 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6487 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    32146 2024-05-18 14:46:39.621759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.css
--rw-r--r--   0        0        0   254963 2024-05-18 14:46:39.625759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.js
--rw-r--r--   0        0        0    87533 2024-05-18 14:46:39.625759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/jquery.min.js
--rw-r--r--   0        0        0    10026 2024-05-18 14:46:39.625759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/panzoom.min.js
--rw-r--r--   0        0        0    10465 2024-05-18 14:46:39.625759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.css
--rw-r--r--   0        0        0    27904 2024-05-18 14:46:39.625759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.js
--rw-r--r--   0        0        0     6584 2024-05-18 14:46:39.625759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/pgv-viewer.js
--rw-r--r--   0        0        0    13512 2024-05-18 14:46:39.625759 pygenomeviz-1.0.0/src/pygenomeviz/viewer/pgv-viewer-template.html
--rw-r--r--   0        0        0    17598 1970-01-01 00:00:00.000000 pygenomeviz-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-26 07:26:55.386359 pygenomeviz-1.1.0/LICENSE
+-rw-r--r--   0        0        0    16604 2024-05-26 07:26:55.386359 pygenomeviz-1.1.0/README.md
+-rw-r--r--   0        0        0     2525 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      614 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/__init__.py
+-rw-r--r--   0        0        0      281 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/align/__init__.py
+-rw-r--r--   0        0        0    13548 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/align/coord.py
+-rw-r--r--   0        0        0      359 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/align/tool/__init__.py
+-rw-r--r--   0        0        0     6290 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/align/tool/base.py
+-rw-r--r--   0        0        0     5207 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/align/tool/blast.py
+-rw-r--r--   0        0        0     5880 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/align/tool/mmseqs.py
+-rw-r--r--   0        0        0     6130 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/align/tool/mummer.py
+-rw-r--r--   0        0        0     4474 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/align/tool/pmauve.py
+-rw-r--r--   0        0        0      334 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/exception.py
+-rw-r--r--   0        0        0    26760 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/genomeviz.py
+-rw-r--r--   0        0        0        0 2024-05-26 07:26:55.526359 pygenomeviz-1.1.0/src/pygenomeviz/gui/__init__.py
+-rw-r--r--   0        0        0    16606 2024-05-26 07:26:55.530359 pygenomeviz-1.1.0/src/pygenomeviz/gui/app.py
+-rw-r--r--   0        0        0  1422986 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/gui/assets/pgv_demo.gif
+-rw-r--r--   0        0        0     1950 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/gui/config.py
+-rw-r--r--   0        0        0     5534 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/gui/plot.py
+-rw-r--r--   0        0        0     3551 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/gui/utils.py
+-rw-r--r--   0        0        0     1687 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/logger.py
+-rw-r--r--   0        0        0      127 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/parser/__init__.py
+-rw-r--r--   0        0        0    15497 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/parser/genbank.py
+-rw-r--r--   0        0        0    17202 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/parser/gff.py
+-rw-r--r--   0        0        0    11554 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/patches.py
+-rw-r--r--   0        0        0    15745 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/scripts/__init__.py
+-rw-r--r--   0        0        0     6819 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/scripts/blast.py
+-rw-r--r--   0        0        0     2856 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/scripts/download.py
+-rw-r--r--   0        0        0     2566 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/scripts/gui.py
+-rw-r--r--   0        0        0     6758 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/scripts/mmseqs.py
+-rw-r--r--   0        0        0     6775 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/scripts/mummer.py
+-rw-r--r--   0        0        0     5212 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/scripts/pmauve.py
+-rw-r--r--   0        0        0       92 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/segment/__init__.py
+-rw-r--r--   0        0        0    24508 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/segment/feature.py
+-rw-r--r--   0        0        0      242 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/track/__init__.py
+-rw-r--r--   0        0        0     3351 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/track/base.py
+-rw-r--r--   0        0        0    31454 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/track/feature.py
+-rw-r--r--   0        0        0     6766 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/track/link.py
+-rw-r--r--   0        0        0      901 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/typing.py
+-rw-r--r--   0        0        0      487 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/utils/__init__.py
+-rw-r--r--   0        0        0     6364 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/utils/download.py
+-rw-r--r--   0        0        0     6061 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/utils/helper.py
+-rw-r--r--   0        0        0     1124 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/utils/plot.py
+-rw-r--r--   0        0        0     2319 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/__init__.py
+-rw-r--r--   0        0        0     7090 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     7074 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4618 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     7111 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4618 2024-05-26 07:26:55.534359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6487 2024-05-26 07:26:55.538359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    32146 2024-05-26 07:26:55.538359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.css
+-rw-r--r--   0        0        0   254963 2024-05-26 07:26:55.538359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.js
+-rw-r--r--   0        0        0    87533 2024-05-26 07:26:55.538359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/jquery.min.js
+-rw-r--r--   0        0        0    10026 2024-05-26 07:26:55.538359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/panzoom.min.js
+-rw-r--r--   0        0        0    10465 2024-05-26 07:26:55.538359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.css
+-rw-r--r--   0        0        0    27904 2024-05-26 07:26:55.538359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.js
+-rw-r--r--   0        0        0     6584 2024-05-26 07:26:55.538359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/pgv-viewer.js
+-rw-r--r--   0        0        0    13512 2024-05-26 07:26:55.538359 pygenomeviz-1.1.0/src/pygenomeviz/viewer/pgv-viewer-template.html
+-rw-r--r--   0        0        0    17790 1970-01-01 00:00:00.000000 pygenomeviz-1.1.0/PKG-INFO
```

### Comparing `pygenomeviz-1.0.0/LICENSE` & `pygenomeviz-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/README.md` & `pygenomeviz-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # pyGenomeViz
 
 ![Python3](https://img.shields.io/badge/Language-Python3-steelblue)
 ![OS](https://img.shields.io/badge/OS-_Windows_|_Mac_|_Linux-steelblue)
 ![License](https://img.shields.io/badge/License-MIT-steelblue)
 [![Latest PyPI version](https://img.shields.io/pypi/v/pygenomeviz.svg)](https://pypi.python.org/pypi/pygenomeviz)
-[![Bioconda](https://img.shields.io/conda/vn/bioconda/pygenomeviz.svg?color=green)](https://anaconda.org/bioconda/pygenomeviz)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/pygenomeviz.svg?color=green)](https://anaconda.org/conda-forge/pygenomeviz)
 [![CI](https://github.com/moshi4/pyGenomeViz/actions/workflows/ci.yml/badge.svg)](https://github.com/moshi4/pyGenomeViz/actions/workflows/ci.yml)
 
 > [!NOTE]
 > A major version upgrade, pyGenomeViz **v1.0.0**, was released on 2024/05.
 > Backward incompatible changes have been made between v1.0.0 and v0.X.X to make for a more sophisticated API/CLI design.
-> Therefore, v0.X.X users should be careful.
+> Therefore, v0.X.X users should pin the version to v0.4.4 or update existing code for v1.0.0.
+> Previous v0.4.4 documentation is available [here](https://moshi4.github.io/docs/pygenomeviz/v0.4.4/).
 
 ## Table of contents
 
 - [Overview](#overview)
 - [Installation](#installation)
 - [API Examples](#api-examples)
 - [CLI Examples](#cli-examples)
@@ -45,25 +46,25 @@
 
 `Python 3.8 or later` is required for installation.
 
 **Install PyPI package:**
 
     pip install pygenomeviz
 
-**Install bioconda package:**
+**Install conda-forge package:**
 
-    conda install -c conda-forge -c bioconda pygenomeviz
+    conda install -c conda-forge pygenomeviz
 
 **Use Docker ([Image Registry](https://github.com/moshi4/pyGenomeViz/pkgs/container/pygenomeviz)):**
 
     docker run -it --rm -p 8501:8501 ghcr.io/moshi4/pygenomeviz:latest pgv-gui -h
 
 ## API Examples
 
-Jupyter notebooks containing code examples below is available [here](https://moshi4.github.io/pyGenomeViz/getting_started/).
+Jupyter notebooks containing code examples below is available [here](https://github.com/moshi4/pyGenomeViz/blob/main/notebooks/example.ipynb).
 
 ### Features
 
 ```python
 from pygenomeviz import GenomeViz
 
 gv = GenomeViz()
@@ -184,15 +185,15 @@
 track.add_features(features)
 
 gv.savefig("genbank_features.png")
 ```
 
 ![genbank_features.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example/genbank_features.png)
 
-### GFF Range Features
+### GFF Features
 
 ```python
 from pygenomeviz import GenomeViz
 from pygenomeviz.parser import Gff
 from pygenomeviz.utils import load_example_gff_file
 
 gff_file = load_example_gff_file("escherichia_coli.gff.gz")
@@ -233,17 +234,17 @@
 gv.set_scale_xticks(labelsize=10)
 
 # Plot CDS, rRNA features for each contig to tracks
 for seqid, size in gff.get_seqid2size().items():
     track = gv.add_feature_track(seqid, size, labelsize=15)
     track.add_sublabel(size=10, color="grey")
     cds_features = gff.get_seqid2features(feature_type="CDS")[seqid]
-    # CDS: blue, CDS(pseudo): lightgrey
+    # CDS: blue, CDS(pseudo): grey
     for cds_feature in cds_features:
-        color = "lightgrey" if is_pseudo_feature(cds_feature) else "blue"
+        color = "grey" if is_pseudo_feature(cds_feature) else "blue"
         track.add_features(cds_feature, color=color)
     # rRNA: lime
     rrna_features = gff.get_seqid2features(feature_type="rRNA")[seqid]
     track.add_features(rrna_features, color="lime")
 
 gv.savefig("gff_contigs.png")
 ```
@@ -286,15 +287,16 @@
 gv.savefig("genbank_comparison_by_blast.png")
 ```
 
 ![genbank_comparison_by_blast.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example/genbank_comparison_by_blast.png)
 
 ## CLI Examples
 
-pyGenomeViz provides CLI workflow for visualization of genome alignment results using `BLAST`/`MUMmer`/`MMseqs`/`progressiveMauve`.
+pyGenomeViz provides CLI workflows for genome alignment result visualization of
+Genbank genomes using `BLAST` / `MUMmer` / `MMseqs` / `progressiveMauve`, respectively.
 
 ### BLAST CLI Workflow
 
 See [pgv-blast document](https://moshi4.github.io/pyGenomeViz/cli-docs/pgv-blast/) for details.
 
 ```shell
 # Download example dataset
```

### Comparing `pygenomeviz-1.0.0/pyproject.toml` & `pygenomeviz-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygenomeviz"
-version = "1.0.0"
+version = "1.1.0"
 description = "A genome visualization python package for comparative genomics"
 authors = ["moshi4"]
 license = "MIT"
 homepage = "https://moshi4.github.io/pyGenomeViz/"
 repository = "https://github.com/moshi4/pyGenomeViz/"
 readme = "README.md"
 keywords = [
```

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/align/coord.py` & `pygenomeviz-1.1.0/src/pygenomeviz/align/coord.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/align/tool/base.py` & `pygenomeviz-1.1.0/src/pygenomeviz/align/tool/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import logging
 import os
 import shlex
 import shutil
 import subprocess as sp
-import sys
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Sequence
 
 from pygenomeviz.align import AlignCoord
 from pygenomeviz.logger import get_logger
 from pygenomeviz.parser import Genbank
@@ -117,21 +116,21 @@
         else:
             logger.error("Failed to run command below!!")
             logger.error(f"$ {cmd}")
             stdout_lines = cmd_res.stdout.splitlines()
             if len(stdout_lines) > 0:
                 logger.error("STDOUT:")
                 for line in stdout_lines:
-                    logger.error(line)
+                    logger.error(f"> {line}")
             stderr_lines = cmd_res.stderr.splitlines()
             if len(stderr_lines) > 0:
                 logger.error("STDERR:")
                 for line in stderr_lines:
-                    logger.error(line)
-            sys.exit(1)
+                    logger.error(f"> {line}")
+            raise RuntimeError(f"Failed to run '{self.get_tool_name()}' aligner!!")
 
     def _parse_input_gbk_seqs(
         self, seqs: Sequence[str | Path | Genbank]
     ) -> list[Genbank]:
         """Parse input genbank sequences
 
         Parameters
```

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/align/tool/blast.py` & `pygenomeviz-1.1.0/src/pygenomeviz/align/tool/blast.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/align/tool/mmseqs.py` & `pygenomeviz-1.1.0/src/pygenomeviz/align/tool/mmseqs.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/align/tool/mummer.py` & `pygenomeviz-1.1.0/src/pygenomeviz/align/tool/mummer.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/align/tool/pmauve.py` & `pygenomeviz-1.1.0/src/pygenomeviz/align/tool/pmauve.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/genomeviz.py` & `pygenomeviz-1.1.0/src/pygenomeviz/genomeviz.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,14 +546,19 @@
         ----------
         savefile : str | Path
             Save file
         dpi : int, optional
             DPI
         pad_inches : float, optional
             Padding inches
+
+        Warnings
+        --------
+        To plot a figure that settings a user-defined legend, subtracks, or annotations,
+        call `fig.savefig()` instead of `gv.savefig()`.
         """
         fig = self.plotfig(dpi=dpi)
         fig.savefig(
             fname=str(savefile),
             dpi=dpi,
             pad_inches=pad_inches,
             bbox_inches="tight",
@@ -571,15 +576,16 @@
         """Save figure in html format
 
         Parameters
         ----------
         html_outfile : str | Path | StringIO | BytesIO
             Output HTML file (*.html)
         figure : Figure | None, optional
-            If Figure set, plot html viewer using user customized figure
+            If Figure is set, plot html viewer using user customized figure.
+            Set to output figure including user-specified legend, subtracks, etc.
         """
         # Load SVG contents
         fig = self.plotfig(fast_render=False) if figure is None else figure
         svg_fig_bytes = io.BytesIO()
         fig.savefig(fname=svg_fig_bytes, format="svg")
         svg_fig_bytes.seek(0)
         svg_fig_contents = svg_fig_bytes.read().decode("utf-8")
```

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/gui/app.py` & `pygenomeviz-1.1.0/src/pygenomeviz/gui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,27 +385,27 @@
 expand_figure = st.checkbox(label="Expand Figure", value=False)
 fig_container = st.container()
 fig_ctl_container = st.container()
 genome_info_container = st.container()
 
 with genome_info_container.form(key="form"):
     title_col, form_col = st.columns([4, 1])
-    title_col.markdown("**Genome Min-Max Range Option**")
+    title_col.markdown("**Genome Min-Max Range & Reverse Option**")
     form_col.form_submit_button(
         label="Update Figure",
-        help="Apply min-max range option changes to figure",
+        help="Apply min-max range & reverse option changes to figure",
     )
 
     name2seqid2range: dict[str, dict[str, tuple[int, int]]] = {}
     for gbk in gbk_list:
         expander_label = f"**{gbk.name} ({len(gbk.records)} records)**"
         with st.expander(expander_label, expanded=False):
             seqid2range = {}
             seqid2features = gbk.get_seqid2features(None)
-            for seqid, size in gbk.get_seqid2size().items():
+            for idx, (seqid, size) in enumerate(gbk.get_seqid2size().items()):
                 range_cols = st.columns([3, 3, 1])
                 min_range = range_cols[0].number_input(
                     label=f"**{seqid}** ({size:,} bp)",
                     min_value=0,
                     max_value=size,
                     value=0,
                     step=1,
@@ -423,17 +423,27 @@
                     label_visibility="hidden",
                     key=f"{gbk.name} {seqid} end",
                 )
                 max_range = int(max_range)
                 if min_range > max_range:
                     st.error(f"**{max_range=}** must be larger than **{min_range=}**")
                     st.stop()
-                if min_range == max_range:
-                    continue
-                seqid2range[seqid] = (min_range, max_range)
+                if min_range != max_range:
+                    seqid2range[seqid] = (min_range, max_range)
+                reverse = range_cols[2].selectbox(
+                    label="Reverse",
+                    options=[True, False],
+                    index=1,
+                    format_func=lambda b: "Yes" if b else "No",
+                    key=f"{gbk.name} {seqid} reverse",
+                )
+                if reverse is True:
+                    gbk.records[idx] = gbk.records[idx].reverse_complement(
+                        id=True, name=True, description=True
+                    )
             name2seqid2range[gbk.name] = seqid2range
 
 
 fig_ctl_cols = fig_ctl_container.columns([1, 2, 3])
 
 # Plot figure
 gv, align_coords = plot.plot_by_gui_cfg(
```

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/gui/assets/pgv_demo.gif` & `pygenomeviz-1.1.0/src/pygenomeviz/gui/assets/pgv_demo.gif`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/gui/config.py` & `pygenomeviz-1.1.0/src/pygenomeviz/gui/config.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/gui/plot.py` & `pygenomeviz-1.1.0/src/pygenomeviz/gui/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,18 @@
     gbk_list : list[Genbank]
         Genbank list
     cfg : PgvConfig
         Config
 
     Returns
     -------
-    gv, align_coords : tuple[GenomeViz, list[AlignCoord]]
-        GenomeViz instance, AlignCoord list
+    gv : GenomeViz
+        GenomeViz instance
+    align_coords : list[AlignCoord]
+        AlignCoord list
     """
     # Create genomeviz instance
     gv = GenomeViz(
         fig_width=cfg.fig.width,
         fig_track_height=cfg.fig.track_height,
         track_align_type=cfg.fig.track_align_type,  # type: ignore
         feature_track_ratio=cfg.fig.feature_track_ratio,
@@ -88,16 +90,16 @@
     # Create processig cache directory
     package_name = __name__.split(".")[0]
     gui_cache_dir = Path.home() / ".cache" / package_name / "gui"
     os.makedirs(gui_cache_dir, exist_ok=True)
     utils.remove_old_files(gui_cache_dir)
 
     # Create md5 hash unique filename to enable cache alignment result
-    md5_hash_source = "\n".join([str(gbk) for gbk in gbk_list]).encode()
-    md5_hash_value = hashlib.md5(md5_hash_source).hexdigest()
+    md5_hash_source = "\n".join([f"{gbk} {gbk.full_genome_seq}" for gbk in gbk_list])
+    md5_hash_value = hashlib.md5(md5_hash_source.encode()).hexdigest()
     aln_coords_filename = f"{md5_hash_value}_{cfg.aln.method}.tsv"
     aln_coords_file = gui_cache_dir / aln_coords_filename.replace(" ", "")
 
     # Genome alignment
     if aln_coords_file.exists():
         align_coords = AlignCoord.read(aln_coords_file)
     else:
```

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/gui/utils.py` & `pygenomeviz-1.1.0/src/pygenomeviz/gui/utils.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/logger.py` & `pygenomeviz-1.1.0/src/pygenomeviz/logger.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/parser/genbank.py` & `pygenomeviz-1.1.0/src/pygenomeviz/parser/genbank.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,16 +129,18 @@
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
         seq : str | None, optional
             Sequence for GCskew calculation (Default: `self.genome_seq`)
 
         Returns
         -------
-        gc_skew_result_tuple : tuple[NDArray[np.int64], NDArray[np.float64]]
-            Position list & GC skew list
+        pos_list : NDArray[np.int64]
+            Position list
+        gc_skew_list : NDArray[np.float64]
+            GC skew list
         """
         pos_list, gc_skew_list = [], []
         seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
             step_size = int(len(seq) / 1000)
@@ -181,16 +183,18 @@
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
         seq : str | None, optional
             Sequence for GC content calculation (Default: `self.genome_seq`)
 
         Returns
         -------
-        gc_content_result_tuple : tuple[NDArray[np.int64], NDArray[np.float64]]
-            Position list & GC content list
+        pos_list : NDArray[np.int64]
+            Position list
+        gc_content_list : NDArray[np.float64]
+            GC content list
         """
         pos_list, gc_content_list = [], []
         seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
             step_size = int(len(seq) / 1000)
```

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/parser/gff.py` & `pygenomeviz-1.1.0/src/pygenomeviz/parser/gff.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,16 +255,20 @@
         gff_file : str | Path
             GFF file
         target_seqid : str | None
             Target seqid to be extracted
 
         Returns
         -------
-        gff_records, start, end : tuple[list[GffRecord], int, int]
-            GFF record list, start, end
+        gff_records : list[GffRecord]
+            GFF record list
+        start : int
+            Start position of target_seqid record
+        end : int
+            End position of target_seqid record
         """
         gff_file = Path(gff_file)
         if gff_file.suffix == ".gz":
             with gzip.open(gff_file, mode="rt") as f:
                 gff_records, start, end = self._parse_gff_textio(f, target_seqid)
         elif gff_file.suffix == ".bz2":
             with bz2.open(gff_file, mode="rt") as f:
@@ -292,16 +296,20 @@
         handle : TextIO
             GFF TextIO handle
         target_seqid : str | None, optional
             GFF target seqid
 
         Returns
         -------
-        gff_records, start, end : tuple[list[GffRecord], int, int]
-            GFF record list, start, end
+        gff_records : list[GffRecord]
+            GFF record list
+        start : int
+            Start position of target_seqid record
+        end : int
+            End position of target_seqid record
         """
         # Parse GFF lines
         gff_all_lines = handle.read().splitlines()
         gff_record_lines = filter(GffRecord.is_gff_line, gff_all_lines)
         gff_records = list(map(GffRecord.parse_gff_line, gff_record_lines))
         if len(gff_records) == 0:
             err_msg = f"Failed to parse '{self._gff_file}' as GFF file "
```

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/patches.py` & `pygenomeviz-1.1.0/src/pygenomeviz/patches.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/scripts/__init__.py` & `pygenomeviz-1.1.0/src/pygenomeviz/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/scripts/blast.py` & `pygenomeviz-1.1.0/src/pygenomeviz/scripts/blast.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/scripts/download.py` & `pygenomeviz-1.1.0/src/pygenomeviz/scripts/download.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/scripts/gui.py` & `pygenomeviz-1.1.0/src/pygenomeviz/scripts/gui.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/scripts/mmseqs.py` & `pygenomeviz-1.1.0/src/pygenomeviz/scripts/mmseqs.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/scripts/mummer.py` & `pygenomeviz-1.1.0/src/pygenomeviz/scripts/mummer.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/scripts/pmauve.py` & `pygenomeviz-1.1.0/src/pygenomeviz/scripts/pmauve.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/segment/feature.py` & `pygenomeviz-1.1.0/src/pygenomeviz/segment/feature.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/track/base.py` & `pygenomeviz-1.1.0/src/pygenomeviz/track/base.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/track/feature.py` & `pygenomeviz-1.1.0/src/pygenomeviz/track/feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -829,16 +829,18 @@
         Parameters
         ----------
         feature : SeqFeature
             Exon Feature
 
         Returns
         -------
-        exon_locs, intron_locs : tuple[list[tuple[int, int]], list[tuple[int, int]]]
-            Exon & intron locations
+        exon_locs : list[tuple[int, int]]
+            Exon locations
+        intron_locs : list[tuple[int, int]]
+            Intron locations
         """
         exon_locs: list[tuple[int, int]] = []
         intron_locs: list[tuple[int, int]] = []
         # Extract exon locations
         for loc in feature.location.parts:
             exon_start, exon_end = int(loc.start), int(loc.end)  # type: ignore
             exon_locs.append((exon_start, exon_end))
```

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/track/link.py` & `pygenomeviz-1.1.0/src/pygenomeviz/track/link.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/typing.py` & `pygenomeviz-1.1.0/src/pygenomeviz/typing.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/utils/download.py` & `pygenomeviz-1.1.0/src/pygenomeviz/utils/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     *,
     cache_dir: str | Path | None = None,
     overwrite_cache: bool = False,
     quiet: bool = True,
 ) -> list[Path]:
     """Load pygenomeviz example genbank dataset
 
-    Load genbank datasets from https://github.com/moshi4/pygenomeviz-data-v1
+    Load genbank datasets from <https://github.com/moshi4/pygenomeviz-data-v1>
     and cache datasets in local directory (Default: `~/.cache/pygenomeviz/`).
 
     List of dataset name
 
     - `acinetobacter_phage` (4 species)
     - `yersinia_phage` (4 species)
     - `enterobacteria_phage` (6 species)
@@ -133,15 +133,15 @@
     filename: GffExampleFileName,
     *,
     cache_dir: str | Path | None = None,
     overwrite_cache: bool = False,
 ) -> Path:
     """Load pygenomeviz example GFF file
 
-    Load example GFF file from https://github.com/moshi4/pygenomeviz-data-v1/
+    Load example GFF file from <https://github.com/moshi4/pygenomeviz-data-v1/>
     and cache GFF file in local directory (Default: `~/.cache/pygenomeviz/`).
 
     List of example GFF filename
 
     - `enterobacteria_phage.gff`
     - `mycoplasma_mycoides.gff`
     - `escherichia_coli.gff.gz`
```

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/utils/helper.py` & `pygenomeviz-1.1.0/src/pygenomeviz/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/utils/plot.py` & `pygenomeviz-1.1.0/src/pygenomeviz/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/__init__.py` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_444444_256x240.png` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_555555_256x240.png` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777620_256x240.png` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777777_256x240.png` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_cc0000_256x240.png` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_ffffff_256x240.png` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.css` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.js` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/jquery.min.js` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/panzoom.min.js` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/panzoom.min.js`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.css` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.css`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.js` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.js`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/assets/pgv-viewer.js` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/assets/pgv-viewer.js`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/src/pygenomeviz/viewer/pgv-viewer-template.html` & `pygenomeviz-1.1.0/src/pygenomeviz/viewer/pgv-viewer-template.html`

 * *Files identical despite different names*

### Comparing `pygenomeviz-1.0.0/PKG-INFO` & `pygenomeviz-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenomeviz
-Version: 1.0.0
+Version: 1.1.0
 Summary: A genome visualization python package for comparative genomics
 Home-page: https://moshi4.github.io/pyGenomeViz/
 License: MIT
 Keywords: bioinformatics,genomics,matplotlib,visualization,comparative-genomics
 Author: moshi4
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Matplotlib
@@ -27,21 +27,22 @@
 
 # pyGenomeViz
 
 ![Python3](https://img.shields.io/badge/Language-Python3-steelblue)
 ![OS](https://img.shields.io/badge/OS-_Windows_|_Mac_|_Linux-steelblue)
 ![License](https://img.shields.io/badge/License-MIT-steelblue)
 [![Latest PyPI version](https://img.shields.io/pypi/v/pygenomeviz.svg)](https://pypi.python.org/pypi/pygenomeviz)
-[![Bioconda](https://img.shields.io/conda/vn/bioconda/pygenomeviz.svg?color=green)](https://anaconda.org/bioconda/pygenomeviz)
+[![conda-forge](https://img.shields.io/conda/vn/conda-forge/pygenomeviz.svg?color=green)](https://anaconda.org/conda-forge/pygenomeviz)
 [![CI](https://github.com/moshi4/pyGenomeViz/actions/workflows/ci.yml/badge.svg)](https://github.com/moshi4/pyGenomeViz/actions/workflows/ci.yml)
 
 > [!NOTE]
 > A major version upgrade, pyGenomeViz **v1.0.0**, was released on 2024/05.
 > Backward incompatible changes have been made between v1.0.0 and v0.X.X to make for a more sophisticated API/CLI design.
-> Therefore, v0.X.X users should be careful.
+> Therefore, v0.X.X users should pin the version to v0.4.4 or update existing code for v1.0.0.
+> Previous v0.4.4 documentation is available [here](https://moshi4.github.io/docs/pygenomeviz/v0.4.4/).
 
 ## Table of contents
 
 - [Overview](#overview)
 - [Installation](#installation)
 - [API Examples](#api-examples)
 - [CLI Examples](#cli-examples)
@@ -72,25 +73,25 @@
 
 `Python 3.8 or later` is required for installation.
 
 **Install PyPI package:**
 
     pip install pygenomeviz
 
-**Install bioconda package:**
+**Install conda-forge package:**
 
-    conda install -c conda-forge -c bioconda pygenomeviz
+    conda install -c conda-forge pygenomeviz
 
 **Use Docker ([Image Registry](https://github.com/moshi4/pyGenomeViz/pkgs/container/pygenomeviz)):**
 
     docker run -it --rm -p 8501:8501 ghcr.io/moshi4/pygenomeviz:latest pgv-gui -h
 
 ## API Examples
 
-Jupyter notebooks containing code examples below is available [here](https://moshi4.github.io/pyGenomeViz/getting_started/).
+Jupyter notebooks containing code examples below is available [here](https://github.com/moshi4/pyGenomeViz/blob/main/notebooks/example.ipynb).
 
 ### Features
 
 ```python
 from pygenomeviz import GenomeViz
 
 gv = GenomeViz()
@@ -211,15 +212,15 @@
 track.add_features(features)
 
 gv.savefig("genbank_features.png")
 ```
 
 ![genbank_features.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example/genbank_features.png)
 
-### GFF Range Features
+### GFF Features
 
 ```python
 from pygenomeviz import GenomeViz
 from pygenomeviz.parser import Gff
 from pygenomeviz.utils import load_example_gff_file
 
 gff_file = load_example_gff_file("escherichia_coli.gff.gz")
@@ -260,17 +261,17 @@
 gv.set_scale_xticks(labelsize=10)
 
 # Plot CDS, rRNA features for each contig to tracks
 for seqid, size in gff.get_seqid2size().items():
     track = gv.add_feature_track(seqid, size, labelsize=15)
     track.add_sublabel(size=10, color="grey")
     cds_features = gff.get_seqid2features(feature_type="CDS")[seqid]
-    # CDS: blue, CDS(pseudo): lightgrey
+    # CDS: blue, CDS(pseudo): grey
     for cds_feature in cds_features:
-        color = "lightgrey" if is_pseudo_feature(cds_feature) else "blue"
+        color = "grey" if is_pseudo_feature(cds_feature) else "blue"
         track.add_features(cds_feature, color=color)
     # rRNA: lime
     rrna_features = gff.get_seqid2features(feature_type="rRNA")[seqid]
     track.add_features(rrna_features, color="lime")
 
 gv.savefig("gff_contigs.png")
 ```
@@ -313,15 +314,16 @@
 gv.savefig("genbank_comparison_by_blast.png")
 ```
 
 ![genbank_comparison_by_blast.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example/genbank_comparison_by_blast.png)
 
 ## CLI Examples
 
-pyGenomeViz provides CLI workflow for visualization of genome alignment results using `BLAST`/`MUMmer`/`MMseqs`/`progressiveMauve`.
+pyGenomeViz provides CLI workflows for genome alignment result visualization of
+Genbank genomes using `BLAST` / `MUMmer` / `MMseqs` / `progressiveMauve`, respectively.
 
 ### BLAST CLI Workflow
 
 See [pgv-blast document](https://moshi4.github.io/pyGenomeViz/cli-docs/pgv-blast/) for details.
 
 ```shell
 # Download example dataset
```

