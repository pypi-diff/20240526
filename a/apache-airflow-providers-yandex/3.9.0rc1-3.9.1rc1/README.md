# Comparing `tmp/apache_airflow_providers_yandex-3.9.0rc1.tar.gz` & `tmp/apache_airflow_providers_yandex-3.9.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_yandex-3.9.0rc1.tar", last modified: Sun Feb 11 07:29:22 2024, max compression
+gzip compressed data, was "apache_airflow_providers_yandex-3.9.1rc1.tar", last modified: Tue Apr  9 12:43:01 2024, max compression
```

## Comparing `apache_airflow_providers_yandex-3.9.0rc1.tar` & `apache_airflow_providers_yandex-3.9.1rc1.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0     3103 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/LICENSE
--rw-r--r--   0        0        0     1581 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/__init__.py
--rw-r--r--   0        0        0     3930 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/hooks/__init__.py
--rw-r--r--   0        0        0     7074 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/hooks/yandex.py
--rw-r--r--   0        0        0     1379 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/hooks/yandexcloud_dataproc.py
--rw-r--r--   0        0        0      785 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/operators/__init__.py
--rw-r--r--   0        0        0    25956 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/operators/yandexcloud_dataproc.py
--rw-r--r--   0        0        0      785 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/secrets/__init__.py
--rw-r--r--   0        0        0    11689 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/secrets/lockbox.py
--rw-r--r--   0        0        0      785 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/__init__.py
--rw-r--r--   0        0        0     3335 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/credentials.py
--rw-r--r--   0        0        0      950 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/defaults.py
--rw-r--r--   0        0        0     1728 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/fields.py
--rw-r--r--   0        0        0     1839 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/user_agent.py
--rw-r--r--   0        0        0     2925 2024-02-11 07:29:22.000000 apache_airflow_providers_yandex-3.9.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4750 1970-01-01 00:00:00.000000 apache_airflow_providers_yandex-3.9.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3175 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/LICENSE
+-rw-r--r--   0        0        0     1581 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/__init__.py
+-rw-r--r--   0        0        0     4684 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/hooks/__init__.py
+-rw-r--r--   0        0        0     7097 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/hooks/yandex.py
+-rw-r--r--   0        0        0     1379 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/hooks/yandexcloud_dataproc.py
+-rw-r--r--   0        0        0     3978 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/hooks/yq.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/links/__init__.py
+-rw-r--r--   0        0        0     1578 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/links/yq.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/operators/__init__.py
+-rw-r--r--   0        0        0    25957 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/operators/yandexcloud_dataproc.py
+-rw-r--r--   0        0        0     3223 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/operators/yq.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/secrets/__init__.py
+-rw-r--r--   0        0        0    12161 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/secrets/lockbox.py
+-rw-r--r--   0        0        0      785 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/utils/__init__.py
+-rw-r--r--   0        0        0     3335 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/utils/credentials.py
+-rw-r--r--   0        0        0      950 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/utils/defaults.py
+-rw-r--r--   0        0        0     1728 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/utils/fields.py
+-rw-r--r--   0        0        0     1839 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/utils/user_agent.py
+-rw-r--r--   0        0        0     3003 2024-04-09 12:43:01.000000 apache_airflow_providers_yandex-3.9.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 apache_airflow_providers_yandex-3.9.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/README.rst` & `apache_airflow_providers_yandex-3.9.1rc1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -38,45 +38,46 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-yandex``
 
-Release: ``3.9.0.rc1``
+Release: ``3.9.1.rc1``
 
 
 This package is for Yandex, including:
 
     - `Yandex.Cloud <https://cloud.yandex.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``yandex`` provider. All classes for this provider package
 are in ``airflow.providers.yandex`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-yandex``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
-==================  ==================
-PIP package         Version required
-==================  ==================
-``apache-airflow``  ``>=2.6.0``
-``yandexcloud``     ``>=0.228.0``
-==================  ==================
+=======================  ==================
+PIP package              Version required
+=======================  ==================
+``apache-airflow``       ``>=2.6.0``
+``yandexcloud``          ``>=0.228.0``
+``yandex-query-client``  ``>=0.1.2``
+=======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/LICENSE` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/__init__.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.9.0"
+__version__ = "3.9.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/get_provider_info.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/get_provider_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-yandex",
         "name": "Yandex",
         "description": "This package is for Yandex, including:\n\n    - `Yandex.Cloud <https://cloud.yandex.com/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1707636562,
