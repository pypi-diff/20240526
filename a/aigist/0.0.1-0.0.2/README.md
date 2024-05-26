# Comparing `tmp/aigist-0.0.1.tar.gz` & `tmp/aigist-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigist-0.0.1.tar", last modified: Sun May 26 04:51:37 2024, max compression
+gzip compressed data, was "aigist-0.0.2.tar", last modified: Sun May 26 04:56:40 2024, max compression
```

## Comparing `aigist-0.0.1.tar` & `aigist-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:51:37.334851 aigist-0.0.1/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1060 2024-05-25 17:21:20.000000 aigist-0.0.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5771 2024-05-26 04:51:37.334851 aigist-0.0.1/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4759 2024-05-25 18:19:14.000000 aigist-0.0.1/README.md
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:51:37.330851 aigist-0.0.1/aigist/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:35:37.000000 aigist-0.0.1/aigist/__init__.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:51:37.330851 aigist-0.0.1/aigist/app/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-05-25 17:22:10.000000 aigist-0.0.1/aigist/app/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      211 2024-05-25 17:22:10.000000 aigist-0.0.1/aigist/app/database.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      370 2024-05-26 04:24:22.000000 aigist-0.0.1/aigist/app/lite_llm.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      651 2024-05-26 03:45:02.000000 aigist-0.0.1/aigist/app/models.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2424 2024-05-25 18:03:00.000000 aigist-0.0.1/aigist/app/services.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7286 2024-05-26 04:45:01.000000 aigist-0.0.1/aigist/main.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:51:37.334851 aigist-0.0.1/aigist.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5771 2024-05-26 04:51:37.000000 aigist-0.0.1/aigist.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      397 2024-05-26 04:51:37.000000 aigist-0.0.1/aigist.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-05-26 04:51:37.000000 aigist-0.0.1/aigist.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-05-26 04:51:37.000000 aigist-0.0.1/aigist.egg-info/entry_points.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       56 2024-05-26 04:51:37.000000 aigist-0.0.1/aigist.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-05-26 04:51:37.000000 aigist-0.0.1/aigist.egg-info/top_level.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-05-26 04:51:37.334851 aigist-0.0.1/setup.cfg
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1449 2024-05-26 04:38:33.000000 aigist-0.0.1/setup.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:51:37.334851 aigist-0.0.1/tests/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      727 2024-05-25 17:37:46.000000 aigist-0.0.1/tests/test_main.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      486 2024-05-25 17:22:10.000000 aigist-0.0.1/tests/test_services.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.418840 aigist-0.0.2/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1060 2024-05-25 17:21:20.000000 aigist-0.0.2/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6244 2024-05-26 04:56:40.418840 aigist-0.0.2/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     5231 2024-05-26 04:56:21.000000 aigist-0.0.2/README.md
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.414840 aigist-0.0.2/aigist/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:35:37.000000 aigist-0.0.2/aigist/__init__.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.414840 aigist-0.0.2/aigist/app/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-05-25 17:22:10.000000 aigist-0.0.2/aigist/app/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      211 2024-05-25 17:22:10.000000 aigist-0.0.2/aigist/app/database.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      370 2024-05-26 04:24:22.000000 aigist-0.0.2/aigist/app/lite_llm.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      651 2024-05-26 03:45:02.000000 aigist-0.0.2/aigist/app/models.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2424 2024-05-25 18:03:00.000000 aigist-0.0.2/aigist/app/services.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     7286 2024-05-26 04:45:01.000000 aigist-0.0.2/aigist/main.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.418840 aigist-0.0.2/aigist.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6244 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      397 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       44 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/entry_points.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       56 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-05-26 04:56:40.000000 aigist-0.0.2/aigist.egg-info/top_level.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-05-26 04:56:40.418840 aigist-0.0.2/setup.cfg
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1449 2024-05-26 04:56:36.000000 aigist-0.0.2/setup.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-05-26 04:56:40.418840 aigist-0.0.2/tests/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      727 2024-05-25 17:37:46.000000 aigist-0.0.2/tests/test_main.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      486 2024-05-25 17:22:10.000000 aigist-0.0.2/tests/test_services.py
```

### Comparing `aigist-0.0.1/LICENSE` & `aigist-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aigist-0.0.1/PKG-INFO` & `aigist-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigist
-Version: 0.0.1
+Version: 0.0.2
 Summary: This project provides a FastAPI application to create and update GitHub gists using the GitHub API. It includes SQLite for persistence and is designed to run in a GitHub Codespace.
 Home-page: 
 Author: rUv
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Requires-Dist: setuptools
 Requires-Dist: wheel
 Requires-Dist: flake8
 Requires-Dist: black
 Requires-Dist: pytest
 Requires-Dist: pip-upgrader
 
