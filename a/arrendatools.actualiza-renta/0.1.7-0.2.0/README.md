# Comparing `tmp/arrendatools.actualiza_renta-0.1.7.tar.gz` & `tmp/arrendatools_actualiza_renta-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools.actualiza_renta-0.1.7.tar", last modified: Mon Mar 25 09:33:47 2024, max compression
+gzip compressed data, was "arrendatools_actualiza_renta-0.2.0.tar", last modified: Sun May 26 08:35:06 2024, max compression
```

## Comparing `arrendatools.actualiza_renta-0.1.7.tar` & `arrendatools_actualiza_renta-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 09:33:47.652123 arrendatools.actualiza_renta-0.1.7/
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 09:33:47.648123 arrendatools.actualiza_renta-0.1.7/.github/
--rw-r--r--   0 root         (0) root         (0)      397 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/.github/dependabot.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 09:33:47.648123 arrendatools.actualiza_renta-0.1.7/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1951 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/.github/workflows/main.yml
--rw-r--r--   0 root         (0) root         (0)      868 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/.github/workflows/test.yml
--rw-r--r--   0 root         (0) root         (0)     2774 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 09:33:47.648123 arrendatools.actualiza_renta-0.1.7/.vscode/
--rw-r--r--   0 root         (0) root         (0)      291 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/.vscode/settings.json
--rw-r--r--   0 root         (0) root         (0)    21641 2024-03-25 09:33:41.000000 arrendatools.actualiza_renta-0.1.7/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1062 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4961 2024-03-25 09:33:47.652123 arrendatools.actualiza_renta-0.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4160 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 09:33:47.648123 arrendatools.actualiza_renta-0.1.7/arrendatools/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-25 09:33:41.000000 arrendatools.actualiza_renta-0.1.7/arrendatools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 09:33:47.652123 arrendatools.actualiza_renta-0.1.7/arrendatools/actualiza_renta/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/arrendatools/actualiza_renta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/arrendatools/actualiza_renta/ine.py
--rw-r--r--   0 root         (0) root         (0)    11560 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/arrendatools/actualiza_renta/ipc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 09:33:47.652123 arrendatools.actualiza_renta-0.1.7/arrendatools.actualiza_renta.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4961 2024-03-25 09:33:47.000000 arrendatools.actualiza_renta-0.1.7/arrendatools.actualiza_renta.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      627 2024-03-25 09:33:47.000000 arrendatools.actualiza_renta-0.1.7/arrendatools.actualiza_renta.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 09:33:47.000000 arrendatools.actualiza_renta-0.1.7/arrendatools.actualiza_renta.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-25 09:33:47.000000 arrendatools.actualiza_renta-0.1.7/arrendatools.actualiza_renta.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-25 09:33:47.000000 arrendatools.actualiza_renta-0.1.7/arrendatools.actualiza_renta.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1466 2024-03-25 09:33:41.000000 arrendatools.actualiza_renta-0.1.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 09:33:47.652123 arrendatools.actualiza_renta-0.1.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 09:33:47.652123 arrendatools.actualiza_renta-0.1.7/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3327 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/test/test_ipc.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-25 09:33:40.000000 arrendatools.actualiza_renta-0.1.7/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 08:35:06.277660 arrendatools_actualiza_renta-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/.gitattributes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 08:35:06.273659 arrendatools_actualiza_renta-0.2.0/.github/
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/.github/dependabot.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 08:35:06.273659 arrendatools_actualiza_renta-0.2.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1944 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0 root         (0) root         (0)      861 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 root         (0) root         (0)     2774 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 08:35:06.273659 arrendatools_actualiza_renta-0.2.0/.vscode/
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/.vscode/settings.json
+-rw-r--r--   0 root         (0) root         (0)    28088 2024-05-26 08:34:59.000000 arrendatools_actualiza_renta-0.2.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4911 2024-05-26 08:35:06.277660 arrendatools_actualiza_renta-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4160 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 08:35:06.273659 arrendatools_actualiza_renta-0.2.0/arrendatools/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-26 08:34:59.000000 arrendatools_actualiza_renta-0.2.0/arrendatools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 08:35:06.277660 arrendatools_actualiza_renta-0.2.0/arrendatools/actualiza_renta/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/arrendatools/actualiza_renta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/arrendatools/actualiza_renta/ine.py
+-rw-r--r--   0 root         (0) root         (0)    11560 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/arrendatools/actualiza_renta/ipc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 08:35:06.277660 arrendatools_actualiza_renta-0.2.0/arrendatools.actualiza_renta.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4911 2024-05-26 08:35:06.000000 arrendatools_actualiza_renta-0.2.0/arrendatools.actualiza_renta.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      627 2024-05-26 08:35:06.000000 arrendatools_actualiza_renta-0.2.0/arrendatools.actualiza_renta.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 08:35:06.000000 arrendatools_actualiza_renta-0.2.0/arrendatools.actualiza_renta.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-26 08:35:06.000000 arrendatools_actualiza_renta-0.2.0/arrendatools.actualiza_renta.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-26 08:35:06.000000 arrendatools_actualiza_renta-0.2.0/arrendatools.actualiza_renta.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-05-26 08:34:59.000000 arrendatools_actualiza_renta-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-26 08:35:06.277660 arrendatools_actualiza_renta-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 08:35:06.277660 arrendatools_actualiza_renta-0.2.0/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3327 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/test/test_ipc.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-26 08:34:58.000000 arrendatools_actualiza_renta-0.2.0/tox.ini
```

### Comparing `arrendatools.actualiza_renta-0.1.7/.github/workflows/main.yml` & `arrendatools_actualiza_renta-0.2.0/.github/workflows/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       - master
 jobs:
   test:
     name: Python ${{ matrix.python-version }} tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: Checkout code
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
@@ -40,15 +40,15 @@
       id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing in PyPi
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Python Semantic Release
       id: release
