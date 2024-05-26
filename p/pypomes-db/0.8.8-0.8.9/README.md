# Comparing `tmp/pypomes_db-0.8.8.tar.gz` & `tmp/pypomes_db-0.8.9.tar.gz`

## Comparing `pypomes_db-0.8.8.tar` & `pypomes_db-0.8.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    35290 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    16635 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    15386 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    39427 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18680 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    17852 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    15635 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.9/PKG-INFO
```

### Comparing `pypomes_db-0.8.8/src/pypomes_db/__init__.py` & `pypomes_db-0.8.9/src/pypomes_db/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from .db_pomes import (
     db_setup, db_get_engines, db_get_params,
-    db_assert_connection, db_connect, db_exists,
-    db_select_one, db_select_all, db_update, db_delete,
-    db_insert, db_bulk_insert, db_update_lob, db_execute,
-    db_call_function, db_call_procedure,
+    db_assert_connection, db_connect,
+    db_exists, db_select_one, db_select_all,
+    db_insert, db_update, db_delete,
+    db_bulk_insert, db_bulk_update, db_update_lob,
+    db_execute, db_call_function, db_call_procedure,
 )
 from .migration_pomes import (
     db_migrate_data, db_migrate_lobs,
 )
 
 __all__ = [
     # db_pomes
     "db_setup", "db_get_engines", "db_get_params",
-    "db_assert_connection", "db_connect", "db_exists",
-    "db_select_one", "db_select_all", "db_update", "db_delete",
-    "db_insert", "db_bulk_insert", "db_update_lob", "db_execute",
-    "db_call_function", "db_call_procedure",
+    "db_assert_connection", "db_connect",
+    "db_exists", "db_select_one", "db_select_all",
+    "db_insert", "db_update", "db_delete",
+    "db_bulk_insert", "db_bulk_update", "db_update_lob",
+    "db_execute", "db_call_function", "db_call_procedure",
     # migration_pomes
     "db_migrate_data", "db_migrate_lobs",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_db")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_db-0.8.8/src/pypomes_db/db_common.py` & `pypomes_db-0.8.9/src/pypomes_db/db_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.8/src/pypomes_db/db_pomes.py` & `pypomes_db-0.8.9/src/pypomes_db/db_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noinspection DuplicatedCode
 from logging import Logger
 from pathlib import Path
 from typing import Any
 
 from .db_common import (
     _DB_ENGINES, _DB_CONN_DATA, _assert_engine
 )
@@ -193,15 +194,15 @@
 
     :param errors: incidental error messages
     :param table: the table to be searched
     :param where_attrs: the search attributes
     :param where_vals: the values for the search attributes
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: True if at least one tuple was found
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     # noinspection PyDataSource
@@ -242,15 +243,15 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     require_min: int = 1 if require_nonempty else None
@@ -291,15 +292,15 @@
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
     # initialize the local errors list
@@ -360,15 +361,15 @@
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     result: int = db_execute(errors=op_errors,
@@ -402,15 +403,15 @@
 
     :param errors: incidental error messages
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     bind_vals: tuple | None = None
@@ -448,15 +449,15 @@
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     result: int = db_execute(errors=op_errors,
@@ -481,58 +482,137 @@
                    committable: bool = True,
                    logger: Logger = None) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The target database engine, default or specified, must have been previously configured.
 
+    The binding is done by position. Thus, the *VALUES* clause in *insert_stmt* must contain
+    as many placeholders as there are elements in the tuples found in the list provided in
+    *insert_vals*. This is applicable for *mysql*, *oracle*, and *sqlserver*, where the
+    placeholders are '%VARn%, ':n', and '?', respectively, and 'n' is the 1-based position of the
+    data in the tuple. In the specific case of *postgres*, the *VALUES* clause must be simply *VALUES %s*.
+
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
-    :return: the number of inserted tuples, or None if an error occurred
+    :return: the number of inserted tuples (1 for postgres), or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
     
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.bulk_insert(errors=op_errors,
-                                          insert_stmt=insert_stmt,
-                                          insert_vals=insert_vals,
-                                          conn=connection,
-                                          committable=committable,
-                                          logger=logger)
+        result = oracle_pomes.bulk_execute(errors=op_errors,
+                                           exc_stmt=insert_stmt,
+                                           exc_vals=insert_vals,
+                                           conn=connection,
+                                           committable=committable,
+                                           logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.bulk_insert(errors=op_errors,
-                                            insert_stmt=insert_stmt,
-                                            insert_vals=insert_vals,
-                                            conn=connection,
-                                            committable=committable,
-                                            logger=logger)
+        result = postgres_pomes.bulk_execute(errors=op_errors,
+                                             exc_stmt=insert_stmt,
+                                             exc_vals=insert_vals,
+                                             conn=connection,
+                                             committable=committable,
+                                             logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.bulk_insert(errors=op_errors,
-                                             insert_stmt=insert_stmt,
-                                             insert_vals=insert_vals,
+        result = sqlserver_pomes.bulk_execute(errors=op_errors,
+                                              exc_stmt=insert_stmt,
+                                              exc_vals=insert_vals,
+                                              conn=connection,
+                                              committable=committable,
+                                              logger=logger)
+
+    # acknowledge eventual local errors
+    errors.extend(op_errors)
+
+    return result
+
+
+def db_bulk_update(errors: list[str] | None,
+                   update_stmt: str,
+                   update_vals: list[tuple],
+                   engine: str = None,
+                   connection: Any = None,
+                   committable: bool = True,
+                   logger: Logger = None) -> int:
+    """
+    Insert the tuples, with values defined in *insert_vals*, into the database.
+
+    The target database engine, default or specified, must have been previously configured.
+
+    The binding is done by position. Thus, the binding clauses in *update_stmt* must contain as many
+    placeholders as there are elements in the tuples found in the list provided in *update_vals*.
+    This is applicable for *mysql*, *oracle*, and *sqlserver*, where the placeholders are
+    '%VARn%, ':n', and '?', respectively, and 'n' is the 1-based position of the data in the tuple.
+    Note that the placeholders in the *WHERE* clause will follow the ones in the *SET* clause.
+
+    In the specific case of *postgres*, a unique syntax applies. The *VALUES* clause must be simply
+    *VALUES %s*, and it is used in both *INSERT* and *UPDATE* operations. In the latter case,
+    there is also a *FROM* clause to go along with it.
+
+    :param errors: incidental error messages
+    :param update_stmt: the UPDATE command
+    :param update_vals: the list of values to update the database with, and to locate the tuple
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param connection: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param logger: optional logger
+    :return: the number of updated tuples, or None if an error occurred
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # initialize the local errors list
+    op_errors: list[str] = []
+
+    # determine the database engine
+    curr_engine: str = _assert_engine(op_errors, engine)
+
+    if curr_engine == "mysql":
+        pass
+    elif curr_engine == "oracle":
+        from . import oracle_pomes
+        result = oracle_pomes.bulk_execute(errors=op_errors,
+                                           exc_stmt=update_stmt,
+                                           exc_vals=update_vals,
+                                           conn=connection,
+                                           committable=committable,
+                                           logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes.bulk_execute(errors=op_errors,
+                                             exc_stmt=update_stmt,
+                                             exc_vals=update_vals,
                                              conn=connection,
                                              committable=committable,
                                              logger=logger)
+    elif curr_engine == "sqlserver":
+        from . import sqlserver_pomes
+        result = sqlserver_pomes.bulk_execute(errors=op_errors,
+                                              exc_stmt=update_stmt,
+                                              exc_vals=update_vals,
+                                              conn=connection,
+                                              committable=committable,
+                                              logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -555,15 +635,15 @@
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: number of LOBs effectively copied
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the database engine
@@ -631,15 +711,15 @@
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
@@ -656,20 +736,20 @@
                                       exc_stmt=exc_stmt,
                                       bind_vals=bind_vals,
                                       conn=connection,
                                       committable=committable,
                                       logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_execute(errors=op_errors,
-                                           exc_stmt=exc_stmt,
-                                           bind_vals=bind_vals,
-                                           conn=connection,
-                                           committable=committable,
-                                           logger=logger)
+        result = postgres_pomes.execute(errors=op_errors,
+                                        exc_stmt=exc_stmt,
+                                        bind_vals=bind_vals,
+                                        conn=connection,
+                                        committable=committable,
+                                        logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
         result = sqlserver_pomes.execute(errors=op_errors,
                                          exc_stmt=exc_stmt,
                                          bind_vals=bind_vals,
                                          conn=connection,
                                          committable=committable,
@@ -694,15 +774,15 @@
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
@@ -757,15 +837,15 @@
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param engine: the database engine to use (uses the default engine, if not provided)
     :param connection: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
```

### Comparing `pypomes_db-0.8.8/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.8.9/src/pypomes_db/migration_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                     logger: Logger = None) -> int:
     """
     Migrate data from one database to another database.
 
     The origin and destination databases must be in the list of databases configured and
     supported by this package. The columns must not be type LOB (large binary object).
     The columns in the target database must be of equivalent types, respectively,
-    in both the origin and the destination database.
+    in both the origin and the destination databases.
 
     :param errors: incidental error messages
     :param source_engine: the source database engine type
     :param source_table: the origin table
     :param source_columns: the colums to be migrated
     :param target_engine: the destination database engine type
     :param target_table: the table to write the data to (defaults to the source table)
@@ -51,15 +51,14 @@
     # make sure to have connections to the source and destination databases
     curr_source_conn: Any = source_conn or db_connect(errors=op_errors,
                                                       engine=source_engine,
                                                       logger=logger)
     curr_target_conn: Any = target_conn or db_connect(errors=op_errors,
                                                       engine=target_engine,
                                                       logger=logger)
-
     # make sure to have a target table
     if not target_table:
         target_table = source_table
 
     # make sure to have target columns
     if not target_columns:
         target_columns = source_columns
@@ -247,15 +246,14 @@
     # make sure to have connections to the source and destination databases
     curr_source_conn: Any = source_conn or db_connect(errors=op_errors,
                                                       engine=source_engine,
                                                       logger=logger)
     curr_target_conn: Any = target_conn or db_connect(errors=op_errors,
                                                       engine=target_engine,
                                                       logger=logger)
-
     # make sure to have a target table
     if not target_table:
         target_table = source_table
 
     # make sure to have a target column
     if not target_lob_column:
         target_lob_column = source_lob_column
@@ -327,15 +325,17 @@
                 ora_lob = lob_var.getValue()
 
 
             # access the blob in chunks and write it to database
             offset: int = 1
             has_data: bool = False
             lob: Any = row[blob_index]
-            lob_data: bytes | str = lob.read(offset=offset, amount=chunk_size) if lob else None
+            lob_data: bytes | str = lob.read(offset=offset,
+                                             amount=chunk_size) \
+                                    if lob else None
             while lob_data:
                 size: int = len(lob_data)
                 has_data = True
                 match target_engine:
                     case "mysql":
                         pass
                     case "oracle":
```

### Comparing `pypomes_db-0.8.8/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.8.9/src/pypomes_db/oracle_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
@@ -130,50 +130,118 @@
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
-def bulk_insert(errors: list[str],
-                insert_stmt: str,
-                insert_vals: list[tuple],
-                conn: Connection,
-                committable: bool,
-                logger: Logger) -> int:
-    """
-    Insert the tuples, with values defined in *insert_vals*, into the database.
-
-    The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
-    must contain as many ':n' placeholders as there are elements in the tuples found in the
-    list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
+def execute(errors: list[str],
+            exc_stmt: str,
+            bind_vals: tuple,
+            conn: Connection,
+            committable: bool,
+            logger: Logger) -> int:
+    """
+    Execute the command *exc_stmt* on the database.
+
+    This command might be a DML ccommand modifying the database, such as
+    inserting, updating or deleting tuples, or it might be a DDL statement,
+    or it might even be an environment-related command.
+    The optional bind values for this operation are in *bind_vals*.
+    The value returned is the value obtained from the execution of *exc_stmt*.
+    It might be the number of inserted, modified, or deleted tuples,
+    ou None if an error occurred.
+
+    :param errors: incidental error messages
+    :param exc_stmt: the command to execute
+    :param bind_vals: optional bind values
+    :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param logger: optional logger
+    :return: the return value from the command execution
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # make sure to have a connection
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
+                                            logger=logger)
+
+    err_msg: str | None = None
+    try:
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+            cursor.execute(statement=exc_stmt,
+                           parameters=bind_vals)
+            result = cursor.rowcount
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
+    except Exception as e:
+        if curr_conn:
+            curr_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="oracle")
+    finally:
+        # close the connection, if locally acquired
+        if curr_conn and not conn:
+            curr_conn.close()
+
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="oracle",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=exc_stmt,
+                bind_vals=bind_vals)
+
+    return result
+
+
+def bulk_execute(errors: list[str],
+                 exc_stmt: str,
+                 exc_vals: list[tuple],
+                 conn: Connection,
+                 committable: bool,
+                 logger: Logger) -> int:
+    """
+    Bulk-update the database with the statement defined in *execute_stmt*, and the values in *execute_vals*.
+
+    The binding is done by position. Thus, the binding clauses in *execute_stmt* must contain
+    as many ':n' placeholders as there are elements in the tuples found in the list provided in
+    *execute_vals*, where 'n' is the 1-based position of the data in the tuple.
+    Note that, in *UPDATE* operations, the placeholders in the *WHERE* clause will follow
+    the ones in the *SET* clause.
 
     :param errors: incidental error messages
-    :param insert_stmt: the INSERT command
-    :param insert_vals: the list of values to be inserted
+    :param exc_stmt: the command to update the database with
+    :param exc_vals: the list of values for tuple identification, and to update the database with
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
-    :return: the number of inserted tuples, or None if an error occurred
+    :return: the number of inserted or updated tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
                                             autocommit=False,
                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
-            cursor.executemany(statement=insert_stmt,
-                               parameters=insert_vals)
-            result = len(insert_vals)
+            cursor.executemany(statement=exc_stmt,
+                               parameters=exc_vals)
+            result = len(exc_vals)
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
@@ -186,16 +254,16 @@
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
                 engine="oracle",
                 err_msg=err_msg,
                 errors=errors,
-                stmt=insert_stmt,
-                bind_vals=insert_vals[0])
+                stmt=exc_stmt,
+                bind_vals=exc_vals[0])
 
     return result
 
 
 def update_lob(errors: list[str],
                lob_table: str,
                lob_column: str,
@@ -213,15 +281,15 @@
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     """
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
                                             autocommit=False,
                                             logger=logger)
 
@@ -273,80 +341,14 @@
                 err_msg=err_msg,
                 engine="oracle",
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
-def execute(errors: list[str],
-            exc_stmt: str,
-            bind_vals: tuple,
-            conn: Connection,
-            committable: bool,
-            logger: Logger) -> int:
-    """
-    Execute the command *exc_stmt* on the database.
-
-    This command might be a DML ccommand modifying the database, such as
-    inserting, updating or deleting tuples, or it might be a DDL statement,
-    or it might even be an environment-related command.
-    The optional bind values for this operation are in *bind_vals*.
-    The value returned is the value obtained from the execution of *exc_stmt*.
-    It might be the number of inserted, modified, or deleted tuples,
-    ou None if an error occurred.
-
-    :param errors: incidental error messages
-    :param exc_stmt: the command to execute
-    :param bind_vals: optional bind values
-    :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
-    :param logger: optional logger
-    :return: the return value from the command execution
-    """
-    # initialize the return variable
-    result: int | None = None
-
-    # make sure to have a connection
-    curr_conn: Connection = conn or connect(errors=errors,
-                                            autocommit=False,
-                                            logger=logger)
-
-    err_msg: str | None = None
-    try:
-        # obtain a cursor and execute the operation
-        with curr_conn.cursor() as cursor:
-            cursor.execute(statement=exc_stmt,
-                           parameters=bind_vals)
-            result = cursor.rowcount
-
-        # commit the transaction, if appropriate
-        if committable or not conn:
-            curr_conn.commit()
-    except Exception as e:
-        if curr_conn:
-            curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="oracle")
-    finally:
-        # close the connection, if locally acquired
-        if curr_conn and not conn:
-            curr_conn.close()
-
-    # log eventual errors
-    if errors or err_msg:
-        _db_log(logger=logger,
-                engine="oracle",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=exc_stmt,
-                bind_vals=bind_vals)
-
-    return result
-
-
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 # noinspection PyUnusedLocal
 def call_function(errors: list[str],
                   func_name: str,
                   func_vals: tuple,
                   conn: Connection,
                   committable: bool,
@@ -354,15 +356,15 @@
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: list[tuple] = []
 
     return result
@@ -378,15 +380,15 @@
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
```

### Comparing `pypomes_db-0.8.8/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.8.9/src/pypomes_db/postgres_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
@@ -132,83 +132,149 @@
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
-def bulk_insert(errors: list[str],
-                insert_stmt: str,
-                insert_vals: list[tuple],
-                conn: connection,
-                committable: bool,
-                logger: Logger) -> int:
+def execute(errors: list[str],
+            exc_stmt: str,
+            bind_vals: tuple,
+            conn: connection,
+            committable: bool,
+            logger: Logger) -> int:
     """
-    Insert the tuples, with values defined in *insert_vals*, into the database.
+    Execute the command *exc_stmt* on the database.
 
-    The *VALUES* clause in *insert_stmt* must be simply *VALUES %s*.
-    Note that, after the execution of *execute_values*, the *cursor.rowcount* property
-    will not contain a total result, and thus the value 1 (one) is returned on success.
+    This command might be a DML ccommand modifying the database, such as
+    inserting, updating or deleting tuples, or it might be a DDL statement,
+    or it might even be an environment-related command.
+    The optional bind values for this operation are in *bind_vals*.
+    The value returned is the value obtained from the execution of *exc_stmt*.
+    It might be the number of inserted, modified, or deleted tuples,
+    ou None if an error occurred.
 
     :param errors: incidental error messages
-    :param insert_stmt: the INSERT command
-    :param insert_vals: the list of values to be inserted
+    :param exc_stmt: the command to execute
+    :param bind_vals: optional bind values
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
-    :return: the number of inserted tuples, or None if an error occurred
+    :return: the return value from the command execution
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # make sure to have a connection
+    curr_conn: connection = conn or connect(errors=errors,
+                                            autocommit=False,
+                                            logger=logger)
+
+    err_msg: str | None = None
+    try:
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+            cursor.execute(query=f"{exc_stmt};",
+                           vars=bind_vals)
+            result = cursor.rowcount
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
+    except Exception as e:
+        if curr_conn:
+            curr_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="postgres")
+    finally:
+        # close the connection, if locally acquired
+        if curr_conn and not conn:
+            curr_conn.close()
+
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="postgres",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=exc_stmt,
+                bind_vals=bind_vals)
+
+    return result
+
+
+def bulk_execute(errors: list[str],
+                 exc_stmt: str,
+                 exc_vals: list[tuple],
+                 conn: connection,
+                 committable: bool,
+                 logger: Logger) -> int:
+    """
+    Bulk-update the database with the statement defined in *execute_stmt*, and the values in *execute_vals*.
+
+    For *INSERT* operations, the *VALUES* clause must be simply *VALUES %s*. *UPDATE* operations
+    require a sepcial syntax, with *VALUES %s* combined with a *FROM* clause.
+
+    :param errors: incidental error messages
+    :param exc_stmt: the command to update the database with
+    :param exc_vals: the list of values for tuple identification, and to update the database with
+    :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param logger: optional logger
+    :return: the number of inserted or updated tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
     curr_conn: connection = conn or connect(errors=errors,
                                             autocommit=False,
                                             logger=logger)
 
     # execute the bulk insert
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
+            # after the successful execution of 'execute_values', 'cursor.rowcount' has the value 1 (one)
             execute_values(cur=cursor,
-                           sql=insert_stmt,
-                           argslist=insert_vals)
-            result = len(insert_vals)
+                           sql=exc_stmt,
+                           argslist=exc_vals)
+            result = len(exc_vals)
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
     except ValueError as e:
         curr_conn.rollback()
         # is the exception ValueError("A string literal cannot contain NUL (0x00) characters.") ?
         if "contain NUL" in e.args[0]:
             # yes, log the occurrence, remove the NULLs, and try again
             _db_log(logger=logger,
                     engine="postgres",
                     level=WARNING,
-                    stmt=f"Found NULLs in values for {insert_stmt}")
+                    stmt=f"Found NULLs in values for {exc_stmt}")
             # search for NULLs in input data
             cleaned_rows: list[tuple[int, list]] = []
