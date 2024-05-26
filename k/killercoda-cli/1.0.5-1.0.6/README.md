# Comparing `tmp/killercoda_cli-1.0.5.tar.gz` & `tmp/killercoda_cli-1.0.6.tar.gz`

## Comparing `killercoda_cli-1.0.5.tar` & `killercoda_cli-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/.coveragerc
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/killercoda_cli/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/killercoda_cli/__init__.py
--rwxr-xr-x   0        0        0    16127 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/killercoda_cli/cli.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/tests/__init__.py
--rwxr-xr-x   0        0        0    11001 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/tests/test_cli.py
--rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/tests/test_integration_cli.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/README.md
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 killercoda_cli-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/.coveragerc
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/killercoda_cli/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/killercoda_cli/__init__.py
+-rwxr-xr-x   0        0        0    16149 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/killercoda_cli/cli.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/tests/__init__.py
+-rwxr-xr-x   0        0        0    11001 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/tests/test_cli.py
+-rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/tests/test_integration_cli.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/README.md
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 killercoda_cli-1.0.6/PKG-INFO
```

### Comparing `killercoda_cli-1.0.5/.github/workflows/ci.yml` & `killercoda_cli-1.0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.5/killercoda_cli/cli.py` & `killercoda_cli-1.0.6/killercoda_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,15 +377,15 @@
     and applies those changes to the file system and the index.json file.
     Finally, it outputs the changes to the directory structure for the user to review.
     """
     try:
         if len(sys.argv) > 1 and sys.argv[1] in ["-h", "--help"]:
             display_help()
             return
-        if sys.argv[1] in ["-v", "--version"]:
+        if len(sys.argv) > 1 and sys.argv[1] in ["-v", "--version"]:
             print(f"killercoda-cli v{__version__}")
             return
         old_tree_structure = get_tree_structure()
         directory_items = os.listdir(".")
         steps_dict = get_current_steps_dict(directory_items)
         if "index.json" not in directory_items:
             print(
```

### Comparing `killercoda_cli-1.0.5/tests/test_cli.py` & `killercoda_cli-1.0.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.5/tests/test_integration_cli.py` & `killercoda_cli-1.0.6/tests/test_integration_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.5/.gitignore` & `killercoda_cli-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.5/LICENSE.txt` & `killercoda_cli-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.5/README.md` & `killercoda_cli-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.5/pyproject.toml` & `killercoda_cli-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.5/PKG-INFO` & `killercoda_cli-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: killercoda-cli
-Version: 1.0.5
+Version: 1.0.6
 Summary: A CLI helper for writing killercoda scenarios and managing steps
 Project-URL: Documentation, https://github.com/unknown/killercoda-cli#readme
 Project-URL: Issues, https://github.com/unknown/killercoda-cli/issues
 Project-URL: Source, https://github.com/unknown/killercoda-cli
 Author-email: Piotr Zaniewski <piotrzan@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

