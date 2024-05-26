# Comparing `tmp/flask_postgres-0.2.3.tar.gz` & `tmp/flask_postgres-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_postgres-0.2.3.tar", last modified: Sat May 25 21:33:29 2024, max compression
+gzip compressed data, was "flask_postgres-0.2.4.tar", last modified: Sun May 26 04:53:53 2024, max compression
```

## Comparing `flask_postgres-0.2.3.tar` & `flask_postgres-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      467 2021-11-28 00:46:40.336107 flask_postgres-0.2.3/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1836 2024-05-25 21:13:07.985539 flask_postgres-0.2.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3028 2021-11-28 22:41:15.031770 flask_postgres-0.2.3/.gitignore
--rw-r--r--   0        0        0     1080 2021-11-26 16:37:30.106975 flask_postgres-0.2.3/LICENSE
--rw-r--r--   0        0        0      184 2021-11-28 04:25:09.546225 flask_postgres-0.2.3/Makefile
--rw-r--r--   0        0        0     7455 2024-05-25 21:13:07.986691 flask_postgres-0.2.3/README.md
--rw-r--r--   0        0        0      905 2021-11-28 23:30:40.833015 flask_postgres-0.2.3/docs/mkdocs.yml
--rw-r--r--   0        0        0       89 2021-11-28 22:56:53.504954 flask_postgres-0.2.3/docs/requirements.txt
--rw-r--r--   0        0        0   269616 2021-11-27 16:25:00.298000 flask_postgres-0.2.3/docs/src/img/flask-postgres-banner.png
--rw-r--r--   0        0        0     4139 2021-11-29 02:38:27.697000 flask_postgres-0.2.3/docs/src/img/flask-postgres-logo-small.png
--rw-r--r--   0        0        0    12765 2021-11-29 02:37:43.250000 flask_postgres-0.2.3/docs/src/img/flask-postgres-logo.png
--rw-r--r--   0        0        0       17 2021-11-28 23:30:40.829320 flask_postgres-0.2.3/docs/src/index.md
--rw-r--r--   0        0        0      202 2024-05-25 21:13:07.987408 flask_postgres-0.2.3/flask_postgres/__init__.py
--rw-r--r--   0        0        0      927 2021-11-28 03:02:19.203233 flask_postgres-0.2.3/flask_postgres/_compat.py
--rw-r--r--   0        0        0       22 2021-11-28 19:45:15.992245 flask_postgres-0.2.3/flask_postgres/cli/__init__.py
--rw-r--r--   0        0        0     7286 2024-05-25 21:13:07.988558 flask_postgres-0.2.3/flask_postgres/cli/main.py
--rw-r--r--   0        0        0     2536 2024-05-25 21:13:07.989625 flask_postgres-0.2.3/flask_postgres/cli/types.py
--rw-r--r--   0        0        0     1626 2024-05-25 21:13:07.991076 flask_postgres-0.2.3/flask_postgres/config.py
--rw-r--r--   0        0        0     1977 2021-11-28 20:09:06.582787 flask_postgres-0.2.3/flask_postgres/exceptions.py
--rw-r--r--   0        0        0     4207 2021-11-28 22:09:33.030497 flask_postgres-0.2.3/flask_postgres/ops.py
--rw-r--r--   0        0        0     6202 2024-05-25 21:13:07.992147 flask_postgres-0.2.3/flask_postgres/types.py
--rw-r--r--   0        0        0     2897 2024-05-25 21:13:07.993620 flask_postgres-0.2.3/flask_postgres/utils.py
--rw-r--r--   0        0        0     1318 2024-05-25 21:13:07.994730 flask_postgres-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-27 19:11:21.187335 flask_postgres-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     2539 2021-11-28 21:37:37.533439 flask_postgres-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     9573 2021-11-28 20:49:53.514181 flask_postgres-0.2.3/tests/test_cli_normal_app_config.py
--rw-r--r--   0        0        0     4135 2024-05-25 21:13:07.996197 flask_postgres-0.2.3/tests/test_types.py
--rw-r--r--   0        0        0     3008 2024-05-25 21:13:07.997666 flask_postgres-0.2.3/tests/test_utils.py
--rw-r--r--   0        0        0     8924 1970-01-01 00:00:00.000000 flask_postgres-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      467 2021-11-28 00:46:40.336107 flask_postgres-0.2.4/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1583 2024-05-26 04:53:49.764526 flask_postgres-0.2.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3028 2021-11-28 22:41:15.031770 flask_postgres-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1080 2021-11-26 16:37:30.106975 flask_postgres-0.2.4/LICENSE
+-rw-r--r--   0        0        0      440 2024-05-26 04:53:49.765326 flask_postgres-0.2.4/Makefile
+-rw-r--r--   0        0        0     7455 2024-05-25 21:13:07.986691 flask_postgres-0.2.4/README.md
+-rw-r--r--   0        0        0      870 2024-05-26 04:53:49.766007 flask_postgres-0.2.4/docker-compose.yml
+-rw-r--r--   0        0        0      905 2021-11-28 23:30:40.833015 flask_postgres-0.2.4/docs/mkdocs.yml
+-rw-r--r--   0        0        0       89 2021-11-28 22:56:53.504954 flask_postgres-0.2.4/docs/requirements.txt
+-rw-r--r--   0        0        0   269616 2021-11-27 16:25:00.298000 flask_postgres-0.2.4/docs/src/img/flask-postgres-banner.png
+-rw-r--r--   0        0        0     4139 2021-11-29 02:38:27.697000 flask_postgres-0.2.4/docs/src/img/flask-postgres-logo-small.png
+-rw-r--r--   0        0        0    12765 2021-11-29 02:37:43.250000 flask_postgres-0.2.4/docs/src/img/flask-postgres-logo.png
+-rw-r--r--   0        0        0       17 2021-11-28 23:30:40.829320 flask_postgres-0.2.4/docs/src/index.md
+-rw-r--r--   0        0        0      202 2024-05-26 04:53:49.766860 flask_postgres-0.2.4/flask_postgres/__init__.py
+-rw-r--r--   0        0        0      927 2021-11-28 03:02:19.203233 flask_postgres-0.2.4/flask_postgres/_compat.py
+-rw-r--r--   0        0        0       22 2021-11-28 19:45:15.992245 flask_postgres-0.2.4/flask_postgres/cli/__init__.py
+-rw-r--r--   0        0        0     7325 2024-05-26 04:53:49.767801 flask_postgres-0.2.4/flask_postgres/cli/main.py
+-rw-r--r--   0        0        0     2536 2024-05-25 21:13:07.989625 flask_postgres-0.2.4/flask_postgres/cli/types.py
+-rw-r--r--   0        0        0     1626 2024-05-25 21:13:07.991076 flask_postgres-0.2.4/flask_postgres/config.py
+-rw-r--r--   0        0        0     1977 2021-11-28 20:09:06.582787 flask_postgres-0.2.4/flask_postgres/exceptions.py
+-rw-r--r--   0        0        0     4207 2021-11-28 22:09:33.030497 flask_postgres-0.2.4/flask_postgres/ops.py
+-rw-r--r--   0        0        0     6821 2024-05-26 04:53:49.768781 flask_postgres-0.2.4/flask_postgres/types.py
+-rw-r--r--   0        0        0     2897 2024-05-26 04:53:34.008552 flask_postgres-0.2.4/flask_postgres/utils.py
+-rw-r--r--   0        0        0     1321 2024-05-26 04:53:49.769715 flask_postgres-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-27 19:11:21.187335 flask_postgres-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     2539 2021-11-28 21:37:37.533439 flask_postgres-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     9743 2024-05-26 04:53:49.770980 flask_postgres-0.2.4/tests/test_cli_normal_app_config.py
+-rw-r--r--   0        0        0     4135 2024-05-25 21:13:07.996197 flask_postgres-0.2.4/tests/test_types.py
+-rw-r--r--   0        0        0     3422 2024-05-26 04:53:49.772181 flask_postgres-0.2.4/tests/test_utils.py
+-rw-r--r--   0        0        0     8883 1970-01-01 00:00:00.000000 flask_postgres-0.2.4/PKG-INFO
```

### Comparing `flask_postgres-0.2.3/.gitignore` & `flask_postgres-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/LICENSE` & `flask_postgres-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/README.md` & `flask_postgres-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/docs/mkdocs.yml` & `flask_postgres-0.2.4/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/docs/src/img/flask-postgres-banner.png` & `flask_postgres-0.2.4/docs/src/img/flask-postgres-banner.png`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/docs/src/img/flask-postgres-logo-small.png` & `flask_postgres-0.2.4/docs/src/img/flask-postgres-logo-small.png`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/docs/src/img/flask-postgres-logo.png` & `flask_postgres-0.2.4/docs/src/img/flask-postgres-logo.png`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/flask_postgres/_compat.py` & `flask_postgres-0.2.4/flask_postgres/_compat.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/flask_postgres/cli/main.py` & `flask_postgres-0.2.4/flask_postgres/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 
 FC = t.TypeVar("FC", t.Callable[..., t.Any], click.Command)
 
 
 def get_connection(
         ctx: click.Context,
-        uri: str
+        uri: dict
 ) -> "psycopg.Connection":
-    conn = psycopg.connect(uri)
+    conn = psycopg.connect(**uri)
     conn.autocommit = True
     ctx.call_on_close(conn.close)
     return conn
 
 
 def uri_option(
         operation_past_tense: str,
@@ -156,15 +156,15 @@
         overwrite: bool = False,
         **kwargs
 ):
     """Create the database."""
     if overwrite:
         ctx.forward(drop_db_command)
     admin_uri = uri.admin_uri(admin_dbname)
-    conn = get_connection(ctx, admin_uri)
+    conn = get_connection(ctx, admin_uri.connection_dict())
     return create_db(
         conn=conn,
         dbname=uri.dbname,
         command_line_mode=True,
         template=config.get("FLASK_POSTGRES_DATABASE_TEMPLATE")
     )
 
@@ -202,15 +202,15 @@
         admin_dbname: t.Optional[str] = config.get("FLASK_POSTGRES_ADMIN_DBNAME"),
         force: bool = False,
         force_disconnect: bool = False,
         **kwargs
 ):
     """Delete the database."""
     admin_uri = uri.admin_uri(admin_dbname)
-    conn = get_connection(ctx, admin_uri)
+    conn = get_connection(ctx, admin_uri.connection_dict())
     return drop_db(
         conn=conn,
         dbname=uri.dbname,
         command_line_mode=True,
         force_disconnect=force_disconnect,
         confirm=not force
     )
```

