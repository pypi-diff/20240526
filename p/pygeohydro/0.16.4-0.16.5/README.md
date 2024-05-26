# Comparing `tmp/pygeohydro-0.16.4.tar.gz` & `tmp/pygeohydro-0.16.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeohydro-0.16.4.tar", last modified: Mon May 20 21:25:48 2024, max compression
+gzip compressed data, was "pygeohydro-0.16.5.tar", last modified: Sun May 26 15:35:15 2024, max compression
```

## Comparing `pygeohydro-0.16.4.tar` & `pygeohydro-0.16.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.919981 pygeohydro-0.16.4/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.deepsource.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.911981 pygeohydro-0.16.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.911981 pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/bugreport.yml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/newfeature.yml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.911981 pygeohydro-0.16.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/.sonarcloud.properties
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    37149 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22918 2024-05-20 21:25:48.919981 pygeohydro-0.16.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.907981 pygeohydro-0.16.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.911981 pygeohydro-0.16.4/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/ci/requirements/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/ci/requirements/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.915981 pygeohydro-0.16.4/pygeohydro/
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/nfhl.py
--rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/nlcd.py
--rw-r--r--   0 runner    (1001) docker     (127)    27551 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/nwis.py
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    36883 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/pygeohydro.py
--rw-r--r--   0 runner    (1001) docker     (127)    24736 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/stnfloodevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/us_abbrs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/waterdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pygeohydro/watershed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.915981 pygeohydro-0.16.4/pygeohydro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22918 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 21:25:48.000000 pygeohydro-0.16.4/pygeohydro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:25:48.919981 pygeohydro-0.16.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:25:48.915981 pygeohydro-0.16.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14480 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/tests/test_pygeohydro.py
--rw-r--r--   0 runner    (1001) docker     (127)    19485 2024-05-20 21:25:37.000000 pygeohydro-0.16.4/tests/test_stn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:15.714836 pygeohydro-0.16.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.deepsource.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:15.706836 pygeohydro-0.16.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:15.706836 pygeohydro-0.16.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/ISSUE_TEMPLATE/bugreport.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/ISSUE_TEMPLATE/newfeature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:15.706836 pygeohydro-0.16.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/.sonarcloud.properties
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    37583 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-05-26 15:35:15.710836 pygeohydro-0.16.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20936 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:15.702836 pygeohydro-0.16.5/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:15.706836 pygeohydro-0.16.5/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/ci/requirements/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/ci/requirements/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/noxfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:15.710836 pygeohydro-0.16.5/pygeohydro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9190 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/nfhl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/nlcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27551 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/nwis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42639 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/pygeohydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24736 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/stnfloodevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/us_abbrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14950 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/waterdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pygeohydro/watershed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:15.710836 pygeohydro-0.16.5/pygeohydro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-05-26 15:35:15.000000 pygeohydro-0.16.5/pygeohydro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-26 15:35:15.000000 pygeohydro-0.16.5/pygeohydro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:35:15.000000 pygeohydro-0.16.5/pygeohydro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 15:35:15.000000 pygeohydro-0.16.5/pygeohydro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-26 15:35:15.000000 pygeohydro-0.16.5/pygeohydro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 15:35:15.000000 pygeohydro-0.16.5/pygeohydro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 15:35:15.714836 pygeohydro-0.16.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 15:35:15.710836 pygeohydro-0.16.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/tests/test_pygeohydro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19485 2024-05-26 15:35:04.000000 pygeohydro-0.16.5/tests/test_stn.py
```

### Comparing `pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/bugreport.yml` & `pygeohydro-0.16.5/.github/ISSUE_TEMPLATE/bugreport.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/.github/ISSUE_TEMPLATE/newfeature.yml` & `pygeohydro-0.16.5/.github/ISSUE_TEMPLATE/newfeature.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/.github/workflows/codeql-analysis.yml` & `pygeohydro-0.16.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/.github/workflows/release.yml` & `pygeohydro-0.16.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/.github/workflows/test.yml` & `pygeohydro-0.16.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/.gitignore` & `pygeohydro-0.16.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/.pre-commit-config.yaml` & `pygeohydro-0.16.5/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   hooks:
   - id: blacken-docs
     name: Autoformat codes in docstrings with blacken-docs
     additional_dependencies: [black]
     args: [-t, py38, -l, '100']
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.4.4
+  rev: v0.4.5
   hooks:
   - id: ruff
     name: Linting with Ruff
     types_or: [python]
     args: [--fix]
   - id: ruff-format
     name: Formatting with Ruff
