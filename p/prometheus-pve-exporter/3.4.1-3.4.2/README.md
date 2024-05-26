# Comparing `tmp/prometheus_pve_exporter-3.4.1.tar.gz` & `tmp/prometheus_pve_exporter-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_pve_exporter-3.4.1.tar", last modified: Mon May  6 19:58:59 2024, max compression
+gzip compressed data, was "prometheus_pve_exporter-3.4.2.tar", last modified: Sun May 26 17:33:55 2024, max compression
```

## Comparing `prometheus_pve_exporter-3.4.1.tar` & `prometheus_pve_exporter-3.4.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:59.370935 prometheus_pve_exporter-3.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:59.366935 prometheus_pve_exporter-3.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:59.366935 prometheus_pve_exporter-3.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/.github/workflows/container-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/.github/workflows/container-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-05-06 19:58:59.370935 prometheus_pve_exporter-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/pve.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/pylintrc.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:58:59.370935 prometheus_pve_exporter-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:59.362935 prometheus_pve_exporter-3.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:59.370935 prometheus_pve_exporter-3.4.1/src/prometheus_pve_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-05-06 19:58:59.000000 prometheus_pve_exporter-3.4.1/src/prometheus_pve_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-06 19:58:59.000000 prometheus_pve_exporter-3.4.1/src/prometheus_pve_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:58:59.000000 prometheus_pve_exporter-3.4.1/src/prometheus_pve_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 19:58:59.000000 prometheus_pve_exporter-3.4.1/src/prometheus_pve_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 19:58:59.000000 prometheus_pve_exporter-3.4.1/src/prometheus_pve_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 19:58:59.000000 prometheus_pve_exporter-3.4.1/src/prometheus_pve_exporter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:59.370935 prometheus_pve_exporter-3.4.1/src/pve_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/src/pve_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/src/pve_exporter/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4115 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/src/pve_exporter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:59.370935 prometheus_pve_exporter-3.4.1/src/pve_exporter/collector/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/src/pve_exporter/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/src/pve_exporter/collector/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/src/pve_exporter/collector/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/src/pve_exporter/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-06 19:58:54.000000 prometheus_pve_exporter-3.4.1/src/pve_exporter/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:33:55.410620 prometheus_pve_exporter-3.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:33:55.410620 prometheus_pve_exporter-3.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:33:55.410620 prometheus_pve_exporter-3.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/.github/workflows/container-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/.github/workflows/container-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-05-26 17:33:55.410620 prometheus_pve_exporter-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/pve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/pylintrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30041 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 17:33:55.410620 prometheus_pve_exporter-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:33:55.406620 prometheus_pve_exporter-3.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:33:55.410620 prometheus_pve_exporter-3.4.2/src/prometheus_pve_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-05-26 17:33:55.000000 prometheus_pve_exporter-3.4.2/src/prometheus_pve_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-26 17:33:55.000000 prometheus_pve_exporter-3.4.2/src/prometheus_pve_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 17:33:55.000000 prometheus_pve_exporter-3.4.2/src/prometheus_pve_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-26 17:33:55.000000 prometheus_pve_exporter-3.4.2/src/prometheus_pve_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-26 17:33:55.000000 prometheus_pve_exporter-3.4.2/src/prometheus_pve_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 17:33:55.000000 prometheus_pve_exporter-3.4.2/src/prometheus_pve_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:33:55.410620 prometheus_pve_exporter-3.4.2/src/pve_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/src/pve_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/src/pve_exporter/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4115 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/src/pve_exporter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:33:55.410620 prometheus_pve_exporter-3.4.2/src/pve_exporter/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/src/pve_exporter/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/src/pve_exporter/collector/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/src/pve_exporter/collector/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/src/pve_exporter/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-26 17:33:46.000000 prometheus_pve_exporter-3.4.2/src/pve_exporter/http.py
```

### Comparing `prometheus_pve_exporter-3.4.1/.github/workflows/ci.yml` & `prometheus_pve_exporter-3.4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/.github/workflows/container-image.yml` & `prometheus_pve_exporter-3.4.2/.github/workflows/container-image.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/.github/workflows/container-test.yml` & `prometheus_pve_exporter-3.4.2/.github/workflows/container-test.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/.github/workflows/pypi.yml` & `prometheus_pve_exporter-3.4.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/CHANGELOG.rst` & `prometheus_pve_exporter-3.4.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 The format is based on `Keep a Changelog`_ and this project adheres to
 `Semantic Versioning`_.
 
 `Unreleased`_
 -------------
 
 