### Comparing `flask_postgres-0.2.3/flask_postgres/cli/types.py` & `flask_postgres-0.2.4/flask_postgres/cli/types.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/flask_postgres/config.py` & `flask_postgres-0.2.4/flask_postgres/config.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/flask_postgres/exceptions.py` & `flask_postgres-0.2.4/flask_postgres/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/flask_postgres/ops.py` & `flask_postgres-0.2.4/flask_postgres/ops.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/flask_postgres/types.py` & `flask_postgres-0.2.4/flask_postgres/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 
 from flask_postgres._compat import psycopg
 from flask_postgres import config
 from flask_postgres.exceptions import UriValidationError
 
 
 _db_regex = re.compile(
-    r'(?:(?P<scheme>[a-z][a-z0-9+\-.]+(?:\+[a-z0-9+\-.]+)?)://)?'
+    r'(?:(?P<scheme>[a-z][a-z0-9\-.]+)(?:\+(?P<driver>[a-z0-9+\-.]+))?://)?'
     r'(?:(?P<user>[^\s:/]*)'
     r'(?::(?P<password>[^\s/]*))?@)?'
     r'(?P<host>[^\s/:?#]+)'
     r'(?::(?P<port>\d+))?'
     r'(?:/(?P<dbname>[^\s?#]*))?',
     re.IGNORECASE,
 )
 
 
 class _PsqlUriParts(t.NamedTuple):
     scheme: str
