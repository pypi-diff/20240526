# Comparing `tmp/apache_airflow_providers_postgres-5.9.0.tar.gz` & `tmp/apache_airflow_providers_postgres-5.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_postgres-5.9.0.tar", last modified: Thu Dec  7 21:10:09 2023, max compression
+gzip compressed data, was "apache_airflow_providers_postgres-5.9.0rc1.tar", last modified: Thu Dec  7 21:10:09 2023, max compression
```

## Comparing `apache_airflow_providers_postgres-5.9.0.tar` & `apache_airflow_providers_postgres-5.9.0rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4536 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0/README.rst
--rw-r--r--   0        0        0    13569 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/LICENSE
--rw-r--r--   0        0        0     1583 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/__init__.py
--rw-r--r--   0        0        0     3294 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/get_provider_info.py
--rw-r--r--   0        0        0      787 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/hooks/__init__.py
--rw-r--r--   0        0        0    15703 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/hooks/postgres.py
--rw-r--r--   0        0        0      787 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/operators/__init__.py
--rw-r--r--   0        0        0     3544 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/operators/postgres.py
--rw-r--r--   0        0        0     3201 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0/pyproject.toml
--rw-r--r--   0        0        0     6549 1970-01-01 00:00:00.000000 apache_airflow_providers_postgres-5.9.0/PKG-INFO
+-rw-r--r--   0        0        0     4540 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/LICENSE
+-rw-r--r--   0        0        0     1583 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/__init__.py
+-rw-r--r--   0        0        0     3294 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/get_provider_info.py
+-rw-r--r--   0        0        0      787 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/hooks/__init__.py
+-rw-r--r--   0        0        0    15703 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/hooks/postgres.py
+-rw-r--r--   0        0        0      787 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/operators/__init__.py
+-rw-r--r--   0        0        0     3544 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/operators/postgres.py
+-rw-r--r--   0        0        0     3215 2023-12-07 21:10:09.000000 apache_airflow_providers_postgres-5.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6566 1970-01-01 00:00:00.000000 apache_airflow_providers_postgres-5.9.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_postgres-5.9.0/README.rst` & `apache_airflow_providers_postgres-5.9.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.9.0``
+Release: ``5.9.0.rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/LICENSE` & `apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/__init__.py` & `apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/get_provider_info.py` & `apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/hooks/__init__.py` & `apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/hooks/postgres.py` & `apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/operators/__init__.py` & `apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_postgres-5.9.0/airflow/providers/postgres/operators/postgres.py` & `apache_airflow_providers_postgres-5.9.0rc1/airflow/providers/postgres/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_postgres-5.9.0/pyproject.toml` & `apache_airflow_providers_postgres-5.9.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-postgres"
-version = "5.9.0"
+version = "5.9.0.rc1"
 description = "Provider package apache-airflow-providers-postgres for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -51,16 +51,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow-providers-common-sql>=1.3.1",
-    "apache-airflow>=2.6.0",
+    "apache-airflow-providers-common-sql>=1.3.1.dev0",
+    "apache-airflow>=2.6.0.dev0",
     "psycopg2-binary>=2.8.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.9.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.9.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_postgres-5.9.0/PKG-INFO` & `apache_airflow_providers_postgres-5.9.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.9.0
+Version: 5.9.0rc1
 Summary: Provider package apache-airflow-providers-postgres for Apache Airflow
 Keywords: airflow-provider,postgres,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,16 +16,16 @@
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-common-sql>=1.3.1
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow-providers-common-sql>=1.3.1.dev0
+Requires-Dist: apache-airflow>=2.6.0.dev0
 Requires-Dist: psycopg2-binary>=2.8.0
 Requires-Dist: apache-airflow-providers-amazon>=2.6.0 ; extra == "amazon"
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.9.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.9.0
@@ -77,15 +77,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.9.0``
+Release: ``5.9.0.rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

