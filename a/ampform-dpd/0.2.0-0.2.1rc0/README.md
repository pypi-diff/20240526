# Comparing `tmp/ampform_dpd-0.2.0.tar.gz` & `tmp/ampform_dpd-0.2.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampform_dpd-0.2.0.tar", last modified: Mon Apr 29 09:03:00 2024, max compression
+gzip compressed data, was "ampform_dpd-0.2.1rc0.tar", last modified: Sun May 26 09:17:55 2024, max compression
```

## Comparing `ampform_dpd-0.2.0.tar` & `ampform_dpd-0.2.1rc0.tar`

### file list

```diff
@@ -1,83 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.244320 ampform_dpd-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.228320 ampform_dpd-0.2.0/.constraints/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.constraints/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.constraints/py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.constraints/py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.constraints/py3.12.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.constraints/py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.constraints/py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.cspell.json
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.228320 ampform_dpd-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.232320 ampform_dpd-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.github/workflows/clean-caches.yml
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.github/workflows/pr-linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.github/workflows/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.gitpod.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.taplo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.232320 ampform_dpd-0.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-29 09:03:00.244320 ampform_dpd-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.232320 ampform_dpd-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.232320 ampform_dpd-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.236320 ampform_dpd-0.2.0/docs/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)    28057 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/comparison/d2kkk.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    27534 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/comparison/jpsi2phipipi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    27353 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/comparison/jpsi2pipipi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/comparison.md
--rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    15048 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/jpsi2ksp.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8053 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/lc2pkpi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (127)    15383 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/docs/xib2pkk.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 09:03:00.244320 ampform_dpd-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.224320 ampform_dpd-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.236320 ampform_dpd-0.2.0/src/ampform_dpd/
--rw-r--r--   0 runner    (1001) docker     (127)    16582 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.236320 ampform_dpd-0.2.0/src/ampform_dpd/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/adapter/qrules.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/angles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/decay.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.236320 ampform_dpd-0.2.0/src/ampform_dpd/dynamics/
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/dynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/dynamics/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/particle-definitions.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/src/ampform_dpd/spin.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 09:03:00.000000 ampform_dpd-0.2.0/src/ampform_dpd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.240320 ampform_dpd-0.2.0/src/ampform_dpd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-29 09:03:00.000000 ampform_dpd-0.2.0/src/ampform_dpd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-29 09:03:00.000000 ampform_dpd-0.2.0/src/ampform_dpd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:03:00.000000 ampform_dpd-0.2.0/src/ampform_dpd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-29 09:03:00.000000 ampform_dpd-0.2.0/src/ampform_dpd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 09:03:00.000000 ampform_dpd-0.2.0/src/ampform_dpd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.240320 ampform_dpd-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:03:00.240320 ampform_dpd-0.2.0/tests/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/tests/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/tests/adapter/test_qrules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/tests/test_angles.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/tests/test_decay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-29 09:02:52.000000 ampform_dpd-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.269454 ampform_dpd-0.2.1rc0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.253454 ampform_dpd-0.2.1rc0/.constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.constraints/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.constraints/py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.constraints/py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.constraints/py3.12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.constraints/py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.constraints/py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.cspell.json
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.253454 ampform_dpd-0.2.1rc0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.253454 ampform_dpd-0.2.1rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.github/workflows/clean-caches.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.github/workflows/pr-linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.github/workflows/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.gitpod.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.taplo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.253454 ampform_dpd-0.2.1rc0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-26 09:17:55.269454 ampform_dpd-0.2.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.257454 ampform_dpd-0.2.1rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26138 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/Lc2ppiK.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.257454 ampform_dpd-0.2.1rc0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.257454 ampform_dpd-0.2.1rc0/docs/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)    28082 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/comparison/d2kkk.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27559 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/comparison/jpsi2phipipi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27378 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/comparison/jpsi2pipipi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/comparison.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15059 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/jpsi2ksp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/lc2pkpi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/serialization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15394 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/docs/xib2pkk.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 09:17:55.269454 ampform_dpd-0.2.1rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.249454 ampform_dpd-0.2.1rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.257454 ampform_dpd-0.2.1rc0/src/ampform_dpd/
+-rw-r--r--   0 runner    (1001) docker     (127)    17586 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.261454 ampform_dpd-0.2.1rc0/src/ampform_dpd/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/adapter/qrules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/decay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.261454 ampform_dpd-0.2.1rc0/src/ampform_dpd/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/dynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/dynamics/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.261454 ampform_dpd-0.2.1rc0/src/ampform_dpd/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.261454 ampform_dpd-0.2.1rc0/src/ampform_dpd/io/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/io/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/io/serialization/amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/io/serialization/decay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/io/serialization/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/io/serialization/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/particle-definitions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/spin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-26 09:17:55.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.265454 ampform_dpd-0.2.1rc0/src/ampform_dpd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-26 09:17:55.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-26 09:17:55.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 09:17:55.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-26 09:17:55.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-26 09:17:55.000000 ampform_dpd-0.2.1rc0/src/ampform_dpd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.261454 ampform_dpd-0.2.1rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.261454 ampform_dpd-0.2.1rc0/tests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/adapter/test_qrules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:55.265454 ampform_dpd-0.2.1rc0/tests/io_serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/io_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/io_serialization/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/io_serialization/test_amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/io_serialization/test_decay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/io_serialization/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/test_angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/test_decay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-26 09:17:51.000000 ampform_dpd-0.2.1rc0/tox.ini
```

### Comparing `ampform_dpd-0.2.0/.constraints/py3.10.txt` & `ampform_dpd-0.2.1rc0/.constraints/py3.8.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,237 +1,246 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile pyproject.toml -o .constraints/py3.10.txt --all-extras --no-annotate --python-version=3.10 --no-emit-package setuptools
+#    uv pip compile pyproject.toml -o .constraints/py3.8.txt --all-extras --no-annotate --python-version=3.8 --no-emit-package setuptools
 absl-py==2.1.0
 accessible-pygments==0.0.4
-alabaster==0.7.16
-ampform==0.15.0
+alabaster==0.7.13
+ampform==0.15.4
 anyio==4.3.0
 argon2-cffi==23.1.0
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
-babel==2.14.0
+babel==2.15.0
+backcall==0.2.0
 beautifulsoup4==4.12.3
-black==24.4.0
+black==24.4.2
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
-contourpy==1.2.1
-coverage==7.5.0
+contourpy==1.1.1
+coverage==7.5.1
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
-docutils==0.21.2
+docutils==0.17.1
 exceptiongroup==1.2.1
 execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.4
+filelock==3.14.0
 flatbuffers==24.3.25
-fonttools==4.51.0
+fonttools==4.52.1
 fqdn==1.5.1
-gast==0.5.4
+gast==0.4.0
 gitdb==4.0.11
 gitpython==3.1.43
+google-auth==2.29.0
+google-auth-oauthlib==0.4.6
 google-pasta==0.2.0
 graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.2
+grpcio==1.64.0
 h11==0.14.0
 h5py==3.11.0
 hepunits==2.3.3
 httpcore==1.0.5
 httpx==0.27.0
 identify==2.5.36
 idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
 importlib-metadata==7.1.0
+importlib-resources==6.4.0
 iniconfig==2.0.0
 ipykernel==6.29.4
-ipympl==0.9.4
-ipython==8.23.0
+ipympl==0.9.3
+ipython==8.12.3
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
-jax==0.4.26
-jaxlib==0.4.26
+jax==0.4.13
+jaxlib==0.4.13
 jedi==0.19.1
-jinja2==3.1.3
+jinja2==3.1.4
 json5==0.9.25
 jsonpointer==2.4
-jsonschema==4.21.1
+jsonschema==4.22.0
 jsonschema-specifications==2023.12.1
-jupyter-cache==1.0.0
-jupyter-client==8.6.1
+jupyter-cache==0.6.1
+jupyter-client==8.6.2
 jupyter-core==5.7.2
 jupyter-events==0.10.0
 jupyter-lsp==2.2.5
 jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.6
+jupyterlab==4.2.1
 jupyterlab-code-formatter==2.2.1
-jupyterlab-git==0.50.0
+jupyterlab-git==0.50.1
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.2
+jupyterlab-myst==2.4.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.27.1
+jupyterlab-server==2.27.2
 jupyterlab-widgets==3.0.10
-keras==3.3.2
+keras==2.11.0
 kiwisolver==1.4.5
 latexcodec==3.0.0
 libclang==18.1.1
-llvmlite==0.42.0
+livereload==2.6.3
+llvmlite==0.41.1
 lsprotocol==2023.0.1
 markdown==3.6
-markdown-it-py==3.0.0
+markdown-it-py==2.2.0
 markupsafe==2.1.5
-matplotlib==3.8.4
+matplotlib==3.7.5
 matplotlib-inline==0.1.7
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.3.5
 mdurl==0.1.2
 mistune==3.0.2
-ml-dtypes==0.3.2
+ml-dtypes==0.2.0
 mpmath==1.3.0
+mypy==1.10.0
 mypy-extensions==1.0.0
-myst-nb==1.1.0
-myst-parser==3.0.0
-namex==0.0.8
+myst-nb==0.17.2
+myst-parser==0.18.1
 nbclient==0.6.8
-nbconvert==7.16.3
+nbconvert==7.16.4
 nbdime==4.0.1
 nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
-numba==0.59.1
-numpy==1.26.4
+numba==0.58.1
+numpy==1.24.4
+oauthlib==3.2.2
 opt-einsum==3.3.0
-optree==0.11.0
 overrides==7.7.0
 packaging==24.0
 pandocfilters==1.5.1
 parso==0.8.4
 particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
-phasespace==1.10.3
+phasespace==1.9.0
+pickleshare==0.7.5
 pillow==10.3.0
-platformdirs==4.2.1
+pkgutil-resolve-name==1.3.10
+platformdirs==4.2.2
 pluggy==1.5.0
-pre-commit==3.7.0
+pre-commit==3.5.0
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
-protobuf==4.25.3
+protobuf==3.19.6
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
+pyasn1==0.6.0
+pyasn1-modules==0.4.0
 pybtex==0.24.0
 pybtex-docutils==1.0.3
 pycparser==2.22
-pydata-sphinx-theme==0.15.2
-pygments==2.17.2
+pydata-sphinx-theme==0.14.4
+pygments==2.18.0
 pyparsing==3.1.2
 pyproject-api==1.6.1
-pytest==8.1.1
+pytest==8.2.1
 pytest-cov==5.0.0
-pytest-xdist==3.5.0
-python-constraint==1.4.0
+pytest-xdist==3.6.1
+python-constraint2==2.0.0b5
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
-python-lsp-ruff==2.2.0
+python-lsp-ruff==2.2.1
 python-lsp-server==1.11.0
 pytoolconfig==1.3.1
+pytz==2024.1
 pyyaml==6.0.1
-pyzmq==26.0.2
-qrules==0.10.1
-referencing==0.35.0
-requests==2.31.0
+pyzmq==26.0.3
+qrules==0.10.2
+referencing==0.35.1
+requests==2.32.2
+requests-oauthlib==2.0.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
-rich==13.7.1
 rope==1.13.0
-rpds-py==0.18.0
-ruff==0.4.1
-scipy==1.13.0
+rpds-py==0.18.1
+rsa==4.9
+ruff==0.4.5
+scipy==1.10.1
 send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
-sphinx==7.3.7
+sphinx==5.3.0
 sphinx-api-relink==0.0.9
-sphinx-autobuild==2024.4.16
-sphinx-book-theme==1.1.2
+sphinx-autobuild==2021.3.14
+sphinx-book-theme==1.0.1
 sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
 sphinx-design==0.5.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
-sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-bibtex==2.6.2
-sphinxcontrib-devhelp==1.0.6
-sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
-sphinxcontrib-qthelp==1.0.7
-sphinxcontrib-serializinghtml==1.1.10
-sqlalchemy==2.0.29
+sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-serializinghtml==1.1.5
+sqlalchemy==2.0.30
 stack-data==0.6.3
-starlette==0.37.2
 sympy==1.12
 tabulate==0.9.0
-tensorboard==2.16.2
-tensorboard-data-server==0.7.2
-tensorflow==2.16.1
-tensorflow-io-gcs-filesystem==0.36.0
-tensorflow-probability==0.24.0
+tensorboard==2.11.2
+tensorboard-data-server==0.6.1
+tensorboard-plugin-wit==1.8.1
+tensorflow==2.11.1
+tensorflow-estimator==2.11.0
+tensorflow-io-gcs-filesystem==0.34.0
+tensorflow-probability==0.20.1
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
 tinycss2==1.3.0
 tomli==2.0.1
 tornado==6.4
-tox==4.14.2
-tqdm==4.66.2
+tox==4.15.0
+tqdm==4.66.4
 traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.11.0
-ujson==5.9.0
+typing-extensions==4.12.0
+ujson==5.10.0
 uri-template==1.3.0
 urllib3==2.2.1
-uvicorn==0.29.0
-virtualenv==20.26.0
-watchfiles==0.21.0
+virtualenv==20.26.2
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
 websocket-client==1.8.0
-websockets==12.0
-werkzeug==3.0.2
+werkzeug==3.0.3
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
-zipp==3.18.1
+zipp==3.18.2
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform_dpd-0.2.0/.constraints/py3.11.txt` & `ampform_dpd-0.2.1rc0/.constraints/py3.11.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile pyproject.toml -o .constraints/py3.11.txt --all-extras --no-annotate --python-version=3.11 --no-emit-package setuptools
 absl-py==2.1.0
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
 alabaster==0.7.16
-ampform==0.15.0
+ampform==0.15.4
 anyio==4.3.0
 argon2-cffi==23.1.0
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
-babel==2.14.0
+babel==2.15.0
 beautifulsoup4==4.12.3
-black==24.4.0
+black==24.4.2
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
 contourpy==1.2.1
-coverage==7.5.0
+coverage==7.5.1
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
 docutils==0.21.2
 execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.4
