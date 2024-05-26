# Comparing `tmp/flask_postgres-0.2.4.tar.gz` & `tmp/flask_postgres-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_postgres-0.2.4.tar", last modified: Sun May 26 04:53:53 2024, max compression
+gzip compressed data, was "flask_postgres-0.2.5.tar", last modified: Sun May 26 18:30:49 2024, max compression
```

## Comparing `flask_postgres-0.2.4.tar` & `flask_postgres-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      467 2021-11-28 00:46:40.336107 flask_postgres-0.2.4/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1583 2024-05-26 04:53:49.764526 flask_postgres-0.2.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3028 2021-11-28 22:41:15.031770 flask_postgres-0.2.4/.gitignore
--rw-r--r--   0        0        0     1080 2021-11-26 16:37:30.106975 flask_postgres-0.2.4/LICENSE
--rw-r--r--   0        0        0      440 2024-05-26 04:53:49.765326 flask_postgres-0.2.4/Makefile
--rw-r--r--   0        0        0     7455 2024-05-25 21:13:07.986691 flask_postgres-0.2.4/README.md
--rw-r--r--   0        0        0      870 2024-05-26 04:53:49.766007 flask_postgres-0.2.4/docker-compose.yml
--rw-r--r--   0        0        0      905 2021-11-28 23:30:40.833015 flask_postgres-0.2.4/docs/mkdocs.yml
--rw-r--r--   0        0        0       89 2021-11-28 22:56:53.504954 flask_postgres-0.2.4/docs/requirements.txt
--rw-r--r--   0        0        0   269616 2021-11-27 16:25:00.298000 flask_postgres-0.2.4/docs/src/img/flask-postgres-banner.png
--rw-r--r--   0        0        0     4139 2021-11-29 02:38:27.697000 flask_postgres-0.2.4/docs/src/img/flask-postgres-logo-small.png
--rw-r--r--   0        0        0    12765 2021-11-29 02:37:43.250000 flask_postgres-0.2.4/docs/src/img/flask-postgres-logo.png
--rw-r--r--   0        0        0       17 2021-11-28 23:30:40.829320 flask_postgres-0.2.4/docs/src/index.md
--rw-r--r--   0        0        0      202 2024-05-26 04:53:49.766860 flask_postgres-0.2.4/flask_postgres/__init__.py
--rw-r--r--   0        0        0      927 2021-11-28 03:02:19.203233 flask_postgres-0.2.4/flask_postgres/_compat.py
--rw-r--r--   0        0        0       22 2021-11-28 19:45:15.992245 flask_postgres-0.2.4/flask_postgres/cli/__init__.py
--rw-r--r--   0        0        0     7325 2024-05-26 04:53:49.767801 flask_postgres-0.2.4/flask_postgres/cli/main.py
--rw-r--r--   0        0        0     2536 2024-05-25 21:13:07.989625 flask_postgres-0.2.4/flask_postgres/cli/types.py
--rw-r--r--   0        0        0     1626 2024-05-25 21:13:07.991076 flask_postgres-0.2.4/flask_postgres/config.py
--rw-r--r--   0        0        0     1977 2021-11-28 20:09:06.582787 flask_postgres-0.2.4/flask_postgres/exceptions.py
--rw-r--r--   0        0        0     4207 2021-11-28 22:09:33.030497 flask_postgres-0.2.4/flask_postgres/ops.py
--rw-r--r--   0        0        0     6821 2024-05-26 04:53:49.768781 flask_postgres-0.2.4/flask_postgres/types.py
--rw-r--r--   0        0        0     2897 2024-05-26 04:53:34.008552 flask_postgres-0.2.4/flask_postgres/utils.py
--rw-r--r--   0        0        0     1321 2024-05-26 04:53:49.769715 flask_postgres-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-27 19:11:21.187335 flask_postgres-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     2539 2021-11-28 21:37:37.533439 flask_postgres-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0     9743 2024-05-26 04:53:49.770980 flask_postgres-0.2.4/tests/test_cli_normal_app_config.py
--rw-r--r--   0        0        0     4135 2024-05-25 21:13:07.996197 flask_postgres-0.2.4/tests/test_types.py
--rw-r--r--   0        0        0     3422 2024-05-26 04:53:49.772181 flask_postgres-0.2.4/tests/test_utils.py
--rw-r--r--   0        0        0     8883 1970-01-01 00:00:00.000000 flask_postgres-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      467 2021-11-28 00:46:40.336107 flask_postgres-0.2.5/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1583 2024-05-26 18:20:55.472396 flask_postgres-0.2.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3028 2021-11-28 22:41:15.031770 flask_postgres-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1080 2021-11-26 16:37:30.106975 flask_postgres-0.2.5/LICENSE
+-rw-r--r--   0        0        0      440 2024-05-26 18:20:55.472835 flask_postgres-0.2.5/Makefile
+-rw-r--r--   0        0        0     8408 2024-05-26 18:29:55.786328 flask_postgres-0.2.5/README.md
+-rw-r--r--   0        0        0      870 2024-05-26 18:20:55.473577 flask_postgres-0.2.5/docker-compose.yml
+-rw-r--r--   0        0        0      905 2021-11-28 23:30:40.833015 flask_postgres-0.2.5/docs/mkdocs.yml
+-rw-r--r--   0        0        0       89 2021-11-28 22:56:53.504954 flask_postgres-0.2.5/docs/requirements.txt
+-rw-r--r--   0        0        0   269616 2021-11-27 16:25:00.298000 flask_postgres-0.2.5/docs/src/img/flask-postgres-banner.png
+-rw-r--r--   0        0        0     4139 2021-11-29 02:38:27.697000 flask_postgres-0.2.5/docs/src/img/flask-postgres-logo-small.png
+-rw-r--r--   0        0        0    12765 2021-11-29 02:37:43.250000 flask_postgres-0.2.5/docs/src/img/flask-postgres-logo.png
+-rw-r--r--   0        0        0       17 2021-11-28 23:30:40.829320 flask_postgres-0.2.5/docs/src/index.md
+-rw-r--r--   0        0        0      202 2024-05-26 18:26:41.839966 flask_postgres-0.2.5/flask_postgres/__init__.py
+-rw-r--r--   0        0        0      927 2021-11-28 03:02:19.203233 flask_postgres-0.2.5/flask_postgres/_compat.py
+-rw-r--r--   0        0        0       22 2021-11-28 19:45:15.992245 flask_postgres-0.2.5/flask_postgres/cli/__init__.py
+-rw-r--r--   0        0        0     7325 2024-05-26 18:20:55.474416 flask_postgres-0.2.5/flask_postgres/cli/main.py
+-rw-r--r--   0        0        0     2536 2024-05-26 18:20:55.474874 flask_postgres-0.2.5/flask_postgres/cli/types.py
+-rw-r--r--   0        0        0     1626 2024-05-26 18:20:55.475257 flask_postgres-0.2.5/flask_postgres/config.py
+-rw-r--r--   0        0        0     1977 2021-11-28 20:09:06.582787 flask_postgres-0.2.5/flask_postgres/exceptions.py
+-rw-r--r--   0        0        0     4207 2021-11-28 22:09:33.030497 flask_postgres-0.2.5/flask_postgres/ops.py
+-rw-r--r--   0        0        0     6821 2024-05-26 18:20:55.475692 flask_postgres-0.2.5/flask_postgres/types.py
+-rw-r--r--   0        0        0     2897 2024-05-26 18:20:55.476050 flask_postgres-0.2.5/flask_postgres/utils.py
+-rw-r--r--   0        0        0     1321 2024-05-26 18:20:55.476490 flask_postgres-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-27 19:11:21.187335 flask_postgres-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     2539 2021-11-28 21:37:37.533439 flask_postgres-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0     9743 2024-05-26 18:20:55.476967 flask_postgres-0.2.5/tests/test_cli_normal_app_config.py
+-rw-r--r--   0        0        0     4135 2024-05-25 21:13:07.996197 flask_postgres-0.2.5/tests/test_types.py
+-rw-r--r--   0        0        0     3422 2024-05-26 18:20:55.477325 flask_postgres-0.2.5/tests/test_utils.py
+-rw-r--r--   0        0        0     9836 1970-01-01 00:00:00.000000 flask_postgres-0.2.5/PKG-INFO
```

### Comparing `flask_postgres-0.2.4/.github/workflows/tests.yml` & `flask_postgres-0.2.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/.gitignore` & `flask_postgres-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/LICENSE` & `flask_postgres-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/README.md` & `flask_postgres-0.2.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+> [!WARNING]  
+> **This project is no longer supported.**
+> 
+> This was a weekend side project I made back in 2021. I updated it in 2024 so that it should work with **Flask 3** and **Flask-SQLAlchemy 3**. I cannot make any guarantees that it works for Flask versions later than that. I do not ever intend on maintaining this going forward.
+>
+> If you would like to create and drop databases, you have a few options:
+>
+> - For local dev: Docker + Docker Compose
+> - For unit-tests: Docker + Docker Compose, or `devcontainers`, or [pytest-postgresql](https://github.com/ClearcodeHQ/pytest-postgresql)
+>
+> For database initialization, use a migration framework such as Alembic, Flyway, Liquibase, etc.
+
+---
+
 <p align="center">
   <img src="https://raw.githubusercontent.com/dwreeves/Flask-Postgres/main/docs/src/img/flask-postgres-banner.png">
 </p>
 
 <p align="center">
   <img src="https://github.com/dwreeves/Flask-Postgres/workflows/tests/badge.svg">
   <img src="https://github.com/dwreeves/Flask-Postgres/workflows/docs/badge.svg">
@@ -173,14 +187,18 @@
 
 Which is to say, this package is a lightweight alternative to setting up an application in a fully fledged production way.
 
 For serious production stuff, look into Docker Compose (to `create` your database) and Alembic (to `init` your database).
 
 # Release notes
 
+- `0.2.5`:
+  - **⚠️ Project is no longer supported! This is the final version I intend on ever releasing.**
+  - Add support for Flask 3 and Flask-SQLAlchemy 3.
+  - Add `FLASK_POSTGRES_DATABASE_TEMPLATE` and `FLASK_POSTGRES_RICH_CLICK` options.
 - `0.2.0`: Broke the API in a few spots and made it more consistent.
     - `dbname` is the commonly used variable name.
     - Reorganized the config variables around.
     - Lots of refactoring to expose database operations: `create_db` and `drop_db`.
     - Added typo checking in the Click context.
     - Added more options: `--force-disconnect` and `--overwrite`.
     - Added more robust typing with `PostgresUri`. This builds and validates a Postgres URI, and provides helpful information to the user on why it's invalid. This is used both internally to make the code nicer + safer, and it's also as a `click.ParamType`.
```

### Comparing `flask_postgres-0.2.4/docker-compose.yml` & `flask_postgres-0.2.5/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/docs/mkdocs.yml` & `flask_postgres-0.2.5/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/docs/src/img/flask-postgres-banner.png` & `flask_postgres-0.2.5/docs/src/img/flask-postgres-banner.png`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/docs/src/img/flask-postgres-logo-small.png` & `flask_postgres-0.2.5/docs/src/img/flask-postgres-logo-small.png`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/docs/src/img/flask-postgres-logo.png` & `flask_postgres-0.2.5/docs/src/img/flask-postgres-logo.png`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/flask_postgres/_compat.py` & `flask_postgres-0.2.5/flask_postgres/_compat.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/flask_postgres/cli/main.py` & `flask_postgres-0.2.5/flask_postgres/cli/main.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/flask_postgres/cli/types.py` & `flask_postgres-0.2.5/flask_postgres/cli/types.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/flask_postgres/config.py` & `flask_postgres-0.2.5/flask_postgres/config.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/flask_postgres/exceptions.py` & `flask_postgres-0.2.5/flask_postgres/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/flask_postgres/ops.py` & `flask_postgres-0.2.5/flask_postgres/ops.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/flask_postgres/types.py` & `flask_postgres-0.2.5/flask_postgres/types.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/flask_postgres/utils.py` & `flask_postgres-0.2.5/flask_postgres/utils.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/pyproject.toml` & `flask_postgres-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/tests/conftest.py` & `flask_postgres-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/tests/test_cli_normal_app_config.py` & `flask_postgres-0.2.5/tests/test_cli_normal_app_config.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/tests/test_types.py` & `flask_postgres-0.2.5/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/tests/test_utils.py` & `flask_postgres-0.2.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.4/PKG-INFO` & `flask_postgres-0.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_postgres
-Version: 0.2.4
+Version: 0.2.5
 Summary: Simple CLI for managing Postgres databases in Flask.
 Home-page: https://github.com/dwreeves/flask-postgres
 License: MIT
 Author: Daniel Reeves
 Author-email: xdanielreeves@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -32,14 +32,28 @@
 Requires-Dist: pytest>=6.0.1,<7a0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-postgresql ; extra == "test"
 Provides-Extra: doc
 Provides-Extra: rich
 Provides-Extra: test
 
+> [!WARNING]  
+> **This project is no longer supported.**
+> 
+> This was a weekend side project I made back in 2021. I updated it in 2024 so that it should work with **Flask 3** and **Flask-SQLAlchemy 3**. I cannot make any guarantees that it works for Flask versions later than that. I do not ever intend on maintaining this going forward.
+>
+> If you would like to create and drop databases, you have a few options:
+>
+> - For local dev: Docker + Docker Compose
+> - For unit-tests: Docker + Docker Compose, or `devcontainers`, or [pytest-postgresql](https://github.com/ClearcodeHQ/pytest-postgresql)
+>
+> For database initialization, use a migration framework such as Alembic, Flyway, Liquibase, etc.
+
+---
+
 <p align="center">
   <img src="https://raw.githubusercontent.com/dwreeves/Flask-Postgres/main/docs/src/img/flask-postgres-banner.png">
 </p>
 
 <p align="center">
   <img src="https://github.com/dwreeves/Flask-Postgres/workflows/tests/badge.svg">
   <img src="https://github.com/dwreeves/Flask-Postgres/workflows/docs/badge.svg">
@@ -211,14 +225,18 @@
 
 Which is to say, this package is a lightweight alternative to setting up an application in a fully fledged production way.
 
 For serious production stuff, look into Docker Compose (to `create` your database) and Alembic (to `init` your database).
 
 # Release notes
 
+- `0.2.5`:
+  - **⚠️ Project is no longer supported! This is the final version I intend on ever releasing.**
+  - Add support for Flask 3 and Flask-SQLAlchemy 3.
+  - Add `FLASK_POSTGRES_DATABASE_TEMPLATE` and `FLASK_POSTGRES_RICH_CLICK` options.
 - `0.2.0`: Broke the API in a few spots and made it more consistent.
     - `dbname` is the commonly used variable name.
     - Reorganized the config variables around.
     - Lots of refactoring to expose database operations: `create_db` and `drop_db`.
     - Added typo checking in the Click context.
     - Added more options: `--force-disconnect` and `--overwrite`.
     - Added more robust typing with `PostgresUri`. This builds and validates a Postgres URI, and provides helpful information to the user on why it's invalid. This is used both internally to make the code nicer + safer, and it's also as a `click.ParamType`.
```

