# Comparing `tmp/killercoda_cli-1.0.3.tar.gz` & `tmp/killercoda_cli-1.0.4.tar.gz`

## Comparing `killercoda_cli-1.0.3.tar` & `killercoda_cli-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/.coveragerc
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/killercoda_cli/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/killercoda_cli/__init__.py
--rwxr-xr-x   0        0        0    16099 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/killercoda_cli/cli.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/tests/__init__.py
--rwxr-xr-x   0        0        0    11001 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/tests/test_cli.py
--rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/tests/test_integration_cli.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/README.md
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 killercoda_cli-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/.coveragerc
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/killercoda_cli/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/killercoda_cli/__init__.py
+-rwxr-xr-x   0        0        0    16265 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/killercoda_cli/cli.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/tests/__init__.py
+-rwxr-xr-x   0        0        0    11001 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/tests/test_cli.py
+-rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/tests/test_integration_cli.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/README.md
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 killercoda_cli-1.0.4/PKG-INFO
```

### Comparing `killercoda_cli-1.0.3/.github/workflows/ci.yml` & `killercoda_cli-1.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.3/killercoda_cli/cli.py` & `killercoda_cli-1.0.4/killercoda_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import difflib
 import json
 import os
 import subprocess
 import sys
 from typing import List, Optional
-
+from killercoda_cli.__about__ import __version__
 
 class FileOperation:
     """
     Define a type hint for the different types of file operations that can be performed.
     This Union type allows for specifying the operation (as a string literal indicating the type of action),
     and the required arguments for each operation type:
     - 'makedirs': Create a new directory; requires the path of the directory.
@@ -380,14 +380,17 @@
     and applies those changes to the file system and the index.json file.
     Finally, it outputs the changes to the directory structure for the user to review.
     """
     try:
         if len(sys.argv) > 1 and sys.argv[1] in ["-h", "--help"]:
             display_help()
             return
+        if sys.argv[1] in ["-v", "--version"]:
+            print(f"killercoda-cli v{__version__}")
+            return
         old_tree_structure = get_tree_structure()
         directory_items = os.listdir(".")
         steps_dict = get_current_steps_dict(directory_items)
         if "index.json" not in directory_items:
             print(
                 "The 'index.json' file is missing. Please ensure it is present in the current directory."
             )
```

### Comparing `killercoda_cli-1.0.3/tests/test_cli.py` & `killercoda_cli-1.0.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.3/tests/test_integration_cli.py` & `killercoda_cli-1.0.4/tests/test_integration_cli.py`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.3/.gitignore` & `killercoda_cli-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.3/LICENSE.txt` & `killercoda_cli-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.3/README.md` & `killercoda_cli-1.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 **Table of Contents**
 
 * [Installation](#installation)
 * [Introduction](#introduction)
 * [Documentation](#documentation)
   * [Requirements](#requirements)
   * [Example usage](#example-usage)
+* [Development](#development)
+* [Testing](#testing)
 * [Disclaimer](#disclaimer)
 * [License](#license)
-
+ 
 ## Installation
 
 ```console
 pip install killercoda-cli
 ```
 
 > [!NOTE]
@@ -115,14 +117,19 @@
       "title": "Step 2",
       "text": "step3/step3.md"
     }
   ]
 }
 ```
 
+## Development
+
+Installing locally with `pip install -e . --user` will allow you to run the tool
+locally.
+
 ## Testing
 
 To run the tests, use the following commands:
 
 Here is the text rendered as a Markdown list:
 
 * `hatch run test:unit` - to run the unit tests.
```

### Comparing `killercoda_cli-1.0.3/pyproject.toml` & `killercoda_cli-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `killercoda_cli-1.0.3/PKG-INFO` & `killercoda_cli-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: killercoda-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: A CLI helper for writing killercoda scenarios and managing steps
 Project-URL: Documentation, https://github.com/unknown/killercoda-cli#readme
 Project-URL: Issues, https://github.com/unknown/killercoda-cli/issues
 Project-URL: Source, https://github.com/unknown/killercoda-cli
 Author-email: Piotr Zaniewski <piotrzan@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -30,17 +30,19 @@
 **Table of Contents**
 
 * [Installation](#installation)
 * [Introduction](#introduction)
 * [Documentation](#documentation)
   * [Requirements](#requirements)
   * [Example usage](#example-usage)
+* [Development](#development)
+* [Testing](#testing)
 * [Disclaimer](#disclaimer)
 * [License](#license)
-
+ 
 ## Installation
 
 ```console
 pip install killercoda-cli
 ```
 
 > [!NOTE]
@@ -137,14 +139,19 @@
       "title": "Step 2",
       "text": "step3/step3.md"
     }
   ]
 }
 ```
 
+## Development
+
+Installing locally with `pip install -e . --user` will allow you to run the tool
+locally.
+
 ## Testing
 
 To run the tests, use the following commands:
 
 Here is the text rendered as a Markdown list:
 
 * `hatch run test:unit` - to run the unit tests.
```

