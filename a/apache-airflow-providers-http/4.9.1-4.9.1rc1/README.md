# Comparing `tmp/apache_airflow_providers_http-4.9.1.tar.gz` & `tmp/apache_airflow_providers_http-4.9.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_http-4.9.1.tar", last modified: Sun Feb 11 07:26:47 2024, max compression
+gzip compressed data, was "apache_airflow_providers_http-4.9.1rc1.tar", last modified: Sun Feb 11 07:26:47 2024, max compression
```

## Comparing `apache_airflow_providers_http-4.9.1.tar` & `apache_airflow_providers_http-4.9.1rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3156 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/README.rst
--rw-r--r--   0        0        0    13569 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/LICENSE
--rw-r--r--   0        0        0     1579 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/__init__.py
--rw-r--r--   0        0        0     3545 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/hooks/__init__.py
--rw-r--r--   0        0        0    18315 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/hooks/http.py
--rw-r--r--   0        0        0      787 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/operators/__init__.py
--rw-r--r--   0        0        0    17549 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/operators/http.py
--rw-r--r--   0        0        0      787 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/sensors/__init__.py
--rw-r--r--   0        0        0     8109 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/sensors/http.py
--rw-r--r--   0        0        0      787 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/triggers/__init__.py
--rw-r--r--   0        0        0     7702 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/airflow/providers/http/triggers/http.py
--rw-r--r--   0        0        0     2963 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1/pyproject.toml
--rw-r--r--   0        0        0     4870 1970-01-01 00:00:00.000000 apache_airflow_providers_http-4.9.1/PKG-INFO
+-rw-r--r--   0        0        0     3160 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/LICENSE
+-rw-r--r--   0        0        0     1579 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/__init__.py
+-rw-r--r--   0        0        0     3545 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/hooks/__init__.py
+-rw-r--r--   0        0        0    18315 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/hooks/http.py
+-rw-r--r--   0        0        0      787 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/operators/__init__.py
+-rw-r--r--   0        0        0    17549 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/operators/http.py
+-rw-r--r--   0        0        0      787 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/sensors/__init__.py
+-rw-r--r--   0        0        0     8109 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/sensors/http.py
+-rw-r--r--   0        0        0      787 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/triggers/__init__.py
+-rw-r--r--   0        0        0     7702 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/triggers/http.py
+-rw-r--r--   0        0        0     2972 2024-02-11 07:26:47.000000 apache_airflow_providers_http-4.9.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4882 1970-01-01 00:00:00.000000 apache_airflow_providers_http-4.9.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_http-4.9.1/README.rst` & `apache_airflow_providers_http-4.9.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.9.1``
+Release: ``4.9.1.rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/LICENSE` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/__init__.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/get_provider_info.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/hooks/__init__.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/hooks/http.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/hooks/http.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/operators/__init__.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/operators/http.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/operators/http.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/sensors/__init__.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/sensors/http.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/sensors/http.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/triggers/__init__.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/airflow/providers/http/triggers/http.py` & `apache_airflow_providers_http-4.9.1rc1/airflow/providers/http/triggers/http.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_http-4.9.1/pyproject.toml` & `apache_airflow_providers_http-4.9.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-http"
-version = "4.9.1"
+version = "4.9.1.rc1"
 description = "Provider package apache-airflow-providers-http for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,15 +52,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
     "aiohttp>=3.9.2",
-    "apache-airflow>=2.6.0",
+    "apache-airflow>=2.6.0.dev0",
     "asgiref",
     "requests>=2.27.0,<3",
     "requests_toolbelt",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-http/4.9.1"
```

### Comparing `apache_airflow_providers_http-4.9.1/PKG-INFO` & `apache_airflow_providers_http-4.9.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.9.1
+Version: 4.9.1rc1
 Summary: Provider package apache-airflow-providers-http for Apache Airflow
 Keywords: airflow-provider,http,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: aiohttp>=3.9.2
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow>=2.6.0.dev0
 Requires-Dist: asgiref
 Requires-Dist: requests>=2.27.0,<3
 Requires-Dist: requests_toolbelt
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-http/4.9.1/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.9.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
@@ -73,15 +73,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.9.1``
+Release: ``4.9.1.rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