+    driver: t.Optional[str]
     user: t.Optional[str]
     password: t.Optional[str]
     host: str
     port: t.Optional[t.Union[str, int]]
     dbname: str
 
 
@@ -40,43 +41,47 @@
     }
 
     def __init__(
             self,
             uri: t.Optional[str] = None,
             *,
             scheme: str = "postgresql",
+            driver: t.Optional[str] = "postgresql",
             user: t.Optional[str] = None,
             password: t.Optional[str] = None,
             host: str = "localhost",
             port: t.Optional[t.Union[str, int]] = 5432,
             dbname: str = None
     ):
         if uri is None:
             self.build(
                 scheme=scheme,
+                driver=driver,
                 user=user,
                 password=password,
                 host=host,
                 port=port,
                 dbname=dbname
             )
         else:
-            scheme, user, password, host, port, dbname = \
+            scheme, driver, user, password, host, port, dbname = \
                 self._parts_from_str(uri)
         str.__init__(uri)
         self.scheme = scheme
+        self.driver = driver
         self.user = user
         self.password = password
         self.host = host
         self.port = port
         self.dbname = dbname
         if self._validate_when_initializing:
             self.validate(
                 uri=uri,
                 scheme=scheme,
+                driver=driver,
                 user=user,
                 password=password,
                 host=host,
                 port=port,
                 dbname=dbname
             )
             # ^ above validates that `port` is either int or None.
