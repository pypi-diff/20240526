# Comparing `tmp/apache_airflow_providers_common_sql-1.9.0.tar.gz` & `tmp/apache_airflow_providers_common_sql-1.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_common_sql-1.9.0.tar", last modified: Thu Dec  7 21:09:30 2023, max compression
+gzip compressed data, was "apache_airflow_providers_common_sql-1.9.0rc1.tar", last modified: Thu Dec  7 21:09:30 2023, max compression
```

## Comparing `apache_airflow_providers_common_sql-1.9.0.tar` & `apache_airflow_providers_common_sql-1.9.0rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4141 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/README.rst
--rw-r--r--   0        0        0    13569 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/LICENSE
--rw-r--r--   0        0        0     5932 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/README_API.md
--rw-r--r--   0        0        0     1585 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/__init__.py
--rw-r--r--   0        0        0     1675 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/doc/adr/0001-record-architecture-decisions.md
--rw-r--r--   0        0        0     8457 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/doc/adr/0002-return-common-data-structure-from-dbapihook-derived-hooks.md
--rw-r--r--   0        0        0     2837 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/get_provider_info.py
--rw-r--r--   0        0        0      785 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/hooks/__init__.py
--rw-r--r--   0        0        0    25069 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/hooks/sql.py
--rw-r--r--   0        0        0     4072 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/hooks/sql.pyi
--rw-r--r--   0        0        0      785 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0        0        0    47142 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/operators/sql.py
--rw-r--r--   0        0        0     7769 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/operators/sql.pyi
--rw-r--r--   0        0        0      785 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/sensors/__init__.py
--rw-r--r--   0        0        0     5669 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/sensors/sql.py
--rw-r--r--   0        0        0     2295 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/sensors/sql.pyi
--rw-r--r--   0        0        0     3072 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     5973 1970-01-01 00:00:00.000000 apache_airflow_providers_common_sql-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     4145 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/LICENSE
+-rw-r--r--   0        0        0     5932 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/README_API.md
+-rw-r--r--   0        0        0     1585 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0        0        0     1675 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/doc/adr/0001-record-architecture-decisions.md
+-rw-r--r--   0        0        0     8457 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/doc/adr/0002-return-common-data-structure-from-dbapihook-derived-hooks.md
+-rw-r--r--   0        0        0     2837 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/get_provider_info.py
+-rw-r--r--   0        0        0      785 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/hooks/__init__.py
+-rw-r--r--   0        0        0    25069 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/hooks/sql.py
+-rw-r--r--   0        0        0     4072 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/hooks/sql.pyi
+-rw-r--r--   0        0        0      785 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0        0        0    47142 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/operators/sql.py
+-rw-r--r--   0        0        0     7769 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/operators/sql.pyi
+-rw-r--r--   0        0        0      785 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/sensors/__init__.py
+-rw-r--r--   0        0        0     5669 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/sensors/sql.py
+-rw-r--r--   0        0        0     2295 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/sensors/sql.pyi
+-rw-r--r--   0        0        0     3081 2023-12-07 21:09:30.000000 apache_airflow_providers_common_sql-1.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5985 1970-01-01 00:00:00.000000 apache_airflow_providers_common_sql-1.9.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_common_sql-1.9.0/README.rst` & `apache_airflow_providers_common_sql-1.9.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.9.0``
+Release: ``1.9.0.rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/LICENSE` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/README_API.md` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/README_API.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/__init__.py` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/doc/adr/0001-record-architecture-decisions.md` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/doc/adr/0001-record-architecture-decisions.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/doc/adr/0002-return-common-data-structure-from-dbapihook-derived-hooks.md` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/doc/adr/0002-return-common-data-structure-from-dbapihook-derived-hooks.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/get_provider_info.py` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/hooks/__init__.py` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/hooks/sql.py` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/hooks/sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/hooks/sql.pyi` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/hooks/sql.pyi`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/operators/__init__.py` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/operators/sql.py` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/operators/sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/operators/sql.pyi` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/operators/sql.pyi`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/sensors/__init__.py` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/sensors/sql.py` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/airflow/providers/common/sql/sensors/sql.pyi` & `apache_airflow_providers_common_sql-1.9.0rc1/airflow/providers/common/sql/sensors/sql.pyi`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_common_sql-1.9.0/pyproject.toml` & `apache_airflow_providers_common_sql-1.9.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-common-sql"
-version = "1.9.0"
+version = "1.9.0.rc1"
 description = "Provider package apache-airflow-providers-common-sql for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -51,15 +51,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0",
+    "apache-airflow>=2.6.0.dev0",
     "sqlparse>=0.4.2",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.9.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.9.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
```

### Comparing `apache_airflow_providers_common_sql-1.9.0/PKG-INFO` & `apache_airflow_providers_common_sql-1.9.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.9.0
+Version: 1.9.0rc1
 Summary: Provider package apache-airflow-providers-common-sql for Apache Airflow
 Keywords: airflow-provider,common.sql,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow>=2.6.0.dev0
 Requires-Dist: sqlparse>=0.4.2
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Requires-Dist: pandas>=0.17.1 ; extra == "pandas"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.9.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.9.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
@@ -74,15 +74,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.9.0``
+Release: ``1.9.0.rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
```

