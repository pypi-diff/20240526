# Comparing `tmp/finaletoolkit-0.5.2.tar.gz` & `tmp/finaletoolkit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finaletoolkit-0.5.2.tar", last modified: Wed May  8 20:05:46 2024, max compression
+gzip compressed data, was "finaletoolkit-0.6.0.tar", last modified: Sun May 26 21:37:41 2024, max compression
```

## Comparing `finaletoolkit-0.5.2.tar` & `finaletoolkit-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,46 @@
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1067 2024-03-29 01:22:35.000000 finaletoolkit-0.5.2/LICENSE
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6138 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3917 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/README.md
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1131 2024-05-08 20:05:10.000000 finaletoolkit-0.5.2/pyproject.toml
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       38 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/setup.cfg
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6138 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/PKG-INFO
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1190 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        1 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       61 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/entry_points.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      145 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/requires.txt
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       14 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/FinaleToolkit.egg-info/top_level.txt
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/finaletoolkit/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:45.000000 finaletoolkit-0.5.2/src/finaletoolkit/cli/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       40 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/cli/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    28006 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/cli/main_cli.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      547 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9703 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/adjust_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9331 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/cleavage_profile.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     7555 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/coverage.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14535 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3973 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi_gc_correct.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2587 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi_merge_bins.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    30313 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/end_motifs.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    14869 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/frag_length.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     8468 2024-05-08 20:04:27.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/multi_wps.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     6801 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/frag/wps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/genome/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)       39 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/genome/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    15108 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/genome/gaps.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/methylation/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/methylation/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/qc/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/qc/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/too/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/too/__init__.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)      139 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/__init__.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     4889 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/agg_bw.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     1649 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/cli_hist.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     3195 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/filter_bam.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)    18690 2024-05-08 20:04:28.000000 finaletoolkit-0.5.2/src/finaletoolkit/utils/utils.py
-drwxr-xr-x   0 jli18    (89033) mcb190124p (23920)        0 2024-05-08 20:05:46.000000 finaletoolkit-0.5.2/tests/
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     9859 2024-05-08 20:04:29.000000 finaletoolkit-0.5.2/tests/test_end_motifs.py
--rw-r--r--   0 jli18    (89033) mcb190124p (23920)     2128 2024-05-08 20:04:29.000000 finaletoolkit-0.5.2/tests/test_frag_io.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-26 21:37:41.303150 finaletoolkit-0.6.0/
+-rw-r--r--   0 jamesli    (501) staff       (20)     1067 2024-04-01 19:28:48.000000 finaletoolkit-0.6.0/LICENSE
+-rw-r--r--   0 jamesli    (501) staff       (20)     5047 2024-05-26 21:37:41.302939 finaletoolkit-0.6.0/PKG-INFO
+-rw-r--r--   0 jamesli    (501) staff       (20)     2965 2024-05-23 03:36:53.000000 finaletoolkit-0.6.0/README.md
+-rw-r--r--   0 jamesli    (501) staff       (20)     1032 2024-05-26 21:33:55.000000 finaletoolkit-0.6.0/pyproject.toml
+-rw-r--r--   0 jamesli    (501) staff       (20)       38 2024-05-26 21:37:41.303196 finaletoolkit-0.6.0/setup.cfg
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-26 21:37:41.294263 finaletoolkit-0.6.0/src/
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-26 21:37:41.302663 finaletoolkit-0.6.0/src/FinaleToolkit.egg-info/
+-rw-r--r--   0 jamesli    (501) staff       (20)     5047 2024-05-26 21:37:41.000000 finaletoolkit-0.6.0/src/FinaleToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 jamesli    (501) staff       (20)     1154 2024-05-26 21:37:41.000000 finaletoolkit-0.6.0/src/FinaleToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesli    (501) staff       (20)        1 2024-05-26 21:37:41.000000 finaletoolkit-0.6.0/src/FinaleToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesli    (501) staff       (20)       61 2024-05-26 21:37:41.000000 finaletoolkit-0.6.0/src/FinaleToolkit.egg-info/entry_points.txt
+-rw-r--r--   0 jamesli    (501) staff       (20)       81 2024-05-26 21:37:41.000000 finaletoolkit-0.6.0/src/FinaleToolkit.egg-info/requires.txt
+-rw-r--r--   0 jamesli    (501) staff       (20)       14 2024-05-26 21:37:41.000000 finaletoolkit-0.6.0/src/FinaleToolkit.egg-info/top_level.txt
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-26 21:37:41.296156 finaletoolkit-0.6.0/src/finaletoolkit/
+-rw-r--r--   0 jamesli    (501) staff       (20)        0 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/__init__.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-26 21:37:41.297077 finaletoolkit-0.6.0/src/finaletoolkit/cli/
+-rw-r--r--   0 jamesli    (501) staff       (20)       40 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/cli/__init__.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    21817 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/src/finaletoolkit/cli/main_cli.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-26 21:37:41.299963 finaletoolkit-0.6.0/src/finaletoolkit/frag/
+-rw-r--r--   0 jamesli    (501) staff       (20)      547 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/__init__.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     9719 2024-05-23 03:36:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/adjust_wps.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    10071 2024-05-23 03:36:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/cleavage_profile.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     9042 2024-05-23 03:36:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/coverage.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    14535 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/delfi.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     3973 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/delfi_gc_correct.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     2516 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/delfi_merge_bins.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    30236 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/end_motifs.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    14835 2024-05-26 21:27:44.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/frag_length.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     8468 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/multi_wps.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     6568 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/src/finaletoolkit/frag/wps.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-26 21:37:41.300341 finaletoolkit-0.6.0/src/finaletoolkit/genome/
+-rw-r--r--   0 jamesli    (501) staff       (20)       39 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/genome/__init__.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    15032 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/src/finaletoolkit/genome/gaps.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-26 21:37:41.301291 finaletoolkit-0.6.0/src/finaletoolkit/utils/
+-rw-r--r--   0 jamesli    (501) staff       (20)      139 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/utils/__init__.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     4889 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/utils/agg_bw.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     1649 2024-05-14 20:16:53.000000 finaletoolkit-0.6.0/src/finaletoolkit/utils/cli_hist.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     3119 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/src/finaletoolkit/utils/filter_bam.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    19501 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/src/finaletoolkit/utils/utils.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-26 21:37:41.302463 finaletoolkit-0.6.0/tests/
+-rw-r--r--   0 jamesli    (501) staff       (20)      742 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/tests/test_cleavage_profile.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     2324 2024-05-18 04:54:35.000000 finaletoolkit-0.6.0/tests/test_cli_entry.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     9163 2024-05-18 04:54:35.000000 finaletoolkit-0.6.0/tests/test_end_motifs.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     3601 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/tests/test_frag_io.py
+-rw-r--r--   0 jamesli    (501) staff       (20)      718 2024-05-26 21:27:09.000000 finaletoolkit-0.6.0/tests/test_wps.py
```

### Comparing `finaletoolkit-0.5.2/LICENSE` & `finaletoolkit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.2/pyproject.toml` & `finaletoolkit-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,46 +3,41 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "FinaleToolkit"
-version = "0.5.2"
+version = "0.6.0"
 authors = [
     {name="James Li", email="lijw21@wfu.edu"},
     {name="Ravi Bandaru", email="ravi.bandaru@northwestern.edu"},
     {name="Yaping Liu", email="yaping@northwestern.edu"},
 ]
 description = "A package and standalone program to process paired-end reads of cfDNA fragment WGS."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
 ]
 dependencies = [
     "numpy",
     "pysam",
-    "pybedtools",
     "pybigwig",
     "py2bit",
     "tqdm",
     "numba",
     "scipy",
     "matplotlib",
     "pandas",
-    "cython",
     "statsmodels",
-    "sphinx<7.0.0",
-    "sphinx_rtd_theme",
-    "sphinx-argparse",
     "loess",
 ]
 
 [project.scripts]
 finaletoolkit = "finaletoolkit.cli:main_cli"
 
 [project.urls]
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/__init__.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/__init__.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/adjust_wps.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/adjust_wps.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import gzip
 
 import numpy as np
 from numpy.typing import NDArray
 import pyBigWig as pbw
 from scipy.signal import savgol_filter
 