@@ -104,33 +109,38 @@
         if match_obj is None:
             raise UriValidationError(
                 value=s,
                 issue="Could not parse as a valid URI."
             )
         return _PsqlUriParts(
             scheme=match_obj.group("scheme"),
+            driver=match_obj.group("driver"),
             user=match_obj.group("user"),
             password=match_obj.group("password"),
             host=match_obj.group("host"),
             port=match_obj.group("port"),
             dbname=match_obj.group("dbname"),
         )
 
     @classmethod
     def build(
-        cls,
-        *,
-        scheme: str = "postgresql",
-        user: t.Optional[str] = None,
-        password: t.Optional[str] = None,
-        host: str = "localhost",
-        port: t.Optional[t.Union[str, int]] = 5432,
-        dbname: str,
+            cls,
+            *,
+            scheme: str = "postgresql",
+            driver: t.Optional[str] = None,
+            user: t.Optional[str] = None,
+            password: t.Optional[str] = None,
+            host: str = "localhost",
+            port: t.Optional[t.Union[str, int]] = 5432,
+            dbname: str,
     ) -> str:
-        uri = f"{scheme}://"
+        uri = scheme
+        if driver is not None:
+            uri += f"+{driver}"
+        uri += "://"
         if user is not None:
             uri += user
         if password is not None:
             uri += ":" + password
         if user or password:
             uri += "@"
         uri += host
@@ -141,14 +151,15 @@
 
     @classmethod
     def validate(
             cls,
             uri: str,
             *,
             scheme: str = "postgresql",
+            driver: t.Optional[str] = None,
             user: t.Optional[str] = None,
             password: t.Optional[str] = None,
             host: str = "localhost",
             port: t.Optional[t.Union[str, int]] = 5432,
             dbname: str,
     ) -> bool:
         if dbname is None and cls._validation_config["must_have_dbname"]:
@@ -183,14 +194,17 @@
     @classmethod
     def default(cls) -> "PostgresUri":
         return cls(config.get("FLASK_POSTGRES_TARGET_DATABASE_URI"))
 
     def dict(self) -> t.Dict[str, t.Optional[t.Union[str, int]]]:
         return {i: getattr(self, i) for i in self.__slots__}
 
