# Comparing `tmp/my_cli_code_explorer-0.1.3.tar.gz` & `tmp/my_cli_code_explorer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_cli_code_explorer-0.1.3.tar", last modified: Sun May 26 08:34:06 2024, max compression
+gzip compressed data, was "my_cli_code_explorer-0.1.4.tar", last modified: Sun May 26 08:37:48 2024, max compression
```

## Comparing `my_cli_code_explorer-0.1.3.tar` & `my_cli_code_explorer-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 08:34:06.768696 my_cli_code_explorer-0.1.3/
--rw-rw-rw-   0        0        0       16 2024-05-06 06:40:14.000000 my_cli_code_explorer-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      290 2024-05-26 08:34:06.766693 my_cli_code_explorer-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      572 2024-05-22 10:26:29.000000 my_cli_code_explorer-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 08:34:06.726015 my_cli_code_explorer-0.1.3/my_cli_code_explorer/
--rw-rw-rw-   0        0        0        0 2024-05-06 06:40:14.000000 my_cli_code_explorer-0.1.3/my_cli_code_explorer/__init__.py
--rw-rw-rw-   0        0        0     1412 2024-05-26 08:30:55.000000 my_cli_code_explorer-0.1.3/my_cli_code_explorer/main.py
-drwxrwxrwx   0        0        0        0 2024-05-26 08:34:06.763690 my_cli_code_explorer-0.1.3/my_cli_code_explorer.egg-info/
--rw-rw-rw-   0        0        0      290 2024-05-26 08:34:06.000000 my_cli_code_explorer-0.1.3/my_cli_code_explorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-26 08:34:06.000000 my_cli_code_explorer-0.1.3/my_cli_code_explorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 08:34:06.000000 my_cli_code_explorer-0.1.3/my_cli_code_explorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-05-26 08:34:06.000000 my_cli_code_explorer-0.1.3/my_cli_code_explorer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-26 08:34:06.000000 my_cli_code_explorer-0.1.3/my_cli_code_explorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-26 08:34:06.000000 my_cli_code_explorer-0.1.3/my_cli_code_explorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2024-05-22 11:04:12.000000 my_cli_code_explorer-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-26 08:34:06.769691 my_cli_code_explorer-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      662 2024-05-26 08:33:08.000000 my_cli_code_explorer-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:37:48.766151 my_cli_code_explorer-0.1.4/
+-rw-rw-rw-   0        0        0       16 2024-05-06 06:40:14.000000 my_cli_code_explorer-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      290 2024-05-26 08:37:48.764108 my_cli_code_explorer-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2024-05-22 10:26:29.000000 my_cli_code_explorer-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 08:37:48.738622 my_cli_code_explorer-0.1.4/my_cli_code_explorer/
+-rw-rw-rw-   0        0        0        0 2024-05-06 06:40:14.000000 my_cli_code_explorer-0.1.4/my_cli_code_explorer/__init__.py
+-rw-rw-rw-   0        0        0     1413 2024-05-26 08:37:08.000000 my_cli_code_explorer-0.1.4/my_cli_code_explorer/main.py
+drwxrwxrwx   0        0        0        0 2024-05-26 08:37:48.762095 my_cli_code_explorer-0.1.4/my_cli_code_explorer.egg-info/
+-rw-rw-rw-   0        0        0      290 2024-05-26 08:37:48.000000 my_cli_code_explorer-0.1.4/my_cli_code_explorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-05-26 08:37:48.000000 my_cli_code_explorer-0.1.4/my_cli_code_explorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 08:37:48.000000 my_cli_code_explorer-0.1.4/my_cli_code_explorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-26 08:37:48.000000 my_cli_code_explorer-0.1.4/my_cli_code_explorer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-26 08:37:48.000000 my_cli_code_explorer-0.1.4/my_cli_code_explorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-26 08:37:48.000000 my_cli_code_explorer-0.1.4/my_cli_code_explorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2024-05-22 11:04:12.000000 my_cli_code_explorer-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 08:37:48.767100 my_cli_code_explorer-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      662 2024-05-26 08:37:19.000000 my_cli_code_explorer-0.1.4/setup.py
```

### Comparing `my_cli_code_explorer-0.1.3/README.md` & `my_cli_code_explorer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `my_cli_code_explorer-0.1.3/my_cli_code_explorer/main.py` & `my_cli_code_explorer-0.1.4/my_cli_code_explorer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     git_branch: str = typer.Option(..., help="The Git branch"),
     app_name: str = typer.Option(..., help="The application name")
 ):
     """
     A CLI app that calls an API with given Git details and prints the CLI command.
     """
     # Call the API
-    print("git url", git_url)
+    #print("git url", git_url)
     headers = {
         "accept": "application/json",
         "Content-Type": "application/json"
     }
     body = {
         "git_req": {
             "git_url": git_url,
```

### Comparing `my_cli_code_explorer-0.1.3/setup.py` & `my_cli_code_explorer-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name="my_cli_code_explorer",  # Ensure your package name is consistent
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[
         "typer[all]",  # Install Typer with its dependencies
     ],
     entry_points={
         "console_scripts": [
             "my_cli_code_explorer=my_cli_code_explorer.main:app",  # Correct the entry point
```