-from finaletoolkit.utils import genome2list
+from finaletoolkit.utils import chrom_sizes_to_list
 
 def _median_filter(positions: NDArray, data: NDArray, window_size: int):
     """locally adjusted running median"""
     # Calculate the running median
     running_median = np.array(
         [np.median(data[i:i+window_size]) for i in range(len(data) - window_size)]
     )
@@ -251,15 +251,15 @@
         processed_scores = pool.imap(_single_adjust_wps_star, intervals)
 
         if verbose:
             stderr.write('Writing to output\n')
 
         # write to output
         with pbw.open(output_file, 'w') as output_bw:
-            output_bw.addHeader(genome2list(genome_file))
+            output_bw.addHeader(chrom_sizes_to_list(genome_file))
             for scores in processed_scores:
                 contigs, starts, stops, values = scores
                 if len(contigs) == 0:
                     continue
                 try:
                     output_bw.addEntries(
                         contigs,
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/cleavage_profile.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/cleavage_profile.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,37 +5,76 @@
 describes the proportion of fragment ends at a site over the depth at
 the site (cleavage proportion) calculated over a 5+/- nt window around a
 CpG site.
 """
 
 from __future__ import annotations
 from typing import Union
+from pathlib import Path
 from sys import stderr, stdout, stdin
 from multiprocessing import Pool
 import gzip
 import time
 
 import numpy as np
 import pyBigWig as pbw
-from pybedtools import BedTool
 import pysam
 
-from finaletoolkit.utils.utils import frag_array, overlaps
+from finaletoolkit.utils.utils import (
+    frag_array, overlaps, chrom_sizes_to_list, _reduce_overlaps_in_file,
+    _convert_to_list, _merge_all_intervals, chrom_sizes_to_dict
+    )
 
 
 def cleavage_profile(
     input_file: str,
+    chrom_size: int,
     contig: str,
     start: int,
     stop: int,
+    left: int=0,
+    right: int=0,
     fraction_low: int=1,
     fraction_high: int=10000000,
     quality_threshold: int=30,
     verbose: Union[bool, int]=0
 ) -> np.ndarray:
+    """
+    Cleavage profile calculated over a single interval.
+
+    Parameters
+    ---------
+    input_file: str
+        SAM, BAM, CRAM, or FRAG file with fragment information.
+    chrom_size: int
+        length of contig.
+    contig: str
+        Chromosome or contig
+    start: int
+        0-based start coordinate
+    stop: int
+        1-based end coordinate
+    left: int
+        Amount to subtract from start coordinate. Useful if only given
+        coordinates of CpG.
+    right: int
+        Amount to add to stop coordinate.
+    fraction_low: int
+        Minimum fragment size to include
+    fraction_high: int
+        Maximum fragment size to include
+    quality_threshold: int
+        Minimum MAPQ
+    verbose: bool or in
+
+    Return
+    ------
+    cleavage_proportions: NDArray
+        Array of cleavage proportions over given interval.
+    """
     if (verbose):
         start_time = time.time()
         stderr.write(
             f"""
             Calculating cleavage profile
             input_file: {input_file}
             contig: {contig}
@@ -43,26 +82,29 @@
             stop: {stop}
             fraction_low: {fraction_low}
             fraction_high: {fraction_high}
             quality_threshold: {quality_threshold}
             verbose: {verbose}
             """
         )
+    adj_start = max(start-left, 0)
+    adj_stop = min(stop+right, chrom_size)
 
     frags = frag_array(
         input_file=input_file,
         contig=contig,
         quality_threshold=quality_threshold,
-        start=start,
-        stop=stop,
+        start=adj_start,
+        stop=adj_stop,
         fraction_low=fraction_low,
-        fraction_high=fraction_high
+        fraction_high=fraction_high,
+        intersect_policy="any"
     )
 
-    positions = np.arange(start, stop)
+    positions = np.arange(adj_start, adj_stop)
 
     # finding depth at sites
     fragwise_overlaps = np.logical_and(
         np.greater_equal(positions[np.newaxis], frags['start'][:,np.newaxis]),
         np.less(positions[np.newaxis], frags['stop'][:,np.newaxis])
     )
     depth = np.sum(fragwise_overlaps, axis=0)
@@ -75,36 +117,43 @@
     )
     reverse_ends = np.logical_and(
         np.equal(
             positions[np.newaxis], frags['stop'][:, np.newaxis]
         ), np.logical_not(frags['strand'][:, np.newaxis])
     )
     ends = np.sum(np.logical_or(forward_ends, reverse_ends), axis=0)
-    proportions = ends/depth*100
+
+    proportions = np.zeros_like(depth, dtype=np.float64)
+    non_zero_mask = depth != 0
+    proportions[non_zero_mask] = ends[non_zero_mask] / depth[non_zero_mask] * 100
+
 
     results = np.zeros_like(proportions, dtype=[
         ('contig', 'U16'),
         ('pos', 'i8'),
         ('proportion', 'f8'),
     ])
     results['contig'] = contig
-    results['pos'] = np.arange(start, stop)
+    results['pos'] = positions
     results['proportion'] = proportions
 
 
     return results
 
 
 def _cleavage_profile_star(args):
     return cleavage_profile(*args)
 
 
 def _cli_cleavage_profile(
-    input_file: str,
-    interval_file: str,
+    input_file: Union[str, Path],
+    interval_file: Union[str, Path],
+    chrom_sizes: Union[str, Path],
+    left: int=0,
+    right: int=0,
     fraction_low: int=1,
     fraction_high: int=10000000,
     quality_threshold: int=30,
     output_file: str='-',
     workers: int=1,
     verbose: Union[bool, int]=0
 ):
@@ -128,87 +177,65 @@
             verbose: {verbose}
             """
         )
     
     if (input_file == '-' and interval_file == '-'):
         raise ValueError('input_file and site_bed cannot both read from stdin')
     
