# Comparing `tmp/cdmn-2.1.1.tar.gz` & `tmp/cdmn-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdmn-2.1.1.tar", last modified: Mon Jan 22 12:23:53 2024, max compression
+gzip compressed data, was "cdmn-2.1.2.tar", last modified: Sun May 26 08:43:06 2024, max compression
```

## Comparing `cdmn-2.1.1.tar` & `cdmn-2.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2024-01-22 12:23:53.990495 cdmn-2.1.1/
--rw-r--r--   0 sva       (1000) sva       (1001)    35065 2020-11-22 20:11:44.000000 cdmn-2.1.1/LICENSE
--rw-r--r--   0 sva       (1000) sva       (1001)     2341 2024-01-22 12:23:53.990495 cdmn-2.1.1/PKG-INFO
--rw-r--r--   0 sva       (1000) sva       (1001)     2064 2022-11-15 07:18:19.000000 cdmn-2.1.1/README.md
-drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2024-01-22 12:23:53.990495 cdmn-2.1.1/cdmn/
--rw-r--r--   0 sva       (1000) sva       (1001)    19231 2024-01-22 10:35:03.000000 cdmn-2.1.1/cdmn/API.py
--rw-r--r--   0 sva       (1000) sva       (1001)        0 2021-12-28 13:29:55.000000 cdmn-2.1.1/cdmn/__init__.py
--rw-r--r--   0 sva       (1000) sva       (1001)     7480 2024-01-22 12:23:15.000000 cdmn-2.1.1/cdmn/cdmn.py
--rw-r--r--   0 sva       (1000) sva       (1001)    32459 2024-01-22 07:53:30.000000 cdmn-2.1.1/cdmn/glossary.py
--rw-r--r--   0 sva       (1000) sva       (1001)    10299 2024-01-22 08:53:03.000000 cdmn-2.1.1/cdmn/idply.py
--rw-r--r--   0 sva       (1000) sva       (1001)      753 2021-12-28 13:29:55.000000 cdmn-2.1.1/cdmn/idpname.py
--rw-r--r--   0 sva       (1000) sva       (1001)     5462 2024-01-22 10:43:56.000000 cdmn-2.1.1/cdmn/interpret.py
--rw-r--r--   0 sva       (1000) sva       (1001)    22268 2024-01-22 08:53:03.000000 cdmn-2.1.1/cdmn/parse_xml.py
--rw-r--r--   0 sva       (1000) sva       (1001)    10347 2024-01-22 08:53:11.000000 cdmn-2.1.1/cdmn/parsetab.py
--rw-r--r--   0 sva       (1000) sva       (1001)     2944 2022-11-15 07:11:39.000000 cdmn-2.1.1/cdmn/post_process.py
--rw-r--r--   0 sva       (1000) sva       (1001)    22639 2024-01-22 10:35:03.000000 cdmn-2.1.1/cdmn/table.py
--rw-r--r--   0 sva       (1000) sva       (1001)    24084 2024-01-22 10:44:05.000000 cdmn-2.1.1/cdmn/table_operations.py
-drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2024-01-22 12:23:53.990495 cdmn-2.1.1/cdmn.egg-info/
--rw-r--r--   0 sva       (1000) sva       (1001)     2341 2024-01-22 12:23:53.000000 cdmn-2.1.1/cdmn.egg-info/PKG-INFO
--rw-r--r--   0 sva       (1000) sva       (1001)      398 2024-01-22 12:23:53.000000 cdmn-2.1.1/cdmn.egg-info/SOURCES.txt
--rw-r--r--   0 sva       (1000) sva       (1001)        1 2024-01-22 12:23:53.000000 cdmn-2.1.1/cdmn.egg-info/dependency_links.txt
--rw-r--r--   0 sva       (1000) sva       (1001)       40 2024-01-22 12:23:53.000000 cdmn-2.1.1/cdmn.egg-info/entry_points.txt
--rw-r--r--   0 sva       (1000) sva       (1001)       69 2024-01-22 12:23:53.000000 cdmn-2.1.1/cdmn.egg-info/requires.txt
--rw-r--r--   0 sva       (1000) sva       (1001)        5 2024-01-22 12:23:53.000000 cdmn-2.1.1/cdmn.egg-info/top_level.txt
--rw-r--r--   0 sva       (1000) sva       (1001)       38 2024-01-22 12:23:53.990495 cdmn-2.1.1/setup.cfg
--rw-r--r--   0 sva       (1000) sva       (1001)      716 2024-01-22 12:22:52.000000 cdmn-2.1.1/setup.py
+drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2024-05-26 08:43:06.963555 cdmn-2.1.2/
+-rw-r--r--   0 sva       (1000) sva       (1001)    35065 2020-11-22 20:11:44.000000 cdmn-2.1.2/LICENSE
+-rw-r--r--   0 sva       (1000) sva       (1001)     2477 2024-05-26 08:43:06.963555 cdmn-2.1.2/PKG-INFO
+-rw-r--r--   0 sva       (1000) sva       (1001)     2064 2022-11-15 07:18:19.000000 cdmn-2.1.2/README.md
+drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2024-05-26 08:43:06.960222 cdmn-2.1.2/cdmn/
+-rw-r--r--   0 sva       (1000) sva       (1001)    19231 2024-05-26 06:41:25.000000 cdmn-2.1.2/cdmn/API.py
+-rw-r--r--   0 sva       (1000) sva       (1001)        0 2021-12-28 13:29:55.000000 cdmn-2.1.2/cdmn/__init__.py
+-rw-r--r--   0 sva       (1000) sva       (1001)     7491 2024-05-26 08:41:09.000000 cdmn-2.1.2/cdmn/cdmn.py
+-rw-r--r--   0 sva       (1000) sva       (1001)    31947 2024-05-26 06:41:25.000000 cdmn-2.1.2/cdmn/glossary.py
+-rw-r--r--   0 sva       (1000) sva       (1001)    10598 2024-05-26 06:41:25.000000 cdmn-2.1.2/cdmn/idply.py
+-rw-r--r--   0 sva       (1000) sva       (1001)      753 2021-12-28 13:29:55.000000 cdmn-2.1.2/cdmn/idpname.py
+-rw-r--r--   0 sva       (1000) sva       (1001)     6086 2024-05-26 06:41:25.000000 cdmn-2.1.2/cdmn/interpret.py
+-rw-r--r--   0 sva       (1000) sva       (1001)    22268 2024-01-22 08:53:03.000000 cdmn-2.1.2/cdmn/parse_xml.py
+-rw-r--r--   0 sva       (1000) sva       (1001)    10347 2024-04-08 06:51:53.000000 cdmn-2.1.2/cdmn/parsetab.py
+-rw-r--r--   0 sva       (1000) sva       (1001)     2579 2024-04-08 06:55:10.000000 cdmn-2.1.2/cdmn/post_process.py
+-rw-r--r--   0 sva       (1000) sva       (1001)    28001 2024-05-26 08:33:37.000000 cdmn-2.1.2/cdmn/table.py
+-rw-r--r--   0 sva       (1000) sva       (1001)    24100 2024-04-08 06:55:10.000000 cdmn-2.1.2/cdmn/table_operations.py
+drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2024-05-26 08:43:06.963555 cdmn-2.1.2/cdmn.egg-info/
+-rw-r--r--   0 sva       (1000) sva       (1001)     2477 2024-05-26 08:43:06.000000 cdmn-2.1.2/cdmn.egg-info/PKG-INFO
+-rw-r--r--   0 sva       (1000) sva       (1001)      398 2024-05-26 08:43:06.000000 cdmn-2.1.2/cdmn.egg-info/SOURCES.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)        1 2024-05-26 08:43:06.000000 cdmn-2.1.2/cdmn.egg-info/dependency_links.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)       40 2024-05-26 08:43:06.000000 cdmn-2.1.2/cdmn.egg-info/entry_points.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)       61 2024-05-26 08:43:06.000000 cdmn-2.1.2/cdmn.egg-info/requires.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)        5 2024-05-26 08:43:06.000000 cdmn-2.1.2/cdmn.egg-info/top_level.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)       38 2024-05-26 08:43:06.963555 cdmn-2.1.2/setup.cfg
+-rw-r--r--   0 sva       (1000) sva       (1001)      708 2024-05-26 08:40:43.000000 cdmn-2.1.2/setup.py
```

### Comparing `cdmn-2.1.1/LICENSE` & `cdmn-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdmn-2.1.1/PKG-INFO` & `cdmn-2.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: cdmn
-Version: 2.1.1
-Summary: A package providing a (c)DMN solver and API
-Home-page: http://cdmn.be
-Author: Simon Vandevelde
-Author-email: s.vandevelde@kuleuven.be
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cDMN
 
 ## Welcome to the cDMN solver's code repository.
 
 cDMN stands for Constraint Decision and Model Notation.
 It is an extension to the [DMN](https://www.omg.org/spec/DMN/About-DMN/) standard, managed by the Object Management Group (OMG).
 cDMN combines the readability and straighforwardness of DMN and the expressiveness and flexibility of constraint reasoning.
```

### Comparing `cdmn-2.1.1/README.md` & `cdmn-2.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: cdmn
+Version: 2.1.2
+Summary: A package providing a (c)DMN solver and API
+Home-page: http://cdmn.be
+Author: Simon Vandevelde
+Author-email: s.vandevelde@kuleuven.be
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: openpyxl==3.0.10
+Requires-Dist: ply==3.11
+Requires-Dist: numpy
+Requires-Dist: python-dateutil
+Requires-Dist: Levenshtein
+
 # cDMN
 
 ## Welcome to the cDMN solver's code repository.
 
 cDMN stands for Constraint Decision and Model Notation.
 It is an extension to the [DMN](https://www.omg.org/spec/DMN/About-DMN/) standard, managed by the Object Management Group (OMG).
 cDMN combines the readability and straighforwardness of DMN and the expressiveness and flexibility of constraint reasoning.
```

### Comparing `cdmn-2.1.1/cdmn/API.py` & `cdmn-2.1.2/cdmn/API.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import copy
 from typing import Dict, List
 from contextlib import redirect_stdout
 
 try:
     from idp_engine import IDP
 except ImportError:
-    print("You need to install the 'idp_engine' package to use the API.")
+    print("You need to install the 'idp-engine' package to use the API.")
     import sys
     sys.exit(1)
 
 
 class DMNError(Exception):
     """ Base class for all DMN-related exceptions """
     pass
```

### Comparing `cdmn-2.1.1/cdmn/cdmn.py` & `cdmn-2.1.2/cdmn/cdmn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    Copyright 2020 Simon Vandevelde, Bram Aerts, Joost Vennekens
+    Copyright 2020-now Simon Vandevelde, Bram Aerts, Joost Vennekens
     This code is licensed under GNU GPLv3 license (see LICENSE) for more
     information.
     This file is part of the cDMN solver.
 """
 import argparse
 from cdmn.glossary import Glossary
 from cdmn.interpret import VariableInterpreter
@@ -59,15 +59,15 @@
     """
     The main function for the cDMN solver.
     """
 
     # Parse the arguments.
     argparser = argparse.ArgumentParser(description='Run cDMN on DMN tables.')
     argparser.add_argument('--version', '-v', action='version',
-                           version='2.1.1')
+                           version='2.1.2')
     argparser.add_argument('path_to_file', metavar='path_to_file', type=str,
                            help='the path to the xlsx or xml file')
     argparser.add_argument('-n', '--name', metavar='name_of_sheet', type=str,
                            help='the name(s) of the sheet(s) to execute',
                            nargs='+')
     argparser.add_argument('--all-sheets', dest='all_sheets',
                            help='the name(s) of the sheet(s) to execute',
@@ -169,17 +169,17 @@
         fp.close()
 
     # If the IDP-Z3 system was requested, run the idp_engine.
     if args.idp_z3:
         try:
             from idp_engine.Parse import idpparser
         except ImportError:
-            print("You need to install the idp-engine package if you wish to"
-                  " run your cDMN.")
-            pass
+            print("You need to install the idp-engine package"
+                  "if you wish to run your cDMN.")
+            sys.exit(-1)
         print("Running the IDP-Z3 idp_engine.")
         idp = idpparser.model_from_str(fodot)
         idp.execute()
 
     # If no options were supplied, print the specification.
     if not args.outputfile and not args.idp_z3:
         print(fodot)
```

### Comparing `cdmn-2.1.1/cdmn/glossary.py` & `cdmn-2.1.2/cdmn/glossary.py`

 * *Files 5% similar despite different names*

```diff
@@ -609,50 +609,49 @@
         :arg bool: partial, whether or not it's a partial function.
         :arg zero_arity: bool which should be True when the predicate is a
             0-arity predicate (constants and booleans).
         :returns Predicate:
         """
         if not predicate:  # Check if it's a function.
             regex = (r'^(?P<name>.*)$')
-            # regex = (r"^(?P<name>.*) of (?P<args>(?:{0})(?: and (?:{0}))*)$"
-            #          .format('|'.join([x.name for x in glossary.types])))
         else:
             regex = (r'^(?P<name>.*)$')
-        #    regex = ('^(?P<args>(?:{0})(?: and (?:{0}))*) is (?P<name>.*)$'
-        #             .format('|'.join([x.name for x in glossary.types])))
         try:
             name = re.match(regex, full_name).group('name')
         except AttributeError:
             name = full_name
-        try:
-            # args = re.match(regex, full_name).group('args').split(' and ')
-            raise IndexError
-        except (AttributeError, IndexError):
-            if zero_arity:
-                return Predicate(full_name, [], super_type, partial,
-                                 zero_arity=zero_arity)
-            else:  # We need to find the relation's types.
-                # We simply loop over all words and look for full matches.
-                # TODO This should be done better. Types could be multiple
-                # words.
-                args = []
-                name_elements = full_name.split(" ")
-
-                for element in name_elements:
-                    for t in glossary.types:
-                        if re.fullmatch(element, t.name):
-                            args.append(t)
-                            break
-                return Predicate(name, args,
-                                 super_type, partial,
-                                 full_name, zero_arity)
+        if zero_arity:
+            return Predicate(full_name, [], super_type, partial,
+                             zero_arity=zero_arity)
+        else:  # We need to find the relation's types.
+            args = []
+            # TODO: sort the matches so the order is preserved.
+            for typ in glossary.types:
+                for x in re.finditer(r'\b' + f'{typ.name}' + r'\b',
+                                     full_name):
+                    args.append([x.start(), typ])
+            # Sort the args based on their position in the string.
+            args.sort(key=lambda x: x[0])
+            args = [x[1] for x in args]
+            return Predicate(name, args,
+                             super_type, partial,
+                             full_name, zero_arity)
 
         return Predicate(name, [glossary.find_type(t) for t in args],
                          super_type, partial, full_name, zero_arity)
 
+    @property
+    def arity(self):
+        """
+        Returns arity of the symbol's domain.
+
+        :returns int:
+        """
+        return len(self.args)
+
     def is_function(self):
         """
         Method to check whether the predicate is a function.
         Since only functions have super types, we use that as a check.
         Note that constants are a special case of functions.
 
         :returns boolean:
@@ -683,26 +682,21 @@
         For instance, `Country borders Country` becomes
         `(?P<arg0>.+) borders (?P<arg1>.+)`.
         This way, arg0 and arg1 can be found easily later on.
         """
         if not self.args:
             return self.name
         elif self.args:
-            name_elements = self.name.split(" ")
-            new_alias = ""
-            arg_index = 0
             arglist = [arg.name for arg in self.args]
-            for element in name_elements:
-                if element in arglist:
-                    new_alias += f"(?P<arg{arg_index}>.+) "
-                    arg_index += 1
-                    continue
-                else:
-                    new_alias += f"{element} "
-            return new_alias[:-1]  # We drop the last space.
+            new_name = self.name
+            for i, arg in enumerate(arglist):
+                # Replace the first occurrence of each type name by a dummy.
+                new_name = re.sub(r'\b' + arg + r'\b', f'(?P<arg{i}>.+)',
+                                  new_name, 1)
+            return new_name
         else:
             raise ValueError("No idea what went wrong.")
 
     def lookup(self, string: str):
         """
         Method to compare a string to this predicate, to see if the predicate
         appears in the string in any form.
```

### Comparing `cdmn-2.1.1/cdmn/idply.py` & `cdmn-2.1.2/cdmn/idply.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     This code is licensed under GNU GPLv3 license (see LICENSE) for more
     information.
     This file is part of the cDMN solver.
 """
 
 import re
 from ply import lex, yacc
-from cdmn.interpret import VariableInterpreter, PredicateInterpretation
+from cdmn.interpret import VariableInterpreter
 
 
 class Parser:
     """
     The parser is used to parse cDMN strings and find out their underlying
     secrets.
     This is a complex part of the solver, and works on magic and hope.
@@ -21,21 +21,24 @@
         Initialises the parser.
 
         :arg i: a VariableInterpreter object.
         :returns Object:
         """
         self.result = ''
         self.interpreter = i
-        self.lexer = lex.lex(module=self)
+        self.lexer = lex.lex(module=self, reflags=re.UNICODE)
         self.parser = yacc.yacc(module=self)
         self.variables = []
         self.expected_type = None
         self.parsing_errors = {}
 
-    def parse_val(self, column_header: str, value: str, variables) -> str:
+    def parse_val(self, column_header: str,
+                  value: str,
+                  variables,
+                  simplified_variables={}) -> str:
         """
         Parse a cDMN notation inside a cell.
 
         :param column_header: the column header of the cell
         :param value: the value inside the cell
         :param variables: no idea
         :returns str: the parsed notation.
@@ -48,54 +51,59 @@
             return ""
 
         comparator = '^(?:>|<)(?:=)?|='
 
         if not re.match(comparator, str(value)):
             value = f'= {value}'
 
+        # If any variables can be simplified, i.e., always have a set value,
+        # we can replace them by the set value to avoid quantification.
+        for variable, var_value in simplified_variables.items():
+            column_header = re.sub(f'\\b{variable}\\b', var_value, column_header)
+            value = re.sub(f'\\b{variable}\\b', var_value, value)
+
+        if f'= {column_header}' == value:
+            return ""
+
         try:
             self.parser.parse(column_header + value)
         except ValueError:
-            error = (f"Encountered error when parsing: "
-                     f"unable to parse \"{value}\" in column"
-                     f" \"{column_header}\"")
             if column_header in self.parsing_errors:
                 self.parsing_errors[column_header].append(value)
             else:
                 self.parsing_errors[column_header] = [value]
         self.variables = []
         self.expected_type = None
-
         return self.result
 
     reserved = {
         'Not': 'NOT',
         'not': 'NOT',
         'yes': 'YES',
         'Yes': 'YES',
         'No': 'NO',
         'no': 'NO',
         'abs': 'ABS',
         'Abs': 'ABS',
         'min': 'MIN',
         'Min': 'MIN',
         'max': 'MAX',
-        'Max': 'MAX'
+        'Max': 'MAX',
     }
 
     tokens = [
                  'NUMBER', 'COMPARE',
                  'PLUS', 'MINUS', 'TIMES', 'DIVIDE', 'EQUALS', 'COMMA',
                  'LPAREN', 'RPAREN', 'LBRACK', 'RBRACK', 'UNTIL', 'ID',
                  'PERCENT', 'STRAIGHTQUOTE', 'LQUOTE', 'RQUOTE',
                  'LACC', 'RACC', 'DOT', 'HASHTAG'
              ] + list(set(reserved.values()))
 
     def t_ID(self, t):
-        r'[a-zA-Z_][a-zA-Z_0-9\s]*'
+        r'[^\d\W][\w\s]*'
         t.value = t.value.strip()
         t.type = self.reserved.get(t.value, 'ID')  # Check for reserved words
         return t
 
     t_PLUS = r'\+'
     t_MINUS = r'(-|−)'
     t_TIMES = r'\*'
@@ -147,15 +155,14 @@
     # As long as there is no rule that forms a statement, the yacc will try to
     # keep looking for matches.
     # A match that forms a statement, ends the search.
     def p_returnval(self, t):
         'return : statement'
         self.result = t[1]
 
-
     # Yes and No just return the name of the predicate.
     def p_yes(self, t):
         '''statement : expression EQUALS YES'''
         t[0] = f'{t[1]}'
 
     def p_no(self, t):
         '''statement : expression EQUALS NO'''
@@ -322,10 +329,9 @@
 
         t[0] = interpretation
 
     def p_error(self, t):
         try:
             print(f"Syntax error at '{t.value}'")
             raise ValueError(f"Syntax error at '{t.value}'")
-            # breakpoint()
         except AttributeError:
             pass
```

### Comparing `cdmn-2.1.1/cdmn/idpname.py` & `cdmn-2.1.2/cdmn/idpname.py`

 * *Files identical despite different names*

### Comparing `cdmn-2.1.1/cdmn/interpret.py` & `cdmn-2.1.2/cdmn/interpret.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,18 +64,29 @@
 
         if len(interpretations) == 0:
             raise ValueError(f'The value of "{value}" could not be'
                              f' interpreted.')
         if len(interpretations) == 1:
             return interpretations[0]
         if len(interpretations) > 1:
-            # Find most likely interpretation by sorting them on Levenshtein
-            # distance. This distance measures the number of operations needed
-            # to transform one string in another, and should give a good
-            # estimation of the "most likely" match.
+            # Find most likely interpretation by applying a heuristic to find
+            # the "most likely". First, we prioritize nested symbols: for
+            # instance in the Programmer example, `lead knows Java` should be
+            # interpreted as `Employee knows Language`, and not as `lead`.
+            # Practically, we find the highest arity omong the interpretations,
+            # and throw out all those that have a lower arity.
+            # Second, we sort on Levenshtein Distance.
+            # This ensures that, for instance, "SummerTime" is interpreted as
+            # such and not as "Summer".
+
+            # Throw out all interpretations with a lower arity.
+            max_arity = max([x.pred.arity for x in interpretations])
+            interpretations = [x for x in interpretations if x.pred.arity ==
+                               max_arity]
+            # Sort on LDistance
             interpretations.sort(key=lambda interp: distance(value,
                                                              interp.value))
             print(f"Warning: Multiple possible interpretations for {value}."
                   f" Selecting the most likely interpretation:"
                   f" {interpretations[0].value}")
             return interpretations[0]
```

### Comparing `cdmn-2.1.1/cdmn/parse_xml.py` & `cdmn-2.1.2/cdmn/parse_xml.py`

 * *Files identical despite different names*

### Comparing `cdmn-2.1.1/cdmn/parsetab.py` & `cdmn-2.1.2/cdmn/parsetab.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,46 +23,46 @@
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
 _lr_productions = [
   ("S' -> return","S'",1,None,None,None),
-  ('return -> statement','return',1,'p_returnval','idply.py',151),
-  ('statement -> expression EQUALS YES','statement',3,'p_yes','idply.py',157),
-  ('statement -> expression EQUALS NO','statement',3,'p_no','idply.py',161),
-  ('statement -> expression EQUALS MINUS','statement',3,'p_dontcare','idply.py',166),
-  ('statement -> expression EQUALS','statement',2,'p_dontcare','idply.py',167),
-  ('statement -> expression EQUALS NOT LPAREN expression RPAREN','statement',6,'p_eqnotlist','idply.py',170),
-  ('statement -> expression EQUALS NOT LPAREN list RPAREN','statement',6,'p_eqnot','idply.py',174),
-  ('statement -> expression EQUALS list','statement',3,'p_eqlist','idply.py',179),
-  ('statement -> expression EQUALS expression','statement',3,'p_compare','idply.py',184),
-  ('statement -> expression COMPARE expression','statement',3,'p_compare','idply.py',185),
-  ('statement -> expression EQUALS lbound expression UNTIL expression rbound','statement',7,'p_range','idply.py',190),
-  ('statement -> expression EQUALS lbound expression COMMA expression rbound','statement',7,'p_range','idply.py',191),
-  ('statement -> expression EQUALS LPAREN expression UNTIL expression RPAREN','statement',7,'p_prange','idply.py',199),
-  ('statement -> expression EQUALS LPAREN expression UNTIL expression RBRACK','statement',7,'p_rrange','idply.py',208),
-  ('statement -> expression EQUALS NOT LPAREN lbound expression COMMA expression rbound RPAREN','statement',10,'p_nrange','idply.py',216),
-  ('list -> expression COMMA expression','list',3,'p_list','idply.py',227),
-  ('list -> list COMMA expression','list',3,'p_list','idply.py',228),
-  ('expression -> ABS expression','expression',2,'p_expression_abs','idply.py',236),
-  ('expression -> LQUOTE expression RQUOTE','expression',3,'p_quotes','idply.py',241),
-  ('expression -> STRAIGHTQUOTE expression STRAIGHTQUOTE','expression',3,'p_quotes','idply.py',242),
-  ('expression -> HASHTAG expression','expression',2,'p_domain_size','idply.py',255),
-  ('expression -> expression PLUS expression','expression',3,'p_expression_binop','idply.py',262),
-  ('expression -> expression MINUS expression','expression',3,'p_expression_binop','idply.py',263),
-  ('expression -> expression TIMES expression','expression',3,'p_expression_binop','idply.py',264),
-  ('expression -> expression DIVIDE DIVIDE expression','expression',4,'p_expression_binop','idply.py',265),
-  ('expression -> expression DIVIDE expression','expression',3,'p_expression_binop','idply.py',266),
-  ('expression -> expression PERCENT expression','expression',3,'p_expression_binop','idply.py',267),
-  ('expression -> MINUS expression','expression',2,'p_expression_uminus','idply.py',283),
-  ('expression -> LPAREN expression RPAREN','expression',3,'p_expression_group','idply.py',287),
-  ('lbound -> LPAREN','lbound',1,'p_lbound','idply.py',291),
-  ('lbound -> LBRACK','lbound',1,'p_lbound','idply.py',292),
-  ('lbound -> RBRACK','lbound',1,'p_lbound','idply.py',293),
-  ('rbound -> RPAREN','rbound',1,'p_rbound','idply.py',297),
-  ('rbound -> RBRACK','rbound',1,'p_rbound','idply.py',298),
-  ('rbound -> LBRACK','rbound',1,'p_rbound','idply.py',299),
-  ('expression -> NUMBER','expression',1,'p_expression_number','idply.py',303),
-  ('expression -> NUMBER DOT NUMBER','expression',3,'p_dot','idply.py',307),
-  ('expression -> ID','expression',1,'p_expression_name','idply.py',311),
+  ('return -> statement','return',1,'p_returnval','idply.py',160),
+  ('statement -> expression EQUALS YES','statement',3,'p_yes','idply.py',165),
+  ('statement -> expression EQUALS NO','statement',3,'p_no','idply.py',169),
+  ('statement -> expression EQUALS MINUS','statement',3,'p_dontcare','idply.py',174),
+  ('statement -> expression EQUALS','statement',2,'p_dontcare','idply.py',175),
+  ('statement -> expression EQUALS NOT LPAREN expression RPAREN','statement',6,'p_eqnotlist','idply.py',178),
+  ('statement -> expression EQUALS NOT LPAREN list RPAREN','statement',6,'p_eqnot','idply.py',182),
+  ('statement -> expression EQUALS list','statement',3,'p_eqlist','idply.py',187),
+  ('statement -> expression EQUALS expression','statement',3,'p_compare','idply.py',192),
+  ('statement -> expression COMPARE expression','statement',3,'p_compare','idply.py',193),
+  ('statement -> expression EQUALS lbound expression UNTIL expression rbound','statement',7,'p_range','idply.py',198),
+  ('statement -> expression EQUALS lbound expression COMMA expression rbound','statement',7,'p_range','idply.py',199),
+  ('statement -> expression EQUALS LPAREN expression UNTIL expression RPAREN','statement',7,'p_prange','idply.py',207),
+  ('statement -> expression EQUALS LPAREN expression UNTIL expression RBRACK','statement',7,'p_rrange','idply.py',216),
+  ('statement -> expression EQUALS NOT LPAREN lbound expression COMMA expression rbound RPAREN','statement',10,'p_nrange','idply.py',224),
+  ('list -> expression COMMA expression','list',3,'p_list','idply.py',235),
+  ('list -> list COMMA expression','list',3,'p_list','idply.py',236),
+  ('expression -> ABS expression','expression',2,'p_expression_abs','idply.py',244),
+  ('expression -> LQUOTE expression RQUOTE','expression',3,'p_quotes','idply.py',249),
+  ('expression -> STRAIGHTQUOTE expression STRAIGHTQUOTE','expression',3,'p_quotes','idply.py',250),
+  ('expression -> HASHTAG expression','expression',2,'p_domain_size','idply.py',263),
+  ('expression -> expression PLUS expression','expression',3,'p_expression_binop','idply.py',270),
+  ('expression -> expression MINUS expression','expression',3,'p_expression_binop','idply.py',271),
+  ('expression -> expression TIMES expression','expression',3,'p_expression_binop','idply.py',272),
+  ('expression -> expression DIVIDE DIVIDE expression','expression',4,'p_expression_binop','idply.py',273),
+  ('expression -> expression DIVIDE expression','expression',3,'p_expression_binop','idply.py',274),
+  ('expression -> expression PERCENT expression','expression',3,'p_expression_binop','idply.py',275),
+  ('expression -> MINUS expression','expression',2,'p_expression_uminus','idply.py',291),
+  ('expression -> LPAREN expression RPAREN','expression',3,'p_expression_group','idply.py',295),
+  ('lbound -> LPAREN','lbound',1,'p_lbound','idply.py',299),
+  ('lbound -> LBRACK','lbound',1,'p_lbound','idply.py',300),
+  ('lbound -> RBRACK','lbound',1,'p_lbound','idply.py',301),
+  ('rbound -> RPAREN','rbound',1,'p_rbound','idply.py',305),
+  ('rbound -> RBRACK','rbound',1,'p_rbound','idply.py',306),
+  ('rbound -> LBRACK','rbound',1,'p_rbound','idply.py',307),
+  ('expression -> NUMBER','expression',1,'p_expression_number','idply.py',311),
+  ('expression -> NUMBER DOT NUMBER','expression',3,'p_dot','idply.py',315),
+  ('expression -> ID','expression',1,'p_expression_name','idply.py',319),
 ]
```

### Comparing `cdmn-2.1.1/cdmn/post_process.py` & `cdmn-2.1.2/cdmn/post_process.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
     Copyright 2019 Simon Vandevelde, Bram Aerts, Joost Vennekens
     This code is licensed under GNU GPLv3 license (see LICENSE) for more
     information.
     This file is part of the cDMN solver.
 """
-from typing import List, Dict
 import re
+from typing import Dict
+from collections import defaultdict
 
 
 def merge_definitions(idp: str) -> str:
     """
     In cDMN, it is possible to create different tables that each define
     the same concept.
     In cases where relations are defined, this can be problematic.
@@ -28,44 +29,34 @@
     # Grab all rules and their annotations.
     rules = re.findall(r"(\t\t\[.*?\])?\n(.+?)(?=<-)(.+?)(?=\.\n)", idp)
 
     # Remove all rules.
     new_idp = re.sub(r"(\[.*?\])?\n(.+?)(?=<-)(.+?)(?=\.\n)", "", idp)
 
     defined_concepts: Dict[str, str] = {}
+    defined_concepts = defaultdict(list)
     # Go over every rule and identify the defined variable.
     for annotation, head, body in rules:
-        rule = annotation + '\n' + head + body + ".\n"
-        try:  # Find all rules with quantifiers.
-            defined_concept = re.findall(r": (.*?)\(", rule)[0]
-        except IndexError:  # Find all rules without quantifiers.
-            defined_concept = re.findall(r"\t(.*?)\(", rule)[0]
-        if defined_concept in defined_concepts:
-            defined_concepts[defined_concept] += rule
-        else:
-            defined_concepts[defined_concept] = rule
+        rule = annotation + '\n' + head + body + '.'
+        defined_concept = head.split(":")[-1].split("(")[0].strip()
+        defined_concepts[defined_concept].append(rule)
 
     # Grab the common definition annotations, try to find out what concept they
     # annotate. If multiple annotations exist for the same concept, we need to
     # merge them as well.
     definition_annotations = re.findall(r"\[\#(.*?)\#\]\n\t{(.*?)<-", idp,
                                         re.DOTALL)
-    def_annotations: Dict[str, str] = {}
+    # def_annotations: Dict[str, str] = []
+    def_annotations = defaultdict(list)
     for annotation, rule in definition_annotations:
-        try:
-            defined_concept = re.findall(r": (.*?)\(", rule)[0]
-        except IndexError:
-            defined_concept = re.findall(r"\t(.*?)\(", rule)[0]
-        if defined_concept in def_annotations:
-            def_annotations[defined_concept] += ' OR ' + annotation
-        else:
-            def_annotations[defined_concept] = annotation
+        defined_concept = head.split('\t')[-1].split(":")[-1].split("(")[0].strip()
+        def_annotations[defined_concept].append(annotation)
 
     # Remove all { .. }
     new_idp = re.sub(r"\t{[\t\n\.]*?}", "", new_idp)
     new_idp = re.sub(r"\t\[(.*?)\]\n\n", "", new_idp)
     for key, val in defined_concepts.items():
-        new_idp += f"\t[{def_annotations[key]}]\n"
+        new_idp += f"\t[{' OR '.join(def_annotations[key])}]\n"
         new_idp += "\t{\n"
-        new_idp += val
-        new_idp += "\t}\n"
+        new_idp += ''.join(val)
+        new_idp += "\n\t}\n"
     return new_idp
```

### Comparing `cdmn-2.1.1/cdmn/table.py` & `cdmn-2.1.2/cdmn/table.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,27 +8,64 @@
 
 import numpy as np
 import re
 from cdmn.idply import Parser
 from cdmn.idpname import idp_name
 from typing import List
 from collections import OrderedDict
+from copy import copy
 
 
 def variname(string: str) -> str:
     """
     Function to return the variable of a header in the form of "Type called
     var"
 
     :arg string: the headerstring of which the variable name needs to be found.
     :returns str: the variable name.
     """
     return re.split(r'\s+[cC]alled\s+', string)[-1]
 
 
+def typeiname(string: str) -> str:
+    """
+    Function to return the type of a header in the form of "Type called var"
+
+    :arg string: the headerstring of which the variable name needs to be found.
+    :returns str: the variable name.
+    """
+    return re.split(r'\s+[cC]alled\s+', string)[0]
+
+
+def is_variable_introducing(string: str, variables: OrderedDict) -> bool:
+    """
+    Checks whether a column name is variable introducing.
+    There's two types of variable introducing columns:
+        1. Using "Type called T" syntax
+        2. Just using "Type"
+
+    :arg string: the headerstring of a column.
+    :returns bool:
+    """
+    return (len(re.findall(r'\s+[cC]alled\s+', string)) != 0
+            or string in variables)
+
+
+def is_singular_value(string: str) -> bool:
+    """
+    Check whether a cell contains a singular value, such as "foo".
+    Specifically look for signs that there might be multiple values, such as
+    "-", ",", ...
+
+    :arg string: the content of a cell in string form
+    :returns bool:
+    """
+    return len(re.findall(r'[,−()\s-]', string)) == 0
+
+
 class Table:
     """
     The table object represents decision and constraint tables.
 
     :attr name: str
     :attr hit_policy: str
     :attr inputs: List[np.array]
@@ -205,14 +242,78 @@
         ivariables = self._read_types(self.inputs)
         iquantors = self._create_quantors(ivariables, repres)
         oquantors = self._create_quantors(OrderedDict(
             [x for x in variables.items() if x not in ivariables.items()]),
             repres)
         return variables, iquantors, oquantors
 
+    def _parse_row_over_colums(self,
+                               row: list[str],  # TODO type hint
+                               variables: OrderedDict,
+                               simplified_variables: dict[str, str],
+                               quantors: str,
+                               parse_inputs: bool = True
+                               ) -> tuple[list[str],
+                                          dict[str, str],
+                                          str]:
+        """
+        Parse a row for every input/output column of a table.
+        This function also takes care of simplification in the context of
+        quantifiers with singular values. E.g.,
+
+        Monkey called m1 | food of m1
+        -----------------------------
+        Frank            | Berry
+
+        does not need a quantifier -- instead, we can replace m1 by "Frank" in
+        the rest of the formula and drop the quantifier.
+
+        :arg row: list[str], the row of values
+        :arg variables: OrderedDict, mapping variables on Types
+        :arg simplified_variables: dict[str, str], mapping variable names on
+            singular type values.
+        :arg quantors: str representing the quantors
+        :arg parse_inputs: bool. True to parse inputs, Fales to parse outputs.
+
+
+        :returns (list[str], dict[str, str], str):
+        """
+        quantors = copy(quantors)  # orig iquantors are shared over rows.
+
+        if parse_inputs:
+            columns = self.inputs
+            offset = 0
+        else:
+            columns = self.outputs
+            offset = len(self.inputs)
+
+        parse_out = []
+        for i, col in enumerate(columns):
+            # If a variable introducing column has a single value in the
+            # input cell, remove the quantification and replace the
+            # variable by the value in every formula.
+            if (is_variable_introducing(col, variables)
+               and is_singular_value(str(row[i+offset]))):
+                var_name = variname(col)
+                type_name = typeiname(col)
+                simplified_variables[var_name] = str(row[i+offset])
+                quantors = quantors.replace(f"!{var_name.replace(' ', '_')} in"
+                                            f" {type_name.replace(' ', '_')}_t:",
+                                            '')  # Also remove quant
+                continue
+            atom = self.parser.parse_val(variname(col),
+                                         row[i+offset],
+                                         variables,
+                                         simplified_variables)
+            if atom:
+                atom = atom.replace("<=", "=<")  # "=<" is inverted in IDP
+                parse_out.append(atom)
+
+        return parse_out, simplified_variables, quantors
+
     def _export_definitions(self) -> str:
         """
         Method to export the table as definitions.
         When the hitpolicy is 'U', 'A' or 'F', we can translate the entire
         table into definitions in idp form.
 
         If the output is idpz3, then we add a constraint which says that any
@@ -228,64 +329,77 @@
         # Iterate over every outputcolumn.
         for i, col in enumerate(self.outputs):
             if i > 0:
                 # When creating a definition for the second, third, ... output,
                 # we need to add the name again.
                 string += f'\t[#{self.name}#]\n'
             string += '\t{\n'
-            variables, iquantors, oquantors = self.variables_iq_oq(
-                                              repres=quantor_repr)
+            variables, orig_iquantors, oquantors = self.variables_iq_oq(
+                                                   repres=quantor_repr)
             # Iterate over every row and interpret it for the specific
             # outputcolumn (and disregard the other outputcolumns).
             previous_conditions = []
 
             falsecount = 0
             for r, row in enumerate(self.rules):
-                conditions = ' & '.join(filter(
-                    lambda x: x,
-                    (self.parser.parse_val(variname(col), row[i], variables)
-                     for i, col in enumerate(self.inputs))))
+                conditions = []
+                simplified_variables = {}
+                conditions, simplified_variables, iquantors = \
+                    self._parse_row_over_colums(row, variables,
+                                                simplified_variables,
+                                                orig_iquantors,
+                                                True)
+                conditions = ' & '.join(conditions)
                 conclusion = self.parser.parse_val(col,
                                                    row[i + len(self.inputs)],
-                                                   variables)
+                                                   variables,
+                                                   simplified_variables)
                 # A definition can't contain a not in the conclusion.
                 # A negation of a predicate is implied by the other rules.
                 if '~' in conclusion:
                     # If all the row are 'not', we need to specify that none of
                     # the predicates are true because there's no implicit
                     # rule which defines this.
                     if falsecount == len(self.rules) - 1:
                         conditions = "false"
                         conclusion = conclusion.replace("~", " ")
                         conclusion = conclusion[2:-1]  # Strip the brackets.
                     else:
                         falsecount = falsecount + 1
                         continue
 
-                if '<=' in conditions:
-                    conditions = conditions.replace('<=', '=<')
                 if not conclusion:
                     continue
                 if not conditions:
                     conditions = 'true'
 
                 # If an annotation is present, use it. Otherwise, set None.
                 if self.annotations_present:
                     annotation = f'\t\t[{row[-1]}]\n'
                 else:
                     annotation = ''
 
                 if self.hit_policy != 'F' or not previous_conditions:
-                    string += (f'{annotation}\t\t{iquantors}{oquantors}{conclusion} <- {conditions}.\n')
+                    if conditions:
+                        string += (f'{annotation}\t\t{iquantors}{oquantors}'
+                                   f'{conclusion} <- {conditions}.\n')
+                    else:
+                        string += (f'{annotation}\t\t{iquantors}{oquantors}'
+                                   f'{conclusion}.\n')
                 else:
                     # For first hit, we always add a negation of the previous
                     # conditions.
-                    string += (f'{annotation}\t\t{iquantors}{oquantors}{conclusion} <-'
-                               f' {oquantors}{conditions} &'
-                               f' ~(({")|(".join(previous_conditions)})).\n')
+                    if conditions:
+                        string += (f'{annotation}\t\t{iquantors}{oquantors}'
+                                   f'{conclusion} <- {oquantors}{conditions} &'
+                                   f' ~(({")|(".join(previous_conditions)})).\n')
+                    else:
+                        string += (f'{annotation}\t\t{iquantors}{oquantors}'
+                                   f'{conclusion} <- {oquantors}'
+                                   f' ~(({")|(".join(previous_conditions)})).\n')
 
                 previous_conditions.append(conditions)
             string += '\t}\n\n'
         return string
 
     def _export_implication(self) -> str:
         """
@@ -298,44 +412,49 @@
         # Format quantor representation
         quantor_repr = '!{0} in {1}: '
 
         # Set the headername in comments.
         string = f'\t//{self.name}\n'
         # Depending on the inputs and outputs, we need different input and
         # output quantors.
-        variables, iquantors, oquantors = self.variables_iq_oq(
-                                          repres=quantor_repr)
+        variables, orig_iquantors, orig_oquantors = self.variables_iq_oq(repres=quantor_repr)
 
         # For each row, form the conditions and the conclusions.
         # When no conditions are present, the condition defaults to 'true'.
         for row in self.rules:
-            conditions = ' & '.join(filter(
-                lambda x: x, (self.parser.parse_val(variname(col), row[i],
-                                                    variables) for i, col
-                                    in enumerate(self.inputs))))
-            conclusions = ' & '.join(filter(
-                lambda x: x, (self.parser.parse_val(col,
-                                                    row[i + len(self.inputs)],
-                                                    variables) for i, col
-                              in enumerate(self.outputs))))
+            conditions = []
+            simplified_variables = {}
+            conditions, simplified_variables, iquantors = \
+                self._parse_row_over_colums(row, variables,
+                                            simplified_variables,
+                                            orig_iquantors,
+                                            parse_inputs=True)
+            conditions = ' & '.join(conditions)
+
+            conclusions, _, oquantors = \
+                self._parse_row_over_colums(row, variables,
+                                            simplified_variables,
+                                            orig_oquantors,
+                                            parse_inputs=False)
+
+            conclusions = ' & '.join(conclusions)
             if not conclusions:
                 raise ValueError(f'This line has no conclusion: {row}')
-            # <= is inverted in idp.
-            if '<=' in conclusions:
-                conclusions = conclusions.replace('<=', '=<')
-            if not conditions:
-                conditions = 'true'
 
             if self.annotations_present:
                 annotation = f'[{row[-1]}]'
             else:
                 annotation = f'[{self.name}]'
 
-            string += (f'\t{annotation}\n\t{iquantors}{conditions} => '
-                       f'{oquantors}{conclusions}.\n\n')
+            if conditions:
+                string += (f'\t{annotation}\n\t{iquantors}{conditions} => '
+                           f'{oquantors}{conclusions}.\n\n')
+            else:
+                string += (f'\t{annotation}\n\t{iquantors}'
+                           f'{oquantors}{conclusions}.\n\n')
         return string
 
     def _export_aggregate(self) -> str:
         """
         Method to export the table as aggregates.
         When the hitpolicy is 'C+/>/</#', we can translate the table into
         aggregates in idp form.
@@ -434,16 +553,16 @@
                 # Get the weights of the aggregate.
                 weights = self.parser.parse_val('__PLACEHOLDER__',
                                                 row[i + len(self.inputs)],
                                                 variables)
                 if not weights or not re.search(r'__PLACEHOLDER__\s*=',
                                                 weights):
                     raise ValueError(
-                        f'There is no valid value apointed to {col}\'s weights'
-                        f' in the following rule: {row}'
+                        f'There is no valid value appointed to {col}\'s'
+                        f' weights in the following rule: {row}.'
                         f' Maybe you forgot to merge the correct cells?')
                 if self.hit_policy == 'C#':
                     try:
                         x = self.parser.interpreter.interpret_value(
                                 row[i + len(self.inputs)], variables)
                         if x.value not in variables:
                             additional_agg_vars = self._create_quantors(
@@ -494,34 +613,51 @@
                                    assigned_variable,
                                    " " if iquantors else "",
                                    math_operator,
                                    combine_operator.join(aggs),
                                    ''))
         return string
 
+    def _export_FO(self) -> str:
+        """ Export table directly to FO(.). For expert users only.
+
+        :returns str:
+        """
+        string = ''
+        for row in self.rules:
+            if self.annotations_present:
+                annotation = f'[{row[-1]}]'
+            else:
+                annotation = f'[{self.name}]'
+            string += f'\n\t{annotation}\n\t'
+            string += row[0] if str(row[0]).endswith('.') else f'{row[0]}.'
+        return string
+
     def export(self):
         """
         Export tries to find the hit policy for a table, and then returns the
         method needed to transfer the table to idp form.
         These hit policies are currently:
 
           * A, U, F           -> translate to definitions;
           * E*                -> translate to implications;
-          * C+, C<, C>, C#    -> translate to aggregates.
+          * C+, C<, C>, C#    -> translate to aggregates;
+          * FO                -> translate directly to FO.
 
         Every hit policy has its own method.
 
         :returns method: the output of export method for the table.
         """
 
         # List all possible hit policies.
         actions = {
             r'^[AUF]$': self._export_definitions,
             r'^E\*$': self._export_implication,
-            r'^C[\<\>\#\+]$': self._export_aggregate
+            r'^C[\<\>\#\+]$': self._export_aggregate,
+            r'^FO$': self._export_FO
         }
         # Try, except is necessary to avoid StopIteration error.
         try:
             # Find hit policy.
             hp = next(map(lambda x: x.re.pattern,
                           filter(lambda x: x,
                                  (re.match(x, self.hit_policy)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cdmn-2.1.1/cdmn/table_operations.py` & `cdmn-2.1.2/cdmn/table_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     :arg file_name: path to the xlsx file.
     :arg sheet: name of the sheet to load in.
     :returns List<np.array>: a list of all the tables in a sheet.
     """
     def rang(m, n): return range(m, n + 1)
 
-    wb = openpyxl.load_workbook(file_name)
+    wb = openpyxl.load_workbook(file_name, data_only=True)
 
     # If --all-sheets option was used, collect all sheetnames.
     if len(sheet_names) == 0:
         sheet_names = wb.sheetnames
 
     sheets = []
     for sheet_name in sheet_names:
```

### Comparing `cdmn-2.1.1/cdmn.egg-info/PKG-INFO` & `cdmn-2.1.2/cdmn.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: cdmn
-Version: 2.1.1
+Version: 2.1.2
 Summary: A package providing a (c)DMN solver and API
 Home-page: http://cdmn.be
 Author: Simon Vandevelde
 Author-email: s.vandevelde@kuleuven.be
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openpyxl==3.0.10
+Requires-Dist: ply==3.11
+Requires-Dist: numpy
+Requires-Dist: python-dateutil
+Requires-Dist: Levenshtein
 
 # cDMN
 
 ## Welcome to the cDMN solver's code repository.
 
 cDMN stands for Constraint Decision and Model Notation.
 It is an extension to the [DMN](https://www.omg.org/spec/DMN/About-DMN/) standard, managed by the Object Management Group (OMG).
```

### Comparing `cdmn-2.1.1/setup.py` & `cdmn-2.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cdmn",
-    version="2.1.1",
+    version="2.1.2",
     author="Simon Vandevelde",
     author_email="s.vandevelde@kuleuven.be",
     description="A package providing a (c)DMN solver and API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://cdmn.be",
     packages=setuptools.find_packages(),
     python_requires='>=3.7',
     install_requires=['openpyxl==3.0.10', 'ply==3.11',
-                      'numpy==1.24.1', 'python-dateutil',
+                      'numpy', 'python-dateutil',
                       'Levenshtein'],
     entry_points={
         'console_scripts': ['cdmn=cdmn.cdmn:main']
     }
 )
```

