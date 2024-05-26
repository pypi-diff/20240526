# Comparing `tmp/python_re3data-0.2.0.tar.gz` & `tmp/python_re3data-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu May 23 16:47:19 2024, max compression
+gzip compressed data, last modified: Sun May 26 17:18:13 2024, max compression
```

## Comparing `python_re3data-0.2.0.tar` & `python_re3data-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      113 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/__about__.py
--rw-r--r--   0        0        0      295 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/__init__.py
--rw-r--r--   0        0        0      185 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/__main__.py
--rw-r--r--   0        0        0     1084 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/_cli.py
--rw-r--r--   0        0        0     4992 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/_client.py
--rw-r--r--   0        0        0        0 2024-05-23 16:47:19.000000 python_re3data-0.2.0/src/re3data/py.typed
--rw-r--r--   0        0        0     1160 2024-05-23 16:47:19.000000 python_re3data-0.2.0/.gitignore
--rw-r--r--   0        0        0     1082 2024-05-23 16:47:19.000000 python_re3data-0.2.0/LICENSE
--rw-r--r--   0        0        0     7529 2024-05-23 16:47:19.000000 python_re3data-0.2.0/README.md
--rw-r--r--   0        0        0     7008 2024-05-23 16:47:19.000000 python_re3data-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9555 2024-05-23 16:47:19.000000 python_re3data-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/__about__.py
+-rw-r--r--   0        0        0      295 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/__init__.py
+-rw-r--r--   0        0        0      185 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/__main__.py
+-rw-r--r--   0        0        0     1639 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/_cli.py
+-rw-r--r--   0        0        0     4992 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/_client.py
+-rw-r--r--   0        0        0        0 2024-05-26 17:18:13.000000 python_re3data-0.3.0/src/re3data/py.typed
+-rw-r--r--   0        0        0     1160 2024-05-26 17:18:13.000000 python_re3data-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1082 2024-05-26 17:18:13.000000 python_re3data-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7650 2024-05-26 17:18:13.000000 python_re3data-0.3.0/README.md
+-rw-r--r--   0        0        0     7039 2024-05-26 17:18:13.000000 python_re3data-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9734 2024-05-26 17:18:13.000000 python_re3data-0.3.0/PKG-INFO
```

### Comparing `python_re3data-0.2.0/src/re3data/_client.py` & `python_re3data-0.3.0/src/re3data/_client.py`

 * *Files identical despite different names*

### Comparing `python_re3data-0.2.0/.gitignore` & `python_re3data-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python_re3data-0.2.0/LICENSE` & `python_re3data-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_re3data-0.2.0/README.md` & `python_re3data-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 > exercise caution when using this project in production environments. Contributions and feedback are welcome to help
 > move the project towards a more stable release (v1.0.0).
 
 | __CI__      | [![pre-commit.ci status][pre-commit-ci-badge]][pre-commit-ci-status] [![ci][ci-badge]][ci-workflow] [![coverage][coverage-badge]][ci-workflow] [![codeql][codeql-badge]][codeql-workflow]                                                                                      |
 | :---------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | __Docs__    | [![docs][docs-badge]][docs-workflow]                                                                                                                                                                                                                                           |
 | __Package__ | [![pypi-status][status-badge]][pypi-url] [![pypi-version][pypi-version-badge]][pypi-url] [![pypi-python-versions][pypi-python-versions-badge]][pypi-url] [![all-downloads][all-downloads-badge]][pepy-tech-url] [![monthly-downloads][monthly-downloads-badge]][pepy-tech-url] |
