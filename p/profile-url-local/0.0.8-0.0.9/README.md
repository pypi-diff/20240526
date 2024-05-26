# Comparing `tmp/profile-url-local-0.0.8.tar.gz` & `tmp/profile_url_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile-url-local-0.0.8.tar", last modified: Wed Nov 29 18:18:51 2023, max compression
+gzip compressed data, was "profile_url_local-0.0.9.tar", last modified: Sun May 26 20:39:46 2024, max compression
```

## Comparing `profile-url-local-0.0.8.tar` & `profile_url_local-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 18:18:51.896191 profile-url-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2023-11-29 18:18:51.896191 profile-url-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-11-29 18:18:26.000000 profile-url-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 18:18:51.896191 profile-url-local-0.0.8/profile_url_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 18:18:51.896191 profile-url-local-0.0.8/profile_url_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 18:18:26.000000 profile-url-local-0.0.8/profile_url_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-11-29 18:18:26.000000 profile-url-local-0.0.8/profile_url_local/src/constants_url_profile_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2023-11-29 18:18:26.000000 profile-url-local-0.0.8/profile_url_local/src/profile_url_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-29 18:18:26.000000 profile-url-local-0.0.8/profile_url_local/src/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 18:18:51.896191 profile-url-local-0.0.8/profile_url_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2023-11-29 18:18:51.000000 profile-url-local-0.0.8/profile_url_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-11-29 18:18:51.000000 profile-url-local-0.0.8/profile_url_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 18:18:51.000000 profile-url-local-0.0.8/profile_url_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-29 18:18:51.000000 profile-url-local-0.0.8/profile_url_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-29 18:18:51.000000 profile-url-local-0.0.8/profile_url_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-11-29 18:18:26.000000 profile-url-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-29 18:18:51.896191 profile-url-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2023-11-29 18:18:26.000000 profile-url-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:46.389596 profile_url_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-26 20:39:46.389596 profile_url_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-26 20:39:07.000000 profile_url_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:46.385596 profile_url_local-0.0.9/profile_url_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:46.389596 profile_url_local-0.0.9/profile_url_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:07.000000 profile_url_local-0.0.9/profile_url_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-26 20:39:07.000000 profile_url_local-0.0.9/profile_url_local/src/constants_url_profile_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-26 20:39:07.000000 profile_url_local-0.0.9/profile_url_local/src/profile_url_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-26 20:39:07.000000 profile_url_local-0.0.9/profile_url_local/src/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:39:46.389596 profile_url_local-0.0.9/profile_url_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-26 20:39:46.000000 profile_url_local-0.0.9/profile_url_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-26 20:39:46.000000 profile_url_local-0.0.9/profile_url_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:39:46.000000 profile_url_local-0.0.9/profile_url_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 20:39:46.000000 profile_url_local-0.0.9/profile_url_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-26 20:39:46.000000 profile_url_local-0.0.9/profile_url_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-26 20:39:14.000000 profile_url_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 20:39:46.389596 profile_url_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-26 20:39:07.000000 profile_url_local-0.0.9/setup.py
```

### Comparing `profile-url-local-0.0.8/PKG-INFO` & `profile_url_local-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,49 @@
-Metadata-Version: 2.1
-Name: profile-url-local
-Version: 0.0.8
-Summary: PyPI Package for Circles profile-url-local Python
-Home-page: https://github.com/circles
-Author: Circles
-Author-email: info@circlez.ai
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: PyMySQL>=1.0.2
-Requires-Dist: pytest>=7.4.0
-Requires-Dist: mysql-connector>=2.2.9
-Requires-Dist: logzio-python-handler>=4.1.0
-Requires-Dist: user-context-remote>=0.0.17
-Requires-Dist: python-sdk-local>=0.0.27
-
 # python-package-template
+
 This repository is designed to help you create local and remote package layers in Python.  
 It focuses on building package layers and does not include GraphQL and REST-API layers.
 
 ## Download Environment
+
 To set up the environment, follow these steps in your terminal:
+
 ```shell
 git clone https://github.com/circles-zone/<your-repo>.git --branch dev  # or other branch
 cd <your-repo>
 git checkout -b BU-<new-branch>  # if a new branch is needed
 python -m venv venv
 pip install -r requirements.txt
 ... <edit your code> ...
 git add .
 git commit -m "Your commit message"
 git push origin BU-<your-branch>
 ```
 
