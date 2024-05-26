# Comparing `tmp/apache_airflow_providers_odbc-4.6.0rc1.tar.gz` & `tmp/apache_airflow_providers_odbc-4.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_odbc-4.6.0rc1.tar", last modified: Tue Apr 30 11:35:47 2024, max compression
+gzip compressed data, was "apache_airflow_providers_odbc-4.6.1rc1.tar", last modified: Tue May 21 10:43:00 2024, max compression
```

## Comparing `apache_airflow_providers_odbc-4.6.0rc1.tar` & `apache_airflow_providers_odbc-4.6.1rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4225 2024-04-30 11:35:47.000000 apache_airflow_providers_odbc-4.6.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:35:47.000000 apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/LICENSE
--rw-r--r--   0        0        0     1579 2024-04-30 11:35:47.000000 apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/__init__.py
--rw-r--r--   0        0        0     2470 2024-04-30 11:35:47.000000 apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-30 11:35:47.000000 apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/hooks/__init__.py
--rw-r--r--   0        0        0    10016 2024-04-30 11:35:47.000000 apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/hooks/odbc.py
--rw-r--r--   0        0        0     3089 2024-04-30 11:35:47.000000 apache_airflow_providers_odbc-4.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 apache_airflow_providers_odbc-4.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4225 2024-05-21 10:43:00.000000 apache_airflow_providers_odbc-4.6.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:43:00.000000 apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/LICENSE
+-rw-r--r--   0        0        0     1491 2024-05-21 10:43:00.000000 apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/__init__.py
+-rw-r--r--   0        0        0     2491 2024-05-21 10:43:00.000000 apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:43:00.000000 apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/hooks/__init__.py
+-rw-r--r--   0        0        0    10016 2024-05-21 10:43:00.000000 apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/hooks/odbc.py
+-rw-r--r--   0        0        0     3089 2024-05-21 10:43:00.000000 apache_airflow_providers_odbc-4.6.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 apache_airflow_providers_odbc-4.6.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_odbc-4.6.0rc1/README.rst` & `apache_airflow_providers_odbc-4.6.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``4.6.0.rc1``
+Release: ``4.6.1.rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``odbc`` provider. All classes for this provider package
 are in ``airflow.providers.odbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-odbc``
@@ -93,8 +93,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/LICENSE` & `apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/__init__.py` & `apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "4.6.0"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "4.6.1"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-odbc:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/get_provider_info.py` & `apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/get_provider_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-odbc",
         "name": "ODBC",
         "description": "`ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714476947,
+        "source-date-epoch": 1716288180,
         "versions": [
+            "4.6.1",
             "4.6.0",
             "4.5.0",
             "4.4.1",
             "4.4.0",
             "4.3.0",
             "4.2.0",
             "4.1.0",
```

### Comparing `apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/hooks/__init__.py` & `apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.6.0rc1/airflow/providers/odbc/hooks/odbc.py` & `apache_airflow_providers_odbc-4.6.1rc1/airflow/providers/odbc/hooks/odbc.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_odbc-4.6.0rc1/pyproject.toml` & `apache_airflow_providers_odbc-4.6.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-odbc"
-version = "4.6.0.rc1"
+version = "4.6.1.rc1"
 description = "Provider package apache-airflow-providers-odbc for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -58,16 +58,16 @@
 dependencies = [
     "apache-airflow-providers-common-sql>=1.10.0rc0",
     "apache-airflow>=2.7.0rc0",
     "pyodbc",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_odbc-4.6.0rc1/PKG-INFO` & `apache_airflow_providers_odbc-4.6.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-odbc
-Version: 4.6.0rc1
+Version: 4.6.1rc1
 Summary: Provider package apache-airflow-providers-odbc for Apache Airflow
 Keywords: airflow-provider,odbc,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow-providers-common-sql>=1.10.0rc0
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: pyodbc
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 
 
@@ -74,28 +74,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``4.6.0.rc1``
+Release: ``4.6.1.rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``odbc`` provider. All classes for this provider package
 are in ``airflow.providers.odbc`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-odbc``
@@ -129,8 +129,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.6.1/changelog.html>`_.
```

