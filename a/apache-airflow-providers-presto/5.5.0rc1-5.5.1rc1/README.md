# Comparing `tmp/apache_airflow_providers_presto-5.5.0rc1.tar.gz` & `tmp/apache_airflow_providers_presto-5.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_presto-5.5.0rc1.tar", last modified: Tue Apr 30 11:41:43 2024, max compression
+gzip compressed data, was "apache_airflow_providers_presto-5.5.1rc1.tar", last modified: Tue May 21 10:56:23 2024, max compression
```

## Comparing `apache_airflow_providers_presto-5.5.0rc1.tar` & `apache_airflow_providers_presto-5.5.1rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4439 2024-04-30 11:41:43.000000 apache_airflow_providers_presto-5.5.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:41:43.000000 apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/LICENSE
--rw-r--r--   0        0        0     1581 2024-04-30 11:41:43.000000 apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/__init__.py
--rw-r--r--   0        0        0     3196 2024-04-30 11:41:43.000000 apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:41:43.000000 apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/hooks/__init__.py
--rw-r--r--   0        0        0     8486 2024-04-30 11:41:43.000000 apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/hooks/presto.py
--rw-r--r--   0        0        0      785 2024-04-30 11:41:43.000000 apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/transfers/__init__.py
--rw-r--r--   0        0        0     4837 2024-04-30 11:41:43.000000 apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/transfers/gcs_to_presto.py
--rw-r--r--   0        0        0     3203 2024-04-30 11:41:43.000000 apache_airflow_providers_presto-5.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6429 1970-01-01 00:00:00.000000 apache_airflow_providers_presto-5.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4439 2024-05-21 10:56:23.000000 apache_airflow_providers_presto-5.5.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:56:23.000000 apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/LICENSE
+-rw-r--r--   0        0        0     1493 2024-05-21 10:56:23.000000 apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/__init__.py
+-rw-r--r--   0        0        0     3217 2024-05-21 10:56:23.000000 apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:56:23.000000 apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/hooks/__init__.py
+-rw-r--r--   0        0        0     8486 2024-05-21 10:56:23.000000 apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/hooks/presto.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:56:23.000000 apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/transfers/__init__.py
+-rw-r--r--   0        0        0     4837 2024-05-21 10:56:23.000000 apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/transfers/gcs_to_presto.py
+-rw-r--r--   0        0        0     3203 2024-05-21 10:56:23.000000 apache_airflow_providers_presto-5.5.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     6429 1970-01-01 00:00:00.000000 apache_airflow_providers_presto-5.5.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_presto-5.5.0rc1/README.rst` & `apache_airflow_providers_presto-5.5.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.5.0.rc1``
+Release: ``5.5.1.rc1``
 
 
 `Presto <https://prestodb.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``presto`` provider. All classes for this provider package
 are in ``airflow.providers.presto`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-presto``
@@ -95,8 +95,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_          ``google``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/LICENSE` & `apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/__init__.py` & `apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "5.5.0"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "5.5.1"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-presto:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/get_provider_info.py` & `apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-presto",
         "name": "Presto",
         "description": "`Presto <https://prestodb.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714477303,
+        "source-date-epoch": 1716288983,
         "versions": [
+            "5.5.1",
             "5.5.0",
             "5.4.2",
             "5.4.1",
             "5.4.0",
             "5.3.0",
             "5.2.1",
             "5.2.0",
```

### Comparing `apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/hooks/__init__.py` & `apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/hooks/presto.py` & `apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/hooks/presto.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/transfers/__init__.py` & `apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_presto-5.5.0rc1/airflow/providers/presto/transfers/gcs_to_presto.py` & `apache_airflow_providers_presto-5.5.1rc1/airflow/providers/presto/transfers/gcs_to_presto.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_presto-5.5.0rc1/pyproject.toml` & `apache_airflow_providers_presto-5.5.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-presto"
-version = "5.5.0.rc1"
+version = "5.5.1.rc1"
 description = "Provider package apache-airflow-providers-presto for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -59,16 +59,16 @@
     "apache-airflow-providers-common-sql>=1.3.1rc0",
     "apache-airflow>=2.7.0rc0",
     "pandas>=1.2.5,<2.2",
     "presto-python-client>=0.8.4",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_presto-5.5.0rc1/PKG-INFO` & `apache_airflow_providers_presto-5.5.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-presto
-Version: 5.5.0rc1
+Version: 5.5.1rc1
 Summary: Provider package apache-airflow-providers-presto for Apache Airflow
 Keywords: airflow-provider,presto,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,16 +24,16 @@
 Requires-Dist: apache-airflow-providers-common-sql>=1.3.1rc0
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: pandas>=1.2.5,<2.2
 Requires-Dist: presto-python-client>=0.8.4
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: apache-airflow-providers-google ; extra == "google"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 Provides-Extra: google
 
@@ -77,28 +77,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.5.0.rc1``
+Release: ``5.5.1.rc1``
 
 
 `Presto <https://prestodb.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``presto`` provider. All classes for this provider package
 are in ``airflow.providers.presto`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-presto``
@@ -134,8 +134,8 @@
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_          ``google``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-presto/5.5.1/changelog.html>`_.
```