+filelock==3.14.0
 flatbuffers==24.3.25
-fonttools==4.51.0
+fonttools==4.52.1
 fqdn==1.5.1
 gast==0.5.4
 gitdb==4.0.11
 gitpython==3.1.43
 google-pasta==0.2.0
 graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.2
+grpcio==1.64.0
 h11==0.14.0
 h5py==3.11.0
 hepunits==2.3.3
 httpcore==1.0.5
 httpx==0.27.0
 identify==2.5.36
 idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
 importlib-metadata==7.1.0
 iniconfig==2.0.0
 ipykernel==6.29.4
 ipympl==0.9.4
-ipython==8.23.0
+ipython==8.24.0
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
-jax==0.4.26
-jaxlib==0.4.26
+jax==0.4.28
+jaxlib==0.4.28
 jedi==0.19.1
-jinja2==3.1.3
+jinja2==3.1.4
 json5==0.9.25
 jsonpointer==2.4
-jsonschema==4.21.1
+jsonschema==4.22.0
 jsonschema-specifications==2023.12.1
 jupyter-cache==1.0.0
-jupyter-client==8.6.1
+jupyter-client==8.6.2
 jupyter-core==5.7.2
 jupyter-events==0.10.0
 jupyter-lsp==2.2.5
 jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.6
+jupyterlab==4.2.1
 jupyterlab-code-formatter==2.2.1
-jupyterlab-git==0.50.0
+jupyterlab-git==0.50.1
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.2
+jupyterlab-myst==2.4.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.27.1
+jupyterlab-server==2.27.2
 jupyterlab-widgets==3.0.10
-keras==3.3.2
+keras==3.3.3
 kiwisolver==1.4.5
 latexcodec==3.0.0
 libclang==18.1.1
+livereload==2.6.3
 llvmlite==0.42.0
 lsprotocol==2023.0.1
 markdown==3.6
 markdown-it-py==3.0.0
 markupsafe==2.1.5
-matplotlib==3.8.4
+matplotlib==3.9.0
 matplotlib-inline==0.1.7
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
 mdurl==0.1.2
 mistune==3.0.2
 ml-dtypes==0.3.2
 mpmath==1.3.0
+mypy==1.10.0
 mypy-extensions==1.0.0
 myst-nb==1.1.0
-myst-parser==3.0.0
+myst-parser==3.0.1
 namex==0.0.8
 nbclient==0.6.8
-nbconvert==7.16.3
+nbconvert==7.16.4
 nbdime==4.0.1
 nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
 numba==0.59.1
@@ -130,106 +132,102 @@
 pandocfilters==1.5.1
 parso==0.8.4
 particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
 phasespace==1.10.3
 pillow==10.3.0
-platformdirs==4.2.1
+platformdirs==4.2.2
 pluggy==1.5.0
-pre-commit==3.7.0
+pre-commit==3.7.1
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
 protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pybtex==0.24.0
 pybtex-docutils==1.0.3
 pycparser==2.22
 pydata-sphinx-theme==0.15.2
-pygments==2.17.2
+pygments==2.18.0
 pyparsing==3.1.2
 pyproject-api==1.6.1
-pytest==8.1.1
+pytest==8.2.1
 pytest-cov==5.0.0
-pytest-xdist==3.5.0
-python-constraint==1.4.0
+pytest-xdist==3.6.1
+python-constraint2==2.0.0b5
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
-python-lsp-ruff==2.2.0
+python-lsp-ruff==2.2.1
 python-lsp-server==1.11.0
 pytoolconfig==1.3.1
 pyyaml==6.0.1
-pyzmq==26.0.2
-qrules==0.10.1
-referencing==0.35.0
-requests==2.31.0
+pyzmq==26.0.3
+qrules==0.10.2
+referencing==0.35.1
+requests==2.32.2
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rich==13.7.1
 rope==1.13.0
-rpds-py==0.18.0
-ruff==0.4.1
-scipy==1.13.0
+rpds-py==0.18.1
+ruff==0.4.5
+scipy==1.13.1
 send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
 sphinx==7.3.7
 sphinx-api-relink==0.0.9
-sphinx-autobuild==2024.4.16
+sphinx-autobuild==2024.2.4
 sphinx-book-theme==1.1.2
 sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
-sphinx-design==0.5.0
+sphinx-design==0.6.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.8
 sphinxcontrib-bibtex==2.6.2
 sphinxcontrib-devhelp==1.0.6
 sphinxcontrib-htmlhelp==2.0.5
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.7
 sphinxcontrib-serializinghtml==1.1.10
-sqlalchemy==2.0.29
+sqlalchemy==2.0.30
 stack-data==0.6.3
-starlette==0.37.2
 sympy==1.12
 tabulate==0.9.0
 tensorboard==2.16.2
 tensorboard-data-server==0.7.2
 tensorflow==2.16.1
-tensorflow-io-gcs-filesystem==0.36.0
+tensorflow-io-gcs-filesystem==0.37.0
 tensorflow-probability==0.24.0
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
 tinycss2==1.3.0
 tornado==6.4
-tox==4.14.2
-tqdm==4.66.2
+tox==4.15.0
+tqdm==4.66.4
 traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.11.0
-ujson==5.9.0
+typing-extensions==4.12.0
+ujson==5.10.0
 uri-template==1.3.0
 urllib3==2.2.1
-uvicorn==0.29.0
-virtualenv==20.26.0
-watchfiles==0.21.0
+virtualenv==20.26.2
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
 websocket-client==1.8.0
-websockets==12.0
-werkzeug==3.0.2
+werkzeug==3.0.3
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
-zipp==3.18.1
+zipp==3.18.2
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform_dpd-0.2.0/.constraints/py3.12.txt` & `ampform_dpd-0.2.1rc0/.constraints/py3.12.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,124 +1,126 @@
 # This file was autogenerated by uv via the following command:
 #    uv pip compile pyproject.toml -o .constraints/py3.12.txt --all-extras --no-annotate --python-version=3.12 --no-emit-package setuptools
 absl-py==2.1.0
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
 alabaster==0.7.16
-ampform==0.15.0
+ampform==0.15.4
 anyio==4.3.0
 argon2-cffi==23.1.0
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
-babel==2.14.0
+babel==2.15.0
 beautifulsoup4==4.12.3
-black==24.4.0
+black==24.4.2
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
 contourpy==1.2.1
-coverage==7.5.0
+coverage==7.5.1
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
 docutils==0.21.2
 execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.4
+filelock==3.14.0
 flatbuffers==24.3.25
-fonttools==4.51.0
+fonttools==4.52.1
 fqdn==1.5.1
 gast==0.5.4
 gitdb==4.0.11
 gitpython==3.1.43
 google-pasta==0.2.0
 graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.2
+grpcio==1.64.0
 h11==0.14.0
 h5py==3.11.0
 hepunits==2.3.3
 httpcore==1.0.5
 httpx==0.27.0
 identify==2.5.36
 idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
 importlib-metadata==7.1.0
 iniconfig==2.0.0
 ipykernel==6.29.4
 ipympl==0.9.4
-ipython==8.23.0
+ipython==8.24.0
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
-jax==0.4.26
-jaxlib==0.4.26
+jax==0.4.28
+jaxlib==0.4.28
 jedi==0.19.1
-jinja2==3.1.3
+jinja2==3.1.4
 json5==0.9.25
 jsonpointer==2.4
-jsonschema==4.21.1
+jsonschema==4.22.0
 jsonschema-specifications==2023.12.1
 jupyter-cache==1.0.0
-jupyter-client==8.6.1
+jupyter-client==8.6.2
 jupyter-core==5.7.2
 jupyter-events==0.10.0
 jupyter-lsp==2.2.5
 jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.6
+jupyterlab==4.2.1
 jupyterlab-code-formatter==2.2.1
-jupyterlab-git==0.50.0
+jupyterlab-git==0.50.1
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.2
+jupyterlab-myst==2.4.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.27.1
+jupyterlab-server==2.27.2
 jupyterlab-widgets==3.0.10
-keras==3.3.2
+keras==3.3.3
 kiwisolver==1.4.5
 latexcodec==3.0.0
 libclang==18.1.1
+livereload==2.6.3
 llvmlite==0.42.0
 lsprotocol==2023.0.1
 markdown==3.6
 markdown-it-py==3.0.0
 markupsafe==2.1.5
-matplotlib==3.8.4
+matplotlib==3.9.0
 matplotlib-inline==0.1.7
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
 mdurl==0.1.2
 mistune==3.0.2
 ml-dtypes==0.3.2
 mpmath==1.3.0
+mypy==1.10.0
 mypy-extensions==1.0.0
 myst-nb==1.1.0
-myst-parser==3.0.0
+myst-parser==3.0.1
 namex==0.0.8
 nbclient==0.6.8
-nbconvert==7.16.3
+nbconvert==7.16.4
 nbdime==4.0.1
 nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
 numba==0.59.1
@@ -130,105 +132,101 @@
 pandocfilters==1.5.1
 parso==0.8.4
 particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
 phasespace==1.10.3
 pillow==10.3.0
-platformdirs==4.2.1
+platformdirs==4.2.2
 pluggy==1.5.0
-pre-commit==3.7.0
+pre-commit==3.7.1
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
 protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pybtex==0.24.0
 pybtex-docutils==1.0.3
 pycparser==2.22
 pydata-sphinx-theme==0.15.2
-pygments==2.17.2
+pygments==2.18.0
 pyparsing==3.1.2
 pyproject-api==1.6.1
-pytest==8.1.1
+pytest==8.2.1
 pytest-cov==5.0.0
-pytest-xdist==3.5.0
-python-constraint==1.4.0
+pytest-xdist==3.6.1
+python-constraint2==2.0.0b5
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
-python-lsp-ruff==2.2.0
+python-lsp-ruff==2.2.1
 python-lsp-server==1.11.0
 pytoolconfig==1.3.1
 pyyaml==6.0.1
-pyzmq==26.0.2
-qrules==0.10.1
-referencing==0.35.0
-requests==2.31.0
+pyzmq==26.0.3
+qrules==0.10.2
+referencing==0.35.1
+requests==2.32.2
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rich==13.7.1
 rope==1.13.0
-rpds-py==0.18.0
-ruff==0.4.1
-scipy==1.13.0
+rpds-py==0.18.1
+ruff==0.4.5
+scipy==1.13.1
 send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
 sphinx==7.3.7
 sphinx-api-relink==0.0.9
-sphinx-autobuild==2024.4.16
+sphinx-autobuild==2024.2.4
 sphinx-book-theme==1.1.2
 sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
-sphinx-design==0.5.0
+sphinx-design==0.6.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.8
 sphinxcontrib-bibtex==2.6.2
 sphinxcontrib-devhelp==1.0.6
 sphinxcontrib-htmlhelp==2.0.5
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.7
 sphinxcontrib-serializinghtml==1.1.10
-sqlalchemy==2.0.29
+sqlalchemy==2.0.30
 stack-data==0.6.3
-starlette==0.37.2
 sympy==1.12
 tabulate==0.9.0
 tensorboard==2.16.2
 tensorboard-data-server==0.7.2
 tensorflow==2.16.1
 tensorflow-probability==0.24.0
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
 tinycss2==1.3.0
 tornado==6.4
-tox==4.14.2
-tqdm==4.66.2
+tox==4.15.0
+tqdm==4.66.4
 traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.11.0
-ujson==5.9.0
+typing-extensions==4.12.0
+ujson==5.10.0
 uri-template==1.3.0
 urllib3==2.2.1
-uvicorn==0.29.0
-virtualenv==20.26.0
-watchfiles==0.21.0
+virtualenv==20.26.2
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
 websocket-client==1.8.0
-websockets==12.0
-werkzeug==3.0.2
+werkzeug==3.0.3
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
-zipp==3.18.1
+zipp==3.18.2
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform_dpd-0.2.0/.constraints/py3.8.txt` & `ampform_dpd-0.2.1rc0/.constraints/py3.9.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,245 +1,236 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile pyproject.toml -o .constraints/py3.8.txt --all-extras --no-annotate --python-version=3.8 --no-emit-package setuptools
+#    uv pip compile pyproject.toml -o .constraints/py3.9.txt --all-extras --no-annotate --python-version=3.9 --no-emit-package setuptools
 absl-py==2.1.0
-accessible-pygments==0.0.4
-alabaster==0.7.13
-ampform==0.15.0
+accessible-pygments==0.0.5
+alabaster==0.7.16
+ampform==0.15.4
 anyio==4.3.0
 argon2-cffi==23.1.0
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
-babel==2.14.0
-backcall==0.2.0
+babel==2.15.0
 beautifulsoup4==4.12.3
-black==24.4.0
+black==24.4.2
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
-contourpy==1.1.1
-coverage==7.5.0
+contourpy==1.2.1
+coverage==7.5.1
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
-docutils==0.17.1
+docutils==0.21.2
 exceptiongroup==1.2.1
 execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.4
+filelock==3.14.0
 flatbuffers==24.3.25
-fonttools==4.51.0
+fonttools==4.52.1
 fqdn==1.5.1
-gast==0.4.0
+gast==0.5.4
 gitdb==4.0.11
 gitpython==3.1.43
-google-auth==2.29.0
-google-auth-oauthlib==0.4.6
 google-pasta==0.2.0
 graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.2
+grpcio==1.64.0
 h11==0.14.0
 h5py==3.11.0
 hepunits==2.3.3
 httpcore==1.0.5
 httpx==0.27.0
 identify==2.5.36
 idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
 importlib-metadata==7.1.0
 importlib-resources==6.4.0
 iniconfig==2.0.0
 ipykernel==6.29.4
-ipympl==0.9.3
-ipython==8.12.3
+ipympl==0.9.4
+ipython==8.18.1
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
-jax==0.4.13
-jaxlib==0.4.13
+jax==0.4.28
+jaxlib==0.4.28
 jedi==0.19.1
