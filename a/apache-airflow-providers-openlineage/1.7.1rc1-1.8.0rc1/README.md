# Comparing `tmp/apache_airflow_providers_openlineage-1.7.1rc1.tar.gz` & `tmp/apache_airflow_providers_openlineage-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_openlineage-1.7.1rc1.tar", last modified: Tue Apr 30 11:37:38 2024, max compression
+gzip compressed data, was "apache_airflow_providers_openlineage-1.8.0rc1.tar", last modified: Tue May 14 10:58:58 2024, max compression
```

## Comparing `apache_airflow_providers_openlineage-1.7.1rc1.tar` & `apache_airflow_providers_openlineage-1.8.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4410 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/LICENSE
--rw-r--r--   0        0        0     1586 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/__init__.py
--rw-r--r--   0        0        0     3398 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/conf.py
--rw-r--r--   0        0        0     1081 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/__init__.py
--rw-r--r--   0        0        0     5070 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/base.py
--rw-r--r--   0        0        0     2412 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/bash.py
--rw-r--r--   0        0        0     9996 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/manager.py
--rw-r--r--   0        0        0     2999 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/python.py
--rw-r--r--   0        0        0     6626 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/__init__.py
--rw-r--r--   0        0        0    14634 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/adapter.py
--rw-r--r--   0        0        0     2644 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/facets.py
--rw-r--r--   0        0        0    11624 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/listener.py
--rw-r--r--   0        0        0     3076 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/macros.py
--rw-r--r--   0        0        0     1625 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/openlineage.py
--rw-r--r--   0        0        0    15308 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/sqlparser.py
--rw-r--r--   0        0        0      785 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/__init__.py
--rw-r--r--   0        0        0     3072 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/selective_enable.py
--rw-r--r--   0        0        0     9366 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/sql.py
--rw-r--r--   0        0        0    13285 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/utils.py
--rw-r--r--   0        0        0     3355 2024-04-30 11:37:38.000000 apache_airflow_providers_openlineage-1.7.1rc1/pyproject.toml
--rw-r--r--   0        0        0     6381 1970-01-01 00:00:00.000000 apache_airflow_providers_openlineage-1.7.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     4410 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/LICENSE
+-rw-r--r--   0        0        0     1498 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/__init__.py
+-rw-r--r--   0        0        0     4693 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/conf.py
+-rw-r--r--   0        0        0     1081 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/__init__.py
+-rw-r--r--   0        0        0     5476 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/base.py
+-rw-r--r--   0        0        0     2563 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/bash.py
+-rw-r--r--   0        0        0    10315 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/manager.py
+-rw-r--r--   0        0        0     3151 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/python.py
+-rw-r--r--   0        0        0     7072 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/__init__.py
+-rw-r--r--   0        0        0    16917 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/adapter.py
+-rw-r--r--   0        0        0     2644 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/facets.py
+-rw-r--r--   0        0        0    14092 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/listener.py
+-rw-r--r--   0        0        0     3076 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/macros.py
+-rw-r--r--   0        0        0     1678 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/openlineage.py
+-rw-r--r--   0        0        0    15308 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/sqlparser.py
+-rw-r--r--   0        0        0      785 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/utils/__init__.py
+-rw-r--r--   0        0        0     3072 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/utils/selective_enable.py
+-rw-r--r--   0        0        0     9366 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/utils/sql.py
+-rw-r--r--   0        0        0    14036 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/utils/utils.py
+-rw-r--r--   0        0        0     3355 2024-05-14 10:58:58.000000 apache_airflow_providers_openlineage-1.8.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     6381 1970-01-01 00:00:00.000000 apache_airflow_providers_openlineage-1.8.0rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/README.rst` & `apache_airflow_providers_openlineage-1.8.0rc1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.7.1.rc1``
+Release: ``1.8.0.rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openlineage`` provider. All classes for this provider package
 are in ``airflow.providers.openlineage`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.8.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openlineage``
@@ -95,8 +95,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.8.0/changelog.html>`_.
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/LICENSE` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/__init__.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "1.7.1"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "1.8.0"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-openlineage:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/__init__.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/base.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -83,14 +83,17 @@
         by existence of get_openlineage_facets method on operator.
         """
         return []
 
     def _execute_extraction(self) -> OperatorLineage | None:
         # OpenLineage methods are optional - if there's no method, return None
         try:
+            self.log.debug(
+                "Trying to execute `get_openlineage_facets_on_start` for %s.", self.operator.task_type
+            )
             return self._get_openlineage_facets(self.operator.get_openlineage_facets_on_start)  # type: ignore
         except ImportError:
             self.log.error(
                 "OpenLineage provider method failed to import OpenLineage integration. "
                 "This should not happen. Please report this bug to developers."
             )
             return None
@@ -101,17 +104,21 @@
             )
             return None
 
     def extract_on_complete(self, task_instance) -> OperatorLineage | None:
         if task_instance.state == TaskInstanceState.FAILED:
             on_failed = getattr(self.operator, "get_openlineage_facets_on_failure", None)
             if on_failed and callable(on_failed):
+                self.log.debug(
+                    "Executing `get_openlineage_facets_on_failure` for %s.", self.operator.task_type
+                )
                 return self._get_openlineage_facets(on_failed, task_instance)
         on_complete = getattr(self.operator, "get_openlineage_facets_on_complete", None)
         if on_complete and callable(on_complete):
+            self.log.debug("Executing `get_openlineage_facets_on_complete` for %s.", self.operator.task_type)
             return self._get_openlineage_facets(on_complete, task_instance)
         return self.extract()
 
     def _get_openlineage_facets(self, get_facets_method, *args) -> OperatorLineage | None:
         try:
             facets: OperatorLineage = get_facets_method(*args)
             # "rewrite" OperatorLineage to safeguard against different version of the same class
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/bash.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/bash.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,18 @@
             job_facets = {
                 "sourceCode": SourceCodeJobFacet(
                     language="bash",
                     # We're on worker and should have access to DAG files
                     source=self.operator.bash_command,
                 )
             }
+        else:
+            self.log.debug(
+                "OpenLineage disable_source_code option is on - no source code is extracted.",
+            )
 
         return OperatorLineage(
             job_facets=job_facets,
             # The BashOperator is recorded as an "unknownSource" even though we have an extractor,
             # as the <i>data lineage</i> cannot be determined from the operator directly.
             run_facets=get_unknown_source_attribute_run_facet(task=self.operator, name="BashOperator"),
         )
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/manager.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,38 +12,34 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
-from contextlib import suppress
 from typing import TYPE_CHECKING, Iterator
 
 from airflow.providers.openlineage import conf
 from airflow.providers.openlineage.extractors import BaseExtractor, OperatorLineage
 from airflow.providers.openlineage.extractors.base import DefaultExtractor
 from airflow.providers.openlineage.extractors.bash import BashExtractor
 from airflow.providers.openlineage.extractors.python import PythonExtractor
-from airflow.providers.openlineage.utils.utils import get_unknown_source_attribute_run_facet
+from airflow.providers.openlineage.utils.utils import (
+    get_unknown_source_attribute_run_facet,
+    try_import_from_string,
+)
 from airflow.utils.log.logging_mixin import LoggingMixin
-from airflow.utils.module_loading import import_string
 
 if TYPE_CHECKING:
     from openlineage.client.run import Dataset
 
     from airflow.lineage.entities import Table
     from airflow.models import Operator
 
 
-def try_import_from_string(string):
-    with suppress(ImportError):
-        return import_string(string)
-
-
 def _iter_extractor_types() -> Iterator[type[BaseExtractor]]:
     if PythonExtractor is not None:
         yield PythonExtractor
     if BashExtractor is not None:
         yield BashExtractor
 
 
@@ -57,24 +53,35 @@
 
         # Built-in Extractors like Bash and Python
         for extractor in _iter_extractor_types():
             for operator_class in extractor.get_operator_classnames():
                 self.extractors[operator_class] = extractor
 
         for extractor_path in conf.custom_extractors():
-            extractor: type[BaseExtractor] = try_import_from_string(extractor_path)
+            extractor: type[BaseExtractor] | None = try_import_from_string(extractor_path)
+            if not extractor:
+                self.log.warning(
+                    "OpenLineage is unable to import custom extractor `%s`; will ignore it.", extractor_path
+                )
+                continue
             for operator_class in extractor.get_operator_classnames():
                 if operator_class in self.extractors:
-                    self.log.debug(
-                        "Duplicate extractor found for `%s`. `%s` will be used instead of `%s`",
+                    self.log.warning(
+                        "Duplicate OpenLineage custom extractor found for `%s`. "
+                        "`%s` will be used instead of `%s`",
                         operator_class,
                         extractor_path,
                         self.extractors[operator_class],
                     )
                 self.extractors[operator_class] = extractor
+                self.log.debug(
+                    "Registered custom OpenLineage extractor `%s` for class `%s`",
+                    extractor_path,
+                    operator_class,
+                )
 
     def add_extractor(self, operator_class: str, extractor: type[BaseExtractor]):
         self.extractors[operator_class] = extractor
 
     def extract_metadata(self, dagrun, task, complete: bool = False, task_instance=None) -> OperatorLineage:
         extractor = self._get_extractor(task)
         task_info = (
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/extractors/python.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/extractors/python.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,19 @@
             job_facet = {
                 "sourceCode": SourceCodeJobFacet(
                     language="python",
                     # We're on worker and should have access to DAG files
                     source=source_code,
                 )
             }
+        else:
+            self.log.debug(
+                "OpenLineage disable_source_code option is on - no source code is extracted.",
+            )
+
         return OperatorLineage(
             job_facets=job_facet,
             # The PythonOperator is recorded as an "unknownSource" even though we have an extractor,
             # as the <i>data lineage</i> cannot be determined from the operator directly.
             run_facets=get_unknown_source_attribute_run_facet(task=self.operator, name="PythonOperator"),
         )
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/get_provider_info.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-openlineage",
         "name": "OpenLineage Airflow",
         "description": "`OpenLineage <https://openlineage.io/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714477058,
