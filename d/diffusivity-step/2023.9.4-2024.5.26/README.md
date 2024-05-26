# Comparing `tmp/diffusivity_step-2023.9.4.tar.gz` & `tmp/diffusivity_step-2024.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffusivity_step-2023.9.4.tar", last modified: Mon Sep  4 17:45:11 2023, max compression
+gzip compressed data, was "diffusivity_step-2024.5.26.tar", last modified: Sun May 26 13:40:07 2024, max compression
```

## Comparing `diffusivity_step-2023.9.4.tar` & `diffusivity_step-2024.5.26.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/
--rw-r--r--   0 runner    (1001) docker     (999)      126 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (999)     3342 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (999)      637 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1519 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      348 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     3517 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1959 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/diffusivity_step/
--rw-r--r--   0 runner    (1001) docker     (999)      639 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/diffusivity_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      500 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/diffusivity_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)    16548 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/diffusivity_step/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.539353 diffusivity_step-2023.9.4/diffusivity_step/data/
--rw-r--r--   0 runner    (1001) docker     (999)     2460 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/diffusivity_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (999)     1590 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/diffusivity_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (999)    31915 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/diffusivity_step/diffusivity.py
--rw-r--r--   0 runner    (1001) docker     (999)     4666 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/diffusivity_step/diffusivity_parameters.py
--rw-r--r--   0 runner    (1001) docker     (999)     3067 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/diffusivity_step/diffusivity_step.py
--rw-r--r--   0 runner    (1001) docker     (999)     8568 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/diffusivity_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (999)     6693 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/diffusivity_step/tk_diffusivity.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.539353 diffusivity_step-2023.9.4/diffusivity_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3517 2023-09-04 17:45:11.000000 diffusivity_step-2023.9.4/diffusivity_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1337 2023-09-04 17:45:11.000000 diffusivity_step-2023.9.4/diffusivity_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 17:45:11.000000 diffusivity_step-2023.9.4/diffusivity_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      136 2023-09-04 17:45:11.000000 diffusivity_step-2023.9.4/diffusivity_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       62 2023-09-04 17:45:11.000000 diffusivity_step-2023.9.4/diffusivity_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       17 2023-09-04 17:45:11.000000 diffusivity_step-2023.9.4/diffusivity_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 17:44:53.000000 diffusivity_step-2023.9.4/diffusivity_step.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/docs/
--rw-r--r--   0 runner    (1001) docker     (999)     6802 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (999)    22936 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/_static/SEAMM Inverted 288x181.png
--rw-r--r--   0 runner    (1001) docker     (999)    17802 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (999)    79373 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (999)    68255 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (999)    63967 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (999)    32355 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (999)      182 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)       28 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (999)     9586 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (999)       36 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (999)      223 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1257 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (999)       85 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (999)     1039 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)       28 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1470 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     6721 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (999)      830 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)       62 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       89 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (999)       35 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/requirements_install.txt
--rw-r--r--   0 runner    (1001) docker     (999)      432 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     2873 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 17:45:11.543353 diffusivity_step-2023.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (999)       71 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      365 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/tests/test_diffusivity_step.py
--rw-r--r--   0 runner    (1001) docker     (999)    68751 2023-09-04 17:44:48.000000 diffusivity_step-2023.9.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/diffusivity_step/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/diffusivity_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/diffusivity_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16548 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/diffusivity_step/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.616781 diffusivity_step-2024.5.26/diffusivity_step/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/diffusivity_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/diffusivity_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    32050 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/diffusivity_step/diffusivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/diffusivity_step/diffusivity_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/diffusivity_step/diffusivity_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/diffusivity_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/diffusivity_step/tk_diffusivity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/diffusivity_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-26 13:40:07.000000 diffusivity_step-2024.5.26/diffusivity_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-26 13:40:07.000000 diffusivity_step-2024.5.26/diffusivity_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:40:07.000000 diffusivity_step-2024.5.26/diffusivity_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-26 13:40:07.000000 diffusivity_step-2024.5.26/diffusivity_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-26 13:40:07.000000 diffusivity_step-2024.5.26/diffusivity_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-26 13:40:07.000000 diffusivity_step-2024.5.26/diffusivity_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 13:40:03.000000 diffusivity_step-2024.5.26/diffusivity_step.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.616781 diffusivity_step-2024.5.26/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.616781 diffusivity_step-2024.5.26/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    22936 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/_static/SEAMM Inverted 288x181.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.616781 diffusivity_step-2024.5.26/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9586 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/requirements_install.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 13:40:07.620781 diffusivity_step-2024.5.26/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/tests/test_diffusivity_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-26 13:40:00.000000 diffusivity_step-2024.5.26/versioneer.py
```

### Comparing `diffusivity_step-2023.9.4/CONTRIBUTING.rst` & `diffusivity_step-2024.5.26/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/HISTORY.rst` & `diffusivity_step-2024.5.26/HISTORY.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 =======
 History
 =======
