# Comparing `tmp/oresat_configs-0.7.1.tar.gz` & `tmp/oresat_configs-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_configs-0.7.1.tar", last modified: Sun May 19 20:46:54 2024, max compression
+gzip compressed data, was "oresat_configs-0.7.2.tar", last modified: Sun May 26 20:36:10 2024, max compression
```

## Comparing `oresat_configs-0.7.1.tar` & `oresat_configs-0.7.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.479317 oresat_configs-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/build_and_install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/oresat0/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/oresat0/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/oresat0_5/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/oresat0_5/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/oresat1/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/oresat1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/scripts/gen_beacon_rst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.487317 oresat_configs-0.7.1/docs/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/yamls/beacon_config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/yamls/card_config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/yamls/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.487317 oresat_configs-0.7.1/oresat_configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    28421 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/_yaml_to_od.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.491317 oresat_configs-0.7.1/oresat_configs/base/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/adcs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/battery.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17233 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/c3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/cfc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/diode_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/dxwifi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/fw_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/gps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/reaction_wheel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/solar.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/star_tracker.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/sw_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/beacon_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/card_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/card_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/cards.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.491317 oresat_configs-0.7.1/oresat_configs/oresat0/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0/battery_overlay.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.491317 oresat_configs-0.7.1/oresat_configs/oresat0_5/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0_5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0_5/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.491317 oresat_configs-0.7.1/oresat_configs/oresat1/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat1/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/oresat_configs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/gen_dbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/gen_dcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/gen_fw_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/gen_xtce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/list_cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/pdo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/print_od.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/sdo_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/standard_objects.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/oresat_configs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/test_config_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/test_oresat0.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/test_oresat0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/test_oresat1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.729037 oresat_configs-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.713037 oresat_configs-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.717037 oresat_configs-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-26 20:36:10.725037 oresat_configs-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/build_and_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.717037 oresat_configs-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.717037 oresat_configs-0.7.2/docs/oresat0/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/oresat0/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.717037 oresat_configs-0.7.2/docs/oresat0_5/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/oresat0_5/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.717037 oresat_configs-0.7.2/docs/oresat1/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/oresat1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.717037 oresat_configs-0.7.2/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/scripts/gen_beacon_rst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.717037 oresat_configs-0.7.2/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.717037 oresat_configs-0.7.2/docs/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/yamls/beacon_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/yamls/card_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/docs/yamls/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.721037 oresat_configs-0.7.2/oresat_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 20:36:10.000000 oresat_configs-0.7.2/oresat_configs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28421 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/_yaml_to_od.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.725037 oresat_configs-0.7.2/oresat_configs/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/adcs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/battery.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17233 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/cfc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/diode_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/dxwifi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/fw_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/gps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/reaction_wheel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/solar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/star_tracker.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/base/sw_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/beacon_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/card_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/card_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/cards.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.725037 oresat_configs-0.7.2/oresat_configs/oresat0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/oresat0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/oresat0/battery_overlay.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/oresat0/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.725037 oresat_configs-0.7.2/oresat_configs/oresat0_5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/oresat0_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/oresat0_5/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.725037 oresat_configs-0.7.2/oresat_configs/oresat1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/oresat1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/oresat1/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.725037 oresat_configs-0.7.2/oresat_configs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/scripts/gen_dbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/scripts/gen_dcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/scripts/gen_fw_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/scripts/gen_xtce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/scripts/list_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/scripts/pdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/scripts/print_od.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/scripts/sdo_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/oresat_configs/standard_objects.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.725037 oresat_configs-0.7.2/oresat_configs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-26 20:36:10.000000 oresat_configs-0.7.2/oresat_configs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-26 20:36:10.000000 oresat_configs-0.7.2/oresat_configs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:36:10.000000 oresat_configs-0.7.2/oresat_configs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-26 20:36:10.000000 oresat_configs-0.7.2/oresat_configs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 20:36:10.000000 oresat_configs-0.7.2/oresat_configs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 20:36:10.000000 oresat_configs-0.7.2/oresat_configs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 20:36:10.729037 oresat_configs-0.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:36:10.725037 oresat_configs-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/tests/test_config_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/tests/test_oresat0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/tests/test_oresat0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-26 20:36:06.000000 oresat_configs-0.7.2/tests/test_oresat1.py
```

### Comparing `oresat_configs-0.7.1/.github/workflows/pypi.yaml` & `oresat_configs-0.7.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/.github/workflows/tests.yaml` & `oresat_configs-0.7.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/.gitignore` & `oresat_configs-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/LICENSE` & `oresat_configs-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/PKG-INFO` & `oresat_configs-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: oresat-configs
-Version: 0.7.1
+Version: 0.7.2
 Summary: OreSat mission configurations
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: canopen
 Requires-Dist: dacite
 Requires-Dist: pyyaml
