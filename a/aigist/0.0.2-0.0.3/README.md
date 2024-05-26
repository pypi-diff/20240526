# Comparing `tmp/aigist-0.0.2.tar.gz` & `tmp/aigist-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigist-0.0.2.tar", last modified: Sun May 26 04:56:40 2024, max compression
+gzip compressed data, was "aigist-0.0.3.tar", last modified: Sun May 26 04:59:30 2024, max compression
```

## Comparing `aigist-0.0.2.tar` & `aigist-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.418840 aigist-0.0.2/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1060 2024-05-25 17:21:20.000000 aigist-0.0.2/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6244 2024-05-26 04:56:40.418840 aigist-0.0.2/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5231 2024-05-26 04:56:21.000000 aigist-0.0.2/README.md
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.414840 aigist-0.0.2/aigist/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:35:37.000000 aigist-0.0.2/aigist/__init__.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.414840 aigist-0.0.2/aigist/app/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-05-25 17:22:10.000000 aigist-0.0.2/aigist/app/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      211 2024-05-25 17:22:10.000000 aigist-0.0.2/aigist/app/database.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      370 2024-05-26 04:24:22.000000 aigist-0.0.2/aigist/app/lite_llm.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      651 2024-05-26 03:45:02.000000 aigist-0.0.2/aigist/app/models.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2424 2024-05-25 18:03:00.000000 aigist-0.0.2/aigist/app/services.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7286 2024-05-26 04:45:01.000000 aigist-0.0.2/aigist/main.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.418840 aigist-0.0.2/aigist.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6244 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      397 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/entry_points.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       56 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/top_level.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-05-26 04:56:40.418840 aigist-0.0.2/setup.cfg
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1449 2024-05-26 04:56:36.000000 aigist-0.0.2/setup.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.418840 aigist-0.0.2/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      727 2024-05-25 17:37:46.000000 aigist-0.0.2/tests/test_main.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      486 2024-05-25 17:22:10.000000 aigist-0.0.2/tests/test_services.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:59:30.562833 aigist-0.0.3/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1060 2024-05-25 17:21:20.000000 aigist-0.0.3/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6936 2024-05-26 04:59:30.562833 aigist-0.0.3/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5923 2024-05-26 04:59:22.000000 aigist-0.0.3/README.md
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:59:30.558833 aigist-0.0.3/aigist/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:35:37.000000 aigist-0.0.3/aigist/__init__.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:59:30.562833 aigist-0.0.3/aigist/app/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-05-25 17:22:10.000000 aigist-0.0.3/aigist/app/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      211 2024-05-25 17:22:10.000000 aigist-0.0.3/aigist/app/database.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      370 2024-05-26 04:24:22.000000 aigist-0.0.3/aigist/app/lite_llm.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      651 2024-05-26 03:45:02.000000 aigist-0.0.3/aigist/app/models.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2424 2024-05-25 18:03:00.000000 aigist-0.0.3/aigist/app/services.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7286 2024-05-26 04:45:01.000000 aigist-0.0.3/aigist/main.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:59:30.562833 aigist-0.0.3/aigist.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6936 2024-05-26 04:59:30.000000 aigist-0.0.3/aigist.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      397 2024-05-26 04:59:30.000000 aigist-0.0.3/aigist.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-05-26 04:59:30.000000 aigist-0.0.3/aigist.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-05-26 04:59:30.000000 aigist-0.0.3/aigist.egg-info/entry_points.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       56 2024-05-26 04:59:30.000000 aigist-0.0.3/aigist.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-05-26 04:59:30.000000 aigist-0.0.3/aigist.egg-info/top_level.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-05-26 04:59:30.562833 aigist-0.0.3/setup.cfg
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1449 2024-05-26 04:59:28.000000 aigist-0.0.3/setup.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:59:30.562833 aigist-0.0.3/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      727 2024-05-25 17:37:46.000000 aigist-0.0.3/tests/test_main.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      486 2024-05-25 17:22:10.000000 aigist-0.0.3/tests/test_services.py
```

### Comparing `aigist-0.0.2/LICENSE` & `aigist-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aigist-0.0.2/PKG-INFO` & `aigist-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigist
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project provides a FastAPI application to create and update GitHub gists using the GitHub API. It includes SQLite for persistence and is designed to run in a GitHub Codespace.
 Home-page: 
 Author: rUv
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,25 @@
 |     | |  |  | |_ -|  _|
 |__|__|_|_____|_|___|_|  
                                       
     Created by rUv
 ```
 # Ai Gist
 
-This project provides a FastAPI application to create and update GitHub gists using the GitHub API. It includes SQLite for persistence and is designed to run in a GitHub Codespace.
+Ai Gist is python application designed to help you create and manage GitHub gists effortlessly using the GitHub API. With built-in SQLite for persistence and seamless integration with AI language models (LLMs), Ai Gist offers powerful capabilities for automating your workflow.
+
+## Key Features
+
+- **Easy Gist Management**: Create, update, and list GitHub gists with simple API calls.
+- **AI-Powered Interactions**: Utilize advanced AI language models to interpret user messages and perform actions based on responses.
+- **SQLite Integration**: Store and manage data locally with SQLite, ensuring persistence and reliability.
+- **FastAPI Framework**: Benefit from the high performance and ease of use provided by the FastAPI framework.
+
+Get started quickly by installing the application and running the server to leverage these features for an enhanced coding experience.
+
 
 ## Setup
 
 1. **Create a GitHub Codespace**:
    - Create a new GitHub Codespace for your repository.
    - Ensure your GitHub token is stored as a secret in the Codespace.
```

