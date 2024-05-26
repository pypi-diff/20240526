# Comparing `tmp/transdoc-0.2.2.tar.gz` & `tmp/transdoc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transdoc-0.2.2.tar", max compression
+gzip compressed data, was "transdoc-0.2.3.tar", max compression
```

## Comparing `transdoc-0.2.2.tar` & `transdoc-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1073 2024-04-22 11:34:36.998222 transdoc-0.2.2/LICENSE
--rw-r--r--   0        0        0     3932 2024-04-22 11:34:36.998222 transdoc-0.2.2/README.md
--rw-r--r--   0        0        0     1463 2024-04-22 11:34:36.998222 transdoc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1335 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/__cli/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/__cli/mutex.py
--rw-r--r--   0        0        0      648 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/__collect_rules.py
--rw-r--r--   0        0        0       74 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/__consts.py
--rw-r--r--   0        0        0      364 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/__init__.py
--rw-r--r--   0        0        0      201 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/__main__.py
--rw-r--r--   0        0        0     5361 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/__processor.py
--rw-r--r--   0        0        0      228 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/__rule.py
--rw-r--r--   0        0        0    10125 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/__transformer.py
--rw-r--r--   0        0        0      888 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/errors.py
--rw-r--r--   0        0        0        0 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/py.typed
--rw-r--r--   0        0        0     4661 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/rules/__attributes.py
--rw-r--r--   0        0        0      387 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/rules/__file_contents.py
--rw-r--r--   0        0        0      381 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/rules/__init__.py
--rw-r--r--   0        0        0     1294 2024-04-22 11:34:36.998222 transdoc-0.2.2/transdoc/rules/__markdown_docs_link.py
--rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 transdoc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-26 12:48:10.416456 transdoc-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3932 2024-05-26 12:48:10.416456 transdoc-0.2.3/README.md
+-rw-r--r--   0        0        0     1463 2024-05-26 12:48:10.416456 transdoc-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1335 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/__cli/__init__.py
+-rw-r--r--   0        0        0     1277 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/__cli/mutex.py
+-rw-r--r--   0        0        0      648 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/__collect_rules.py
+-rw-r--r--   0        0        0       74 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/__consts.py
+-rw-r--r--   0        0        0      364 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/__init__.py
+-rw-r--r--   0        0        0      201 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/__main__.py
+-rw-r--r--   0        0        0     5361 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/__processor.py
+-rw-r--r--   0        0        0      228 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/__rule.py
+-rw-r--r--   0        0        0    10491 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/__transformer.py
+-rw-r--r--   0        0        0      888 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/errors.py
+-rw-r--r--   0        0        0        0 2024-05-26 12:48:10.416456 transdoc-0.2.3/transdoc/py.typed
+-rw-r--r--   0        0        0     4661 2024-05-26 12:48:10.420456 transdoc-0.2.3/transdoc/rules/__attributes.py
+-rw-r--r--   0        0        0      387 2024-05-26 12:48:10.420456 transdoc-0.2.3/transdoc/rules/__file_contents.py
+-rw-r--r--   0        0        0      381 2024-05-26 12:48:10.420456 transdoc-0.2.3/transdoc/rules/__init__.py
+-rw-r--r--   0        0        0     1294 2024-05-26 12:48:10.420456 transdoc-0.2.3/transdoc/rules/__markdown_docs_link.py
+-rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 transdoc-0.2.3/PKG-INFO
```

### Comparing `transdoc-0.2.2/LICENSE` & `transdoc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.2/README.md` & `transdoc-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.2/pyproject.toml` & `transdoc-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "transdoc"
-version = "0.2.2"
+version = "0.2.3"
 description = "A simple tool for transforming Python docstrings by embedding results from Python function calls"
 authors = ["Miguel Guthridge <hello@miguelguthridge.com>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/MiguelGuthridge/transdoc"
 # documentation = "https://miguelguthridge.github.io/transdoc/"
```

### Comparing `transdoc-0.2.2/transdoc/__cli/__init__.py` & `transdoc-0.2.3/transdoc/__cli/__init__.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.2/transdoc/__cli/mutex.py` & `transdoc-0.2.3/transdoc/__cli/mutex.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.2/transdoc/__collect_rules.py` & `transdoc-0.2.3/transdoc/__collect_rules.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.2/transdoc/__processor.py` & `transdoc-0.2.3/transdoc/__processor.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.2/transdoc/__transformer.py` & `transdoc-0.2.3/transdoc/__transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,20 @@
     CodeType,
     TracebackType,
     FrameType,
     type,
 ]
 
 