+        "source-date-epoch": 1715684338,
         "versions": [
+            "1.8.0",
             "1.7.1",
             "1.7.0",
             "1.6.0",
             "1.5.0",
             "1.4.0",
             "1.3.1",
             "1.3.0",
@@ -117,16 +118,23 @@
                         "type": "string",
                         "example": '{"type": "http", "url": "http://localhost:5000", "endpoint": "api/v1/lineage"}',
                         "default": "",
                         "version_added": None,
                     },
                     "disable_source_code": {
                         "description": "Disable the inclusion of source code in OpenLineage events by setting this to `true`.\nBy default, several Operators (e.g. Python, Bash) will include their source code in the events\nunless disabled.\n",
-                        "default": None,
+                        "default": "False",
                         "example": None,
                         "type": "boolean",
                         "version_added": None,
                     },
+                    "dag_state_change_process_pool_size": {
+                        "description": "Number of processes to utilize for processing DAG state changes\nin an asynchronous manner within the scheduler process.\n",
+                        "default": "1",
+                        "example": None,
+                        "type": "integer",
+                        "version_added": "1.8.0",
+                    },
                 },
             }
         },
     }
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/__init__.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/adapter.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/adapter.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+import traceback
 import uuid
 from contextlib import ExitStack
 from typing import TYPE_CHECKING
 
 import yaml
 from openlineage.client import OpenLineageClient, set_producer
 from openlineage.client.facet import (
@@ -69,33 +70,47 @@
             secrets_masker = _secrets_masker()
         self._redacter = OpenLineageRedactor.from_masker(secrets_masker)
 
     def get_or_create_openlineage_client(self) -> OpenLineageClient:
         if not self._client:
             config = self.get_openlineage_config()
             if config:
+                self.log.debug(
+                    "OpenLineage configuration found. Transport type: `%s`",
+                    config.get("type", "no type provided"),
+                )
                 self._client = OpenLineageClient.from_dict(config=config)
             else:
+                self.log.debug(
+                    "OpenLineage configuration not found directly in Airflow. "
+                    "Looking for legacy environment configuration. "
+                )
                 self._client = OpenLineageClient.from_environment()
         return self._client
 
     def get_openlineage_config(self) -> dict | None:
         # First, try to read from YAML file
         openlineage_config_path = conf.config_path(check_legacy_env_var=False)
         if openlineage_config_path:
             config = self._read_yaml_config(openlineage_config_path)
             if config:
                 return config.get("transport", None)
+            self.log.debug("OpenLineage config file is empty: `%s`", openlineage_config_path)
+        else:
+            self.log.debug("OpenLineage config_path configuration not found.")
+
         # Second, try to get transport config
         transport_config = conf.transport()
         if not transport_config:
+            self.log.debug("OpenLineage transport configuration not found.")
             return None
         return transport_config
 
-    def _read_yaml_config(self, path: str) -> dict | None:
+    @staticmethod
+    def _read_yaml_config(path: str) -> dict | None:
         with open(path) as config_file:
             return yaml.safe_load(config_file)
 
     @staticmethod
     def build_dag_run_id(dag_id, dag_run_id):
         return str(uuid.uuid3(uuid.NAMESPACE_URL, f"{conf.namespace()}.{dag_id}.{dag_run_id}"))
 
@@ -121,14 +136,15 @@
         transport_type = f"{self._client.transport.kind}".lower()
 
         try:
             with ExitStack() as stack:
                 stack.enter_context(Stats.timer(f"ol.emit.attempts.{event_type}.{transport_type}"))
                 stack.enter_context(Stats.timer("ol.emit.attempts"))
                 self._client.emit(redacted_event)
+                self.log.debug("Successfully emitted OpenLineage event of id %s", event.run.runId)
         except Exception as e:
             Stats.incr("ol.emit.failed")
             self.log.warning("Failed to emit OpenLineage event of id %s", event.run.runId)
             self.log.debug("OpenLineage emission failure: %s", e)
 
         return redacted_event
 
@@ -280,56 +296,74 @@
     def dag_started(
         self,
         dag_run: DagRun,
         msg: str,
         nominal_start_time: str,
         nominal_end_time: str,
     ):
-        event = RunEvent(
-            eventType=RunState.START,
-            eventTime=dag_run.start_date.isoformat(),
-            job=self._build_job(job_name=dag_run.dag_id, job_type=_JOB_TYPE_DAG),
-            run=self._build_run(
-                run_id=self.build_dag_run_id(dag_run.dag_id, dag_run.run_id),
-                job_name=dag_run.dag_id,
-                nominal_start_time=nominal_start_time,
-                nominal_end_time=nominal_end_time,
-            ),
-            inputs=[],
-            outputs=[],
-            producer=_PRODUCER,
-        )
-        self.emit(event)
+        try:
+            event = RunEvent(
+                eventType=RunState.START,
+                eventTime=dag_run.start_date.isoformat(),
+                job=self._build_job(job_name=dag_run.dag_id, job_type=_JOB_TYPE_DAG),
+                run=self._build_run(
+                    run_id=self.build_dag_run_id(dag_run.dag_id, dag_run.run_id),
+                    job_name=dag_run.dag_id,
+                    nominal_start_time=nominal_start_time,
+                    nominal_end_time=nominal_end_time,
+                ),
+                inputs=[],
+                outputs=[],
+                producer=_PRODUCER,
+            )
+            self.emit(event)
+        except BaseException:
+            # Catch all exceptions to prevent ProcessPoolExecutor from silently swallowing them.
+            # This ensures that any unexpected exceptions are logged for debugging purposes.
+            # This part cannot be wrapped to deduplicate code, otherwise the method cannot be pickled in multiprocessing.
+            self.log.warning("Failed to emit DAG started event: \n %s", traceback.format_exc())
 
     def dag_success(self, dag_run: DagRun, msg: str):
-        event = RunEvent(
-            eventType=RunState.COMPLETE,
-            eventTime=dag_run.end_date.isoformat(),
-            job=self._build_job(job_name=dag_run.dag_id, job_type=_JOB_TYPE_DAG),
-            run=Run(runId=self.build_dag_run_id(dag_run.dag_id, dag_run.run_id)),
-            inputs=[],
-            outputs=[],
-            producer=_PRODUCER,
-        )
-        self.emit(event)
+        try:
+            event = RunEvent(
+                eventType=RunState.COMPLETE,
+                eventTime=dag_run.end_date.isoformat(),
+                job=self._build_job(job_name=dag_run.dag_id, job_type=_JOB_TYPE_DAG),
+                run=Run(runId=self.build_dag_run_id(dag_run.dag_id, dag_run.run_id)),
+                inputs=[],
+                outputs=[],
+                producer=_PRODUCER,
+            )
+            self.emit(event)
+        except BaseException:
+            # Catch all exceptions to prevent ProcessPoolExecutor from silently swallowing them.
+            # This ensures that any unexpected exceptions are logged for debugging purposes.
+            # This part cannot be wrapped to deduplicate code, otherwise the method cannot be pickled in multiprocessing.
+            self.log.warning("Failed to emit DAG success event: \n %s", traceback.format_exc())
 
     def dag_failed(self, dag_run: DagRun, msg: str):
-        event = RunEvent(
-            eventType=RunState.FAIL,
-            eventTime=dag_run.end_date.isoformat(),
-            job=self._build_job(job_name=dag_run.dag_id, job_type=_JOB_TYPE_DAG),
-            run=Run(
-                runId=self.build_dag_run_id(dag_run.dag_id, dag_run.run_id),
-                facets={"errorMessage": ErrorMessageRunFacet(message=msg, programmingLanguage="python")},
-            ),
-            inputs=[],
-            outputs=[],
-            producer=_PRODUCER,
-        )
-        self.emit(event)
+        try:
+            event = RunEvent(
+                eventType=RunState.FAIL,
+                eventTime=dag_run.end_date.isoformat(),
+                job=self._build_job(job_name=dag_run.dag_id, job_type=_JOB_TYPE_DAG),
+                run=Run(
+                    runId=self.build_dag_run_id(dag_run.dag_id, dag_run.run_id),
+                    facets={"errorMessage": ErrorMessageRunFacet(message=msg, programmingLanguage="python")},
+                ),
+                inputs=[],
+                outputs=[],
+                producer=_PRODUCER,
+            )
+            self.emit(event)
+        except BaseException:
+            # Catch all exceptions to prevent ProcessPoolExecutor from silently swallowing them.
+            # This ensures that any unexpected exceptions are logged for debugging purposes.
+            # This part cannot be wrapped to deduplicate code, otherwise the method cannot be pickled in multiprocessing.
+            self.log.warning("Failed to emit DAG failed event: \n %s", traceback.format_exc())
 
     @staticmethod
     def _build_run(
         run_id: str,
         job_name: str,
         parent_job_name: str | None = None,
         parent_run_id: str | None = None,
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/facets.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/facets.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/listener.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/listener.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,21 +13,23 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
 import logging
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import ProcessPoolExecutor
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 from openlineage.client.serde import Serde
 
+from airflow import __version__ as airflow_version, settings
 from airflow.listeners import hookimpl
+from airflow.providers.openlineage import conf
 from airflow.providers.openlineage.extractors import ExtractorManager
 from airflow.providers.openlineage.plugins.adapter import OpenLineageAdapter, RunState
 from airflow.providers.openlineage.utils.utils import (
     get_airflow_run_facet,
     get_custom_facets,
     get_job_name,
     is_operator_disabled,
@@ -41,14 +43,24 @@
     from sqlalchemy.orm import Session
 
     from airflow.models import DagRun, TaskInstance
 
 _openlineage_listener: OpenLineageListener | None = None
 
 
+def _get_try_number_success(val):
+    # todo: remove when min airflow version >= 2.10.0
+    from packaging.version import parse
+
+    if parse(parse(airflow_version).base_version) < parse("2.10.0"):
+        return val.try_number - 1
+    else:
+        return val.try_number
+
+
 class OpenLineageListener:
     """OpenLineage listener sends events on task instance and dag run starts, completes and failures."""
 
     def __init__(self):
         self._executor = None
         self.log = logging.getLogger(__name__)
         self.extractor_manager = ExtractorManager()
@@ -74,21 +86,27 @@
         dagrun = task_instance.dag_run
         task = task_instance.task
         if TYPE_CHECKING:
             assert task
         dag = task.dag
         if is_operator_disabled(task):
             self.log.debug(
-                "Skipping OpenLineage event emission for operator %s "
+                "Skipping OpenLineage event emission for operator `%s` "
                 "due to its presence in [openlineage] disabled_for_operators.",
                 task.task_type,
             )
-            return None
+            return
 
         if not is_selective_lineage_enabled(task):
+            self.log.debug(
+                "Skipping OpenLineage event emission for task `%s` "
+                "due to lack of explicit lineage enablement for task or DAG while "
+                "[openlineage] selective_enable is on.",
+                task.task_id,
+            )
             return
 
         @print_warning(self.log)
         def on_running():
             # that's a workaround to detect task running from deferred state
             # we return here because Airflow 2.3 needs task from deferred state
             if task_instance.next_method is not None:
@@ -142,34 +160,41 @@
         self.log.debug("OpenLineage listener got notification about task instance success")
 
         dagrun = task_instance.dag_run
         task = task_instance.task
         if TYPE_CHECKING:
             assert task
         dag = task.dag
+
         if is_operator_disabled(task):
             self.log.debug(
-                "Skipping OpenLineage event emission for operator %s "
+                "Skipping OpenLineage event emission for operator `%s` "
                 "due to its presence in [openlineage] disabled_for_operators.",
                 task.task_type,
             )
-            return None
+            return
 
         if not is_selective_lineage_enabled(task):
+            self.log.debug(
+                "Skipping OpenLineage event emission for task `%s` "
+                "due to lack of explicit lineage enablement for task or DAG while "
+                "[openlineage] selective_enable is on.",
+                task.task_id,
+            )
             return
 
         @print_warning(self.log)
         def on_success():
             parent_run_id = OpenLineageAdapter.build_dag_run_id(dag.dag_id, dagrun.run_id)
 
             task_uuid = OpenLineageAdapter.build_task_instance_run_id(
                 dag_id=dag.dag_id,
                 task_id=task.task_id,
                 execution_date=task_instance.execution_date,
-                try_number=task_instance.try_number - 1,
+                try_number=_get_try_number_success(task_instance),
             )
             event_type = RunState.COMPLETE.value.lower()
             operator_name = task.task_type.lower()
 
             with Stats.timer(f"ol.extract.{event_type}.{operator_name}"):
                 task_metadata = self.extractor_manager.extract_metadata(
                     dagrun, task, complete=True, task_instance=task_instance
@@ -197,23 +222,30 @@
         self.log.debug("OpenLineage listener got notification about task instance failure")
 
         dagrun = task_instance.dag_run
         task = task_instance.task
         if TYPE_CHECKING:
             assert task
         dag = task.dag
+
         if is_operator_disabled(task):
             self.log.debug(
-                "Skipping OpenLineage event emission for operator %s "
+                "Skipping OpenLineage event emission for operator `%s` "
                 "due to its presence in [openlineage] disabled_for_operators.",
                 task.task_type,
             )
-            return None
+            return
 
         if not is_selective_lineage_enabled(task):
+            self.log.debug(
+                "Skipping OpenLineage event emission for task `%s` "
+                "due to lack of explicit lineage enablement for task or DAG while "
+                "[openlineage] selective_enable is on.",
+                task.task_id,
+            )
             return
 
         @print_warning(self.log)
         def on_failure():
             parent_run_id = OpenLineageAdapter.build_dag_run_id(dag.dag_id, dagrun.run_id)
 
             task_uuid = OpenLineageAdapter.build_task_instance_run_id(
@@ -245,16 +277,24 @@
                 len(Serde.to_json(redacted_event).encode("utf-8")),
             )
 
         on_failure()
 
     @property
     def executor(self):
+        def initializer():
+            # Re-configure the ORM engine as there are issues with multiple processes
+            # if process calls Airflow DB.
+            settings.configure_orm()
+
         if not self._executor:
-            self._executor = ThreadPoolExecutor(max_workers=8, thread_name_prefix="openlineage_")
+            self._executor = ProcessPoolExecutor(
+                max_workers=conf.dag_state_change_process_pool_size(),
+                initializer=initializer,
+            )
         return self._executor
 
     @hookimpl
     def on_starting(self, component):
         self.log.debug("on_starting: %s", component.__class__.__name__)
 
     @hookimpl
@@ -262,41 +302,68 @@
         self.log.debug("before_stopping: %s", component.__class__.__name__)
         with timeout(30):
             self.executor.shutdown(wait=True)
 
     @hookimpl
     def on_dag_run_running(self, dag_run: DagRun, msg: str):
         if dag_run.dag and not is_selective_lineage_enabled(dag_run.dag):
+            self.log.debug(
+                "Skipping OpenLineage event emission for DAG `%s` "
+                "due to lack of explicit lineage enablement for DAG while "
+                "[openlineage] selective_enable is on.",
+                dag_run.dag_id,
+            )
             return
+
+        if not self.executor:
+            self.log.debug("Executor have not started before `on_dag_run_running`")
+            return
+
         data_interval_start = dag_run.data_interval_start.isoformat() if dag_run.data_interval_start else None
         data_interval_end = dag_run.data_interval_end.isoformat() if dag_run.data_interval_end else None
         self.executor.submit(
             self.adapter.dag_started,
             dag_run=dag_run,
             msg=msg,
             nominal_start_time=data_interval_start,
             nominal_end_time=data_interval_end,
         )
 
     @hookimpl
     def on_dag_run_success(self, dag_run: DagRun, msg: str):
         if dag_run.dag and not is_selective_lineage_enabled(dag_run.dag):
+            self.log.debug(
+                "Skipping OpenLineage event emission for DAG `%s` "
+                "due to lack of explicit lineage enablement for DAG while "
+                "[openlineage] selective_enable is on.",
+                dag_run.dag_id,
+            )
             return
+
         if not self.executor:
             self.log.debug("Executor have not started before `on_dag_run_success`")
             return
+
         self.executor.submit(self.adapter.dag_success, dag_run=dag_run, msg=msg)
 
     @hookimpl
     def on_dag_run_failed(self, dag_run: DagRun, msg: str):
         if dag_run.dag and not is_selective_lineage_enabled(dag_run.dag):
+            self.log.debug(
+                "Skipping OpenLineage event emission for DAG `%s` "
+                "due to lack of explicit lineage enablement for DAG while "
+                "[openlineage] selective_enable is on.",
+                dag_run.dag_id,
+            )
             return
+
         if not self.executor:
             self.log.debug("Executor have not started before `on_dag_run_failed`")
             return
+
         self.executor.submit(self.adapter.dag_failed, dag_run=dag_run, msg=msg)
 
 
 def get_openlineage_listener() -> OpenLineageListener:
     """Get singleton listener manager."""
     global _openlineage_listener
     if not _openlineage_listener:
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/macros.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/macros.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/plugins/openlineage.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/plugins/openlineage.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,7 +35,10 @@
     complete and failure and TaskInstances start, complete and failure.
     """
 
     name = "OpenLineageProviderPlugin"
     if not conf.is_disabled():
         macros = [lineage_job_namespace, lineage_job_name, lineage_run_id, lineage_parent_id]
         listeners = [get_openlineage_listener()]
+    else:
+        macros = []
+        listeners = []
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/sqlparser.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/sqlparser.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/__init__.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/selective_enable.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/utils/selective_enable.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/sql.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/utils/sql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/airflow/providers/openlineage/utils/utils.py` & `apache_airflow_providers_openlineage-1.8.0rc1/airflow/providers/openlineage/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,39 +21,47 @@
 import json
 import logging
 from contextlib import suppress
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Iterable
 
 import attrs
-from openlineage.client.utils import RedactMixin  # TODO: move this maybe to Airflow's logic?
+from deprecated import deprecated
+from openlineage.client.utils import RedactMixin
 
+from airflow.exceptions import AirflowProviderDeprecationWarning  # TODO: move this maybe to Airflow's logic?
 from airflow.models import DAG, BaseOperator, MappedOperator
 from airflow.providers.openlineage import conf
 from airflow.providers.openlineage.plugins.facets import (
     AirflowMappedTaskRunFacet,
     AirflowRunFacet,
     UnknownOperatorAttributeRunFacet,
     UnknownOperatorInstance,
 )
 from airflow.providers.openlineage.utils.selective_enable import (
     is_dag_lineage_enabled,
     is_task_lineage_enabled,
 )
 from airflow.utils.context import AirflowContextDeprecationWarning
 from airflow.utils.log.secrets_masker import Redactable, Redacted, SecretsMasker, should_hide_value_for_key
+from airflow.utils.module_loading import import_string
 
 if TYPE_CHECKING:
     from airflow.models import DagRun, TaskInstance
 
 
 log = logging.getLogger(__name__)
 _NOMINAL_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
+def try_import_from_string(string: str) -> Any:
+    with suppress(ImportError):
+        return import_string(string)
+
+
 def get_operator_class(task: BaseOperator) -> type:
     if task.__class__.__name__ in ("DecoratedMappedOperator", "MappedOperator"):
         return task.operator_class
     return task.__class__
 
 
 def get_job_name(task: TaskInstance) -> str:
@@ -363,26 +371,36 @@
 def print_warning(log):
     def decorator(f):
         @wraps(f)
         def wrapper(*args, **kwargs):
             try:
                 return f(*args, **kwargs)
             except Exception as e:
+                log.warning(
+                    "Note: exception below is being caught: it's printed for visibility. However OpenLineage events aren't being emitted. If you see that, task has completed successfully despite not getting OL events."
+                )
                 log.warning(e)
 
         return wrapper
 
     return decorator
 
 
 def get_filtered_unknown_operator_keys(operator: BaseOperator) -> dict:
     not_required_keys = {"dag", "task_group"}
     return {attr: value for attr, value in operator.__dict__.items() if attr not in not_required_keys}
 
 
+@deprecated(
+    reason=(
+        "`airflow.providers.openlineage.utils.utils.normalize_sql` "
+        "has been deprecated and will be removed in future"
+    ),
+    category=AirflowProviderDeprecationWarning,
+)
 def normalize_sql(sql: str | Iterable[str]):
     if isinstance(sql, str):
         sql = [stmt for stmt in sql.split(";") if stmt != ""]
     sql = [obj for stmt in sql for obj in stmt.split(";") if obj != ""]
     return ";\n".join(sql)
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/pyproject.toml` & `apache_airflow_providers_openlineage-1.8.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-openlineage"
-version = "1.7.1.rc1"
+version = "1.8.0.rc1"
 description = "Provider package apache-airflow-providers-openlineage for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -60,16 +60,16 @@
     "apache-airflow>=2.7.0rc0",
     "attrs>=22.2",
     "openlineage-integration-common>=0.28.0",
     "openlineage-python>=0.28.0",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.8.0"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.8.0/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_openlineage-1.7.1rc1/PKG-INFO` & `apache_airflow_providers_openlineage-1.8.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.7.1rc1
+Version: 1.8.0rc1
 Summary: Provider package apache-airflow-providers-openlineage for Apache Airflow
 Keywords: airflow-provider,openlineage,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,16 +24,16 @@
 Requires-Dist: apache-airflow-providers-common-sql>=1.6.0rc0
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: attrs>=22.2
 Requires-Dist: openlineage-integration-common>=0.28.0
 Requires-Dist: openlineage-python>=0.28.0
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.8.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.8.0
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 
 
@@ -76,28 +76,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.7.1.rc1``
+Release: ``1.8.0.rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openlineage`` provider. All classes for this provider package
 are in ``airflow.providers.openlineage`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.8.0/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-openlineage``
@@ -133,8 +133,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.7.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.8.0/changelog.html>`_.
```