-            for inx, vals in enumerate(insert_vals):
+            for inx, vals in enumerate(exc_vals):
                 cleaned_row: list[Any] = _db_remove_nulls(vals)
                 # has the row been cleaned ?
                 if cleaned_row:
                     # yes, register it
                     cleaned_rows.append((inx, cleaned_row))
             # replace the cleaned rows
             for cleaned_row in cleaned_rows:
-                insert_vals[cleaned_row[0]] = tuple(cleaned_row[1])
+                exc_vals[cleaned_row[0]] = tuple(cleaned_row[1])
             # bulk insert the cleaned data
-            bulk_insert(errors=errors,
-                        insert_stmt=insert_stmt,
-                        insert_vals=insert_vals,
-                        conn=conn,
-                        committable=committable,
-                        logger=logger)
+            bulk_execute(errors=errors,
+                         exc_stmt=exc_stmt,
+                         exc_vals=exc_vals,
+                         conn=conn,
+                         committable=committable,
+                         logger=logger)
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
@@ -217,15 +283,15 @@
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
                 engine="postgres",
                 err_msg=err_msg,
                 errors=errors,
-                stmt=insert_stmt)
+                stmt=exc_stmt)
 
     return result
 
 
 def update_lob(errors: list[str],
                lob_table: str,
                lob_column: str,
@@ -243,15 +309,15 @@
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     """
     # make sure to have a connection
     curr_conn: connection = conn or connect(errors=errors,
                                             autocommit=False,
                                             logger=logger)
 
@@ -300,95 +366,28 @@
                 engine="postgres",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
-def db_execute(errors: list[str],
-               exc_stmt: str,
-               bind_vals: tuple,
-               conn: connection,
-               committable: bool,
-               logger: Logger) -> int:
-    """
-    Execute the command *exc_stmt* on the database.
-
-    This command might be a DML ccommand modifying the database, such as
-    inserting, updating or deleting tuples, or it might be a DDL statement,
-    or it might even be an environment-related command.
-    The optional bind values for this operation are in *bind_vals*.
-    The value returned is the value obtained from the execution of *exc_stmt*.
-    It might be the number of inserted, modified, or deleted tuples,
-    ou None if an error occurred.
-
-    :param errors: incidental error messages
-    :param exc_stmt: the command to execute
-    :param bind_vals: optional bind values
-    :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
-    :param logger: optional logger
-    :return: the return value from the command execution
-    """
-    # initialize the return variable
-    result: int | None = None
-
-    # make sure to have a connection
-    curr_conn: connection = conn or connect(errors=errors,
-                                            autocommit=False,
-                                            logger=logger)
-
-    err_msg: str | None = None
-    try:
-        # obtain a cursor and execute the operation
-        with curr_conn.cursor() as cursor:
-            cursor.execute(query=f"{exc_stmt};",
-                           vars=bind_vals)
-            result = cursor.rowcount
-
-        # commit the transaction, if appropriate
-        if committable or not conn:
-            curr_conn.commit()
-    except Exception as e:
-        if curr_conn:
-            curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="postgres")
-    finally:
-        # close the connection, if locally acquired
-        if curr_conn and not conn:
-            curr_conn.close()
-
-    # log eventual errors
-    if errors or err_msg:
-        _db_log(logger=logger,
-                engine="postgres",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=exc_stmt,
-                bind_vals=bind_vals)
-
-    return result
-
-
-
 def call_procedure(errors: list[str],
                    proc_name: str,
                    proc_vals: tuple,
                    conn: connection,
                    committable: bool,
                    logger: Logger) -> list[tuple]:
     """
     Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
 
     :param errors:  incidental error messages
     :param proc_name: the name of the sotred procedure
     :param proc_vals: the arguments to be passed
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] = [()]
 
     # make sure to have a connection