+        "source-date-epoch": 1712666581,
         "versions": [
+            "3.9.1",
             "3.9.0",
             "3.8.0",
             "3.7.1",
             "3.7.0",
             "3.6.0",
             "3.5.0",
             "3.4.0",
@@ -46,50 +47,63 @@
             "2.2.1",
             "2.2.0",
             "2.1.0",
             "2.0.0",
             "1.0.1",
             "1.0.0",
         ],
-        "dependencies": ["apache-airflow>=2.6.0", "yandexcloud>=0.228.0"],
+        "dependencies": ["apache-airflow>=2.6.0", "yandexcloud>=0.228.0", "yandex-query-client>=0.1.2"],
         "integrations": [
             {
                 "integration-name": "Yandex.Cloud",
                 "external-doc-url": "https://cloud.yandex.com/",
                 "logo": "/integration-logos/yandex/Yandex-Cloud.png",
                 "tags": ["service"],
             },
             {
                 "integration-name": "Yandex.Cloud Dataproc",
                 "external-doc-url": "https://cloud.yandex.com/dataproc",
                 "how-to-guide": ["/docs/apache-airflow-providers-yandex/operators.rst"],
                 "logo": "/integration-logos/yandex/Yandex-Cloud.png",
                 "tags": ["service"],
             },
+            {
+                "integration-name": "Yandex.Cloud YQ",
+                "external-doc-url": "https://cloud.yandex.com/en/services/query",
+                "how-to-guide": ["/docs/apache-airflow-providers-yandex/operators.rst"],
+                "logo": "/integration-logos/yandex/Yandex-Cloud.png",
+                "tags": ["service"],
+            },
         ],
         "operators": [
             {
                 "integration-name": "Yandex.Cloud Dataproc",
                 "python-modules": ["airflow.providers.yandex.operators.yandexcloud_dataproc"],
-            }
+            },
+            {
+                "integration-name": "Yandex.Cloud YQ",
+                "python-modules": ["airflow.providers.yandex.operators.yq"],
+            },
         ],
         "hooks": [
             {"integration-name": "Yandex.Cloud", "python-modules": ["airflow.providers.yandex.hooks.yandex"]},
             {
                 "integration-name": "Yandex.Cloud Dataproc",
                 "python-modules": ["airflow.providers.yandex.hooks.yandexcloud_dataproc"],
             },
+            {"integration-name": "Yandex.Cloud YQ", "python-modules": ["airflow.providers.yandex.hooks.yq"]},
         ],
         "connection-types": [
             {
                 "hook-class-name": "airflow.providers.yandex.hooks.yandex.YandexCloudBaseHook",
                 "connection-type": "yandexcloud",
             }
         ],
         "secrets-backends": ["airflow.providers.yandex.secrets.lockbox.LockboxSecretBackend"],
