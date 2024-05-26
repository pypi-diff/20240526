# Comparing `tmp/gypsum_client-0.1.1.tar.gz` & `tmp/gypsum_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gypsum_client-0.1.1.tar", last modified: Mon May 20 03:08:11 2024, max compression
+gzip compressed data, was "gypsum_client-0.1.2.tar", last modified: Sun May 26 01:12:41 2024, max compression
```

## Comparing `gypsum_client-0.1.1.tar` & `gypsum_client-0.1.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:08:11.024049 gypsum_client-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:08:11.008049 gypsum_client-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:08:11.012049 gypsum_client-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-20 03:08:11.024049 gypsum_client-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:08:11.012049 gypsum_client-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:08:11.012049 gypsum_client-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-20 03:08:11.024049 gypsum_client-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:08:11.008049 gypsum_client-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:08:11.016049 gypsum_client-0.1.1/src/gypsum_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/cache_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/clone_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/create_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/fetch_metadata_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/fetch_metadata_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/fetch_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/list_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/prepare_directory_for_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/probation_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/refresh_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/remove_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/resolve_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/rest_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/s3_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/save_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/search_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/set_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/upload_api_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/upload_file_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/src/gypsum_client/validate_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:08:11.024049 gypsum_client-0.1.1/src/gypsum_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-20 03:08:10.000000 gypsum_client-0.1.1/src/gypsum_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-20 03:08:11.000000 gypsum_client-0.1.1/src/gypsum_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:08:10.000000 gypsum_client-0.1.1/src/gypsum_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:08:10.000000 gypsum_client-0.1.1/src/gypsum_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 03:08:10.000000 gypsum_client-0.1.1/src/gypsum_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 03:08:10.000000 gypsum_client-0.1.1/src/gypsum_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:08:11.024049 gypsum_client-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_fetch_metadata_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_fetch_metadata_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_latest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_prepare_dir_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_probation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-20 03:06:55.000000 gypsum_client-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.464810 gypsum_client-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.448810 gypsum_client-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.452810 gypsum_client-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-26 01:12:41.464810 gypsum_client-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.456810 gypsum_client-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.456810 gypsum_client-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-26 01:12:41.468810 gypsum_client-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.452810 gypsum_client-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.460810 gypsum_client-0.1.2/src/gypsum_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/cache_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/clone_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/create_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/fetch_metadata_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/fetch_metadata_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/fetch_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/list_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/prepare_directory_for_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/probation_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/refresh_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/remove_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/resolve_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/rest_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/s3_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/save_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/search_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/set_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/upload_api_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/upload_file_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/src/gypsum_client/validate_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.464810 gypsum_client-0.1.2/src/gypsum_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 01:12:41.000000 gypsum_client-0.1.2/src/gypsum_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 01:12:41.464810 gypsum_client-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_fetch_metadata_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_fetch_metadata_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_prepare_dir_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_probation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-26 01:11:21.000000 gypsum_client-0.1.2/tox.ini
```

### Comparing `gypsum_client-0.1.1/.coveragerc` & `gypsum_client-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/.github/workflows/pypi-publish.yml` & `gypsum_client-0.1.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/.github/workflows/pypi-test.yml` & `gypsum_client-0.1.2/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/.gitignore` & `gypsum_client-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/.pre-commit-config.yaml` & `gypsum_client-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/.readthedocs.yml` & `gypsum_client-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/CONTRIBUTING.md` & `gypsum_client-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/LICENSE.txt` & `gypsum_client-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/PKG-INFO` & `gypsum_client-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gypsum-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client to gypsum REST API
 Home-page: https://github.com/ArtifactDB/gypsum-py
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/gypsum-py
 Platform: any
```

### Comparing `gypsum_client-0.1.1/README.md` & `gypsum_client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/docs/Makefile` & `gypsum_client-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/docs/conf.py` & `gypsum_client-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/docs/index.md` & `gypsum_client-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/docs/tutorial.md` & `gypsum_client-0.1.2/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/setup.cfg` & `gypsum_client-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/setup.py` & `gypsum_client-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/__init__.py` & `gypsum_client-0.1.2/src/gypsum_client/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
 
+from ._utils import BUCKET_CACHE_NAME
 from .auth import access_token, set_access_token
 from .cache_directory import cache_directory
 from .clone_operations import clone_version
 from .config import REQUESTS_MOD
 from .create_operations import create_project
 from .fetch_metadata_database import fetch_metadata_database
 from .fetch_metadata_schema import fetch_metadata_schema
@@ -40,7 +41,8 @@
 from .rest_url import rest_url
 from .s3_config import public_s3_config
 from .save_operations import save_file, save_version
 from .search_metadata import define_text_query, search_metadata_text
 from .set_operations import set_permissions, set_quota
 from .upload_api_operations import abort_upload, complete_upload, start_upload
 from .upload_file_actions import upload_directory, upload_files