+    if chrom_sizes is None:
+        raise ValueError(
+            '--chrom_sizes must be specified'
+        )
+    
       # get header from input_file
     if (input_file.endswith('.sam')
         or input_file.endswith('.bam')
         or input_file.endswith('.cram')):
         with pysam.AlignmentFile(input_file, 'r') as bam:
             references = bam.references
             lengths = bam.lengths
             header = list(zip(references, lengths))
-    # TODO: get a header when reading tabix
     elif (input_file.endswith('.bed')
           or input_file.endswith('.bed.gz')
           or input_file.endswith('.frag')
           or input_file.endswith('.frag.gz')
     ):
-        with pysam.TabixFile(input_file, 'r') as tbx:
-            raise NotImplementedError('tabix files not yet supported!')
+        header = chrom_sizes_to_list(chrom_sizes)
     else:
         raise ValueError("Not a supported file type.")
 
     if (verbose > 1):
         stderr.write(f'header is {header}\n')
     
     # reading intervals from bed and removing overlaps
     # NOTE: assumes that bed file is sorted.
-    contigs = []
-    starts = []
-    stops = []
-    try:
-        if interval_file == '-':
-            bed = stdin
-        else:
-            bed = open(interval_file)
-
-        # for overlap checking
-        prev_contig = None
-        prev_start = 0
-        prev_stop = 0
-        for line in bed:
-            contents = line.split()
-            contig = contents[0].strip()
-            start = int(contents[1])
-            stop = int(contents[2])
-
-            # cut off part of previous interval if overlap
-            if contig == prev_contig and start < prev_stop:
-                prev_stop = start
-
-            if prev_contig is not None:
-                contigs.append(prev_contig)
-                starts.append(prev_start)
-                stops.append(prev_stop)
-
-            prev_contig = contig
-            prev_start = start
-            prev_stop = stop
-        # appending last interval
-        contigs.append(prev_contig)
-        starts.append(prev_start)
-        stops.append(prev_stop)
-    finally:
-        if interval_file != '-':
-            bed.close()
+    reduced_intervals = _reduce_overlaps_in_file(interval_file)
+    converted_intervals = _convert_to_list(reduced_intervals)
+    all_intervals = _merge_all_intervals(converted_intervals)
+    contigs, starts, stops = zip(*all_intervals)
+
+    # reading chrom.sizes file
+
+    size_dict = chrom_sizes_to_dict(chrom_sizes)
+
+    sizes = [size_dict[contig] for contig in contigs]
     
     count = len(contigs)
 
     if (verbose):
         stderr.write('Zipping inputs\n')
 
     interval_list = zip(
         count*[input_file],
+        sizes,
         contigs,
         starts,
         stops,
+        count*[left],
+        count*[right],
         count*[fraction_low],
         count*[fraction_high],
         count*[quality_threshold],
         count*[max(verbose-1, 0)]
     )
 
     if (verbose):
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/coverage.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/coverage.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,88 @@
 from __future__ import annotations
 import sys
 import time
