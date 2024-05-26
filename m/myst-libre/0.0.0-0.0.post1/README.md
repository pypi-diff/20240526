# Comparing `tmp/myst_libre-0.0.0.tar.gz` & `tmp/myst_libre-0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myst_libre-0.0.0.tar", last modified: Sun May 26 14:08:22 2024, max compression
+gzip compressed data, was "myst_libre-0.0.post1.tar", last modified: Sun May 26 14:47:23 2024, max compression
```

## Comparing `myst_libre-0.0.0.tar` & `myst_libre-0.0.post1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:22.908753 myst_libre-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:22.904753 myst_libre-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:22.904753 myst_libre-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-26 14:08:04.000000 myst_libre-0.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-26 14:08:04.000000 myst_libre-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-26 14:08:22.908753 myst_libre-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-26 14:08:04.000000 myst_libre-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 14:08:04.000000 myst_libre-0.0.0/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:22.904753 myst_libre-0.0.0/myst_libre/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/abstract_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:22.908753 myst_libre-0.0.0/myst_libre/builders/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/builders/myst_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:22.908753 myst_libre-0.0.0/myst_libre/rees/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/rees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/rees/rees.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:22.908753 myst_libre-0.0.0/myst_libre/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/test/test_myst_libre.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:22.908753 myst_libre-0.0.0/myst_libre/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/tools/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/tools/build_source_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/tools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/tools/docker_registry_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/tools/jupyter_hub_local_spawner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/tools/myst_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-26 14:08:04.000000 myst_libre-0.0.0/myst_libre/tools/rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:08:22.908753 myst_libre-0.0.0/myst_libre.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-26 14:08:22.000000 myst_libre-0.0.0/myst_libre.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-26 14:08:22.000000 myst_libre-0.0.0/myst_libre.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:08:22.000000 myst_libre-0.0.0/myst_libre.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-26 14:08:22.000000 myst_libre-0.0.0/myst_libre.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 14:08:22.000000 myst_libre-0.0.0/myst_libre.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-26 14:08:04.000000 myst_libre-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-26 14:08:04.000000 myst_libre-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 14:08:22.908753 myst_libre-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:47:23.231505 myst_libre-0.0.post1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:47:23.227505 myst_libre-0.0.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:47:23.227505 myst_libre-0.0.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-26 14:47:23.231505 myst_libre-0.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:47:23.227505 myst_libre-0.0.post1/myst_libre/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/abstract_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:47:23.231505 myst_libre-0.0.post1/myst_libre/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/builders/myst_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:47:23.231505 myst_libre-0.0.post1/myst_libre/rees/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/rees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/rees/rees.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:47:23.231505 myst_libre-0.0.post1/myst_libre/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/test/test_myst_libre.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:47:23.231505 myst_libre-0.0.post1/myst_libre/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/tools/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/tools/build_source_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/tools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/tools/docker_registry_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/tools/jupyter_hub_local_spawner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5043 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/tools/myst_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/myst_libre/tools/rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:47:23.231505 myst_libre-0.0.post1/myst_libre.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-05-26 14:47:23.000000 myst_libre-0.0.post1/myst_libre.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-26 14:47:23.000000 myst_libre-0.0.post1/myst_libre.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:47:23.000000 myst_libre-0.0.post1/myst_libre.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-26 14:47:23.000000 myst_libre-0.0.post1/myst_libre.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-26 14:47:23.000000 myst_libre-0.0.post1/myst_libre.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-26 14:46:59.000000 myst_libre-0.0.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 14:47:23.231505 myst_libre-0.0.post1/setup.cfg
```

### Comparing `myst_libre-0.0.0/.github/workflows/publish.yml` & `myst_libre-0.0.post1/.github/workflows/publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,14 @@
         uses: actions/setup-python@v5
         with:
           python-version: '3.10.4'
           cache: pip
           cache-dependency-path: '**/pyproject.toml'
       - name: Install dependencies
         run: |
-          pip install setuptools wheel build
+          pip install setuptools wheel build twine setuptools_scm
       - name: Build
         run: |
           python -m build
       # retrieve your distributions here
       - name: Publish package distributions to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `myst_libre-0.0.0/.gitignore` & `myst_libre-0.0.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/PKG-INFO` & `myst_libre-0.0.post1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: myst_libre
-Version: 0.0.0
-Summary: A Python library for managing source code repositories, interacting with Docker registries, handling MyST markdown operations, and spawning JupyterHub instances locally.
-Author-email: agahkarakuzu <agahkarakuzu@gmail.com>
-Project-URL: Homepage, https://github.com/agahkarakuzu/myst_libre
-Keywords: myst,docker,jupyterhub,markdown,repository
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: docker
-Requires-Dist: dotenv
-Requires-Dist: PyGithub
-Requires-Dist: hashlib
-Requires-Dist: termcolor
-Requires-Dist: mystmd
-
 
 # MyST Libre
 
 ## JupyterHub in Docker for MyST
 
 A small library to manage reproducible execution environments using Docker and JupyterHub 
 to build MyST articles in containers.
```

### Comparing `myst_libre-0.0.0/example.py` & `myst_libre-0.0.post1/example.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/abstract_class.py` & `myst_libre-0.0.post1/myst_libre/abstract_class.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/builders/myst_builder.py` & `myst_libre-0.0.post1/myst_libre/builders/myst_builder.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/rees/rees.py` & `myst_libre-0.0.post1/myst_libre/rees/rees.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/test/test_myst_libre.py` & `myst_libre-0.0.post1/myst_libre/test/test_myst_libre.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/tools/authenticator.py` & `myst_libre-0.0.post1/myst_libre/tools/authenticator.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/tools/build_source_manager.py` & `myst_libre-0.0.post1/myst_libre/tools/build_source_manager.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/tools/decorators.py` & `myst_libre-0.0.post1/myst_libre/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/tools/docker_registry_client.py` & `myst_libre-0.0.post1/myst_libre/tools/docker_registry_client.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/tools/jupyter_hub_local_spawner.py` & `myst_libre-0.0.post1/myst_libre/tools/jupyter_hub_local_spawner.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/tools/myst_client.py` & `myst_libre-0.0.post1/myst_libre/tools/myst_client.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre/tools/rest_client.py` & `myst_libre-0.0.post1/myst_libre/tools/rest_client.py`

 * *Files identical despite different names*

### Comparing `myst_libre-0.0.0/myst_libre.egg-info/SOURCES.txt` & `myst_libre-0.0.post1/myst_libre.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+LICENSE
 README.md
 example.py
 pyproject.toml
 requirements.txt
 .github/workflows/publish.yml
 myst_libre/__init__.py
 myst_libre/abstract_class.py
```

### Comparing `myst_libre-0.0.0/pyproject.toml` & `myst_libre-0.0.post1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -17,16 +17,20 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests",
     "docker",
-    "dotenv",
+    "python-dotenv",
     "PyGithub",
     "hashlib",
     "termcolor",
     "mystmd"
 ]
 
 [project.urls]
-Homepage = "https://github.com/agahkarakuzu/myst_libre"
+Homepage = "https://github.com/agahkarakuzu/myst_libre"
+
+[tool.setuptools_scm]
+version_scheme = "post-release"
+local_scheme = "dirty-tag"
```