-| __Meta__    | [![OpenSSF Scorecard][scorecard-badge]][scorecard-url] [![hatch][hatch-badge]][hatch] [![ruff][ruff-badge]][ruff] [![mypy][mypy-badge]][mypy] [![License][license-badge]][license-url]                                                                                         |
+| __Meta__    | [![doi][doi-badge]][doi-url] [![OpenSSF Scorecard][scorecard-badge]][scorecard-url] [![hatch][hatch-badge]][hatch] [![ruff][ruff-badge]][ruff] [![mypy][mypy-badge]][mypy] [![License][license-badge]][license-url]                                                            |
 
 `python-re3data` is a Python library that simplifies interacting with the [re3data](https://www.re3data.org) (Registry
 of Research Data Repositories) [REST API](https://www.re3data.org/api/doc), allowing you to easily retrieve and process
 metadata about research data repositories in a convenient and Pythonic way.
 
 ```pycon
 >>> import re3data
@@ -94,14 +94,16 @@
 [ci-workflow]: https://github.com/afuetterer/python-re3data/actions/workflows/main.yml
 [codeql-badge]: https://github.com/afuetterer/python-re3data/actions/workflows/codeql.yml/badge.svg
 [codeql-workflow]: https://github.com/afuetterer/python-re3data/actions/workflows/codeql.yml
 [coverage-badge]: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/afuetterer/adc66df152c473c1aa136557ee8181ca/raw/coverage-badge.json
 [docs-badge]: https://github.com/afuetterer/python-re3data/actions/workflows/docs.yml/badge.svg
 [docs-url]: https://afuetterer.github.io/python-re3data
 [docs-workflow]: https://github.com/afuetterer/python-re3data/actions/workflows/docs.yml
+[doi-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.11264510.svg
+[doi-url]: https://doi.org/10.5281/zenodo.11264510
 [hatch]: https://github.com/pypa/hatch
 [hatch-badge]: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
 [license-badge]: https://img.shields.io/badge/license-MIT-blue.svg
 [license-url]: https://spdx.org/licenses/MIT.html
 [monthly-downloads-badge]: https://static.pepy.tech/badge/python-re3data/month
 [mypy]: https://mypy-lang.org
 [mypy-badge]: https://img.shields.io/badge/types-mypy-blue.svg
```

### Comparing `python_re3data-0.2.0/pyproject.toml` & `python_re3data-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
   "python-re3data[cli]",
 ]
 optional-dependencies.docs = [
   "mike~=2.1",
   "mkdocs~=1.6",
   "mkdocs-include-markdown-plugin~=6.0",
   "mkdocs-material~=9.5",
+  "mkdocs-minify-plugin~=0.7",
   "mkdocstrings[python]~=0.25",
 ]
 optional-dependencies.test = [
   "pytest~=8.2",
   "pytest-cov~=5.0",
   "pytest-mock~=3.14",
   "pytest-randomly~=3.15",
```

### Comparing `python_re3data-0.2.0/PKG-INFO` & `python_re3data-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python-re3data
-Version: 0.2.0
+Version: 0.3.0
 Summary: The Pythonic client for the re3data API.
 Project-URL: Changelog, https://github.com/afuetterer/python-re3data/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://afuetterer.github.io/python-re3data
 Project-URL: Issues, https://github.com/afuetterer/python-re3data/issues
 Project-URL: Repository, https://github.com/afuetterer/python-re3data.git
 Author: Heinz-Alexander Fütterer
 License: MIT
@@ -28,14 +28,15 @@
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.7; extra == 'dev'
 Requires-Dist: typer>=0.12; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mike~=2.1; extra == 'docs'
 Requires-Dist: mkdocs-include-markdown-plugin~=6.0; extra == 'docs'
 Requires-Dist: mkdocs-material~=9.5; extra == 'docs'
+Requires-Dist: mkdocs-minify-plugin~=0.7; extra == 'docs'
 Requires-Dist: mkdocstrings[python]~=0.25; extra == 'docs'
 Requires-Dist: mkdocs~=1.6; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest-cov~=5.0; extra == 'test'
 Requires-Dist: pytest-mock~=3.14; extra == 'test'
 Requires-Dist: pytest-randomly~=3.15; extra == 'test'
 Requires-Dist: pytest-recording~=0.13; extra == 'test'
@@ -51,15 +52,15 @@
 > exercise caution when using this project in production environments. Contributions and feedback are welcome to help
 > move the project towards a more stable release (v1.0.0).
 
 | __CI__      | [![pre-commit.ci status][pre-commit-ci-badge]][pre-commit-ci-status] [![ci][ci-badge]][ci-workflow] [![coverage][coverage-badge]][ci-workflow] [![codeql][codeql-badge]][codeql-workflow]                                                                                      |
 | :---------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | __Docs__    | [![docs][docs-badge]][docs-workflow]                                                                                                                                                                                                                                           |
 | __Package__ | [![pypi-status][status-badge]][pypi-url] [![pypi-version][pypi-version-badge]][pypi-url] [![pypi-python-versions][pypi-python-versions-badge]][pypi-url] [![all-downloads][all-downloads-badge]][pepy-tech-url] [![monthly-downloads][monthly-downloads-badge]][pepy-tech-url] |
-| __Meta__    | [![OpenSSF Scorecard][scorecard-badge]][scorecard-url] [![hatch][hatch-badge]][hatch] [![ruff][ruff-badge]][ruff] [![mypy][mypy-badge]][mypy] [![License][license-badge]][license-url]                                                                                         |
+| __Meta__    | [![doi][doi-badge]][doi-url] [![OpenSSF Scorecard][scorecard-badge]][scorecard-url] [![hatch][hatch-badge]][hatch] [![ruff][ruff-badge]][ruff] [![mypy][mypy-badge]][mypy] [![License][license-badge]][license-url]                                                            |
 
 `python-re3data` is a Python library that simplifies interacting with the [re3data](https://www.re3data.org) (Registry
 of Research Data Repositories) [REST API](https://www.re3data.org/api/doc), allowing you to easily retrieve and process
 metadata about research data repositories in a convenient and Pythonic way.
 
 ```pycon
 >>> import re3data
@@ -140,14 +141,16 @@
 [ci-workflow]: https://github.com/afuetterer/python-re3data/actions/workflows/main.yml
 [codeql-badge]: https://github.com/afuetterer/python-re3data/actions/workflows/codeql.yml/badge.svg
 [codeql-workflow]: https://github.com/afuetterer/python-re3data/actions/workflows/codeql.yml
 [coverage-badge]: https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/afuetterer/adc66df152c473c1aa136557ee8181ca/raw/coverage-badge.json
 [docs-badge]: https://github.com/afuetterer/python-re3data/actions/workflows/docs.yml/badge.svg
 [docs-url]: https://afuetterer.github.io/python-re3data
 [docs-workflow]: https://github.com/afuetterer/python-re3data/actions/workflows/docs.yml
+[doi-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.11264510.svg
+[doi-url]: https://doi.org/10.5281/zenodo.11264510
 [hatch]: https://github.com/pypa/hatch
 [hatch-badge]: https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg
 [license-badge]: https://img.shields.io/badge/license-MIT-blue.svg
 [license-url]: https://spdx.org/licenses/MIT.html
 [monthly-downloads-badge]: https://static.pepy.tech/badge/python-re3data/month
 [mypy]: https://mypy-lang.org
 [mypy-badge]: https://img.shields.io/badge/types-mypy-blue.svg
```