-For more detailed information, refer to the [documentation](https://docs.google.com/document/d/1HKhwlhwLD3S8uJ9LPI7h4Nxu77-DXKZe/edit?usp=sharing&ouid=104468990154530891864&rtpof=true&sd=true).
+For more detailed information, refer to
+the [documentation](https://docs.google.com/document/d/1HKhwlhwLD3S8uJ9LPI7h4Nxu77-DXKZe/edit?usp=sharing&ouid=104468990154530891864&rtpof=true&sd=true).
 
 ## Check List:
 
 ### Directory Structure
 
 Ensure that the root directory has the following structure:
+
 - `.github/`
 - `.vscode/` (optional)
 - `directory_with_same_name_as_the_repo/`
-  - `db/`
-  - `reports/`
-  - `project_name/`
-    - `src/`
-      - `__init__.py`
-      - `example_class.py`
-    - `tests/`
-      - `example_class_test.py`
-    - `__init__.py`
+    - `db/`
+    - `reports/`
+    - `project_name/`
+        - `src/`
+            - `__init__.py`
+            - `example_class.py`
+        - `tests/`
+            - `example_class_test.py`
+        - `__init__.py`
 
 This setup enables easy switching to a mono repo configuration.
 
 ### Database Python Scripts
 
 Place `<table-name>.py` in the `/db` folder if needed.  
 There's no need for a separate file for `_ml` tables.  
@@ -68,32 +55,39 @@
 - Use `/db/<table-name>.py` to create the schema, tables, views (including `_ml_table`).
 - Use `/db/<table-name>_insert.py` to create metadata and test data records.
 
 ### Update `setup.py`
 
 Don't forget to update the `setup.py` file, including the package name and version.  
 Remember to upload the version after every deployment.
+
 ### Working with VS Code
+
 Ensure that you push the `launch.json` file to the repository.  
 This enables running and debugging the code smoothly.
 
 ### Unit Testing
+
 We recommend using `pytest` over the `unittest` package.  
 Create a `pytest.ini` file in the project directory, not the root directory.
 run in termianl: pytest
 
 ## Workflow Completion
-When you've addressed all the TODOs in the repository, using infrastructure classes like Logger, Database, Url, Importer, and others, make sure your Feature Branch GitHub Actions Workflow is green without warnings.  
-All tests should run in GitHub Actions, your code should be well-documented, the `README.md` file should be clear and self-explanatory, test coverage should be above 90%, and all lines of code should be covered by unit tests.
+
+When you've addressed all the TODOs in the repository, using infrastructure classes like Logger, Database, Url,
+Importer, and others, make sure your Feature Branch GitHub Actions Workflow is green without warnings.  
+All tests should run in GitHub Actions, your code should be well-documented, the `README.md` file should be clear and
+self-explanatory, test coverage should be above 90%, and all lines of code should be covered by unit tests.
 
 Once these conditions are met, you can filter and analyze your records in Logz.io.  
 Pull the `dev` branch to your Feature Branch and then create a Pull Request to `dev`.
 
 Good luck :)
 
 ## check your code visibility lint with flake (Mandatory before pusj):
+
 run those command
 python -m pip install flake8 pytest
 flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
 flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
 
 note: you should use autopep8 extension in your code!
```

### Comparing `profile-url-local-0.0.8/profile_url_local/src/constants_url_profile_local.py` & `profile_url_local-0.0.9/profile_url_local/src/constants_url_profile_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 
 class UrlProfileLocalConstants:
-
     URL_PROFILE_LOCAL_PYTHON_COMPONENT_ID = 234
     URL_PROFILE_COMPONENT_NAME = 'profile_url_local/profile_url_local.py'
     URL_PROFILE_TESTS_COMPONENT_NAME = 'tests/test_profile_url_local.py'
     SCHEMA_NAME = 'profile_url'
     DEFAULT_COLUMN_NAME = 'url'
     DEFAULT_TABLE_NAME = 'url_table'
```

### Comparing `profile-url-local-0.0.8/pyproject.toml` & `profile_url_local-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 # TODO: Please update the name, similar to storage-local (suffix -local)
 name = "<project-name>"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.1" # https://pypi.org/project/<project-name> i.e. https://pypi.org/project/storage-local/
+version = "0.0.2" # https://pypi.org/project/<project-name> i.e. https://pypi.org/project/storage-local/
 description = "<project-name> Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