@@ -35,15 +35,15 @@
   rev: v1.1.1
   hooks:
   - id: doc8
     name: Check documentation formats with doc8
     args: [--max-line-length, '100']
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.6
+  rev: v2.3.0
   hooks:
   - id: codespell
     name: Check common misspellings in text files with codespell.
     additional_dependencies:
     - tomli
 
 - repo: https://github.com/dosisod/refurb
@@ -51,15 +51,15 @@
   hooks:
   - id: refurb
     name: Modernizing Python codebases using Refurb
     additional_dependencies:
     - numpy
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: 2.1.1
+  rev: 2.1.3
   hooks:
   - id: pyproject-fmt
     name: Apply a consistent format to pyproject.toml
 
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.6.0
   hooks:
```

### Comparing `pygeohydro-0.16.4/CITATION.cff` & `pygeohydro-0.16.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/CODE_OF_CONDUCT.rst` & `pygeohydro-0.16.5/CODE_OF_CONDUCT.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ----------
 
 In the interest of fostering an open and welcoming environment, we as
 contributors and maintainers pledge to making participation in our
 project and our community a harassment-free experience for everyone,
 regardless of age, body size, disability, ethnicity, sex
 characteristics, gender identity and expression, level of experience,
-education, socio-economic status, nationality, personal appearance,
+education, socioeconomic status, nationality, personal appearance,
 race, religion, or sexual identity and orientation.
 
 Our Standards
 -------------
 
 Examples of behavior that contributes to creating a positive environment
 include:
```

### Comparing `pygeohydro-0.16.4/CONTRIBUTING.rst` & `pygeohydro-0.16.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/HISTORY.rst` & `pygeohydro-0.16.5/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =======
 History
 =======
 
+0.16.5 (2024-05-26)
+-------------------
+
+New Features
+~~~~~~~~~~~~
+- Add new function called ``soil_soilgrids`` to get soil data from the
+  SoilGrids dataset. The signature of the function is the same as of the
+  ``soil_gnatsgo`` function, so they can be used interchangeably.
+  For more information on the SoilGrids dataset, visit
+  `ISRIC <https://www.isric.org/explore/soilgrids/faq-soilgrids#What_do_the_filename_codes_mean>`__.
+
 0.16.4 (2024-05-20)
 -------------------
 
 Bug Fixes
 ~~~~~~~~~
 - Fix an issue in ``NID.stage_nid_inventory`` where the function was failing
   when the response status code was 206 (partial content). This issue is fixed
```

### Comparing `pygeohydro-0.16.4/LICENSE` & `pygeohydro-0.16.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/PKG-INFO` & `pygeohydro-0.16.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeohydro
-Version: 0.16.4
+Version: 0.16.5
 Summary: Access geospatial web services that offer hydrological data
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pygeohydro.html
 Project-URL: CI, https://github.com/hyriver/pygeohydro/actions
 Project-URL: Homepage, https://docs.hyriver.io/readme/pygeohydro.html
 Project-URL: Issues, https://github.com/hyriver/pygeohydro/issues
@@ -158,17 +158,17 @@
 
 |
 
 .. image:: https://www.codefactor.io/repository/github/hyriver/pygeohydro/badge/main
     :target: https://www.codefactor.io/repository/github/hyriver/pygeohydro/overview/main
     :alt: CodeFactor
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: black
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
     :target: https://github.com/pre-commit/pre-commit
     :alt: pre-commit
 
 .. image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/hyriver/HyRiver-examples/main?urlpath=lab/tree/notebooks