-
+2024.5.26 -- Updated for new task handling
+    * The new handling of running tasks such as LAMMPS required a small change in the
+      code.
+      
 2023.9.5 -- Changed default to using only MSD
     * The Helfand moments approach seems give incorrect results if the sampling time is
       too long. It is not dramatic, but gives increasingly incorrect results as the
       sampling time is increased. Thus using the Helfand moments is dangerous because
       the results may be wrong, but not obviously so.
 
 2023.8.30 -- Initial working version
```

### Comparing `diffusivity_step-2023.9.4/LICENSE` & `diffusivity_step-2024.5.26/LICENSE`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/PKG-INFO` & `diffusivity_step-2024.5.26/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffusivity_step
-Version: 2023.9.4
+Version: 2024.5.26
 Summary: A SEAMM plug-in for Diffusivity
 Home-page: https://github.com/molssi-seamm/diffusivity_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -20,14 +20,21 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: molsystem
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: seamm
+Requires-Dist: seamm-util
+Requires-Dist: seamm-widgets
+Requires-Dist: tabulate
 
 =========================
 SEAMM Diffusivity Plug-in
 =========================
 
 .. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/diffusivity_step
    :target: https://github.com/molssi-seamm/diffusivity_step/pulls
@@ -80,15 +87,18 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-
+2024.5.26 -- Updated for new task handling
+    * The new handling of running tasks such as LAMMPS required a small change in the
+      code.
+      
 2023.9.5 -- Changed default to using only MSD
     * The Helfand moments approach seems give incorrect results if the sampling time is
       too long. It is not dramatic, but gives increasingly incorrect results as the
       sampling time is increased. Thus using the Helfand moments is dangerous because
       the results may be wrong, but not obviously so.
 
 2023.8.30 -- Initial working version
```

### Comparing `diffusivity_step-2023.9.4/README.rst` & `diffusivity_step-2024.5.26/README.rst`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/diffusivity_step/__init__.py` & `diffusivity_step-2024.5.26/diffusivity_step/__init__.py`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/diffusivity_step/analysis.py` & `diffusivity_step-2024.5.26/diffusivity_step/analysis.py`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/diffusivity_step/data/properties.csv` & `diffusivity_step-2024.5.26/diffusivity_step/data/properties.csv`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/diffusivity_step/data/references.bib` & `diffusivity_step-2024.5.26/diffusivity_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/diffusivity_step/diffusivity.py` & `diffusivity_step-2024.5.26/diffusivity_step/diffusivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -504,15 +504,15 @@
                     "center",
                     "decimal",
                     "left",
                 ),
             )
             length = len(tmp.splitlines()[0])
             text += "\n"
-            text += f"Diffusion Coefficients (* {self._scale:.1e})".center(length)
+            text += f"Diffusion Coefficients (* {self._scale:.1e} m^2/s)".center(length)
             text += "\n"
             text += tmp
             text += "\n"
 
             printer.normal(__(text, indent=8 * " ", wrap=False, dedent=False))
 
             # And store results, only for the full output at the end
@@ -584,14 +584,17 @@
                 f"Calculate the diffusivity using the {P['approach']} approach, "
                 f"averaging over {P['nruns']} runs.\n\n"
             )
         if not short:
             # The subflowchart
             self.subflowchart.root_directory = self.flowchart.root_directory
 
+            # Make sure that the subflowchart has the executor
+            self.subflowchart.executor = self.flowchart.executor
+
             # Get the first real node
             node = self.subflowchart.get_node("1").next()
 
             while node is not None:
                 try:
                     text += __(node.description_text()).__str__()
                 except Exception as e:
```

### Comparing `diffusivity_step-2023.9.4/diffusivity_step/diffusivity_parameters.py` & `diffusivity_step-2024.5.26/diffusivity_step/diffusivity_parameters.py`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/diffusivity_step/diffusivity_step.py` & `diffusivity_step-2024.5.26/diffusivity_step/diffusivity_step.py`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/diffusivity_step/metadata.py` & `diffusivity_step-2024.5.26/diffusivity_step/metadata.py`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/diffusivity_step/tk_diffusivity.py` & `diffusivity_step-2024.5.26/diffusivity_step/tk_diffusivity.py`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/diffusivity_step.egg-info/PKG-INFO` & `diffusivity_step-2024.5.26/diffusivity_step.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: diffusivity-step
-Version: 2023.9.4
+Name: diffusivity_step
+Version: 2024.5.26
 Summary: A SEAMM plug-in for Diffusivity
 Home-page: https://github.com/molssi-seamm/diffusivity_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMplugin,flowchart
 Platform: Linux