-      uses: python-semantic-release/python-semantic-release@v9.3.1
+      uses: python-semantic-release/python-semantic-release@v9.7.3
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
     - name: Publish package distributions to PyPI
       id: pypi-publish
       uses: pypa/gh-action-pypi-publish@release/v1
       # NOTE: DO NOT wrap the conditional in ${{ }} as it will always evaluate to true.
       # See https://github.com/actions/runner/issues/1173
```

### Comparing `arrendatools.actualiza_renta-0.1.7/.github/workflows/test.yml` & `arrendatools_actualiza_renta-0.2.0/.github/workflows/test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
   pull_request:
 jobs:
   test:
     name: Python ${{ matrix.python-version }} tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: Checkout code
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
```

### Comparing `arrendatools.actualiza_renta-0.1.7/.gitignore` & `arrendatools_actualiza_renta-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `arrendatools.actualiza_renta-0.1.7/CHANGELOG.md` & `arrendatools_actualiza_renta-0.2.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,126 @@
 # CHANGELOG
 
 
 
+## v0.2.0 (2024-05-26)
+
+### Build
+
+* build(deps): bump python-semantic-release/python-semantic-release
+
+Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 9.7.1 to 9.7.3.
+- [Release notes](https://github.com/python-semantic-release/python-semantic-release/releases)
+- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/python-semantic-release/python-semantic-release/compare/v9.7.1...v9.7.3)
+
+---
+updated-dependencies:
+- dependency-name: python-semantic-release/python-semantic-release
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`0907086`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/09070869a8185cd7681ce2d8221f390ce9556704))
+
+* build(deps): bump python-semantic-release/python-semantic-release
+
+Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 9.5.0 to 9.7.1.
+- [Release notes](https://github.com/python-semantic-release/python-semantic-release/releases)
+- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/python-semantic-release/python-semantic-release/compare/v9.5.0...v9.7.1)
+
+---
+updated-dependencies:
+- dependency-name: python-semantic-release/python-semantic-release
+  dependency-type: direct:production
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`936e2d0`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/936e2d01c3188b03f962394cfd949b6241f076e6))
+
+* build(deps): bump python-semantic-release/python-semantic-release
+
+Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 9.4.1 to 9.5.0.
+- [Release notes](https://github.com/python-semantic-release/python-semantic-release/releases)
+- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/python-semantic-release/python-semantic-release/compare/v9.4.1...v9.5.0)
+
+---
+updated-dependencies:
+- dependency-name: python-semantic-release/python-semantic-release
+  dependency-type: direct:production
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`e96dde3`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/e96dde3926029a544584993d7ca8618ee9e8e13b))
+
+* build(deps): bump python-semantic-release/python-semantic-release
+
+Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 9.4.0 to 9.4.1.
+- [Release notes](https://github.com/python-semantic-release/python-semantic-release/releases)
+- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/python-semantic-release/python-semantic-release/compare/v9.4.0...v9.4.1)
+
+---
+updated-dependencies:
+- dependency-name: python-semantic-release/python-semantic-release
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`d693c3c`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/d693c3c7ca3ac80678ed762b7b990ef0fe9bbb5e))
+
+* build(deps): bump python-semantic-release/python-semantic-release
+
+Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 9.3.1 to 9.4.0.
+- [Release notes](https://github.com/python-semantic-release/python-semantic-release/releases)
+- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/python-semantic-release/python-semantic-release/compare/v9.3.1...v9.4.0)
+
+---
+updated-dependencies:
+- dependency-name: python-semantic-release/python-semantic-release
+  dependency-type: direct:production
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`e48e4cc`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/e48e4ccbf65f00298ea4b51f1dd8df0144c873c6))
+
+### Feature
+
+* feat(python-version): minimum python version is now 3.8 ([`90dda34`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/90dda347fe89a1734dc4f47e652558a5f2465023))
+
+### Unknown
+
+* Merge pull request #41 from hokus15/devel
+
+feat(python-version): minimum python version is now 3.8 ([`d5b02f6`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/d5b02f67ebcc4cc550522109d5962098ba24eb26))
+
+* Merge pull request #38 from hokus15/dependabot/github_actions/python-semantic-release/python-semantic-release-9.7.3
+
+build(deps): bump python-semantic-release/python-semantic-release from 9.7.1 to 9.7.3 ([`e534c77`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/e534c779b7342e85e720a42640b1234276b43d21))
+
+* Merge pull request #36 from hokus15/dependabot/github_actions/python-semantic-release/python-semantic-release-9.7.1
+
+build(deps): bump python-semantic-release/python-semantic-release from 9.5.0 to 9.7.1 ([`b03e0b4`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/b03e0b4b841e8cd0319b6b7f8e1e41536cdd8129))
+
+* Merge pull request #33 from hokus15/dependabot/github_actions/python-semantic-release/python-semantic-release-9.5.0
+
+build(deps): bump python-semantic-release/python-semantic-release from 9.4.1 to 9.5.0 ([`9c2281c`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/9c2281cd81464479f0d5a13fe04890eb90d95d9c))
+
+* Merge pull request #31 from hokus15/dependabot/github_actions/python-semantic-release/python-semantic-release-9.4.1
+
+build(deps): bump python-semantic-release/python-semantic-release from 9.4.0 to 9.4.1 ([`44b0d5b`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/44b0d5b89a30b7ce391a340343e0411ceee9ada7))
+
+* Merge pull request #30 from hokus15/dependabot/github_actions/python-semantic-release/python-semantic-release-9.4.0
+
+build(deps): bump python-semantic-release/python-semantic-release from 9.3.1 to 9.4.0 ([`a172045`](https://github.com/hokus15/ArrendaToolsActualizaRenta/commit/a172045e2ee19131754fae296d46ce50532df55b))
+
+
 ## v0.1.7 (2024-03-25)
 
 ### Build
 
 * build(deps): bump python-semantic-release/python-semantic-release
 
 Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 9.3.0 to 9.3.1.
```

