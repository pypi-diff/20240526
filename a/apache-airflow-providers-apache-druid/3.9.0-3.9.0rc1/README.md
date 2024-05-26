# Comparing `tmp/apache_airflow_providers_apache_druid-3.9.0.tar.gz` & `tmp/apache_airflow_providers_apache_druid-3.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_apache_druid-3.9.0.tar", last modified: Mon Mar  4 12:20:43 2024, max compression
+gzip compressed data, was "apache_airflow_providers_apache_druid-3.9.0rc1.tar", last modified: Mon Mar  4 12:20:43 2024, max compression
```

## Comparing `apache_airflow_providers_apache_druid-3.9.0.tar` & `apache_airflow_providers_apache_druid-3.9.0rc1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4447 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/README.rst
--rw-r--r--   0        0        0    13569 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/LICENSE
--rw-r--r--   0        0        0     1587 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/__init__.py
--rw-r--r--   0        0        0     3460 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/hooks/__init__.py
--rw-r--r--   0        0        0     8801 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/hooks/druid.py
--rw-r--r--   0        0        0      787 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/operators/__init__.py
--rw-r--r--   0        0        0     3086 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/operators/druid.py
--rw-r--r--   0        0        0     1476 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/operators/druid_check.py
--rw-r--r--   0        0        0      785 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/transfers/__init__.py
--rw-r--r--   0        0        0    10080 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/transfers/hive_to_druid.py
--rw-r--r--   0        0        0     3160 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_druid-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     4451 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/LICENSE
+-rw-r--r--   0        0        0     1587 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/__init__.py
+-rw-r--r--   0        0        0     3460 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/hooks/__init__.py
+-rw-r--r--   0        0        0     8801 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/hooks/druid.py
+-rw-r--r--   0        0        0      787 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/operators/__init__.py
+-rw-r--r--   0        0        0     3086 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/operators/druid.py
+-rw-r--r--   0        0        0     1476 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/operators/druid_check.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/transfers/__init__.py
+-rw-r--r--   0        0        0    10080 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/transfers/hive_to_druid.py
+-rw-r--r--   0        0        0     3174 2024-03-04 12:20:43.000000 apache_airflow_providers_apache_druid-3.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6392 1970-01-01 00:00:00.000000 apache_airflow_providers_apache_druid-3.9.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_apache_druid-3.9.0/README.rst` & `apache_airflow_providers_apache_druid-3.9.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.9.0``
+Release: ``3.9.0.rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/LICENSE` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/__init__.py` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/get_provider_info.py` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/hooks/__init__.py` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/hooks/druid.py` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/hooks/druid.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/operators/__init__.py` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/operators/druid.py` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/operators/druid.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/operators/druid_check.py` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/operators/druid_check.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/transfers/__init__.py` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/airflow/providers/apache/druid/transfers/hive_to_druid.py` & `apache_airflow_providers_apache_druid-3.9.0rc1/airflow/providers/apache/druid/transfers/hive_to_druid.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_apache_druid-3.9.0/pyproject.toml` & `apache_airflow_providers_apache_druid-3.9.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-apache-druid"
-version = "3.9.0"
+version = "3.9.0.rc1"
 description = "Provider package apache-airflow-providers-apache-druid for Apache Airflow"
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
     "pydruid>=0.4.1",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.9.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.9.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_apache_druid-3.9.0/PKG-INFO` & `apache_airflow_providers_apache_druid-3.9.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-druid
-Version: 3.9.0
+Version: 3.9.0rc1
 Summary: Provider package apache-airflow-providers-apache-druid for Apache Airflow
 Keywords: airflow-provider,apache.druid,airflow,integration
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
 Requires-Dist: pydruid>=0.4.1
 Requires-Dist: apache-airflow-providers-apache-hive ; extra == "apache.hive"
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.9.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.9.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
@@ -75,15 +75,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.9.0``
+Release: ``3.9.0.rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
```

