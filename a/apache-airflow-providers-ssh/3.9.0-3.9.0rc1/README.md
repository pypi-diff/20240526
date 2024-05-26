# Comparing `tmp/apache_airflow_providers_ssh-3.9.0.tar.gz` & `tmp/apache_airflow_providers_ssh-3.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_ssh-3.9.0.tar", last modified: Thu Dec  7 21:10:23 2023, max compression
+gzip compressed data, was "apache_airflow_providers_ssh-3.9.0rc1.tar", last modified: Thu Dec  7 21:10:23 2023, max compression
```

## Comparing `apache_airflow_providers_ssh-3.9.0.tar` & `apache_airflow_providers_ssh-3.9.0rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3081 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0/README.rst
--rw-r--r--   0        0        0    13569 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/LICENSE
--rw-r--r--   0        0        0     1578 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/__init__.py
--rw-r--r--   0        0        0     2815 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/get_provider_info.py
--rw-r--r--   0        0        0      787 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/hooks/__init__.py
--rw-r--r--   0        0        0    22644 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/hooks/ssh.py
--rw-r--r--   0        0        0      787 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/operators/__init__.py
--rw-r--r--   0        0        0     7929 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/operators/ssh.py
--rw-r--r--   0        0        0     2914 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     4732 1970-01-01 00:00:00.000000 apache_airflow_providers_ssh-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3085 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/LICENSE
+-rw-r--r--   0        0        0     1578 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/__init__.py
+-rw-r--r--   0        0        0     2815 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/get_provider_info.py
+-rw-r--r--   0        0        0      787 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/hooks/__init__.py
+-rw-r--r--   0        0        0    22644 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/hooks/ssh.py
+-rw-r--r--   0        0        0      787 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/operators/__init__.py
+-rw-r--r--   0        0        0     7929 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/operators/ssh.py
+-rw-r--r--   0        0        0     2923 2023-12-07 21:10:23.000000 apache_airflow_providers_ssh-3.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4744 1970-01-01 00:00:00.000000 apache_airflow_providers_ssh-3.9.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_ssh-3.9.0/README.rst` & `apache_airflow_providers_ssh-3.9.0rc1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-ssh``
 
-Release: ``3.9.0``
+Release: ``3.9.0.rc1``
 
 
 `Secure Shell (SSH) <https://tools.ietf.org/html/rfc4251>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/LICENSE` & `apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/__init__.py` & `apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/get_provider_info.py` & `apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/hooks/__init__.py` & `apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/hooks/ssh.py` & `apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/hooks/ssh.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/operators/__init__.py` & `apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ssh-3.9.0/airflow/providers/ssh/operators/ssh.py` & `apache_airflow_providers_ssh-3.9.0rc1/airflow/providers/ssh/operators/ssh.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_ssh-3.9.0/pyproject.toml` & `apache_airflow_providers_ssh-3.9.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-ssh"
-version = "3.9.0"
+version = "3.9.0.rc1"
 description = "Provider package apache-airflow-providers-ssh for Apache Airflow"
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
     "paramiko>=2.6.0",
     "sshtunnel>=0.3.2",
 ]
 
 [project.urls]
 "Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-ssh/3.9.0"
 "Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-ssh/3.9.0/changelog.html"
```

### Comparing `apache_airflow_providers_ssh-3.9.0/PKG-INFO` & `apache_airflow_providers_ssh-3.9.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ssh
-Version: 3.9.0
+Version: 3.9.0rc1
 Summary: Provider package apache-airflow-providers-ssh for Apache Airflow
 Keywords: airflow-provider,ssh,airflow,integration
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
 Requires-Dist: paramiko>=2.6.0
 Requires-Dist: sshtunnel>=0.3.2
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-ssh/3.9.0/changelog.html
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ssh/3.9.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
@@ -71,15 +71,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-ssh``
 
-Release: ``3.9.0``
+Release: ``3.9.0.rc1``
 
 
 `Secure Shell (SSH) <https://tools.ietf.org/html/rfc4251>`__
 
 
 Provider package
 ----------------
```