-from typing import Union, Tuple
+from typing import Union, Iterable
+from pathlib import Path
 
 from multiprocessing import Pool
 
 import pysam
 import gzip
 from tqdm import tqdm
 
 from finaletoolkit.utils.utils import (
-    _not_read1_or_low_quality, _get_contigs, _get_intervals, frag_generator
+    _get_intervals, frag_generator
 )
 
 
 def single_coverage(
-        input_file: Union[str, pysam.AlignmentFile],
+        input_file: Union[str, pysam.TabixFile, pysam.AlignmentFile, Path],
         contig: str=None,
         start: int=0,
         stop: int=None,
         name: str='.',
         intersect_policy: str="midpoint",
         quality_threshold: int=30,
         verbose: Union[bool, int]=False
-    ) -> Tuple[str, int, int, str, float]:
+    ) -> tuple[str, int, int, str, float]:
     """
     Return estimated fragment coverage over specified `contig` and
     region of`input_file`. Uses an algorithm where the midpoints of
     fragments are calculated and coverage is tabulated from the
     midpoints that fall into the specified region. Not suitable for
     fragments of size approaching region size.
 
     Parameters
     ----------
     input_file : str or pysam.AlignmentFile
         BAM, SAM, CRAM, or Frag.gz file containing paired-end fragment reads or
         its path. `AlignmentFile` must be opened in read mode.
-    contig : string
-    start : int
-    stop : int
-    name : str
+    contig : string, optional
+        Default is None.
+    start : int, optional
+        0-based start coordinate to get coverage from. Default is 0.
+    stop : int, optional
+        1-based stop coordinate to get coverage from. Default is None
+        and goes to end of chromosome/contig.
+    name : str, optional
+        Name of interval. Default is '.'.
+    intersect_policy: str, optional
+        Specifies how to determine whether fragments are in interval.
+        'midpoint' (default) calculates the central coordinate of each fragment
+        and only selects the fragment if the midpoint is in the
+        interval. 'any' includes fragments with any overlap with the
+        interval.
     quality_threshold : int, optional
+        Minimum MAPQ to filter for. Default is 30.
     verbose : bool, optional
-
+        Prints messages to stderr. Default is false.
     Returns
     -------
-    coverage : int
+    (contig, start, stop, name, coverage) : tuple[str, int, int, str, float]
         Fragment coverage over contig and region.
     """