+    def connection_dict(self) -> t.Dict[str, t.Optional[t.Union[str, int]]]:
+        return {k: v for k, v in self.dict().items() if k in {"dbname", "user", "password", "host", "port"}}
+
     def admin_uri(self, dbname: t.Optional[str] = None) -> "PostgresUri":
         d = self.dict()
         dbname = dbname or config.get("FLASK_POSTGRES_ADMIN_DBNAME")
         if dbname.startswith("/"):
             warnings.warn(
                 "Please do not put a slash in front of the"
                 " `FLASK_POSTGRES_ADMIN_DBNAME`.",
```

### Comparing `flask_postgres-0.2.3/flask_postgres/utils.py` & `flask_postgres-0.2.4/flask_postgres/utils.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/pyproject.toml` & `flask_postgres-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Database"
 ]
 requires = [
-    "Flask>=1.0",
+    "Flask>=2.0",
     "Click>=7.0",
-    "SQLAlchemy>=1.2.2",
-    "Flask-SQLAlchemy>=2.4",
+    "SQLAlchemy>=1.4.0",
+    "Flask-SQLAlchemy>=2.5",
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 
 [tool.flit.metadata.requires-extra]
 test = [
-    "psycopg",
+    # "psycopg2",
     "pytest>=6.0.1,<7a0",
     "pytest-cov",
     "pytest-postgresql",
 ]
 doc = [
     "mkdocs",
     "pymdown-extensions",
```

### Comparing `flask_postgres-0.2.3/tests/conftest.py` & `flask_postgres-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/tests/test_cli_normal_app_config.py` & `flask_postgres-0.2.4/tests/test_cli_normal_app_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,18 +59,18 @@
         typically_configured_app: Flask,
         db_params: dict
 ):
     dbname = db_params.get("dbname")
 
     assert not db_exists(admin_connection, dbname)
 
-    client = typically_configured_app.test_cli_runner()
-    res = client.invoke(typically_configured_app.cli, ["psql", "create"])
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
+    res: Result = client.invoke(typically_configured_app.cli, ["psql", "create"])
 
-    assert res.exit_code == 0
+    assert res.exit_code == 0, res.output
     assert res.output == f'database "{dbname}" was created\n'
     assert db_exists(admin_connection, dbname)
 
 
 def test_psql_init_command(
         typically_configured_app: Flask,
         activated_database,
@@ -80,15 +80,15 @@
 ):
     dbname = db_params.get("dbname")
 
     with typically_configured_app.app_context():
         db_inspector = sa.inspect(db.engine)
         assert not db_inspector.has_table("pet")
 
-    client = typically_configured_app.test_cli_runner()
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
     res = client.invoke(typically_configured_app.cli, ["psql", "init"])
 
     assert res.exit_code == 0, res.output
     assert res.output == f'database "{dbname}" was initialized\n', res.output
 
     with typically_configured_app.app_context():
         db_inspector = sa.inspect(db.engine)
@@ -106,15 +106,15 @@
         db_params: dict,
         admin_connection
 ):
     dbname = db_params.get("dbname")
 
     assert not db_exists(admin_connection, dbname)
 
-    client = typically_configured_app.test_cli_runner()
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
     res = client.invoke(typically_configured_app.cli, ["psql", "init"])
 
     assert res.output == f'database "{dbname}" does not exist\n', res.output
     assert not db_exists(admin_connection, dbname)
 
 
 def test_psql_init_command_with_custom_callback(
@@ -123,15 +123,15 @@
         db_params: dict,
         db,
         example_model,
         custom_init_db_callback,
 ):
     dbname = db_params.get("dbname")
 
-    client = typically_configured_app.test_cli_runner()
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
     res = client.invoke(typically_configured_app.cli, ["psql", "init"])
 
     assert res.exit_code == 0, res.output
     assert res.output == f'database "{dbname}" was initialized\n', res.output
 
     with typically_configured_app.app_context():
         first_row_of_data = db.session.query(example_model).first()
@@ -164,15 +164,15 @@
     assert db_exists(admin_connection, dbname)
 
     if cli_test_conf.type_in_db_name:
         input_stream = dbname
     else:
         input_stream = None
 
-    client = typically_configured_app.test_cli_runner()
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
     res = client.invoke(
         typically_configured_app.cli,
         ["psql", "drop", *cli_test_conf.options],
         input=input_stream
     )
 
     assert res.exit_code == 0, res.output
@@ -195,15 +195,15 @@
 ):
     dbname = db_params.get("dbname")
 
     assert db_exists(admin_connection, dbname)
 
     input_stream = uri + "extratext"
 
-    client = typically_configured_app.test_cli_runner()
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
     res = client.invoke(
         typically_configured_app.cli,
         ["psql", "drop"],
         input=input_stream
     )
 
     assert res.exit_code == 1, res.output
@@ -222,15 +222,15 @@
         db,
         example_model
 ):
     dbname = db_params.get("dbname")
 
     assert not db_exists(admin_connection, dbname)
 
-    client = typically_configured_app.test_cli_runner()
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
     res = client.invoke(typically_configured_app.cli, ["psql", "setup"])
 
     assert res.exit_code == 0, res.output
     assert res.output == (
         f'database "{dbname}" was created\n'
         f'database "{dbname}" was initialized\n'
     ), res.output
@@ -250,15 +250,15 @@
         example_model,
         custom_init_db_callback,
 ):
     dbname = db_params.get("dbname")
 
     assert not db_exists(admin_connection, dbname)
 
-    client = typically_configured_app.test_cli_runner()
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
     res = client.invoke(typically_configured_app.cli, ["psql", "setup"])
 
     assert res.exit_code == 0, res.output
     assert res.output == (
         f'database "{dbname}" was created\n'
         f'database "{dbname}" was initialized\n'
     ), res.output