@@ -20,14 +20,21 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: molsystem
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: seamm
+Requires-Dist: seamm-util
+Requires-Dist: seamm-widgets
+Requires-Dist: tabulate
 
 =========================
 SEAMM Diffusivity Plug-in
 =========================
 
 .. image:: https://img.shields.io/github/issues-pr-raw/molssi-seamm/diffusivity_step
    :target: https://github.com/molssi-seamm/diffusivity_step/pulls
@@ -80,15 +87,18 @@
 .. _MolSSI: https://molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
-
+2024.5.26 -- Updated for new task handling
+    * The new handling of running tasks such as LAMMPS required a small change in the
+      code.
+      
 2023.9.5 -- Changed default to using only MSD
     * The Helfand moments approach seems give incorrect results if the sampling time is
       too long. It is not dramatic, but gives increasingly incorrect results as the
       sampling time is increased. Thus using the Helfand moments is dangerous because
       the results may be wrong, but not obviously so.
 
 2023.8.30 -- Initial working version
```

### Comparing `diffusivity_step-2023.9.4/diffusivity_step.egg-info/SOURCES.txt` & `diffusivity_step-2024.5.26/diffusivity_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/Makefile` & `diffusivity_step-2024.5.26/docs/Makefile`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/_static/SEAMM Inverted 288x181.png` & `diffusivity_step-2024.5.26/docs/_static/SEAMM Inverted 288x181.png`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/_static/SEAMM logo.png` & `diffusivity_step-2024.5.26/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/_static/molssi_main_logo.png` & `diffusivity_step-2024.5.26/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/_static/molssi_main_logo_inverted_white.png` & `diffusivity_step-2024.5.26/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/_static/molssi_square.png` & `diffusivity_step-2024.5.26/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/_static/nsf.png` & `diffusivity_step-2024.5.26/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/conf.py` & `diffusivity_step-2024.5.26/docs/conf.py`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/developer_guide/installation.rst` & `diffusivity_step-2024.5.26/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/getting_started/index.rst` & `diffusivity_step-2024.5.26/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/index.rst` & `diffusivity_step-2024.5.26/docs/index.rst`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/make.bat` & `diffusivity_step-2024.5.26/docs/make.bat`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/docs/user_guide/index.rst` & `diffusivity_step-2024.5.26/docs/user_guide/index.rst`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/setup.py` & `diffusivity_step-2024.5.26/setup.py`

 * *Files identical despite different names*

### Comparing `diffusivity_step-2023.9.4/versioneer.py` & `diffusivity_step-2024.5.26/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -272,15 +273,14 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
-
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,59 +304,54 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = (
-            "Versioneer was unable to run the project root directory. "
-            "Versioneer requires setup.py to be executed from "
-            "its immediate directory (like 'python setup.py COMMAND'), "
-            "or in a way that lets it use sys.argv[0] to find the root "
-            "(like 'python path/to/setup.py COMMAND')."
-        )
+        err = ("Versioneer was unable to run the project root directory. "
+               "Versioneer requires setup.py to be executed from "
+               "its immediate directory (like 'python setup.py COMMAND'), "
+               "or in a way that lets it use sys.argv[0] to find the root "
+               "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print(
-                "Warning: build in %s is using versioneer.py from %s"
-                % (os.path.dirname(me), versioneer_py)
-            )
+            print("Warning: build in %s is using versioneer.py from %s"
+                  % (os.path.dirname(me), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
+    parser = configparser.ConfigParser()
     with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+        parser.read_file(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
-
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -373,40 +368,36 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
-
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
-
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
+                env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen(
-                [c] + args,
-                cwd=cwd,
-                env=env,
-                stdout=subprocess.PIPE,
-                stderr=(subprocess.PIPE if hide_stderr else None),
-            )
+            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
+                                 stdout=subprocess.PIPE,
+                                 stderr=(subprocess.PIPE if hide_stderr
+                                         else None))
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -423,17 +414,15 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY[
-    "git"
-] = '''
+LONG_VERSION_PY['git'] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -1000,86 +989,71 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r"\d", r)])
+        tags = set([r for r in refs if re.search(r'\d', r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix) :]
+            r = ref[len(tag_prefix):]
             if verbose:
                 print("picking %s" % r)
-            return {
-                "version": r,
-                "full-revisionid": keywords["full"].strip(),
-                "dirty": False,
-                "error": None,
-                "date": date,
-            }
+            return {"version": r,
+                    "full-revisionid": keywords["full"].strip(),
+                    "dirty": False, "error": None,
+                    "date": date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {
-        "version": "0+unknown",
-        "full-revisionid": keywords["full"].strip(),
-        "dirty": False,
-        "error": "no suitable tags",
-        "date": None,
-    }
+    return {"version": "0+unknown",
+            "full-revisionid": keywords["full"].strip(),
+            "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
+                          hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(
-        GITS,
-        [
-            "describe",
-            "--tags",
-            "--dirty",
-            "--always",
-            "--long",
-            "--match",
-            "%s*" % tag_prefix,
-        ],
-        cwd=root,
-    )
+    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
+                                          "--always", "--long",
+                                          "--match", "%s*" % tag_prefix],
+                                   cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1094,55 +1068,54 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[: git_describe.rindex("-dirty")]
+        git_describe = git_describe[:git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
+        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
+            pieces["error"] = ("unable to parse git-describe output: '%s'"
+                               % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
-                full_tag,
-                tag_prefix,
-            )
+            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
+                               % (full_tag, tag_prefix))
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
+        pieces["closest-tag"] = full_tag[len(tag_prefix):]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
+                                    cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[
-        0
-    ].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
+                       cwd=root)[0].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1190,30 +1163,24 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {
-                "version": dirname[len(parentdir_prefix) :],
-                "full-revisionid": None,
-                "dirty": False,
-                "error": None,
-                "date": None,
-            }
+            return {"version": dirname[len(parentdir_prefix):],
+                    "full-revisionid": None,
+                    "dirty": False, "error": None, "date": None}
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print(
-            "Tried directories %s but none started with prefix %s"
-            % (str(rootdirs), parentdir_prefix)
-        )
+        print("Tried directories %s but none started with prefix %s" %
+              (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1234,30 +1201,29 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(
-        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-    )
+    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
+                   contents, re.M | re.S)
     if not mo:
-        mo = re.search(
-            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
-        )
+        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
+                       contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True,
+                          indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1281,15 +1247,16 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
+                                          pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1395,21 +1362,19 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {
-            "version": "unknown",
-            "full-revisionid": pieces.get("long"),
-            "dirty": None,
-            "error": pieces["error"],
-            "date": None,
-        }
+        return {"version": "unknown",
+                "full-revisionid": pieces.get("long"),
+                "dirty": None,
+                "error": pieces["error"],
+                "date": None}
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1421,21 +1386,17 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {
-        "version": rendered,
-        "full-revisionid": pieces["long"],
-        "dirty": pieces["dirty"],
-        "error": None,
-        "date": pieces.get("date"),
-    }
+    return {"version": rendered, "full-revisionid": pieces["long"],
+            "dirty": pieces["dirty"], "error": None,
+            "date": pieces.get("date")}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1450,17 +1411,16 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert (
-        cfg.versionfile_source is not None
-    ), "please set versioneer.versionfile_source"
+    assert cfg.versionfile_source is not None, \
+        "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1506,21 +1466,17 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {
-        "version": "0+unknown",
-        "full-revisionid": None,
-        "dirty": None,
-        "error": "unable to compute version",
-        "date": None,
-    }
+    return {"version": "0+unknown", "full-revisionid": None,
+            "dirty": None, "error": "unable to compute version",
+            "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1561,15 +1517,14 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
-
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1594,23 +1549,22 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib,
+                                                  cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
-
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
-
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1623,29 +1577,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if "py2exe" in sys.modules:  # py2exe enabled?
+    if 'py2exe' in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1656,25 +1606,21 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(
-                        LONG
-                        % {
-                            "DOLLAR": "$",
-                            "STYLE": cfg.style,
-                            "TAG_PREFIX": cfg.tag_prefix,
-                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        }
-                    )
-
+                    f.write(LONG %
+                            {"DOLLAR": "$",
+                             "STYLE": cfg.style,
+                             "TAG_PREFIX": cfg.tag_prefix,
+                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                             })
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1693,18 +1639,16 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(
-                target_versionfile, self._versioneer_generated_versions
-            )
-
+            write_to_version_file(target_versionfile,
+                                  self._versioneer_generated_versions)
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1751,41 +1695,36 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (
-        EnvironmentError,
-        configparser.NoSectionError,
-        configparser.NoOptionError,
-    ) as e:
+    except (EnvironmentError, configparser.NoSectionError,
+            configparser.NoOptionError) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg",
+                  file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(
-            LONG
-            % {
-                "DOLLAR": "$",
-                "STYLE": cfg.style,
-                "TAG_PREFIX": cfg.tag_prefix,
-                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                "VERSIONFILE_SOURCE": cfg.versionfile_source,
-            }
-        )
+        f.write(LONG % {"DOLLAR": "$",
+                        "STYLE": cfg.style,
+                        "TAG_PREFIX": cfg.tag_prefix,
+                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        })
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
+                       "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1819,18 +1758,16 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(
-            " appending versionfile_source ('%s') to MANIFEST.in"
-            % cfg.versionfile_source
-        )
+        print(" appending versionfile_source ('%s') to MANIFEST.in" %
+              cfg.versionfile_source)
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