-jinja2==3.1.3
+jinja2==3.1.4
 json5==0.9.25
 jsonpointer==2.4
-jsonschema==4.21.1
+jsonschema==4.22.0
 jsonschema-specifications==2023.12.1
-jupyter-cache==0.6.1
-jupyter-client==8.6.1
+jupyter-cache==1.0.0
+jupyter-client==8.6.2
 jupyter-core==5.7.2
 jupyter-events==0.10.0
 jupyter-lsp==2.2.5
 jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.6
+jupyterlab==4.2.1
 jupyterlab-code-formatter==2.2.1
-jupyterlab-git==0.50.0
+jupyterlab-git==0.50.1
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.2
+jupyterlab-myst==2.4.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.27.1
+jupyterlab-server==2.27.2
 jupyterlab-widgets==3.0.10
-keras==2.11.0
+keras==3.3.3
 kiwisolver==1.4.5
 latexcodec==3.0.0
 libclang==18.1.1
 livereload==2.6.3
-llvmlite==0.41.1
+llvmlite==0.42.0
 lsprotocol==2023.0.1
 markdown==3.6
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
 markupsafe==2.1.5
-matplotlib==3.7.5
+matplotlib==3.9.0
 matplotlib-inline==0.1.7
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.1
 mdurl==0.1.2
 mistune==3.0.2
-ml-dtypes==0.2.0
+ml-dtypes==0.3.2
 mpmath==1.3.0
+mypy==1.10.0
 mypy-extensions==1.0.0
-myst-nb==0.17.2
-myst-parser==0.18.1
+myst-nb==1.1.0
+myst-parser==3.0.1
+namex==0.0.8
 nbclient==0.6.8
-nbconvert==7.16.3
+nbconvert==7.16.4
 nbdime==4.0.1
 nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
-numba==0.58.1
-numpy==1.24.4
-oauthlib==3.2.2
+numba==0.59.1
+numpy==1.26.4
 opt-einsum==3.3.0
+optree==0.11.0
 overrides==7.7.0
 packaging==24.0
 pandocfilters==1.5.1
 parso==0.8.4
 particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
-phasespace==1.9.0
-pickleshare==0.7.5
+phasespace==1.10.3
 pillow==10.3.0
-pkgutil-resolve-name==1.3.10
-platformdirs==4.2.1
+platformdirs==4.2.2
 pluggy==1.5.0
-pre-commit==3.5.0
+pre-commit==3.7.1
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
-protobuf==3.19.6
+protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
-pyasn1==0.6.0
-pyasn1-modules==0.4.0
 pybtex==0.24.0
 pybtex-docutils==1.0.3
 pycparser==2.22
-pydata-sphinx-theme==0.14.4
-pygments==2.17.2
+pydata-sphinx-theme==0.15.2
+pygments==2.18.0
 pyparsing==3.1.2
 pyproject-api==1.6.1
-pytest==8.1.1
+pytest==8.2.1
 pytest-cov==5.0.0
-pytest-xdist==3.5.0
-python-constraint==1.4.0
+pytest-xdist==3.6.1
+python-constraint2==2.0.0b5
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
-python-lsp-ruff==2.2.0
+python-lsp-ruff==2.2.1
 python-lsp-server==1.11.0
 pytoolconfig==1.3.1
-pytz==2024.1
 pyyaml==6.0.1
-pyzmq==26.0.2
-qrules==0.10.1
-referencing==0.35.0
-requests==2.31.0
-requests-oauthlib==2.0.0
+pyzmq==26.0.3
+qrules==0.10.2
+referencing==0.35.1
+requests==2.32.2
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
+rich==13.7.1
 rope==1.13.0
-rpds-py==0.18.0
-rsa==4.9
-ruff==0.4.1
-scipy==1.10.1
+rpds-py==0.18.1
+ruff==0.4.5
+scipy==1.13.1
 send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
-sphinx==5.3.0
+sphinx==7.3.7
 sphinx-api-relink==0.0.9
-sphinx-autobuild==2021.3.14
-sphinx-book-theme==1.0.1
+sphinx-autobuild==2024.2.4
+sphinx-book-theme==1.1.2
 sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
-sphinx-design==0.5.0
+sphinx-design==0.6.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
-sphinxcontrib-applehelp==1.0.4
+sphinxcontrib-applehelp==1.0.8
 sphinxcontrib-bibtex==2.6.2
-sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-htmlhelp==2.0.5
 sphinxcontrib-jsmath==1.0.1
-sphinxcontrib-qthelp==1.0.3
-sphinxcontrib-serializinghtml==1.1.5
-sqlalchemy==2.0.29
+sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-serializinghtml==1.1.10
+sqlalchemy==2.0.30
 stack-data==0.6.3
 sympy==1.12
 tabulate==0.9.0
-tensorboard==2.11.2
-tensorboard-data-server==0.6.1
-tensorboard-plugin-wit==1.8.1
-tensorflow==2.11.1
-tensorflow-estimator==2.11.0
-tensorflow-io-gcs-filesystem==0.34.0
-tensorflow-probability==0.20.1
+tensorboard==2.16.2
+tensorboard-data-server==0.7.2
+tensorflow==2.16.1
+tensorflow-io-gcs-filesystem==0.37.0
+tensorflow-probability==0.24.0
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
 tinycss2==1.3.0
 tomli==2.0.1
 tornado==6.4
-tox==4.14.2
-tqdm==4.66.2
+tox==4.15.0
+tqdm==4.66.4
 traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.11.0
-ujson==5.9.0
+typing-extensions==4.12.0
+ujson==5.10.0
 uri-template==1.3.0
 urllib3==2.2.1
-virtualenv==20.26.0
+virtualenv==20.26.2
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
 websocket-client==1.8.0
-werkzeug==3.0.2
+werkzeug==3.0.3
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
-zipp==3.18.1
+zipp==3.18.2
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform_dpd-0.2.0/.constraints/py3.9.txt` & `ampform_dpd-0.2.1rc0/.constraints/py3.10.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,126 +1,127 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile pyproject.toml -o .constraints/py3.9.txt --all-extras --no-annotate --python-version=3.9 --no-emit-package setuptools
+#    uv pip compile pyproject.toml -o .constraints/py3.10.txt --all-extras --no-annotate --python-version=3.10 --no-emit-package setuptools
 absl-py==2.1.0
-accessible-pygments==0.0.4
+accessible-pygments==0.0.5
 alabaster==0.7.16
-ampform==0.15.0
+ampform==0.15.4
 anyio==4.3.0
 argon2-cffi==23.1.0
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
-babel==2.14.0
+babel==2.15.0
 beautifulsoup4==4.12.3
-black==24.4.0
+black==24.4.2
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
 contourpy==1.2.1
-coverage==7.5.0
+coverage==7.5.1
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
 docutils==0.21.2
 exceptiongroup==1.2.1
 execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.4
+filelock==3.14.0
 flatbuffers==24.3.25
-fonttools==4.51.0
+fonttools==4.52.1
 fqdn==1.5.1
 gast==0.5.4
 gitdb==4.0.11
 gitpython==3.1.43
 google-pasta==0.2.0
 graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.2
+grpcio==1.64.0
 h11==0.14.0
 h5py==3.11.0
 hepunits==2.3.3
 httpcore==1.0.5
 httpx==0.27.0
 identify==2.5.36
 idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
 importlib-metadata==7.1.0
-importlib-resources==6.4.0
 iniconfig==2.0.0
 ipykernel==6.29.4
 ipympl==0.9.4
-ipython==8.18.1
+ipython==8.24.0
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
-jax==0.4.26
-jaxlib==0.4.26
+jax==0.4.28
+jaxlib==0.4.28
 jedi==0.19.1
-jinja2==3.1.3
+jinja2==3.1.4
 json5==0.9.25
 jsonpointer==2.4
-jsonschema==4.21.1
+jsonschema==4.22.0
 jsonschema-specifications==2023.12.1
 jupyter-cache==1.0.0
-jupyter-client==8.6.1
+jupyter-client==8.6.2
 jupyter-core==5.7.2
 jupyter-events==0.10.0
 jupyter-lsp==2.2.5
 jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.6
+jupyterlab==4.2.1
 jupyterlab-code-formatter==2.2.1
-jupyterlab-git==0.50.0
+jupyterlab-git==0.50.1
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.2
+jupyterlab-myst==2.4.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.27.1
+jupyterlab-server==2.27.2
 jupyterlab-widgets==3.0.10
-keras==3.3.2
+keras==3.3.3
 kiwisolver==1.4.5
 latexcodec==3.0.0
 libclang==18.1.1
+livereload==2.6.3
 llvmlite==0.42.0
 lsprotocol==2023.0.1
 markdown==3.6
 markdown-it-py==3.0.0
 markupsafe==2.1.5
-matplotlib==3.8.4
+matplotlib==3.9.0
 matplotlib-inline==0.1.7
-mdit-py-plugins==0.4.0
+mdit-py-plugins==0.4.1
 mdurl==0.1.2
 mistune==3.0.2
 ml-dtypes==0.3.2
 mpmath==1.3.0
+mypy==1.10.0
 mypy-extensions==1.0.0
 myst-nb==1.1.0
-myst-parser==3.0.0
+myst-parser==3.0.1
 namex==0.0.8
 nbclient==0.6.8
-nbconvert==7.16.3
+nbconvert==7.16.4
 nbdime==4.0.1
 nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
 numba==0.59.1
@@ -132,107 +133,103 @@
 pandocfilters==1.5.1
 parso==0.8.4
 particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
 phasespace==1.10.3
 pillow==10.3.0
-platformdirs==4.2.1
+platformdirs==4.2.2
 pluggy==1.5.0
-pre-commit==3.7.0
+pre-commit==3.7.1
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
 protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pybtex==0.24.0
 pybtex-docutils==1.0.3
 pycparser==2.22
 pydata-sphinx-theme==0.15.2
-pygments==2.17.2
+pygments==2.18.0
 pyparsing==3.1.2
 pyproject-api==1.6.1
-pytest==8.1.1
+pytest==8.2.1
 pytest-cov==5.0.0
-pytest-xdist==3.5.0
-python-constraint==1.4.0
+pytest-xdist==3.6.1
+python-constraint2==2.0.0b5
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
-python-lsp-ruff==2.2.0
+python-lsp-ruff==2.2.1
 python-lsp-server==1.11.0
 pytoolconfig==1.3.1
 pyyaml==6.0.1
-pyzmq==26.0.2
-qrules==0.10.1
-referencing==0.35.0
-requests==2.31.0
+pyzmq==26.0.3
+qrules==0.10.2
+referencing==0.35.1
+requests==2.32.2
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rich==13.7.1
 rope==1.13.0
-rpds-py==0.18.0
-ruff==0.4.1
-scipy==1.13.0
+rpds-py==0.18.1
+ruff==0.4.5
+scipy==1.13.1
 send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
 sphinx==7.3.7
 sphinx-api-relink==0.0.9
-sphinx-autobuild==2024.4.16
+sphinx-autobuild==2024.2.4
 sphinx-book-theme==1.1.2
 sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
-sphinx-design==0.5.0
+sphinx-design==0.6.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.8
 sphinxcontrib-bibtex==2.6.2
 sphinxcontrib-devhelp==1.0.6
 sphinxcontrib-htmlhelp==2.0.5
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.7
 sphinxcontrib-serializinghtml==1.1.10
-sqlalchemy==2.0.29
+sqlalchemy==2.0.30
 stack-data==0.6.3
-starlette==0.37.2
 sympy==1.12
 tabulate==0.9.0
 tensorboard==2.16.2
 tensorboard-data-server==0.7.2
 tensorflow==2.16.1
-tensorflow-io-gcs-filesystem==0.36.0
+tensorflow-io-gcs-filesystem==0.37.0
 tensorflow-probability==0.24.0
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
 tinycss2==1.3.0
 tomli==2.0.1
 tornado==6.4
-tox==4.14.2
-tqdm==4.66.2
+tox==4.15.0
+tqdm==4.66.4
 traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.11.0
-ujson==5.9.0
+typing-extensions==4.12.0
+ujson==5.10.0
 uri-template==1.3.0
 urllib3==2.2.1
-uvicorn==0.29.0
-virtualenv==20.26.0
-watchfiles==0.21.0
+virtualenv==20.26.2
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
 websocket-client==1.8.0
-websockets==12.0
-werkzeug==3.0.2
+werkzeug==3.0.3
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
-zipp==3.18.1
+zipp==3.18.2
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform_dpd-0.2.0/.cspell.json` & `ampform_dpd-0.2.1rc0/.cspell.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9840150345852627%*

 * *Differences: {"'ignorePaths'": "{insert: [(10, '.readthedocs.yml')]}",*

 * * "'ignoreWords'": "{insert: [(6, 'asdict'), (20, 'costheta'), (21, 'difflib'), (29, 'formfactor'), "*

 * *                  "(30, 'funcs'), (33, 'imag'), (58, 'noqa'), (78, 'setattr')]}",*

 * * "'words'": "{insert: [(15, 'JHEP'), (30, 'recoupling'), (31, 'recouplings')]}"}*

