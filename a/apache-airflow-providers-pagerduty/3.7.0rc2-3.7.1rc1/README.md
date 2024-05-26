# Comparing `tmp/apache_airflow_providers_pagerduty-3.7.0rc2.tar.gz` & `tmp/apache_airflow_providers_pagerduty-3.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_pagerduty-3.7.0rc2.tar", last modified: Tue Apr 30 11:39:07 2024, max compression
+gzip compressed data, was "apache_airflow_providers_pagerduty-3.7.1rc1.tar", last modified: Tue May 21 10:54:43 2024, max compression
```

## Comparing `apache_airflow_providers_pagerduty-3.7.0rc2.tar` & `apache_airflow_providers_pagerduty-3.7.1rc1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3076 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/LICENSE
--rw-r--r--   0        0        0     1584 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/__init__.py
--rw-r--r--   0        0        0     2944 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/__init__.py
--rw-r--r--   0        0        0     7880 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/pagerduty.py
--rw-r--r--   0        0        0    12306 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/pagerduty_events.py
--rw-r--r--   0        0        0      785 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/notifications/__init__.py
--rw-r--r--   0        0        0     5033 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/notifications/pagerduty.py
--rw-r--r--   0        0        0     2984 2024-04-30 11:39:07.000000 apache_airflow_providers_pagerduty-3.7.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 apache_airflow_providers_pagerduty-3.7.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     3076 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/LICENSE
+-rw-r--r--   0        0        0     1496 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/__init__.py
+-rw-r--r--   0        0        0     2965 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/hooks/__init__.py
+-rw-r--r--   0        0        0     7880 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/hooks/pagerduty.py
+-rw-r--r--   0        0        0    12306 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py
+-rw-r--r--   0        0        0      785 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/notifications/__init__.py
+-rw-r--r--   0        0        0     5033 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/notifications/pagerduty.py
+-rw-r--r--   0        0        0     2984 2024-05-21 10:54:43.000000 apache_airflow_providers_pagerduty-3.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4781 1970-01-01 00:00:00.000000 apache_airflow_providers_pagerduty-3.7.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/README.rst` & `apache_airflow_providers_pagerduty-3.7.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.7.0.rc2``
+Release: ``3.7.1.rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pagerduty`` provider. All classes for this provider package
 are in ``airflow.providers.pagerduty`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-pagerduty``
@@ -73,8 +73,8 @@
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.7.0``
 ``pdpyras``         ``>=4.1.2``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/LICENSE` & `apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/__init__.py` & `apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/__init__.py`

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
         f"The package `apache-airflow-providers-pagerduty:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/get_provider_info.py` & `apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-pagerduty",
         "name": "Pagerduty",
         "description": "`Pagerduty <https://www.pagerduty.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714477147,
+        "source-date-epoch": 1716288883,
         "versions": [
+            "3.7.1",
             "3.7.0",
             "3.6.2",
             "3.6.1",
             "3.6.0",
             "3.5.1",
             "3.5.0",
             "3.4.0",
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/__init__.py` & `apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/pagerduty.py` & `apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/hooks/pagerduty.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/hooks/pagerduty_events.py` & `apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/notifications/__init__.py` & `apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/airflow/providers/pagerduty/notifications/pagerduty.py` & `apache_airflow_providers_pagerduty-3.7.1rc1/airflow/providers/pagerduty/notifications/pagerduty.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/pyproject.toml` & `apache_airflow_providers_pagerduty-3.7.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-pagerduty"
-version = "3.7.0.rc2"
+version = "3.7.1.rc1"
 description = "Provider package apache-airflow-providers-pagerduty for Apache Airflow"
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
     "pdpyras>=4.1.2",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_pagerduty-3.7.0rc2/PKG-INFO` & `apache_airflow_providers_pagerduty-3.7.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.7.0rc2
+Version: 3.7.1rc1
 Summary: Provider package apache-airflow-providers-pagerduty for Apache Airflow
 Keywords: airflow-provider,pagerduty,airflow,integration
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
 Requires-Dist: pdpyras>=4.1.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -71,28 +71,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.7.0.rc2``
+Release: ``3.7.1.rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``pagerduty`` provider. All classes for this provider package
 are in ``airflow.providers.pagerduty`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-pagerduty``
@@ -106,8 +106,8 @@
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.7.0``
 ``pdpyras``         ``>=4.1.2``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.7.1/changelog.html>`_.
```