+def indent_by(amount: int, string: str) -> str:
+    return '\n'.join(
+        [f"{' ' * amount}{line.rstrip()}" for line in string.splitlines()]
+    ).lstrip()
+
+
 class DocTransformer(cst.CSTTransformer):
     """
     Rewrite documentation.
     """
     METADATA_DEPENDENCIES = (PositionProvider,)
 
     def __init__(self, rules: dict[str, Rule]) -> None:
@@ -106,47 +112,52 @@
             self.__report_error(
                 position,
                 TransdocNameError(f"unknown rule '{rule_name}'"),
             )
             return True
         return False
 
-    def __eval_rule(self, rule: str, position: CodePosition) -> str:
+    def __eval_rule(
+        self,
+        rule: str,
+        position: CodePosition,
+        indent: int,
+    ) -> str:
         """
         Execute a command, alongside the given set of rules.
         """
         # if it's just a function name, evaluate it as a call with no arguments
         if rule.isidentifier():
             if self.__report_rule_if_unknown(rule, position):
                 return ""
             try:
-                return self.__rules[rule]()
+                return indent_by(indent, self.__rules[rule]())
             except Exception as e:
                 self.__report_error(position, e)
                 return ""
         # If it uses square brackets, then extract the contained string, and
         # pass that
         if rule.split('[')[0].isidentifier() and rule.endswith(']'):
             rule_name, *content = rule.split('[')
             content_str = '['.join(content).removesuffix(']')
             if self.__report_rule_if_unknown(rule_name, position):
                 return ""
             try:
-                return self.__rules[rule_name](content_str)
+                return indent_by(indent, self.__rules[rule_name](content_str))
             except Exception as e:
                 self.__report_error(position, e)
                 return ""
         # Otherwise, it should be a regular function call
         # This calls `eval` with the rules dictionary set as the globals, since
         # otherwise it'd just be too complex to parse things.
         if rule.split('(')[0].isidentifier() and rule.endswith(')'):
             if self.__report_rule_if_unknown(rule.split('(')[0], position):
                 return ""
             try:
-                return eval(rule, self.__rules)
+                return indent_by(indent, eval(rule, self.__rules))
             except Exception as e:
                 self.__report_error(position, e)
                 return ""
 
         # If we reach this point, it's not valid data, and we should give an
         # error
         self.__report_error(
@@ -167,14 +178,16 @@
         # Perhaps I could use a state machine or something?
         new_doc = StringIO()
         cmd_buffer = StringIO()
         in_cmd_buffer = False
         brace_count = 0
         cmd_start_position: Optional[CodePosition] = None
 
+        indent_level = self.__get_position().column
+
         # Column offset starts at 3 to account for stripped out triple-quotes
         col_offset = 3
         line_offset = 0
         for c in docstring:
             if in_cmd_buffer:
                 # FIXME: This assumes that all instances of `}}` close the
                 # buffer, which isn't necessarily the case. This will break
@@ -184,14 +197,15 @@
                     if brace_count == 2:
                         # End of command, let's execute it
                         cmd_buffer.seek(0)
                         assert cmd_start_position is not None
                         new_doc.write(self.__eval_rule(
                             cmd_buffer.read(),
                             cmd_start_position,
+                            indent_level,
                         ))
                         cmd_buffer = StringIO()
                         in_cmd_buffer = False
                         cmd_start_position = None
                         brace_count = 0
                 else:
                     # If we previously found a closing brace
```

### Comparing `transdoc-0.2.2/transdoc/errors.py` & `transdoc-0.2.3/transdoc/errors.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.2/transdoc/rules/__attributes.py` & `transdoc-0.2.3/transdoc/rules/__attributes.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.2/transdoc/rules/__markdown_docs_link.py` & `transdoc-0.2.3/transdoc/rules/__markdown_docs_link.py`

 * *Files identical despite different names*

### Comparing `transdoc-0.2.2/PKG-INFO` & `transdoc-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transdoc
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple tool for transforming Python docstrings by embedding results from Python function calls
 Home-page: https://github.com/MiguelGuthridge/transdoc
 License: MIT
 Keywords: documentation,source,transform,parse,pre-processor
 Author: Miguel Guthridge
 Author-email: hello@miguelguthridge.com
 Requires-Python: >=3.10,<4.0
```

