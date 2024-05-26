# Comparing `tmp/apache_airflow_providers_microsoft_mssql-3.7.0rc1.tar.gz` & `tmp/apache_airflow_providers_microsoft_mssql-3.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_microsoft_mssql-3.7.0rc1.tar", last modified: Tue Apr 30 11:33:11 2024, max compression
+gzip compressed data, was "apache_airflow_providers_microsoft_mssql-3.7.1rc1.tar", last modified: Tue May 21 10:41:50 2024, max compression
```

## Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1.tar` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4362 2024-04-30 11:33:11.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-30 11:33:11.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/LICENSE
--rw-r--r--   0        0        0     1590 2024-04-30 11:33:11.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/__init__.py
--rw-r--r--   0        0        0     3118 2024-04-30 11:33:11.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/get_provider_info.py
--rw-r--r--   0        0        0      787 2024-04-30 11:33:11.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/hooks/__init__.py
--rw-r--r--   0        0        0     4203 2024-04-30 11:33:11.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/hooks/mssql.py
--rw-r--r--   0        0        0      787 2024-04-30 11:33:11.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/operators/__init__.py
--rw-r--r--   0        0        0     2857 2024-04-30 11:33:11.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/operators/mssql.py
--rw-r--r--   0        0        0     3173 2024-04-30 11:33:11.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6260 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_mssql-3.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     4362 2024-05-21 10:41:50.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-05-21 10:41:50.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/LICENSE
+-rw-r--r--   0        0        0     1502 2024-05-21 10:41:50.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/__init__.py
+-rw-r--r--   0        0        0     3139 2024-05-21 10:41:50.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/get_provider_info.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:41:50.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/hooks/__init__.py
+-rw-r--r--   0        0        0     4409 2024-05-21 10:41:50.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/hooks/mssql.py
+-rw-r--r--   0        0        0      787 2024-05-21 10:41:50.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/operators/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-21 10:41:50.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/operators/mssql.py
+-rw-r--r--   0        0        0     3173 2024-05-21 10:41:50.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     6260 1970-01-01 00:00:00.000000 apache_airflow_providers_microsoft_mssql-3.7.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/README.rst` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,28 +38,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.1.rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/sql-server/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.mssql`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.mssql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-mssql``
@@ -93,8 +93,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.1/changelog.html>`_.
```

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/LICENSE` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/__init__.py` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,22 +21,19 @@
 # IF YOU WANT TO MODIFY THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
 # `PROVIDER__INIT__PY_TEMPLATE.py.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 #
 from __future__ import annotations
 
 import packaging.version
 
-__all__ = ["__version__"]
+from airflow import __version__ as airflow_version
 
-__version__ = "3.7.0"
+__all__ = ["__version__"]
 
-try:
-    from airflow import __version__ as airflow_version
-except ImportError:
-    from airflow.version import version as airflow_version
+__version__ = "3.7.1"
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
     "2.7.0"
 ):
     raise RuntimeError(
         f"The package `apache-airflow-providers-microsoft-mssql:{__version__}` needs Apache Airflow 2.7.0+"
     )
```

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/get_provider_info.py` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-microsoft-mssql",
         "name": "Microsoft SQL Server (MSSQL)",
         "description": "`Microsoft SQL Server (MSSQL) <https://www.microsoft.com/sql-server/>`__\n",
         "state": "ready",