+from .validate_metadata import validate_metadata
```

### Comparing `gypsum_client-0.1.1/src/gypsum_client/_github.py` & `gypsum_client-0.1.2/src/gypsum_client/_github.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/_utils.py` & `gypsum_client-0.1.2/src/gypsum_client/_utils.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/auth.py` & `gypsum_client-0.1.2/src/gypsum_client/auth.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/cache_directory.py` & `gypsum_client-0.1.2/src/gypsum_client/cache_directory.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/clone_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/clone_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/create_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/create_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/fetch_metadata_database.py` & `gypsum_client-0.1.2/src/gypsum_client/fetch_metadata_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 __copyright__ = "Jayaram Kancherla"
 __license__ = "MIT"
 
 LAST_CHECK = {"req_time": None, "mod_time": None}
 
 
 def fetch_metadata_database(
-    name: str = "bioconductor.sqlite3", cache_dir: str = None, overwrite: bool = False
+    name: str = "bioconductor.sqlite3",
+    cache_dir: str = cache_directory(),
+    overwrite: bool = False,
 ) -> str:
     """Fetch the SQLite database containing metadata from the gypsum backend.
 
     See `metadata index <https://github.com/ArtifactDB/bioconductor-metadata-index>`_
     for more details.
 
     Each database is generated by aggregating metadata across multiple assets
@@ -68,15 +70,15 @@
         Path to the downloaded database.
     """
     base_url = "https://github.com/ArtifactDB/bioconductor-metadata-index/releases/download/latest/"
 
     if cache_dir is None:
         cache_path = tempfile.NamedTemporaryFile(suffix=".sqlite3").name
     else:
-        cache_dir = os.path.join(cache_directory(cache_dir), "databases")
+        cache_dir = os.path.join(cache_dir, "databases")
 
         cache_path = os.path.join(cache_dir, name)
         if not os.path.exists(cache_path):
             os.makedirs(os.path.dirname(cache_path), exist_ok=True)
 
         if os.path.exists(cache_path) and not overwrite:
             old_lastmod_raw = None
```

### Comparing `gypsum_client-0.1.1/src/gypsum_client/fetch_metadata_schema.py` & `gypsum_client-0.1.2/src/gypsum_client/fetch_metadata_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 __author__ = "Jayaram Kancherla"
 __copyright__ = "Jayaram Kancherla"
 __license__ = "MIT"
 
 
 def fetch_metadata_schema(
     name: str = "bioconductor/v1.json",
-    cache_dir: str = None,
+    cache_dir: str = cache_directory(),
     overwrite: bool = False,
 ) -> str:
     """Fetch a JSON schema file for metadata to be inserted into a SQLite database.
 
     Fetch a JSON schema file for metadata to be inserted into a SQLite database
     See `metadata index <https://github.com/ArtifactDB/bioconductor-metadata-index>`_
     for more details.
@@ -54,15 +54,15 @@
     Returns:
         Path containing the downloaded schema.
     """
     cache_path = None
     if cache_dir is None:
         cache_path = tempfile.mktemp(suffix=".json")
     else:
-        cache_dir = os.path.join(cache_directory(cache_dir), "schemas")
+        cache_dir = os.path.join(cache_dir, "schemas")
 
         cache_path = os.path.join(cache_dir, name)
         if not os.path.exists(cache_path):
             os.makedirs(os.path.dirname(cache_path), exist_ok=True)
 
         if os.path.exists(cache_path) and not overwrite:
             _lock = FileLock(cache_path + ".LOCK")
```

### Comparing `gypsum_client-0.1.1/src/gypsum_client/fetch_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/fetch_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/list_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/list_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/prepare_directory_for_upload.py` & `gypsum_client-0.1.2/src/gypsum_client/prepare_directory_for_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,33 +117,32 @@
     cache_dir = _normalize_and_sanitize_path(cache_dir)
     if not cache_dir.endswith("/"):
         cache_dir += "/"
 
     for root, _, files in os.walk(directory):
         for name in files:
             rel_path = os.path.relpath(os.path.join(root, name), directory)
-            dest = (
-                os.readlink(os.path.join(directory, rel_path))
-                if os.path.islink(os.path.join(directory, rel_path))
-                else None
-            )
-            if not dest:
+
+            if not os.path.islink(os.path.join(directory, rel_path)):
                 out_files.append(rel_path)
                 continue
 
+            dest = os.readlink(os.path.join(directory, rel_path))
+
             if links == "never":
                 if not os.path.exists(dest):
                     raise ValueError(
                         f"Cannot use a dangling link to '{dest}' as a regular upload."
                     )
                 out_files.append(rel_path)
                 continue
 
             dest = _normalize_and_sanitize_path(dest)
             dest_components = _match_path_to_cache(dest, cache_dir)
