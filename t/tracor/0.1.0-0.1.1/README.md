# Comparing `tmp/tracor-0.1.0.tar.gz` & `tmp/tracor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracor-0.1.0.tar", last modified: Sun May 26 06:31:25 2024, max compression
+gzip compressed data, was "tracor-0.1.1.tar", last modified: Sun May 26 07:56:09 2024, max compression
```

## Comparing `tracor-0.1.0.tar` & `tracor-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 jairelan   (502) staff       (20)        0 2024-05-26 06:31:25.712261 tracor-0.1.0/
--rw-r--r--   0 jairelan   (502) staff       (20)     2638 2024-05-26 06:31:25.712065 tracor-0.1.0/PKG-INFO
--rw-r--r--   0 jairelan   (502) staff       (20)     2160 2024-05-26 05:31:20.000000 tracor-0.1.0/README.md
--rw-r--r--   0 jairelan   (502) staff       (20)       38 2024-05-26 06:31:25.712302 tracor-0.1.0/setup.cfg
--rw-r--r--   0 jairelan   (502) staff       (20)      803 2024-05-26 06:28:40.000000 tracor-0.1.0/setup.py
-drwxr-xr-x   0 jairelan   (502) staff       (20)        0 2024-05-26 06:31:25.711866 tracor-0.1.0/tracor.egg-info/
--rw-r--r--   0 jairelan   (502) staff       (20)     2638 2024-05-26 06:31:25.000000 tracor-0.1.0/tracor.egg-info/PKG-INFO
--rw-r--r--   0 jairelan   (502) staff       (20)      200 2024-05-26 06:31:25.000000 tracor-0.1.0/tracor.egg-info/SOURCES.txt
--rw-r--r--   0 jairelan   (502) staff       (20)        1 2024-05-26 06:31:25.000000 tracor-0.1.0/tracor.egg-info/dependency_links.txt
--rw-r--r--   0 jairelan   (502) staff       (20)       44 2024-05-26 06:31:25.000000 tracor-0.1.0/tracor.egg-info/entry_points.txt
--rw-r--r--   0 jairelan   (502) staff       (20)        9 2024-05-26 06:31:25.000000 tracor-0.1.0/tracor.egg-info/requires.txt
--rw-r--r--   0 jairelan   (502) staff       (20)        1 2024-05-26 06:31:25.000000 tracor-0.1.0/tracor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:56:09.684624 tracor-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 07:56:05.000000 tracor-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-26 07:56:09.684624 tracor-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-26 07:56:05.000000 tracor-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:56:09.684624 tracor-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-26 07:56:05.000000 tracor-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:56:09.684624 tracor-0.1.1/tracor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:56:09.000000 tracor-0.1.1/tracor.egg-info/top_level.txt
```

### Comparing `tracor-0.1.0/PKG-INFO` & `tracor-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: tracor
-Version: 0.1.0
-Summary: A tool for running Python scripts line by line with error handling and reporting.
-Home-page: https://github.com/ArlinJae/Tracor
-Author: Jae Arlin
-Author-email: jairelan.2005@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Requires-Dist: colorama
-
 # Tracor
 
 ## 🚀 Debug Python Scripts Faster
 
 This utility script allows you to execute a Python script line by line, catch any errors that occur along the way, and provide essential debugging information with enhanced context. Additionally, it generates a well-formatted Markdown report highlighting the errors encountered during execution.
 
 ## Features
@@ -27,16 +13,22 @@
 - Supports stopping execution on the first error or after a specified number of errors.
 - Includes options to show full tracebacks in the Markdown report.
 
 ## Usage
 
 ### Basic Usage
 