@@ -185,14 +185,16 @@
 access to some public web services that offer geospatial hydrology data. It has three
 main modules: ``pygeohydro``, ``plot``, and ``helpers``.
 
 PyGeoHydro supports the following datasets:
 
 * `gNATSGO <https://planetarycomputer.microsoft.com/dataset/gnatsgo-rasters>`__ for
   US soil properties.
+* `SoilGrids <https://www.isric.org/explore/soilgrids/faq-soilgrids#What_do_the_filename_codes_mean>`__
+  for seamless global soil properties.
 * `Derived Soil Properties <https://www.sciencebase.gov/catalog/item/5fd7c19cd34e30b9123cb51f>`__
   for soil porosity, available water capacity, and field capacity across the US.
 * `NWIS <https://nwis.waterdata.usgs.gov/nwis>`__ for daily mean streamflow observations
   (returned as a ``pandas.DataFrame`` or ``xarray.Dataset`` with station attributes),
 * `SensorThings API <https://labs.waterdata.usgs.gov/api-docs/about-sensorthings-api/index.html>`__
   for accessing real-time data of USGS sensors.
 * `CAMELS <https://ral.ucar.edu/solutions/products/camels>`__ for accessing streamflow
```

### Comparing `pygeohydro-0.16.4/README.rst` & `pygeohydro-0.16.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,17 @@
 
 |
 
 .. image:: https://www.codefactor.io/repository/github/hyriver/pygeohydro/badge/main
     :target: https://www.codefactor.io/repository/github/hyriver/pygeohydro/overview/main
     :alt: CodeFactor
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: black
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
     :target: https://github.com/pre-commit/pre-commit
     :alt: pre-commit
 
 .. image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/hyriver/HyRiver-examples/main?urlpath=lab/tree/notebooks
@@ -127,14 +127,16 @@
 access to some public web services that offer geospatial hydrology data. It has three
 main modules: ``pygeohydro``, ``plot``, and ``helpers``.
 
 PyGeoHydro supports the following datasets:
 
 * `gNATSGO <https://planetarycomputer.microsoft.com/dataset/gnatsgo-rasters>`__ for
   US soil properties.
+* `SoilGrids <https://www.isric.org/explore/soilgrids/faq-soilgrids#What_do_the_filename_codes_mean>`__
+  for seamless global soil properties.
 * `Derived Soil Properties <https://www.sciencebase.gov/catalog/item/5fd7c19cd34e30b9123cb51f>`__
   for soil porosity, available water capacity, and field capacity across the US.
 * `NWIS <https://nwis.waterdata.usgs.gov/nwis>`__ for daily mean streamflow observations
   (returned as a ``pandas.DataFrame`` or ``xarray.Dataset`` with station attributes),
 * `SensorThings API <https://labs.waterdata.usgs.gov/api-docs/about-sensorthings-api/index.html>`__
   for accessing real-time data of USGS sensors.
 * `CAMELS <https://ral.ucar.edu/solutions/products/camels>`__ for accessing streamflow
```

### Comparing `pygeohydro-0.16.4/ci/requirements/environment-dev.yml` & `pygeohydro-0.16.5/ci/requirements/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/ci/requirements/environment.yml` & `pygeohydro-0.16.5/ci/requirements/environment.yml`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/noxfile.py` & `pygeohydro-0.16.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/__init__.py` & `pygeohydro-0.16.5/pygeohydro/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from pygeohydro.print_versions import show_versions
 from pygeohydro.pygeohydro import (
     NID,
     EHydro,
     get_camels,
     soil_gnatsgo,
     soil_properties,
+    soil_soilgrids,
     ssebopeta_bycoords,
     ssebopeta_bygeom,
 )
 from pygeohydro.stnfloodevents import STNFloodEventData, stn_flood_event
 from pygeohydro.waterdata import SensorThings, WaterQuality
 from pygeohydro.watershed import WBD, huc_wb_full, irrigation_withdrawals
 
@@ -67,14 +68,15 @@
     "nlcd_bygeom",
     "nlcd_bycoords",
     "nlcd_area_percent",
     "ssebopeta_bygeom",
     "ssebopeta_bycoords",
     "soil_properties",
     "soil_gnatsgo",
+    "soil_soilgrids",
     "helpers",
     "get_us_states",
     "plot",
     "DataNotAvailableError",
     "InputRangeError",
     "InputTypeError",
     "MissingCRSError",
```

