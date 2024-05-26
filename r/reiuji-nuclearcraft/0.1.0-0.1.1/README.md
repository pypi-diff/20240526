# Comparing `tmp/reiuji_nuclearcraft-0.1.0.tar.gz` & `tmp/reiuji_nuclearcraft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reiuji_nuclearcraft-0.1.0.tar", last modified: Fri May 24 03:05:03 2024, max compression
+gzip compressed data, was "reiuji_nuclearcraft-0.1.1.tar", last modified: Sun May 26 10:59:43 2024, max compression
```

## Comparing `reiuji_nuclearcraft-0.1.0.tar` & `reiuji_nuclearcraft-0.1.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.089560 reiuji_nuclearcraft-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11306 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-05-24 03:05:03.085560 reiuji_nuclearcraft-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 03:05:03.089560 reiuji_nuclearcraft-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.077560 reiuji_nuclearcraft-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.077560 reiuji_nuclearcraft-0.1.0/src/reiuji/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.077560 reiuji_nuclearcraft-0.1.0/src/reiuji/components/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.077560 reiuji_nuclearcraft-0.1.0/src/reiuji/components/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/components/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15271 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/components/defaults/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/components/defaults/nucleosynthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/components/defaults/turbine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/components/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.077560 reiuji_nuclearcraft-0.1.0/src/reiuji/core/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/core/multi_sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.077560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.081560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/designer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15842 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/placement_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/scaled_calculations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.081560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.081560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_dynamo/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_dynamo/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_dynamo/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_dynamo/designer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.081560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_rotor/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_rotor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_rotor/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_rotor/designer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.081560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.081560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/decelerator/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/decelerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/decelerator/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/decelerator/designer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.081560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/linear/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/linear/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/linear/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/linear/designer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.085560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/nucleosynthesis/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/nucleosynthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/nucleosynthesis/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/nucleosynthesis/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/nucleosynthesis/designer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.085560 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/synchrotron/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/synchrotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32491 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/synchrotron/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    41330 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/synchrotron/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/synchrotron/designer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.085560 reiuji_nuclearcraft-0.1.0/src/reiuji/io/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.085560 reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/nucleosynthesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/turbine.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-24 03:04:55.000000 reiuji_nuclearcraft-0.1.0/src/reiuji/io/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:05:03.085560 reiuji_nuclearcraft-0.1.0/src/reiuji_nuclearcraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-05-24 03:05:03.000000 reiuji_nuclearcraft-0.1.0/src/reiuji_nuclearcraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-24 03:05:03.000000 reiuji_nuclearcraft-0.1.0/src/reiuji_nuclearcraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:05:03.000000 reiuji_nuclearcraft-0.1.0/src/reiuji_nuclearcraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 03:05:03.000000 reiuji_nuclearcraft-0.1.0/src/reiuji_nuclearcraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 03:05:03.000000 reiuji_nuclearcraft-0.1.0/src/reiuji_nuclearcraft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.774653 reiuji_nuclearcraft-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11306 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-05-26 10:59:43.774653 reiuji_nuclearcraft-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 10:59:43.774653 reiuji_nuclearcraft-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.762653 reiuji_nuclearcraft-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.762653 reiuji_nuclearcraft-0.1.1/src/reiuji/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.766653 reiuji_nuclearcraft-0.1.1/src/reiuji/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.766653 reiuji_nuclearcraft-0.1.1/src/reiuji/components/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/components/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15271 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/components/defaults/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/components/defaults/nucleosynthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/components/defaults/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/components/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.766653 reiuji_nuclearcraft-0.1.1/src/reiuji/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/core/multi_sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.766653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.766653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/designer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15842 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/placement_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/scaled_calculations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.766653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.766653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_dynamo/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_dynamo/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_dynamo/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_dynamo/designer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.766653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_rotor/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_rotor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_rotor/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_rotor/designer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.766653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.770653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/decelerator/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/decelerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/decelerator/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/decelerator/designer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.770653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/linear/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/linear/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/linear/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/linear/designer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.770653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/nucleosynthesis/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/nucleosynthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/nucleosynthesis/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/nucleosynthesis/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/nucleosynthesis/designer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.770653 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/synchrotron/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/synchrotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32491 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/synchrotron/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41330 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/synchrotron/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/synchrotron/designer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.770653 reiuji_nuclearcraft-0.1.1/src/reiuji/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.770653 reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/nucleosynthesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-26 10:59:39.000000 reiuji_nuclearcraft-0.1.1/src/reiuji/io/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 10:59:43.774653 reiuji_nuclearcraft-0.1.1/src/reiuji_nuclearcraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-05-26 10:59:43.000000 reiuji_nuclearcraft-0.1.1/src/reiuji_nuclearcraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-26 10:59:43.000000 reiuji_nuclearcraft-0.1.1/src/reiuji_nuclearcraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 10:59:43.000000 reiuji_nuclearcraft-0.1.1/src/reiuji_nuclearcraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 10:59:43.000000 reiuji_nuclearcraft-0.1.1/src/reiuji_nuclearcraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-26 10:59:43.000000 reiuji_nuclearcraft-0.1.1/src/reiuji_nuclearcraft.egg-info/top_level.txt
```

### Comparing `reiuji_nuclearcraft-0.1.0/LICENSE` & `reiuji_nuclearcraft-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/PKG-INFO` & `reiuji_nuclearcraft-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reiuji_nuclearcraft
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for designing NuclearCraft multiblocks.
 Author-email: Celeste Ma <mtcelestema@proton.me>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,14 +201,15 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 Project-URL: Homepage, https://github.com/MtCelesteMa/reiuji
