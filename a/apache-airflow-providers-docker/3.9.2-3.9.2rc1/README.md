# Comparing `tmp/apache_airflow_providers_docker-3.9.2.tar.gz` & `tmp/apache_airflow_providers_docker-3.9.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_docker-3.9.2.tar", last modified: Mon Mar  4 12:29:24 2024, max compression
+gzip compressed data, was "apache_airflow_providers_docker-3.9.2rc1.tar", last modified: Mon Mar  4 12:29:24 2024, max compression
```

## Comparing `apache_airflow_providers_docker-3.9.2.tar` & `apache_airflow_providers_docker-3.9.2rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3072 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/README.rst
--rw-r--r--   0        0        0    13569 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/LICENSE
--rw-r--r--   0        0        0     1581 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/__init__.py
--rw-r--r--   0        0        0      787 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/decorators/__init__.py
--rw-r--r--   0        0        0     6361 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/decorators/docker.py
--rw-r--r--   0        0        0     1670 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/exceptions.py
--rw-r--r--   0        0        0     3545 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/hooks/__init__.py
--rw-r--r--   0        0        0     9257 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/hooks/docker.py
--rw-r--r--   0        0        0      787 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/operators/__init__.py
--rw-r--r--   0        0        0    24865 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/operators/docker.py
--rw-r--r--   0        0        0    10298 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/airflow/providers/docker/operators/docker_swarm.py
--rw-r--r--   0        0        0     2934 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2/pyproject.toml
--rw-r--r--   0        0        0     4737 1970-01-01 00:00:00.000000 apache_airflow_providers_docker-3.9.2/PKG-INFO
+-rw-r--r--   0        0        0     3076 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/LICENSE
+-rw-r--r--   0        0        0     1581 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/__init__.py
+-rw-r--r--   0        0        0      787 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/decorators/__init__.py
+-rw-r--r--   0        0        0     6361 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/decorators/docker.py
+-rw-r--r--   0        0        0     1670 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/exceptions.py
+-rw-r--r--   0        0        0     3545 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/hooks/__init__.py
+-rw-r--r--   0        0        0     9257 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/hooks/docker.py
+-rw-r--r--   0        0        0      787 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/operators/__init__.py
+-rw-r--r--   0        0        0    24865 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/operators/docker.py
+-rw-r--r--   0        0        0    10298 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/operators/docker_swarm.py
+-rw-r--r--   0        0        0     2943 2024-03-04 12:29:24.000000 apache_airflow_providers_docker-3.9.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 apache_airflow_providers_docker-3.9.2rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_docker-3.9.2/README.rst` & `apache_airflow_providers_docker-3.9.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.9.2``
+Release: ``3.9.2.rc1``
 
 
 `Docker <https://www.docker.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/LICENSE` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/__init__.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/decorators/__init__.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/decorators/docker.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/decorators/docker.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/exceptions.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/get_provider_info.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/hooks/__init__.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/hooks/docker.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/hooks/docker.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/operators/__init__.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/operators/docker.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/operators/docker.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/airflow/providers/docker/operators/docker_swarm.py` & `apache_airflow_providers_docker-3.9.2rc1/airflow/providers/docker/operators/docker_swarm.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_docker-3.9.2/pyproject.toml` & `apache_airflow_providers_docker-3.9.2rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-docker"
-version = "3.9.2"
+version = "3.9.2.rc1"
 description = "Provider package apache-airflow-providers-docker for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -51,15 +51,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0",
+    "apache-airflow>=2.6.0.dev0",
     "docker>=6",
     "python-dotenv>=0.21.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-docker/3.9.2"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-docker/3.9.2/changelog.html"
```

### Comparing `apache_airflow_providers_docker-3.9.2/PKG-INFO` & `apache_airflow_providers_docker-3.9.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.9.2
+Version: 3.9.2rc1
 Summary: Provider package apache-airflow-providers-docker for Apache Airflow
 Keywords: airflow-provider,docker,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow>=2.6.0.dev0
 Requires-Dist: docker>=6
 Requires-Dist: python-dotenv>=0.21.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.9.2/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.9.2
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -71,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.9.2``
+Release: ``3.9.2.rc1``
 
 
 `Docker <https://www.docker.com/>`__
 
 
 Provider package
 ----------------
```

