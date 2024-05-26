# Comparing `tmp/killercoda_cli-1.0.4.tar.gz` & `tmp/killercoda_cli-1.0.5.tar.gz`

## Comparing `killercoda_cli-1.0.4.tar` & `killercoda_cli-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/.coveragerc
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/killercoda_cli/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/killercoda_cli/__init__.py
--rwxr-xr-x   0        0        0    16265 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/killercoda_cli/cli.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/tests/__init__.py
--rwxr-xr-x   0        0        0    11001 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/tests/test_cli.py
--rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/tests/test_integration_cli.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/README.md
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/.coveragerc
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/killercoda_cli/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/killercoda_cli/__init__.py
+-rwxr-xr-x   0        0        0    16127 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/killercoda_cli/cli.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/tests/__init__.py
+-rwxr-xr-x   0        0        0    11001 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/tests/test_cli.py
+-rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/tests/test_integration_cli.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/README.md
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/PKG-INFO
```

### Comparing `killercoda_cli-1.0.4/.github/workflows/ci.yml` & `killercoda_cli-1.0.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.4/killercoda_cli/cli.py` & `killercoda_cli-1.0.5/killercoda_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,17 +352,14 @@
           - Renames and renumbers step files and directories based on user input.
           - Updates the 'index.json' file to reflect changes in step order and titles.
     """
     print(help_text)
 
 
 def execute_file_operations(file_operations):
-    print("Debug file operations before execution:")  # Debugging line
-    for op in file_operations:
-        print(op)  # Debugging line
     for operation in file_operations:
         if operation.operation == "makedirs":
             os.makedirs(operation.path, exist_ok=True)
         elif operation.operation == "write_file":
             with open(operation.path, "w") as file:
                 file.write(operation.content)
         elif operation.operation == "chmod":
```

### Comparing `killercoda_cli-1.0.4/tests/test_cli.py` & `killercoda_cli-1.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.4/tests/test_integration_cli.py` & `killercoda_cli-1.0.5/tests/test_integration_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.4/.gitignore` & `killercoda_cli-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.4/LICENSE.txt` & `killercoda_cli-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.4/README.md` & `killercoda_cli-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.4/pyproject.toml` & `killercoda_cli-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.4/PKG-INFO` & `killercoda_cli-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: killercoda-cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: A CLI helper for writing killercoda scenarios and managing steps
 Project-URL: Documentation, https://github.com/unknown/killercoda-cli#readme
 Project-URL: Issues, https://github.com/unknown/killercoda-cli/issues
 Project-URL: Source, https://github.com/unknown/killercoda-cli
 Author-email: Piotr Zaniewski <piotrzan@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

