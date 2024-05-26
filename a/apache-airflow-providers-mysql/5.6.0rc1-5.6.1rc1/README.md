# Comparing `tmp/apache_airflow_providers_mysql-5.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_mysql-5.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_mysql-5.6.0rc1.tar", last modified: Tue Apr 30 11:34:47 2024, max compression
+gzip compressed data, was "apache_airflow_providers_mysql-5.6.1rc1.tar", last modified: Tue May 21 10:42:54 2024, max compression
```

## Comparing `apache_airflow_providers_mysql-5.6.0rc1.tar` & `apache_airflow_providers_mysql-5.6.1rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4937 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/LICENSE
--rw-r--r--   0        0        0     1580 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/__init__.py
--rw-r--r--   0        0        0      785 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/datasets/__init__.py
--rw-r--r--   0        0        0     1385 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/datasets/mysql.py
--rw-r--r--   0        0        0     4247 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/hooks/__init__.py
--rw-r--r--   0        0        0    13220 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/hooks/mysql.py
--rw-r--r--   0        0        0      787 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/operators/__init__.py
--rw-r--r--   0        0        0     2934 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/operators/mysql.py
--rw-r--r--   0        0        0      785 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/__init__.py
--rw-r--r--   0        0        0     3269 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
--rw-r--r--   0        0        0     3876 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
--rw-r--r--   0        0        0     3251 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
--rw-r--r--   0        0        0     6308 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
--rw-r--r--   0        0        0     3456 2024-04-30 11:34:47.000000 apache_airflow_providers_mysql-5.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7339 1970-01-01 00:00:00.000000 apache_airflow_providers_mysql-5.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4937 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/LICENSE
+-rw-r--r--   0        0        0     1492 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/__init__.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/datasets/__init__.py
+-rw-r--r--   0        0        0     1385 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/datasets/mysql.py
+-rw-r--r--   0        0        0     4268 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/hooks/__init__.py
+-rw-r--r--   0        0        0    13220 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/hooks/mysql.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/operators/__init__.py
+-rw-r--r--   0        0        0     2934 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/operators/mysql.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/__init__.py
+-rw-r--r--   0        0        0     3269 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
+-rw-r--r--   0        0        0     3876 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
+-rw-r--r--   0        0        0     3251 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
+-rw-r--r--   0        0        0     6308 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
+-rw-r--r--   0        0        0     3456 2024-05-21 10:42:54.000000 apache_airflow_providers_mysql-5.6.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     7339 1970-01-01 00:00:00.000000 apache_airflow_providers_mysql-5.6.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/README.rst` & `apache_airflow_providers_mysql-5.6.1rc1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.6.0.rc1``
+Release: ``5.6.1.rc1``
 
 
 `MySQL <https://www.mysql.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-mysql``
@@ -99,8 +99,8 @@
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-presto <https://airflow.apache.org/docs/apache-airflow-providers-presto>`_            ``presto``
 `apache-airflow-providers-trino <https://airflow.apache.org/docs/apache-airflow-providers-trino>`_              ``trino``
 `apache-airflow-providers-vertica <https://airflow.apache.org/docs/apache-airflow-providers-vertica>`_          ``vertica``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/LICENSE` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/__init__.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "5.6.0"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "5.6.1"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-mysql:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/datasets/__init__.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/datasets/mysql.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/datasets/mysql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/get_provider_info.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-mysql",
         "name": "MySQL",
         "description": "`MySQL <https://www.mysql.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714476887,
+        "source-date-epoch": 1716288174,
         "versions": [
+            "5.6.1",
             "5.6.0",
             "5.5.4",
             "5.5.3",
             "5.5.2",
             "5.5.1",
             "5.5.0",
             "5.4.0",
```

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/hooks/__init__.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/hooks/mysql.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/operators/__init__.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/operators/mysql.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/operators/mysql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/__init__.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/presto_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/s3_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/trino_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py` & `apache_airflow_providers_mysql-5.6.1rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/pyproject.toml` & `apache_airflow_providers_mysql-5.6.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-mysql"
-version = "5.6.0.rc1"
+version = "5.6.1.rc1"
 description = "Provider package apache-airflow-providers-mysql for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -59,16 +59,16 @@
     "apache-airflow-providers-common-sql>=1.3.1rc0",
     "apache-airflow>=2.7.0rc0",
     "mysql-connector-python>=8.0.29",
     "mysqlclient>=1.3.6",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_mysql-5.6.0rc1/PKG-INFO` & `apache_airflow_providers_mysql-5.6.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.6.0rc1
+Version: 5.6.1rc1
 Summary: Provider package apache-airflow-providers-mysql for Apache Airflow
 Keywords: airflow-provider,mysql,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,16 +28,16 @@
 Requires-Dist: apache-airflow-providers-amazon ; extra == "amazon"
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Requires-Dist: apache-airflow-providers-presto ; extra == "presto"
 Requires-Dist: apache-airflow-providers-trino ; extra == "trino"
 Requires-Dist: apache-airflow-providers-vertica ; extra == "vertica"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: amazon
 Provides-Extra: common.sql
 Provides-Extra: mysql-connector-python
@@ -86,28 +86,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.6.0.rc1``
+Release: ``5.6.1.rc1``
 
 
 `MySQL <https://www.mysql.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-mysql``
@@ -147,8 +147,8 @@
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-presto <https://airflow.apache.org/docs/apache-airflow-providers-presto>`_            ``presto``
 `apache-airflow-providers-trino <https://airflow.apache.org/docs/apache-airflow-providers-trino>`_              ``trino``
 `apache-airflow-providers-vertica <https://airflow.apache.org/docs/apache-airflow-providers-vertica>`_          ``vertica``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.6.1/changelog.html>`_.
```