+You can download tracor from [PyPI](https://pypi.org/project/tracor/):
+```sh
+pip install tracor
+```
+
+Then, you can run it with:
 ```sh
-python main.py <script_path>
+tracor path/to/your_script.py [options]
 ```
 
 ### Usage With Flags
 * `--stop-on-error`: Stop execution on the first error.
 * `--output-file <file>`: Specify the output Markdown file for the error report.
 * `--log-level <level>`: Set the logging level (DEBUG, INFO, WARNING, ERROR, CRITICAL).
 * `--max-errors <n>`: Limit the number of errors to report before stopping execution.
@@ -44,16 +36,22 @@
 * `--execution-color <color>`: Color for executed lines (default: GREEN).
 * `--error-color <color>`: Color for error lines (default: RED).
 * `--code-color <color>`: Color for code in error messages (default: YELLOW).
 * `--type-color <color>`: Color for error type in error messages (default: CYAN).
 * `--message-color <color>`: Color for error message in error messages (default: MAGENTA).
 * `--traceback-color <color>`: Color for traceback in error messages (default: WHITE).
 
+
+Example - 
+```sh
+tracor example_script.py --output-file custom_error_report.md --log-level DEBUG --max-errors 5 --show-traceback --execution-color GREEN --error-color RED --code-color YELLOW --type-color CYAN --message-color MAGENTA --traceback-color WHITE
+```
+
 ## Output
 ### Terminal Output
 The terminal output will show the execution of each line and any errors encountered with enhanced multi-colored highlighting for better readability.
 
 ### Markdown Report
 A well-formatted Markdown report summarizing the errors will be generated. The report includes:
 
 A summary section with the total number of errors.
-A detailed table with line numbers, code snippets, error types, error messages, and tracebacks.
+A detailed table with line numbers, code snippets, error types, error messages, and tracebacks.
```

### Comparing `tracor-0.1.0/setup.py` & `tracor-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# setup.py
-
 from setuptools import setup, find_packages
 
 setup(
     name="tracor",
-    version="0.1.0",
+    version="0.1.1",  # Ensure this is the updated version
     packages=find_packages(),
     install_requires=[
         "colorama",
     ],
     entry_points={
         'console_scripts': [
             'tracor = tracor.core:main',
```

### Comparing `tracor-0.1.0/tracor.egg-info/PKG-INFO` & `tracor-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: tracor
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for running Python scripts line by line with error handling and reporting.
 Home-page: https://github.com/ArlinJae/Tracor
 Author: Jae Arlin
 Author-email: jairelan.2005@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: colorama
 
 # Tracor
 
 ## 🚀 Debug Python Scripts Faster
 
 This utility script allows you to execute a Python script line by line, catch any errors that occur along the way, and provide essential debugging information with enhanced context. Additionally, it generates a well-formatted Markdown report highlighting the errors encountered during execution.
@@ -27,16 +28,22 @@
 - Supports stopping execution on the first error or after a specified number of errors.
 - Includes options to show full tracebacks in the Markdown report.
 
 ## Usage
 
 ### Basic Usage
 
+You can download tracor from [PyPI](https://pypi.org/project/tracor/):
 ```sh
-python main.py <script_path>
+pip install tracor
+```
+
+Then, you can run it with:
+```sh
+tracor path/to/your_script.py [options]
 ```
 
 ### Usage With Flags
 * `--stop-on-error`: Stop execution on the first error.
 * `--output-file <file>`: Specify the output Markdown file for the error report.
 * `--log-level <level>`: Set the logging level (DEBUG, INFO, WARNING, ERROR, CRITICAL).
 * `--max-errors <n>`: Limit the number of errors to report before stopping execution.
@@ -44,14 +51,20 @@
 * `--execution-color <color>`: Color for executed lines (default: GREEN).
 * `--error-color <color>`: Color for error lines (default: RED).
 * `--code-color <color>`: Color for code in error messages (default: YELLOW).
 * `--type-color <color>`: Color for error type in error messages (default: CYAN).
 * `--message-color <color>`: Color for error message in error messages (default: MAGENTA).
 * `--traceback-color <color>`: Color for traceback in error messages (default: WHITE).
 
+
+Example - 
+```sh
+tracor example_script.py --output-file custom_error_report.md --log-level DEBUG --max-errors 5 --show-traceback --execution-color GREEN --error-color RED --code-color YELLOW --type-color CYAN --message-color MAGENTA --traceback-color WHITE
+```
+
 ## Output
 ### Terminal Output
 The terminal output will show the execution of each line and any errors encountered with enhanced multi-colored highlighting for better readability.
 
 ### Markdown Report
 A well-formatted Markdown report summarizing the errors will be generated. The report includes:
```