+        "extra-links": ["airflow.providers.yandex.links.yq.YQLink"],
         "config": {
             "yandex": {
                 "description": "This section contains settings for Yandex Cloud integration.",
                 "options": {
                     "sdk_user_agent_prefix": {
                         "description": "Prefix for User-Agent header in Yandex.Cloud SDK requests\n",
                         "version_added": "3.6.0",
```

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/hooks/__init__.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/hooks/yandex.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/hooks/yandex.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,22 +75,22 @@
                 widget=BS3PasswordFieldWidget(),
                 description="User account OAuth token. "
                 "Either this or service account JSON must be specified.",
             ),
             "folder_id": StringField(
                 lazy_gettext("Default folder ID"),
                 widget=BS3TextFieldWidget(),
-                description="Optional. This folder will be used "
-                "to create all new clusters and nodes by default",
+                description="Optional. "
+                "If specified, this ID will be used by default when creating nodes and clusters.",
             ),
             "public_ssh_key": StringField(
                 lazy_gettext("Public SSH key"),
                 widget=BS3TextFieldWidget(),
-                description="Optional. This key will be placed to all created Compute nodes "
-                "to let you have a root shell there",
+                description="Optional. The key will be placed to all created Compute nodes, "
+                "allowing you to have a root shell there.",
             ),
             "endpoint": StringField(
                 lazy_gettext("API endpoint"),
                 widget=BS3TextFieldWidget(),
                 description="Optional. Specify an API endpoint. Leave blank to use default.",
             ),
         }
@@ -128,21 +128,21 @@
                 "Using `connection_id` is deprecated. Please use `yandex_conn_id` parameter.",
                 AirflowProviderDeprecationWarning,
                 stacklevel=2,
             )
         self.connection_id = yandex_conn_id or connection_id or default_conn_name
         self.connection = self.get_connection(self.connection_id)
         self.extras = self.connection.extra_dejson
-        credentials = get_credentials(
+        self.credentials = get_credentials(
             oauth_token=self._get_field("oauth"),
             service_account_json=self._get_field("service_account_json"),
             service_account_json_path=self._get_field("service_account_json_path"),
         )
         sdk_config = self._get_endpoint()
-        self.sdk = yandexcloud.SDK(user_agent=provider_user_agent(), **sdk_config, **credentials)
+        self.sdk = yandexcloud.SDK(user_agent=provider_user_agent(), **sdk_config, **self.credentials)
         self.default_folder_id = default_folder_id or self._get_field("folder_id")
         self.default_public_ssh_key = default_public_ssh_key or self._get_field("public_ssh_key")
         self.default_service_account_id = default_service_account_id or get_service_account_id(
             service_account_json=self._get_field("service_account_json"),
             service_account_json_path=self._get_field("service_account_json_path"),
         )
         self.client = self.sdk.client
```

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/hooks/yandexcloud_dataproc.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/hooks/yandexcloud_dataproc.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/operators/__init__.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/operators/yandexcloud_dataproc.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/operators/yandexcloud_dataproc.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                         Docs: https://cloud.yandex.com/docs/data-proc/concepts/network#security-groups
     :param log_group_id: Id of log group to write logs. By default logs will be sent to default log group.
                     To disable cloud log sending set cluster property dataproc:disable_cloud_logging = true
                     Docs: https://cloud.yandex.com/docs/data-proc/concepts/logs
     :param initialization_actions: Set of init-actions to run when cluster starts.
                         Docs: https://cloud.yandex.com/docs/data-proc/concepts/init-action
     :param labels: Cluster labels as key:value pairs. No more than 64 per resource.
-                        Docs: https://cloud.yandex.ru/docs/resource-manager/concepts/labels
+                        Docs: https://cloud.yandex.com/docs/resource-manager/concepts/labels
     """
 
     def __init__(
         self,
         *,
         folder_id: str | None = None,
         cluster_name: str | None = None,
```

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/secrets/__init__.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/secrets/lockbox.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/secrets/lockbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Objects relating to sourcing secrets from Yandex Cloud Lockbox."""
+
 from __future__ import annotations
 
 from functools import cached_property
 from typing import Any
 
 import yandex.cloud.lockbox.v1.payload_pb2 as payload_pb
 import yandex.cloud.lockbox.v1.payload_service_pb2 as payload_service_pb
@@ -35,15 +36,15 @@
 from airflow.providers.yandex.utils.user_agent import provider_user_agent
 from airflow.secrets import BaseSecretsBackend
 from airflow.utils.log.logging_mixin import LoggingMixin
 
 
 class LockboxSecretBackend(BaseSecretsBackend, LoggingMixin):
     """
-    Retrieves Connection or Variables or Configs from Yandex Lockbox.
+    Retrieves connections or variables or configs from Yandex Lockbox.
 
     Configurable via ``airflow.cfg`` like so:
 
     .. code-block:: ini
 
         [secrets]
         backend = airflow.providers.yandex.secrets.lockbox.LockboxSecretBackend
@@ -56,59 +57,65 @@
     When ``{"variables_prefix": "airflow/variables"}`` is set, if a secret is defined with
     the path ``airflow/variables/hello``, the variable with the name ``hello`` would be accessible.
 
     When ``{"config_prefix": "airflow/config"}`` is set, if a secret is defined with
     the path ``airflow/config/sql_alchemy_conn``, the config with key ``sql_alchemy_conn`` would be
     accessible.
 
-    When the prefix is empty, keys will use the Lockbox Secrets without any prefix.
+    If the prefix is empty, the requests will not be sent to Yandex Lockbox.
 
     .. code-block:: ini
 
         [secrets]
         backend = airflow.providers.yandex.secrets.lockbox.LockboxSecretBackend
         backend_kwargs = {"yc_connection_id": "<connection_ID>", "folder_id": "<folder_ID>"}
 
-    You need to specify credentials or id of yandexcloud connection to connect to Yandex Lockbox with.
-    Credentials will be used with this priority:
+    You need to specify credentials or the ID of the ``yandexcloud`` connection to connect to Yandex Lockbox.
+    The credentials will be used with the following priority:
 
-    * OAuth Token
-    * Service Account JSON file
-    * Service Account JSON
-    * Yandex Cloud Connection
+    * OAuth token
+    * Service account key in JSON from file
+    * Service account key in JSON
+    * Yandex Cloud connection
 
-    If no credentials specified, default connection id will be used.
+    If you do not specify any credentials,
+    the system will use the default connection ID:``yandexcloud_default``.
 
     Also, you need to specify the Yandex Cloud folder ID to search for Yandex Lockbox secrets in.
+    If you do not specify folder ID, the requests will use the connection ``folder_id`` if specified.
 
-    :param yc_oauth_token: Specifies the user account OAuth token to connect to Yandex Lockbox with.
-        Looks like ``y3_xxxxx``.
-    :param yc_sa_key_json: Specifies the service account auth JSON.
-        Looks like ``{"id": "...", "service_account_id": "...", "private_key": "..."}``.
-    :param yc_sa_key_json_path: Specifies the service account auth JSON file path.
-        Looks like ``/home/airflow/authorized_key.json``.
-        File content looks like ``{"id": "...", "service_account_id": "...", "private_key": "..."}``.
-    :param yc_connection_id: Specifies the connection ID to connect to Yandex Lockbox with.
-        Default: "yandexcloud_default"
+    :param yc_oauth_token: Specifies the user account OAuth token to connect to Yandex Lockbox.
+        The parameter value should look like ``y3_xx123``.
+    :param yc_sa_key_json: Specifies the service account key in JSON.
+        The parameter value should look like
+        ``{"id": "...", "service_account_id": "...", "private_key": "..."}``.
+    :param yc_sa_key_json_path: Specifies the service account key in JSON file path.
+        The parameter value should look like ``/home/airflow/authorized_key.json``,
+        while the file content should have the following format:
+        ``{"id": "...", "service_account_id": "...", "private_key": "..."}``.
+    :param yc_connection_id: Specifies the connection ID to connect to Yandex Lockbox.
+        The default value is ``yandexcloud_default``.
     :param folder_id: Specifies the folder ID to search for Yandex Lockbox secrets in.
-        If set to None (null in JSON), requests will use the connection folder_id if specified.
-    :param connections_prefix: Specifies the prefix of the secret to read to get Connections.
-        If set to None (null in JSON), requests for connections will not be sent to Yandex Lockbox.
-        Default: "airflow/connections"
-    :param variables_prefix: Specifies the prefix of the secret to read to get Variables.
-        If set to None (null in JSON), requests for variables will not be sent to Yandex Lockbox.
-        Default: "airflow/variables"
-    :param config_prefix: Specifies the prefix of the secret to read to get Configurations.
-        If set to None (null in JSON), requests for variables will not be sent to Yandex Lockbox.
-        Default: "airflow/config"
-    :param sep: Specifies the separator used to concatenate secret_prefix and secret_id.
-        Default: "/"
-    :param endpoint: Specifies an API endpoint.
-        If set to None (null in JSON), requests will use the connection endpoint, if specified,
-        or the default endpoint.
+        If set to ``None`` (``null`` in JSON),
+        the requests will use the connection ``folder_id``, if specified.
+    :param connections_prefix: Specifies the prefix of the secret to read to get connections.
+        If set to ``None`` (``null`` in JSON),
+        the requests for connections will not be sent to Yandex Lockbox.
+        The default value is ``airflow/connections``.
+    :param variables_prefix: Specifies the prefix of the secret to read to get variables.
+        If set to ``None`` (``null`` in JSON), the requests for variables will not be sent to Yandex Lockbox.
+        The default value is ``airflow/variables``.
+    :param config_prefix: Specifies the prefix of the secret to read to get configurations.
+        If set to ``None`` (``null`` in JSON), the requests for variables will not be sent to Yandex Lockbox.
+        The default value is ``airflow/config``.
+    :param sep: Specifies the separator to concatenate ``secret_prefix`` and ``secret_id``.
+        The default value is ``/``.
+    :param endpoint: Specifies the API endpoint.
+        If set to ``None`` (``null`` in JSON), the requests will use the connection endpoint, if specified;
+        otherwise, they will use the default endpoint.
     """
 
     def __init__(
         self,
         yc_oauth_token: str | None = None,
         yc_sa_key_json: dict | str | None = None,
         yc_sa_key_json_path: str | None = None,
@@ -124,18 +131,16 @@
 
         self.yc_oauth_token = yc_oauth_token
         self.yc_sa_key_json = yc_sa_key_json
         self.yc_sa_key_json_path = yc_sa_key_json_path
         self.yc_connection_id = None
         if not any([yc_oauth_token, yc_sa_key_json, yc_sa_key_json_path]):
             self.yc_connection_id = yc_connection_id or default_conn_name
-        else:
-            assert (
-                yc_connection_id is None
-            ), "yc_connection_id should not be used if other credentials are specified"
+        elif yc_connection_id is not None:
+            raise ValueError("`yc_connection_id` should not be used if other credentials are specified")
 
         self.folder_id = folder_id
         self.connections_prefix = connections_prefix.rstrip(sep) if connections_prefix is not None else None
         self.variables_prefix = variables_prefix.rstrip(sep) if variables_prefix is not None else None
         self.config_prefix = config_prefix.rstrip(sep) if config_prefix is not None else None
         self.sep = sep
         self.endpoint = endpoint
```

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/__init__.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/credentials.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/defaults.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/fields.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/utils/fields.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/airflow/providers/yandex/utils/user_agent.py` & `apache_airflow_providers_yandex-3.9.1rc1/airflow/providers/yandex/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/pyproject.toml` & `apache_airflow_providers_yandex-3.9.1rc1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-yandex"
-version = "3.9.0.rc1"
+version = "3.9.1.rc1"
 description = "Provider package apache-airflow-providers-yandex for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -47,25 +47,27 @@
     "Framework :: Apache Airflow",
     "Framework :: Apache Airflow :: Provider",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
-    "apache-airflow>=2.6.0.dev0",
+    "apache-airflow>=2.6.0rc0",
+    "yandex-query-client>=0.1.2",
     "yandexcloud>=0.228.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_yandex-3.9.0rc1/PKG-INFO` & `apache_airflow_providers_yandex-3.9.1rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-yandex
-Version: 3.9.0rc1
+Version: 3.9.1rc1
 Summary: Provider package apache-airflow-providers-yandex for Apache Airflow
 Keywords: airflow-provider,yandex,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,20 +15,22 @@
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: apache-airflow>=2.6.0.dev0
+Requires-Dist: apache-airflow>=2.6.0rc0
+Requires-Dist: yandex-query-client>=0.1.2
 Requires-Dist: yandexcloud>=0.228.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -70,45 +72,46 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-yandex``
 
-Release: ``3.9.0.rc1``
+Release: ``3.9.1.rc1``
 
 
 This package is for Yandex, including:
 
     - `Yandex.Cloud <https://cloud.yandex.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``yandex`` provider. All classes for this provider package
 are in ``airflow.providers.yandex`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-yandex``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.8,3.9,3.10,3.11,3.12
 
 Requirements
 ------------
 
-==================  ==================
-PIP package         Version required
-==================  ==================
-``apache-airflow``  ``>=2.6.0``
-``yandexcloud``     ``>=0.228.0``
-==================  ==================
+=======================  ==================
+PIP package              Version required
+=======================  ==================
+``apache-airflow``       ``>=2.6.0``
+``yandexcloud``          ``>=0.228.0``
+``yandex-query-client``  ``>=0.1.2``
+=======================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-yandex/3.9.1/changelog.html>`_.
```