### Comparing `arrendatools.actualiza_renta-0.1.7/LICENSE` & `arrendatools_actualiza_renta-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools.actualiza_renta-0.1.7/PKG-INFO` & `arrendatools_actualiza_renta-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: arrendatools.actualiza_renta
-Version: 0.1.7
+Version: 0.2.0
 Summary: Módulo de Python que realiza la actualización de rentas de alquiler por anualidades completas con el IPC (LAU) descrita en la web del INE de España.
 Author-email: Jordi Morell <hokus@hotmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 
 # ArrendaTools Actualiza Renta
 ![License](https://img.shields.io/github/license/hokus15/ArrendaToolsActualizaRenta)
 [![Build Status](https://github.com/hokus15/ArrendaToolsActualizaRenta/actions/workflows/main.yml/badge.svg)](https://github.com/hokus15/ArrendaToolsActualizaRenta/actions)
```

### Comparing `arrendatools.actualiza_renta-0.1.7/README.md` & `arrendatools_actualiza_renta-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `arrendatools.actualiza_renta-0.1.7/arrendatools/actualiza_renta/ine.py` & `arrendatools_actualiza_renta-0.2.0/arrendatools/actualiza_renta/ine.py`

 * *Files identical despite different names*

### Comparing `arrendatools.actualiza_renta-0.1.7/arrendatools/actualiza_renta/ipc.py` & `arrendatools_actualiza_renta-0.2.0/arrendatools/actualiza_renta/ipc.py`

 * *Files identical despite different names*

### Comparing `arrendatools.actualiza_renta-0.1.7/arrendatools.actualiza_renta.egg-info/PKG-INFO` & `arrendatools_actualiza_renta-0.2.0/arrendatools.actualiza_renta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: arrendatools.actualiza_renta
-Version: 0.1.7
+Version: 0.2.0
 Summary: Módulo de Python que realiza la actualización de rentas de alquiler por anualidades completas con el IPC (LAU) descrita en la web del INE de España.
 Author-email: Jordi Morell <hokus@hotmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 
 # ArrendaTools Actualiza Renta
 ![License](https://img.shields.io/github/license/hokus15/ArrendaToolsActualizaRenta)
 [![Build Status](https://github.com/hokus15/ArrendaToolsActualizaRenta/actions/workflows/main.yml/badge.svg)](https://github.com/hokus15/ArrendaToolsActualizaRenta/actions)
```

### Comparing `arrendatools.actualiza_renta-0.1.7/arrendatools.actualiza_renta.egg-info/SOURCES.txt` & `arrendatools_actualiza_renta-0.2.0/arrendatools.actualiza_renta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arrendatools.actualiza_renta-0.1.7/pyproject.toml` & `arrendatools_actualiza_renta-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arrendatools.actualiza_renta"
-version = "0.1.7"
+version = "0.2.0"
 authors = [
     {name = "Jordi Morell", email = "hokus@hotmail.com"},
 ]
 description = "Módulo de Python que realiza la actualización de rentas de alquiler por anualidades completas con el IPC (LAU) descrita en la web del INE de España."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "requests==2.31.0",
```

### Comparing `arrendatools.actualiza_renta-0.1.7/test/test_ipc.py` & `arrendatools_actualiza_renta-0.2.0/test/test_ipc.py`

 * *Files identical despite different names*

