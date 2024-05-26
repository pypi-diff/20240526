# Comparing `tmp/intellikit-0.0.4.tar.gz` & `tmp/intellikit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellikit-0.0.4.tar", last modified: Mon Apr 15 00:06:51 2024, max compression
+gzip compressed data, was "intellikit-0.0.5.tar", last modified: Sun May 26 02:35:37 2024, max compression
```

## Comparing `intellikit-0.0.4.tar` & `intellikit-0.0.5.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-15 00:06:40.000000 intellikit-0.0.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.216092 intellikit-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.220092 intellikit-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.220092 intellikit-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-15 00:06:40.000000 intellikit-0.0.4/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-15 00:06:40.000000 intellikit-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:06:40.000000 intellikit-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 00:06:40.000000 intellikit-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-15 00:06:51.228092 intellikit-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-15 00:06:40.000000 intellikit-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/Car_Search_System.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/Document_Search_System.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/Recommendation_System.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/docs/examples/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)    81283 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/datasets/cars-1k.csv
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    90528 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/examples/similarity_output.csv
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/intellikit.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/ir.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/sim.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-15 00:06:40.000000 intellikit-0.0.4/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.224092 intellikit-0.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-15 00:06:40.000000 intellikit-0.0.4/examples/Car_Search_System.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/examples/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)    81283 2024-04-15 00:06:40.000000 intellikit-0.0.4/examples/datasets/cars-1k.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:40.000000 intellikit-0.0.4/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    90528 2024-04-15 00:06:40.000000 intellikit-0.0.4/examples/similarity_output.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/intellikit/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/intellikit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-15 00:06:40.000000 intellikit-0.0.4/intellikit/sim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/intellikit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 00:06:51.000000 intellikit-0.0.4/intellikit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-15 00:06:40.000000 intellikit-0.0.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-15 00:06:40.000000 intellikit-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 00:06:40.000000 intellikit-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-15 00:06:40.000000 intellikit-0.0.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:06:51.228092 intellikit-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:06:51.228092 intellikit-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 00:06:40.000000 intellikit-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-15 00:06:40.000000 intellikit-0.0.4/tests/test_intellikit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.938504 intellikit-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-26 02:35:25.000000 intellikit-0.0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.926504 intellikit-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.930504 intellikit-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.930504 intellikit-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-26 02:35:25.000000 intellikit-0.0.5/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-26 02:35:25.000000 intellikit-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 02:35:25.000000 intellikit-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-26 02:35:25.000000 intellikit-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-26 02:35:37.938504 intellikit-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-26 02:35:25.000000 intellikit-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.930504 intellikit-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.934504 intellikit-0.0.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/examples/Car_Search_System.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13665 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/examples/Document_Search_System.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/examples/Recommendation_System.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.934504 intellikit-0.0.5/docs/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    81283 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/examples/datasets/cars-1k.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    90528 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/examples/similarity_output.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/intellikit.md
+-rw-r--r--   0 runner    (1001) docker     (127)    55165 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/intellikit_package.png
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/ir.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.934504 intellikit-0.0.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/sim.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-26 02:35:25.000000 intellikit-0.0.5/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.934504 intellikit-0.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-26 02:35:25.000000 intellikit-0.0.5/examples/Car_Search_System.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.934504 intellikit-0.0.5/examples/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)    81283 2024-05-26 02:35:25.000000 intellikit-0.0.5/examples/datasets/cars-1k.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:25.000000 intellikit-0.0.5/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    90528 2024-05-26 02:35:25.000000 intellikit-0.0.5/examples/similarity_output.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.934504 intellikit-0.0.5/intellikit/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-26 02:35:25.000000 intellikit-0.0.5/intellikit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7608 2024-05-26 02:35:25.000000 intellikit-0.0.5/intellikit/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-26 02:35:25.000000 intellikit-0.0.5/intellikit/intellikit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-26 02:35:25.000000 intellikit-0.0.5/intellikit/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14463 2024-05-26 02:35:25.000000 intellikit-0.0.5/intellikit/sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.934504 intellikit-0.0.5/intellikit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-26 02:35:37.000000 intellikit-0.0.5/intellikit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-26 02:35:37.000000 intellikit-0.0.5/intellikit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 02:35:37.000000 intellikit-0.0.5/intellikit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-26 02:35:37.000000 intellikit-0.0.5/intellikit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-26 02:35:37.000000 intellikit-0.0.5/intellikit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 02:35:37.000000 intellikit-0.0.5/intellikit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-26 02:35:25.000000 intellikit-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-26 02:35:25.000000 intellikit-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-26 02:35:25.000000 intellikit-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-26 02:35:25.000000 intellikit-0.0.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 02:35:37.938504 intellikit-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 02:35:37.934504 intellikit-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-26 02:35:25.000000 intellikit-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-26 02:35:25.000000 intellikit-0.0.5/tests/test_intellikit.py
```

### Comparing `intellikit-0.0.4/.github/ISSUE_TEMPLATE/config.yml` & `intellikit-0.0.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/.github/workflows/docs-build.yml` & `intellikit-0.0.5/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/.github/workflows/docs.yml` & `intellikit-0.0.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/.github/workflows/installation.yml` & `intellikit-0.0.5/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/.github/workflows/macos.yml` & `intellikit-0.0.5/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/.github/workflows/pypi.yml` & `intellikit-0.0.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/.github/workflows/ubuntu.yml` & `intellikit-0.0.5/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/.github/workflows/windows.yml` & `intellikit-0.0.5/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/.gitignore` & `intellikit-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/PKG-INFO` & `intellikit-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellikit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python toolkit for case based reasoning, information retrieval, natural language processing and other techniques for AI and intelligent systems.
 Author-email: Arthur Kakande <kaksarthur@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ArthurKakande/intellikit
 Keywords: intellikit
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intellikit-0.0.4/README.md` & `intellikit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/docs/contributing.md` & `intellikit-0.0.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/docs/examples/Car_Search_System.ipynb` & `intellikit-0.0.5/docs/examples/Car_Search_System.ipynb`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/docs/examples/Document_Search_System.ipynb` & `intellikit-0.0.5/docs/examples/Document_Search_System.ipynb`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/docs/examples/datasets/cars-1k.csv` & `intellikit-0.0.5/docs/examples/datasets/cars-1k.csv`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/docs/examples/similarity_output.csv` & `intellikit-0.0.5/docs/examples/similarity_output.csv`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/docs/installation.md` & `intellikit-0.0.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/examples/Car_Search_System.ipynb` & `intellikit-0.0.5/examples/Car_Search_System.ipynb`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/examples/datasets/cars-1k.csv` & `intellikit-0.0.5/examples/datasets/cars-1k.csv`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/examples/similarity_output.csv` & `intellikit-0.0.5/examples/similarity_output.csv`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/intellikit/intellikit.py` & `intellikit-0.0.5/intellikit/intellikit.py`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/intellikit/ir.py` & `intellikit-0.0.5/intellikit/ir.py`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/intellikit.egg-info/PKG-INFO` & `intellikit-0.0.5/intellikit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellikit
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python toolkit for case based reasoning, information retrieval, natural language processing and other techniques for AI and intelligent systems.
 Author-email: Arthur Kakande <kaksarthur@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ArthurKakande/intellikit
 Keywords: intellikit
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intellikit-0.0.4/intellikit.egg-info/SOURCES.txt` & `intellikit-0.0.5/intellikit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 docs/changelog.md
 docs/common.md
 docs/contributing.md
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/intellikit.md
+docs/intellikit_package.png
 docs/ir.md
 docs/sim.md
 docs/usage.md
 docs/examples/Car_Search_System.ipynb
 docs/examples/Document_Search_System.ipynb
 docs/examples/Recommendation_System.ipynb
 docs/examples/intro.ipynb
```

### Comparing `intellikit-0.0.4/mkdocs.yml` & `intellikit-0.0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `intellikit-0.0.4/pyproject.toml` & `intellikit-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "intellikit"
-version = "0.0.4"
+version = "0.0.5"
 dynamic = [
     "dependencies",
 ]
 description = "A python toolkit for case based reasoning, information retrieval, natural language processing and other techniques for AI and intelligent systems."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.4"
+current_version = "0.0.5"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

