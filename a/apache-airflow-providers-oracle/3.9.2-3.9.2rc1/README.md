# Comparing `tmp/apache_airflow_providers_oracle-3.9.2.tar.gz` & `tmp/apache_airflow_providers_oracle-3.9.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_oracle-3.9.2.tar", last modified: Sun Feb 11 07:27:52 2024, max compression
+gzip compressed data, was "apache_airflow_providers_oracle-3.9.2rc1.tar", last modified: Sun Feb 11 07:27:52 2024, max compression
```

## Comparing `apache_airflow_providers_oracle-3.9.2.tar` & `apache_airflow_providers_oracle-3.9.2rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4266 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/README.rst
--rw-r--r--   0        0        0    13569 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/LICENSE
--rw-r--r--   0        0        0     1581 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/__init__.py
--rw-r--r--   0        0        0      785 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/example_dags/__init__.py
--rw-r--r--   0        0        0     2192 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/example_dags/example_oracle.py
--rw-r--r--   0        0        0     3186 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/hooks/__init__.py
--rw-r--r--   0        0        0    17367 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/hooks/oracle.py
--rw-r--r--   0        0        0      787 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/operators/__init__.py
--rw-r--r--   0        0        0     4167 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/operators/oracle.py
--rw-r--r--   0        0        0      785 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/transfers/__init__.py
--rw-r--r--   0        0        0     3569 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/transfers/oracle_to_oracle.py
--rw-r--r--   0        0        0     3082 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2/pyproject.toml
--rw-r--r--   0        0        0     6122 1970-01-01 00:00:00.000000 apache_airflow_providers_oracle-3.9.2/PKG-INFO
+-rw-r--r--   0        0        0     4270 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/LICENSE
+-rw-r--r--   0        0        0     1581 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/__init__.py
+-rw-r--r--   0        0        0      785 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/example_dags/__init__.py
+-rw-r--r--   0        0        0     2192 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/example_dags/example_oracle.py
+-rw-r--r--   0        0        0     3186 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/hooks/__init__.py
+-rw-r--r--   0        0        0    17367 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/hooks/oracle.py
+-rw-r--r--   0        0        0      787 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/operators/__init__.py
+-rw-r--r--   0        0        0     4167 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/operators/oracle.py
+-rw-r--r--   0        0        0      785 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/transfers/__init__.py
+-rw-r--r--   0        0        0     3569 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py
+-rw-r--r--   0        0        0     3096 2024-02-11 07:27:52.000000 apache_airflow_providers_oracle-3.9.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     6139 1970-01-01 00:00:00.000000 apache_airflow_providers_oracle-3.9.2rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_oracle-3.9.2/README.rst` & `apache_airflow_providers_oracle-3.9.2rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.9.2``
+Release: ``3.9.2.rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/LICENSE` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/__init__.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/example_dags/__init__.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/example_dags/example_oracle.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/example_dags/example_oracle.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/get_provider_info.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/hooks/__init__.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/hooks/oracle.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/hooks/oracle.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/operators/__init__.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/operators/oracle.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/operators/oracle.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/transfers/__init__.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/airflow/providers/oracle/transfers/oracle_to_oracle.py` & `apache_airflow_providers_oracle-3.9.2rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_oracle-3.9.2/pyproject.toml` & `apache_airflow_providers_oracle-3.9.2rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-oracle"
-version = "3.9.2"
+version = "3.9.2.rc1"
 description = "Provider package apache-airflow-providers-oracle for Apache Airflow"
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
     "oracledb>=1.0.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.9.2"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.9.2/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_oracle-3.9.2/PKG-INFO` & `apache_airflow_providers_oracle-3.9.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-oracle
-Version: 3.9.2
+Version: 3.9.2rc1
 Summary: Provider package apache-airflow-providers-oracle for Apache Airflow
 Keywords: airflow-provider,oracle,airflow,integration
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
 Requires-Dist: oracledb>=1.0.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Requires-Dist: numpy ; extra == "numpy"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.9.2/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.9.2
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
@@ -75,15 +75,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.9.2``
+Release: ``3.9.2.rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
```