### Comparing `pygeohydro-0.16.4/pygeohydro/exceptions.py` & `pygeohydro-0.16.5/pygeohydro/exceptions.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/helpers.py` & `pygeohydro-0.16.5/pygeohydro/helpers.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/nfhl.py` & `pygeohydro-0.16.5/pygeohydro/nfhl.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/nlcd.py` & `pygeohydro-0.16.5/pygeohydro/nlcd.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/nwis.py` & `pygeohydro-0.16.5/pygeohydro/nwis.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/plot.py` & `pygeohydro-0.16.5/pygeohydro/plot.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/print_versions.py` & `pygeohydro-0.16.5/pygeohydro/print_versions.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/pygeohydro.py` & `pygeohydro-0.16.5/pygeohydro/pygeohydro.py`

 * *Files 24% similar despite different names*

```diff
@@ -51,19 +51,101 @@
 
 __all__ = [
     "get_camels",
     "ssebopeta_bycoords",
     "ssebopeta_bygeom",
     "soil_properties",
     "soil_gnatsgo",
+    "soil_properties",
     "NID",
     "EHydro",
 ]
 
 
+SG_ATTRS = {
+    "bdod": {
+        "description": "Bulk density of the fine earth fraction",
+        "long_name": "Bulk Density",
+        "mapped_units": "cg/cm³",
+        "conversion_factor": 100,
+        "conventional_units": "kg/dm³",
+    },
+    "cec": {
+        "description": "Cation Exchange Capacity of the soil",
+        "long_name": "Cation Exchange Capacity",
+        "mapped_units": "mmol(c)/kg",
+        "conversion_factor": 10,
+        "conventional_units": "cmol(c)/kg",
+    },
+    "cfvo": {
+        "description": "Volumetric fraction of coarse fragments (> 2 mm)",
+        "long_name": "Coarse Fragments Vol",
+        "mapped_units": "cm3/dm3 (vol‰)",
+        "conversion_factor": 10,
+        "conventional_units": "cm3/100cm3 (vol%)",
+    },
+    "clay": {
+        "description": "Proportion of clay particles (< 0.002 mm) in the fine earth fraction",
+        "long_name": "Clay Content",
+        "mapped_units": "g/kg",
+        "conversion_factor": 10,
+        "conventional_units": "g/100g (%)",
+    },
+    "nitrogen": {
+        "description": "Total nitrogen (N)",
+        "long_name": "Nitrogen Content",
+        "mapped_units": "cg/kg",
+        "conversion_factor": 100,
+        "conventional_units": "g/kg",
+    },
+    "phh2o": {
+        "description": "Soil pH",
+        "long_name": "Ph In H2O",
+        "mapped_units": "pHx10",
+        "conversion_factor": 10,
+        "conventional_units": "pH",
+    },
+    "sand": {
+        "description": "Proportion of sand particles (> 0.05 mm) in the fine earth fraction",
+        "long_name": "Sand Content",
+        "mapped_units": "g/kg",
+        "conversion_factor": 10,
+        "conventional_units": "g/100g (%)",
+    },
+    "silt": {
+        "description": "Proportion of silt particles (≥ 0.002 mm and ≤ 0.05 mm) in the fine earth fraction",
+        "long_name": "Silt Content",
+        "mapped_units": "g/kg",
+        "conversion_factor": 10,
+        "conventional_units": "g/100g (%)",
+    },
+    "soc": {
+        "description": "Soil organic carbon content in the fine earth fraction",
+        "long_name": "Soil Organic Carbon",
+        "mapped_units": "dg/kg",
+        "conversion_factor": 10,
+        "conventional_units": "g/kg",
+    },
+    "ocd": {
+        "description": "Organic carbon density",
+        "long_name": "Organic Carbon Density",
+        "mapped_units": "hg/m³",
+        "conversion_factor": 10,
+        "conventional_units": "kg/m³",
+    },
+    "ocs": {
+        "description": "Organic carbon stocks",
+        "long_name": "Organic Carbon Stock",
+        "mapped_units": "t/ha",
+        "conversion_factor": 10,
+        "conventional_units": "kg/m²",
+    },
+}
+
+
 def get_camels() -> tuple[gpd.GeoDataFrame, xr.Dataset]:
     """Get streaflow and basin attributes of all 671 stations in CAMELS dataset.
 
     Notes
     -----
     For more info on CAMELS visit: https://ral.ucar.edu/solutions/products/camels
 
@@ -806,37 +888,117 @@
         modifier=planetary_computer.sign_inplace,
     )
     bounds = geoutils.geo2polygon(geometry, crs, 4326).bounds
     search = catalog.search(collections=["gnatsgo-rasters"], bbox=bounds)
     lyr_href = tlz.merge_with(
         set, ({n: a.href for n, a in i.assets.items()} for i in search.items())
     )
-    lyrs = [layers.lower()] if isinstance(layers, str) else map(str.lower, layers)
+    layers_ = [layers] if isinstance(layers, str) else list(layers)
 
     def get_layer(lyr: str) -> xr.DataArray:
         fpaths = ogc.streaming_download(list(lyr_href[lyr]), file_extention="tiff")
         fpaths = [f for f in fpaths if f is not None]
         ds = xr.merge(_open_tiff(f, lyr) for f in fpaths)
         affine = ds.rio.transform(recalc=True)
         with rio.open(fpaths[0]) as src:
             ds_crs = src.crs
         ds = ds.rio.write_transform(affine)
         ds = ds.rio.write_crs(ds_crs)
         ds = ds.rio.write_coordinate_system()
         return ds
 
-    soil = xr.merge((get_layer(lyr) for lyr in lyrs), combine_attrs="drop_conflicts")
+    soil = xr.merge((get_layer(lyr) for lyr in layers_), combine_attrs="drop_conflicts")
     poly = geoutils.geo2polygon(geometry, crs, soil.rio.crs)
     soil = geoutils.xarray_geomask(soil, poly, soil.rio.crs)
     _ = soil.attrs.pop("_FillValue", None)
     _ = soil.attrs.pop("units", None)
     _ = soil.attrs.pop("long_name", None)
     return soil
 
 
+def soil_soilgrids(
+    layers: list[str] | str,
+    geometry: GTYPE,
+    geo_crs: CRSTYPE = 4326,
+) -> xr.Dataset:
+    """Get soil data from SoilGrids for the area of interest.
+
+    Notes
+    -----
+    For more information on the SoilGrids dataset, visit
+    `ISRIC <https://www.isric.org/explore/soilgrids/faq-soilgrids#What_do_the_filename_codes_mean>`__.
+
+    Parameters
+    ----------
+    layers : list of str
+        SoilGrids layers to get. Available options are:
+        ``bdod_*``, ``cec_*``, ``cfvo_*``, ``clay_*``, ``nitrogen_*``, ``ocd_*``,
+        ``ocs_*``, ``phh2o_*``, ``sand_*``, ``silt_*``, and ``soc_*`` where ``*``
+        is the depth in cm and can be one of ``5``, ``15``, ``30``, ``60``,
+        ``100``, or ``200``. For example, ``bdod_5`` is the mean bulk density of
+        the fine earth fraction at 0-5 cm depth, and ``bdod_200`` is the mean bulk
+        density of the fine earth fraction at 100-200 cm depth.
+    geometry : Polygon, MultiPolygon, or tuple of length 4
+        Geometry to get DEM within. It can be a polygon or a boundong box
+        of form (xmin, ymin, xmax, ymax).
+    geo_crs : int, str, of pyproj.CRS, optional
+        CRS of the input geometry, defaults to ``epsg:4326``.
+
+    Returns
+    -------
+    xarray.DataArray
+        The request DEM at the specified resolution.
+    """
+    layers_ = [layers] if isinstance(layers, str) else list(layers)
+    valid_depths = {
+        "5": "0-5cm",
+        "15": "5-15cm",
+        "30": "15-30cm",
+        "60": "30-60cm",
+        "100": "60-100cm",
+        "200": "100-200cm",
+    }
+    valid_layers = [
+        f"{layer}_{depth}"
+        for layer, depth in itertools.product(SG_ATTRS.keys(), valid_depths.keys())
+    ]
+    invalid_layers = [layer for layer in layers_ if layer not in valid_layers]
+    if invalid_layers:
+        raise InputValueError("layers", valid_layers, ", ".join(invalid_layers))
+    lyr_names, lyr_depths = zip(*[layer.split("_") for layer in layers_])
+    base_url = "https://files.isric.org/soilgrids/latest/data"
+    geometry_ = geoutils.geo2polygon(geometry)
+    bounds = geometry_.bounds
+
+    def _read_layer(lyr: str, depth: str) -> xr.DataArray:
+        """Read a SoilGrids layer."""
+        ds = rxr.open_rasterio(f"{base_url}/{lyr}/{lyr}_{depth}_mean.vrt")
+        ds = cast("xr.DataArray", ds)
+        ds = (
+            ds.squeeze(drop=True)
+            .rio.clip_box(*bounds, crs=geo_crs)
+            .rio.clip([geometry_], crs=geo_crs)
+        )
+        ds = ds.where(ds != ds.rio.nodata)
+        ds = ds.rio.write_nodata(np.nan)
+
+        # Convert mapped units to conventional units
+        attributes = SG_ATTRS[lyr]
+        ds = ds / attributes["conversion_factor"]
+
+        ds.name = f"{lyr}_{depth.replace('-', '_')}_mean"
+        ds.attrs["long_name"] = f"Mean {attributes['long_name']} ({depth})"
+        ds.attrs["description"] = attributes["description"]
+        ds.attrs["units"] = attributes["conventional_units"]
+
+        return ds
+
+    return xr.merge([_read_layer(lyr, valid_depths[d]) for lyr, d in zip(lyr_names, lyr_depths)])
+
+
 class EHydro(AGRBase):
     """Access USACE Hydrographic Surveys (eHydro).
 
     Notes
     -----
     For more info visit: https://navigation.usace.army.mil/Survey/Hydro
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygeohydro-0.16.4/pygeohydro/stnfloodevents.py` & `pygeohydro-0.16.5/pygeohydro/stnfloodevents.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/us_abbrs.py` & `pygeohydro-0.16.5/pygeohydro/us_abbrs.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/waterdata.py` & `pygeohydro-0.16.5/pygeohydro/waterdata.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro/watershed.py` & `pygeohydro-0.16.5/pygeohydro/watershed.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pygeohydro.egg-info/PKG-INFO` & `pygeohydro-0.16.5/pygeohydro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeohydro
-Version: 0.16.4
+Version: 0.16.5
 Summary: Access geospatial web services that offer hydrological data
 Author-email: Taher Chegini <cheginit@gmail.com>
 License: MIT
 Project-URL: Changelog, https://docs.hyriver.io/changelogs/pygeohydro.html
 Project-URL: CI, https://github.com/hyriver/pygeohydro/actions
 Project-URL: Homepage, https://docs.hyriver.io/readme/pygeohydro.html
 Project-URL: Issues, https://github.com/hyriver/pygeohydro/issues
