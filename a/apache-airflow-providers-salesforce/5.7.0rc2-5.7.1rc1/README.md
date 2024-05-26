# Comparing `tmp/apache_airflow_providers_salesforce-5.7.0rc2.tar.gz` & `tmp/apache_airflow_providers_salesforce-5.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_salesforce-5.7.0rc2.tar", last modified: Tue Apr 30 11:43:28 2024, max compression
+gzip compressed data, was "apache_airflow_providers_salesforce-5.7.1rc1.tar", last modified: Tue May 21 10:56:30 2024, max compression
```

## Comparing `apache_airflow_providers_salesforce-5.7.0rc2.tar` & `apache_airflow_providers_salesforce-5.7.1rc1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3142 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/LICENSE
--rw-r--r--   0        0        0     1585 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/__init__.py
--rw-r--r--   0        0        0     3306 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/hooks/__init__.py
--rw-r--r--   0        0        0    18220 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/hooks/salesforce.py
--rw-r--r--   0        0        0      785 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/__init__.py
--rw-r--r--   0        0        0     4894 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/bulk.py
--rw-r--r--   0        0        0     2554 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/salesforce_apex_rest.py
--rw-r--r--   0        0        0     3027 2024-04-30 11:43:28.000000 apache_airflow_providers_salesforce-5.7.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4896 1970-01-01 00:00:00.000000 apache_airflow_providers_salesforce-5.7.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     3142 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/LICENSE
+-rw-r--r--   0        0        0     1497 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/__init__.py
+-rw-r--r--   0        0        0     3327 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/hooks/__init__.py
+-rw-r--r--   0        0        0    18220 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/hooks/salesforce.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/operators/__init__.py
+-rw-r--r--   0        0        0     4894 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/operators/bulk.py
+-rw-r--r--   0        0        0     2554 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py
+-rw-r--r--   0        0        0     3027 2024-05-21 10:56:30.000000 apache_airflow_providers_salesforce-5.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4896 1970-01-01 00:00:00.000000 apache_airflow_providers_salesforce-5.7.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/README.rst` & `apache_airflow_providers_salesforce-5.7.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.7.0.rc2``
+Release: ``5.7.1.rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``salesforce`` provider. All classes for this provider package
 are in ``airflow.providers.salesforce`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-salesforce``
@@ -74,8 +74,8 @@
 =====================  ==================
 ``apache-airflow``     ``>=2.7.0``
 ``simple-salesforce``  ``>=1.0.0``
 ``pandas``             ``>=1.2.5,<2.2``
 =====================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/LICENSE` & `apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/__init__.py` & `apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "5.7.0"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "5.7.1"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-salesforce:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/get_provider_info.py` & `apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-salesforce",
         "name": "Salesforce",
         "description": "`Salesforce <https://www.salesforce.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714477408,
+        "source-date-epoch": 1716288990,
         "versions": [
+            "5.7.1",
             "5.7.0",
             "5.6.3",
             "5.6.2",
             "5.6.1",
             "5.6.0",
             "5.5.1",
             "5.5.0",
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/hooks/__init__.py` & `apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/hooks/salesforce.py` & `apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/hooks/salesforce.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/__init__.py` & `apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/bulk.py` & `apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/operators/bulk.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/airflow/providers/salesforce/operators/salesforce_apex_rest.py` & `apache_airflow_providers_salesforce-5.7.1rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/pyproject.toml` & `apache_airflow_providers_salesforce-5.7.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-salesforce"
-version = "5.7.0.rc2"
+version = "5.7.1.rc1"
 description = "Provider package apache-airflow-providers-salesforce for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -58,16 +58,16 @@
 dependencies = [
     "apache-airflow>=2.7.0rc0",
     "pandas>=1.2.5,<2.2",
     "simple-salesforce>=1.0.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_salesforce-5.7.0rc2/PKG-INFO` & `apache_airflow_providers_salesforce-5.7.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-salesforce
-Version: 5.7.0rc2
+Version: 5.7.1rc1
 Summary: Provider package apache-airflow-providers-salesforce for Apache Airflow
 Keywords: airflow-provider,salesforce,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: pandas>=1.2.5,<2.2
 Requires-Dist: simple-salesforce>=1.0.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -72,28 +72,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.7.0.rc2``
+Release: ``5.7.1.rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``salesforce`` provider. All classes for this provider package
 are in ``airflow.providers.salesforce`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-salesforce``
@@ -108,8 +108,8 @@
 =====================  ==================
 ``apache-airflow``     ``>=2.7.0``
 ``simple-salesforce``  ``>=1.0.0``
 ``pandas``             ``>=1.2.5,<2.2``
 =====================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.7.1/changelog.html>`_.
```

