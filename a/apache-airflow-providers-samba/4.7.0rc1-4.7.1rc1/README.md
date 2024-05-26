# Comparing `tmp/apache_airflow_providers_samba-4.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_samba-4.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_samba-4.7.0rc1.tar", last modified: Tue Apr 30 11:43:59 2024, max compression
+gzip compressed data, was "apache_airflow_providers_samba-4.7.1rc1.tar", last modified: Tue May 21 10:56:32 2024, max compression
```

## Comparing `apache_airflow_providers_samba-4.7.0rc1.tar` & `apache_airflow_providers_samba-4.7.1rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4015 2024-04-30 11:43:59.000000 apache_airflow_providers_samba-4.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:43:59.000000 apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/LICENSE
--rw-r--r--   0        0        0     1580 2024-04-30 11:43:59.000000 apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/__init__.py
--rw-r--r--   0        0        0     2692 2024-04-30 11:43:59.000000 apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:43:59.000000 apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/hooks/__init__.py
--rw-r--r--   0        0        0     9141 2024-04-30 11:43:59.000000 apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/hooks/samba.py
--rw-r--r--   0        0        0      785 2024-04-30 11:43:59.000000 apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/transfers/__init__.py
--rw-r--r--   0        0        0     8958 2024-04-30 11:43:59.000000 apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/transfers/gcs_to_samba.py
--rw-r--r--   0        0        0     3046 2024-04-30 11:43:59.000000 apache_airflow_providers_samba-4.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     5794 1970-01-01 00:00:00.000000 apache_airflow_providers_samba-4.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4015 2024-05-21 10:56:32.000000 apache_airflow_providers_samba-4.7.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:56:32.000000 apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/LICENSE
+-rw-r--r--   0        0        0     1492 2024-05-21 10:56:32.000000 apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/__init__.py
+-rw-r--r--   0        0        0     2713 2024-05-21 10:56:32.000000 apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:56:32.000000 apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/hooks/__init__.py
+-rw-r--r--   0        0        0     9141 2024-05-21 10:56:32.000000 apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/hooks/samba.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:56:32.000000 apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/transfers/__init__.py
+-rw-r--r--   0        0        0     8958 2024-05-21 10:56:32.000000 apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/transfers/gcs_to_samba.py
+-rw-r--r--   0        0        0     3046 2024-05-21 10:56:32.000000 apache_airflow_providers_samba-4.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     5794 1970-01-01 00:00:00.000000 apache_airflow_providers_samba-4.7.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_samba-4.7.0rc1/README.rst` & `apache_airflow_providers_samba-4.7.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-samba``
 
-Release: ``4.7.0.rc1``
+Release: ``4.7.1.rc1``
 
 
 `Samba <https://www.samba.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``samba`` provider. All classes for this provider package
 are in ``airflow.providers.samba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-samba``
@@ -92,8 +92,8 @@
 ====================================================================================================  ==========
 Dependent package                                                                                     Extra
 ====================================================================================================  ==========
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_  ``google``
 ====================================================================================================  ==========
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/LICENSE` & `apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/__init__.py` & `apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/__init__.py`

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
 
-__version__ = "4.7.0"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "4.7.1"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-samba:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/get_provider_info.py` & `apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-samba",
         "name": "Samba",
         "description": "`Samba <https://www.samba.org/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714477439,
+        "source-date-epoch": 1716288992,
         "versions": [
+            "4.7.1",
             "4.7.0",
             "4.6.0",
             "4.5.0",
             "4.4.0",
             "4.3.0",
             "4.2.2",
             "4.2.1",
```

### Comparing `apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/hooks/__init__.py` & `apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/hooks/samba.py` & `apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/hooks/samba.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/transfers/__init__.py` & `apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_samba-4.7.0rc1/airflow/providers/samba/transfers/gcs_to_samba.py` & `apache_airflow_providers_samba-4.7.1rc1/airflow/providers/samba/transfers/gcs_to_samba.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_samba-4.7.0rc1/pyproject.toml` & `apache_airflow_providers_samba-4.7.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-samba"
-version = "4.7.0.rc1"
+version = "4.7.1.rc1"
 description = "Provider package apache-airflow-providers-samba for Apache Airflow"
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
     "smbprotocol>=1.5.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_samba-4.7.0rc1/PKG-INFO` & `apache_airflow_providers_samba-4.7.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-samba
-Version: 4.7.0rc1
+Version: 4.7.1rc1
 Summary: Provider package apache-airflow-providers-samba for Apache Airflow
 Keywords: airflow-provider,samba,airflow,integration
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
 Requires-Dist: smbprotocol>=1.5.0
 Requires-Dist: apache-airflow-providers-google ; extra == "google"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: google
 
 
@@ -73,28 +73,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-samba``
 
-Release: ``4.7.0.rc1``
+Release: ``4.7.1.rc1``
 
 
 `Samba <https://www.samba.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``samba`` provider. All classes for this provider package
 are in ``airflow.providers.samba`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-samba``
@@ -127,8 +127,8 @@
 ====================================================================================================  ==========
 Dependent package                                                                                     Extra
 ====================================================================================================  ==========
 `apache-airflow-providers-google <https://airflow.apache.org/docs/apache-airflow-providers-google>`_  ``google``
 ====================================================================================================  ==========
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-samba/4.7.1/changelog.html>`_.
```