@@ -158,17 +158,17 @@
 
 |
 
 .. image:: https://www.codefactor.io/repository/github/hyriver/pygeohydro/badge/main
     :target: https://www.codefactor.io/repository/github/hyriver/pygeohydro/overview/main
     :alt: CodeFactor
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: black
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
 .. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
     :target: https://github.com/pre-commit/pre-commit
     :alt: pre-commit
 
 .. image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/hyriver/HyRiver-examples/main?urlpath=lab/tree/notebooks
@@ -185,14 +185,16 @@
 access to some public web services that offer geospatial hydrology data. It has three
 main modules: ``pygeohydro``, ``plot``, and ``helpers``.
 
 PyGeoHydro supports the following datasets:
 
 * `gNATSGO <https://planetarycomputer.microsoft.com/dataset/gnatsgo-rasters>`__ for
   US soil properties.
+* `SoilGrids <https://www.isric.org/explore/soilgrids/faq-soilgrids#What_do_the_filename_codes_mean>`__
+  for seamless global soil properties.
 * `Derived Soil Properties <https://www.sciencebase.gov/catalog/item/5fd7c19cd34e30b9123cb51f>`__
   for soil porosity, available water capacity, and field capacity across the US.
 * `NWIS <https://nwis.waterdata.usgs.gov/nwis>`__ for daily mean streamflow observations
   (returned as a ``pandas.DataFrame`` or ``xarray.Dataset`` with station attributes),
 * `SensorThings API <https://labs.waterdata.usgs.gov/api-docs/about-sensorthings-api/index.html>`__
   for accessing real-time data of USGS sensors.
 * `CAMELS <https://ral.ucar.edu/solutions/products/camels>`__ for accessing streamflow