+Project-URL: Repository, https://github.com/MtCelesteMa/reiuji
 Project-URL: Bug Tracker, https://github.com/MtCelesteMa/reiuji/issues
 Keywords: nuclearcraft,multiblock,design,minecraft
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.12
@@ -240,7 +241,9 @@
 - NBT schematic writers for copy-and-pasting designed structures directly into Minecraft worlds.
 
 **Note:** Features already covered by other programs like [LEU-235](https://leu-235.com/) will have lower priority. NuclearCraft Classic molten salt reactor and heat exchanger designers might never be implemented due to their complexity.
 
 ## Usage
 
 Reiuji has a command line interface that can be found [here](https://github.com/MtCelesteMa/reiuji-cli).
+
+There is also a web app in the works.
```

### Comparing `reiuji_nuclearcraft-0.1.0/README.md` & `reiuji_nuclearcraft-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,7 +19,9 @@
 - NBT schematic writers for copy-and-pasting designed structures directly into Minecraft worlds.
 
 **Note:** Features already covered by other programs like [LEU-235](https://leu-235.com/) will have lower priority. NuclearCraft Classic molten salt reactor and heat exchanger designers might never be implemented due to their complexity.
 
 ## Usage
 
 Reiuji has a command line interface that can be found [here](https://github.com/MtCelesteMa/reiuji-cli).
+
+There is also a web app in the works.
```

### Comparing `reiuji_nuclearcraft-0.1.0/pyproject.toml` & `reiuji_nuclearcraft-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reiuji_nuclearcraft"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
     "pydantic",
     "ortools",
     "nbt"
 ]
 requires-python = ">=3.12"
 authors = [
@@ -29,8 +29,9 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["reiuji*"]
 namespaces = false
 
 [project.urls]
 Homepage = "https://github.com/MtCelesteMa/reiuji"
+Repository = "https://github.com/MtCelesteMa/reiuji"
 "Bug Tracker" = "https://github.com/MtCelesteMa/reiuji/issues"
```

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/components/base.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/components/base.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/components/defaults/accelerator.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/components/defaults/accelerator.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/components/defaults/nucleosynthesis.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/components/defaults/nucleosynthesis.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/components/defaults/turbine.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/components/defaults/turbine.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/components/types.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/components/types.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/core/multi_sequence.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/core/multi_sequence.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/calculations.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/calculations.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/constraints.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,28 +135,32 @@
             idx = seq.index_int_to_tuple(i)
             mirror_idx = (idx[:self.axis] + (seq.shape[self.axis] - 1 - idx[self.axis],) + idx[self.axis + 1:])
             model.Add(component == seq[mirror_idx])
 
 
 class QuantityConstraint(Constraint):
     """Limits the number of a specific component type in the sequence."""
-    def __init__(self, component_full_name: str, max_quantity: int, min_quantity: int = 0) -> None:
+    def __init__(self, component_full_name: str, max_quantity: int | None = None, min_quantity: int | None = None) -> None:
         self.component_full_name = component_full_name
         self.max_quantity = max_quantity
-        self.min_quantity = min_quantity
+        self.min_quantity = min_quantity if isinstance(min_quantity, int) else 0
     
     def is_satisfied(self, seq: core.multi_sequence.MultiSequence[Component]) -> bool:
-        return sum([1 for component in seq if component.full_name == self.component_full_name]) <= self.max_quantity
+        count = sum([1 for component in seq if component.full_name == self.component_full_name])
+        if count < self.min_quantity or (isinstance(self.max_quantity, int) and count > self.max_quantity):
+            return False
+        return True
     
     def to_model(
         self,
         model: cp_model.CpModel,
         seq: core.multi_sequence.MultiSequence[cp_model.IntVar],
         components: list[Component]
     ) -> None:
         component_id = [component.full_name for component in components].index(self.component_full_name)
         is_equal = [model.NewBoolVar(str(uuid.uuid4())) for _ in seq]
         for i, component in enumerate(seq):
             model.Add(component == component_id).OnlyEnforceIf(is_equal[i])
             model.Add(component != component_id).OnlyEnforceIf(is_equal[i].Not())
         model.Add(sum(is_equal) >= self.min_quantity)
-        model.Add(sum(is_equal) <= self.max_quantity)
+        if isinstance(self.max_quantity, int):
+            model.Add(sum(is_equal) <= self.max_quantity)
```

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/designer.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/designer.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/placement_rules.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/placement_rules.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/base/scaled_calculations.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/base/scaled_calculations.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_dynamo/calculations.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_dynamo/calculations.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_dynamo/constraints.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_dynamo/constraints.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_dynamo/designer.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_dynamo/designer.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             self,
             side_length: int,
             *,
             shaft_width: int = 1,
             x_symmetry: bool = False,
             y_symmetry: bool = False,
             components: list[Component] | None = None,
-            component_limits: dict[str, tuple[int, int]] | None = None
+            component_limits: dict[str, tuple[int | None, int | None]] | None = None
     ) -> None:
         super().__init__(components=components if not isinstance(components, type(None)) else OVERHAULED_TURBINE_DYNAMO_COMPONENTS)
         self.side_length = side_length
         self.shaft_width = shaft_width
         self.x_symmetry = x_symmetry
         self.y_symmetry = y_symmetry
         self.component_limits = component_limits if not isinstance(component_limits, type(None)) else dict()
```

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_rotor/calculations.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_rotor/calculations.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/overhauled/turbine_rotor/designer.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/overhauled/turbine_rotor/designer.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class TurbineRotorDesigner(base.designer.Designer):
     def __init__(
             self,
             length: int,
             optimal_expansion: float,
             *,
             components: list[Component] | None = None,
-            component_limits: dict[str, tuple[int, int]] | None = None
+            component_limits: dict[str, tuple[int | None, int | None]] | None = None
     ) -> None:
         super().__init__(components=components if not isinstance(components, type(None)) else OVERHAULED_TURBINE_ROTOR_COMPONENTS)
         self.length = length
         self.optimal_expansion = optimal_expansion
         self.component_limits = component_limits if not isinstance(component_limits, type(None)) else dict()
     
     @property
```

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/decelerator/constraints.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/decelerator/constraints.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/decelerator/designer.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/decelerator/designer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             env_temperature: int = 300,
             kappa: float = 0.0025,
             scaling_factor: int = 10000,
             initial_focus: float = 0.0,
             heat_neutral: bool = True,
             internal_symmetry: bool = False,
             components: list[Component] | None = None,
-            component_limits: dict[str, tuple[int, int]] | None = None
+            component_limits: dict[str, tuple[int | None, int | None]] | None = None
     ) -> None:
         super().__init__(components=components if not isinstance(components, type(None)) else QMD_ACCELERATOR_COMPONENTS)
         self.side_length = side_length
         self.minimum_energy = minimum_energy
         self.maximum_energy = maximum_energy
         self.target_focus = target_focus
         self.charge = charge
```

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/linear/calculations.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/linear/calculations.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/linear/constraints.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/linear/constraints.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/linear/designer.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/linear/designer.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             initial_focus: float = 0.0,
             env_temperature: int = 300,
             kappa: float = 0.0025,
             heat_neutral: bool = True,
             y_symmetry: bool = False,
             z_symmetry: bool = False,
             components: list[Component] | None = None,
-            component_limits: dict[str, tuple[int, int]] | None = None
+            component_limits: dict[str, tuple[int | None, int | None]] | None = None
     ) -> None:
         super().__init__(components=components if not isinstance(components, type(None)) else QMD_LINEAR_ACCELERATOR_COMPONENTS)
         self.length = length
         self.minimum_energy = minimum_energy
         self.maximum_energy = maximum_energy
         self.target_focus = target_focus
         self.charge = charge
```

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/nucleosynthesis/calculations.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/nucleosynthesis/calculations.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/nucleosynthesis/constraints.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/nucleosynthesis/constraints.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/nucleosynthesis/designer.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/nucleosynthesis/designer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(
             self,
             *,
             recipe_heat: int,
             x_symmetry: bool = False,
             z_symmetry: bool = False,
             components: list[Component] | None = None,
-            component_limits: dict[str, tuple[int, int]] | None = None
+            component_limits: dict[str, tuple[int | None, int | None]] | None = None
     ) -> None:
         super().__init__(components=components if not isinstance(components, type(None)) else QMD_NUCLEOSYNTHESIS_COMPONENTS)
         self.recipe_heat = recipe_heat
         self.x_symmetry = x_symmetry
         self.z_symmetry = z_symmetry
         self.component_limits = component_limits if not isinstance(component_limits, type(None)) else dict()
```

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/synchrotron/calculations.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/synchrotron/calculations.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/synchrotron/constraints.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/synchrotron/constraints.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/designer/qmd/synchrotron/designer.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/designer/qmd/synchrotron/designer.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             env_temperature: int = 300,
             kappa: float = 0.0025,
             scaling_factor: int = 10000,
             initial_focus: float = 0.0,
             heat_neutral: bool = True,
             internal_symmetry: bool = False,
             components: list[Component] | None = None,
-            component_limits: dict[str, tuple[int, int]] | None = None
+            component_limits: dict[str, tuple[int | None, int | None]] | None = None
     ) -> None:
         super().__init__(components=components if not isinstance(components, type(None)) else QMD_ACCELERATOR_COMPONENTS)
         self.side_length = side_length
         self.minimum_energy = minimum_energy
         self.maximum_energy = maximum_energy
         self.target_focus = target_focus
         self.charge = charge
```

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/accelerator.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/accelerator.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/base.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/base.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/nucleosynthesis.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/nucleosynthesis.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/io/schematics/turbine.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/io/schematics/turbine.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji/io/serialization.py` & `reiuji_nuclearcraft-0.1.1/src/reiuji/io/serialization.py`

 * *Files identical despite different names*

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji_nuclearcraft.egg-info/PKG-INFO` & `reiuji_nuclearcraft-0.1.1/src/reiuji_nuclearcraft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reiuji_nuclearcraft
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for designing NuclearCraft multiblocks.
 Author-email: Celeste Ma <mtcelestema@proton.me>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,14 +201,15 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 Project-URL: Homepage, https://github.com/MtCelesteMa/reiuji
+Project-URL: Repository, https://github.com/MtCelesteMa/reiuji
 Project-URL: Bug Tracker, https://github.com/MtCelesteMa/reiuji/issues
 Keywords: nuclearcraft,multiblock,design,minecraft
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Games/Entertainment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.12
@@ -240,7 +241,9 @@
 - NBT schematic writers for copy-and-pasting designed structures directly into Minecraft worlds.
 
 **Note:** Features already covered by other programs like [LEU-235](https://leu-235.com/) will have lower priority. NuclearCraft Classic molten salt reactor and heat exchanger designers might never be implemented due to their complexity.
 
 ## Usage
 
 Reiuji has a command line interface that can be found [here](https://github.com/MtCelesteMa/reiuji-cli).
+
+There is also a web app in the works.
```

### Comparing `reiuji_nuclearcraft-0.1.0/src/reiuji_nuclearcraft.egg-info/SOURCES.txt` & `reiuji_nuclearcraft-0.1.1/src/reiuji_nuclearcraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