+`3.4.2`_ - 2024-05-26
+---------------------
+
+Changed
+~~~~~~~
+
+- Bump requests from 2.31.0 to 2.32.0 (#251)
+
+
 `3.4.1`_ - 2024-05-06
 ---------------------
 
 Changed
 ~~~~~~~
 
 - Bump werkzeug from 3.0.2 to 3.0.3 (#249)
@@ -412,15 +421,16 @@
 ~~~~~
 
 -  IPv6 support
 
 
 .. _Keep a Changelog: http://keepachangelog.com/en/1.0.0/
 .. _Semantic Versioning: http://semver.org/spec/v2.0.0.html
-.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.4.1...HEAD
+.. _Unreleased: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.4.2...HEAD
+.. _3.4.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.4.1...v3.4.2
 .. _3.4.1: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.4.0...v3.4.1
 .. _3.4.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.3.0...v3.4.0
 .. _3.3.0: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.5...v3.3.0
 .. _3.2.5: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.4...v3.2.5
 .. _3.2.4: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.3...v3.2.4
 .. _3.2.3: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.2...v3.2.3
 .. _3.2.2: https://github.com/prometheus-pve/prometheus-pve-exporter/compare/v3.2.1...v3.2.2
```

### Comparing `prometheus_pve_exporter-3.4.1/Dockerfile` & `prometheus_pve_exporter-3.4.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/LICENSE` & `prometheus_pve_exporter-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/PKG-INFO` & `prometheus_pve_exporter-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.4.1
+Version: 3.4.2
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `prometheus_pve_exporter-3.4.1/README.rst` & `prometheus_pve_exporter-3.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/pylintrc.toml` & `prometheus_pve_exporter-3.4.2/pylintrc.toml`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/pyproject.toml` & `prometheus_pve_exporter-3.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prometheus-pve-exporter"
-version = "3.4.1"
+version = "3.4.2"
 authors = [{ name = "Lorenz Schori", email = "lo@znerol.ch" }]
 description = "Proxmox VE exporter for the Prometheus monitoring system."
 requires-python = ">=3.9"
 keywords = ["prometheus", "exporter", "network", "monitoring", "proxmox"]
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `prometheus_pve_exporter-3.4.1/requirements.txt` & `prometheus_pve_exporter-3.4.2/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -369,17 +369,17 @@
     --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
     --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
     --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
     --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
     --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
     --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
     # via -r requirements.in
-requests==2.31.0 \
-    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
-    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
+requests==2.32.0 \
+    --hash=sha256:f2c3881dddb70d056c5bd7600a4fae312b2a300e39be6a118d30b90bd27262b5 \
+    --hash=sha256:fa5490319474c82ef1d2c9bc459d3652e3ae4ef4c4ebdd18a21145a47ca4b6b8
     # via -r requirements.in
 urllib3==2.1.0 \
     --hash=sha256:55901e917a5896a349ff771be919f8bd99aff50b79fe58fec595eb37bbc56bb3 \
     --hash=sha256:df7aa8afb0148fa78488e7899b2c59b5f4ffcfa82e6c54ccb9dd37c1d7b52d54
     # via requests
 werkzeug==3.0.3 \
     --hash=sha256:097e5bfda9f0aba8da6b8545146def481d06aa7d3266e7448e2cccf67dd8bd18 \
```

### Comparing `prometheus_pve_exporter-3.4.1/src/prometheus_pve_exporter.egg-info/PKG-INFO` & `prometheus_pve_exporter-3.4.2/src/prometheus_pve_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-exporter
-Version: 3.4.1
+Version: 3.4.2
 Summary: Proxmox VE exporter for the Prometheus monitoring system.
 Author-email: Lorenz Schori <lo@znerol.ch>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/prometheus-pve/prometheus-pve-exporter
 Keywords: prometheus,exporter,network,monitoring,proxmox
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

### Comparing `prometheus_pve_exporter-3.4.1/src/prometheus_pve_exporter.egg-info/SOURCES.txt` & `prometheus_pve_exporter-3.4.2/src/prometheus_pve_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/src/pve_exporter/cli.py` & `prometheus_pve_exporter-3.4.2/src/pve_exporter/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/src/pve_exporter/collector/__init__.py` & `prometheus_pve_exporter-3.4.2/src/pve_exporter/collector/__init__.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/src/pve_exporter/collector/cluster.py` & `prometheus_pve_exporter-3.4.2/src/pve_exporter/collector/cluster.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/src/pve_exporter/collector/node.py` & `prometheus_pve_exporter-3.4.2/src/pve_exporter/collector/node.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/src/pve_exporter/config.py` & `prometheus_pve_exporter-3.4.2/src/pve_exporter/config.py`

 * *Files identical despite different names*

### Comparing `prometheus_pve_exporter-3.4.1/src/pve_exporter/http.py` & `prometheus_pve_exporter-3.4.2/src/pve_exporter/http.py`

 * *Files identical despite different names*

