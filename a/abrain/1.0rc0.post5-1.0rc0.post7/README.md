# Comparing `tmp/abrain-1.0rc0.post5.tar.gz` & `tmp/abrain-1.0rc0.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abrain-1.0rc0.post5.tar", last modified: Fri Mar 15 19:03:36 2024, max compression
+gzip compressed data, was "abrain-1.0rc0.post7.tar", last modified: Sun May 26 17:42:53 2024, max compression
```

## Comparing `abrain-1.0rc0.post5.tar` & `abrain-1.0rc0.post7.tar`

### file list

```diff
@@ -1,69 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.478598 abrain-1.0rc0.post5/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8439 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-03-15 19:03:36.478598 abrain-1.0rc0.post5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 19:03:36.478598 abrain-1.0rc0.post5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.466598 abrain-1.0rc0.post5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.466598 abrain-1.0rc0.post5/src/abrain/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.470598 abrain-1.0rc0.post5/src/abrain/_bindings/
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_bindings/config.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_bindings/genotype.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_bindings/module.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.470598 abrain-1.0rc0.post5/src/abrain/_bindings/phenotype/
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_bindings/phenotype/ann.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_bindings/phenotype/cppn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_bindings/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.470598 abrain-1.0rc0.post5/src/abrain/_cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/config.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/config.h
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/genotype.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.470598 abrain-1.0rc0.post5/src/abrain/_cpp/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/misc/constants_template.h
--rwxr-xr-x   0 runner    (1001) docker     (127)     3548 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/misc/point.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.470598 abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7300 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/ann.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     4056 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/ann.h
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/cppn.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/cppn.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    15183 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/eshn.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/eshn.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.474598 abrain-1.0rc0.post5/src/abrain/core/
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/ann.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.474598 abrain-1.0rc0.post5/src/abrain/core/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/abs.png
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/abs.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/bsgm.png
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/bsgm.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/gaus.png
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/gaus.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/id.png
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/id.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3212 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/plotter.sh
--rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/sin.png
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/sin.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8605 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/ssgm.png
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/ssgm.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/ssgn.png
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/ssgn.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/step.png
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/step.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/functions/template.tex
--rw-r--r--   0 runner    (1001) docker     (127)    21772 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/src/abrain/core/genome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.478598 abrain-1.0rc0.post5/src/abrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-03-15 19:03:36.000000 abrain-1.0rc0.post5/src/abrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-15 19:03:36.000000 abrain-1.0rc0.post5/src/abrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 19:03:36.000000 abrain-1.0rc0.post5/src/abrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-15 19:03:36.000000 abrain-1.0rc0.post5/src/abrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 19:03:36.000000 abrain-1.0rc0.post5/src/abrain.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 19:03:36.478598 abrain-1.0rc0.post5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/tests/test_ann.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/tests/test_cppn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/tests/test_evolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-03-15 19:03:31.000000 abrain-1.0rc0.post5/tests/test_genome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.684395 abrain-1.0rc0.post7/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7604 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-26 17:42:53.684395 abrain-1.0rc0.post7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 17:42:53.684395 abrain-1.0rc0.post7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.668395 abrain-1.0rc0.post7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.672395 abrain-1.0rc0.post7/src/abrain/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.672395 abrain-1.0rc0.post7/src/abrain/_bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_bindings/config.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_bindings/genotype.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_bindings/innovations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_bindings/module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.672395 abrain-1.0rc0.post7/src/abrain/_bindings/phenotype/
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_bindings/phenotype/ann.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_bindings/phenotype/cppn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_bindings/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.676395 abrain-1.0rc0.post7/src/abrain/_cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/config.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/config.h
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/genotype.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/innovations.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/innovations.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.676395 abrain-1.0rc0.post7/src/abrain/_cpp/misc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3279 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/misc/point.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/misc/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.676395 abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8461 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/ann.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4606 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/ann.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/cppn.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/cppn.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17099 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/eshn.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1742 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/eshn.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.676395 abrain-1.0rc0.post7/src/abrain/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    11233 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/ann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/cppn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.680395 abrain-1.0rc0.post7/src/abrain/core/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/abs.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/abs.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/bsgm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/bsgm.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/gaus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/gaus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/id.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/id.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3212 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/plotter.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    10419 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/sin.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/sin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8605 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/ssgm.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/ssgm.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/ssgn.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/ssgn.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7893 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/step.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/step.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/functions/template.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    41279 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/src/abrain/core/genome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.680395 abrain-1.0rc0.post7/src/abrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-26 17:42:53.000000 abrain-1.0rc0.post7/src/abrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-26 17:42:53.000000 abrain-1.0rc0.post7/src/abrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 17:42:53.000000 abrain-1.0rc0.post7/src/abrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-26 17:42:53.000000 abrain-1.0rc0.post7/src/abrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-26 17:42:53.000000 abrain-1.0rc0.post7/src/abrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:42:53.680395 abrain-1.0rc0.post7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/tests/test_ann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/tests/test_cppn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/tests/test_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20472 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/tests/test_genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-05-26 17:42:49.000000 abrain-1.0rc0.post7/tests/test_innovations.py
```

### Comparing `abrain-1.0rc0.post5/CMakeLists.txt` & `abrain-1.0rc0.post7/CMakeLists.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,45 @@
-cmake_minimum_required(VERSION 3.4)
+cmake_minimum_required(VERSION 3.5)
 
 ################################################################################
 ## General settings
 ################################################################################
 
 project("abrain")
 message("\n####################################################################"
-    "############\n## CMakeFile for ${PROJECT_NAME}")
+    "############\n## CMakeFile for ${PROJECT_NAME} ${VERSION_INFO}")
 
 # set(CMAKE_CXX_FLAGS "")
 if(LINUX)
   string(APPEND CMAKE_CXX_FLAGS " -Wall -Wextra -pedantic")
 endif()
 if(MSVC)
   string(APPEND CMAKE_CXX_FLAGS " /EHsc")
 endif()
 
-set(CMAKE_CXX_STANDARD 17)
+set(CMAKE_CXX_STANDARD 20)
 
 set(CMAKE_CXX_FLAGS_RELEASE "-O2 -DNDEBUG")
+set(CMAKE_CXX_FLAGS_DEBUG "-fno-elide-constructors -fno-default-inline")
+
+################################################################################
+## Dependencies
+################################################################################
+
+if (Python3_EXECUTABLE)
+    get_filename_component(PYTHON_BIN ${Python3_EXECUTABLE} DIRECTORY)
+    set(ENV{PATH} "$ENV{PATH}:${PYTHON_BIN}")
+    message("Provided python: ${Python3_EXECUTABLE} (added to path)")
+endif()
+#
+#find_package (Python3 COMPONENTS Interpreter Development)
+#message("Using python* ${Python_EXECUTABLE} ${PYTHON_EXECUTABLE}")
+#message("Using python3 ${Python3_EXECUTABLE}")
+
+find_package(pybind11 REQUIRED)
 
 ################################################################################
 ## Source files
 ################################################################################
 
 FUNCTION(PREPEND output prefix)
    SET(listVar "")
@@ -31,42 +48,46 @@
    ENDFOREACH(f)
    SET(${output} "${listVar}" PARENT_SCOPE)
 ENDFUNCTION(PREPEND)
 
 set(CPP_SRC
     "config.cpp"
 
-    "misc/constants.h"
+#    "misc/constants.h"
     "misc/point.hpp"
 
     "genotype.h"
+    "innovations.cpp"
+    "innovations.h"
 
     "phenotype/cppn.cpp"
+    "phenotype/cppn.h"
     "phenotype/ann.cpp"
     "phenotype/eshn.cpp"
 )
 PREPEND(CPP_SRC "src/abrain/_cpp")
 
 set(PYBIND_SRC
     "module.cpp"
     "config.cpp"
 
     "genotype.cpp"
+    "innovations.cpp"
 
     "phenotype/cppn.cpp"
     "phenotype/ann.cpp"
+
+    "utils.hpp"
 )
 PREPEND(PYBIND_SRC "src/abrain/_bindings")
 
 set(LIB_CPP _cpp)
-#add_subdirectory(extern/pybind11)
-find_package(pybind11 REQUIRED)
 pybind11_add_module(${LIB_CPP} ${CPP_SRC} ${PYBIND_SRC})
 target_compile_definitions(${LIB_CPP}
-                           PRIVATE VERSION_INFO=${EXAMPLE_VERSION_INFO})
+                           PRIVATE VERSION_INFO=${VERSION_INFO})
 
 ################################################################################
 ## C++ Coverage
 ################################################################################
 message("> With coverage ${WITH_COVERAGE}")
 if(WITH_COVERAGE)
     message("#### Searching for packages")
@@ -89,19 +110,24 @@
 #################################################################################
 
 if (DEV_BUILD)
     set(DEV_SUFFIX " (dev)")
 endif()
 
 message("> Build type: ${CMAKE_BUILD_TYPE}${DEV_SUFFIX}")
+message(">    Version: ${VERSION_INFO}")
+
 message("> On n cores: ${CMAKE_BUILD_PARALLEL_LEVEL}")
 
 option(MAKE_STUBS "Sets whether to generate pyi files from module" ON)
 message("> Generate stubs " ${MAKE_STUBS})
 
+option(AUTO_INSTALL "Sets whether to copy compiled library to source folder during build" OFF)
+message("> Auto install " ${AUTO_INSTALL})
+
 option(WITH_DEBUG_INFO "Sets whether to maximize debug data collection" OFF)
 message("> With debug info " ${WITH_DEBUG_INFO})
 if(WITH_DEBUG_INFO)
     add_definitions(-DWITH_DEBUG_INFO)
 
     # Enable small memory error detector (fuse=gold fixes linker errors)
 #    set(ASAN "-fsanitize=thread")
@@ -129,107 +155,64 @@
     if(WITH_COVERAGE)
         message(SEND_ERROR
             "Generating coverage information is only available in debug mode "
             "(currently using ${CMAKE_BUILD_TYPE})")
     endif()
 endif()
 
-option(ESHN_WITH_DISTANCE "Whether CPPN inputs include connection length" ON)
-message("> CPPN distance: ${ESHN_WITH_DISTANCE}")
-if (ESHN_WITH_DISTANCE)
-    add_definitions(-DESHN_WITH_DISTANCE)
-endif()
-
-set(ESHN_SUBSTRATE_DIMENSION "3" CACHE STRING
-    "Dimension of the ANN substrate (2 or 3)")
-set_property(CACHE ESHN_SUBSTRATE_DIMENSION PROPERTY STRINGS 2 3)
-message("> Substrate dimension: ${ESHN_SUBSTRATE_DIMENSION}")
-add_definitions(-DESHN_SUBSTRATE_DIMENSION=${ESHN_SUBSTRATE_DIMENSION})
-
-#################################################################################
-### Generate configuration files
-#################################################################################
-
-set(CPPN_CONSTANTS ${PROJECT_SOURCE_DIR}/src/abrain/_cpp/misc/constants)
-
-## CPPN Inputs (depends on arguments)
-set(CPPN_INPUTS_LIST "")
-set(CPPN_INPUT_NAMES "")
-foreach(i RANGE 0 1)
-    string(APPEND CPPN_INPUTS_LIST "X${i} Y${i} ")
-    string(APPEND CPPN_INPUT_NAMES "x_${i} y_${i} ")
-    if (${ESHN_SUBSTRATE_DIMENSION} EQUAL 3)
-        string(APPEND CPPN_INPUTS_LIST "Z${i} ")
-        string(APPEND CPPN_INPUT_NAMES "z_${i} ")
-    endif()
-endforeach()
-if(ESHN_WITH_DISTANCE)
-    string(APPEND CPPN_INPUTS_LIST "Length ")
-    string(APPEND CPPN_INPUT_NAMES "l ")
-endif()
-string(APPEND CPPN_INPUTS_LIST "Bias")
-string(APPEND CPPN_INPUT_NAMES "b")
-string(REGEX REPLACE "([^ ]+)" "\"\\1\"," CPPN_INPUT_NAMES ${CPPN_INPUT_NAMES})
-string(REGEX MATCHALL "[^ ]+" tokens ${CPPN_INPUTS_LIST})
-list(LENGTH tokens CPPN_INPUTS_COUNT)
-message("> CPPN inputs: ${CPPN_INPUTS_LIST}")
-
-## CPPN Outputs (constant for now)
-set(CPPN_OUTPUTS_LIST "Weight LEO Bias")
-set(CPPN_OUTPUT_NAMES "w l b")
-string(REGEX MATCHALL "[^ ]+" tokens ${CPPN_OUTPUTS_LIST})
-string(REGEX REPLACE "([^ ]+)" "\"\\1\"," CPPN_OUTPUT_NAMES ${CPPN_OUTPUT_NAMES})
-list(LENGTH tokens CPPN_OUTPUTS_COUNT)
-
-string(REPLACE " " ", " CPPN_INPUTS_LIST ${CPPN_INPUTS_LIST})
-string(REGEX REPLACE "([^ ,]+)" "\"\\1\""
-    CPPN_INPUT_ENUM_NAMES ${CPPN_INPUTS_LIST})
-string(REPLACE " " ", " CPPN_OUTPUTS_LIST ${CPPN_OUTPUTS_LIST})
-string(REGEX REPLACE "([^ ,]+)" "\"\\1\""
-    CPPN_OUTPUT_ENUM_NAMES ${CPPN_OUTPUTS_LIST})
-string(REGEX REPLACE "([^ ]+)" "CPPN_OUTPUT::\\1"    
-    CPPN_QUALIFIED_OUTPUTS ${CPPN_OUTPUTS_LIST})
-
-configure_file(${CPPN_CONSTANTS}_template.h ${CPPN_CONSTANTS}.h)
-message("-+ Generated cppn constants config '${CPPN_CONSTANTS}.h'")
-
 message("> Compile with: ${CMAKE_CXX_FLAGS}")
 
 #################################################################################
 ### Install cpp library
 #################################################################################
 
 if (MAKE_STUBS)
     set(STUBS_DIR ${PROJECT_SOURCE_DIR}/src/${PROJECT_NAME}/${LIB_CPP})
     set(PATH_SEP ":")
     if (WIN32)
       set(PATH_SEP ";")
     endif()
+    find_program(STUBGEN pybind11-stubgen REQUIRED)
+    message("Generating stubs with ${STUBGEN}")
     add_custom_command(
         TARGET ${LIB_CPP} POST_BUILD
         COMMAND echo "binary dir is: ${PROJECT_BINARY_DIR}"
         COMMAND echo "lib has been built as: $<TARGET_FILE:${LIB_CPP}>"
         COMMAND echo "CMAKE_PREFIX_PATH: '${CMAKE_PREFIX_PATH}'"
         COMMAND echo "             PATH: '$ENV{PATH}'"
         COMMAND echo "  BUILD_TIME_PATH: '${BUILD_TIME_PATH}'"
         COMMAND echo "      PYTHON_PATH: '$ENV{PYTHONPATH}'"
+        COMMAND pwd
+        COMMAND ls -d $<TARGET_FILE_DIR:${LIB_CPP}>
+        COMMAND ls $<TARGET_FILE_DIR:${LIB_CPP}>
+        COMMAND which ${STUBGEN}
         COMMAND ${CMAKE_COMMAND} -E
             env "PATH=${BUILD_TIME_PATH}"
             env "PYTHONPATH=.${PATH_SEP}$ENV{PYTHONPATH}"
-            pybind11-stubgen -o ${PROJECT_BINARY_DIR}/
+            ${STUBGEN} -o ${PROJECT_BINARY_DIR}/
                 #--skip-signature-downgrade --no-setup-py --log-level DEBUG
                 --exit-code
                 ${LIB_CPP}
         COMMAND ${CMAKE_COMMAND} -E copy_directory
             ${PROJECT_BINARY_DIR}/${LIB_CPP}/ ${STUBS_DIR}
         WORKING_DIRECTORY $<TARGET_FILE_DIR:${LIB_CPP}>
         COMMENT "-+ Generating python stubs from c++ bindings"
     )
 endif()
 