```

### Comparing `pypomes_db-0.8.8/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.8.9/src/pypomes_db/sqlserver_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
@@ -128,33 +128,100 @@
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
-def bulk_insert(errors: list[str],
-                insert_stmt: str,
-                insert_vals: list[tuple],
-                conn: Connection,
-                committable: bool,
-                logger: Logger) -> int:
+def execute(errors: list[str],
+            exc_stmt: str,
+            bind_vals: tuple,
+            conn: Connection,
+            committable: bool,
+            logger: Logger) -> int:
     """
-    Insert the tuples, with values defined in *insert_vals*, into the database.
+    Execute the command *exc_stmt* on the database.
 
-    The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
-    as there are elements in the tuples found in the list provided in *insert_vals*.
+    This command might be a DML ccommand modifying the database, such as
+    inserting, updating or deleting tuples, or it might be a DDL statement,
+    or it might even be an environment-related command.
+    The optional bind values for this operation are in *bind_vals*.
+    The value returned is the value obtained from the execution of *exc_stmt*.
+    It might be the number of inserted, modified, or deleted tuples,
+    ou None if an error occurred.
 
     :param errors: incidental error messages
-    :param insert_stmt: the INSERT command
-    :param insert_vals: the list of values to be inserted
+    :param exc_stmt: the command to execute
+    :param bind_vals: optional bind values
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
-    :return: the number of inserted tuples, or None if an error occurred
+    :return: the return value from the command execution
+    """
+    # initialize the return variable
+    result: int | None = None
+
+    # make sure to have a connection
+    curr_conn: Connection = conn or connect(errors=errors,
+                                            autocommit=False,
+                                            logger=logger)
+
+    err_msg: str | None = None
+    try:
+        # obtain a cursor and execute the operation
+        with curr_conn.cursor() as cursor:
+            cursor.execute(exc_stmt, bind_vals)
+            result = cursor.rowcount
+
+        # commit the transaction, if appropriate
+        if committable or not conn:
+            curr_conn.commit()
+    except Exception as e:
+        if curr_conn:
+            curr_conn.rollback()
+        err_msg = _db_except_msg(exception=e,
+                                 engine="sqlserver")
+    finally:
+        # close the connection, if locally acquired
+        if curr_conn and not conn:
+            curr_conn.close()
+
+    # log eventual errors
+    if errors or err_msg:
+        _db_log(logger=logger,
+                engine="sqlserver",
+                err_msg=err_msg,
+                errors=errors,
+                stmt=exc_stmt,
+                bind_vals=bind_vals)
+
+    return result
+
+
+def bulk_execute(errors: list[str],
+                 exc_stmt: str,
+                 exc_vals: list[tuple],
+                 conn: Connection,
+                 committable: bool,
+                 logger: Logger) -> int:
+    """
+    Bulk-update the database with the statement defined in *execute_stmt*, and the values in *execute_vals*.
+
+    The binding is done by position. Thus, the binding clauses in *execute_stmt* must contain as many '?'
+    placeholders as there are elements in the tuples found in the list provided in *execute_vals*.
+    Note that, in *UPDATE* operations, the placeholders in the *WHERE* clause will follow
+    the ones in the *SET* clause.
+
+    :param errors: incidental error messages
+    :param exc_stmt: the command to update the database with
+    :param exc_vals: the list of values for tuple identification, and to update the database with
+    :param conn: optional connection to use (obtains a new one, if not provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
+    :param logger: optional logger
+    :return: the number of inserted or updated tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
                                             autocommit=False,
@@ -162,16 +229,16 @@
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             cursor.fast_executemany = True
             try:
-                cursor.executemany(insert_stmt, insert_vals)
-                result = len(insert_vals)
+                cursor.executemany(exc_stmt, exc_vals)
+                result = len(exc_vals)
             except Exception:
                 conn.rollback()
                 raise
 
         # commit the transaction, if appropriate
         if committable or not conn:
             curr_conn.commit()
@@ -187,16 +254,16 @@
 
     # log eventual errors
     if errors or err_msg:
         _db_log(logger=logger,
                 engine="sqlserver",
                 err_msg=err_msg,
                 errors=errors,
-                stmt=insert_stmt,
-                bind_vals=insert_vals[0])
+                stmt=exc_stmt,
+                bind_vals=exc_vals[0])
 
     return result
 
 
 def update_lob(errors: list[str],
                lob_table: str,
                lob_column: str,
@@ -214,15 +281,15 @@
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     """
     # make sure to have a connection
     curr_conn: Connection = conn or connect(errors=errors,
                                             autocommit=False,
                                             logger=logger)
 