### Comparing `aigist-0.0.2/README.md` & `aigist-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,25 @@
 |     | |  |  | |_ -|  _|
 |__|__|_|_____|_|___|_|  
                                       
     Created by rUv
 ```
 # Ai Gist
 
-This project provides a FastAPI application to create and update GitHub gists using the GitHub API. It includes SQLite for persistence and is designed to run in a GitHub Codespace.
+Ai Gist is python application designed to help you create and manage GitHub gists effortlessly using the GitHub API. With built-in SQLite for persistence and seamless integration with AI language models (LLMs), Ai Gist offers powerful capabilities for automating your workflow.
+
+## Key Features
+
+- **Easy Gist Management**: Create, update, and list GitHub gists with simple API calls.
+- **AI-Powered Interactions**: Utilize advanced AI language models to interpret user messages and perform actions based on responses.
+- **SQLite Integration**: Store and manage data locally with SQLite, ensuring persistence and reliability.
+- **FastAPI Framework**: Benefit from the high performance and ease of use provided by the FastAPI framework.
+
+Get started quickly by installing the application and running the server to leverage these features for an enhanced coding experience.
+
 
 ## Setup
 
 1. **Create a GitHub Codespace**:
    - Create a new GitHub Codespace for your repository.
    - Ensure your GitHub token is stored as a secret in the Codespace.
```

### Comparing `aigist-0.0.2/aigist/app/models.py` & `aigist-0.0.3/aigist/app/models.py`

 * *Files identical despite different names*

### Comparing `aigist-0.0.2/aigist/app/services.py` & `aigist-0.0.3/aigist/app/services.py`

 * *Files identical despite different names*

### Comparing `aigist-0.0.2/aigist/main.py` & `aigist-0.0.3/aigist/main.py`

 * *Files identical despite different names*

### Comparing `aigist-0.0.2/aigist.egg-info/PKG-INFO` & `aigist-0.0.3/aigist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigist
-Version: 0.0.2
+Version: 0.0.3
 Summary: This project provides a FastAPI application to create and update GitHub gists using the GitHub API. It includes SQLite for persistence and is designed to run in a GitHub Codespace.
 Home-page: 
 Author: rUv
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,25 @@
 |     | |  |  | |_ -|  _|
 |__|__|_|_____|_|___|_|  
                                       
     Created by rUv
 ```
 # Ai Gist
 
-This project provides a FastAPI application to create and update GitHub gists using the GitHub API. It includes SQLite for persistence and is designed to run in a GitHub Codespace.
+Ai Gist is python application designed to help you create and manage GitHub gists effortlessly using the GitHub API. With built-in SQLite for persistence and seamless integration with AI language models (LLMs), Ai Gist offers powerful capabilities for automating your workflow.
+
+## Key Features
+
+- **Easy Gist Management**: Create, update, and list GitHub gists with simple API calls.
+- **AI-Powered Interactions**: Utilize advanced AI language models to interpret user messages and perform actions based on responses.
+- **SQLite Integration**: Store and manage data locally with SQLite, ensuring persistence and reliability.
+- **FastAPI Framework**: Benefit from the high performance and ease of use provided by the FastAPI framework.
+
+Get started quickly by installing the application and running the server to leverage these features for an enhanced coding experience.
+
 
 ## Setup
 
 1. **Create a GitHub Codespace**:
    - Create a new GitHub Codespace for your repository.
    - Ensure your GitHub token is stored as a secret in the Codespace.
```

### Comparing `aigist-0.0.2/setup.py` & `aigist-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='aigist',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
         'black',
```

### Comparing `aigist-0.0.2/tests/test_main.py` & `aigist-0.0.3/tests/test_main.py`

 * *Files identical despite different names*