-        "source-date-epoch": 1714476791,
+        "source-date-epoch": 1716288110,
         "versions": [
+            "3.7.1",
             "3.7.0",
             "3.6.1",
             "3.6.0",
             "3.5.0",
             "3.4.2",
             "3.4.1",
             "3.4.0",
```

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/hooks/__init__.py` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/hooks/mssql.py` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/hooks/mssql.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Microsoft SQLServer hook module."""
 
 from __future__ import annotations
 
-from typing import Any
+from functools import cached_property
+from typing import TYPE_CHECKING, Any
 
 import pymssql
 
 from airflow.providers.common.sql.hooks.sql import DbApiHook
 
+if TYPE_CHECKING:
+    from airflow.models import Connection
+
 
 class MsSqlHook(DbApiHook):
     """
     Interact with Microsoft SQL Server.
 
     :param args: passed to DBApiHook
     :param sqlalchemy_scheme: Scheme sqlalchemy connection.  Default is ``mssql+pymssql`` Only used for
@@ -49,23 +53,31 @@
         sqlalchemy_scheme: str | None = None,
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
         self.schema = kwargs.pop("schema", None)
         self._sqlalchemy_scheme = sqlalchemy_scheme
 
+    @cached_property
+    def connection(self) -> Connection:
+        """
+        Get the airflow connection object.
+
+        :return: The connection object.
+        """
+        return self.get_connection(getattr(self, self.conn_name_attr))
+
     @property
     def connection_extra_lower(self) -> dict:
         """
         ``connection.extra_dejson`` but where keys are converted to lower case.
 
         This is used internally for case-insensitive access of mssql params.
         """
-        conn = self.get_connection(self.mssql_conn_id)  # type: ignore[attr-defined]
-        return {k.lower(): v for k, v in conn.extra_dejson.items()}
+        return {k.lower(): v for k, v in self.connection.extra_dejson.items()}
 
     @property
     def sqlalchemy_scheme(self) -> str:
         """Sqlalchemy scheme either from constructor, connection extras or default."""
         extra_scheme = self.connection_extra_lower.get("sqlalchemy_scheme")
         if not self._sqlalchemy_scheme and extra_scheme and (":" in extra_scheme or "/" in extra_scheme):
             raise RuntimeError("sqlalchemy_scheme in connection extra should not contain : or / characters")
@@ -90,24 +102,22 @@
     ) -> Any:
         """Sqlalchemy connection object."""
         engine = self.get_sqlalchemy_engine(engine_kwargs=engine_kwargs)
         return engine.connect(**(connect_kwargs or {}))
 
     def get_conn(self) -> pymssql.connect:
         """Return ``pymssql`` connection object."""
-        conn = self.get_connection(self.mssql_conn_id)  # type: ignore[attr-defined]
-
-        conn = pymssql.connect(
+        conn = self.connection
+        return pymssql.connect(
             server=conn.host,
             user=conn.login,
             password=conn.password,
             database=self.schema or conn.schema,
             port=conn.port,
         )
-        return conn
 
     def set_autocommit(
         self,
         conn: pymssql.connect,
         autocommit: bool,
     ) -> None:
         conn.autocommit(autocommit)
```

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/operators/__init__.py` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/airflow/providers/microsoft/mssql/operators/mssql.py` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/airflow/providers/microsoft/mssql/operators/mssql.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/pyproject.toml` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-microsoft-mssql"
-version = "3.7.0.rc1"
+version = "3.7.1.rc1"
 description = "Provider package apache-airflow-providers-microsoft-mssql for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -58,16 +58,16 @@
 dependencies = [
     "apache-airflow-providers-common-sql>=1.3.1rc0",
     "apache-airflow>=2.7.0rc0",
     "pymssql>=2.1.8",
 ]
 
 [project.urls]
-"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.0"
-"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.0/changelog.html"
+"Documentation" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.1"
+"Changelog" = "https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.1/changelog.html"
 "Bug Tracker" = "https://github.com/apache/airflow/issues"
 "Source Code" = "https://github.com/apache/airflow"
 "Slack Chat" = "https://s.apache.org/airflow-slack"
 "Twitter" = "https://twitter.com/ApacheAirflow"
 "YouTube" = "https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/"
 
 [project.entry-points."apache_airflow_provider"]
```

### Comparing `apache_airflow_providers_microsoft_mssql-3.7.0rc1/PKG-INFO` & `apache_airflow_providers_microsoft_mssql-3.7.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-mssql
-Version: 3.7.0rc1
+Version: 3.7.1rc1
 Summary: Provider package apache-airflow-providers-microsoft-mssql for Apache Airflow
 Keywords: airflow-provider,microsoft.mssql,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: apache-airflow-providers-common-sql>=1.3.1rc0
 Requires-Dist: apache-airflow>=2.7.0rc0
 Requires-Dist: pymssql>=2.1.8
 Requires-Dist: apache-airflow-providers-common-sql ; extra == "common.sql"
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.0/changelog.html
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.0
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.1
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Provides-Extra: common.sql
 
 
@@ -74,28 +74,28 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.7.0.rc1``
+Release: ``3.7.1.rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/sql-server/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``microsoft.mssql`` provider. All classes for this provider package
 are in ``airflow.providers.microsoft.mssql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.1/>`_.
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-microsoft-mssql``
@@ -129,8 +129,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.7.1/changelog.html>`_.
```