```diff
@@ -25,50 +25,57 @@
         "*particle*.*ml",
         ".constraints/*.txt",
         ".editorconfig",
         ".gitignore",
         ".gitpod.*",
         ".pre-commit-config.yaml",
         ".prettierignore",
+        ".readthedocs.yml",
         ".vscode/*",
         ".vscode/.gitignore",
         "codecov.yml",
         "docs/conf.py",
         "pyproject.toml",
         "tox.ini"
     ],
     "ignoreWords": [
         "Jpsi",
         "Kallen",
         "MAINT",
         "PyPI",
         "absl",
         "arange",
+        "asdict",
         "asdot",
         "aslatex",
         "autoscale",
         "autoupdate",
         "axvline",
         "bdist",
         "caplog",
         "cloudpickle",
         "codecov",
         "codemirror",
         "colorbar",
         "commitlint",
         "concat",
+        "costheta",
+        "difflib",
         "docnb",
         "elif",
         "endswith",
         "eqnarray",
         "eqref",
         "figsize",
         "fontsize",
+        "formfactor",
+        "funcs",
         "gcov",
         "graphviz",
+        "imag",
         "ipykernel",
         "ipynb",
         "ipython",
         "ipywidgets",
         "isinstance",
         "isnan",
         "itertools",
@@ -85,14 +92,15 @@
         "mystnb",
         "nanmax",
         "nansum",
         "nbconvert",
         "nbformat",
         "ncols",
         "ndarray",
+        "noqa",
         "noreply",
         "nrows",
         "pandoc",
         "pbar",
         "pcolormesh",
         "phasespace",
         "phipipi",
@@ -104,14 +112,15 @@
         "pycache",
         "pygments",
         "redeboer",
         "repr",
         "savefig",
         "sdist",
         "seealso",
+        "setattr",
         "setuptools",
         "sharey",
         "simplefilter",
         "startswith",
         "suptitle",
         "textwrap",
         "toctree",
@@ -142,27 +151,30 @@
         "Dalitz",
         "doctests",
         "Flatt\u00e9",
         "Gordan",
         "helicities",
         "helicity",
         "isospin",
+        "JHEP",
         "JPAC",
         "lambdify",
         "lambdifying",
         "LHCb",
         "lineshape",
         "lineshapes",
         "matplotlib",
         "NumPy",
         "PyPA",
         "pyplot",
         "pyright",
         "pytest",
         "PYTHONHASHSEED",
         "QRules",
+        "recoupling",
+        "recouplings",
         "sympify",
         "SymPy",
         "TensorWaves",
         "Weisskopf"
     ]
 }
```

### Comparing `ampform_dpd-0.2.0/.github/release-drafter.yml` & `ampform_dpd-0.2.1rc0/.github/release-drafter.yml`

 * *Files 19% similar despite different names*

```diff
@@ -28,10 +28,12 @@
 replacers:
   - search: /([A-Z]+!?:\s*)(.*)/g
     replace: $2
 
 sort-direction: ascending
 
 template: |
+  _See all documentation for this version [here](https://ampform-dpd.rtfd.io/en/$NEXT_PATCH_VERSION)._
+
   $CHANGES
 
   _The full changelog as commits can be found [here](https://github.com/ComPWA/ampform-dpd/compare/$PREVIOUS_TAG...$NEXT_PATCH_VERSION)._
```

### Comparing `ampform_dpd-0.2.0/.github/workflows/cd.yml` & `ampform_dpd-0.2.1rc0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/.github/workflows/ci.yml` & `ampform_dpd-0.2.1rc0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/.github/workflows/requirements.yml` & `ampform_dpd-0.2.1rc0/.github/workflows/requirements.yml`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/.gitpod.yml` & `ampform_dpd-0.2.1rc0/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/.pre-commit-config.yaml` & `ampform_dpd-0.2.1rc0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     rev: 0.7.1
     hooks:
       - id: nbstripout
         args:
           - --extra-keys
           - |
             cell.attachments
+            cell.id
             cell.metadata.code_folding
             cell.metadata.editable
             cell.metadata.id
             cell.metadata.pycharm
             cell.metadata.slideshow
             cell.metadata.user_expressions
             metadata.celltoolbar
@@ -37,27 +38,28 @@
             metadata.toc-showcode
             metadata.toc-showmarkdowntxt
             metadata.toc-showtags
             metadata.varInspector
             metadata.vscode
 
   - repo: https://github.com/ComPWA/policy
-    rev: 0.3.6
+    rev: 0.3.9
     hooks:
       - id: check-dev-files
         args:
           - --doc-apt-packages=graphviz
+          - --github-pages
           - --no-prettierrc
           - --pin-requirements=bimonthly
           - --repo-name=ampform-dpd
           - --repo-title=AmpForm-DPD
       - id: colab-toc-visible
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.1
+    rev: v0.4.5
     hooks:
       - id: ruff
         args: [--fix]
         types_or: [python, pyi, jupyter]
       - id: ruff-format
         types_or: [python, pyi, jupyter]
 
@@ -90,15 +92,15 @@
     rev: v0.23.1
     hooks:
       - id: toml-sort
         args:
           - --in-place
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v8.7.0
+    rev: v8.8.2
     hooks:
       - id: cspell
 
   - repo: https://github.com/editorconfig-checker/editorconfig-checker.python
     rev: 2.7.3
     hooks:
       - id: editorconfig-checker
@@ -116,10 +118,10 @@
         entry: mypy
         language: system
         require_serial: true
         types:
           - python
 
   - repo: https://github.com/ComPWA/mirrors-pyright
-    rev: v1.1.359
+    rev: v1.1.364
     hooks:
       - id: pyright
```

### Comparing `ampform_dpd-0.2.0/.vscode/extensions.json` & `ampform_dpd-0.2.1rc0/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/.vscode/settings.json` & `ampform_dpd-0.2.1rc0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/LICENSE` & `ampform_dpd-0.2.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/PKG-INFO` & `ampform_dpd-0.2.1rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampform-dpd
-Version: 0.2.0
+Version: 0.2.1rc0
 Summary: Symbolic expressions for Dalitz-Plot Decomposition
 Author-email: Common Partial Wave Analysis <compwa-admin@ep1.rub.de>
 License: GPLv3 or later
 Project-URL: Changelog, https://github.com/ComPWA/ampform-dpd/releases
 Project-URL: Documentation, https://compwa.github.io/ampform-dpd
 Project-URL: Source, https://github.com/ComPWA/ampform-dpd
 Project-URL: Tracker, https://github.com/ComPWA/ampform-dpd/issues
@@ -23,33 +23,36 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ampform>=0.14.8
+Requires-Dist: ampform>=0.15.1
 Requires-Dist: attrs>=20.1.0
 Requires-Dist: cloudpickle
 Requires-Dist: qrules>=0.10.0
 Requires-Dist: sympy>=1.10
 Requires-Dist: tensorwaves[jax]
+Requires-Dist: typing-extensions; python_version < "3.11.0"
 Provides-Extra: dev
 Requires-Dist: ampform-dpd[doc]; extra == "dev"
 Requires-Dist: ampform-dpd[jupyter]; extra == "dev"
 Requires-Dist: ampform-dpd[sty]; extra == "dev"
 Requires-Dist: ampform-dpd[test]; extra == "dev"
+Requires-Dist: sphinx-autobuild!=2024.04.*; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: tox>=1.9; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: graphviz; extra == "doc"
 Requires-Dist: ipympl; extra == "doc"
 Requires-Dist: ipywidgets; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: myst-nb>=0.14; extra == "doc"
+Requires-Dist: pandas; extra == "doc"
 Requires-Dist: sphinx-api-relink>=0.0.4; extra == "doc"
 Requires-Dist: sphinx-book-theme; extra == "doc"
 Requires-Dist: sphinx-codeautolink[ipython]; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
 Requires-Dist: sphinx-design; extra == "doc"
 Requires-Dist: sphinx-pybtex-etal-style; extra == "doc"
 Requires-Dist: sphinx-togglebutton; extra == "doc"