@@ -282,15 +282,15 @@
 
     assert db_exists(admin_connection, dbname)
 
     with typically_configured_app.app_context():
         db_inspector = sa.inspect(db.engine)
         assert not db_inspector.has_table("pet")
 
-    client = typically_configured_app.test_cli_runner()
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
     res = client.invoke(typically_configured_app.cli, ["psql", "setup"])
 
     assert res.exit_code == 0, res.output
     assert res.output == (
         f'database "{dbname}" already exists\n'
         f'database "{dbname}" was initialized\n'
     ), res.output
@@ -314,15 +314,15 @@
         db,
         example_model
 ):
     dbname = db_params.get("dbname")
 
     assert db_exists(admin_connection, dbname)
 
-    client = typically_configured_app.test_cli_runner()
+    client = typically_configured_app.test_cli_runner(mix_stderr=True)
     res = client.invoke(typically_configured_app.cli, ["psql", "reset", "-f"])
 
     assert res.exit_code == 0, res.output
     assert res.output == (
         f'database "{dbname}" was deleted\n'
         f'database "{dbname}" was created\n'
         f'database "{dbname}" was initialized\n'
```

### Comparing `flask_postgres-0.2.3/tests/test_types.py` & `flask_postgres-0.2.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.3/tests/test_utils.py` & `flask_postgres-0.2.4/tests/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 from flask_postgres.ops import database_exists
 from flask_postgres.utils import resolve_init_db_callback
 from flask_postgres.utils import get_db
 from flask_postgres.utils import raise_err_if_disallowed
 from flask_postgres.exceptions import SqlaExtensionNotFound
 from flask_postgres.exceptions import EnvironmentNotAllowed
 
+try:
+    from importlib import metadata  # type: ignore[import,unused-ignore]
+except ImportError:
+    # Python < 3.8
+    import importlib_metadata as metadata  # type: ignore[no-redef,import-not-found]
+
 
 def test_database_exists_function(
         admin_connection,
         db_params
 ):
     """It's critical that this test passes because other tests use the
     `database_exists` function to run their own tests.
@@ -80,14 +86,21 @@
     assert db1 is db2
 
     # No app context
     with pytest.raises(RuntimeError):
         get_db()
 
 
+major, minor, *_ = metadata.version("flask").split(".")
+
+# ≤ 2.2 only
+@pytest.mark.skipif(
+    condition=not (3 > int(major) >= 2 and 3 > int(minor) >= 0),
+    reason="app.env is deprecated in Flask 2.3.0+"
+)
 def test_raise_err_if_disallowed_function(base_app):
     # Nothing should happen
     with base_app.app_context():
         raise_err_if_disallowed()
 
     base_app.config["FLASK_POSTGRES_CLI_DISALLOWED_ENVS"] = [base_app.env]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flask_postgres-0.2.3/PKG-INFO` & `flask_postgres-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: flask_postgres
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple CLI for managing Postgres databases in Flask.
 Home-page: https://github.com/dwreeves/flask-postgres
 License: MIT
 Author: Daniel Reeves
 Author-email: xdanielreeves@gmail.com
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Database
-Requires-Dist: Flask>=1.0
+Requires-Dist: Flask>=2.0
 Requires-Dist: Click>=7.0
-Requires-Dist: SQLAlchemy>=1.2.2
-Requires-Dist: Flask-SQLAlchemy>=2.4
+Requires-Dist: SQLAlchemy>=1.4.0
+Requires-Dist: Flask-SQLAlchemy>=2.5
 Requires-Dist: mkdocs ; extra == "doc"
 Requires-Dist: pymdown-extensions ; extra == "doc"
 Requires-Dist: mkdocs-material ; extra == "doc"
 Requires-Dist: mkdocs-macros-plugin ; extra == "doc"
 Requires-Dist: pygments ; extra == "doc"
 Requires-Dist: rich ; extra == "rich"
 Requires-Dist: rich-click ; extra == "rich"
-Requires-Dist: psycopg ; extra == "test"
 Requires-Dist: pytest>=6.0.1,<7a0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-postgresql ; extra == "test"
 Provides-Extra: doc
 Provides-Extra: rich
 Provides-Extra: test
```

