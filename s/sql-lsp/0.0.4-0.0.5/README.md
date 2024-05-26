# Comparing `tmp/sql_lsp-0.0.4.tar.gz` & `tmp/sql_lsp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_lsp-0.0.4.tar", max compression
+gzip compressed data, was "sql_lsp-0.0.5.tar", max compression
```

## Comparing `sql_lsp-0.0.4.tar` & `sql_lsp-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1624 2024-05-06 02:35:19.504764 sql_lsp-0.0.4/README.md
--rw-r--r--   0        0        0      539 2024-05-06 02:35:44.950919 sql_lsp-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 03:55:22.443530 sql_lsp-0.0.4/sql_lsp/__init__.py
--rw-r--r--   0        0        0       71 2024-05-05 03:55:22.443530 sql_lsp-0.0.4/sql_lsp/__main__.py
--rw-r--r--   0        0        0     6169 2024-05-05 03:55:22.443530 sql_lsp-0.0.4/sql_lsp/completion.py
--rw-r--r--   0        0        0      321 2024-05-05 03:55:22.443530 sql_lsp-0.0.4/sql_lsp/config.py
--rw-r--r--   0        0        0     2369 2024-05-05 03:55:22.443530 sql_lsp-0.0.4/sql_lsp/database.py
--rw-r--r--   0        0        0     7885 2024-05-05 22:35:06.934031 sql_lsp-0.0.4/sql_lsp/mysql_connector.py
--rw-r--r--   0        0        0     9783 2024-05-06 02:35:50.564952 sql_lsp-0.0.4/sql_lsp/server.py
--rw-r--r--   0        0        0     3966 2024-05-05 03:55:22.443530 sql_lsp-0.0.4/sql_lsp/utils.py
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 sql_lsp-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1624 2024-05-06 02:35:19.504764 sql_lsp-0.0.5/README.md
+-rw-r--r--   0        0        0      539 2024-05-26 21:50:23.592151 sql_lsp-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-05 03:55:22.443530 sql_lsp-0.0.5/sql_lsp/__init__.py
+-rw-r--r--   0        0        0       71 2024-05-05 03:55:22.443530 sql_lsp-0.0.5/sql_lsp/__main__.py
+-rw-r--r--   0        0        0     6169 2024-05-24 04:20:41.975414 sql_lsp-0.0.5/sql_lsp/completion.py
+-rw-r--r--   0        0        0      329 2024-05-24 05:19:48.464502 sql_lsp-0.0.5/sql_lsp/config.py
+-rw-r--r--   0        0        0     2369 2024-05-05 03:55:22.443530 sql_lsp-0.0.5/sql_lsp/database.py
+-rw-r--r--   0        0        0     7991 2024-05-24 05:15:54.405504 sql_lsp-0.0.5/sql_lsp/mysql_connector.py
+-rw-r--r--   0        0        0    10831 2024-05-26 21:50:30.576400 sql_lsp-0.0.5/sql_lsp/server.py
+-rw-r--r--   0        0        0     4677 2024-05-24 05:26:46.789314 sql_lsp-0.0.5/sql_lsp/utils.py
+-rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 sql_lsp-0.0.5/PKG-INFO
```

### Comparing `sql_lsp-0.0.4/README.md` & `sql_lsp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sql_lsp-0.0.4/pyproject.toml` & `sql_lsp-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 sql-ls = "sql_lsp.__main__:main"
 
 [tool.poetry]
 name = "sql-lsp"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Chahak Mehta <chahakmehta013@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pygls = "^1.1.1"
