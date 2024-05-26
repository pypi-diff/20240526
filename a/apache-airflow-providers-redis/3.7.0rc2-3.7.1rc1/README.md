# Comparing `tmp/apache_airflow_providers_redis-3.7.0rc2.tar.gz` & `tmp/apache_airflow_providers_redis-3.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_redis-3.7.0rc2.tar", last modified: Tue Apr 30 11:43:11 2024, max compression
+gzip compressed data, was "apache_airflow_providers_redis-3.7.1rc1.tar", last modified: Tue May 21 10:56:28 2024, max compression
```

## Comparing `apache_airflow_providers_redis-3.7.0rc2.tar` & `apache_airflow_providers_redis-3.7.1rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3082 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/LICENSE
--rw-r--r--   0        0        0     1580 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/__init__.py
--rw-r--r--   0        0        0     2938 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/hooks/__init__.py
--rw-r--r--   0        0        0     5804 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/hooks/redis.py
--rw-r--r--   0        0        0      787 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/log/__init__.py
--rw-r--r--   0        0        0     3677 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/log/redis_task_handler.py
--rw-r--r--   0        0        0      787 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/operators/__init__.py
--rw-r--r--   0        0        0     2096 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/operators/redis_publish.py
--rw-r--r--   0        0        0      787 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/__init__.py
--rw-r--r--   0        0        0     1585 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/redis_key.py
--rw-r--r--   0        0        0     2672 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/redis_pub_sub.py
--rw-r--r--   0        0        0     2970 2024-04-30 11:43:11.000000 apache_airflow_providers_redis-3.7.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 apache_airflow_providers_redis-3.7.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     3082 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/LICENSE
+-rw-r--r--   0        0        0     1492 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/__init__.py
+-rw-r--r--   0        0        0     2959 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/hooks/__init__.py
+-rw-r--r--   0        0        0     5804 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/hooks/redis.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/log/__init__.py
+-rw-r--r--   0        0        0     3677 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/log/redis_task_handler.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/operators/__init__.py
+-rw-r--r--   0        0        0     2096 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/operators/redis_publish.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/sensors/__init__.py
+-rw-r--r--   0        0        0     1585 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/sensors/redis_key.py
+-rw-r--r--   0        0        0     2672 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/sensors/redis_pub_sub.py
+-rw-r--r--   0        0        0     2970 2024-05-21 10:56:28.000000 apache_airflow_providers_redis-3.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 apache_airflow_providers_redis-3.7.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_redis-3.7.0rc2/README.rst` & `apache_airflow_providers_redis-3.7.1rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.7.0.rc2``
+Release: ``3.7.1.rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``redis`` provider. All classes for this provider package
 are in ``airflow.providers.redis`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-redis``
@@ -73,8 +73,8 @@
 PIP package         Version required
 ==================  ===========================
 ``apache-airflow``  ``>=2.7.0``
 ``redis``           ``>=4.5.2,!=4.5.5,!=5.0.2``
 ==================  ===========================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/LICENSE` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/__init__.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "3.7.0"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "3.7.1"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-redis:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/get_provider_info.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-redis",
         "name": "Redis",
         "description": "`Redis <https://redis.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714477391,
+        "source-date-epoch": 1716288988,
         "versions": [
+            "3.7.1",
             "3.7.0",
             "3.6.1",
             "3.6.0",
             "3.5.0",
             "3.4.1",
             "3.4.0",
             "3.3.2",
```

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/hooks/__init__.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/hooks/redis.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/hooks/redis.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/log/__init__.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/log/redis_task_handler.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/log/redis_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/operators/__init__.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/operators/redis_publish.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/operators/redis_publish.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/__init__.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/redis_key.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/sensors/redis_key.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/airflow/providers/redis/sensors/redis_pub_sub.py` & `apache_airflow_providers_redis-3.7.1rc1/airflow/providers/redis/sensors/redis_pub_sub.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_redis-3.7.0rc2/pyproject.toml` & `apache_airflow_providers_redis-3.7.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-redis"
-version = "3.7.0.rc2"
+version = "3.7.1.rc1"
 description = "Provider package apache-airflow-providers-redis for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -57,16 +57,16 @@
 requires-python = "~=3.8"
 dependencies = [
     "apache-airflow>=2.7.0rc0",
     "redis>=4.5.2,!=4.5.5,!=5.0.2",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_redis-3.7.0rc2/PKG-INFO` & `apache_airflow_providers_redis-3.7.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.7.0rc2
+Version: 3.7.1rc1
 Summary: Provider package apache-airflow-providers-redis for Apache Airflow
 Keywords: airflow-provider,redis,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: redis>=4.5.2,!=4.5.5,!=5.0.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -71,28 +71,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.7.0.rc2``
+Release: ``3.7.1.rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``redis`` provider. All classes for this provider package
 are in ``airflow.providers.redis`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-redis``
@@ -106,8 +106,8 @@
 PIP package         Version required
 ==================  ===========================
 ``apache-airflow``  ``>=2.7.0``
 ``redis``           ``>=4.5.2,!=4.5.5,!=5.0.2``
 ==================  ===========================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.7.1/changelog.html>`_.
```