-    # TODO: determine if reference (like as found in pysam) is necessary
-    # TODO: consider including region string (like in pysam)
     if verbose:
         start_time = time.time()
         tqdm.write(
             f"""
-input_file: 
-contig: {contig}
-start: {start}
-stop: {stop}
-name: {name}
-intersect_policy: {intersect_policy}
-quality_threshold: {quality_threshold}
-verbose: {verbose}
-"""
+            input_file: {input_file}
+            contig: {contig}
+            start: {start}
+            stop: {stop}
+            name: {name}
+            intersect_policy: {intersect_policy}
+            quality_threshold: {quality_threshold}
+            verbose: {verbose}
+            """
         )
 
     # initializing variable for coverage tuple outside of with statement
     coverage = 0
 
-    input_type = type(input_file)
-
     frags = frag_generator(
         input_file=input_file,
         contig=contig,
         quality_threshold=quality_threshold,
         start=start,
         stop=stop,
         fraction_low=10,
@@ -97,24 +106,25 @@
 def _single_coverage_star(args):
     """
     Helper function that takes a tuple of args and applies to
     single_coverage. To be used in imap.
     """
     return single_coverage(*args)
 
-
+# TODO: add normalized coverage
 def coverage(
-        input_file: Union[str, pysam.AlignmentFile],
+        input_file: Union[str, pysam.TabixFile, pysam.AlignmentFile, Path],
         interval_file: str,
         output_file: str,
         scale_factor: float=1e6,
+        intersect_policy: str="midpoint",
         quality_threshold: int=30,
         workers: int=1,
         verbose: Union[bool, int]=False
-    ):
+    ) -> Iterable[tuple[str, int, int, str, float]]:
     """
     Return estimated fragment coverage over intervals specified in
     `intervals`. Fragments are read from `input_file` which may be
     a SAM, BAM, CRAM, or Frag.gz file. Uses an algorithm where the midpoints of
     fragments are calculated and coverage is tabulated from the
     midpoints that fall into the specified region. Not suitable for
     fragments of size approaching interval size.
@@ -124,34 +134,45 @@
     input_file : str or pysam.AlignmentFile
         SAM, BAM, CRAM, or Frag.gz file containing paired-end fragment 
         reads or its path. `AlignmentFile` must be opened in read mode.
     interval_file : str
         BED4 file containing intervals over which to generate coverage
         statistics.
     output_file : string, optional
-        Path for bed file to print coverages to. If output_file = `_`,
+        Path for bed file to print coverages to. If output_file = `-`,
         results will be printed to stdout.
     scale_factor : int, optional
         Amount to multiply coverages by. Default is 10^6.
+    intersect_policy: str, optional
+        Specifies how to determine whether fragments are in interval.
+        'midpoint' (default) calculates the central coordinate of each fragment
+        and only selects the fragment if the midpoint is in the
+        interval. 'any' includes fragments with any overlap with the
+        interval.
     quality_threshold : int, optional
+        Minimum MAPQ. Default is 30.
+    workers : int, optional
+        Number of subprocesses to spawn. Increases speed at the expense
+        of memory.
     verbose : int or bool, optional
 
     Returns
     -------
-    coverage : int
-        Fragment coverage over contig and region.
+    coverages : Iterable[tuple[str, int, int, str, float]]
+        Fragment coverages over intervals.
     """
-    #FIXME update docstring
     if (verbose):
         start_time = time.time()
         sys.stderr.write(
             f"""
             input_file: {input_file}
-            interval file: {interval_file}
+            interval_file: {interval_file}
             output_file: {output_file}
+            scale_factor: {scale_factor}
+            intersect_policy: {intersect_policy}
             quality_threshold: {quality_threshold}
             workers: {workers}
             verbose: {verbose}\n
             """
         )
 
     if verbose:
@@ -167,15 +188,15 @@
         )
 
         if verbose:
             tqdm.write('reading intervals\n')
 
         intervals = _get_intervals(
             input_file, interval_file,
-            intersect_policy="midpoint",
+            intersect_policy=intersect_policy,
             quality_threshold=quality_threshold,
             verbose=verbose)
 
         if verbose:
             tqdm.write('calculating coverage\n')
 
         coverages = pool.imap(
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/delfi.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi_gc_correct.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/delfi_gc_correct.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/delfi_merge_bins.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/delfi_merge_bins.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-try:
-    from importlib.resources import files
-except ImportError:
-    from importlib_resources import files
+from importlib.resources import files
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 
 import finaletoolkit.frag as pkg_data
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/end_motifs.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/end_motifs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 from collections.abc import Iterator
-from typing import Union, Iterable, Tuple
+from typing import Union, Iterable
 from multiprocessing import Pool
 from time import time
 from sys import stderr, stdout, stdin
 import gzip
-try:
-    from importlib.resources import files
-except ImportError:
-    from importlib_resources import files
+
+from importlib.resources import files
 from pathlib import Path
 from collections import UserDict
 
 import tqdm
 import py2bit
 import numpy as np
 from numpy.typing import NDArray
@@ -270,15 +268,15 @@
                 dict_freqs = dict(zip(kmers, float_freqs))
                 intervals.append(((contig, start, stop, name), dict_freqs))
         finally:
             if is_file:
                 file.close()
         return cls(intervals, k, quality_threshold)
 
-    def freq(self, kmer: str) -> list[Tuple[str, int, int, float]]:
+    def freq(self, kmer: str) -> list[tuple[str, int, int, float]]:
         """
         Returns a list of intervals and associated frquency for given
         kmer. Results are in the form (chrom, 0-based start, 1-based
         stop, frequency).
         """
         return dict(
             [(*interval, freq[kmer]) for interval, freq in self.intervals]
@@ -790,15 +788,15 @@
 
     return results
 
 
 def interval_end_motifs(
     input_file: str,
     refseq_file: Union[str, Path],
-    intervals: Union[str, Iterable[Tuple[str,int,int,str]]],
+    intervals: Union[str, Iterable[tuple[str,int,int,str]]],
     k: int = 4,
     fraction_low: int = 10,
     fraction_high: int = 600,
     both_strands: bool = True,
     output_file: Union[None, str] = None,
     quality_threshold: int = 30,
     workers: int = 1,
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/frag_length.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/frag_length.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 import time
-from typing import Union, Tuple
+from typing import Union
 from sys import stdout, stderr
 from shutil import get_terminal_size
 from multiprocessing import Pool
 import gzip
 
 import numpy as np
 import pysam
 import tqdm
 
 from finaletoolkit.utils.utils import (
-    _not_read1_or_low_quality, _get_intervals, frag_generator
+    _get_intervals, frag_generator
 )
 from finaletoolkit.utils.cli_hist import _cli_hist
 
 
 def frag_length(
         input_file: Union[str, pysam.AlignmentFile, pysam.TabixFile],
         contig: str=None,
@@ -221,15 +221,15 @@
     bin_size: int=None,
     output_file: str=None,
     contig_by_contig: bool=False,
     histogram: bool=False,
     intersect_policy: str="midpoint",
     quality_threshold: int=30,
     verbose: Union[bool, int]=False
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """
     Takes input_file, computes frag lengths of fragments and returns
     two arrays containing bins and counts by size. Optionally prints
     data to output as a tab delimited table or histogram.
 
     Parameters
     ----------
@@ -357,22 +357,22 @@
             f'frag_length_bins took {stop_time-start_time} s to complete.\n'
         )
 
     return bins, counts
 
 
 def _frag_length_stats(
-    input_file: Union(str, pysam.AlignmentFile),
+    input_file: Union[str, pysam.AlignmentFile],
     contig: str,
     start: int,
     stop: int,
     name: str,
     intersect_policy: str,
     quality_threshold: int,
-    verbose: Union(bool, int)
+    verbose: Union[bool, int]
 ):
     # generating fragment lengths
     frag_lengths = frag_length(
         input_file=input_file,
         contig=contig,
         start=start,
         stop=stop,
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/multi_wps.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/multi_wps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/frag/wps.py` & `finaletoolkit-0.6.0/src/finaletoolkit/frag/wps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from __future__ import annotations
-import argparse
 import gzip
 import time
-import os
-import tempfile as tf
-from multiprocessing.pool import Pool
-from typing import Union, TextIO, BinaryIO
-from sys import stdout, stderr, getsizeof
+from typing import Union
+from sys import stdout, stderr
 
 import pysam
 import numpy as np
 from numba import jit
-from tqdm import tqdm
 
 from finaletoolkit.utils import frag_array
 
 @jit(nopython=True)
 def _single_wps(contig: str,
                 window_start: int,
                 window_stop: int,
@@ -75,17 +70,15 @@
     quality_threshold : int, optional
     workers : int, optional
     verbose : bool, optional
 
     Returns
     -------
     scores : numpy.ndarray
-        np array of shape (n, 2) where column 1 is the coordinate and
-        column 2 is the score and n is the number of coordinates in
-        region [start,stop)
+        np struct array of with columns `contig`, `start`, and `wps`.
     """
 
     if (verbose):
         start_time = time.time()
         stderr.write("[finaletoolkit-wps] Reading fragments\n")
         stderr.write(f'Region: {contig}:{start}-{stop}\n')
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/genome/gaps.py` & `finaletoolkit-0.6.0/src/finaletoolkit/genome/gaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """
-FinaleTools.gaps
+finaletoolkit.gaps
 ================
 
 This module contains classes and functions to use the gap tracks found
 on the UCSC Genome Browser (Kent et al 2002).
 """
 
 from __future__ import annotations
-from typing import Union, Tuple, Iterable
+from typing import Union, Iterable
 import gzip
-try:
-    from importlib.resources import files
-except ImportError:
-    from importlib_resources import files
+from importlib.resources import files
 from pathlib import Path
 from sys import stdout
 
 import numpy as np
 from numpy.typing import NDArray
 
 import finaletoolkit.genome as genome
@@ -324,16 +321,16 @@
                         f"{interval['stop']}\t{interval['type']}\n"
                     )
 
 
 class ContigGaps():
     def __init__(self,
                  contig: str,
-                 centromere: Tuple[int, int],
-                 telomeres:Iterable[Tuple[int, int]],
+                 centromere: tuple[int, int],
+                 telomeres:Iterable[tuple[int, int]],
                  has_short_arm: bool=False):
         self.contig = contig
         self.centromere = centromere
         self.telomeres = telomeres
         self.has_short_arm = has_short_arm
 
     def in_tcmere(self, start: int, stop: int) -> bool:
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/utils/agg_bw.py` & `finaletoolkit-0.6.0/src/finaletoolkit/utils/agg_bw.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/utils/cli_hist.py` & `finaletoolkit-0.6.0/src/finaletoolkit/utils/cli_hist.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/utils/filter_bam.py` & `finaletoolkit-0.6.0/src/finaletoolkit/utils/filter_bam.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from __future__ import annotations
 import tempfile as tf
 import subprocess
 import traceback
-from sys import stderr
-from os.path import isdir
-from shutil import rmtree
 
 import pysam
 
 def filter_bam(
         input_file: str,
         region_file: str=None,
         output_file: str=None,
@@ -49,15 +46,15 @@
 
 
         # create temp dir to store intermediate sorted file
     try:
         with tf.TemporaryDirectory() as temp_dir:
             flag_filtered_bam = f'{temp_dir}/flag_filtered.bam'
             samtools_command = (
-                f'samtools view {input_file} -F 3852 -f 66 -b -h -o '
+                f'samtools view {input_file} -F 3852 -f 3 -b -h -o '
                 f'{flag_filtered_bam} -q {quality_threshold} -@ {workers}'
             )
 
             if region_file is not None:
                 samtools_command += f' -M -L {region_file}'
 
             try:
```

### Comparing `finaletoolkit-0.5.2/src/finaletoolkit/utils/utils.py` & `finaletoolkit-0.6.0/src/finaletoolkit/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,89 @@
 from __future__ import annotations
 import time
 import gzip
 import tempfile as tf
-from typing import Union, TextIO, Tuple, List, Generator
+from typing import Union, TextIO, Generator, Iterable
 from sys import stderr, stdout
 from pathlib import Path
 
 import numpy as np
 from numpy.typing import NDArray
 from numba import jit
 import pysam
 from tqdm import tqdm
 
 
-def _get_contigs(
-        input_file: Union[str, pysam.AlignmentFile],
-        verbose: bool=False
-    ) -> list:
+def chrom_sizes_to_list(
+    chrom_sizes_file: Union[str, Path]) -> list[tuple[str][int]]:
     """
-    Retrieves contigs from input_file and returns lists of contig names
-    and lengths
+    Reads chromosome names and sizes from a CHROMSIZE file into a list.
     """
+    chrom_sizes = []
+    with open(chrom_sizes_file, 'r') as file:
+        for line in file:
+            if line != '\n':
+                chrom, size = line.strip().split('\t')
+                chrom_sizes.append((chrom, int(size)))
+    return chrom_sizes
 
-    input_is_file = False
-    try:
-        # handling input types
-        if (type(input_file) == pysam.AlignmentFile):
-            sam_file = input_file
-        elif input_file.endswith('bam'):
-            input_is_file = True
-            if (verbose):
-                stderr.write(f'Opening {input_file}\n')
-            sam_file = pysam.AlignmentFile(input_file)
+
+def chrom_sizes_to_dict(
+    chrom_sizes_file: Union[str, Path]) -> list[tuple[str][int]]:
+    """
+    Reads chromosome names and sizes from a CHROMSIZE file into a list.
+    """
+    chrom_sizes = {}
+    with open(chrom_sizes_file, 'r') as file:
+        for line in file:
+            if line != '\n':
+                chrom, size = line.strip().split('\t')
+                chrom_sizes[chrom] = size
+    return chrom_sizes
+
+
+def _merge_overlapping_intervals(intervals):
+    intervals.sort(key=lambda x: x[0])
+    merged = []
+    for interval in intervals:
+        if not merged or interval[0] > merged[-1][1]:
+            merged.append(interval)
         else:
-            raise ValueError(
-                'Invalid input_file type. Only BAM or SAM files are allowed.'
-            )
-        contigs = sam_file.references
-        lengths = sam_file.lengths
-    finally:
-        if input_is_file:
-            sam_file.close()
+            merged[-1] = (merged[-1][0], max(merged[-1][1], interval[1]))
+    return merged
 
-    return zip(contigs, lengths)
+
+def _reduce_overlaps_in_file(interval_file):
+    intervals_dict = {}
+    with open(interval_file, 'r') as file:
+        for line in file:
+            chrom, start, end = line.strip().split('\t')[:3]
+            start, end = int(start), int(end)
+            if chrom not in intervals_dict:
+                intervals_dict[chrom] = []
+            intervals_dict[chrom].append((start, end))
+
+    reduced_intervals = {}
+    for chrom, intervals in intervals_dict.items():
+        reduced_intervals[chrom] = _merge_overlapping_intervals(intervals)
+    return reduced_intervals    
+
+
+def _convert_to_list(reduced_intervals):
+    converted_intervals = {}
+    for chrom, intervals in reduced_intervals.items():
+        converted_intervals[chrom] = [[chrom, start, end] for start, end in intervals]
+    return converted_intervals
+
+
+def _merge_all_intervals(converted_intervals):
+    all_intervals = []
+    for intervals in converted_intervals.values():
+        all_intervals.extend(intervals)
+    return all_intervals
 
 
 def frag_bam_to_bed(input_file: Union[str, pysam.AlignmentFile],
                     output_file: str,
                     contig: str=None,
                     quality_threshold: int=30,
                     verbose: bool=False):
@@ -142,15 +179,15 @@
     quality_threshold: int=30,
     start: int=None,
     stop: int=None,
     fraction_low: int=120,
     fraction_high: int=180,
     intersect_policy: str="midpoint",
     verbose: bool=False
-) -> Generator[Tuple]:
+) -> Generator[tuple]:
     """
     Reads from BAM, SAM, or BED file and returns tuples containing
     contig (chromosome), start, stop (end), mapq, and strand for each fragment.
     Optionally may filter for mapq, size, and intersection with a region.
 
     Parameters
     ----------
@@ -226,15 +263,19 @@
             check_intersect = lambda r_start, r_stop, f_start, f_stop : (
                 (r_start is None or f_stop > r_start)
                 and (r_stop is None or f_start < r_stop)
             )
         else:
             raise ValueError(f'{intersect_policy} is not a valid policy')
 
-        #FIXME: raise exception if start and stop specified but not contig
+        # Raise exception if start and stop specified but not contig
+        if contig is None and not (start is None and stop is None):
+            raise ValueError("contig should be specified if start or "
+                             "stop given.")
+
         if is_sam:
             for read in sam_file.fetch(contig, start, stop):
                 # Only select read1 and filter out non-paired-end
                 # reads and low-quality reads
                 try:
                     if (low_quality_read_pairs(read, quality_threshold)
                         or read.is_read2):
@@ -263,15 +304,14 @@
                                 yield (
                                     read.reference_name,
                                     read.reference_end + read.template_length,
                                     read.reference_end,
                                     read.mapping_quality,
                                     read.is_forward 
                                 )
-                # HACK: for some reason read_length is sometimes None
                 except TypeError as e:
                     stderr.writelines(["Type error encountered.\n",
                                        f"Fragment length: {frag_length}\n",
                                        f"fraction_low: {fraction_low}\n",
                                        f"fraction_high: {fraction_high}\n",
                                        "Skipping interval.\n",
                                        f"Error: {e}\n"])
@@ -310,16 +350,16 @@
     stop: int=None,
     fraction_low: int=120,
     fraction_high: int=180,
     intersect_policy: str="midpoint",
     verbose: bool=False
     ) -> NDArray:
     """
-    Reads from BAM, SAM, or BED file and returns a two column matrix
-    with fragment start and stop positions.
+    Reads from BAM, SAM, or BED file and returns a three column matrix
+    with fragment start and stop positions and strand.
 
     Parameters
     ----------
     input_file : str or AlignmentFile
     contig : str
     quality_threshold : int, optional
     start : int, optional
@@ -331,15 +371,15 @@
         Specifies highest fragment length included in array. Default is
         120, equivalent to long fraction.
         intersect_policy : str, optional
         Specifies what policy is used to include fragments in the
         given interval. Default is "midpoint". Policies include:
         - midpoint: the average of end coordinates of a fragment lies
         in the interval.
-        - any: any part of the fragment is in the interval.v
+        - any: any part of the fragment is in the interval.
     verbose : bool, optional
 
     Returns
     -------
     frag_ends : NDArray
         'NDArray' with shape (n, 3) where column 1 contains fragment
         start position and column 2 contains fragment stop position, and
@@ -436,15 +476,15 @@
 
 def _get_intervals(
     input_file: Union[str, pysam.AlignmentFile],
     interval_file: str,
     intersect_policy: str,
     quality_threshold: int,
     verbose: Union[bool, int]
-) -> list[Tuple[str, str, int, int, str, str, int]]:
+) -> list[tuple[str, str, int, int, str, str, int]]:
     """
     Helper function to read intervals from bed file.
     Returns list of tuples:
     (input_file, chrom, start, stop, name, intersect_policy,
     quality_threshold, verbosity)
     """
     intervals = []  # list of inputs for single_coverage
@@ -469,39 +509,14 @@
                     )
                     intervals.append(interval)
                 else:
                     break
     return intervals
 
 
-def genome2list(genome_file: str) -> list:
-    """
-    Reads a GENOME text file into a list of tuples (chrom, length)
-
-    Parameters
-    ----------
-    genome_file : str
-        String containing path to GENOME format file
-
-    Returns
-    _______
-    chroms : str
-        List of tuples containing chrom/contig names and lengths
-    """
-    chroms = []
-    with open(genome_file) as file:
-        for line in file:
-            if line != '\n':
-                chroms.append((
-                    (contents:=line.split('\t'))[0],
-                    int(contents[1])
-                ))
-    return chroms
-
-
 def overlaps(
     contigs_1: NDArray,
     starts_1: NDArray,
     stops_1: NDArray,
     contigs_2: NDArray,
     starts_2: NDArray,
     stops_2: NDArray,
```

### Comparing `finaletoolkit-0.5.2/tests/test_frag_io.py` & `finaletoolkit-0.6.0/tests/test_frag_io.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,9 +52,48 @@
         
         assert len(frags) == 17, "Incorrect number of frags"
 
         
 
 
 class TestFragArray:
-    pass
+    def test_bam(self, request):
+        """
+        See if frag_array runs when opening a BAM file and reads the
+        right number of reads
+        """
+        bam = request.path.parent / 'data' / '12.3444.b37.bam'
+        frags = frag_array(
+            bam, "12", quality_threshold=0, fraction_low=0, fraction_high=9999
+        )
+
+        starts = frags['start']
+        stops = frags['stop']
+        strands = frags['strand']
+
+        in_region = np.any(overlaps(np.array(['12']), np.array([34442500]),
+                               np.array([34446500]), np.array(['12']), starts, stops))
+        assert in_region, "Some fragments are outside of region"
+        
+        assert len(frags) == 17, "Incorrect number of frags"
+
+    def test_frag_gz(self, request):
+        """
+        See if frag_array runs when opening a frag.gz file and reads the
+        right number of reads
+        """
+        path = request.path.parent / 'data' / '12.3444.b37.frag.gz'
+        frags = frag_array(
+            path, "12", quality_threshold=0, fraction_low=0, fraction_high=9999
+        )
+
+        starts = frags['start']
+        stops = frags['stop']
+        strands = frags['strand']
+
+        in_region = np.any(
+            overlaps(np.array(['12']), np.array([34442500]),
+                     np.array([34446500]), np.array(['12']), starts, stops))
+        assert in_region, "Some fragments are outside of region"
+        
+        assert len(frags) == 17, "Incorrect number of frags"
```

