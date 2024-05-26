# Comparing `tmp/apache_airflow_providers_sftp-4.9.1.tar.gz` & `tmp/apache_airflow_providers_sftp-4.9.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_sftp-4.9.1.tar", last modified: Tue Apr  9 12:40:52 2024, max compression
+gzip compressed data, was "apache_airflow_providers_sftp-4.9.1rc1.tar", last modified: Tue Apr  9 12:40:52 2024, max compression
```

## Comparing `apache_airflow_providers_sftp-4.9.1.tar` & `apache_airflow_providers_sftp-4.9.1rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4440 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/LICENSE
--rw-r--r--   0        0        0     1579 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/__init__.py
--rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/decorators/__init__.py
--rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/decorators/sensors/__init__.py
--rw-r--r--   0        0        0     2861 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/decorators/sensors/sftp.py
--rw-r--r--   0        0        0     3933 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/hooks/__init__.py
--rw-r--r--   0        0        0    21856 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/hooks/sftp.py
--rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/operators/__init__.py
--rw-r--r--   0        0        0    11508 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/operators/sftp.py
--rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/sensors/__init__.py
--rw-r--r--   0        0        0     7382 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/sensors/sftp.py
--rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/triggers/__init__.py
--rw-r--r--   0        0        0     6155 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/triggers/sftp.py
--rw-r--r--   0        0        0     3154 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1/pyproject.toml
--rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 apache_airflow_providers_sftp-4.9.1/PKG-INFO
+-rw-r--r--   0        0        0     4444 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/LICENSE
+-rw-r--r--   0        0        0     1579 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/sensors/__init__.py
+-rw-r--r--   0        0        0     2861 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/sensors/sftp.py
+-rw-r--r--   0        0        0     3933 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/hooks/__init__.py
+-rw-r--r--   0        0        0    21856 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/hooks/sftp.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/operators/__init__.py
+-rw-r--r--   0        0        0    11508 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/operators/sftp.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/sensors/__init__.py
+-rw-r--r--   0        0        0     7382 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/sensors/sftp.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/triggers/__init__.py
+-rw-r--r--   0        0        0     6155 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/triggers/sftp.py
+-rw-r--r--   0        0        0     3164 2024-04-09 12:40:52.000000 apache_airflow_providers_sftp-4.9.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     6397 1970-01-01 00:00:00.000000 apache_airflow_providers_sftp-4.9.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_sftp-4.9.1/README.rst` & `apache_airflow_providers_sftp-4.9.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.9.1``
+Release: ``4.9.1.rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/LICENSE` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/decorators/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/decorators/sensors/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/decorators/sensors/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/decorators/sensors/sftp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/get_provider_info.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/hooks/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/hooks/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/hooks/sftp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/operators/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/operators/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/operators/sftp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/sensors/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/sensors/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/sensors/sftp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/triggers/__init__.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/airflow/providers/sftp/triggers/sftp.py` & `apache_airflow_providers_sftp-4.9.1rc1/airflow/providers/sftp/triggers/sftp.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_sftp-4.9.1/pyproject.toml` & `apache_airflow_providers_sftp-4.9.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-sftp"
-version = "4.9.1"
+version = "4.9.1.rc1"
 description = "Provider package apache-airflow-providers-sftp for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -52,16 +52,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow-providers-ssh>=2.1.0",
-    "apache-airflow>=2.6.0",
+    "apache-airflow-providers-ssh>=2.1.0rc0",
+    "apache-airflow>=2.6.0rc0",
     "asyncssh>=2.12.0",
     "paramiko>=2.8.0",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1/changelog.html"
```

### Comparing `apache_airflow_providers_sftp-4.9.1/PKG-INFO` & `apache_airflow_providers_sftp-4.9.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sftp
-Version: 4.9.1
+Version: 4.9.1rc1
 Summary: Provider package apache-airflow-providers-sftp for Apache Airflow
 Keywords: airflow-provider,sftp,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,16 +17,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow-providers-ssh>=2.1.0
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow-providers-ssh>=2.1.0rc0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: asyncssh>=2.12.0
 Requires-Dist: paramiko>=2.8.0
 Requires-Dist: apache-airflow-providers-openlineage ; extra == "openlineage"
 Requires-Dist: apache-airflow-providers-ssh ; extra == "ssh"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.9.1
@@ -77,15 +77,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.9.1``
+Release: ``4.9.1.rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
```