@@ -271,93 +338,28 @@
                 engine="sqlserver",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
-def execute(errors: list[str],
-            exc_stmt: str,
-            bind_vals: tuple,
-            conn: Connection,
-            committable: bool,
-            logger: Logger) -> int:
-    """
-    Execute the command *exc_stmt* on the database.
-
-    This command might be a DML ccommand modifying the database, such as
-    inserting, updating or deleting tuples, or it might be a DDL statement,
-    or it might even be an environment-related command.
-    The optional bind values for this operation are in *bind_vals*.
-    The value returned is the value obtained from the execution of *exc_stmt*.
-    It might be the number of inserted, modified, or deleted tuples,
-    ou None if an error occurred.
-
-    :param errors: incidental error messages
-    :param exc_stmt: the command to execute
-    :param bind_vals: optional bind values
-    :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
-    :param logger: optional logger
-    :return: the return value from the command execution
-    """
-    # initialize the return variable
-    result: int | None = None
-
-    # make sure to have a connection
-    curr_conn: Connection = conn or connect(errors=errors,
-                                            autocommit=False,
-                                            logger=logger)
-
-    err_msg: str | None = None
-    try:
-        # obtain a cursor and execute the operation
-        with curr_conn.cursor() as cursor:
-            cursor.execute(exc_stmt, bind_vals)
-            result = cursor.rowcount
-
-        # commit the transaction, if appropriate
-        if committable or not conn:
-            curr_conn.commit()
-    except Exception as e:
-        if curr_conn:
-            curr_conn.rollback()
-        err_msg = _db_except_msg(exception=e,
-                                 engine="sqlserver")
-    finally:
-        # close the connection, if locally acquired
-        if curr_conn and not conn:
-            curr_conn.close()
-
-    # log eventual errors
-    if errors or err_msg:
-        _db_log(logger=logger,
-                engine="sqlserver",
-                err_msg=err_msg,
-                errors=errors,
-                stmt=exc_stmt,
-                bind_vals=bind_vals)
-
-    return result
-
-
 def call_procedure(errors: list[str],
                    proc_name: str,
                    proc_vals: tuple,
                    conn: Connection,
                    committable: bool,
                    logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
     :param conn: optional connection to use (obtains a new one, if not provided)
-    :param committable: whether to commit upon errorless completion ('False' requires *conn* to be provided)
+    :param committable: whether to commit upon errorless completion ('False' requires 'conn' to be provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
     # make sure to have a connection
```

### Comparing `pypomes_db-0.8.8/LICENSE` & `pypomes_db-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.8/pyproject.toml` & `pypomes_db-0.8.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.8.8"
+version = "0.8.9"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -20,15 +20,15 @@
 ]
 dependencies = [
     "pip>=24.0",
 #   "mysql-connector-python>=8.4.0",
 #   "oracledb>=2.2.0",
 #   "psycopg2-binary>=2.9.9",
 #   "pyodbc>=5.1.0",
-    "pypomes_core>=1.0.5",
+    "pypomes_core>=1.0.7",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-DB"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes-DB/issues"
```

### Comparing `pypomes_db-0.8.8/PKG-INFO` & `pypomes_db-0.8.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.8.8
+Version: 0.8.9
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=1.0.5
+Requires-Dist: pypomes-core>=1.0.7
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

