# Comparing `tmp/killercoda_cli-1.0.6.tar.gz` & `tmp/killercoda_cli-1.0.7.tar.gz`

## Comparing `killercoda_cli-1.0.6.tar` & `killercoda_cli-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/.coveragerc
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/killercoda_cli/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/killercoda_cli/__init__.py
--rwxr-xr-x   0        0        0    16149 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/killercoda_cli/cli.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/tests/__init__.py
--rwxr-xr-x   0        0        0    11001 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/tests/test_cli.py
--rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/tests/test_integration_cli.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/LICENSE.txt
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/README.md
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/.coveragerc
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/killercoda_cli/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/killercoda_cli/__init__.py
+-rwxr-xr-x   0        0        0    16830 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/killercoda_cli/cli.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/tests/__init__.py
+-rwxr-xr-x   0        0        0    12187 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/tests/test_cli.py
+-rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/tests/test_integration_cli.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/README.md
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 killercoda_cli-1.0.7/PKG-INFO
```

### Comparing `killercoda_cli-1.0.6/.github/workflows/ci.yml` & `killercoda_cli-1.0.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.6/killercoda_cli/cli.py` & `killercoda_cli-1.0.7/killercoda_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -336,17 +336,19 @@
     help_text = """
         Usage: killercoda-cli [OPTIONS]
 
         A CLI helper for writing KillerCoda scenarios and managing steps. This tool facilitates the addition, renaming, and renumbering of step files and directories in a structured and automated manner.
 
         Options:
           -h, --help    Show this message and exit.
+          -v, --version Display the version of the tool.
 
         Basic Commands:
-          No specific commands needed. Running 'killercoda-cli' starts the interactive process.
+          Running 'killercoda-cli' starts the interactive process.
+          init: Initialize a new project by creating an 'index.json' file.
 
         Requirements:
           - The tool must be run in a directory containing step files or directories (e.g., step1.md, step2/).
           - An 'index.json' file must be present in the directory, which contains metadata about the steps.
 
         Functionality:
           - Renames and renumbers step files and directories based on user input.
@@ -362,15 +364,26 @@
         elif operation.operation == "write_file":
             with open(operation.path, "w") as file:
                 file.write(operation.content)
         elif operation.operation == "chmod":
             os.chmod(operation.path, operation.mode)
         elif operation.operation == "rename":
             os.rename(operation.path, operation.content)
-
+def init_project():
+    """initialize a new project by creting index.json file"""
+    index_data = {
+        "details": {
+            "title": "Project Title",
+            "description": "Project Description",
+            "steps": [],
+        }
+    }
+    with open("index.json", "w") as index_file:
+        json.dump(index_data, index_file, ensure_ascii=False, indent=4)
+    print("Project initialized successfully. Please edit the 'index.json' file to add steps.")
 
 def main():
     """
     This function orchestrates the entire process of adding a new step to the scenario,
     from taking user input to updating the file system and the index.json file.
     It ensures that the 'index.json' file is present, gathers the current directory structure,
     prompts the user for the new step's title and number, calculates the necessary file operations,
@@ -380,14 +393,18 @@
     try:
         if len(sys.argv) > 1 and sys.argv[1] in ["-h", "--help"]:
             display_help()
             return
         if len(sys.argv) > 1 and sys.argv[1] in ["-v", "--version"]:
             print(f"killercoda-cli v{__version__}")
             return
+        if len(sys.argv) > 1 and sys.argv[1] in ["init"]:
+            init_project()
+            return
+        
         old_tree_structure = get_tree_structure()
         directory_items = os.listdir(".")
         steps_dict = get_current_steps_dict(directory_items)
         if "index.json" not in directory_items:
             print(
                 "The 'index.json' file is missing. Please ensure it is present in the current directory."
             )
```

### Comparing `killercoda_cli-1.0.6/tests/test_cli.py` & `killercoda_cli-1.0.7/tests/test_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -254,7 +254,31 @@
         assert (
             updated_data == expected_data
         ), "The updated index.json data did not match the expected output."
 
 
 if __name__ == "__main__":
     unittest.main()
+    @mock.patch("builtins.open", new_callable=mock.mock_open)
+    @mock.patch("json.dump")
+    @mock.patch("os.path.exists", return_value=False)
+    def test_init_project(self, mock_exists, mock_json_dump, mock_open):
+        cli.init_project()
+        mock_open.assert_called_once_with("index.json", "w")
+        mock_json_dump.assert_called_once()
+        expected_index_data = {
+            "details": {
+                "title": "Project Title",
+                "description": "Project Description",
+                "steps": [],
+            }
+        }
+        args, kwargs = mock_json_dump.call_args
+        self.assertEqual(args[0], expected_index_data, "The index.json data does not match the expected structure.")
+        self.assertTrue("ensure_ascii" in kwargs and not kwargs["ensure_ascii"], "ensure_ascii should be False.")
+        self.assertTrue("indent" in kwargs and kwargs["indent"] == 4, "Indentation should be set to 4.")
+
+    @mock.patch("sys.argv", ["killercoda-cli", "--version"])
+    @mock.patch("builtins.print")
+    def test_version_flag(self, mock_print):
+        cli.main()
+        mock_print.assert_called_with(f"killercoda-cli v{cli.__about__.__version__}")
```

### Comparing `killercoda_cli-1.0.6/tests/test_integration_cli.py` & `killercoda_cli-1.0.7/tests/test_integration_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.6/.gitignore` & `killercoda_cli-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.6/LICENSE.txt` & `killercoda_cli-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.6/README.md` & `killercoda_cli-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.6/pyproject.toml` & `killercoda_cli-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.6/PKG-INFO` & `killercoda_cli-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: killercoda-cli
-Version: 1.0.6
+Version: 1.0.7
 Summary: A CLI helper for writing killercoda scenarios and managing steps
 Project-URL: Documentation, https://github.com/unknown/killercoda-cli#readme
 Project-URL: Issues, https://github.com/unknown/killercoda-cli/issues
 Project-URL: Source, https://github.com/unknown/killercoda-cli
 Author-email: Piotr Zaniewski <piotrzan@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