+Requires-Dist: tabulate
 
 # OreSat Configs
 
 Firmware/software configurations for OreSat missions.
 
 Includes:
```

### Comparing `oresat_configs-0.7.1/README.md` & `oresat_configs-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/docs/Makefile` & `oresat_configs-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/docs/conf.py` & `oresat_configs-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/docs/make.bat` & `oresat_configs-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/docs/scripts/gen_beacon_rst.py` & `oresat_configs-0.7.2/docs/scripts/gen_beacon_rst.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/docs/yamls/card_config.rst` & `oresat_configs-0.7.2/docs/yamls/card_config.rst`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/__init__.py` & `oresat_configs-0.7.2/oresat_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/__main__.py` & `oresat_configs-0.7.2/oresat_configs/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/_yaml_to_od.py` & `oresat_configs-0.7.2/oresat_configs/_yaml_to_od.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/__init__.py` & `oresat_configs-0.7.2/oresat_configs/base/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/adcs.yaml` & `oresat_configs-0.7.2/oresat_configs/base/adcs.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/battery.yaml` & `oresat_configs-0.7.2/oresat_configs/base/battery.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/c3.yaml` & `oresat_configs-0.7.2/oresat_configs/base/c3.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         access_type: ro
 
       - subindex: 0x2
         name: timeout
         data_type: uint32
         description: tx enable timeout
         access_type: const
-        default: 1209600 # 2 weeks
+        default: 2592000 # 30 days
         unit: s
 
       - subindex: 0x3
         name: last_enable_timestamp
         data_type: uint32
         description: last tx enable timestamp
         access_type: ro
```

### Comparing `oresat_configs-0.7.1/oresat_configs/base/cfc.yaml` & `oresat_configs-0.7.2/oresat_configs/base/cfc.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/dxwifi.yaml` & `oresat_configs-0.7.2/oresat_configs/base/dxwifi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/fw_common.yaml` & `oresat_configs-0.7.2/oresat_configs/base/fw_common.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/gps.yaml` & `oresat_configs-0.7.2/oresat_configs/base/gps.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   - index: 0x4000
     name: status
     data_type: uint8
     value_descriptions:
       'off': 0
       searching: 1
       locked: 2
-      error: 3
+      error: 0xFF
     access_type: ro
 
   - index: 0x4001
     name: time_syncd
     data_type: bool
     description: system time has syncd to gps time
     access_type: ro
@@ -174,14 +174,26 @@
       - subindex: 0x14
         name: time_since_midnight
         data_type: uint32
         description: time since midnight when the gps data was received
         access_type: ro
         unit: ms
 
+      - subindex: 0x15
+        name: packet_count
+        data_type: uint32
+        description: number of packet received since boot
+        access_type: ro
+
+      - subindex: 0x16
+        name: last_packet
+        data_type: octet_str
+        description: last packet received
+        access_type: ro
+
 tpdos:
   - num: 3
     fields:
       -  [skytraq, time_since_midnight]
 
   - num: 4
     fields:
@@ -200,12 +212,13 @@
 
   - num: 7
     fields:
       - [status]
       - [skytraq, number_of_sv]
       - [skytraq, fix_mode]
       - [time_syncd]
