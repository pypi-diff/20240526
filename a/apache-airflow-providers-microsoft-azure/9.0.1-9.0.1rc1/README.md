# Comparing `tmp/apache_airflow_providers_microsoft_azure-9.0.1.tar.gz` & `tmp/apache_airflow_providers_microsoft_azure-9.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_microsoft_azure-9.0.1.tar", last modified: Mon Mar  4 12:37:32 2024, max compression
+gzip compressed data, was "apache_airflow_providers_microsoft_azure-9.0.1rc1.tar", last modified: Mon Mar  4 12:37:32 2024, max compression
```

## Comparing `apache_airflow_providers_microsoft_azure-9.0.1.tar` & `apache_airflow_providers_microsoft_azure-9.0.1rc1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     5269 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/README.rst
--rw-r--r--   0        0        0    13569 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/LICENSE
--rw-r--r--   0        0        0     1590 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/__init__.py
--rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/fs/__init__.py
--rw-r--r--   0        0        0     1697 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/fs/adls.py
--rw-r--r--   0        0        0    18925 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/__init__.py
--rw-r--r--   0        0        0     9999 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/adx.py
--rw-r--r--   0        0        0    14429 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/asb.py
--rw-r--r--   0        0        0     6283 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/base_azure.py
--rw-r--r--   0        0        0    16114 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/batch.py
--rw-r--r--   0        0        0     9015 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/container_instance.py
--rw-r--r--   0        0        0     4854 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/container_registry.py
--rw-r--r--   0        0        0     5758 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/container_volume.py
--rw-r--r--   0        0        0    16637 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/cosmos.py
--rw-r--r--   0        0        0    45554 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/data_factory.py
--rw-r--r--   0        0        0    23580 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/data_lake.py
--rw-r--r--   0        0        0    10884 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/fileshare.py
--rw-r--r--   0        0        0    14730 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/synapse.py
--rw-r--r--   0        0        0    31121 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/wasb.py
--rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/log/__init__.py
--rw-r--r--   0        0        0     9910 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
--rw-r--r--   0        0        0      787 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/__init__.py
--rw-r--r--   0        0        0     3790 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/adls.py
--rw-r--r--   0        0        0     3406 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/adx.py
--rw-r--r--   0        0        0    29415 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/asb.py
--rw-r--r--   0        0        0    16538 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/batch.py
--rw-r--r--   0        0        0    15731 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/container_instances.py
--rw-r--r--   0        0        0     2782 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/cosmos.py
--rw-r--r--   0        0        0    12441 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/data_factory.py
--rw-r--r--   0        0        0    12379 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/synapse.py
--rw-r--r--   0        0        0     2687 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
--rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/secrets/__init__.py
--rw-r--r--   0        0        0     9666 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/secrets/key_vault.py
--rw-r--r--   0        0        0      787 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/sensors/__init__.py
--rw-r--r--   0        0        0     2637 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/sensors/cosmos.py
--rw-r--r--   0        0        0     5552 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/sensors/data_factory.py
--rw-r--r--   0        0        0     9043 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/sensors/wasb.py
--rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/__init__.py
--rw-r--r--   0        0        0     1628 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
--rw-r--r--   0        0        0     4176 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
--rw-r--r--   0        0        0     2936 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
--rw-r--r--   0        0        0     4468 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
--rw-r--r--   0        0        0     8194 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
--rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/triggers/__init__.py
--rw-r--r--   0        0        0    11128 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/triggers/data_factory.py
--rw-r--r--   0        0        0     7367 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/triggers/wasb.py
--rw-r--r--   0        0        0     7187 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/utils.py
--rw-r--r--   0        0        0     3835 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1/pyproject.toml
--rw-r--r--   0        0        0     8043 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_azure-9.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5273 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/LICENSE
+-rw-r--r--   0        0        0     1590 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/__init__.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/fs/__init__.py
+-rw-r--r--   0        0        0     1697 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/fs/adls.py
+-rw-r--r--   0        0        0    18925 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py
+-rw-r--r--   0        0        0     9999 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/adx.py
+-rw-r--r--   0        0        0    14429 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/asb.py
+-rw-r--r--   0        0        0     6283 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py
+-rw-r--r--   0        0        0    16114 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/batch.py
+-rw-r--r--   0        0        0     9015 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py
+-rw-r--r--   0        0        0     4854 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py
+-rw-r--r--   0        0        0     5758 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py
+-rw-r--r--   0        0        0    16637 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py
+-rw-r--r--   0        0        0    45554 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py
+-rw-r--r--   0        0        0    23580 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py
+-rw-r--r--   0        0        0    10884 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py
+-rw-r--r--   0        0        0    14730 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py
+-rw-r--r--   0        0        0    31121 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/log/__init__.py
+-rw-r--r--   0        0        0     9910 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py
+-rw-r--r--   0        0        0      787 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/__init__.py
+-rw-r--r--   0        0        0     3790 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/adls.py
+-rw-r--r--   0        0        0     3406 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/adx.py
+-rw-r--r--   0        0        0    29415 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/asb.py
+-rw-r--r--   0        0        0    16538 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/batch.py
+-rw-r--r--   0        0        0    15731 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py
+-rw-r--r--   0        0        0     2782 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py
+-rw-r--r--   0        0        0    12441 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py
+-rw-r--r--   0        0        0    12379 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/synapse.py
+-rw-r--r--   0        0        0     2687 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py
+-rw-r--r--   0        0        0     9666 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py
+-rw-r--r--   0        0        0      787 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py
+-rw-r--r--   0        0        0     2637 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py
+-rw-r--r--   0        0        0     5552 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py
+-rw-r--r--   0        0        0     9043 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py
+-rw-r--r--   0        0        0     1628 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py
+-rw-r--r--   0        0        0     4176 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py
+-rw-r--r--   0        0        0     2936 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py
+-rw-r--r--   0        0        0     4468 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py
+-rw-r--r--   0        0        0     8194 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py
+-rw-r--r--   0        0        0      785 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py
+-rw-r--r--   0        0        0    11128 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py
+-rw-r--r--   0        0        0     7367 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py
+-rw-r--r--   0        0        0     7187 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/utils.py
+-rw-r--r--   0        0        0     3844 2024-03-04 12:37:32.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     8055 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_azure-9.0.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/README.rst` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``9.0.1``
+Release: ``9.0.1.rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/LICENSE` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/__init__.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/fs/__init__.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/fs/adls.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/fs/adls.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/get_provider_info.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/__init__.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/adx.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/adx.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/asb.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/asb.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/base_azure.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/base_azure.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/batch.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/batch.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/container_instance.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/container_instance.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/container_registry.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/container_registry.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/container_volume.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/container_volume.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/cosmos.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/data_factory.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/data_lake.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/data_lake.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/fileshare.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/fileshare.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/synapse.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/synapse.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/hooks/wasb.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/hooks/wasb.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/log/__init__.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/log/wasb_task_handler.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/log/wasb_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/__init__.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/adls.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/adls.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/adx.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/adx.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/asb.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/asb.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/batch.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/container_instances.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/container_instances.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/cosmos.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/data_factory.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/synapse.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/synapse.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/operators/wasb_delete_blob.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/secrets/__init__.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/secrets/key_vault.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/secrets/key_vault.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/sensors/__init__.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/sensors/cosmos.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/sensors/cosmos.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/sensors/data_factory.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/sensors/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/sensors/wasb.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/sensors/wasb.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/__init__.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/azure_blob_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/local_to_adls.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/local_to_adls.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/local_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/oracle_to_azure_data_lake.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/transfers/sftp_to_wasb.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/triggers/__init__.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/triggers/data_factory.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/triggers/data_factory.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/triggers/wasb.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/triggers/wasb.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/airflow/providers/microsoft/azure/utils.py` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/airflow/providers/microsoft/azure/utils.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/pyproject.toml` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-microsoft-azure"
-version = "9.0.1"
+version = "9.0.1.rc1"
 description = "Provider package apache-airflow-providers-microsoft-azure for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -53,15 +53,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
     "adal>=1.2.7",
     "adlfs>=2023.10.0",