-```                       
+```
  _____ _ _____ _     _   
 |  _  |_|   __|_|___| |_ 
 |     | |  |  | |_ -|  _|
 |__|__|_|_____|_|___|_|  
                                       
     Created by rUv
 ```
@@ -42,20 +42,41 @@
 1. **Create a GitHub Codespace**:
    - Create a new GitHub Codespace for your repository.
    - Ensure your GitHub token is stored as a secret in the Codespace.
 
 2. **Install Dependencies**:
    - The setup script will automatically install necessary dependencies and set up the environment.
 
-3. **Run the Application**:
+3. **Initialize the Database**:
+   - Run the database initialization script to create the necessary database and tables:
+     ```bash
+     python init_db.py
+     ```
+
+4. **Install the Package**:
+   - Install the package in editable mode:
+     ```bash
+     pip install aigist
+     ```
+
+5. **Run the Application**:
    - Start the FastAPI server using Uvicorn:
      ```bash
-     uvicorn app.main:app --reload
+     aigist
      ```
 
+## Configuration
+
+- **Environment Variables**:
+  - Ensure the following environment variables are set:
+    - `GITHUB_TOKEN`: Your GitHub token.
+    - `LITELLM_API_BASE`: The base URL for the LiteLLM API.
+    - `LITELLM_API_KEY`: Your LiteLLM API key.
+    - `LITELLM_MODEL`: The model to use for LiteLLM (e.g., gpt-4o-2024-05-1).
+
 ## Endpoints
 
 - **Create Gist**: `POST /gists`
   - **Request Body**:
     ```json
     {
       "description": "Sample Gist",
@@ -123,22 +144,17 @@
 Run the tests using pytest:
 ```bash
 pytest
 ```
 
 ## Database Setup
 
-To ensure the database and table setup is correct, run the `setup_database.sh` script:
-```bash
-./setup_database.sh
-```
-
-To check the database contents, use the `check_db.sh` script:
+To ensure the database and table setup is correct, run the `init_db.py` script:
 ```bash
-./check_db.sh
+python init_db.py
 ```
 
 ### Example JSON Payloads
 
 - **Create Gist**:
   ```json
   {
@@ -187,7 +203,8 @@
 - **Open-Source and Community-Driven**: Benefit from transparency and ongoing development by the open-source community.
 - **Reduced Complexity**: Simplifies interactions with different provider APIs.
 - **Increased Flexibility**: Allows experimentation with various LLMs.
 - **Improved Efficiency**: Saves time with uniform code structure and automated error handling.
 - **Cost-Effectiveness**: Optimizes costs by exploring different pricing models across providers.
 
 For more details, refer to the [LiteLLM documentation](https://docs.litellm.ai).
+
```

### Comparing `aigist-0.0.1/README.md` & `aigist-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-```                       
+```
  _____ _ _____ _     _   
 |  _  |_|   __|_|___| |_ 
 |     | |  |  | |_ -|  _|
 |__|__|_|_____|_|___|_|  
                                       
     Created by rUv
 ```
@@ -15,20 +15,41 @@
 1. **Create a GitHub Codespace**:
    - Create a new GitHub Codespace for your repository.
    - Ensure your GitHub token is stored as a secret in the Codespace.
 
 2. **Install Dependencies**:
    - The setup script will automatically install necessary dependencies and set up the environment.
 
-3. **Run the Application**:
+3. **Initialize the Database**:
+   - Run the database initialization script to create the necessary database and tables:
+     ```bash
+     python init_db.py
+     ```
+
+4. **Install the Package**:
+   - Install the package in editable mode:
+     ```bash
+     pip install aigist
+     ```
+
+5. **Run the Application**:
    - Start the FastAPI server using Uvicorn:
      ```bash
-     uvicorn app.main:app --reload
+     aigist
      ```
 
+## Configuration
+
+- **Environment Variables**:
+  - Ensure the following environment variables are set:
+    - `GITHUB_TOKEN`: Your GitHub token.
+    - `LITELLM_API_BASE`: The base URL for the LiteLLM API.
+    - `LITELLM_API_KEY`: Your LiteLLM API key.
+    - `LITELLM_MODEL`: The model to use for LiteLLM (e.g., gpt-4o-2024-05-1).
+
 ## Endpoints
 
 - **Create Gist**: `POST /gists`
   - **Request Body**:
     ```json
     {
       "description": "Sample Gist",
@@ -96,22 +117,17 @@
 Run the tests using pytest:
 ```bash
 pytest
 ```
 
 ## Database Setup
 
-To ensure the database and table setup is correct, run the `setup_database.sh` script:
-```bash
-./setup_database.sh
-```
-
-To check the database contents, use the `check_db.sh` script:
+To ensure the database and table setup is correct, run the `init_db.py` script:
 ```bash
-./check_db.sh
+python init_db.py
 ```
 
 ### Example JSON Payloads
 
 - **Create Gist**:
   ```json
   {
@@ -160,7 +176,8 @@
 - **Open-Source and Community-Driven**: Benefit from transparency and ongoing development by the open-source community.
 - **Reduced Complexity**: Simplifies interactions with different provider APIs.
 - **Increased Flexibility**: Allows experimentation with various LLMs.
 - **Improved Efficiency**: Saves time with uniform code structure and automated error handling.
 - **Cost-Effectiveness**: Optimizes costs by exploring different pricing models across providers.
 
 For more details, refer to the [LiteLLM documentation](https://docs.litellm.ai).
+
```

### Comparing `aigist-0.0.1/aigist/app/models.py` & `aigist-0.0.2/aigist/app/models.py`

 * *Files identical despite different names*

### Comparing `aigist-0.0.1/aigist/app/services.py` & `aigist-0.0.2/aigist/app/services.py`

 * *Files identical despite different names*

### Comparing `aigist-0.0.1/aigist/main.py` & `aigist-0.0.2/aigist/main.py`

 * *Files identical despite different names*

### Comparing `aigist-0.0.1/aigist.egg-info/PKG-INFO` & `aigist-0.0.2/aigist.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigist
-Version: 0.0.1
+Version: 0.0.2
 Summary: This project provides a FastAPI application to create and update GitHub gists using the GitHub API. It includes SQLite for persistence and is designed to run in a GitHub Codespace.
 Home-page: 
 Author: rUv
 Author-email: 
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Requires-Dist: setuptools
 Requires-Dist: wheel
 Requires-Dist: flake8
 Requires-Dist: black
 Requires-Dist: pytest
 Requires-Dist: pip-upgrader
 
-```                       
+```
  _____ _ _____ _     _   
 |  _  |_|   __|_|___| |_ 
 |     | |  |  | |_ -|  _|
 |__|__|_|_____|_|___|_|  
                                       
     Created by rUv
 ```
@@ -42,20 +42,41 @@
 1. **Create a GitHub Codespace**:
    - Create a new GitHub Codespace for your repository.
    - Ensure your GitHub token is stored as a secret in the Codespace.
 
 2. **Install Dependencies**:
    - The setup script will automatically install necessary dependencies and set up the environment.
 
-3. **Run the Application**:
+3. **Initialize the Database**:
+   - Run the database initialization script to create the necessary database and tables:
+     ```bash
+     python init_db.py
+     ```
+
+4. **Install the Package**:
+   - Install the package in editable mode:
+     ```bash
+     pip install aigist
+     ```
+
+5. **Run the Application**:
    - Start the FastAPI server using Uvicorn:
      ```bash
-     uvicorn app.main:app --reload
+     aigist
      ```
 
+## Configuration
+
+- **Environment Variables**:
+  - Ensure the following environment variables are set:
+    - `GITHUB_TOKEN`: Your GitHub token.
+    - `LITELLM_API_BASE`: The base URL for the LiteLLM API.
+    - `LITELLM_API_KEY`: Your LiteLLM API key.
+    - `LITELLM_MODEL`: The model to use for LiteLLM (e.g., gpt-4o-2024-05-1).
+
 ## Endpoints
 
 - **Create Gist**: `POST /gists`
   - **Request Body**:
     ```json
     {
       "description": "Sample Gist",
@@ -123,22 +144,17 @@
 Run the tests using pytest:
 ```bash
 pytest
 ```
 
 ## Database Setup
 
-To ensure the database and table setup is correct, run the `setup_database.sh` script:
-```bash
-./setup_database.sh
-```
-
-To check the database contents, use the `check_db.sh` script:
+To ensure the database and table setup is correct, run the `init_db.py` script:
 ```bash
-./check_db.sh
+python init_db.py
 ```
 
 ### Example JSON Payloads
 
 - **Create Gist**:
   ```json
   {
@@ -187,7 +203,8 @@
 - **Open-Source and Community-Driven**: Benefit from transparency and ongoing development by the open-source community.
 - **Reduced Complexity**: Simplifies interactions with different provider APIs.
 - **Increased Flexibility**: Allows experimentation with various LLMs.
 - **Improved Efficiency**: Saves time with uniform code structure and automated error handling.
 - **Cost-Effectiveness**: Optimizes costs by exploring different pricing models across providers.
 
 For more details, refer to the [LiteLLM documentation](https://docs.litellm.ai).
+
```

### Comparing `aigist-0.0.1/setup.py` & `aigist-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='aigist',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[
         'twine',
         'setuptools',
         'wheel',
         'flake8',
         'black',
```

### Comparing `aigist-0.0.1/tests/test_main.py` & `aigist-0.0.2/tests/test_main.py`

 * *Files identical despite different names*

