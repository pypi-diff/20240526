# Comparing `tmp/apache_airflow_providers_papermill-3.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_papermill-3.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_papermill-3.7.0rc1.tar", last modified: Tue Apr 30 11:39:38 2024, max compression
+gzip compressed data, was "apache_airflow_providers_papermill-3.7.1rc1.tar", last modified: Tue May 21 10:54:46 2024, max compression
```

## Comparing `apache_airflow_providers_papermill-3.7.0rc1.tar` & `apache_airflow_providers_papermill-3.7.1rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3114 2024-04-30 11:39:38.000000 apache_airflow_providers_papermill-3.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:39:38.000000 apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/LICENSE
--rw-r--r--   0        0        0     1584 2024-04-30 11:39:38.000000 apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/__init__.py
--rw-r--r--   0        0        0     2902 2024-04-30 11:39:38.000000 apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:39:38.000000 apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/hooks/__init__.py
--rw-r--r--   0        0        0     5937 2024-04-30 11:39:38.000000 apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/hooks/kernel.py
--rw-r--r--   0        0        0      787 2024-04-30 11:39:38.000000 apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/operators/__init__.py
--rw-r--r--   0        0        0     4689 2024-04-30 11:39:38.000000 apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/operators/papermill.py
--rw-r--r--   0        0        0     2984 2024-04-30 11:39:38.000000 apache_airflow_providers_papermill-3.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 apache_airflow_providers_papermill-3.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3114 2024-05-21 10:54:46.000000 apache_airflow_providers_papermill-3.7.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:54:46.000000 apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/LICENSE
+-rw-r--r--   0        0        0     1496 2024-05-21 10:54:46.000000 apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/__init__.py
+-rw-r--r--   0        0        0     2923 2024-05-21 10:54:46.000000 apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:54:46.000000 apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/hooks/__init__.py
+-rw-r--r--   0        0        0     5937 2024-05-21 10:54:46.000000 apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/hooks/kernel.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:54:46.000000 apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/operators/__init__.py
+-rw-r--r--   0        0        0     4689 2024-05-21 10:54:46.000000 apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/operators/papermill.py
+-rw-r--r--   0        0        0     2984 2024-05-21 10:54:46.000000 apache_airflow_providers_papermill-3.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4830 1970-01-01 00:00:00.000000 apache_airflow_providers_papermill-3.7.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/README.rst` & `apache_airflow_providers_papermill-3.7.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-papermill``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.1.rc1``
 
 
 `Papermill <https://github.com/nteract/papermill>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``papermill`` provider. All classes for this provider package
 are in ``airflow.providers.papermill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-papermill``
@@ -75,8 +75,8 @@
 ``apache-airflow``  ``>=2.7.0``
 ``papermill[all]``  ``>=2.4.0``
 ``scrapbook[all]``
 ``ipykernel``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/LICENSE` & `apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/__init__.py` & `apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/__init__.py`

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
         f"The package `apache-airflow-providers-papermill:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/get_provider_info.py` & `apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-papermill",
         "name": "Papermill",
         "description": "`Papermill <https://github.com/nteract/papermill>`__\n",
         "excluded-python-versions": ["3.12"],
         "state": "ready",
-        "source-date-epoch": 1714477178,
+        "source-date-epoch": 1716288886,
         "versions": [
+            "3.7.1",
             "3.7.0",
             "3.6.2",
             "3.6.1",
             "3.6.0",
             "3.5.0",
             "3.4.0",
             "3.2.1",
```

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/hooks/__init__.py` & `apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/hooks/kernel.py` & `apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/hooks/kernel.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/operators/__init__.py` & `apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/airflow/providers/papermill/operators/papermill.py` & `apache_airflow_providers_papermill-3.7.1rc1/airflow/providers/papermill/operators/papermill.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/pyproject.toml` & `apache_airflow_providers_papermill-3.7.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-papermill"
-version = "3.7.0.rc1"
+version = "3.7.1.rc1"
 description = "Provider package apache-airflow-providers-papermill for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -58,16 +58,16 @@
     "apache-airflow>=2.7.0rc0",
     "ipykernel",
     "papermill[all]>=2.4.0",
     "scrapbook[all]",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_papermill-3.7.0rc1/PKG-INFO` & `apache_airflow_providers_papermill-3.7.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-papermill
-Version: 3.7.0rc1
+Version: 3.7.1rc1
 Summary: Provider package apache-airflow-providers-papermill for Apache Airflow
 Keywords: airflow-provider,papermill,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: ipykernel
 Requires-Dist: papermill[all]>=2.4.0
 Requires-Dist: scrapbook[all]
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -72,28 +72,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-papermill``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.1.rc1``
 
 
 `Papermill <https://github.com/nteract/papermill>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``papermill`` provider. All classes for this provider package
 are in ``airflow.providers.papermill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-papermill``
@@ -109,8 +109,8 @@
 ``apache-airflow``  ``>=2.7.0``
 ``papermill[all]``  ``>=2.4.0``
 ``scrapbook[all]``
 ``ipykernel``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.7.1/changelog.html>`_.
```