```

### Comparing `sql_lsp-0.0.4/sql_lsp/completion.py` & `sql_lsp-0.0.5/sql_lsp/completion.py`

 * *Files identical despite different names*

### Comparing `sql_lsp-0.0.4/sql_lsp/database.py` & `sql_lsp-0.0.5/sql_lsp/database.py`

 * *Files identical despite different names*

### Comparing `sql_lsp-0.0.4/sql_lsp/mysql_connector.py` & `sql_lsp-0.0.5/sql_lsp/mysql_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,16 @@
         str
             Help string from the manual if a valid function.
 
         """
         keyword_lower = keyword.lower()
         if keyword_lower in self.table_cache:
             return self.table_cache[keyword_lower].description
+        if keyword_lower in self.column_cache:
+            return str(self.column_cache[keyword.lower()])
         if keyword_lower in self.help_cache:
             return self.help_cache.get(keyword_lower, "")
 
     def get_tables(self) -> ValuesView[TableInfo]:
         """Fetch dictionary of table and their types."""
         logger.info(f"Table cache: {self.table_cache}")
         return self.table_cache.values()
```

### Comparing `sql_lsp-0.0.4/sql_lsp/server.py` & `sql_lsp-0.0.5/sql_lsp/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import logging.config
 import os
+import traceback
 
 import sqlfluff
 
 from pathlib import Path
 from typing import override, TypedDict, ParamSpec
 
 from lsprotocol import validators
@@ -28,22 +29,30 @@
     Hover,
     HoverParams,
     InitializeParams,
     Position,
     Range,
     TextEdit,
 )
+
+from sqlfluff.core import Lexer, Parser
 from pygls.server import LanguageServer
 from pygls.protocol import LanguageServerProtocol, lsp_method
 from pygls.workspace import TextDocument
 
 from .completion import get_completion_candidates
 from .config import fluff_config
 from .database import DBConnection, ConnectionConfig
-from .utils import current_word_range, get_text_in_range, tabulate_result
+from .utils import (
+    current_word_range,
+    get_current_query_statement,
+    get_text_in_range,
+    tabulate_result,
+    get_query_statements,
+)
 
 P = ParamSpec("P")
 
 sqlfluff_logger = logging.getLogger("sqlfluff")
 sqlfluff_logger.setLevel(logging.WARNING)
 sqlfluff_rules_logger = logging.getLogger("sqlfluff.rules.reflow")
 sqlfluff_rules_logger.setLevel(logging.WARNING)
@@ -87,15 +96,15 @@
             self.available_connections = server_config["connections"]
             self.dbconn = DBConnection(
                 config=list(self.available_connections.values())[0]
             )
         return super().lsp_initialize(params)
 
 
-sql_server = LanguageServer("sql-ls", "v0.0.4", protocol_cls=SqlLanguageServerProtocol)
+sql_server = LanguageServer("sql-ls", "v0.0.5", protocol_cls=SqlLanguageServerProtocol)
 
 
 def _publish_diagnostics(ls: LanguageServer, uri: str):
     """Publish diagnostics to LSP server."""
     document = ls.workspace.get_text_document(uri)
     lint_diagnostics = sqlfluff.lint(
         document.source, dialect="mysql", config=fluff_config
@@ -117,15 +126,14 @@
 
 
 @sql_server.feature(TEXT_DOCUMENT_COMPLETION)
 def completions(ls: LanguageServer, params: CompletionParams):
     items = []
     document = ls.workspace.get_document(params.text_document.uri)
     items = get_completion_candidates(document, params.position, ls.lsp.dbconn)
-    logger.info(f"Completion items: {items}")
     return CompletionList(is_incomplete=False, items=items)
 
 
 @sql_server.feature(TEXT_DOCUMENT_DID_OPEN)
 async def did_open(ls: LanguageServer, params: DidOpenTextDocumentParams):
     _publish_diagnostics(ls, params.text_document.uri)
 
@@ -189,16 +197,18 @@
         Command(title="Show Databases", command="showDatabases"),
         Command(title="Show Connections", command="showConnections"),
         Command(
             title="Switch Connections",
             command="switchConnections",
             arguments=[params],
         ),
+        Command(
+            title="Show Tables in Database", command="showTables", arguments=[params]
+        ),
     ]
-    logger.info(f"Trying to send: {commands}")
     return commands
 
 
 # NOTE: While the type for `args` is a tuple of `TextDocument` and
 # `CodeActionParams`, the actual parameters that get passed into the
 # function by pygls is actually a dictionary version of the classes.
 # Hence, to access the values, we use dictionary keys instead of
@@ -210,20 +220,31 @@
     """Execute query."""
     if not ls.lsp.dbconn:
         raise KeyError(
             "DB Connection not found on server. `LanguageServer`"
             + " might not have been initialzied with `LanguageServerProtocol`."
             + " Please check."
         )
-    logger.info(f"chahak: execute_query (args): {args}")
     document_args = args[0][0]
     document = ls.workspace.get_text_document(document_args["uri"])
+
+    lexer = Lexer(config=fluff_config)
+    parser = Parser(config=fluff_config)
+    parsed_query = parser.parse(lexer.lex(document.source)[0])
+    segments = parsed_query.segments
+    statements = get_query_statements(segments)
+
     action_params = args[0][1]
-    query = get_text_in_range(document, action_params["range"])
-    logger.info(f"execute_query(query): {query}")
+    cursor_position = action_params["range"]["start"]
+
+    current_statement = get_current_query_statement(segments, cursor_position)
+    if current_statement is None:
+        return ""
+
+    query = current_statement.raw
     rows, error = ls.lsp.dbconn.execute_query(query)
     if error is not None:
         return str(error)
     return tabulate_result(rows)
 
 
 @sql_server.command("explainQuery")
@@ -233,60 +254,77 @@
     """Execute query."""
     if not ls.lsp.dbconn:
         raise KeyError(
             "DB Connection not found on server. `LanguageServer`"
             + " might not have been initialzied with `LanguageServerProtocol`."
             + " Please check."
         )
-    logger.info(f"explain_query (args): {args}")
     document_args = args[0][0]
     document = ls.workspace.get_text_document(document_args["uri"])
     action_params = args[0][1]
     query = "explain " + get_text_in_range(document, action_params["range"])
-    logger.info(f"execute_query(query): {query}")
     rows, error = ls.lsp.dbconn.execute_query(query)
     if error is not None:
         return str(error)
     return tabulate_result(rows)
 
 
 @sql_server.command("showDatabases")
-def show_databases(ls: LanguageServer) -> str:
+def show_databases(ls: LanguageServer, *args) -> str:
     """Show Databases in the connection."""
     if not ls.lsp.dbconn:
         raise KeyError(
             "DB Connection not found on server. `LanguageServer`"
             + " might not have been initialzied with `LanguageServerProtocol`."
             + " Please check."
         )
     query = "show databases;"
-    rows = ls.lsp.dbconn.execute_query(query)
+    rows, error = ls.lsp.dbconn.execute_query(query)
+    if error is not None:
+        return "".join(traceback.format_exception(e))
     return tabulate_result(rows)
 
 
 @sql_server.command("showConnections")
-def show_connections(ls: LanguageServer) -> str:
+def show_connections(ls: LanguageServer, *args) -> str:
     """Show available connections."""
     return tabulate_result(
         [
             {"alias": alias, **conn, "password": "****"}
             for alias, conn in ls.lsp.available_connections.items()
         ]
     )
 
 
+@sql_server.command("showTables")
+def show_databases(ls: LanguageServer, *args) -> str:
+    """Show Databases in the connection."""
+    if not ls.lsp.dbconn:
+        raise KeyError(
+            "DB Connection not found on server. `LanguageServer`"
+            + " might not have been initialzied with `LanguageServerProtocol`."
+            + " Please check."
+        )
+    query = "show tables;"
+    rows, error = ls.lsp.dbconn.execute_query(query)
+    if error is not None:
+        return "".join(traceback.format_exception(e))
+    return tabulate_result(rows)
+
+
 @sql_server.command("showConnectionAliases")
-def show_connection_aliases(ls: LanguageServer) -> str:
+def show_connection_aliases(ls: LanguageServer, *args) -> str:
     """Show aliases for all the connections.
 
     Useful for providing a selection list to switch connections.
     """
     return "\n".join(list(ls.lsp.available_connections.keys()))
 
 
 @sql_server.command("switchConnections")
 def switch_connections(ls: LanguageServer, *args: tuple[CodeActionParams]):
     """Switch Databases in the connection."""
-    selected_alias = args[0][0]
+    selected_alias = args[0][0]["connection"]
     selected_config = ls.lsp.available_connections[selected_alias]
     ls.lsp.dbconn = DBConnection(selected_config)
     ls.send_notification(f"Changed DB Connection to {selected_alias}")
+    return selected_alias
```

### Comparing `sql_lsp-0.0.4/sql_lsp/utils.py` & `sql_lsp-0.0.5/sql_lsp/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import logging
 
 from collections.abc import Iterator
 from typing import Any, TypedDict
 
 from lsprotocol.types import Position, Range
 from pygls.workspace import TextDocument
+from sqlfluff.core.parser import RawSegment
+from sqlfluff.core.parser.segments import UnparsableSegment
 from sqlfluff.core.parser.segments.base import RecordSerialisedSegment
+from sqlfluff.dialects.dialect_ansi import StatementSegment
 from tabulate import tabulate
 
 logger = logging.getLogger(__file__)
 
 
 def current_word_range(document: TextDocument, position: Position) -> Range | None:
     """Get the range of the word under the cursor."""
@@ -60,19 +63,16 @@
         )
 
     if first_line_index == last_line_index:
         if first_char_index == last_char_index:
             return "\n".join(doc_lines)
         return doc_lines[first_line_index][first_char_index:last_char_index]
 
-    logger.debug("utils (doc_lines):")
-    logger.debug(f"{doc_lines}")
     lines: list[str] = []
     for i in range(first_line_index - 1, last_line_index):
-        logger.debug(f"Line: {i} of {len(doc_lines) - 1}")
         if i == first_line_index:
             lines.append(doc_lines[i][first_char_index:])
         elif i == last_line_index:
             lines.append(doc_lines[i][:last_char_index])
         elif i < len(doc_lines) - 1:
             lines.append(doc_lines[i])
     return "\n".join(lines)
@@ -101,7 +101,28 @@
         if k == segment_type:
             yield v
         elif isinstance(v, dict):
             yield from get_json_segment(v, segment_type)
         elif isinstance(v, list):
             for s in v:
                 yield from get_json_segment(s, segment_type)
+
+
+def get_query_statements(segments: list[RawSegment]):
+    statements: list[StatementSegment] = []
+    for segment in segments:
+        if isinstance(segment, StatementSegment) or isinstance(
+            segment, UnparsableSegment
+        ):
+            statements.append(segment)
+    return statements
+
+
+def get_current_query_statement(
+    segments: list[RawSegment], cursor_position: PositionAsDict
+):
+    statements = get_query_statements(segments)
+    for statement in statements:
+        start_line, _ = statement.get_start_loc()
+        end_line, _ = statement.get_end_loc()
+        if start_line <= cursor_position["line"] + 1 <= end_line:
+            return statement
```

### Comparing `sql_lsp-0.0.4/PKG-INFO` & `sql_lsp-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-lsp
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Chahak Mehta
 Author-email: chahakmehta013@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mysql-connector (>=8.2.0,<9.0.0)
```