+if (AUTO_INSTALL)
+    set(LIB_DEST "${PROJECT_SOURCE_DIR}/src/abrain/")
+    add_custom_command(
+        TARGET ${LIB_CPP} POST_BUILD
+            COMMAND ${CMAKE_COMMAND} -E copy $<TARGET_FILE:${LIB_CPP}> ${LIB_DEST}
+            COMMAND ${CMAKE_COMMAND} -E echo "Copied $<TARGET_FILE:${LIB_CPP}> to ${LIB_DEST}"
+    )
+    message(">> Library ${LIB_CPP} will be automatically copied to ${LIB_DEST}")
+endif()
+
 #################################################################################
 ### Ugly hack to get additional files
 #################################################################################
 
 file(GLOB FUNCS
     ${CMAKE_SOURCE_DIR}/ps/*.ps
     ${CMAKE_SOURCE_DIR}/ps/*.png)
```

### Comparing `abrain-1.0rc0.post5/LICENSE` & `abrain-1.0rc0.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/PKG-INFO` & `abrain-1.0rc0.post7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abrain
-Version: 1.0rc0.post5
+Version: 1.0rc0.post7
 Summary: NeuroEvolution in Python backed by C++ computations
 Author-email: Kevin Godin-Dubois <k.j.m.godin-dubois@vu.nl>
 Project-URL: Homepage, https://github.com/kgd-al/abrain
 Project-URL: Documentation, https://abrain.rtfd.io
 Project-URL: Bug Tracker, https://github.com/kgd-al/abrain/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C++
@@ -24,18 +24,26 @@
 Requires-Dist: pyrecord
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-steps; extra == "tests"
 Requires-Dist: pytest-sugar; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
 Requires-Dist: flake8; extra == "tests"
+Provides-Extra: all-tests
+Requires-Dist: abrain[kaleido,tests]; extra == "all-tests"
+Requires-Dist: leap-ec; extra == "all-tests"
+Requires-Dist: Pillow; extra == "all-tests"
+Requires-Dist: qdpy; extra == "all-tests"
+Requires-Dist: tqdm; extra == "all-tests"
+Requires-Dist: matplotlib; extra == "all-tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-pyproject; extra == "docs"
 Requires-Dist: sphinx_design; extra == "docs"
+Requires-Dist: sphinx-tabs; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: kaleido
 Requires-Dist: kaleido; extra == "kaleido"
```

### Comparing `abrain-1.0rc0.post5/README.md` & `abrain-1.0rc0.post7/README.md`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/pyproject.toml` & `abrain-1.0rc0.post7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "abrain"
-version = "1.0rc-post5"
+version = "1.0rc-post7"
 authors = [{ name="Kevin Godin-Dubois", email="k.j.m.godin-dubois@vu.nl"}]
 description = "NeuroEvolution in Python backed by C++ computations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 3 - Alpha",
   
@@ -32,31 +32,38 @@
 Documentation = "https://abrain.rtfd.io"
 "Bug Tracker" = "https://github.com/kgd-al/abrain/issues"
 
 [build-system]
 requires = [
   "setuptools>=65.0",
   "cmake>=3.12",
-  "pybind11",
+  "pybind11[global]",
   "pybind11-stubgen",
 ]
 build-backend = "setuptools.build_meta"
 
 [project.optional-dependencies]
 tests = [
   "pytest",
   "pytest-steps", "pytest-sugar",
   "coverage",
   "flake8",
 ]
 
+all-tests = [
+  "abrain[tests,kaleido]",
+  "leap-ec", "Pillow", "qdpy", "tqdm", "matplotlib"
+]
+
+
 docs = [
   "sphinx",
   "sphinx-pyproject",   # Auto-extract project version
   "sphinx_design",      # for the nice flowing cards
+  "sphinx-tabs",        # For the 2D/3D cards
   "matplotlib",         # for the plot extension
   "sphinx-copybutton",  # Easily copy code
   "myst-parser",        # Better parser
   "furo"                # Style
 
 ]
```

### Comparing `abrain-1.0rc0.post5/setup.py` & `abrain-1.0rc0.post7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,20 +66,21 @@
         build_args = []
         # Adding CMake arguments set as environment variable
         # (needed e.g. to build for ARM OSx on conda-forge)
 
         if "CMAKE_ARGS" in os.environ:
             cmake_args += [item for item in os.environ["CMAKE_ARGS"].split(" ")
                            if item]
-        print('[kgd-debug]', cmake_args)
 
         # Pass the version to C++ (why not?)
-        cmake_args +=\
-            [f"-DEXAMPLE_VERSION_INFO={self.distribution.get_version()}"] \
+        if version := self.distribution.get_version():
             # type: ignore[attr-defined]
+            cmake_args += [f"-DVERSION_INFO={version}"]
+        else:
+            print("No version")
 
         if self.compiler.compiler_type != "msvc":
             # Using Ninja-build since it a) is available as a wheel and b)
             # multithreads automatically. MSVC would require all variables be
             # exported for Ninja to pick it up, which is a little tricky to do.
             # Users can override the generator with CMAKE_GENERATOR in CMake
             # 3.15+.
@@ -138,25 +139,39 @@
                 build_args += [f"-j{self.parallel}"]
 
         build_temp = Path(self.build_temp) / ext.name
         if not build_temp.exists():
             build_temp.mkdir(parents=True)
 
         # == kgd - Additions == #
-        # Allow discovering packages in build site-packages (overlay?)
-        cmake_args += [f"-DCMAKE_PREFIX_PATH={';'.join(sys.path)}"]
         if with_tests:
             cmake_args += ["-DWITH_COVERAGE=ON"]
-        # Ensure discovery of executables (pybind11-stubgen for instance)
-        cmake_args += [f"-DBUILD_TIME_PATH={os.environ.get('PATH')}"]
         # Forward if we need develop-level info (notably the stubs)
         if dev_build:
             cmake_args += ["-DDEV_BUILD=ON"]
 
         # ===================== #
+        # Write clion configuration (if requested)
+        if (path := os.environ.get("CLION_CONFIG")) is not None:
+            with open(path, "w") as cc:
+                cc.write("Replace the ninja builder with default (Makefile)\n")
+                cc.write("Replace the default build folder with:\n")
+                cc.write(f"\t{build_temp}\n")
+                cc.write("Give the following arguments for cmake:\n")
+                config_str = ' '.join(['-DAUTO_INSTALL=ON'] + cmake_args)
+                cc.write(f"\t{config_str}\n")
+                cc.write("Ensure the build command looks like:\n")
+                build_str = ' '.join(['cmake', '--build', '.'] + build_args)
+                cc.write(f"       build: {build_str}\n")
+        # ===================== #
+
+        # Allow discovering packages in build site-packages (overlay?)
+        cmake_args += [f"-DCMAKE_PREFIX_PATH={';'.join(sys.path)}"]
+        # Ensure discovery of executables (pybind11-stubgen for instance)
+        cmake_args += [f"-DBUILD_TIME_PATH={os.environ.get('PATH')}"]
 
         subprocess.run(
             ["cmake", ext.sourcedir] + cmake_args, cwd=build_temp, check=True
         )
         subprocess.run(
             ["cmake", "--build", "."] + build_args, cwd=build_temp, check=True
         )
```

### Comparing `abrain-1.0rc0.post5/src/abrain/__init__.py` & `abrain-1.0rc0.post7/src/abrain/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Docstring for abrain module/top-level package"""
 
 import importlib.metadata
 
-from ._cpp.phenotype import ANN as ANN
-from ._cpp.phenotype import CPPN as CPPN
-from ._cpp.phenotype import Point as Point
-from .core.ann import plotly_render
+from .core.cppn import (
+    Point2D, Point3D,
+    CPPN, CPPN2D, CPPN3D)
+from .core.ann import ANN2D, ANN3D
+
 from .core.config import Config
-from .core.genome import Genome, GIDManager
+from .core.genome import Genome
 
 try:  # pragma: no cover
     # __package__ allows for the case where __name__ is "__main__"
     __version__ = importlib.metadata.version(__package__ or __name__)
 except importlib.metadata.PackageNotFoundError:  # pragma: no cover
     __version__ = "0.0.0"
 
 
-__all__ = ['Genome', 'ANN', 'Config', 'Point', 'GIDManager', 'CPPN',
-           'plotly_render']
+__all__ = ['Genome',
+           'CPPN',
+           'Point2D', 'CPPN2D', 'ANN2D',
+           'Point3D', 'CPPN3D', 'ANN3D',
+           'Config']
```

### Comparing `abrain-1.0rc0.post5/src/abrain/_bindings/genotype.cpp` & `abrain-1.0rc0.post7/src/abrain/_bindings/genotype.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -10,103 +10,116 @@
 #include "pybind11/stl_bind.h"
 PYBIND11_MAKE_OPAQUE(std::vector<kgd::eshn::genotype::CPPNData::Node>)
 PYBIND11_MAKE_OPAQUE(std::vector<kgd::eshn::genotype::CPPNData::Link>)
 
 using namespace kgd::eshn::genotype;
 namespace kgd::eshn::pybind {
 
-static const utils::DocMap _cppn_doc {
-  { "INPUTS",  "Number of inputs for the CPPN"  },
-  { "OUTPUTS", "Number of outputs for the CPPN" },
-};
-
 py::dict to_json (const CPPNData &d) {
   py::dict dict;
   py::list nodes, links;
-  for (auto &n: d.nodes)  nodes.append(py::make_tuple(n.id, n.func));
-  for (auto &l: d.links)
-    links.append(py::make_tuple(l.id, l.src, l.dst, l.weight));
+  for (const auto &[id, func]: d.nodes)  nodes.append(py::make_tuple(id, func));
+  for (const auto &[id, src, dst, weight]: d.links)
+    links.append(py::make_tuple(id, src, dst, weight));
+  dict["inputs"] = d.inputs;
+  dict["outputs"] = d.outputs;
+  dict["bias"] = d.bias;
+  dict["labels"] = d.labels;
   dict["nodes"] = nodes;
   dict["links"] = links;
-  dict["nextNodeID"] = d.nextNodeID;
-  dict["nextLinkID"] = d.nextLinkID;
   return dict;
 }
 
 using Node = CPPNData::Node;
 using Link = CPPNData::Link;
 
-CPPNData from_json (py::dict dict) {
+CPPNData genotype_from_json (const py::dict& dict) {
   CPPNData d;
-  d.nextNodeID = dict["nextNodeID"].cast<int>();
-  d.nextLinkID = dict["nextLinkID"].cast<int>();
+  d.inputs = dict["inputs"].cast<int>();
+  d.outputs = dict["outputs"].cast<int>();
+  d.bias = dict["bias"].cast<bool>();
+  d.labels = dict["labels"].cast<std::string>();
   for (const py::handle &h: dict["nodes"]) {
-    py::tuple t = h.cast<py::tuple>();
+    auto t = h.cast<py::tuple>();
     d.nodes.push_back(Node{t[0].cast<int>(), t[1].cast<std::string>()});
   }
   for (const py::handle &h: dict["links"]) {
-    py::tuple t = h.cast<py::tuple>();
+    auto t = h.cast<py::tuple>();
     d.links.push_back(Link{t[0].cast<int>(),
-                            t[1].cast<uint>(), t[2].cast<uint>(),
+                            t[1].cast<unsigned int>(), t[2].cast<unsigned int>(),
                             t[3].cast<float>()});
   }
   return d;
 }
 
+template <typename T>
+void id_sorted(std::vector<T> &v) {
+  std::sort(v.begin(), v.end(), [] (const T &lhs, const T &rhs) {
+    return lhs.id < rhs.id;
+  });
+}
+
 void init_genotype (py::module_ &m) {
   auto cppn = py::class_<CPPNData>(m, "CPPNData");
   auto node = py::class_<Node>(cppn, "Node");
   auto link = py::class_<Link>(cppn, "Link");
 
   py::bind_vector<std::vector<Node>>(cppn, "Nodes", "Collection of Nodes");
   py::bind_vector<std::vector<Link>>(cppn, "Links", "Collection of Links");
 
 #define ID(X, ...) (#X, &CLASS::X, ##__VA_ARGS__)
 #define CLASS CPPNData
   cppn.doc() = R"(C++ supporting type for genomic data)";
   cppn.def(py::init<>())
-      .def_readonly_static ID(INPUTS, "")
-      .def_readonly_static ID(OUTPUTS)
-      .def_readonly_static("_docstrings", &_cppn_doc)
+      .def_readwrite ID(inputs, "Number of inputs")
+      .def_readwrite ID(outputs, "Number of outputs")
+      .def_readwrite ID(bias, "Whether to use an input bias")
+      .def_readwrite ID(labels, "(optional) label for the inputs/outputs")
       .def_readwrite ID(nodes, "The collection of computing nodes")
       .def_readwrite ID(links, "The collection of inter-node relationships")
-      .def_readwrite ID(nextNodeID, "ID for the next random node (monotonic)")
-      .def_readwrite ID(nextLinkID, "ID for the next random link (monotonic")
+
+      .def(
+        "_sort_by_id",
+        [] (CPPNData &d) {
+          id_sorted(d.nodes);
+          id_sorted(d.links);
+        }, "Ensures both nodes and links are id-sorted")
+
       .def("to_json", to_json, "Convert to a json-compliant Python dictionary")
-      .def_static("from_json", from_json, "j"_a,
+      .def_static("from_json", genotype_from_json, "j"_a,
                   "Convert from the json-compliant Python dictionary `j`")
       .def(py::pickle(
-        [] (const CLASS &d) { return to_json(d); },
-        [](py::dict d) {      return from_json(d);  }
+        [](const CLASS &d) { return to_json(d); },
+        [](const py::dict &d) { return genotype_from_json(d);  }
       ))
       ;
 
 #undef CLASS
 #define CLASS Node
   node.doc() = "Computational node of a CPPN";
   node.def(py::init<int, const Node::FuncID &>())
       .def("__repr__", [] (const Node &n) {
         std::ostringstream oss;
         oss << "N" << n.id << ":" << n.func;
         return oss.str();
       })
-      .def_readwrite ID(id, "Numerical identifier")
+      .def_readwrite ID(id, "Historical marking")
       .def_readwrite ID(func, "Function used to compute");
 
 #undef CLASS
 #define CLASS Link
   link.doc() = "From-to relationship between two computational node";
-  link.def(py::init<int, uint, uint, float>())
+  link.def(py::init<int, unsigned int, unsigned int, float>())
       .def("__repr__", [] (const Link &l) {
         std::ostringstream oss;
         oss << "L" << l.id << ":" << l.src << " -(" << l.weight << ")-> "
             << l.dst;
         return oss.str();
       })
-      .def_readwrite ID(id, "Numerical identifier")
+      .def_readwrite ID(id, "Historical marking")
       .def_readwrite ID(src, "ID of the source node")
       .def_readwrite ID(dst, "ID of the destination node")
       .def_readwrite ID(weight, "Connection weight");
 }
 
 
 } // end of namespace kgd::eshn::pybind
```

### Comparing `abrain-1.0rc0.post5/src/abrain/_bindings/module.cpp` & `abrain-1.0rc0.post7/src/abrain/_bindings/module.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,50 @@
+#include "../_cpp/phenotype/ann.h"
 #include "pybind11/pybind11.h"
 namespace py = pybind11;
 
 namespace kgd::eshn::pybind {
 
 void init_genotype (py::module_ &m);
-void init_cppn_phenotype (py::module_ &m);
-void init_ann_phenotype (py::module_ &m);
+void init_innovations (py::module_ &m);
+
+void init_generic_cppn_phenotype(py::module_ &m);
+
+template <unsigned int DI> void init_point_type (py::module_ &m, const char *name);
+template <typename CPPN> void init_eshn_cppn_phenotype (
+        py::module_ &m, const char *name, const char *pname);
+
+template <typename ANN> void init_ann_phenotype (py::module_ &m, const char *name);
+
 void init_config (py::module_ &m);
 
 PYBIND11_MODULE(_cpp, main) {
   main.doc() = "Docstring main module";
 
+  auto config = main.def_submodule(
+          "config",
+          "Docstring for config submodule");
+  init_config(config);
+
   auto genotype = main.def_submodule(
         "genotype",
         "Docstring for genotype submodule");
   init_genotype(genotype);
+  init_innovations(genotype);
 
   auto phenotype = main.def_submodule(
         "phenotype",
         "Docstring for phenotype submodule");
-  init_cppn_phenotype(phenotype);
-  init_ann_phenotype(phenotype);
-
-  auto config = main.def_submodule(
-        "config",
-        "Docstring for config submodule");
-  init_config(config);
+  init_point_type<2>(phenotype, "Point2D");
+  init_point_type<3>(phenotype, "Point3D");
+  init_generic_cppn_phenotype(phenotype);
+  init_eshn_cppn_phenotype<phenotype::CPPN2D>(phenotype, "CPPN2D", "Point2D");
+  init_eshn_cppn_phenotype<phenotype::CPPN3D>(phenotype, "CPPN3D", "Point3D");
+  init_ann_phenotype<phenotype::ANN2D>(phenotype, "ANN2D");
+  init_ann_phenotype<phenotype::ANN3D>(phenotype, "ANN3D");
 
   auto misc = main.def_submodule(
         "misc",
         "Docstring for phenotype submodule");
 
 #define STRINGIFY(x) #x
 #define MACRO_STRINGIFY(x) STRINGIFY(x)
```

### Comparing `abrain-1.0rc0.post5/src/abrain/_cpp/config.h` & `abrain-1.0rc0.post7/src/abrain/_cpp/config.h`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #ifndef KGD_GENOTYPE_CONFIG_H
 #define KGD_GENOTYPE_CONFIG_H
 
 #include <vector>
-#include <set>
 #include <map>
 
 #include "genotype.h"
 
 namespace kgd::eshn {
 
 template <typename T>
@@ -20,31 +19,37 @@
 
   using FID = genotype::CPPNData::Node::FuncID;
   using Functions = std::vector<FID>;
 
   using FunctionSet = Functions;
   static FunctionSet functionSet;
 
-  using OutputFunctions = Functions;
-  static OutputFunctions outputFunctions;
+  static FID defaultOutputFunction;
+
+  enum ESHNOutputs {
+    WEIGHT, LEO, BIAS
+  };
+
+  using OutputFunctions = std::map<ESHNOutputs, FID>;
+  static OutputFunctions eshnOutputFunctions;
 
   using MutationRates = std::map<std::string, float>;
   static MutationRates mutationRates;
 
   using FBounds = Bounds<float>;
   static FBounds cppnWeightBounds;
 
   /// ================================================
   /// ANN parameters
   static float annWeightsRange;
   static FID activationFunc;
 
   /// ================================================
   /// ES-HyperNEAT parameters
-  static uint initialDepth, maxDepth, iterations;
+  static unsigned int initialDepth, maxDepth, iterations;
   static float divThr, varThr, bndThr;
   static bool allowPerceptrons;
 };
 
 } // end of namespace kgd::eshn
 
 #endif // KGD_GENOTYPE_CONFIG_H
```

### Comparing `abrain-1.0rc0.post5/src/abrain/_cpp/misc/point.hpp` & `abrain-1.0rc0.post7/src/abrain/_cpp/misc/point.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,106 @@
 #ifndef ES_HYPERNEAT_POINT_HPP
 #define ES_HYPERNEAT_POINT_HPP
 
 #include <cmath>
+#include <cstdint>
 #include <sstream>
 #include <array>
 
-#include "constants.h"
-
 namespace kgd::eshn::misc {
 
-template <uint DI, uint DE>
+template <unsigned int DI>
 class Point_t {
-  static_assert(DI > 0, "Null points do not make sense");
-  static_assert(DI > 1, "1D ANNs do not make much sense, right?");
-  static_assert(DI < 4, "n-D ANNs are really not a good idea");
-
-  static constexpr uint MAX_DECIMALS = std::numeric_limits<int>::digits10-1;
-  static_assert(DE <= MAX_DECIMALS,
-                "Cannot represent such precision in fixed point type");
+  using int_t = std::int16_t;
 
-  std::array<int, DI> _data;
+  std::array<int_t, DI> _data;
 
 public:
+  static constexpr auto DECIMALS = std::numeric_limits<int_t>::digits10 - 1;
   static constexpr auto DIMENSIONS = DI;
-  static constexpr auto DECIMALS = DE;
-//   static constexpr int RATIO = std::pow(10, DE);
+
   static constexpr int RATIO = [] {
     int r = 1;
-    for (uint i=0; i<DE; i++) r *= 10;
+    for (unsigned int i=0; i<DECIMALS; i++) r *= 10;
     return r;
   }();
 
   static constexpr float EPSILON = [] {
     float v = 1;
-    for (uint i=0; i<DECIMALS; i++)  v /= 10.f;
+    for (unsigned int i=0; i<DECIMALS; i++)  v /= 10.f;
     return v;
   }();
 
   Point_t(std::initializer_list<float> &&flist) {
-    uint i=0;
-    for (float f: flist) set(i++, f);
+    unsigned int i=0;
+    for (const float f: flist) set(i++, f);
     for (; i<DIMENSIONS; i++) set(i, 0);
   }
 
-  Point_t(void) { set(0); }
+  Point_t() { set(0); }
 
-  static Point_t null (void) { return Point_t(); }
+  static Point_t null () { return Point_t(); }
 
-  float x (void) const {  return get(0); }
+  [[nodiscard]] float x () const {  return get(0); }
 
-  template <uint DI_ = DI>
-  std::enable_if_t<DI_ >= 2, float> y (void) const {
+  [[nodiscard]] float y () const {
     return get(1);
   }
 
-  template <uint DI_ = DI>
-  std::enable_if_t<DI_ >= 3, float> z (void) const {
+  template <unsigned int DI_ = DIMENSIONS>
+  std::enable_if_t<DI_ >= 3, float> z () const {
     return get(2);
   }
 
-  float get (uint i) const {
-    return _data[i] / float(RATIO);
+  [[nodiscard]] float get (unsigned int i) const {
+    return _data[i] / static_cast<float>(RATIO);
   }
 
-  void set (uint i, float v) {
-    _data[i] = int(std::round(RATIO * v));
+  void set (unsigned int i, const float v) {
+    _data[i] = static_cast<int>(std::round(RATIO * v));
   }
 
-  void set (float v) {
-    for (uint i=0; i<DIMENSIONS; i++) set(i, v);
+  void set (const float v) {
+    for (unsigned int i=0; i<DIMENSIONS; i++) set(i, v);
   }
 
-  const auto& data (void) const {
+  const auto& data () const {
     return _data;
   }
 
   Point_t& operator+= (const Point_t &that) {
-    for (uint i=0; i<DIMENSIONS; i++) set(i, get(i) + that.get(i));
+    for (unsigned int i=0; i<DIMENSIONS; i++) set(i, get(i) + that.get(i));
     return *this;
   }
 
   Point_t& operator-= (const Point_t &that) {
-    for (uint i=0; i<DIMENSIONS; i++) set(i, get(i) - that.get(i));
+    for (unsigned int i=0; i<DIMENSIONS; i++) set(i, get(i) - that.get(i));
     return *this;
   }
 
   Point_t& operator/= (float v) {
-    for (uint i=0; i<DIMENSIONS; i++) set(i, get(i) / v);
+    for (unsigned int i=0; i<DIMENSIONS; i++) set(i, get(i) / v);
     return *this;
   }
 
-  float length (void) const {
+  [[nodiscard]] float length () const {
     float sum = 0;
-    for (uint i=0; i<DIMENSIONS; i++) sum += get(i)*get(i);
+    for (unsigned int i=0; i<DIMENSIONS; i++) sum += get(i)*get(i);
     return std::sqrt(sum);
   }
 
   friend Point_t operator- (const Point_t &lhs, const Point_t &rhs) {
     Point_t res;
-    for (uint i=0; i<DIMENSIONS; i++) res.set(i, lhs.get(i) - rhs.get(i));
+    for (unsigned int i=0; i<DIMENSIONS; i++) res.set(i, lhs.get(i) - rhs.get(i));
     return res;
   }
 
   friend Point_t operator* (float v, const Point_t &p) {
     Point_t res;
-    for (uint i=0; i<DIMENSIONS; i++) res.set(i, v * p.get(i));
+    for (unsigned int i=0; i<DIMENSIONS; i++) res.set(i, v * p.get(i));
     return res;
   }
 
   friend bool operator< (const Point_t &lhs, const Point_t &rhs) {
     return lhs._data < rhs._data;
   }
 
@@ -118,30 +110,29 @@
 
   friend bool operator!= (const Point_t &lhs, const Point_t &rhs) {
     return lhs._data != rhs._data;
   }
 
   friend std::ostream& operator<< (std::ostream &os, const Point_t &p) {
     os << p.get(0);
-    for (uint i=1; i<DIMENSIONS; i++)  os << "," << p.get(i);
+    for (unsigned int i=1; i<DIMENSIONS; i++)  os << "," << p.get(i);
     return os;
   }
 
   friend std::istream& operator>> (std::istream &is, Point_t &p) {
     char c;
     float f;
     is >> f;
     p.set(0, f);
-    for (uint i=1; i<DIMENSIONS; i++) {
+    for (unsigned int i=1; i<DIMENSIONS; i++) {
       is >> c >> f;
       p.set(i, f);
     }
     return is;
   }
 };
-using Point2D = Point_t<2, 3>;
-using Point3D = Point_t<3, 3>;
-using Point = Point_t<ESHN_SUBSTRATE_DIMENSION, 3>;
+using Point2D = Point_t<2>;
+using Point3D = Point_t<3>;
 
 } // end of namespace kgd::eshn::misc
 
 #endif // ES_HYPERNEAT_POINT_HPP
```

### Comparing `abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/ann.cpp` & `abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/ann.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,102 @@
 #include <memory>
 #include <cassert>
 #include <algorithm>
 
 #include "../config.h"
+#include "../misc/utils.hpp"
 #include "ann.h"
 
 #include <iostream>
 
 namespace kgd::eshn::phenotype {
 
 #ifndef NDEBUG
 //#define DEBUG_COMPUTE 1
 #endif
 
 #ifndef NDEBUG  // Timing utilities
 using timing_clock = std::chrono::high_resolution_clock;
 using time_point = std::chrono::time_point<timing_clock>;
 
-static time_point t_now(void) { return timing_clock::now(); }
-static ANN::Stats::rep t_diff(time_point start) {
-  return std::chrono::duration_cast<ANN::Stats::duration>(t_now() - start).count();
+static time_point t_now() { return timing_clock::now(); }
+
+template <typename ANN>
+static typename ANN::Stats::rep t_diff(const time_point start) {
+  return std::chrono::duration_cast<typename ANN::Stats::duration>(t_now() - start).count();
 }
 #endif
 
-using Output = CPPN::Output;
-using Point = es::Point;
-
-bool ANN::empty(bool strict) const {
+template <unsigned int DI>
+bool ANN_t<DI>::empty(bool strict) const {
   return strict ? (stats().hidden == 0) : (stats().edges == 0);
 }
 
-bool ANN::perceptron(void) const {
+template <unsigned int DI>
+bool ANN_t<DI>::perceptron() const {
   return (stats().hidden == 0) && stats().edges > 0;
 }
 
-ANN ANN::build (const Coordinates &inputs,
-                const Coordinates &outputs,
-                const genotype::CPPNData &genome) {
+template <unsigned int DI>
+ANN_t<DI> ANN_t<DI>::build (
+    const Coordinates &inputs,
+    const Coordinates &outputs,
+    const genotype::CPPNData &genome) {
+
+  if (genome.inputs < 2*DI + genome.bias || 2*DI + genome.bias + 1 < genome.inputs)
+    throw std::invalid_argument(utils::mergeToString(
+      "Unable to build a ", DI, "D ANN from a genome with ",
+      genome.inputs, " inputs. Did you mix it up with the one for the body?"
+    ));
+  using ANN = ANN_t<DI>;
 
 #ifndef NDEBUG
-//  const auto start_time = t_now();
 const auto start_time = timing_clock::now();
 #endif
 
   static const auto& weightRange = Config::annWeightsRange;
 
   CPPN cppn (genome);
+
   ANN ann;
 
   NeuronsMap &neurons = ann._neurons;
 
   const auto add = [&cppn, &ann] (auto p, auto t) {
     float bias = 0;
     if (t != Neuron::I)
-      bias = cppn(p, Point::null(), Output::Bias);
+      bias = cppn(p, Point::null(), CPPN::Output::BIAS);
     return ann.addNeuron(p, t, bias);
   };
 
-  uint i = 0;
+  unsigned int i = 0;
   ann._inputs.resize(inputs.size());
   ann._ibuffer.resize(inputs.size());
   for (auto &p: inputs) neurons.insert(ann._inputs[i++] = add(p, Neuron::I));
 
   i = 0;
   ann._outputs.resize(outputs.size());
   ann._obuffer.resize(outputs.size());
   for (auto &p: outputs) neurons.insert(ann._outputs[i++] = add(p, Neuron::O));
 
   Coordinates hidden;
-  evolvable_substrate::Connections connections;
+  evolvable_substrate::Connections_t<DI> connections;
   if (evolvable_substrate::connect(cppn, inputs, outputs,
                                    hidden, connections,
                                    ann._stats.iterations)) {
     for (auto &p: hidden) neurons.insert(add(p, Neuron::H));
     for (auto &c: connections)
       ann.neuronAt(c.to)->addLink(c.weight * weightRange, ann.neuronAt(c.from));
   }
 
   ann.computeStats();
 
 #ifndef NDEBUG
-  ann._stats.time.build = t_diff(start_time);
-  ann._stats.time.eval = Stats::rep{0};
+  ann._stats.time.build = t_diff<ANN>(start_time);
+  ann._stats.time.eval = typename ANN::Stats::rep{0};
 #endif
 
   return ann;
 }
 
 // Deepcopy implementation
 // Not used for now
@@ -116,117 +127,144 @@
 //  for (const Neuron::ptr &n: _outputs)
 //    that._outputs.push_back(that.neuronAt(n->pos));
 
 //  // Copy stats
 //  that._stats = _stats;
 //}
 
-void ANN::reset(void) {
+template <unsigned int DI>
+void ANN_t<DI>::reset() {
   for (auto &p: _neurons)   p->reset();
 }
 
-uint computeDepth (ANN &ann) {
+template <unsigned int DI>
+unsigned int ANN_t<DI>::max_hidden_neurons(void) {
+  return std::pow(2, DI*Config::maxDepth);
+}
+
+template <typename ANN>
+unsigned int computeDepth (ANN &ann) {
+  using Neuron = typename ANN::Neuron;
+  using NeuronPtr = typename ANN::NeuronPtr;
+  using Point = typename ANN::Point;
   struct ReverseNeuron {
-    ANN::Neuron &n;
+    Neuron &n;
     std::vector<ReverseNeuron*> o;
-    ReverseNeuron (ANN::Neuron &n) : n(n) {}
+    explicit ReverseNeuron (Neuron &n) : n(n) {}
   };
 
   std::map<Point, ReverseNeuron*> neurons;
   std::set<ReverseNeuron*> next;
 
-  uint hcount = 0, hseen = 0;
-  for (const ANN::Neuron::ptr &n: ann.neurons()) {
+  unsigned int hcount = 0, hseen = 0;
+  for (const NeuronPtr &n: ann.neurons()) {
     auto p = neurons.emplace(std::make_pair(n->pos, new ReverseNeuron(*n)));
-    if (n->type == ANN::Neuron::I) next.insert(p.first->second);
-    else if (n->type == ANN::Neuron::H) hcount++;
+    if (n->type == Neuron::I) next.insert(p.first->second);
+    else if (n->type == Neuron::H) hcount++;
   }
 
-  for (const ANN::Neuron::ptr &n: ann.neurons())
-    for (phenotype::ANN::Neuron::Link &l: n->links())
+  for (const NeuronPtr &n: ann.neurons())
+    for (auto &l: n->links())
       neurons.at(l.in.lock()->pos)->o.push_back(neurons.at(n->pos));
 
   std::set<ReverseNeuron*> seen;
-  uint depth = 0;
+  unsigned int depth = 0;
   while (!next.empty()) {
     auto current = next;
     next.clear();
 
     for (ReverseNeuron *n: current) {
       n->n.depth = depth;
 //      std::cerr << n->n.pos << ": " << depth << "\n";
       seen.insert(n);
-      if (n->n.type == ANN::Neuron::H)  hseen++;
+      if (n->n.type == Neuron::H)  hseen++;
       for (ReverseNeuron *o: n->o) next.insert(o);
     }
 
     decltype(seen) news;
     std::set_difference(next.begin(), next.end(),
                         seen.begin(), seen.end(),
                         std::inserter(news, news.end()));
     next = news;
     assert(hseen == hcount || next.size() > 0);
 
     depth++;
   }
 
-  uint d = 0;
+  unsigned int d = 0;
   for (auto &p: neurons) {
     d = std::max(d, p.second->n.depth);
     delete p.second;
   }
   return d;
 }
 
-void ANN::computeStats(void) {
+template <unsigned int DI>
+void ANN_t<DI>::computeStats() {
+  using Link = typename Neuron::Link;
   auto &e = _stats.edges = 0;
   float &l = _stats.axons = 0;
-  for (const Neuron::ptr &n: _neurons) {
-    e += uint(n->links().size());
-    for (const Neuron::Link &link: n->links())
-      l += (n->pos - link.in.lock()->pos).length();
+
+  float &u = _stats.utility = 0;
+  std::set<Point> connected_inputs;
+
+  for (const NeuronPtr &n: _neurons) {
+    e += static_cast<unsigned int>(n->links().size());
+    for (const Link &link: n->links()) {
+      const auto &_n = link.in.lock();
+      l += (n->pos - _n->pos).length();
+
+      if (_n->type == Neuron::I)
+        connected_inputs.insert(_n->pos);
+    }
+
+    if (n->type == Neuron::O && n->links().size() > 0) u++;
   }
 
-  _stats.hidden = uint(_neurons.size() - _inputs.size() - _outputs.size());
-  _stats.density = _stats.edges;
+  u += connected_inputs.size();
+  u /= float(_inputs.size() + _outputs.size());
+
+  _stats.hidden = static_cast<unsigned int>(_neurons.size() - _inputs.size() - _outputs.size());
+  _stats.density = _stats.edges / float(max_edges());
+
   if (_stats.hidden == 0) {
-    for (Neuron::ptr &n: _inputs)   n->depth = 0;
-    for (Neuron::ptr &n: _outputs)  n->depth = 1;
+    for (NeuronPtr &n: _inputs)   n->depth = 0;
+    for (NeuronPtr &n: _outputs)  n->depth = 1;
     _stats.depth = 1;
-    _stats.density /= _inputs.size() * _outputs.size();
 
-  } else {
+  } else
     _stats.depth = computeDepth(*this);
-    _stats.density /= (_inputs.size() * _stats.hidden + _stats.hidden * _outputs.size());
-  }
 }
 
-ANN::Neuron::ptr ANN::addNeuron(const Point &p, Neuron::Type t, float bias) {
+template <unsigned int DI>
+typename ANN_t<DI>::NeuronPtr
+ANN_t<DI>::addNeuron(const Point &p, typename Neuron::Type t, float bias) {
   return std::make_shared<Neuron>(p, t, bias);
 }
 
-void ANN::operator() (const IBuffer &inputs, OBuffer &outputs, uint substeps) {
+template <unsigned int DI>
+void ANN_t<DI>::operator() (const IBuffer &inputs, OBuffer &outputs, unsigned int substeps) {
 #ifndef NDEBUG
   const auto start_time = t_now();
 #endif
 
   static const auto &activation =
     phenotype::CPPN::functions.at(Config::activationFunc);
   assert(inputs.size() == _inputs.size());
   assert(outputs.size() == outputs.size());
 
-  for (uint i=0; i<inputs.size(); i++) _inputs[i]->value = inputs[i];
+  for (unsigned int i=0; i<inputs.size(); i++) _inputs[i]->value = inputs[i];
 
 #ifdef DEBUG_COMPUTE
   std::cerr << std::setprecision(std::numeric_limits<float>::max_digits10);
   using utils::operator<<;
   std::cerr << "## Compute step --\n inputs:\t" << inputs << "\n";
 #endif
 
-  for (uint s = 0; s < substeps; s++) {
+  for (unsigned int s = 0; s < substeps; s++) {
 #ifdef DEBUG_COMPUTE
     std::cerr << "#### Substep " << s+1 << " / " << substeps << "\n";
 #endif
 
     for (const auto &p: _neurons) {
       if (p->isInput()) continue;
 
@@ -248,20 +286,23 @@
       std::cerr << "      <o " << p->pos << ": " << p->value << " = "
                 << config::EvolvableSubstrate::activationFunc() << "("
                 << v << ")\n";
 #endif
     }
   }
 
-  for (uint i=0; i<_outputs.size(); i++)  outputs[i] = _outputs[i]->value;
+  for (unsigned int i=0; i<_outputs.size(); i++)  outputs[i] = _outputs[i]->value;
 
 #ifdef DEBUG_COMPUTE
   std::cerr << "outputs:\t" << outputs << "\n## --\n";
 #endif
 
 #ifndef NDEBUG
-  _stats.time.eval += t_diff(start_time);
+  _stats.time.eval += t_diff<ANN_t<DI>>(start_time);
 #endif
 
 }
 
+template class ANN_t<2>;
+template class ANN_t<3>;
+
 } // end of namespace kgd::eshn::genotype
```

### Comparing `abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/ann.h` & `abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/ann.h`

 * *Files 18% similar despite different names*

```diff
@@ -9,155 +9,173 @@
 
 #include "cppn.h"
 #include "eshn.h"
 
 namespace kgd::eshn::phenotype {
 namespace es = evolvable_substrate;
 
-class ANN {
+template <unsigned int DI>
+class ANN_t {
 public:
-  using Point = es::Point;
-  static constexpr auto DIMENSIONS = CPPN::DIMENSIONS;
+  using CPPN = CPPN_ND<DI>;
+  using Point = typename CPPN::Point;
+  static constexpr auto DIMENSIONS = DI;
 
   struct Neuron {// : public std::enable_shared_from_this<Neuron> {
     const Point pos;
     enum Type { I, O, H };
     const Type type;
 
     const float bias;
     float value;
 
-    uint depth = 0;
+    unsigned int depth = 0;
 
     // For clustering purposes (bitwise mask)
-    using Flags_t = uint;
+    using Flags_t = unsigned int;
     Flags_t flags;
 
     Neuron (const Point &p, Type t, float b)
       : pos(p), type(t), bias(b), value(0), flags(0) {}
 
-    bool isInput (void) const {   return type == I;  }
-    bool isOutput (void) const {  return type == O; }
-    bool isHidden (void) const {  return type == H; }
+    [[nodiscard]] bool isInput () const {   return type == I;  }
+    [[nodiscard]] bool isOutput () const {  return type == O; }
+    [[nodiscard]] bool isHidden () const {  return type == H; }
 
-    void reset (void) { value = 0;  }
+    void reset () { value = 0;  }
 
     using ptr = std::shared_ptr<Neuron>;
     using wptr = std::weak_ptr<Neuron>;
     struct Link {
       float weight;
       wptr in;
     };
     using Links = std::vector<Link>;
 
-    const Links& links (void) const {   return _ilinks; }
-    Links& links (void) {               return _ilinks; }
+    const Links& links () const {   return _ilinks; }
+    Links& links () {               return _ilinks; }
 
     void addLink (float w, wptr n) {    _ilinks.push_back({w,n});  }
 
-    friend void assertEqual (const Neuron &lhs, const Neuron &rhs,
+    static void assertEqual (const Neuron &lhs, const Neuron &rhs,
                              bool deepcopy);
 
-    friend void assertEqual (const Link &lhs, const Link &rhs, bool deepcopy);
+    static void assertEqual (const Link &lhs, const Link &rhs, bool deepcopy);
 
   private:
     Links _ilinks;
   };
 
   struct Stats {
-    uint depth;
-    uint hidden;
-    uint edges;
-    float axons;  // total length
+    unsigned int depth;
+    unsigned int hidden;
+    unsigned int edges;
+    float axons;    // total length
     float density;
-    uint iterations;
+    float utility;
+    unsigned int iterations;
 #ifndef NDEBUG
     using duration = std::chrono::duration<double>;
     using rep = duration::rep;
     struct {
       rep build; // Construction time
       rep eval; // Evaluation time
     } time;
 #endif
   };
+  using NeuronPtr = typename Neuron::ptr;
 
-  ANN(void) = default;
+  ANN_t() = default;
 
-  const auto& neurons (void) const {  return _neurons;  }
-  auto& neurons (void) {  return _neurons;  }
-
-  const Neuron::ptr& neuronAt (const Point &p) const {
+  const NeuronPtr& neuronAt (const Point &p) const {
     auto it = _neurons.find(p);
     if (it == _neurons.end())
       throw std::invalid_argument("No neuron there");
     return *it;
   }
 
   struct IBuffer : std::vector<float> {};
-  auto& ibuffer (void) { return _ibuffer; }
+  auto& ibuffer () { return _ibuffer; }
 
   struct OBuffer : std::vector<float> {};
-  auto& obuffer (void) { return _obuffer; }
+  auto& obuffer () { return _obuffer; }
 
-  void reset (void);
+  void reset ();
 
   /// TODO Modify with buffer-based eval. Maybe
   /// .. todo:: Modify with buffer-based eval. Maybe
-  void operator() (const IBuffer &inputs, OBuffer &outputs, uint substeps = 1);
+  void operator() (const IBuffer &inputs, OBuffer &outputs, unsigned int substeps = 1);
 
-  bool empty (bool strict = false) const;
-  bool perceptron (void) const;
+  [[nodiscard]] bool empty (bool strict = false) const;
+  [[nodiscard]] bool perceptron () const;
 
-  void computeStats (void);
-  const auto& stats (void) const {
+  void computeStats ();
+  const auto& stats () const {
     return _stats;
   }
 
+  static unsigned int max_hidden_neurons();
+
+  unsigned int max_edges() {
+    if (_stats.hidden == 0)
+      return _inputs.size() * _outputs.size();
+    else
+      return (_inputs.size() * _stats.hidden
+              + _stats.hidden * _stats.hidden
+              + _stats.hidden * _outputs.size());
+  }
+
   // Deepcopy for develop once / use many
   // Not useful yet.
 //  void copyInto (ANN &that) const;
 
-  using Coordinates = es::Coordinates;
-  static ANN build (const Coordinates &inputs,
+  using Coordinates = es::Coordinates_t<DI>;
+  static ANN_t build (const Coordinates &inputs,
                     const Coordinates &outputs,
                     const genotype::CPPNData &genome);
 
 private:
   struct NeuronCMP {
     using is_transparent = void;
     bool operator() (const Point &lhs, const Point &rhs) const {
       if (lhs.y() != rhs.y()) return lhs.y() < rhs.y();
-#if ESHN_SUBSTRATE_DIMENSION == 3
-      if (lhs.z() != rhs.z()) return lhs.z() < rhs.z();
-#endif
+      if constexpr (DIMENSIONS == 3)
+        if (lhs.z() != rhs.z()) return lhs.z() < rhs.z();
       return lhs.x() < rhs.x();
     }
 
-    bool operator() (const Neuron::ptr &lhs, const Point &rhs) const {
+    bool operator() (const NeuronPtr &lhs, const Point &rhs) const {
       return operator()(lhs->pos, rhs);
     }
 
-    bool operator() (const Point &lhs, const Neuron::ptr &rhs) const {
+    bool operator() (const Point &lhs, const NeuronPtr &rhs) const {
       return operator()(lhs, rhs->pos);
     }
 
-    bool operator() (const Neuron::ptr &lhs, const Neuron::ptr &rhs) const {
+    bool operator() (const NeuronPtr &lhs, const NeuronPtr &rhs) const {
       return operator()(lhs->pos, rhs->pos);
     }
   };
 public:
-  using NeuronsMap = std::set<Neuron::ptr, NeuronCMP>;
+  using NeuronsMap = std::set<NeuronPtr, NeuronCMP>;
+
+  const NeuronsMap& neurons () const {  return _neurons;  }
+  NeuronsMap& neurons () {  return _neurons;  }
+
 private:
   NeuronsMap _neurons;
 
-  std::vector<Neuron::ptr> _inputs, _outputs;
+  std::vector<NeuronPtr> _inputs, _outputs;
   IBuffer _ibuffer;
   OBuffer _obuffer;
 
   Stats _stats;
 
-  Neuron::ptr addNeuron (const Point &p, Neuron::Type t, float bias);
+  NeuronPtr addNeuron (const Point &p, typename Neuron::Type t, float bias);
 };
 
+using ANN2D = ANN_t<2>;
+using ANN3D = ANN_t<3>;
+
 } // end of namespace kgd::eshn::phenotype
 
 #endif // KGD_ANN_PHENOTYPE_H
```

### Comparing `abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/cppn.cpp` & `abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/cppn.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 #include <cmath>
 #include <cassert>
 
+#include <iostream>
+
 #include "cppn.h"
 #include "../config.h"
 
-#include <iostream>
-
 #ifndef NDEBUG
 //#define DEBUG_CPPN
+#include <iomanip>
 #endif
 
-#include <iomanip> /// TODO REMOVE
-
 #ifdef DEBUG_CPPN
 #include <iomanip>
 
 namespace utils { // Contains debugging tools
 std::ostream& operator<< (std::ostream &os,
-                         const kgd::eshn::phenotype::CPPN::Outputs &outputs) {
-  os << "[ " << outputs[0];
-  for (uint i=1; i<outputs.size(); i++) os << " " << outputs[i];
+                         const kgd::eshn::phenotype::CPPN::Buffer &buffer) {
+  os << "[ " << buffer[0];
+  for (unsigned int i=1; i<buffer.size(); i++) os << " " << buffer[i];
   return os << "]";
 }
 
-
 /// Manages indentation for provided ostream
 /// \author James Kanze @ https://stackoverflow.com/a/9600752
 class IndentingOStreambuf : public std::streambuf {
-  static constexpr uint DEFAULT_INDENT = 2;   ///< Default indenting value
+  static constexpr unsigned int DEFAULT_INDENT = 2;   ///< Default indenting value
 
   std::ostream*       _owner;   ///< Associated ostream
   std::streambuf*     _buffer;  ///< Associated buffer
   bool                _isAtStartOfLine; ///< Whether to insert indentation
 
   const std::string   _indent;  ///< Indentation value
 
@@ -43,24 +41,23 @@
     _isAtStartOfLine = (ch == '\n');
     return _buffer->sputc(ch);
   }
 
 public:
   /// Creates a proxy buffer managing indentation level
   explicit IndentingOStreambuf(std::ostream& dest,
-                               uint spaces = DEFAULT_INDENT)
+                               unsigned int spaces = DEFAULT_INDENT)
     : _owner(&dest), _buffer(dest.rdbuf()),
       _isAtStartOfLine(true),
       _indent(spaces, ' ' ) { _owner->rdbuf( this );  }
 
   /// Returns control of the buffer to its owner
   virtual ~IndentingOStreambuf(void) { _owner->rdbuf(_buffer); }
 };
 
-
 } // end of namespace utils
 #endif
 
 namespace kgd::eshn::phenotype {
 using CPPNData = kgd::eshn::genotype::CPPNData;
 
 
@@ -68,19 +65,19 @@
 
 // -- Ugly solution to numerical non-determinism
 // Divergences observed on local/remote machines can be solved by requesting
 //  value in double precision (accurate within 1ULP?) and truncating back to
 //  float. Computationally more expensive but ensures bitwise identical CPPN/ANN
 
 float fd_exp(float x) {
-  return (float)static_cast<double(*)(double)>(std::exp)(x);
+  return static_cast<float>(static_cast<double(*)(double)>(std::exp)(x));
 }
 
 float fd_sin(float x) {
-  return (float)static_cast<double(*)(double)>(std::sin)(x);
+  return static_cast<float>(static_cast<double(*)(double)>(std::sin)(x));
 }
 
 #define KGD_EXP fd_exp
 #define KGD_EXP_STR "dexp"
 
 // =============================================================================
 
@@ -137,64 +134,69 @@
 };
 #undef F
 
 // =============================================================================
 
 
 CPPN::CPPN (const CPPNData &genotype) {
-  using NID = uint;//CPPNData::Node::ID;
-  static constexpr auto NI = INPUTS;
-  static constexpr auto NO = OUTPUTS;
-
-  const auto &ofuncs = [] (uint index) {
-    return Config::outputFunctions[index];
-  };
+  using NID = unsigned int;//CPPNData::Node::ID;
+  const auto NI = genotype.inputs;
+  const auto NO = genotype.outputs;
+  const auto NH = genotype.nodes.size() - NO;
 
   auto fnode = [] (const CPPNData::Node::FuncID &fid) {
     return std::make_shared<FNode>(functions.at(fid));
   };
 
   std::map<NID, Node_ptr> nodes;
+#ifdef DEBUG_CPPN
+  std::cerr << "Building CPPN with " << NI << " inputs, " << NO << " outputs,"
+            << " and " << NH << " internal nodes" << std::endl;
+#endif
+
+  _has_input_bias = genotype.bias;
 
-  uint off = 0; // Inputs are first
   _inputs.resize(NI);
+  _outputs.resize(NO);
+  _hidden.resize(NH);
+
+  _ibuffer = IBuffer(n_inputs(false));
+  _obuffer = OBuffer(NO);
+
   for (NID i=0; i<NI; i++) {
 #ifdef DEBUG_CPPN
     std::cerr << "(I) " << NID(i) << " " << i << std::endl;
 #endif
     nodes[i] = _inputs[i] = std::make_shared<INode>();
   }
 
-  off = NI; // Outputs are after inputs
-  _outputs.resize(NO);
   for (NID i=0; i<NO; i++) {
+    const auto [id, func] = genotype.nodes[i];
 #ifdef DEBUG_CPPN
-    std::cerr << "(O) " << i+off << " " << i << " " << ofuncs(i) << std::endl;
+    std::cerr << "(O) " << i+NI << " " << i << " " << func << std::endl;
 #endif
-    nodes[i+off] = _outputs[i] = fnode(ofuncs(i));
+    nodes[id] = _outputs[i] = fnode(func);
   }
 
-  uint i=0;
-  _hidden.resize(genotype.nodes.size());
-  for (const CPPNData::Node &n_g: genotype.nodes) {
+  for (NID i=NO; i<genotype.nodes.size(); i++) {
+    const auto [id, func] = genotype.nodes[i];
 #ifdef DEBUG_CPPN
-    std::cerr << "(H) " << n_g.id << " " << i << " " << n_g.func << std::endl;
+    std::cerr << "(H) " << id << " " << i << " " << func << std::endl;
 #endif
-    nodes[n_g.id] = _hidden[i] = fnode(n_g.func);
-    i++;
+    nodes[id] = _hidden[i-NO] = fnode(func);
   }
 
-  for (const CPPNData::Link &l_g: genotype.links) {
-    FNode &n = dynamic_cast<FNode&>(*nodes.at(l_g.dst));
+  for (const auto &l_g: genotype.links) {
+    auto &n = dynamic_cast<FNode&>(*nodes.at(l_g.dst));
     n.links.push_back({l_g.weight, nodes.at(l_g.src)});
   }
 
 #ifdef DEBUG_CPPN
-  i=0;
-  std::map<Node_ptr, uint> map;
+  unsigned int i=0;
+  std::map<Node_ptr, unsigned int> map;
   printf("Built CPPN:\n");
   for (const auto &v: {_inputs, _outputs, _hidden})
     for (const Node_ptr &n: v)
       map[n] = i++;
 
   for (const auto &v: {_hidden, _outputs}) {
     for (const Node_ptr &n: v) {
@@ -202,32 +204,33 @@
       printf("\t[%d]\n", map.at(n));
       std::string fname (functionToName.at(fn.func));
       printf("\t\t%s\n", fname.c_str());
       for (const Link &l: fn.links)
         printf("\t\t[%d]\t%g %a\n", map.at(l.node.lock()), l.weight, l.weight);
     }
   }
+  printf("--\n");
 #endif
 }
 
-float CPPN::INode::value (void) {
+float CPPN::INode::value () {
 #ifdef DEBUG_CPPN
   utils::IndentingOStreambuf indent (std::cout);
   std::cout << "I: " << data << std::endl;
 #endif
   return data;
 }
 
-float CPPN::FNode::value (void) {
+float CPPN::FNode::value () {
 #ifdef DEBUG_CPPN
   utils::IndentingOStreambuf indent (std::cout);
   std::cout << "F:\n";
 #endif
   if (std::isnan(data)) {
-    data = 0;
+    data = 0.f;
     for (Link &l: links)
       data += l.weight * l.node.lock()->value();
 
 #ifdef DEBUG_CPPN
     auto val = func(data);
     std::cout << val << " = " << functionToName.at(func)
               << "(" << data << ")\n";
@@ -249,75 +252,117 @@
 std::ostream& operator<< (std::ostream &os, const std::vector<float> &v) {
   os << "[";
   for (float f: v)  os << " " << f;
   return os << " ]";
 }
 #endif
 
-void CPPN::pre_evaluation(const Point &src, const Point &dst) {
-  static constexpr auto N = DIMENSIONS;
-  for (uint i=0; i<N; i++)  _inputs[i]->data = src.get(i);
-  for (uint i=0; i<N; i++)  _inputs[i+N]->data = dst.get(i);
-
-#if ESHN_WITH_DISTANCE
-  static const float norm = float(2*std::sqrt(2));
-  _inputs[2*N]->data = (src - dst).length() / norm;
-#endif
+void CPPN::pre_evaluation(const IBuffer &inputs) {
+  if (inputs.size() != n_inputs())
+    throw std::runtime_error("Invalid number of inputs");
+  for (unsigned int i=0; i<_inputs.size(); i++) _inputs[i]->data = inputs[i];
+  common_pre_evaluation();
+}
 
-  _inputs.back()->data = 1;
+void CPPN::common_pre_evaluation() {
+  if (_has_input_bias)
+    _inputs.back()->data = 1;
 
-  for (auto &n: _hidden)  n->data = NAN;
-  for (auto &n: _outputs)  n->data = NAN;
+  for (const auto &n: _hidden)  n->data = NAN;
+  for (const auto &n: _outputs)  n->data = NAN;
 
 #ifdef DEBUG_CPPN
   utils::IndentingOStreambuf indent (std::cout);
   std::cout << "compute step\n\tInputs:"
             << std::setprecision(std::numeric_limits<float>::max_digits10);
   for (auto &i: _inputs) std::cout << " " << i->data;
   std::cout << "\n";
 #endif
 }
 
-void CPPN::operator() (const Point &src, const Point &dst,
-                       Outputs &outputs) {
+void CPPN::operator() (OBuffer &outputs, const IBuffer &inputs) {
+  pre_evaluation(inputs);
+  for (unsigned int i=0; i<outputs.size(); i++)
+    outputs[i] = _outputs[i]->value();
+}
+
+float CPPN::operator() (unsigned int o, const IBuffer &inputs) {
+  pre_evaluation(inputs);
+  return _outputs[o]->value();
+}
+
+
+// =============================================================================
+
+template <unsigned int DI>
+CPPN_ND<DI>::CPPN_ND(const Genotype &genotype) : CPPN(genotype) {}
+template CPPN_ND<2>::CPPN_ND(const Genotype &genotype);
+template CPPN_ND<3>::CPPN_ND(const Genotype &genotype);
+
+template <unsigned int DI>
+void CPPN_ND<DI>::pre_evaluation(const CPPN_ND<DI>::Point &src,
+                                 const CPPN_ND<DI>::Point &dst) {
+  static constexpr auto N = DIMENSIONS;
+  const auto I = n_inputs(true);
+  for (unsigned int i=0; i<N; i++)  _inputs[i]->data = src.get(i);
+  for (unsigned int i=0; i<N; i++)  _inputs[i+N]->data = dst.get(i);
+
+  static const auto norm = static_cast<float>(2*std::sqrt(2));
+  if (I - static_cast<int>(_has_input_bias) > 2*N)
+    _inputs[2*N]->data = (src - dst).length() / norm;
+
+  common_pre_evaluation();
+}
+
+template <unsigned int DI>
+void CPPN_ND<DI>::operator() (const Point &src, const Point &dst, OBuffer &outputs) {
   assert(outputs.size() == _outputs.size());
 
   pre_evaluation(src, dst);
-  for (uint i=0; i<outputs.size(); i++) outputs[i] = _outputs[i]->value();
+  for (unsigned int i=0; i<outputs.size(); i++) outputs[i] = _outputs[i]->value();
 
 #ifdef DEBUG_CPPN
   using utils::operator<<;
   std::cout << outputs << "\n" << std::endl;
 #endif
 }
+template void CPPN_ND<2>::operator() (const Point &src, const Point &dst, OBuffer &outputs);
+template void CPPN_ND<3>::operator() (const Point &src, const Point &dst, OBuffer &outputs);
 
-void CPPN::operator() (const Point &src, const Point &dst, Outputs &outputs,
-                       const OutputSubset &oset) {
+template <unsigned int DI>
+void CPPN_ND<DI>::operator() (
+    const Point &src, const Point &dst,
+    OBuffer &outputs,
+    const OutputSubset &oset) {
   assert(outputs.size() == _outputs.size());
   assert(oset.size() <= _outputs.size());
 
   pre_evaluation(src, dst);
-  for (auto o: oset) outputs[uint(o)] = _outputs[uint(o)]->value();
+  for (const auto o: oset) outputs[o] = _outputs[o]->value();
 
 #ifdef DEBUG_CPPN
   using utils::operator<<;
   std::cout << outputs << "\n" << std::endl;
 #endif
 }
+template void CPPN_ND<2>::operator() (const Point &src, const Point &dst, OBuffer &outputs, const OutputSubset &oset);
+template void CPPN_ND<3>::operator() (const Point &src, const Point &dst, OBuffer &outputs, const OutputSubset &oset);
+
 
 // Hopefully will get rid of i686 float c++ -> python transfer errors
 #if __i386__
 #pragma GCC push_options
 #pragma GCC optimize ("O0")
 #endif
-float CPPN::operator() (const Point &src, const Point &dst,
-                        CPPNData::Output o) {
+template <unsigned int DI>
+float CPPN_ND<DI>::operator() (const Point &src, const Point &dst, const Output o) {
   pre_evaluation(src, dst);
     
-  float v =  _outputs[uint(o)]->value();
-  return v;
+  return _outputs[o]->value();
 }
+template float CPPN_ND<2>::operator() (const Point &src, const Point &dst, Output o);
+template float CPPN_ND<3>::operator() (const Point &src, const Point &dst, Output o);
 #if __i386__
 #pragma GCC pop_options
 #endif
 
 } // end of namespace kgd::eshn::phenotype
```

### Comparing `abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/eshn.cpp` & `abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/eshn.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,430 +1,444 @@
 #include <iostream>
 #include <algorithm>
 #include <queue>
 
 #include "eshn.h"
 
-#include "../config.h"
 #include "ann.h"
 
 namespace kgd::eshn::evolvable_substrate {
 
-using ANN = phenotype::ANN;
-using Point = ANN::Point;
-using Coordinates = phenotype::ANN::Coordinates;
-using Coordinates_s = std::set<Coordinates::value_type>;
-
-using Output = CPPN::Output;
-
-struct QOTreeNode {
-  Point center;
-  float radius;
-  uint level;
-  float weight;
-
-  using ptr = std::shared_ptr<QOTreeNode>;
-  std::vector<ptr> cs;
-
-  QOTreeNode (const Point &p, float r, uint l)
-    : center(p), radius(r), level(l), weight(NAN) {}
-
-#if ESHN_SUBSTRATE_DIMENSION == 2
-  QOTreeNode (float x, float y, float r, uint l)
-    : QOTreeNode({x,y}, r, l) {}
-#elif ESHN_SUBSTRATE_DIMENSION == 3
-  QOTreeNode (float x, float y, float z, float r, uint l)
-    : QOTreeNode({x,y,z}, r, l) {}
-#endif
-
-  float variance (void) const {
-    if (cs.empty()) return 0;
-    float mean = 0;
-    for (auto &c: cs) mean += c->weight;
-    mean /= cs.size();
-    float var = 0;
-    for (auto &c: cs) var += float(std::pow(c->weight - mean, 2));
-    return var / cs.size();
-  }
+template <unsigned int D>
+struct ESHN {
+  using Point = misc::Point_t<D>;
+  using CPPN = phenotype::CPPN_ND<D>;
+  using ANN = phenotype::ANN_t<D>;
+
+  using Coordinates = typename ANN::Coordinates;
+  using Coordinates_s = std::set<typename Coordinates::value_type>;
+
+  using Connection = Connection_t<D>;
+  using Connections = Connections_t<D>;
+
+  using Output = typename CPPN::Output;
+
+  struct QOTreeNode {
+    Point center;
+    float radius;
+    unsigned int level;
+    float weight;
+
+    using ptr = std::shared_ptr<QOTreeNode>;
+    std::vector<ptr> cs;
+
+    QOTreeNode (const Point &p, const float r, const unsigned int l)
+      : center(p), radius(r), level(l), weight(NAN) {}
+
+    QOTreeNode (float x, float y, float r, unsigned int l) requires (D == 2)
+      : QOTreeNode({x,y}, r, l) {}
+
+    QOTreeNode (float x, float y, float z, float r, unsigned int l) requires (D == 3)
+      : QOTreeNode({x,y,z}, r, l) {}
+
+    [[nodiscard]] float variance () const {
+      if (cs.empty()) return 0;
+      float mean = 0;
+      for (auto &c: cs) mean += c->weight;
+      mean /= cs.size();
+      float var = 0;
+      for (auto &c: cs) var += static_cast<float>(std::pow(c->weight - mean, 2));
+      return var / cs.size();
+    }
 
 #if DEBUG_ES_QUADTREE
-  friend std::ostream& operator<< (std::ostream &os, const QuadTreeNode &n) {
-    utils::IndentingOStreambuf indent (os);
-    os << "QTN " << n.center << " " << n.radius << " " << n.level << " "
-              << n.weight << "\n";
-    for (const auto &c: n.cs) os << *c;
-    return os;
-  }
+    friend std::ostream& operator<< (std::ostream &os, const QuadTreeNode &n) {
+      utils::IndentingOStreambuf indent (os);
+      os << "QTN " << n.center << " " << n.radius << " " << n.level << " "
+                << n.weight << "\n";
+      for (const auto &c: n.cs) os << *c;
+      return os;
+    }
 #endif
-};
-using QOTree = QOTreeNode::ptr;
+  };
+  using QOTree = typename QOTreeNode::ptr;
 
-// =============================================================================
-// Debug streamers
+  // =============================================================================
+  // Debug streamers
 
 #if DEBUG_ES >= 3  // Only in deep debug
-std::ostream& operator<< (std::ostream &os, const Coordinates_s &c) {
-  os << "[";
-  if (c.size() >= 1) {
-    os << " " << *c.begin() << " ";
-    for (auto it = std::next(c.begin()); it != c.end(); ++it) os << *it << " ";
+  std::ostream& operator<< (std::ostream &os, const Coordinates_s &c) {
+    os << "[";
+    if (c.size() >= 1) {
+      os << " " << *c.begin() << " ";
+      for (auto it = std::next(c.begin()); it != c.end(); ++it) os << *it << " ";
+    }
+    return os << "]";
   }
-  return os << "]";
-}
 
-void showConnections(std::ostream &os, const Connections &c, size_t start = 0) {
-  auto it = c.begin();
-  std::advance(it, start);
-  for (; it != c.end(); ++it) os << "\t" << *it << "\n";
-}
+  void showConnections(std::ostream &os, const Connections &c, size_t start = 0) {
+    auto it = c.begin();
+    std::advance(it, start);
+    for (; it != c.end(); ++it) os << "\t" << *it << "\n";
+  }
 #endif
 
-// Triggered by duplicate coordinates
-std::ostream& operator<< (std::ostream &os, const Coordinates &c) {
-  os << "[";
-  if (c.size() >= 1) os << " " << c[0] << " ";
-  for (uint i=1; i<c.size(); i++) os << c[i] << " ";
-  return os << "]";
-}
+  // =============================================================================
 
-// =============================================================================
+  template <typename... ARGS>
+  static QOTree node (ARGS... args) {
+    return std::make_shared<QOTreeNode>(args...);
+  }
 
-template <typename... ARGS>
-QOTreeNode::ptr node (ARGS... args) {
-  return std::make_shared<QOTreeNode>(args...);
-}
+  static QOTree divisionAndInitialisation(CPPN &cppn, const Point &p, bool out) {
+    static const auto &initialDepth = Config::initialDepth;
+    static const auto &maxDepth = Config::maxDepth;
+    static const auto &divThr = Config::divThr;
 
-QOTree divisionAndInitialisation(CPPN &cppn, const Point &p, bool out) {
-  static const auto &initialDepth = Config::initialDepth;
-  static const auto &maxDepth = Config::maxDepth;
-  static const auto &divThr = Config::divThr;
-
-  QOTree root = node(Point::null(), 1.f, 1);
-  std::queue<QOTreeNode*> q;
-  q.push(root.get());
+    QOTree root = node(Point::null(), 1.f, 1);
+    std::queue<QOTreeNode*> q;
+    q.push(root.get());
 
-  const auto weight = [&cppn] (const Point &p0, const Point &p1) {
-    return cppn(p0, p1, Output::Weight);
-  };
+    const auto weight = [&cppn] (const Point &p0, const Point &p1) {
+      return cppn(p0, p1, Output::WEIGHT);
+    };
 
 #if DEBUG_QUADTREE_DIVISION
-  std::cout << "divisionAndInitialisation(" << p << ", " << out << ")\n";
+    std::cout << "divisionAndInitialisation(" << p << ", " << out << ")\n";
 #endif
 
-  while (!q.empty()) {
-    QOTreeNode &n = *q.front();
-    q.pop();
+    while (!q.empty()) {
+      QOTreeNode &n = *q.front();
+      q.pop();
 
-    float cx = n.center.x(), cy = n.center.y();
-#if ESHN_SUBSTRATE_DIMENSION == 3
-    float cz = n.center.z();
-#endif
-    float hr = .5 * n.radius;
-    float nl = float(n.level) + 1;
+      n.cs.resize(1 << D);
+      unsigned int i=0;
 
-    n.cs.resize(1 << ESHN_SUBSTRATE_DIMENSION);
-    uint i=0;
-    for (int x: {-1,1})
-      for (int y: {-1, 1})
-#if ESHN_SUBSTRATE_DIMENSION == 2
-        n.cs[i++] = node(cx + x * hr, cy + y * hr, hr, nl);
-#elif ESHN_SUBSTRATE_DIMENSION == 3
-        for (int z: {-1,1})
-          n.cs[i++] = node(cx + x * hr, cy + y * hr, cz + z * hr, hr, nl);
-#endif
+      const float hr = .5 * n.radius;
+      const float nl = static_cast<float>(n.level) + 1;
+      const auto &nc = n.center;
+      if constexpr (D == 2) {
+        const float cx = nc.x(), cy = nc.y();
+        for (const float x: {-1.f, 1.f})
+          for (const float y: {-1.f, 1.f})
+            n.cs[i++] = node(cx + x * hr, cy + y * hr, hr, nl);
+
+      } else if (D == 3) {
+        const float cx = nc.x(), cy = nc.y(), cz = nc.z();
+        for (const float x: {-1.f, 1.f})
+          for (const float y: {-1.f, 1.f})
+            for (const float z: {-1.f, 1.f})
+                n.cs[i++] = node(cx + x * hr, cy + y * hr, cz + z * hr, hr, nl);
 
-    for (auto &c: n.cs)
-      c->weight = out ? weight(p, c->center) : weight(c->center, p);
+      }
+
+      for (auto &c: n.cs)
+        c->weight = out ? weight(p, c->center) : weight(c->center, p);
 
 #if DEBUG_QUADTREE_DIVISION
-    std::string indent (2*n.level, ' ');
-    std::cout << indent << n.center << ", r=" << n.radius << ", l=" << n.level
-              << ":";
-    for (auto &c: n.cs) std::cout << " " << c->weight;
-    std::cout << "\n" << indent << "> var = " << n.variance() << "\n";
+      std::string indent (2*n.level, ' ');
+      std::cout << indent << n.center << ", r=" << n.radius << ", l=" << n.level
+                << ":";
+      for (auto &c: n.cs) std::cout << " " << c->weight;
+      std::cout << "\n" << indent << "> var = " << n.variance() << "\n";
 #endif
 
-    if (n.level < initialDepth || (n.level < maxDepth && n.variance() > divThr))
-      for (auto &c: n.cs) q.push(c.get());
-  }
+      if (n.level < initialDepth || (n.level < maxDepth && n.variance() > divThr))
+        for (auto &c: n.cs) q.push(c.get());
+    }
 
 #if DEBUG_ES_QUADTREE
-  std::cerr << *root;
+    std::cerr << *root;
 #endif
 
 #if DEBUG_QUADTREE
-  quadtree_debug::debugGenerateImages(*root, p, !out);
+    quadtree_debug::debugGenerateImages(*root, p, !out);
 #endif
 
-  return root;
-}
+    return root;
+  }
 
-void pruneAndExtract (CPPN &cppn, const Point &p, Connections &con,
-                      const QOTree &t, bool out) {
+  static void pruneAndExtract (
+          CPPN &cppn, const Point &p, Connections &con,
+          const QOTree &t, bool out) {
 
-  static const auto &varThr = Config::varThr;
-  static const auto &bndThr = Config::bndThr;
-  static const auto leo = [] (auto &cppn, auto i, auto o) {
-    return (bool)cppn(i, o, Output::LEO);
-  };
+    static const auto &varThr = Config::varThr;
+    static const auto &bndThr = Config::bndThr;
+    static const auto leo = [] (auto &_cppn, auto i, auto o) {
+      return static_cast<bool>(_cppn(i, o, Output::LEO));
+    };
 
 #if DEBUG_QUADTREE_PRUNING
-  if (t->level == 1)  std::cout << "\n---\n";
-  utils::IndentingOStreambuf indent (std::cout);
-  std::cout << "pruneAndExtract(" << p << ", " << t->center << ", "
-            << t->radius << ", " << t->level << ", " << out << ") {\n";
+    if (t->level == 1)  std::cout << "\n---\n";
+    utils::IndentingOStreambuf indent (std::cout);
+    std::cout << "pruneAndExtract(" << p << ", " << t->center << ", "
+              << t->radius << ", " << t->level << ", " << out << ") {\n";
 #endif
 
-  for (auto &c: t->cs) {
+    for (auto &c: t->cs) {
 #if DEBUG_QUADTREE_PRUNING
-    utils::IndentingOStreambuf indent1 (std::cout);
-    std::cout << "processing " << c->center << "\n";
-    utils::IndentingOStreambuf indent2 (std::cout);
+      utils::IndentingOStreambuf indent1 (std::cout);
+      std::cout << "processing " << c->center << "\n";
+      utils::IndentingOStreambuf indent2 (std::cout);
 #endif
 
-    if (c->variance() >= varThr) {
-      // More information at lower resolution -> explore
+      if (c->variance() >= varThr) {
+        // More information at lower resolution -> explore
 #if DEBUG_QUADTREE_PRUNING
-      std::cout << "a> " << c->variance() << " >= " << varThr
-                << " >> digging\n";
+        std::cout << "a> " << c->variance() << " >= " << varThr
+                  << " >> digging\n";
 #endif
-      pruneAndExtract(cppn, p, con, c, out);
-
-    } else {
-      // Not enough information at lower resolution -> test if part of band
+        pruneAndExtract(cppn, p, con, c, out);
 
-      float r = c->radius;
-      float bnd = 0;
-
-      float cx = c->center.x(), cy = c->center.y();
-      const auto dweight = [&cppn, &p, &c, out] (auto... coords) {
-        Point src = out ? p : Point{coords...},
-              dst = out ? Point{coords...} : p;
-        return std::fabs(c->weight
-                         - cppn(src, dst, Output::Weight));
-      };
-
-
-#if ESHN_SUBSTRATE_DIMENSION == 2
-      bnd = std::max(
-        std::min(dweight(cx-r, cy), dweight(cx+r, cy)),
-        std::min(dweight(cx, cy-r), dweight(cx, cy+r))
-      );
-
-#elif ESHN_SUBSTRATE_DIMENSION == 3
-      float cz = c->center.z();
-      std::vector<float> bnds {
-        std::min(dweight(cx-r, cy, cz), dweight(cx+r, cy, cz)),
-        std::min(dweight(cx, cy-r, cz), dweight(cx, cy+r, cz)),
-        std::min(dweight(cx, cy, cz-r), dweight(cx, cy, cz+r))
-      };
-      bnd = *std::max_element(bnds.begin(), bnds.end());
+      } else {
+        // Not enough information at lower resolution -> test if part of band
 
-#endif
+        float r = c->radius;
+        float bnd = 0;
+
+        float cx = c->center.x(), cy = c->center.y();
+        const auto dweight = [&cppn, &p, &c, out] (auto... coords) {
+          Point src = out ? p : Point{coords...},
+                dst = out ? Point{coords...} : p;
+          return std::fabs(c->weight
+                           - cppn(src, dst, Output::WEIGHT));
+        };
+
+        if constexpr (D == 2) {
+          bnd = std::max(
+            std::min(dweight(cx-r, cy), dweight(cx+r, cy)),
+            std::min(dweight(cx, cy-r), dweight(cx, cy+r))
+          );
+
+        } else {
+          float cz = c->center.z();
+          std::vector<float> bnds {
+            std::min(dweight(cx-r, cy, cz), dweight(cx+r, cy, cz)),
+            std::min(dweight(cx, cy-r, cz), dweight(cx, cy+r, cz)),
+            std::min(dweight(cx, cy, cz-r), dweight(cx, cy, cz+r))
+          };
+          bnd = *std::ranges::max_element(bnds.begin(), bnds.end());
+        }
 
 #if DEBUG_QUADTREE_PRUNING
-      std::cout << "b> var = " << c->variance() << ", bnd = "
-                << std::max(std::min(dl, dr), std::min(dt, db))
-                << " = max(min(" << dl << ", " << dr << "), min(" << dt
-                << ", " << db << ")) && leo = "
-                << leoConnection(cppn, out ? p : c->center, out ? c->center : p)
-                << "\n";
+        std::cout << "b> var = " << c->variance() << ", bnd = "
+                  << std::max(std::min(dl, dr), std::min(dt, db))
+                  << " = max(min(" << dl << ", " << dr << "), min(" << dt
+                  << ", " << db << ")) && leo = "
+                  << leoConnection(cppn, out ? p : c->center, out ? c->center : p)
+                  << "\n";
 #endif
 
-      if (bnd > bndThr
-          && leo(cppn, out ? p : c->center, out ? c->center : p)
-          && c->weight != 0) {
-        con.insert({
-          out ? p : c->center, out ? c->center : p, c->weight
-        });
+        if (bnd > bndThr
+            && leo(cppn, out ? p : c->center, out ? c->center : p)
+            && c->weight != 0) {
+          con.insert({
+            out ? p : c->center, out ? c->center : p, c->weight
+          });
 #if DEBUG_QUADTREE_PRUNING
-        std::cout << " < created " << (out ? p : c->center) << " -> "
-                  << (out ? c->center : p) << " [" << c->weight << "]\n";
+          std::cout << " < created " << (out ? p : c->center) << " -> "
+                    << (out ? c->center : p) << " [" << c->weight << "]\n";
 #endif
+        }
       }
     }
-  }
 
 #if DEBUG_QUADTREE_PRUNING
-  std::cout << "}\n";
+    std::cout << "}\n";
 #endif
-}
+  }
 
-void removeUnconnectedNeurons (const Coordinates &inputs,
-                               const Coordinates &outputs,
-                               Coordinates_s &shidden,
-                               Connections &connections) {
-  using Type = ANN::Neuron::Type;
+  using Type = typename ANN::Neuron::Type;
   struct L;
   struct N {
-    Point p;
-    Type t;
-    std::vector<L> i, o;
-    N (const Point &p, Type t = Type::H) : p(p), t(t) {}
+      Point p;
+      Type t;
+      std::vector<L> i, o;
+      explicit N (const Point &p, Type t = Type::H) : p(p), t(t) {}
   };
   struct L {
-    N *n;
-    float w;
+      N *n;
+      float w;
+      explicit L (N *n, const float w) : n(n), w(w) {}
   };
   struct CMP {
-    using is_transparent = void;
-    bool operator() (const N *lhs, const Point &rhs) const {
-      return lhs->p < rhs;
-    }
-    bool operator() (const Point &lhs, const N *rhs) const {
-      return lhs < rhs->p;
-    }
-    bool operator() (const N *lhs, const N *rhs) const {
-      return lhs->p < rhs->p;
-    }
-  };
-
-  std::set<N*, CMP> nodes, inodes, onodes;
-  for (const Point &p: inputs)
-    nodes.insert(*inodes.insert(new N(p, Type::I)).first);
-  for (const Point &p: outputs)
-    nodes.insert(*onodes.insert(new N(p, Type::O)).first);
-
-  const auto getOrCreate = [&nodes] (const Point &p) {
-    auto it = nodes.find(p);
-    if (it != nodes.end())  return *it;
-    else                    return *nodes.insert(new N(p)).first;
+      using is_transparent [[maybe_unused]] = void;
+      bool operator() (const N *lhs, const Point &rhs) const {
+        return lhs->p < rhs;
+      }
+      bool operator() (const Point &lhs, const N *rhs) const {
+        return lhs < rhs->p;
+      }
+      bool operator() (const N *lhs, const N *rhs) const {
+        return lhs->p < rhs->p;
+      }
   };
-  for (const Connection &c: connections) {
-    N *i = getOrCreate(c.from), *o = getOrCreate(c.to);
-    i->o.push_back({o,c.weight});
-    o->i.push_back({i,c.weight});
-  }
-
-#if DEBUG_ES >= 2
-  std::cerr << "\ninodes:\n";
-  for (const auto &n: inodes) std::cerr << "\t" << n->p << "\n";
-  std::cerr << "\nonodes:\n";
-  for (const auto &n: onodes) std::cerr << "\t" << n->p << "\n";
-  std::cerr << "\nconnections:\n";
-  for (const auto &c: connections)
-    std::cerr << "\t" << c.from << " -> " << c.to << "\n";
-  std::cerr << "\n";
-#endif
-
-  const auto breadthFirstSearch =
-      [] (const auto &src, auto &set, auto field) {
-    std::queue<N*> q;
-    typename std::remove_reference_t<decltype(set)> seen;
-    for (const auto &n: src)  q.push(n), seen.insert(n);
-    while (!q.empty()) {
-      N *n = q.front();
-      q.pop();
 
-      for (auto &l: n->*field) {
-        N *n_ = l.n;
-        if (seen.find(n_) == seen.end()) {
-          if (n_->t == Type::H) set.insert(n_);
-          seen.insert(n_);
-          q.push(n_);
-        }
-      }
+  static void removeUnconnectedNeurons (
+      const Coordinates &inputs, const Coordinates &outputs,
+      Coordinates_s &shidden, Connections &connections) {
+
+    std::set<N*, CMP> nodes, inodes, onodes;
+    for (const Point &p: inputs)
+      nodes.insert(*inodes.insert(new N(p, Type::I)).first);
+    for (const Point &p: outputs)
+      nodes.insert(*onodes.insert(new N(p, Type::O)).first);
+
+    const auto getOrCreate = [&nodes] (const Point &p) {
+      auto it = nodes.find(p);
+      if (it != nodes.end())
+        return *it;
+      return *nodes.insert(new N(p)).first;
+    };
+    for (const Connection &c: connections) {
+      N *i = getOrCreate(c.from), *o = getOrCreate(c.to);
+      i->o.push_back(L(o, c.weight));
+      o->i.push_back(L(i, c.weight));
     }
-  };
 
-  std::set<N*, CMP> iseen, oseen;
-  breadthFirstSearch(inodes, iseen, &N::o);
-  breadthFirstSearch(onodes, oseen, &N::i);
+#if DEBUG_ES >= 2
+    std::cerr << "\ninodes:\n";
+    for (const auto &n: inodes) std::cerr << "\t" << n->p << "\n";
+    std::cerr << "\nonodes:\n";
+    for (const auto &n: onodes) std::cerr << "\t" << n->p << "\n";
+    std::cerr << "\nconnections:\n";
+    for (const auto &c: connections)
+      std::cerr << "\t" << c.from << " -> " << c.to << "\n";
+    std::cerr << "\n";
+#endif
+
+    const auto breadthFirstSearch =
+        [] (const auto &src, auto &set, auto field) {
+          std::queue<N*> q;
+          typename std::remove_reference_t<decltype(set)> seen;
+          for (const auto &n: src)  q.push(n), seen.insert(n);
+          while (!q.empty()) {
+            N *n = q.front();
+            q.pop();
+
+            for (auto &l: n->*field) {
+              if (N *n_ = l.n; seen.find(n_) == seen.end()) {
+                if (n_->t == Type::H) set.insert(n_);
+                seen.insert(n_);
+                q.push(n_);
+              }
+            }
+          }
+    };
+
+    std::set<N*, CMP> iseen, oseen;
+    breadthFirstSearch(inodes, iseen, &N::o);
+    breadthFirstSearch(onodes, oseen, &N::i);
 
 #if DEBUG_ES >= 2
-  std::cerr << "hidden nodes:\n\tiseen:\n";
-  for (const auto *n: iseen)  std::cerr << "\t\t" << n->p << "\n";
-  std::cerr << "\n\toseen:\n";
-  for (const auto *n: oseen)  std::cerr << "\t\t" << n->p << "\n";
-  std::cerr << "\n";
+    std::cerr << "hidden nodes:\n\tiseen:\n";
+    for (const auto *n: iseen)  std::cerr << "\t\t" << n->p << "\n";
+    std::cerr << "\n\toseen:\n";
+    for (const auto *n: oseen)  std::cerr << "\t\t" << n->p << "\n";
+    std::cerr << "\n";
 #endif
 
-  CMP cmp;
-  std::vector<N*> hiddenNodes;
-  std::set_intersection(iseen.begin(), iseen.end(), oseen.begin(), oseen.end(),
-                        std::back_inserter(hiddenNodes), cmp);
+    CMP cmp;
+    std::vector<N*> hiddenNodes;
+    std::set_intersection(iseen.begin(), iseen.end(), oseen.begin(), oseen.end(),
+                          std::back_inserter(hiddenNodes), cmp);
 
-  connections.clear();
-  for (const N *n: hiddenNodes) {
+    connections.clear();
+    for (const N *n: hiddenNodes) {
 #if DEBUG_ES >= 3
-    std::cerr << "\t" << n->p << "\n";
+      std::cerr << "\t" << n->p << "\n";
 #endif
-    shidden.insert(n->p);
-    for (const L &l: n->i)  connections.insert({l.n->p, n->p, l.w});
-    for (const L &l: n->o)
-      if (l.n->t == Type::O)
-        connections.insert({n->p, l.n->p, l.w});
-  }
+      shidden.insert(n->p);
+      for (const L &l: n->i)  connections.insert({l.n->p, n->p, l.w});
+      for (const L &l: n->o)
+        if (l.n->t == Type::O)
+          connections.insert({n->p, l.n->p, l.w});
+    }
 
-  for (auto it=nodes.begin(); it!=nodes.end();) {
-    delete *it;
-    it = nodes.erase(it);
+    for (auto it=nodes.begin(); it!=nodes.end();) {
+      delete *it;
+      it = nodes.erase(it);
+    }
   }
-}
 
-/// Collect new hidden nodes and connections
-void collect (const Connections &newConnections, Connections &connections,
-              Coordinates_s &hiddens, Coordinates_s &newHiddens) {
-  for (auto &c: newConnections) {
-    auto r = hiddens.insert(c.to);
-    if (r.second) newHiddens.insert(c.to);
+  /// Collect new hidden nodes and connections
+  static void collect (const Connections &newConnections, Connections &connections,
+                       Coordinates_s &hiddens, Coordinates_s &newHiddens) {
+    for (auto &c: newConnections) {
+      auto r = hiddens.insert(c.to);
+      if (r.second) newHiddens.insert(c.to);
+    }
+    connections.insert(newConnections.begin(), newConnections.end());
   }
-  connections.insert(newConnections.begin(), newConnections.end());
-}
 
-/// Query for direct input-output connections
-void generatePerceptron(CPPN &cppn,
-                        const Coordinates &inputs, const Coordinates &outputs,
-                        Connections &connections) {
-
-  CPPN::OutputSubset wl {{ Output::Weight, Output::LEO }};
-  CPPN::Outputs res;
-
-  for (const Point &i: inputs) {
-    for (const Point &o: outputs) {
-      cppn(i, o, res, wl);
-      if (res[uint(Output::LEO)])
-        connections.insert({i, o, res[uint(Output::Weight)]});
+  /// Query for direct input-output connections
+  static void generatePerceptron(CPPN &cppn,
+                                 const Coordinates &inputs, const Coordinates &outputs,
+                                 Connections &connections) {
+
+    typename CPPN::OutputSubset wl {{ Output::WEIGHT, Output::LEO }};
+    auto res = cppn.obuffer();
+
+    for (const Point &i: inputs) {
+      for (const Point &o: outputs) {
+        cppn(i, o, res, wl);
+        if (res[static_cast<unsigned int>(Output::LEO)])
+          connections.insert({i, o, res[static_cast<unsigned int>(Output::WEIGHT)]});
+      }
     }
   }
+};
+
+// Triggered by duplicate coordinates
+template <unsigned int D>
+std::ostream& operator<< (std::ostream &os, const Coordinates_t<D> &c) {
+  os << "[";
+  if (!c.empty()) os << " " << c[0] << " ";
+  for (unsigned int i=1; i<c.size(); i++) os << c[i] << " ";
+  return os << "]";
 }
 
-bool connect (CPPN &cppn,
-              const Coordinates &inputs, const Coordinates &outputs,
-              Coordinates &hidden, Connections &connections, uint &iterations) {
+template <unsigned int D>
+bool connect (phenotype::CPPN_ND<D> &cppn,
+              const Coordinates_t<D> &inputs, const Coordinates_t<D> &outputs,
+              Coordinates_t<D> &hidden, Connections_t<D> &connections, unsigned int &iterations) {
+
+  using E = ESHN<D>;
+  using Coordinates_s = typename E::Coordinates_s;
+  using Connections = typename E::Connections;
+  using Point = typename E::Point;
 
   static const auto &max_iterations = Config::iterations;
 
   Coordinates_s sio;  // All fixed positions
   for (const auto &vec: {inputs, outputs}) {
     for (Point p: vec) {
-      auto r = sio.insert(p);
-      if (!r.second) {
+      if (const auto r = sio.insert(p); !r.second) {
         std::cerr << "inputs: " << inputs << "\noutputs: " << outputs
                   << std::endl;
         throw std::invalid_argument("Unable to insert duplicate coordinate ");
       }
     }
   }
 
 #if DEBUG_ES
   std::ostringstream oss;
   oss << "\n## --\nStarting evolvable substrate instantiation\n";
-  uint n_hidden = 0, n_connections = 0;
+  unsigned int n_hidden = 0, n_connections = 0;
 #endif
 
   Coordinates_s shidden;
 
   for (const Point &p: inputs) {
     Connections tmpConnections;
-    auto t = divisionAndInitialisation(cppn, p, true);
-    pruneAndExtract(cppn, p, tmpConnections, t, true);
+    auto t = E::divisionAndInitialisation(cppn, p, true);
+    E::pruneAndExtract(cppn, p, tmpConnections, t, true);
 
     Coordinates_s newHiddens;
-    collect(tmpConnections, connections, shidden, newHiddens);
+    E::collect(tmpConnections, connections, shidden, newHiddens);
   }
 
 #if DEBUG_ES
   oss << "[I -> H] found " << shidden.size() - n_hidden << " hidden neurons";
 #if DEBUG_ES >= 3
   oss << "\n\t" << shidden << "\n";
 #endif
@@ -442,17 +456,17 @@
   bool converged = false;
   Coordinates_s unexploredHidden = shidden;
   for (iterations = 0; iterations<max_iterations && !converged; iterations++) {
 
     Coordinates_s newHiddens;
     for (const Point &p: unexploredHidden) {
       Connections tmpConnections;
-      auto t = divisionAndInitialisation(cppn, p, true);
-      pruneAndExtract(cppn, p, tmpConnections, t, true);
-      collect(tmpConnections, connections, shidden, newHiddens);
+      auto t = E::divisionAndInitialisation(cppn, p, true);
+      E::pruneAndExtract(cppn, p, tmpConnections, t, true);
+      E::collect(tmpConnections, connections, shidden, newHiddens);
     }
 
     unexploredHidden = newHiddens;
 
 #if DEBUG_ES
   oss << "[H -> H] found " << shidden.size() - n_hidden
       << " hidden neurons (" << unexploredHidden.size() << " to explore)";
@@ -475,16 +489,16 @@
     if (converged)
       oss << "\t> Premature convergence at iteration " << i << "\n";
 #endif
   }
 
   for (const Point &p: outputs) {
     Connections tmpConnections;
-    auto t = divisionAndInitialisation(cppn, p, false);
-    pruneAndExtract(cppn, p, tmpConnections, t, false);
+    auto t = E::divisionAndInitialisation(cppn, p, false);
+    E::pruneAndExtract(cppn, p, tmpConnections, t, false);
     connections.insert(tmpConnections.begin(), tmpConnections.end());
   }
 
 #if DEBUG_ES
   oss << "[H -> O] found " << connections.size() - n_connections
       << " connections";
 #if DEBUG_ES >= 3
@@ -492,15 +506,15 @@
   showConnections(oss, connections, n_connections);
   oss << "\n";
 #endif
   oss << "\n";
 #endif
 
   Coordinates_s shidden2;
-  removeUnconnectedNeurons(inputs, outputs, shidden2, connections);
+  E::removeUnconnectedNeurons(inputs, outputs, shidden2, connections);
 
 #if DEBUG_ES
   oss << "[Filtrd] total " << shidden2.size() << " hidden neurons";
 #if DEBUG_ES >= 3
   oss << "\n\t" << shidden2 << "\n";
 #endif
   oss << " and " << connections.size() << " connections";
@@ -510,17 +524,35 @@
   oss << "\n";
 #endif
 #endif
 
   std::copy(shidden2.begin(), shidden2.end(), std::back_inserter(hidden));
 
   if (hidden.empty() && Config::allowPerceptrons)
-    generatePerceptron(cppn, inputs, outputs, connections);
+    E::generatePerceptron(cppn, inputs, outputs, connections);
 
 #if DEBUG_ES
   std::cerr << oss.str() << std::endl;
 #endif
 
   return true;
 }
 
+using namespace phenotype;
+template struct ESHN<2>;
+template struct ESHN<3>;
+
+template bool connect<2>(
+        phenotype::CPPN2D &cppn,
+        const Coordinates_t<2> &inputs,
+        const Coordinates_t<2> &outputs,
+        Coordinates_t<2> &hidden,
+        Connections_t<2> &connections, unsigned int &iterations);
+
+template bool connect<3>(
+        phenotype::CPPN3D &cppn,
+        const Coordinates_t<3> &inputs,
+        const Coordinates_t<3> &outputs,
+        Coordinates_t<3> &hidden,
+        Connections_t<3> &connections, unsigned int &iterations);
+
 } // end of namespace evolvable substrate
```

### Comparing `abrain-1.0rc0.post5/src/abrain/_cpp/phenotype/eshn.h` & `abrain-1.0rc0.post7/src/abrain/_cpp/phenotype/eshn.h`

 * *Files 11% similar despite different names*

```diff
@@ -24,34 +24,38 @@
 void debugGenerateImages (const phenotype::evolvable_substrate::QuadTreeNode &t,
                           const phenotype::ANN::Point &p, bool in);
 /// Set where to store debug (a lot of) files
 const stdfs::path& debugFilePrefix (const stdfs::path &path = "");
 }
 #endif
 
-struct Connection {
-  kgd::eshn::phenotype::CPPN::Point from, to;
-  float weight;
+template <unsigned int D>
+struct Connection_t {
+  using Point = typename misc::Point_t<D>;
+  Point from{}, to{};
+  float weight{};
 #if DEBUG_ES
   friend std::ostream& operator<< (std::ostream &os, const Connection &c) {
     return os << "{ " << c.from << " -> " << c.to << " [" << c.weight << "]}";
   }
 #endif
-  friend bool operator< (const Connection &lhs, const Connection &rhs) {
+  friend bool operator< (const Connection_t &lhs, const Connection_t &rhs) {
     if (lhs.from != rhs.from) return lhs.from < rhs.from;
     return lhs.to < rhs.to;
   }
 };
-using Connections = std::set<Connection>;
 
-using CPPN = kgd::eshn::phenotype::CPPN;
-using Point = CPPN::Point;
-using Coordinates = std::vector<Point>;
-
-bool connect (CPPN &cppn,
-              const Coordinates &inputs, const Coordinates &outputs,
-              Coordinates &hidden, Connections &connections,
-              uint &iterations);
+template <unsigned int D>
+using Connections_t = std::set<Connection_t<D>>;
+
+template <unsigned int D>
+using Coordinates_t = std::vector<misc::Point_t<D>>;
+
+template <unsigned int D>
+bool connect (phenotype::CPPN_ND<D> &cppn,
+              const Coordinates_t<D> &inputs, const Coordinates_t<D> &outputs,
+              Coordinates_t<D> &hidden, Connections_t<D> &connections,
+              unsigned int &iterations);
 
 } // end of namespace kgd::eshn::evolvable_substrate
 
 #endif // KGD_EVOLV_SUBSTRATE_H
```

### Comparing `abrain-1.0rc0.post5/src/abrain/core/ann.py` & `abrain-1.0rc0.post7/src/abrain/core/ann.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,64 @@
 import math
 from itertools import chain
 from pathlib import Path
 from typing import Optional, Dict, List, Iterable, Union
 
 import plotly.graph_objects as go
 
-from .._cpp.phenotype import ANN, Point
+from .._cpp.phenotype import (ANN2D, Point2D, CPPN2D,
+                              ANN3D, Point3D, CPPN3D)
 
 logger = logging.getLogger(__name__)
 
 
-def plotly_render(ann: ANN, labels: Optional[Dict[Point, str]] = None) \
+_ANN = Union[ANN2D, ANN3D]
+_Point = Union[Point2D, Point3D]
+
+
+ANN2D.Point = Point2D
+ANN2D.CPPN = CPPN2D
+ANN3D.Point = Point3D
+ANN3D.CPPN = CPPN3D
+
+
+def plotly_render(ann: ANN3D, labels: Optional[Dict[Point3D, str]] = None,
+                  edges_alpha=1.0) \
         -> go.Figure:
     """
     Produce a 3D figure from an artificial neural network
 
     The returned figure can be used to save an interactive html session or a
     (probably poorly) rendering to e.g. a png file
+
+    :param ann: The neural network to render
+    :param labels: The names to use for the neurons
+    :param edges_alpha: The alpha value to use for the edges
     """
 
-    return _figure(data=[_edges(ann), _neurons(ann, labels)])
+    return _figure(data=[_edges(ann, alpha=edges_alpha),
+                         _neurons(ann, labels)])
 
 
-def _iter_neurons(ann: ANN):
+ANN3D.render3D = plotly_render
+
+
+def _iter_neurons(ann: _ANN):
     for n in ann.neurons():
         yield n
 
 
-def _iter_axons(ann: ANN):
+def _iter_axons(ann: _ANN):
     for dst in ann.neurons():
         for link in dst.links():
             yield link, link.src(), dst
 
 
 class ANNMonitor:
-    def __init__(self, ann: ANN, labels: Optional[Dict[Point, str]],
+    def __init__(self, ann: _ANN, labels: Optional[Dict[_Point, str]],
                  folder: Path,
                  neurons_file: Optional[Union[Path, str]],
                  dynamics_file: Optional[Union[Path, str]],
                  dt: Optional[float] = None):
         self.ann = ann
 
         self.labels = labels
@@ -103,22 +123,17 @@
                             v_min = v
                         if v_max < v:
                             v_max = v
                 v_min = min([v_min, -v_min, v_max, -v_max])
                 return [v_min, -v_min]
 
             nv_min, nv_max = c_range(self.neurons_data.data)
-            # print(f"[kgd-debug] {nv_min=}, {nv_max=}")
-
             ew_min, ew_max = c_range(
                 [link.weight for link, _, _ in _iter_axons(self.ann)])
-            # print(f"[kgd-debug] {ew_min=}, {ew_max=}")
-
             ev_min, ev_max = c_range(self.axonal_data.data)
-            # print(f"[kgd-debug] {ev_min=}, {ev_max=}")
 
             frames = [
                 go.Frame(
                     data=[_neurons(self.ann, self.labels, data=n_row,
                                    cmin=nv_min, cmax=nv_max),
                           _edges(self.ann, data=a_row,
                                  wmin=ew_min, wmax=ew_max,
@@ -184,19 +199,19 @@
 
             interactive_plot_file = self.axonal_data_file.with_suffix(".html")
             fig.write_html(interactive_plot_file,
                            auto_play=False)
             logger.info(f"Generated {interactive_plot_file}")
 
 
-def _neurons(ann: ANN, labels: Dict[Point, str],
+def _neurons(ann: _ANN, labels: Dict[_Point, str],
              data: Optional[Iterable[float]] = None,
              **kwargs) -> go.Scatter3d:
     # noinspection PyPep8Naming
-    NT = ANN.Neuron.Type
+    NT = ann.Neuron.Type
 
     x, y, z = zip(*[n.pos.tuple() for n in _iter_neurons(ann)])
     names = []
     types = {NT.I: "Input", NT.H: "Hidden", NT.O: "Output"}
     n_types = {t: 0 for t in types}
     for n in _iter_neurons(ann):
         if labels is None or (label := labels.get(n.pos, None)) is None:
@@ -241,32 +256,33 @@
             hovertemplate='<br>'.join(hover_items) + "<extra></extra>",
             customdata=custom_data,
             hovertext=names,
             **kwargs
         )
 
 
-def _edges(ann: ANN, data: Optional[Iterable[float]] = None,
+def _edges(ann: _ANN, data: Optional[Iterable[float]] = None,
+           alpha=1.0,
            **kwargs) -> go.Scatter3d:
 
-    if ann.stats().edges == 0:
+    if ann.stats().edges == 0:  # pragma: no cover
         return go.Scatter3d()
 
     x, y, z = (
         list(chain.from_iterable(lst)) for lst in
         zip(*[zip(*(src.pos.tuple(), dst.pos.tuple(), (None, None, None)))
               for _, src, dst in _iter_axons(ann)]))
     # w = [link.weight for link, _, _ in _iter_axons(ann)]
 
     c_min, c_max = kwargs.pop("cmin", None), kwargs.pop("cmax", None)
     _, _ = kwargs.pop("wmin", None), kwargs.pop("wmax", None)
 
     lines = dict(width=1)
     if data is None:
-        lines['color'] = "black"
+        lines['color'] = f"rgba(0, 0, 0, {alpha})"
     else:
         # for (link, src, dst), v in zip(_iter_axons(ann), data):
         #     x0, y0, z0 = src.pos.tuple()
         #     x1, y1, z1 = dst.pos.tuple()
         #     print(f"({x0:+.3f}, {y0:+.3f}, {z0:+.3f})"
         #           f" -> ({x1:+.3f}, {y1:+.3f}, {z1:+.3f})"
         #           f" [w={link.weight:+.3f}, v={v:+.3f}]")
```

### Comparing `abrain-1.0rc0.post5/src/abrain/core/config.py` & `abrain-1.0rc0.post7/src/abrain/core/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 import json
 import logging
 import pprint
 from pathlib import Path
 from typing import Optional, Dict
 
-from .._cpp.config import Config as CPPConfig
-from .._cpp.phenotype import CPPN
+# noinspection PyUnresolvedReferences
+from .._cpp.config import (Config as CPPConfig,
+                           OutputFunctions as _OutputFunctions,
+                           MutationRates as _MutationRates,
+                           )
 
 logger = logging.getLogger(__name__)
 
 
 class Config(CPPConfig):
     """
     Wrapper for the C++ configuration data
 
     Allows transparent access to the values used for CPPN structure,
     genome mutation (:func:`Genome.mutate`), and ANN/ES-HyperNEAT parameters
     """
 
+    OutputFunctions = _OutputFunctions
+    MutationRates = _MutationRates
+
     #: The set of all wrapped C++ values
     _dict = {
         k: v for k, v in CPPConfig.__dict__.items() if not k.startswith('_')
     }
 
     #: Private reference to the config sections
     _sections = CPPConfig.__dict__['_sections']
 
     @classmethod
     def to_json(cls) -> Dict:
         """
         Convert to a json-compliant Python dictionary
         """
         dct = {}
-
         for section, items in cls._sections.items():
             dct[section] = {}
             for k in items:
                 attr = getattr(cls, k)
                 if hasattr(attr, "toJson"):
                     attr = attr.toJson()
                 dct[section][k] = attr
 
+        pprint.pprint(dct)
+
         return dct
 
     @classmethod
     def from_json(cls, j: Dict):
         """
         Restore values from a json-compliant Python dictionary
 
@@ -106,28 +113,16 @@
 
         if not path.exists():
             raise IOError(f"Input path '{path}' does not exist")
 
         with open(path, 'r') as f:
             cls.from_json(json.load(f))
 
-        # Then check relationship assertions
-        if not cls.known_function(cls.activationFunc):
-            raise ValueError(f"Activation function {cls.activationFunc}"
-                             f" is unknown")
-
-        for func in cls.functionSet:
-            if not cls.known_function(func):
-                raise ValueError(f"CPPN internal function {func} is unknown")
-
-        for func in cls.outputFunctions:
-            if not cls.known_function(func):
-                raise ValueError(f"CPPN output function {func} is unknown")
-
-        if len(cls.outputFunctions) != CPPN.OUTPUTS:
-            raise ValueError(f"Invalid number of output functions in"
-                             f" {cls.outputFunctions}. CPPN requires"
-                             f" {CPPN.OUTPUTS}")
-
-        # Let us assume I am careful enough for the other values
+        try:
+            # Delegate relationship tests to the C++
+            Config.test_valid()
+        except ValueError as e:
+            raise ValueError("C++ layer exception when checking"
+                             " the provided configuration") \
+                from e
 
         return path
```

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/abs.png` & `abrain-1.0rc0.post7/src/abrain/core/functions/abs.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/abs.svg` & `abrain-1.0rc0.post7/src/abrain/core/functions/abs.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/bsgm.png` & `abrain-1.0rc0.post7/src/abrain/core/functions/bsgm.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/bsgm.svg` & `abrain-1.0rc0.post7/src/abrain/core/functions/bsgm.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/gaus.png` & `abrain-1.0rc0.post7/src/abrain/core/functions/gaus.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/gaus.svg` & `abrain-1.0rc0.post7/src/abrain/core/functions/gaus.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/id.png` & `abrain-1.0rc0.post7/src/abrain/core/functions/id.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/id.svg` & `abrain-1.0rc0.post7/src/abrain/core/functions/id.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/plotter.sh` & `abrain-1.0rc0.post7/src/abrain/core/functions/plotter.sh`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/sin.png` & `abrain-1.0rc0.post7/src/abrain/core/functions/sin.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/sin.svg` & `abrain-1.0rc0.post7/src/abrain/core/functions/sin.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/ssgm.png` & `abrain-1.0rc0.post7/src/abrain/core/functions/ssgm.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/ssgm.svg` & `abrain-1.0rc0.post7/src/abrain/core/functions/ssgm.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/ssgn.png` & `abrain-1.0rc0.post7/src/abrain/core/functions/ssgn.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/ssgn.svg` & `abrain-1.0rc0.post7/src/abrain/core/functions/ssgn.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/step.png` & `abrain-1.0rc0.post7/src/abrain/core/functions/step.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/step.svg` & `abrain-1.0rc0.post7/src/abrain/core/functions/step.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain/core/functions/template.tex` & `abrain-1.0rc0.post7/src/abrain/core/functions/template.tex`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0.post5/src/abrain.egg-info/PKG-INFO` & `abrain-1.0rc0.post7/src/abrain.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abrain
-Version: 1.0rc0.post5
+Version: 1.0rc0.post7
 Summary: NeuroEvolution in Python backed by C++ computations
 Author-email: Kevin Godin-Dubois <k.j.m.godin-dubois@vu.nl>
 Project-URL: Homepage, https://github.com/kgd-al/abrain
 Project-URL: Documentation, https://abrain.rtfd.io
 Project-URL: Bug Tracker, https://github.com/kgd-al/abrain/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C++
@@ -24,18 +24,26 @@
 Requires-Dist: pyrecord
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-steps; extra == "tests"
 Requires-Dist: pytest-sugar; extra == "tests"
 Requires-Dist: coverage; extra == "tests"
 Requires-Dist: flake8; extra == "tests"
+Provides-Extra: all-tests
+Requires-Dist: abrain[kaleido,tests]; extra == "all-tests"
+Requires-Dist: leap-ec; extra == "all-tests"
+Requires-Dist: Pillow; extra == "all-tests"
+Requires-Dist: qdpy; extra == "all-tests"
+Requires-Dist: tqdm; extra == "all-tests"
+Requires-Dist: matplotlib; extra == "all-tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-pyproject; extra == "docs"
 Requires-Dist: sphinx_design; extra == "docs"
+Requires-Dist: sphinx-tabs; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Provides-Extra: kaleido
 Requires-Dist: kaleido; extra == "kaleido"
```

### Comparing `abrain-1.0rc0.post5/src/abrain.egg-info/SOURCES.txt` & `abrain-1.0rc0.post7/src/abrain.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,31 +8,35 @@
 src/abrain.egg-info/PKG-INFO
 src/abrain.egg-info/SOURCES.txt
 src/abrain.egg-info/dependency_links.txt
 src/abrain.egg-info/requires.txt
 src/abrain.egg-info/top_level.txt
 src/abrain/_bindings/config.cpp
 src/abrain/_bindings/genotype.cpp
+src/abrain/_bindings/innovations.cpp
 src/abrain/_bindings/module.cpp
 src/abrain/_bindings/utils.hpp
 src/abrain/_bindings/phenotype/ann.cpp
 src/abrain/_bindings/phenotype/cppn.cpp
 src/abrain/_cpp/config.cpp
 src/abrain/_cpp/config.h
 src/abrain/_cpp/genotype.h
-src/abrain/_cpp/misc/constants_template.h
+src/abrain/_cpp/innovations.cpp
+src/abrain/_cpp/innovations.h
 src/abrain/_cpp/misc/point.hpp
+src/abrain/_cpp/misc/utils.hpp
 src/abrain/_cpp/phenotype/ann.cpp
 src/abrain/_cpp/phenotype/ann.h
 src/abrain/_cpp/phenotype/cppn.cpp
 src/abrain/_cpp/phenotype/cppn.h
 src/abrain/_cpp/phenotype/eshn.cpp
 src/abrain/_cpp/phenotype/eshn.h
 src/abrain/core/ann.py
 src/abrain/core/config.py
+src/abrain/core/cppn.py
 src/abrain/core/genome.py
 src/abrain/core/functions/abs.png
 src/abrain/core/functions/abs.svg
 src/abrain/core/functions/bsgm.png
 src/abrain/core/functions/bsgm.svg
 src/abrain/core/functions/gaus.png
 src/abrain/core/functions/gaus.svg
@@ -48,8 +52,10 @@
 src/abrain/core/functions/step.png
 src/abrain/core/functions/step.svg
 src/abrain/core/functions/template.tex
 tests/test_ann.py
 tests/test_config.py
 tests/test_cppn.py
 tests/test_evolution.py
-tests/test_genome.py
+tests/test_examples.py
+tests/test_genome.py
+tests/test_innovations.py
```

### Comparing `abrain-1.0rc0.post5/tests/test_ann.py` & `abrain-1.0rc0.post7/tests/test_ann.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,83 @@
 import logging
 import math
 from random import Random
 from time import perf_counter
-from typing import Tuple, List, Dict
+from typing import Tuple, List, Dict, Union, Callable
 
 import pytest
 
-from abrain import Point, Config, Genome, ANN, plotly_render
+from abrain import Config, Genome, Point2D, Point3D, ANN2D, ANN3D
 from abrain.core.ann import ANNMonitor
 from abrain.core.genome import logger as genome_logger
 
+ANN = Union[ANN2D, ANN3D]
+Point = Union[Point2D, Point3D]
 
-def test_default_is_empty():
-    ann = ANN()
-    assert ann.empty()
-    assert len(ann.ibuffer()) == 0
-    assert len(ann.obuffer()) == 0
 
-    stats = ann.stats()
-    assert stats.depth == 0
-    assert stats.edges == 0
-    assert stats.axons == 0
+def _ann_type(dimension):
+    if dimension == 2:
+        return ANN2D
+    else:
+        return ANN3D
+
 
+def test_default_is_empty(dimension):
+    # No default constructor
+    with pytest.raises(TypeError):
+        _ann_type(dimension)()
+
+    ann, _, _ = _make_ann(dimension, 0, 0)
     with pytest.raises(ValueError):
-        p0 = Point(0, 0, 0)
-        print("Testing no point at", p0)
-        ann.neuronAt(p0)
+        ann.neuronAt(ann.Point.null())
 
 
-def _make_ann(mutations, rng, other_inputs=None, other_outputs=None) -> \
+def _make_ann(dimension, mutations, seed,
+              other_inputs=None, other_outputs=None) -> \
         Tuple[ANN, List[Point], List[Point]]:
-    genome = Genome.random(rng)
+
+    data = Genome.Data.create_for_eshn_cppn(dimension=dimension,
+                                            seed=seed)
+    genome = Genome.random(data)
     for _ in range(mutations):
-        genome.mutate(rng)
+        genome.mutate(data)
+
+    rng = data.rng
+    ann_t = _ann_type(dimension)
 
     def d(): return rng.randint(10, 20)
     def c(): return rng.uniform(-1, 1)
-    def p(y): return Point(c(), y, c())
+
+    if dimension == 2:
+        def p(y): return ann_t.Point(c(), rng.uniform(.8*y, y))
+    else:
+        def p(y): return ann_t.Point(c(), y, c())
 
     def append(lhs, rhs):
         if rhs is not None:
-            lhs += [Point(x, y, z) for x, y, z in rhs]
+            lhs.extend(rhs)
 
     inputs = [p(-1) for _ in range(d())]
     append(inputs, other_inputs)
 
     outputs = [p(1) for _ in range(d())]
     append(outputs, other_outputs)
 
-    return ANN.build(inputs, outputs, genome), inputs, outputs
+    return ann_t.build(inputs, outputs, genome), inputs, outputs
 
 
-def test_empty_perceptrons(mutations, seed):
+# Force both dimensions to be tested even with small scale test
+@pytest.mark.parametrize('_dimension', [2, 3])
+def test_empty_perceptrons(_dimension, mutations, seed):
     n = 10
 
     def generate_stats():
-        rng = Random(seed)
         l_stats: Dict = {key: 0 for key in ['empty', 'perceptron', 'ann']}
         for _ in range(n):
-            ann, _, _ = _make_ann(mutations, rng)
+            ann, _, _ = _make_ann(_dimension, mutations, seed)
             l_stats['empty'] += ann.empty()
             l_stats['perceptron'] += ann.perceptron()
             l_stats['ann'] += (not ann.empty(strict=True))
             assert not ann.empty() or ann.empty(strict=True)
             assert not ann.perceptron() or ann.empty(strict=True)
             assert not (ann.empty() and ann.perceptron())
             assert not ann.perceptron() or Config.allowPerceptrons
@@ -87,44 +102,112 @@
 
     for s in [stats_t, stats_f]:
         assert (sum(s.values()) == n)
     assert stats_t['empty'] <= stats_f['empty']
     assert stats_f['perceptron'] == 0
 
 
+@pytest.mark.parametrize('_dimension', [2, 3])
+def test_invalid_genome(_dimension):
+    ann_t = _ann_type(_dimension)
+    genome = Genome.random(Genome.Data.create_for_generic_cppn(2, 2))
+    with pytest.raises(ValueError):
+        ann_t.build([], [], genome)
+
+    genome = Genome.random(Genome.Data.create_for_eshn_cppn(5 - _dimension))
+    with pytest.raises(ValueError):
+        print()
+        ann_t.build([], [], genome)
+
+
 @pytest.mark.parametrize(
-    'inputs, outputs',
+    'i, o',
     [
-        pytest.param([(0, 0, 0), (0, 0, 0)], [(1, 1, 1)], id="in"),
-        pytest.param([(1, 1, 1)], [(0, 0, 0), (0, 0, 0)], id="out"),
-        pytest.param([(0, 0, 0)], [(0, 0, 0)], id="io"),
+        pytest.param([0, 0], [1], id="in"),
+        pytest.param([1], [0, 0], id="out"),
+        pytest.param([0], [0], id="io"),
     ])
-def test_invalid_duplicates(inputs, outputs):
+def test_invalid_duplicates(dimension, i, o):
+    p_t = _ann_type(dimension).Point
+    def p(c): return p_t(*[c for _ in range(dimension)])
+    inputs = [p(c) for c in i]
+    outputs = [p(c) for c in o]
     with pytest.raises(ValueError):
         print(f"ANN.build({inputs}, {outputs}, genome)")
-        _make_ann(0, Random(0), inputs, outputs)
+        _make_ann(dimension, 0, 0, inputs, outputs)
+
+
+def test_inspect_neurons(dimension, mutations, seed):
+    ann, _, _ = _make_ann(dimension, mutations, seed)
+    attrs = [k for k in ann.Neuron.__dict__.keys()
+             if k[0].islower() and k[0].isalpha() and k != "links"]
+    data = []
+    widths = [len(k) for k in attrs]
+    for i, n in enumerate(ann.neurons()):
+        n: ANN.Neuron
+        data.append([])
+        for j, k in enumerate(attrs):
+            attr = getattr(n, k)
+            if isinstance(attr, Callable):
+                s = str(attr())
+            else:
+                s = str(attr)
+            data[i].append(s)
+            widths[j] = max(widths[j], len(s))
+    fmts = " ".join(f"{{:{w}}}" for w in widths)
+    print(fmts.format(*attrs))
+    for i in range(len(data)):
+        print(fmts.format(*data[i]))
 
 
 # .. todo:: implement (code exists in ann.cpp)
 # def test_deepcopy():
 #     original = _make_ann(1000, 0)
 #     original.cop
 
 
-def test_random_eval(mutations, seed):
-    rng = Random(seed)
-    ann, inputs, outputs = _make_ann(mutations, rng)
+def test_stats(dimension, mutations, seed):
+    ann, _, _ = _make_ann(dimension, mutations, seed)
+    ann_t = type(ann)
+
+    stats = ann.stats()
+
+    print("==")
+    print(stats.hidden)
+    print(len(ann.ibuffer()))
+    print(len(ann.obuffer()))
+
+    assert isinstance(stats.dict(), dict), f"{type(stats)=}"
+    assert all([k in stats.dict().keys() for k in
+                "depth hidden edges axons density utility iterations".split()])
+    assert 0 <= stats.depth <= Config.iterations
+    assert ann_t.max_hidden_neurons() == 2**(ann.DIMENSIONS * Config.maxDepth)
+    assert 0 <= stats.hidden <= ann_t.max_hidden_neurons()
+    assert ((ann.max_edges() == (len(ann.ibuffer()) * len(ann.obuffer()))) or
+            (ann.max_edges() == (len(ann.ibuffer()) * stats.hidden
+                                 + stats.hidden * stats.hidden
+                                 + len(ann.obuffer()) * stats.hidden)))
+    assert 0 <= stats.edges <= ann.max_edges()
+    assert 0 <= stats.axons <= ann.max_edges() * math.sqrt(12)
+    assert 0 <= stats.density <= 1
+    assert 0 <= stats.utility <= 1
+    assert 1 <= stats.iterations <= Config.iterations
+
+
+def test_random_eval(dimension, mutations, seed):
+    ann, inputs, outputs = _make_ann(dimension, mutations, seed)
 
     assert len(ann.ibuffer()) == len(inputs)
     assert len(ann.obuffer()) == len(outputs)
     assert ann.empty() or ann.stats().edges > 0
 
     assert ann.ibuffer() == ann.ibuffer()  # same objects
     assert ann.obuffer() == ann.obuffer()  #
 
+    rng = Random(seed)
     avg_output = 0
     for _ in range(1000):
         # inputs, outputs = ann.buffers()
         inputs, outputs = ann.ibuffer(), ann.obuffer()
         for j in range(len(inputs)):
             inputs[j] = rng.uniform(-1, 1)
         if hasattr(outputs, "set_to_nan"):  # pragma: no cover
@@ -147,17 +230,16 @@
     for j in range(len(inputs)):
         inputs[j] = rng.uniform(-1, 1)
 
     ann(inputs, outputs, 1)
     return outputs
 
 
-def test_reset(mutations, seed):
-    rng = Random(seed)
-    ann, _, _ = _make_ann(mutations, rng)
+def test_reset(dimension, mutations, seed):
+    ann, _, _ = _make_ann(dimension, mutations, seed)
 
     n = 1000
     all_outputs = [[], []]
     for i in range(2):
         ann.reset()
         rng = Random(seed)
         for _ in range(n):
@@ -167,19 +249,18 @@
     assert all(all_outputs[0][i] == all_outputs[1][i]
                for i in range(n)), \
         "\n".join(f"{a} =?= {b}" for a, b
                   in zip(all_outputs[0], all_outputs[1]))
 
 
 def test_view_neurons_png(mutations, seed, tmp_path):
-    rng = Random(seed)
-    ann, _, _ = _make_ann(mutations, rng)
+    ann, _, _ = _make_ann(3, mutations, seed)
 
     file = f"{tmp_path}/ann.png"
-    fig = plotly_render(ann)
+    fig = ann.render3D()
 
     try:
         fig.write_image(file)
         print("Generated", file)    # pragma: no cover
     except Exception as e:  # pragma: no cover
         pytest.skip(f"Ignoring exceptions from unstable kaleido: "
                     f"{e=}, {type(e)=}")
@@ -193,26 +274,25 @@
 
 @pytest.mark.parametrize('mutations', [10])
 @pytest.mark.parametrize('seed', [1])
 @pytest.mark.parametrize('with_labels', [True, False])
 def test_view_neurons_interactive(mutations, seed, with_labels, tmp_path):
     _, start = _time()
 
-    rng = Random(seed)
-    ann, inputs, _ = _make_ann(mutations, rng)
+    ann, inputs, _ = _make_ann(3, mutations, seed)
     duration, start = _time(start)
     print(f"Generating ANN(gen={mutations}, seed={seed}): {duration}s")
 
     labels = None
     if with_labels:
         labels = {}
         for i in inputs:
             labels[i] = f"Input{len(labels)}"
 
-    fig = plotly_render(ann, labels)
+    fig = ann.render3D(labels)
     duration, start = _time(start)
     print(f"Preparing rendering: {duration}s")
 
     labels_str = "_with_labels" if with_labels else ""
     fig.write_html(f"{tmp_path}/interactive{labels_str}.ann.html")
     duration, start = _time(start)
     print(f"Writing: {duration}s")
@@ -231,16 +311,15 @@
     prefix = f"interactive{labels_str}"
 
     neurons_file = f"{prefix}.neurons.dat" if with_neurons else None
     dynamics_file = f"{prefix}.dynamics.dat" if with_dynamics else None
 
     _, start = _time()
 
-    rng = Random(seed)
-    ann, inputs, _ = _make_ann(mutations, rng)
+    ann, inputs, _ = _make_ann(3, mutations, seed)
     duration, start = _time(start)
     print(f"Generating ANN(gen={mutations}, seed={seed}): {duration}s")
 
     labels = None
     if with_labels:
         labels = {}
         for i in inputs:
@@ -253,21 +332,22 @@
         labels=labels,
         folder=tmp_path,
         neurons_file=neurons_file,
         dynamics_file=dynamics_file,
         dt=dt
     )
 
+    rng = Random(seed)
     for _ in range(n):
         _random_step(ann, rng)
         ann_monitor.step()
 
     ann_monitor.close()
 
-    fig = plotly_render(ann, labels)
+    fig = ann.render3D(labels)
     duration, start = _time(start)
     print(f"Preparing rendering: {duration}s")
 
     ann_path = f"{tmp_path}/{prefix}.ann.html"
     fig.write_html(ann_path)
     duration, start = _time(start)
     print(f"Writing: {duration}s")
```

### Comparing `abrain-1.0rc0.post5/tests/test_config.py` & `abrain-1.0rc0.post7/tests/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
 import shutil
 from pathlib import Path
 from typing import Dict
 
 import pytest
 
-from abrain.core.config import Config
+from abrain import Config
+
+OutputFunctions = Config.OutputFunctions
+ESHNOutputs = Config.ESHNOutputs
 
 default_config = None
 
 
 @pytest.fixture
 def tmp_config_file(tmp_path):
     return tmp_path.joinpath("config.json")
@@ -18,14 +21,22 @@
 def get_default_config():
     global default_config
     if default_config is None:
         default_config = Config.to_json()
     return default_config
 
 
+def id_output_functions():
+    Config.eshnOutputFunctions = OutputFunctions({
+        ESHNOutputs.Weight: "id",
+        ESHNOutputs.LEO: "id",
+        ESHNOutputs.Bias: "id",
+    })
+
+
 @pytest.fixture
 def restore_config_after():
     config = get_default_config()
 
     yield
 
     # noinspection PyProtectedMember
@@ -39,15 +50,16 @@
     assert len(Config._dict) > 0
 
     for k, v in Config._dict.items():
         print(f"\t{k}: {v}")
 
 
 @pytest.mark.parametrize("key", ["cppnWeightBounds",
-                                 "functionSet", "outputFunctions",
+                                 "functionSet",
+                                 "eshnOutputFunctions",
                                  "mutationRates"])
 def test_json_conversions(key):
     value = getattr(Config, key)
     fake_json = value.toJson()
     roundtrip = type(value).fromJson(fake_json)
 
     print(value, fake_json, roundtrip)
@@ -127,15 +139,15 @@
 
 def nested_setter(key: str, value, j: Dict):  # pragma: no cover
     for section, items in Config._sections.items():
         for k in items:
             if k == key:
                 j[section][key] = value
                 return
-    raise KeyError
+    raise KeyError(f"{key} not found")
 
 
 def change_config_value(key, value, path):
     contents = Config.to_json()
 
     # print("--"*80)
     # print(f"Changing {key}: {value}")
@@ -157,20 +169,26 @@
     'key, value',
     [
         pytest.param("iterations", 15, id="int->int"),
         pytest.param("annWeightsRange", 1.5, id="float->float"),
         pytest.param("activationFunc", "id", id="str->str"),
         pytest.param("cppnWeightBounds", [1, 1, 1, 1, 1],
                      id="List->Bounds"),
-        pytest.param("functionSet", ["id", "abs", "ssgn"], id="List->Strings"),
+        pytest.param("functionSet", ["id", "sin", "abs"],
+                     id="List->Strings"),
         pytest.param("mutationRates",
                      nested_getter("mutationRates", get_default_config()),
-                     id="MutationRates->MutationRates")
+                     id="MutationRates->MutationRates"),
+        pytest.param("eshnOutputFunctions",
+                     nested_getter("eshnOutputFunctions",
+                                   get_default_config()),
+                     id="OutputFunction->OutputFunctions")
     ])
 def test_correct_read_type(key, value, tmp_config_file):
+    id_output_functions()
     change_config_value(key, value, tmp_config_file)
 
 
 @pytest.mark.usefixtures("restore_config_after")
 @pytest.mark.parametrize(
     'key, value',
     [
@@ -187,37 +205,41 @@
 
 @pytest.mark.usefixtures("restore_config_after")
 @pytest.mark.parametrize(
     'key, value',
     [
         pytest.param("activationFunc", "sin", id="act"),
         pytest.param("functionSet", ["abs", "id"], id="funcs"),
-        pytest.param("outputFunctions", ["id", "id", "id"], id="outputs")
     ])
 def test_correct_read_depends(key, value, tmp_config_file):
+    id_output_functions()
     change_config_value(key, value, tmp_config_file)
 
 
 @pytest.mark.usefixtures("restore_config_after")
 @pytest.mark.parametrize(
     'key, value',
     [
-        pytest.param("activationFunc", "1", id="act"),
+        # pytest.param("activationFunc", "1", id="act"),
         pytest.param("functionSet", ["circle_quadrature"], id="funcs"),
-        pytest.param("outputFunctions", ["id", "id"], id="outputs"),
-        pytest.param("outputFunctions", ["sa", "la", "mi"], id="outputs"),
+        pytest.param("eshnOutputFunctions",
+                     {"Weight": "id", "LEO": "id"}, id="outputs"),
+        pytest.param("eshnOutputFunctions",
+                     {"Weight": "sa", "LEO": "la", "Bias": "mi"},
+                     id="outputs"),
         pytest.param("cppnWeightBounds", [3, 1, -1, -3, .1],
                      id="inv_bounds"),
         pytest.param("cppnWeightBounds", [-3, -1, 1, 3, -.1],
                      id="neg_bounds"),
         pytest.param("mutationRates", {}, id="empty_mr"),
         pytest.param("mutationRates", {"add_n": 0}, id="null_mr"),
         pytest.param("mutationRates", {"add_n": -1}, id="neg_mr"),
     ])
 def test_failed_read_depends(key, value, tmp_config_file):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError) as e:
         change_config_value(key, value, tmp_config_file)
+    print("Except as expected:", e)
 
 
 def test_activation_function():
     assert Config.activationFunc == 'ssgn'
     print(Config.activationFunc)
```

### Comparing `abrain-1.0rc0.post5/tests/test_evolution.py` & `abrain-1.0rc0.post7/tests/test_evolution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import json
 import math
 import random
 from pathlib import Path
-from random import Random
 
-from _utils import assert_equal
-from abrain.core.ann import ANN, Point
-from abrain.core.genome import Genome, GIDManager
+from _utils import assert_genomes_equal
+from abrain import Genome, ANN3D as ANN, Point3D as Point
 
 
 class Robot:
     """A bare-bones individual
 
     :param genome: the collection of inheritable characteristics
     """
@@ -41,15 +39,15 @@
             data = json.load(f)
             r = Robot(Genome.from_json(data["genome"]))
             r.fitness = data["fitness"]
             return r
 
     @staticmethod
     def assert_equal(lhs, rhs):
-        assert_equal(lhs.genome, rhs.genome)
+        assert_genomes_equal(lhs.genome, rhs.genome)
         assert lhs.fitness == rhs.fitness
         assert len(lhs.brain.neurons()) == len(rhs.brain.neurons())
 
         lhs_stats, rhs_stats = lhs.brain.stats(), rhs.brain.stats()
         assert lhs_stats.depth == rhs_stats.depth
         assert lhs_stats.edges == rhs_stats.edges
         assert lhs_stats.axons == rhs_stats.axons
@@ -58,37 +56,38 @@
 def test_evolution(evo_config, capsys, tmp_path):
     pop_size = evo_config["population"]
     gens = evo_config["generations"]
     seed = evo_config["seed"]
     fitness = evo_config["fitness"]
 
     tour_size = 4
-    rng = Random(seed)
+    data = Genome.Data.create_for_eshn_cppn(
+        dimension=3, seed=seed,
+        with_lineage=True
+    )
 
     def random_coordinates(n_min, n_max, y):
         def rc(): return random.uniform(-1, 1)
         return [Point(rc(), y, rc()) for _ in
                 range(random.randint(n_min, n_max))]
 
     # By personal convention inputs and outputs are on the y=-1 and y=1 planes,
     # respectively
     Robot.ann_inputs = random_coordinates(10, 20, -1)
     Robot.ann_outputs = random_coordinates(5, 10, 1)
 
-    id_manager = GIDManager()
-
     with capsys.disabled():
         print()
         print("  ========================")
         print("==== Starting evolution ====")
         for k, v in evo_config.items():
             print(f"\t{k}: {v}")
         print()
 
-        population = [Robot(Genome.random(rng, id_manager))
+        population = [Robot(Genome.random(data))
                       for _ in range(pop_size)]
         print("== Initialized population")
 
         def champion(pop=None) -> Robot:
             if pop is None:
                 pop = population
             return pop[max(range(len(pop)), key=lambda r: pop[r].fitness)]
@@ -104,17 +103,17 @@
             Robot.assert_equal(first_champ, roundtrip_champ)
 
         for g in range(gens):
             print(f"> Best {fitness}: {champion().fitness}")
 
             new_population = []
             for _ in range(pop_size):
-                winner = champion(rng.sample(population, tour_size))
-                child = Robot(winner.genome.mutated(rng, id_manager))
-                child.genome.update_lineage(id_manager, [winner.genome])
+                winner = champion(data.rng.sample(population, tour_size))
+                child = Robot(winner.genome.mutated(data))
+                child.genome.update_lineage(data, [winner.genome])
                 new_population.append(child)
 
             population = new_population
             print("== Generated new population [{:0{width}d}] =="
                   .format(g+1, width=math.ceil(math.log10(gens))))
 
         print("== Final champion ==")
@@ -126,9 +125,9 @@
         json_path = f"{base_path}.json"
         champ.to_json(json_path)
         print(">>> Logged to", json_path)
 
         roundtrip_champ = Robot.from_json_file(json_path)
         Robot.assert_equal(champ, roundtrip_champ)
 
-        dot_path = champ.genome.to_dot(base_path, "pdf")
+        dot_path = champ.genome.to_dot(data, base_path, "pdf")
         print(">>> Drawn to", dot_path)
```