```

### Comparing `pygeohydro-0.16.4/pygeohydro.egg-info/SOURCES.txt` & `pygeohydro-0.16.5/pygeohydro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/pyproject.toml` & `pygeohydro-0.16.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -160,14 +160,25 @@
   "UP",
   # Warning
   "W",
   # flake8-2020
   "YTT",
 ]
 
+lint.ignore = [
+  "D103",
+  "D105",
+  "E501",
+  # conflict with ruff-formatter
+  "ISC001",
+  "PGH003",
+  "PLR0913",
+  "PLR2004",
+]
+
 lint.per-file-ignores."tests/*.py" = [
   "D100",
   "D101",
   "D102",
   "D103",
   "D104",
   "D105",
@@ -205,24 +216,14 @@
   "pygridmet",
   "pynldas2",
 ]
 lint.isort.required-imports = [
   "from __future__ import annotations",
 ]
 lint.pydocstyle.convention = "numpy"
-lint.ignore = [
-  "D103",
-  "D105",
-  "E501",
-  # conflict with ruff-formatter
-  "ISC001",
-  "PGH003",
-  "PLR0913",
-  "PLR2004",
-]
 
 [tool.codespell]
 skip = "__pycache__,_build,.mypy_cache,.git,./htmlcov,.nox,**/us_abbrs.py,cache"
 ignore-words-list = "gage,gages,paramss,trough"
 
 [tool.pytest.ini_options]
 addopts = "--ignore=noxfile.py -n=auto -v --cov=pygeohydro --cov-report xml --durations=5"