@@ -106,10 +109,10 @@
 [![Test coverage](https://codecov.io/gh/ComPWA/ampform-dpd/branch/main/graph/badge.svg)](https://codecov.io/gh/ComPWA/ampform-dpd)
 
 [![GitPod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ComPWA/ampform-dpd)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
 [![Spelling checked](https://img.shields.io/badge/cspell-checked-brightgreen.svg)](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-This repository is a (temporary) extension of [AmpForm](https://ampform.rtfd.io) and provides a symbolic implementation of Dalitz-plot decomposition ([10.1103/PhysRevD.101.034033](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.101.034033)) with [SymPy](https://www.sympy.org/en/index.html). It has been extracted from the [ComPWA/polarimetry](https://github.com/ComPWA/polarimetry) repository, which is not yet public.
+This repository is a (temporary) extension of [AmpForm](https://ampform.rtfd.io) and provides a symbolic implementation of Dalitz-plot decomposition ([10.1103/PhysRevD.101.034033](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.101.034033)) with [SymPy](https://www.sympy.org/en/index.html). It has been extracted from the [ComPWA/polarimetry](https://github.com/ComPWA/polarimetry) repository ([10.1007/JHEP07(2023)228](<https://doi.org/10.1007/JHEP07(2023)228>)).
 
 Installation instructions can be found [here](https://compwa.github.io/ampform-dpd/#installation).
```

### Comparing `ampform_dpd-0.2.0/README.md` & `ampform_dpd-0.2.1rc0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 [![Test coverage](https://codecov.io/gh/ComPWA/ampform-dpd/branch/main/graph/badge.svg)](https://codecov.io/gh/ComPWA/ampform-dpd)
 
 [![GitPod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ComPWA/ampform-dpd)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
 [![Spelling checked](https://img.shields.io/badge/cspell-checked-brightgreen.svg)](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-This repository is a (temporary) extension of [AmpForm](https://ampform.rtfd.io) and provides a symbolic implementation of Dalitz-plot decomposition ([10.1103/PhysRevD.101.034033](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.101.034033)) with [SymPy](https://www.sympy.org/en/index.html). It has been extracted from the [ComPWA/polarimetry](https://github.com/ComPWA/polarimetry) repository, which is not yet public.
+This repository is a (temporary) extension of [AmpForm](https://ampform.rtfd.io) and provides a symbolic implementation of Dalitz-plot decomposition ([10.1103/PhysRevD.101.034033](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.101.034033)) with [SymPy](https://www.sympy.org/en/index.html). It has been extracted from the [ComPWA/polarimetry](https://github.com/ComPWA/polarimetry) repository ([10.1007/JHEP07(2023)228](<https://doi.org/10.1007/JHEP07(2023)228>)).
 
 Installation instructions can be found [here](https://compwa.github.io/ampform-dpd/#installation).
```

### Comparing `ampform_dpd-0.2.0/codecov.yml` & `ampform_dpd-0.2.1rc0/codecov.yml`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/docs/_static/favicon.ico` & `ampform_dpd-0.2.1rc0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/docs/comparison/d2kkk.ipynb` & `ampform_dpd-0.2.1rc0/docs/comparison/d2kkk.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999853886616015%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(53, \'warnings.simplefilter("ignore", '*

 * *            "category=RuntimeWarning)\\n')], delete: [53]}}}"}*

```diff
@@ -80,15 +80,15 @@
                 "    from ampform.helicity import HelicityModel\n",
                 "    from qrules.transition import ReactionInfo\n",
                 "    from tensorwaves.interface import DataSample, ParameterValue, ParametrizedFunction\n",
                 "\n",
                 "simplify_latex_rendering()\n",
                 "logging.getLogger(\"jax\").setLevel(logging.ERROR)  # mute JAX\n",
                 "os.environ[\"TF_CPP_MIN_LOG_LEVEL\"] = \"3\"  # mute TF\n",
-                "warnings.simplefilter(\"ignore\")\n",
+                "warnings.simplefilter(\"ignore\", category=RuntimeWarning)\n",
                 "NO_TQDM = \"EXECUTE_NB\" in os.environ\n",
                 "if NO_TQDM:\n",
                 "    logging.getLogger(\"ampform.sympy\").setLevel(logging.ERROR)\n",
                 "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)"
             ]
         },
         {
```

### Comparing `ampform_dpd-0.2.0/docs/comparison/jpsi2phipipi.ipynb` & `ampform_dpd-0.2.1rc0/docs/comparison/jpsi2phipipi.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999843063402385%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(53, \'warnings.simplefilter("ignore", '*

 * *            "category=RuntimeWarning)\\n')], delete: [53]}}}"}*

```diff
@@ -80,15 +80,15 @@
                 "    from ampform.helicity import HelicityModel\n",
                 "    from qrules.transition import ReactionInfo\n",
                 "    from tensorwaves.interface import DataSample, ParameterValue, ParametrizedFunction\n",
                 "\n",
                 "simplify_latex_rendering()\n",
                 "logging.getLogger(\"jax\").setLevel(logging.ERROR)  # mute JAX\n",
                 "os.environ[\"TF_CPP_MIN_LOG_LEVEL\"] = \"3\"  # mute TF\n",
-                "warnings.simplefilter(\"ignore\")\n",
+                "warnings.simplefilter(\"ignore\", category=RuntimeWarning)\n",
                 "NO_TQDM = \"EXECUTE_NB\" in os.environ\n",
                 "if NO_TQDM:\n",
                 "    logging.getLogger(\"ampform.sympy\").setLevel(logging.ERROR)\n",
                 "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)"
             ]
         },
         {
```

### Comparing `ampform_dpd-0.2.0/docs/comparison/jpsi2pipipi.ipynb` & `ampform_dpd-0.2.1rc0/docs/comparison/jpsi2pipipi.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999843063402385%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(53, \'warnings.simplefilter("ignore", '*

 * *            "category=RuntimeWarning)\\n')], delete: [53]}}}"}*

```diff
@@ -80,15 +80,15 @@
                 "    from ampform.helicity import HelicityModel\n",
                 "    from qrules.transition import ReactionInfo\n",
                 "    from tensorwaves.interface import DataSample, ParameterValue, ParametrizedFunction\n",
                 "\n",
                 "simplify_latex_rendering()\n",
                 "logging.getLogger(\"jax\").setLevel(logging.ERROR)  # mute JAX\n",
                 "os.environ[\"TF_CPP_MIN_LOG_LEVEL\"] = \"3\"  # mute TF\n",
-                "warnings.simplefilter(\"ignore\")\n",
+                "warnings.simplefilter(\"ignore\", category=RuntimeWarning)\n",
                 "NO_TQDM = \"EXECUTE_NB\" in os.environ\n",
                 "if NO_TQDM:\n",
                 "    logging.getLogger(\"ampform.sympy\").setLevel(logging.ERROR)\n",
                 "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)"
             ]
         },
         {
```

### Comparing `ampform_dpd-0.2.0/docs/conf.py` & `ampform_dpd-0.2.1rc0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,34 +33,38 @@
 EXECUTE_NB = get_execution_mode() != "off"
 
 
 add_module_names = False
 api_github_repo = f"{ORGANIZATION}/{REPO_NAME}"
 api_target_substitutions: dict[str, str | tuple[str, str]] = {
     "ampform_dpd.decay.StateIDTemplate": ("obj", "ampform_dpd.decay.StateID"),
+    "ampform_dpd.io.serialization.dynamics.T": "typing.TypeVar",
     "DecayNode": ("obj", "ampform_dpd.decay.DecayNode"),
     "FinalState": ("obj", "ampform_dpd.decay.FinalState"),
     "FinalStateID": ("obj", "ampform_dpd.decay.FinalStateID"),
     "FrozenTransition": "qrules.topology.FrozenTransition",
     "InitialStateID": ("obj", "ampform_dpd.decay.InitialStateID"),
     "Literal[-1, 1]": "typing.Literal",
     "Literal[(-1, 1)]": "typing.Literal",
+    "Node": ("obj", "ampform_dpd.io.serialization.format.Node"),
     "ParameterValue": ("obj", "tensorwaves.interface.ParameterValue"),
     "ParametrizedBackendFunction": "tensorwaves.function.ParametrizedBackendFunction",
     "PoolSum": "ampform.sympy.PoolSum",
     "PositionalArgumentFunction": "tensorwaves.function.PositionalArgumentFunction",
     "qrules.topology.EdgeType": "typing.TypeVar",
     "qrules.topology.NodeType": "typing.TypeVar",
     "sp.acos": "sympy.functions.elementary.trigonometric.acos",
     "sp.Expr": "sympy.core.expr.Expr",
     "sp.Indexed": "sympy.tensor.indexed.Indexed",
     "sp.Rational": "sympy.core.numbers.Rational",
     "sp.Symbol": "sympy.core.symbol.Symbol",
     "StateID": ("obj", "ampform_dpd.decay.StateID"),
     "StateIDTemplate": ("obj", "ampform_dpd.decay.StateID"),
+    "Topology": ("obj", "ampform_dpd.io.serialization.format.Topology"),
+    "typing_extensions.Required": ("obj", "typing.Required"),
 }
 api_target_types: dict[str, str] = {}
 author = "Common Partial Wave Analysis"
 autodoc_default_options = {
     "exclude-members": ", ".join([
         "default_assumptions",
         "doit",
```

### Comparing `ampform_dpd-0.2.0/docs/index.md` & `ampform_dpd-0.2.1rc0/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
 ```{toctree}
 ---
 maxdepth: 1
 ---
 lc2pkpi
 jpsi2ksp
 xib2pkk
+serialization
 ```
 
 ```{toctree}
 ---
 maxdepth: 2
 ---
 comparison
```

### Comparing `ampform_dpd-0.2.0/docs/jpsi2ksp.ipynb` & `ampform_dpd-0.2.1rc0/docs/jpsi2ksp.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999295267489712%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(32, \'warnings.simplefilter("ignore", '*

 * *            "category=RuntimeWarning)\\n')], delete: [32]}}, 10: {'source': {insert: [(5, 'model = "*

 * *            "model_builder.formulate(reference_subsystem=2)\\n')], delete: [5]}}, 13: {'source': "*

 * *            "['Latex(aslatex(model.amplitudes))']}, 14: {'source': {insert: [(0, 's, m0, w0, m1, "*

 * *            'm2, L, R, z = sp.symbols("s m0 Gamma0 m1 m2 L R z", nonnegative=True)\\n\')], delete: '*

 * *            '[0]}}}'}*

```diff
@@ -54,15 +54,15 @@
                 "    aslatex,\n",
                 "    perform_cached_lambdify,\n",
                 "    simplify_latex_rendering,\n",
                 ")\n",
                 "\n",
                 "simplify_latex_rendering()\n",
                 "logging.getLogger(\"absl\").setLevel(logging.ERROR)  # mute JAX\n",
-                "warnings.simplefilter(\"ignore\")\n",
+                "warnings.simplefilter(\"ignore\", category=RuntimeWarning)\n",
                 "\n",
                 "NO_TQDM = \"EXECUTE_NB\" in os.environ\n",
                 "if NO_TQDM:\n",
                 "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)\n",
                 "if TYPE_CHECKING:\n",
                 "    from tensorwaves.interface import DataSample, ParametrizedFunction"
             ]
@@ -187,15 +187,15 @@
             "outputs": [],
             "source": [
                 "model_builder = DalitzPlotDecompositionBuilder(DECAY, min_ls=False)\n",
                 "for chain in model_builder.decay.chains:\n",
                 "    model_builder.dynamics_choices.register_builder(\n",
                 "        chain, formulate_breit_wigner_with_form_factor\n",
                 "    )\n",
-                "model = model_builder.formulate(reference_subsystem=1)\n",
+                "model = model_builder.formulate(reference_subsystem=2)\n",
                 "model.intensity"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -226,15 +226,15 @@
                     "hide-input",
                     "full-width",
                     "hide-output"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex({k: v for k, v in model.amplitudes.items() if v}))"
+                "Latex(aslatex(model.amplitudes))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -243,15 +243,15 @@
                 "tags": [
                     "hide-input",
                     "full-width"
                 ]
             },
             "outputs": [],
             "source": [
-                "s, m0, w0, m1, m2, L, R, z = sp.symbols(\"s m0 Gamma0 m1 m2 L R z\")\n",
+                "s, m0, w0, m1, m2, L, R, z = sp.symbols(\"s m0 Gamma0 m1 m2 L R z\", nonnegative=True)\n",
                 "exprs = [\n",
                 "    RelativisticBreitWigner(s, m0, w0, m1, m2, L, R),\n",
                 "    EnergyDependentWidth(s, m0, w0, m1, m2, L, R),\n",
                 "    FormFactor(s, m1, m2, L, R),\n",
                 "    BlattWeisskopfSquared(z, L),\n",
                 "]\n",
                 "Latex(aslatex({e: e.doit(deep=False) for e in exprs}))"
```

### Comparing `ampform_dpd-0.2.0/docs/lc2pkpi.ipynb` & `ampform_dpd-0.2.1rc0/docs/lc2pkpi.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990583691670648%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(18, 'simplify_latex_rendering()')], delete: [21, 20, 2, "*

 * *            '1]}}, 8: {\'source\': {insert: [(1, \'m_top, m_spec = sp.symbols(R"m_\\\\mathrm{top} '*

 * *            'm_\\\\mathrm{spectator}", nonnegative=True)\\n\'), (2, \'R_dec, R_prod = '*

 * *            'sp.symbols(R"R_\\\\mathrm{res} R_{\\\\Lambda_c}", nonnegative=True)\\n\'), (3, '*

 * *            '\'l_Λc, l_R = sp.symbols(R"l_{\\\\Lambda_c} l_R", integer=True, '*

 * *            "nonnegative=True)\\n')], delete: [3, 2, 1 […]*

```diff
@@ -22,16 +22,14 @@
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "from __future__ import annotations\n",
                 "\n",
-                "import warnings\n",
-                "\n",
                 "import graphviz\n",
                 "import qrules\n",
                 "import sympy as sp\n",
                 "from IPython.display import Latex, Markdown\n",
                 "\n",
                 "from ampform_dpd import DalitzPlotDecompositionBuilder\n",
                 "from ampform_dpd.adapter.qrules import (\n",
@@ -40,16 +38,15 @@
                 "    to_three_body_decay,\n",
                 ")\n",
                 "from ampform_dpd.decay import ThreeBodyDecayChain\n",
                 "from ampform_dpd.dynamics import BreitWignerMinL\n",
                 "from ampform_dpd.dynamics.builder import create_mass_symbol, get_mandelstam_s\n",
                 "from ampform_dpd.io import as_markdown_table, aslatex, simplify_latex_rendering\n",
                 "\n",
-                "simplify_latex_rendering()\n",
-                "warnings.simplefilter(\"ignore\")"
+                "simplify_latex_rendering()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Decay definition"
@@ -168,17 +165,17 @@
                     "scroll-input",
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "s, m0, \u03930, m1, m2 = sp.symbols(\"s m0 Gamma0 m1 m2\", nonnegative=True)\n",
-                "m_top, m_spec = sp.symbols(R\"m_\\mathrm{top} m_\\mathrm{spectator}\")\n",
-                "R_dec, R_prod = sp.symbols(R\"R_\\mathrm{res} R_{\\Lambda_c}\")\n",
-                "l_\u039bc, l_R = sp.symbols(R\"l_{\\Lambda_c} l_R\", integer=True, positive=True)\n",
+                "m_top, m_spec = sp.symbols(R\"m_\\mathrm{top} m_\\mathrm{spectator}\", nonnegative=True)\n",
+                "R_dec, R_prod = sp.symbols(R\"R_\\mathrm{res} R_{\\Lambda_c}\", nonnegative=True)\n",
+                "l_\u039bc, l_R = sp.symbols(R\"l_{\\Lambda_c} l_R\", integer=True, nonnegative=True)\n",
                 "bw = BreitWignerMinL(s, m_top, m_spec, m0, \u03930, m1, m2, l_R, l_\u039bc, R_dec, R_prod)\n",
                 "Latex(aslatex({bw: bw.doit(deep=False)}))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -204,16 +201,16 @@
                 "    l_prod = sp.Rational(decay_chain.incoming_ls.L)\n",
                 "    parent_mass = sp.Symbol(f\"m_{{{decay_chain.parent.latex}}}\", nonnegative=True)\n",
                 "    spectator_mass = sp.Symbol(f\"m_{{{decay_chain.spectator.latex}}}\", nonnegative=True)\n",
                 "    resonance_mass = sp.Symbol(f\"m_{{{decay_chain.resonance.latex}}}\", nonnegative=True)\n",
                 "    resonance_width = sp.Symbol(\n",
                 "        Rf\"\\Gamma_{{{decay_chain.resonance.latex}}}\", nonnegative=True\n",
                 "    )\n",
-                "    R_dec = sp.Symbol(R\"R_\\mathrm{res}\")\n",
-                "    R_prod = sp.Symbol(R\"R_{\\Lambda_c}\")\n",
+                "    R_dec = sp.Symbol(R\"R_\\mathrm{res}\", nonnegative=True)\n",
+                "    R_prod = sp.Symbol(R\"R_{\\Lambda_c}\", nonnegative=True)\n",
                 "    parameter_defaults = {\n",
                 "        parent_mass: decay_chain.parent.mass,\n",
                 "        spectator_mass: decay_chain.spectator.mass,\n",
                 "        resonance_mass: decay_chain.resonance.mass,\n",
                 "        resonance_width: decay_chain.resonance.width,\n",
                 "        child1_mass: decay_chain.decay_products[0].mass,\n",
                 "        child2_mass: decay_chain.decay_products[1].mass,\n",
```

### Comparing `ampform_dpd-0.2.0/docs/references.bib` & `ampform_dpd-0.2.1rc0/docs/references.bib`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/docs/xib2pkk.ipynb` & `ampform_dpd-0.2.1rc0/docs/xib2pkk.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993910256410257%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(37, \'warnings.simplefilter("ignore", '*

 * *            "category=RuntimeWarning)\\n')], delete: [37]}}, 12: {'source': "*

 * *            "['Latex(aslatex(model.amplitudes))']}, 13: {'source': {insert: [(0, 's, m0, w0, m1, "*

 * *            'm2, L, R, z = sp.symbols("s m0 Gamma0 m1 m2 L R z", nonnegative=True)\\n\')], delete: '*

 * *            '[0]}}}'}*

```diff
@@ -59,15 +59,15 @@
                 "    aslatex,\n",
                 "    perform_cached_lambdify,\n",
                 "    simplify_latex_rendering,\n",
                 ")\n",
                 "\n",
                 "simplify_latex_rendering()\n",
                 "logging.getLogger(\"absl\").setLevel(logging.ERROR)  # mute JAX\n",
-                "warnings.simplefilter(\"ignore\")\n",
+                "warnings.simplefilter(\"ignore\", category=RuntimeWarning)\n",
                 "\n",
                 "NO_TQDM = \"EXECUTE_NB\" in os.environ\n",
                 "if NO_TQDM:\n",
                 "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)\n",
                 "if TYPE_CHECKING:\n",
                 "    from tensorwaves.interface import DataSample, ParametrizedFunction"
             ]
@@ -252,15 +252,15 @@
                     "hide-input",
                     "full-width",
                     "hide-output"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex({k: v for k, v in model.amplitudes.items() if v}))"
+                "Latex(aslatex(model.amplitudes))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -269,15 +269,15 @@
                 "tags": [
                     "hide-input",
                     "full-width"
                 ]
             },
             "outputs": [],
             "source": [
-                "s, m0, w0, m1, m2, L, R, z = sp.symbols(\"s m0 Gamma0 m1 m2 L R z\")\n",
+                "s, m0, w0, m1, m2, L, R, z = sp.symbols(\"s m0 Gamma0 m1 m2 L R z\", nonnegative=True)\n",
                 "exprs = [\n",
                 "    RelativisticBreitWigner(s, m0, w0, m1, m2, L, R),\n",
                 "    EnergyDependentWidth(s, m0, w0, m1, m2, L, R),\n",
                 "    FormFactor(s, m1, m2, L, R),\n",
                 "    BlattWeisskopfSquared(z, L),\n",
                 "]\n",
                 "Latex(aslatex({e: e.doit(deep=False) for e in exprs}))"
```

### Comparing `ampform_dpd-0.2.0/pyproject.toml` & `ampform_dpd-0.2.1rc0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,42 +22,45 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering",
     "Typing :: Typed",
 ]
 dependencies = [
-    "ampform >=0.14.8", # Kibble and Kallen functions, perform_cached_doit, @unevaluated
+    "ampform >=0.15.1", # aslatex with keyword arguments
     "attrs >=20.1.0", # on_setattr and https://www.attrs.org/en/stable/api.html#next-gen
     "cloudpickle",
     "qrules >=0.10.0",
     "sympy >=1.10", # module sympy.printing.numpy and array expressions with shape kwarg
     "tensorwaves[jax]",
+    'typing-extensions; python_version <"3.11.0"',
 ]
 description = "Symbolic expressions for Dalitz-Plot Decomposition"
 dynamic = ["version"]
 license = {text = "GPLv3 or later"}
 name = "ampform-dpd"
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = [
     "ampform-dpd[doc]",
     "ampform-dpd[jupyter]",
     "ampform-dpd[sty]",
     "ampform-dpd[test]",
+    "sphinx-autobuild!=2024.04.*",
     "sphinx-autobuild",
     "tox >=1.9", # for skip_install, use_develop
 ]
 doc = [
     "graphviz",
     "ipympl",
     "ipywidgets",
     "matplotlib",
     "myst-nb >=0.14", # nb_render_markdown_format for Markdown tables
+    "pandas",
     "sphinx-api-relink >=0.0.4",
     "sphinx-book-theme",
     "sphinx-codeautolink[ipython]",
     "sphinx-copybutton",
     "sphinx-design",
     "sphinx-pybtex-etal-style",
     "sphinx-togglebutton",
@@ -182,14 +185,17 @@
     "--color=yes",
     "--doctest-continue-on-failure",
     "--doctest-modules",
     "--durations=3",
     "--ignore=docs/conf.py",
     "-m not slow",
 ]
+doctest_optionflags = [
+    "IGNORE_EXCEPTION_DETAIL",
+]
 filterwarnings = [
     "error",
     "ignore:the imp module is deprecated in favour of importlib.*:DeprecationWarning",
 ]
 markers = [
     "slow: marks tests as slow (select with '-m slow')",
 ]
@@ -314,16 +320,25 @@
     "PLR2004",
     "S101",
     "S113",
     "T201",
 ]
 "docs/conf.py" = ["D100"]
 "jpsi2ksp.ipynb" = ["PLC2701"]
+"serialization.ipynb" = [
+    "E741",
+    "N813",
+    "PLC2403",
+    "PLC2701",
+    "RUF100",
+]
 "setup.py" = ["D100"]
-"src/ampform_dpd/io.py" = ["S403"]
+"src/ampform_dpd/io/__init__.py" = ["S403"]
+"src/ampform_dpd/io/serialization/amplitude.py" = ["E741"]
+"src/ampform_dpd/io/serialization/format.py" = ["E741"]
 "tests/*" = [
     "D",
     "INP001",
     "PGH001",
     "PLC2701",
     "PLR0913",
     "PLR2004",
@@ -331,14 +346,17 @@
     "S101",
     "T20",
 ]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
+[tool.ruff.lint.pylint]
+allow-dunder-method-names = ["_latex_repr_"]
+
 [tool.tomlsort]
 all = false
 ignore_case = true
 in_place = true
 sort_first = [
     "build-system",
     "project",
```

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/__init__.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 """Module for formulating the amplitude model for a three-body decay using DPD."""
 
 from __future__ import annotations
 
+from collections import abc
 from functools import lru_cache
 from itertools import product
-from typing import Literal, Protocol
+from typing import Any, Literal, Protocol
+from warnings import warn
 
 import sympy as sp
 from ampform.kinematics.phasespace import compute_third_mandelstam
 from ampform.sympy import PoolSum
-from attrs import field, frozen
+from attrs import define, field, frozen
 from sympy.core.symbol import Str
 from sympy.physics.quantum.spin import CG, WignerD
 from sympy.physics.quantum.spin import Rotation as Wigner
 
 from ampform_dpd.angles import formulate_scattering_angle, formulate_zeta_angle
 from ampform_dpd.decay import (
     FinalStateID,
     IsobarNode,
     LSCoupling,
     Particle,
     ThreeBodyDecay,
     ThreeBodyDecayChain,
+    _get_decay_description,  # pyright:ignore[reportPrivateUsage]
+    _get_subsystem_ids,  # pyright:ignore[reportPrivateUsage]
     get_decay_product_ids,
     to_particle,
 )
-from ampform_dpd.io import (
-    simplify_latex_rendering,  # noqa: F401  # pyright:ignore[reportUnusedImport]
-)
 from ampform_dpd.spin import create_spin_range
 
 
 @frozen
 class AmplitudeModel:
     decay: ThreeBodyDecay
     intensity: sp.Expr = sp.S.One
     amplitudes: dict[sp.Indexed, sp.Expr] = field(factory=dict)
     variables: dict[sp.Symbol, sp.Expr] = field(factory=dict)
     parameter_defaults: dict[sp.Symbol, float | complex] = field(factory=dict)
-    masses: dict[sp.Symbol, float | complex] = field(factory=dict)
+    masses: dict[sp.Symbol, float] = field(factory=dict)
     invariants: dict[sp.Symbol, sp.Expr] = field(factory=dict)
 
     @property
     def full_expression(self) -> sp.Expr:
         return self.intensity.doit().xreplace(self.amplitudes)
 
 
@@ -77,27 +78,28 @@
             raise NotImplementedError(msg, min_ls)
 
     def formulate(
         self,
         reference_subsystem: FinalStateID = 1,
         cleanup_summations: bool = False,
     ) -> AmplitudeModel:
+        _check_reference_subsystems(self.decay, reference_subsystem)
         helicity_symbols: tuple[sp.Symbol, sp.Symbol, sp.Symbol, sp.Symbol] = (
             sp.symbols("lambda:4", rational=True)
         )
         allowed_helicities = {
             symbol: create_spin_range(self.decay.states[i].spin)  # type:ignore[index]
             for i, symbol in enumerate(helicity_symbols)
         }
         amplitude_definitions = {}
         angle_definitions = {}
         parameter_defaults = {}
         args: tuple[sp.Rational, sp.Rational, sp.Rational, sp.Rational]
         for args in product(*allowed_helicities.values()):  # type:ignore[assignment]
-            for sub_system in (1, 2, 3):
+            for sub_system in _get_subsystem_ids(self.decay):
                 chain_model = self.formulate_subsystem_amplitude(*args, sub_system)  # type:ignore[arg-type]
                 amplitude_definitions.update(chain_model.amplitudes)
                 angle_definitions.update(chain_model.variables)
                 parameter_defaults.update(chain_model.parameter_defaults)
         aligned_amp, zeta_defs = self.formulate_aligned_amplitude(
             *helicity_symbols, reference_subsystem
         )
@@ -230,42 +232,50 @@
         self,
         λ0: sp.Rational | sp.Symbol,
         λ1: sp.Rational | sp.Symbol,
         λ2: sp.Rational | sp.Symbol,
         λ3: sp.Rational | sp.Symbol,
         reference_subsystem: FinalStateID = 1,
     ) -> tuple[PoolSum, dict[sp.Symbol, sp.Expr]]:
+        _check_reference_subsystems(self.decay, reference_subsystem)
         wigner_generator = _AlignmentWignerGenerator(reference_subsystem)
         _λ0, _λ1, _λ2, _λ3 = sp.symbols(R"\lambda_(0:4)^{\prime}", rational=True)
         j0, j1, j2, j3 = (self.decay.states[i].spin for i in sorted(self.decay.states))
         A = _generate_amplitude_index_bases()
         amp_expr = PoolSum(
-            A[1][_λ0, _λ1, _λ2, _λ3]
-            * wigner_generator(j0, λ0, _λ0, rotated_state=0, aligned_subsystem=1)
-            * wigner_generator(j1, _λ1, λ1, rotated_state=1, aligned_subsystem=1)
-            * wigner_generator(j2, _λ2, λ2, rotated_state=2, aligned_subsystem=1)
-            * wigner_generator(j3, _λ3, λ3, rotated_state=3, aligned_subsystem=1)
-            + A[2][_λ0, _λ1, _λ2, _λ3]
-            * wigner_generator(j0, λ0, _λ0, rotated_state=0, aligned_subsystem=2)
-            * wigner_generator(j1, _λ1, λ1, rotated_state=1, aligned_subsystem=2)
-            * wigner_generator(j2, _λ2, λ2, rotated_state=2, aligned_subsystem=2)
-            * wigner_generator(j3, _λ3, λ3, rotated_state=3, aligned_subsystem=2)
-            + A[3][_λ0, _λ1, _λ2, _λ3]
-            * wigner_generator(j0, λ0, _λ0, rotated_state=0, aligned_subsystem=3)
-            * wigner_generator(j1, _λ1, λ1, rotated_state=1, aligned_subsystem=3)
-            * wigner_generator(j2, _λ2, λ2, rotated_state=2, aligned_subsystem=3)
-            * wigner_generator(j3, _λ3, λ3, rotated_state=3, aligned_subsystem=3),
+            sum(
+                A[k][_λ0, _λ1, _λ2, _λ3]
+                * wigner_generator(j0, λ0, _λ0, rotated_state=0, aligned_subsystem=k)
+                * wigner_generator(j1, _λ1, λ1, rotated_state=1, aligned_subsystem=k)
+                * wigner_generator(j2, _λ2, λ2, rotated_state=2, aligned_subsystem=k)
+                * wigner_generator(j3, _λ3, λ3, rotated_state=3, aligned_subsystem=k)
+                for k in _get_subsystem_ids(self.decay)
+            ),
             (_λ0, create_spin_range(j0)),
             (_λ1, create_spin_range(j1)),
             (_λ2, create_spin_range(j2)),
             (_λ3, create_spin_range(j3)),
         )
         return amp_expr, wigner_generator.angle_definitions  # type:ignore[return-value]
 
 
+def _check_reference_subsystems(
+    decay: ThreeBodyDecay, reference_subsystem: FinalStateID
+) -> None:
+    subsystem_ids = _get_subsystem_ids(decay)
+    if reference_subsystem not in subsystem_ids:
+        decay_description = _get_decay_description(decay)
+        subsystems = ", ".join(sorted(str(i) for i in _get_subsystem_ids(decay)))
+        msg = (
+            f"Decay {decay_description} only has subsystems {subsystems}. Are you"
+            f" sure you want to use subsystem {reference_subsystem} as reference?"
+        )
+        warn(msg, category=UserWarning)
+
+
 def _create_coupling_symbol(
     helicity_coupling: bool,
     resonance: Str,
     helicities: tuple[sp.Basic, sp.Basic],
     interaction: LSCoupling | None,
     typ: Literal["production", "decay"],
 ) -> sp.Indexed:
@@ -380,23 +390,44 @@
 
 class DynamicsBuilder(Protocol):
     def __call__(
         self, decay_chain: ThreeBodyDecayChain
     ) -> tuple[sp.Expr, dict[sp.Symbol, float | complex]]: ...
 
 
+@define
+class DefinedExpression:
+    expression: sp.Expr = sp.S.One
+    definitions: dict[sp.Symbol, complex | float] = field(factory=dict)
+
+    def __mul__(self, other: Any) -> DefinedExpression:
+        if isinstance(other, DefinedExpression):
+            return DefinedExpression(
+                expression=self.expression * other.expression,
+                definitions={**self.definitions, **other.definitions},
+            )
+        if isinstance(other, abc.Sequence) and len(other) == 2:  # noqa: PLR2004
+            expression, definitions = other
+            return DefinedExpression(
+                expression=self.expression * expression,
+                definitions={**self.definitions, **definitions},
+            )
+        return DefinedExpression(
+            expression=self.expression * other,
+            definitions=self.definitions,
+        )
+
+
 def formulate_non_resonant(
     decay_chain: ThreeBodyDecayChain,
 ) -> tuple[sp.Expr, dict[sp.Symbol, float | complex]]:
     return sp.Rational(1), {}
 
 
-def create_mass_symbol_mapping(
-    decay: ThreeBodyDecay,
-) -> dict[sp.Symbol, float | complex]:
+def create_mass_symbol_mapping(decay: ThreeBodyDecay) -> dict[sp.Symbol, float]:
     return {
         sp.Symbol(f"m{i}", nonnegative=True): decay.states[i].mass
         for i in sorted(decay.states)  # ensure that dict keys are sorted by state ID
     }
 
 
 def formulate_invariants(decay: ThreeBodyDecay) -> dict[sp.Symbol, sp.Expr]:
```

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/_attrs.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/_attrs.py`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/_cache.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/_cache.py`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/adapter/qrules.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/adapter/qrules.py`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/angles.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/angles.py`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/decay.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/decay.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Data structures that describe a three-body decay."""
 
 from __future__ import annotations
 
 from functools import lru_cache
 from textwrap import dedent
 from typing import TYPE_CHECKING, Generic, Literal, TypeVar, overload
+from warnings import warn
 
 from attrs import field, frozen
 from attrs.validators import instance_of
 
 from ampform_dpd._attrs import assert_spin_value, to_chains, to_ls, to_rational
 
 if TYPE_CHECKING:
     import sympy as sp
 
-
 InitialStateID = Literal[0]
 """ID for the initial state particle in a three-body decay."""
 FinalStateID = Literal[1, 2, 3]
 """ID for a particle in the final state of a three-body decay."""
 StateID = Literal[0, 1, 2, 3]
 """ID for any of the initial state or final state particles in a three-body decay."""
 StateIDTemplate = TypeVar("StateIDTemplate", InitialStateID, FinalStateID, StateID)
@@ -26,15 +26,15 @@
 
 
 @frozen(order=True)
 class Particle:
     name: str
     latex: str
     spin: sp.Rational = field(converter=to_rational, validator=assert_spin_value)
-    parity: Literal[-1, 1]
+    parity: Literal[-1, 1] | None
     mass: float
     width: float
 
 
 @frozen(order=True)
 class State(Particle, Generic[StateIDTemplate]):
     """Initial or final state `.Particle` in a `ThreeBodyDecay`, carrying an index."""
@@ -113,25 +113,33 @@
         for chain in self.chains:
             if chain.resonance.name == resonance_name:
                 return chain
         msg = f"No decay chain found for resonance {resonance_name}"
         raise KeyError(msg)
 
     def get_subsystem(self, subsystem_id: FinalStateID) -> ThreeBodyDecay:
-        child1_id, child2_id = get_decay_product_ids(subsystem_id)
-        child1 = self.final_state[child1_id]
-        child2 = self.final_state[child2_id]
-        filtered_chains = [
-            chain
-            for chain in self.chains
-            if chain.decay_products in {(child1, child2), (child2, child1)}
-        ]
+        filtered_chains = [c for c in self.chains if c.spectator.index == subsystem_id]
+        if not filtered_chains:
+            decay_description = _get_decay_description(self)
+            subsystems = ", ".join(sorted(str(i) for i in _get_subsystem_ids(self)))
+            msg = f"Decay {decay_description} only has subsystems {subsystems}, not {subsystem_id}"
+            warn(msg, category=UserWarning)
         return ThreeBodyDecay(self.states, filtered_chains)
 
 
+def _get_decay_description(decay: ThreeBodyDecay) -> str:
+    initial_state = decay.initial_state.name
+    final_state = ", ".join(f"{i}: {s.name}" for i, s in decay.final_state.items())
+    return f"{initial_state} → {final_state}"
+
+
+def _get_subsystem_ids(decay: ThreeBodyDecay) -> set[FinalStateID]:
+    return {c.spectator.index for c in decay.chains}
+
+
 def get_decay_product_ids(
     spectator_id: FinalStateID,
 ) -> tuple[FinalStateID, FinalStateID]:
     if spectator_id == 1:
         return 2, 3
     if spectator_id == 2:  # noqa: PLR2004
         return 3, 1
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/dynamics/__init__.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/dynamics/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Functions for dynamics lineshapes and kinematics."""
 
+# pyright:reportPrivateUsage=false
 from __future__ import annotations
 
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import sympy as sp
 from ampform.dynamics import formulate_form_factor
 from ampform.kinematics.phasespace import Kallen
 from ampform.sympy import unevaluated
 
+if TYPE_CHECKING:
+    from sympy.printing.latex import LatexPrinter
+
 
 @unevaluated
 class RelativisticBreitWigner(sp.Expr):
     s: Any
     mass0: Any
     gamma0: Any
     m1: Any
@@ -41,27 +45,27 @@
 
 
 @unevaluated
 class P(sp.Expr):
     s: Any
     mi: Any
     mj: Any
-    _latex_repr_ = R"p_{{{mi},{mj}}}\left({s}\right)"
+    _latex_repr_ = R"p_{{_{{{mi},{mj}}}}}\left({s}\right)"
 
     def evaluate(self):
         s, mi, mj = self.args
         return sp.sqrt(Kallen(s, mi**2, mj**2)) / (2 * sp.sqrt(s))
 
 
 @unevaluated
 class Q(sp.Expr):
     s: Any
     m0: Any
     mk: Any
-    _latex_repr_ = R"q_{{{m0},{mk}}}\left({s}\right)"
+    _latex_repr_ = R"q_{{_{{{m0},{mk}}}}}\left({s}\right)"
 
     def evaluate(self):
         s, m0, mk = self.args
         return sp.sqrt(Kallen(s, m0**2, mk**2)) / (2 * m0)  # <-- not s!
 
 
 @unevaluated
@@ -144,15 +148,14 @@
     s: Any
     m0: Any
     Γ0: Any
     m1: Any
     m2: Any
     L: Any
     R: Any
-    _latex_repr_ = R"\Gamma\left({s}\right)"
 
     def evaluate(self):
         s, m0, Γ0, m1, m2, L, R = self.args
         p = P(s, m1, m2)
         p0 = P(m0**2, m1, m2)
         ff = BlattWeisskopf(p * R, L) ** 2
         ff0 = BlattWeisskopf(p0 * R, L) ** 2
@@ -160,14 +163,23 @@
             Γ0,
             (p / p0) ** (2 * L + 1),
             m0 / sp.sqrt(s),
             ff / ff0,
             evaluate=False,
         )
 
+    def _latex_repr_(self, printer: LatexPrinter) -> str:
+        s = printer._print(self.s)  # pyright:ignore[reportPrivateUsage]
+        if self.L == 0:
+            if self.m1 == 0 and self.m2 == 0:
+                return printer._print(self.Γ0)  # pyright:ignore[reportPrivateUsage]
+            return Rf"\Gamma\left({s}\right)"
+        L = printer._print(self.L)  # pyright:ignore[reportPrivateUsage]
+        return Rf"\Gamma_{{{L}}}\left({s}\right)"
+
 
 @unevaluated
 class BlattWeisskopf(sp.Expr):
     z: Any
     L: Any
     _latex_repr_ = R"F_{{{L}}}\left({z}\right)"
 
@@ -198,7 +210,91 @@
         return formulate_form_factor(
             s=s,
             m_a=m1,
             m_b=m2,
             angular_momentum=angular_momentum,
             meson_radius=meson_radius,
         )
+
+
+@unevaluated
+class MultichannelBreitWigner(sp.Expr):
+    s: Any
+    mass: Any
+    channels: tuple[ChannelArguments, ...]
+
+    def evaluate(self):
+        s = self.s
+        m0 = self.mass
+        width = sum(channel.evaluate() for channel in self.channels)
+        return BreitWigner(s, m0, width)
+
+    def _latex_repr_(self, printer: LatexPrinter, *args) -> str:
+        latex = R"\mathcal{R}^\mathrm{BW}_\mathrm{multi}\left("
+        latex += printer._print(self.s) + "; "
+        latex += ", ".join(printer._print(channel.width) for channel in self.channels)
+        latex += R"\right)"
+        return latex
+
+
+@unevaluated
+class ChannelArguments(sp.Expr):
+    s: Any
+    m0: Any
+    width: Any
+    m1: Any = 0
+    m2: Any = 0
+    angular_momentum: Any = 0
+    meson_radius: Any = 1
+    _latex_repr_ = R"\Gamma^\text{channel}\left({{s}}, {{m0}}, {{width}}\right)"
+
+    def evaluate(self) -> sp.Expr:
+        s, m0, Γ0, m1, m2, L, R = self.args
+        ff = FormFactor(s, m1, m2, L, R) ** 2
+        return Γ0 * m0 / sp.sqrt(s) * ff  # type:ignore[operator]
+
+
+@unevaluated
+class BreitWigner(sp.Expr):
+    s: Any
+    mass: Any
+    width: Any
+    m1: Any = 0
+    m2: Any = 0
+    angular_momentum: Any = 0
+    meson_radius: Any = 1
+
+    def evaluate(self):
+        width = self.energy_dependent_width()
+        expr = SimpleBreitWigner(self.s, self.mass, width)
+        if self.angular_momentum == 0 and self.m1 == 0 and self.m2 == 0:
+            return expr.evaluate()
+        return expr
+
+    def energy_dependent_width(self) -> sp.Expr:
+        s, m0, Γ0, m1, m2, L, d = self.args
+        if L == 0 and m1 == 0 and m2 == 0:
+            return Γ0  # type:ignore[return-value]
+        return EnergyDependentWidth(s, m0, Γ0, m1, m2, L, d)
+
+    def _latex_repr_(self, printer: LatexPrinter, *args) -> str:
+        s = printer._print(self.s)
+        function_symbol = R"\mathcal{R}^\mathrm{BW}"
+        mass = printer._print(self.mass)
+        width = printer._print(self.width)
+        arg = Rf"\left({s}; {mass}, {width}\right)"
+        L = printer._print(self.angular_momentum)
+        if isinstance(self.angular_momentum, sp.Integer):
+            return Rf"{function_symbol}_{{L={L}}}{arg}"
+        return Rf"{function_symbol}_{{{L}}}{arg}"
+
+
+@unevaluated
+class SimpleBreitWigner(sp.Expr):
+    s: Any
+    mass: Any
+    width: Any
+    _latex_repr_ = R"\mathcal{{R}}^\mathrm{{BW}}\left({s}; {mass}, {width}\right)"
+
+    def evaluate(self):
+        s, m0, Γ0 = self.args
+        return 1 / (m0**2 - s - m0 * Γ0 * 1j)
```

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/dynamics/builder.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/dynamics/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     ThreeBodyDecayChain,
 )
 from ampform_dpd.dynamics import FormFactor, RelativisticBreitWigner
 
 
 def formulate_breit_wigner_with_form_factor(
     decay: ThreeBodyDecayChain,
-) -> tuple[sp.Expr, dict[sp.Symbol, float]]:
+) -> tuple[sp.Expr, dict[sp.Symbol, complex | float]]:
     decay_node = decay.decay_node
     s = get_mandelstam_s(decay_node)
     parameter_defaults = {}
     production_ff, new_pars = _create_form_factor(s, decay.production_node)
     parameter_defaults.update(new_pars)
     decay_ff, new_pars = _create_form_factor(s, decay_node)
     parameter_defaults.update(new_pars)
@@ -37,42 +37,42 @@
         production_ff * decay_ff * breit_wigner,
         parameter_defaults,
     )
 
 
 def _create_form_factor(
     s: sp.Symbol, isobar: IsobarNode
-) -> tuple[sp.Expr, dict[sp.Symbol, float]]:
+) -> tuple[sp.Expr, dict[sp.Symbol, complex | float]]:
     if isinstance(isobar.parent, State):
         inv_mass = sp.Symbol("m0", nonnegative=True)
     else:
         inv_mass = get_mandelstam_s(isobar)
     outgoing_state_mass1 = create_mass_symbol(isobar.child1)
     outgoing_state_mass2 = create_mass_symbol(isobar.child2)
     meson_radius = _create_meson_radius_symbol(isobar)
     form_factor = FormFactor(
         s=inv_mass**2,
         m1=outgoing_state_mass1,
         m2=outgoing_state_mass2,
         angular_momentum=_get_angular_momentum(isobar),
         meson_radius=meson_radius,
     )
-    parameter_defaults = {
+    parameter_defaults: dict[sp.Symbol, complex | float] = {
         meson_radius: 1,
         outgoing_state_mass1: to_particle(isobar.child1).mass,
         outgoing_state_mass2: to_particle(isobar.child2).mass,
     }
     if not inv_mass.name.startswith("s"):
         parameter_defaults[inv_mass] = to_particle(isobar).mass
     return form_factor, parameter_defaults
 
 
 def _create_breit_wigner(
     s: sp.Symbol, isobar: DecayNode
-) -> tuple[sp.Expr, dict[sp.Symbol, float]]:
+) -> tuple[sp.Expr, dict[sp.Symbol, complex | float]]:
     outgoing_state_mass1 = create_mass_symbol(isobar.child1)
     outgoing_state_mass2 = create_mass_symbol(isobar.child2)
     angular_momentum = _get_angular_momentum(isobar)
     res_mass = create_mass_symbol(isobar.parent)
     res_width = sp.Symbol(Rf"\Gamma_{{{isobar.parent.latex}}}", nonnegative=True)
     meson_radius = _create_meson_radius_symbol(isobar)
 
@@ -81,15 +81,15 @@
         mass0=res_mass,
         gamma0=res_width,
         m1=outgoing_state_mass1,
         m2=outgoing_state_mass2,
         angular_momentum=angular_momentum,
         meson_radius=meson_radius,
     )
-    parameter_defaults = {
+    parameter_defaults: dict[sp.Symbol, complex | float] = {
         res_mass: isobar.parent.mass,
         res_width: isobar.parent.width,
         meson_radius: 1,
     }
     return breit_wigner_expr, parameter_defaults
 
 
@@ -98,16 +98,16 @@
         msg = "Need LS couplings to formulate a form factor"
         raise ValueError(msg)
     return isobar.interaction.L
 
 
 def _create_meson_radius_symbol(isobar: IsobarNode) -> sp.Symbol:
     if isinstance(isobar.parent, State):
-        return sp.Symbol(Rf"R_{{{isobar.parent.latex}}}")
-    return sp.Symbol(R"R_\mathrm{res}")
+        return sp.Symbol(Rf"R_{{{isobar.parent.latex}}}", nonnegative=True)
+    return sp.Symbol(R"R_\mathrm{res}", nonnegative=True)
 
 
 def create_mass_symbol(particle: IsobarNode | Particle) -> sp.Symbol:
     particle = to_particle(particle)
     return sp.Symbol(f"m_{{{particle.latex}}}", nonnegative=True)
```

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/io.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/io/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,19 +24,17 @@
 from importlib.metadata import version
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Iterable, Mapping, Sequence, overload
 
 import cloudpickle
 import sympy as sp
 from ampform.io import aslatex
-from ampform.sympy import (
-    perform_cached_doit,  # noqa: F401  # pyright:ignore[reportUnusedImport]
-)
 from tensorwaves.function.sympy import create_function, create_parametrized_function
 
+from ampform_dpd import DefinedExpression
 from ampform_dpd._cache import get_readable_hash, get_system_cache_directory
 from ampform_dpd.decay import (
     IsobarNode,
     Particle,
     State,
     ThreeBodyDecay,
     ThreeBodyDecayChain,
@@ -48,59 +46,14 @@
         PositionalArgumentFunction,
     )
     from tensorwaves.interface import Function, ParameterValue, ParametrizedFunction
 
 _LOGGER = logging.getLogger(__name__)
 
 
-@aslatex.register(complex)
-def _(obj: complex, **kwargs) -> str:
-    real = __downcast(obj.real)
-    imag = __downcast(obj.imag)
-    plus = "+" if imag >= 0 else ""
-    return f"{real}{plus}{imag}i"
-
-
-def __downcast(obj: float) -> float | int:
-    if obj.is_integer():
-        return int(obj)
-    return obj
-
-
-@aslatex.register(sp.Basic)
-def _(obj: sp.Basic, **kwargs) -> str:
-    return sp.latex(obj)
-
-
-@aslatex.register(abc.Mapping)
-def _(obj: Mapping, **kwargs) -> str:
-    if len(obj) == 0:
-        msg = "Need at least one dictionary item"
-        raise ValueError(msg)
-    latex = R"\begin{array}{rcl}" + "\n"
-    for lhs, rhs in obj.items():
-        latex += Rf"  {aslatex(lhs, **kwargs)} &=& {aslatex(rhs, **kwargs)} \\" + "\n"
-    latex += R"\end{array}"
-    return latex
-
-
-@aslatex.register(abc.Iterable)
-def _(obj: Iterable, **kwargs) -> str:
-    obj = list(obj)
-    if len(obj) == 0:
-        msg = "Need at least one item to render as LaTeX"
-        raise ValueError(msg)
-    latex = R"\begin{array}{c}" + "\n"
-    for item in obj:
-        item_latex = aslatex(item, **kwargs)
-        latex += Rf"  {item_latex} \\" + "\n"
-    latex += R"\end{array}"
-    return latex
-
-
 @aslatex.register(IsobarNode)
 def _(obj: IsobarNode, **kwargs) -> str:
     def render_arrow(node: IsobarNode) -> str:
         if node.interaction is None:
             return R"\to"
         return Rf"\xrightarrow[S={node.interaction.S}]{{L={node.interaction.L}}}"
 
@@ -130,20 +83,37 @@
         return _render_jp(obj)
     if with_jp:
         jp = _render_jp(obj)
         return Rf"{obj.latex}\left[{jp}\right]"
     return obj.latex
 
 
+@aslatex.register(DefinedExpression)
+def _(obj: DefinedExpression, **kwargs) -> str:
+    latex = R"\begin{array}{rcl}" + "\n"
+    expr = obj.expression
+    unfolded = expr.doit(deep=False)
+    if expr == unfolded:
+        latex += Rf"  {aslatex(obj.expression, **kwargs)} \\" + "\n"
+    else:
+        latex += Rf"  {aslatex(expr)} &=& {aslatex(unfolded)} \\" + "\n"
+    for lhs, rhs in obj.definitions.items():
+        latex += Rf"  {aslatex(lhs)} &=& {aslatex(rhs)} \\" + "\n"
+    latex += R"\end{array}"
+    return latex
+
+
 def _render_jp(particle: Particle) -> str:
-    parity = "-" if particle.parity < 0 else "+"
     if particle.spin.denominator == 1:
         spin = sp.latex(particle.spin)
     else:
         spin = Rf"\frac{{{particle.spin.numerator}}}{{{particle.spin.denominator}}}"
+    if particle.parity is None:
+        return f"J={spin}"
+    parity = "-" if particle.parity < 0 else "+"
     return f"{spin}^{parity}"
 
 
 def as_markdown_table(obj: Sequence) -> str:
     """Render objects a `str` suitable for generating a table."""
     if isinstance(obj, ThreeBodyDecay):
         return _as_decay_markdown_table(obj.chains)
@@ -155,21 +125,42 @@
     msg = (
         f"Cannot render a sequence with {item_type.__name__} items as a Markdown table"
     )
     raise NotImplementedError(msg)
 
 
 def _determine_item_type(obj) -> type:
+    """Determine the type of the items in a sequence.
+
+    >>> _determine_item_type([1, 2, 3])
+    <class 'int'>
+    >>> _determine_item_type([True, False])
+    <class 'bool'>
+    >>> _determine_item_type([True, False, 1])
+    <class 'int'>
+    >>> _determine_item_type([3.14, 1 + 1j])
+    Traceback (most recent call last):
+        ...
+    ValueError: Not all items are of type float'
+    """
     if not isinstance(obj, abc.Sequence):
         return type(obj)
     if len(obj) < 1:
         msg = "Need at least one entry to render a table"
         raise ValueError(msg)
-    item_type = type(obj[0])
-    if not all(isinstance(i, item_type) for i in obj):
+    existing_types = {type(i) for i in obj}
+    existing_types = {
+        typ
+        for typ in existing_types
+        if not any(
+            typ is not other and issubclass(typ, other) for other in existing_types
+        )
+    }
+    item_type = next(iter(existing_types))
+    if len(existing_types) != 1:
         msg = f"Not all items are of type {item_type.__name__}"
         raise ValueError(msg)
     return item_type
 
 
 def _as_resonance_markdown_table(items: Sequence[Particle | State]) -> str:
     column_names = [
@@ -199,17 +190,19 @@
 
 def _as_decay_markdown_table(decay_chains: Sequence[ThreeBodyDecayChain]) -> str:
     column_names = [
         "resonance",
         R"$J^P$",
         R"mass (MeV)",
         R"width (MeV)",
-        R"$L_\mathrm{dec}^\mathrm{min}$",
-        R"$L_\mathrm{prod}^\mathrm{min}$",
     ]
+    if any(c.outgoing_ls is not None for c in decay_chains):
+        column_names.append(R"$L_\mathrm{dec}^\mathrm{min}$")
+    if any(c.incoming_ls is not None for c in decay_chains):
+        column_names.append(R"$L_\mathrm{prod}^\mathrm{min}$")
     src = _create_markdown_table_header(column_names)
     for chain in decay_chains:
         child1, child2 = map(aslatex, chain.decay_products)
         row_items: list = [
             Rf"${chain.resonance.latex} \to {child1} {child2}$",
             Rf"${aslatex(chain.resonance, only_jp=True)}$",  # type:ignore[call-arg]
             f"{int(1e3 * chain.resonance.mass):,.0f}",
```

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd/spin.py` & `ampform_dpd-0.2.1rc0/src/ampform_dpd/spin.py`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd.egg-info/PKG-INFO` & `ampform_dpd-0.2.1rc0/src/ampform_dpd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampform-dpd
-Version: 0.2.0
+Version: 0.2.1rc0
 Summary: Symbolic expressions for Dalitz-Plot Decomposition
 Author-email: Common Partial Wave Analysis <compwa-admin@ep1.rub.de>
 License: GPLv3 or later
 Project-URL: Changelog, https://github.com/ComPWA/ampform-dpd/releases
 Project-URL: Documentation, https://compwa.github.io/ampform-dpd
 Project-URL: Source, https://github.com/ComPWA/ampform-dpd
 Project-URL: Tracker, https://github.com/ComPWA/ampform-dpd/issues
@@ -23,33 +23,36 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ampform>=0.14.8
+Requires-Dist: ampform>=0.15.1
 Requires-Dist: attrs>=20.1.0
 Requires-Dist: cloudpickle
 Requires-Dist: qrules>=0.10.0
 Requires-Dist: sympy>=1.10
 Requires-Dist: tensorwaves[jax]
+Requires-Dist: typing-extensions; python_version < "3.11.0"
 Provides-Extra: dev
 Requires-Dist: ampform-dpd[doc]; extra == "dev"
 Requires-Dist: ampform-dpd[jupyter]; extra == "dev"
 Requires-Dist: ampform-dpd[sty]; extra == "dev"
 Requires-Dist: ampform-dpd[test]; extra == "dev"
+Requires-Dist: sphinx-autobuild!=2024.04.*; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: tox>=1.9; extra == "dev"
 Provides-Extra: doc
 Requires-Dist: graphviz; extra == "doc"
 Requires-Dist: ipympl; extra == "doc"
 Requires-Dist: ipywidgets; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: myst-nb>=0.14; extra == "doc"
+Requires-Dist: pandas; extra == "doc"
 Requires-Dist: sphinx-api-relink>=0.0.4; extra == "doc"
 Requires-Dist: sphinx-book-theme; extra == "doc"
 Requires-Dist: sphinx-codeautolink[ipython]; extra == "doc"
 Requires-Dist: sphinx-copybutton; extra == "doc"
 Requires-Dist: sphinx-design; extra == "doc"
 Requires-Dist: sphinx-pybtex-etal-style; extra == "doc"
 Requires-Dist: sphinx-togglebutton; extra == "doc"
@@ -106,10 +109,10 @@
 [![Test coverage](https://codecov.io/gh/ComPWA/ampform-dpd/branch/main/graph/badge.svg)](https://codecov.io/gh/ComPWA/ampform-dpd)
 
 [![GitPod](https://img.shields.io/badge/gitpod-open-blue?logo=gitpod)](https://gitpod.io/#https://github.com/ComPWA/ampform-dpd)
 [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
 [![Spelling checked](https://img.shields.io/badge/cspell-checked-brightgreen.svg)](https://github.com/streetsidesoftware/cspell/tree/master/packages/cspell)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-This repository is a (temporary) extension of [AmpForm](https://ampform.rtfd.io) and provides a symbolic implementation of Dalitz-plot decomposition ([10.1103/PhysRevD.101.034033](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.101.034033)) with [SymPy](https://www.sympy.org/en/index.html). It has been extracted from the [ComPWA/polarimetry](https://github.com/ComPWA/polarimetry) repository, which is not yet public.
+This repository is a (temporary) extension of [AmpForm](https://ampform.rtfd.io) and provides a symbolic implementation of Dalitz-plot decomposition ([10.1103/PhysRevD.101.034033](https://journals.aps.org/prd/abstract/10.1103/PhysRevD.101.034033)) with [SymPy](https://www.sympy.org/en/index.html). It has been extracted from the [ComPWA/polarimetry](https://github.com/ComPWA/polarimetry) repository ([10.1007/JHEP07(2023)228](<https://doi.org/10.1007/JHEP07(2023)228>)).
 
 Installation instructions can be found [here](https://compwa.github.io/ampform-dpd/#installation).
```

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd.egg-info/SOURCES.txt` & `ampform_dpd-0.2.1rc0/src/ampform_dpd.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .cspell.json
 .editorconfig
 .gitignore
 .gitpod.yml
 .pre-commit-config.yaml
 .prettierignore
+.readthedocs.yml
 .taplo.toml
 LICENSE
 README.md
 codecov.yml
 environment.yml
 pyproject.toml
 tox.ini
@@ -24,43 +25,55 @@
 .github/workflows/pr-linting.yml
 .github/workflows/release-drafter.yml
 .github/workflows/requirements.yml
 .vscode/.gitignore
 .vscode/extensions.json
 .vscode/settings.json
 docs/.gitignore
+docs/Lc2ppiK.json
 docs/comparison.md
 docs/conf.py
 docs/index.md
 docs/jpsi2ksp.ipynb
 docs/lc2pkpi.ipynb
 docs/references.bib
 docs/references.md
+docs/serialization.ipynb
 docs/xib2pkk.ipynb
 docs/_static/favicon.ico
 docs/comparison/d2kkk.ipynb
 docs/comparison/jpsi2phipipi.ipynb
 docs/comparison/jpsi2pipipi.ipynb
 src/ampform_dpd/__init__.py
 src/ampform_dpd/_attrs.py
 src/ampform_dpd/_cache.py
 src/ampform_dpd/angles.py
 src/ampform_dpd/decay.py
-src/ampform_dpd/io.py
 src/ampform_dpd/particle-definitions.yml
 src/ampform_dpd/py.typed
 src/ampform_dpd/spin.py
 src/ampform_dpd/version.py
 src/ampform_dpd.egg-info/PKG-INFO
 src/ampform_dpd.egg-info/SOURCES.txt
 src/ampform_dpd.egg-info/dependency_links.txt
 src/ampform_dpd.egg-info/requires.txt
 src/ampform_dpd.egg-info/top_level.txt
 src/ampform_dpd/adapter/__init__.py
 src/ampform_dpd/adapter/qrules.py
 src/ampform_dpd/dynamics/__init__.py
 src/ampform_dpd/dynamics/builder.py
+src/ampform_dpd/io/__init__.py
+src/ampform_dpd/io/serialization/__init__.py
+src/ampform_dpd/io/serialization/amplitude.py
+src/ampform_dpd/io/serialization/decay.py
+src/ampform_dpd/io/serialization/dynamics.py
+src/ampform_dpd/io/serialization/format.py
 tests/test_angles.py
 tests/test_decay.py
 tests/test_io.py
 tests/adapter/__init__.py
-tests/adapter/test_qrules.py
+tests/adapter/test_qrules.py
+tests/io_serialization/__init__.py
+tests/io_serialization/conftest.py
+tests/io_serialization/test_amplitude.py
+tests/io_serialization/test_decay.py
+tests/io_serialization/test_format.py
```

### Comparing `ampform_dpd-0.2.0/src/ampform_dpd.egg-info/requires.txt` & `ampform_dpd-0.2.1rc0/src/ampform_dpd.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-ampform>=0.14.8
+ampform>=0.15.1
 attrs>=20.1.0
 cloudpickle
 qrules>=0.10.0
 sympy>=1.10
 tensorwaves[jax]
 
+[:python_version < "3.11.0"]
+typing-extensions
+
 [dev]
 ampform-dpd[doc]
 ampform-dpd[jupyter]
 ampform-dpd[sty]
 ampform-dpd[test]
+sphinx-autobuild!=2024.04.*
 sphinx-autobuild
 tox>=1.9
 
 [doc]
 graphviz
 ipympl
 ipywidgets
 matplotlib
 myst-nb>=0.14
+pandas
 sphinx-api-relink>=0.0.4
 sphinx-book-theme
 sphinx-codeautolink[ipython]
 sphinx-copybutton
 sphinx-design
 sphinx-pybtex-etal-style
 sphinx-togglebutton
```

### Comparing `ampform_dpd-0.2.0/tests/adapter/test_qrules.py` & `ampform_dpd-0.2.1rc0/tests/adapter/test_qrules.py`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/tests/test_angles.py` & `ampform_dpd-0.2.1rc0/tests/test_angles.py`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/tests/test_decay.py` & `ampform_dpd-0.2.1rc0/tests/test_decay.py`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/tests/test_io.py` & `ampform_dpd-0.2.1rc0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `ampform_dpd-0.2.0/tox.ini` & `ampform_dpd-0.2.1rc0/tox.ini`

 * *Files identical despite different names*