+
             if dest_components:
                 out_links.append(
                     {
                         "from.path": rel_path,
                         "to.project": dest_components["project"],
                         "to.asset": dest_components["asset"],
                         "to.version": dest_components["version"],
@@ -156,14 +155,15 @@
                 raise ValueError(
                     f"Failed to convert symlink '{dest}' to an upload link."
                 )
             elif not os.path.exists(dest):
                 raise ValueError(
                     f"Cannot use a dangling link to '{dest}' as a regular upload."
                 )
+
             out_files.append(rel_path)
 
     return {"files": out_files, "links": out_links}
 
 
 def _normalize_and_sanitize_path(path: str) -> str:
     if os.path.exists(path):
```

### Comparing `gypsum_client-0.1.1/src/gypsum_client/probation_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/probation_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/refresh_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/refresh_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/remove_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/remove_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/resolve_links.py` & `gypsum_client-0.1.2/src/gypsum_client/resolve_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 __license__ = "MIT"
 
 
 def resolve_links(
     project: str,
     asset: str,
     version: str,
-    cache_dir: Optional[str] = None,
+    cache_dir: Optional[str] = cache_directory(),
     overwrite: str = False,
     url: str = rest_url(),
 ):
     """Resolve links in the cache directory.
 
     Create hard links (or copies, if filesystem links
     are not supported) for linked-from files to their
```

### Comparing `gypsum_client-0.1.1/src/gypsum_client/rest_url.py` & `gypsum_client-0.1.2/src/gypsum_client/rest_url.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/s3_config.py` & `gypsum_client-0.1.2/src/gypsum_client/s3_config.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/save_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/save_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     _save_file(path=path, destination=dest, overwrite=overwrite, url=url, verify=verify)
 
 
 def save_version(
     project: str,
     asset: str,
     version: str,
-    cache_dir: Optional[str] = None,
+    cache_dir: Optional[str] = cache_directory(),
     overwrite: bool = False,
     relink: bool = True,
     concurrent: int = 1,
     url: str = rest_url(),
 ) -> str:
     """Download all files associated with a version of an asset
     of a project from the gypsum bucket.
@@ -199,15 +199,15 @@
 
 
 def save_file(
     project: str,
     asset: str,
     version: str,
     path: str,
-    cache_dir: Optional[str] = None,
+    cache_dir: Optional[str] = cache_directory(),
     overwrite: bool = False,
     url: str = rest_url(),
 ):
     """Save a file from a version of a project asset.
 
     Download a file from the gypsum bucket, for a version of
     an asset of a project.
```

### Comparing `gypsum_client-0.1.1/src/gypsum_client/search_metadata.py` & `gypsum_client-0.1.2/src/gypsum_client/search_metadata.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/set_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/set_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/upload_api_operations.py` & `gypsum_client-0.1.2/src/gypsum_client/upload_api_operations.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/upload_file_actions.py` & `gypsum_client-0.1.2/src/gypsum_client/upload_file_actions.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client/validate_metadata.py` & `gypsum_client-0.1.2/src/gypsum_client/validate_metadata.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/src/gypsum_client.egg-info/PKG-INFO` & `gypsum_client-0.1.2/src/gypsum_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gypsum-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client to gypsum REST API
 Home-page: https://github.com/ArtifactDB/gypsum-py
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/gypsum-py
 Platform: any
```

### Comparing `gypsum_client-0.1.1/src/gypsum_client.egg-info/SOURCES.txt` & `gypsum_client-0.1.2/src/gypsum_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_auth.py` & `gypsum_client-0.1.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_clone.py` & `gypsum_client-0.1.2/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_fetch.py` & `gypsum_client-0.1.2/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_fetch_metadata_database.py` & `gypsum_client-0.1.2/tests/test_fetch_metadata_database.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_fetch_metadata_schema.py` & `gypsum_client-0.1.2/tests/test_fetch_metadata_schema.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_latest.py` & `gypsum_client-0.1.2/tests/test_latest.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_list.py` & `gypsum_client-0.1.2/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_permissions.py` & `gypsum_client-0.1.2/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_prepare_dir_upload.py` & `gypsum_client-0.1.2/tests/test_prepare_dir_upload.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_probation.py` & `gypsum_client-0.1.2/tests/test_probation.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_quota.py` & `gypsum_client-0.1.2/tests/test_quota.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_remove.py` & `gypsum_client-0.1.2/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_save.py` & `gypsum_client-0.1.2/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_search.py` & `gypsum_client-0.1.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tests/test_upload.py` & `gypsum_client-0.1.2/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `gypsum_client-0.1.1/tox.ini` & `gypsum_client-0.1.2/tox.ini`

 * *Files identical despite different names*