-    "apache-airflow>=2.6.0",
+    "apache-airflow>=2.6.0.dev0",
     "azure-batch>=8.0.0",
     "azure-cosmos>=4.0.0",
     "azure-datalake-store>=0.0.45",
     "azure-identity>=1.3.1",
     "azure-keyvault-secrets>=4.1.0",
     "azure-kusto-data>=4.1.0",
     "azure-mgmt-containerinstance>=9.0.0",
```

### Comparing `apache_airflow_providers_microsoft_azure-9.0.1/PKG-INFO` & `apache_airflow_providers_microsoft_azure-9.0.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-azure
-Version: 9.0.1
+Version: 9.0.1rc1
 Summary: Provider package apache-airflow-providers-microsoft-azure for Apache Airflow
 Keywords: airflow-provider,microsoft.azure,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: adal>=1.2.7
 Requires-Dist: adlfs>=2023.10.0
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow>=2.6.0.dev0
 Requires-Dist: azure-batch>=8.0.0
 Requires-Dist: azure-cosmos>=4.0.0
 Requires-Dist: azure-datalake-store>=0.0.45
 Requires-Dist: azure-identity>=1.3.1
 Requires-Dist: azure-keyvault-secrets>=4.1.0
 Requires-Dist: azure-kusto-data>=4.1.0
 Requires-Dist: azure-mgmt-containerinstance>=9.0.0
@@ -96,15 +96,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-azure``
 
-Release: ``9.0.1``
+Release: ``9.0.1.rc1``
 
 
 `Microsoft Azure <https://azure.microsoft.com/>`__
 
 
 Provider package
 ----------------
```