```

### Comparing `pygeohydro-0.16.4/tests/test_exceptions.py` & `pygeohydro-0.16.5/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pygeohydro-0.16.4/tests/test_pygeohydro.py` & `pygeohydro-0.16.5/tests/test_pygeohydro.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,22 @@
     assert soil.sizes["x"] == 266301
 
 
 def test_gnatsgo():
     layers = ["Tk0_100a", "Soc20_50"]
     geometry = (-95.624515, 30.121598, -95.448253, 30.264074)
     soil = gh.soil_gnatsgo(layers, geometry, 4326)
-    assert_close(soil.tk0_100a.mean().compute().item(), 89.848)
+    assert_close(soil.tk0_100a.mean().item(), 89.848)
+
+
+def test_soilgrid():
+    layers = "bdod_5"
+    geometry = (-95.624515, 30.121598, -95.448253, 30.264074)
+    soil = gh.soil_soilgrids(layers, geometry, 4326)
+    assert_close(soil.bdod_0_5cm_mean.mean().item(), 1.4459)
 
 
 def test_sensorthings():
     sensor = gh.SensorThings()
     cond = " and ".join(
         ("properties/monitoringLocationType eq 'Stream'", "properties/stateFIPS eq 'US:04'")
     )
```

### Comparing `pygeohydro-0.16.4/tests/test_stn.py` & `pygeohydro-0.16.5/tests/test_stn.py`

 * *Files identical despite different names*