+    event_timer_ms: 1000
 
   - num: 16 # the time sync TPDO
     fields:
       - [scet]
     sync: 1
```

### Comparing `oresat_configs-0.7.1/oresat_configs/base/reaction_wheel.yaml` & `oresat_configs-0.7.2/oresat_configs/base/reaction_wheel.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/solar.yaml` & `oresat_configs-0.7.2/oresat_configs/base/solar.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/star_tracker.yaml` & `oresat_configs-0.7.2/oresat_configs/base/star_tracker.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/base/sw_common.yaml` & `oresat_configs-0.7.2/oresat_configs/base/sw_common.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/beacon_config.py` & `oresat_configs-0.7.2/oresat_configs/beacon_config.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/card_config.py` & `oresat_configs-0.7.2/oresat_configs/card_config.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/card_info.py` & `oresat_configs-0.7.2/oresat_configs/card_info.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/cards.csv` & `oresat_configs-0.7.2/oresat_configs/cards.csv`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/constants.py` & `oresat_configs-0.7.2/oresat_configs/constants.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/oresat0/__init__.py` & `oresat_configs-0.7.2/oresat_configs/oresat0/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/oresat0/battery_overlay.yaml` & `oresat_configs-0.7.2/oresat_configs/oresat0/battery_overlay.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/oresat0/beacon.yaml` & `oresat_configs-0.7.2/oresat_configs/oresat0/beacon.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/oresat0_5/__init__.py` & `oresat_configs-0.7.2/oresat_configs/oresat0_5/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/oresat0_5/beacon.yaml` & `oresat_configs-0.7.2/oresat_configs/oresat0_5/beacon.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/oresat1/__init__.py` & `oresat_configs-0.7.2/oresat_configs/oresat1/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/scripts/gen_dbc.py` & `oresat_configs-0.7.2/oresat_configs/scripts/gen_dbc.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/scripts/gen_dcf.py` & `oresat_configs-0.7.2/oresat_configs/scripts/gen_dcf.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/scripts/gen_fw_files.py` & `oresat_configs-0.7.2/oresat_configs/scripts/gen_fw_files.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/scripts/gen_xtce.py` & `oresat_configs-0.7.2/oresat_configs/scripts/gen_xtce.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/scripts/list_cards.py` & `oresat_configs-0.7.2/oresat_configs/scripts/list_cards.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/scripts/pdo.py` & `oresat_configs-0.7.2/oresat_configs/scripts/pdo.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/scripts/print_od.py` & `oresat_configs-0.7.2/oresat_configs/scripts/print_od.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/scripts/sdo_transfer.py` & `oresat_configs-0.7.2/oresat_configs/scripts/sdo_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs/standard_objects.yaml` & `oresat_configs-0.7.2/oresat_configs/standard_objects.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/oresat_configs.egg-info/PKG-INFO` & `oresat_configs-0.7.2/oresat_configs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: oresat-configs
-Version: 0.7.1
+Version: 0.7.2
 Summary: OreSat mission configurations
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: canopen
 Requires-Dist: dacite
 Requires-Dist: pyyaml
+Requires-Dist: tabulate
 
 # OreSat Configs
 
 Firmware/software configurations for OreSat missions.
 
 Includes:
```

### Comparing `oresat_configs-0.7.1/oresat_configs.egg-info/SOURCES.txt` & `oresat_configs-0.7.2/oresat_configs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/pyproject.toml` & `oresat_configs-0.7.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "canopen",
     "dacite",
     "pyyaml",
+    "tabulate",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 oresat-configs = "oresat_configs.__main__:oresat_configs"
 oresat-gen-fw-files = "oresat_configs.scripts.gen_fw_files:gen_fw_files"
 oresat-gen-dcf = "oresat_configs.scripts.gen_dcf:gen_dcf"
```

### Comparing `oresat_configs-0.7.1/tests/__init__.py` & `oresat_configs-0.7.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.1/tests/test_config_types.py` & `oresat_configs-0.7.2/tests/test_config_types.py`

 * *Files identical despite different names*

