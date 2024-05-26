# Comparing `tmp/ai_alchemy-0.1.3.tar.gz` & `tmp/ai_alchemy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_alchemy-0.1.3.tar", max compression
+gzip compressed data, was "ai_alchemy-0.1.4.tar", max compression
```

## Comparing `ai_alchemy-0.1.3.tar` & `ai_alchemy-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1265 2024-05-26 14:16:20.744590 ai_alchemy-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-11 15:33:37.265411 ai_alchemy-0.1.3/ai_alchemy/__init__.py
--rw-r--r--   0        0        0       85 2024-05-26 15:05:18.718403 ai_alchemy-0.1.3/ai_alchemy/ai.py
--rw-r--r--   0        0        0      178 2024-05-26 15:04:12.359955 ai_alchemy-0.1.3/ai_alchemy/cast.py
--rw-r--r--   0        0        0        0 2024-05-18 18:09:08.354325 ai_alchemy-0.1.3/ai_alchemy/core/__init__.py
--rw-r--r--   0        0        0     1134 2024-05-26 14:08:36.369856 ai_alchemy-0.1.3/ai_alchemy/core/ai.py
--rw-r--r--   0        0        0     3908 2024-05-26 13:57:31.843641 ai_alchemy-0.1.3/ai_alchemy/core/cast.py
--rw-r--r--   0        0        0        0 2024-05-26 13:58:28.808652 ai_alchemy-0.1.3/ai_alchemy/server.py
--rw-r--r--   0        0        0      575 2024-05-26 15:06:23.185741 ai_alchemy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 ai_alchemy-0.1.3/setup.py
--rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 ai_alchemy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1265 2024-05-26 14:16:20.744590 ai_alchemy-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 15:33:37.265411 ai_alchemy-0.1.4/ai_alchemy/__init__.py
+-rw-r--r--   0        0        0      110 2024-05-26 15:10:26.742442 ai_alchemy-0.1.4/ai_alchemy/ai.py
+-rw-r--r--   0        0        0      256 2024-05-26 15:10:37.642526 ai_alchemy-0.1.4/ai_alchemy/cast.py
+-rw-r--r--   0        0        0        0 2024-05-18 18:09:08.354325 ai_alchemy-0.1.4/ai_alchemy/core/__init__.py
+-rw-r--r--   0        0        0     1134 2024-05-26 14:08:36.369856 ai_alchemy-0.1.4/ai_alchemy/core/ai.py
+-rw-r--r--   0        0        0     3908 2024-05-26 13:57:31.843641 ai_alchemy-0.1.4/ai_alchemy/core/cast.py
+-rw-r--r--   0        0        0        0 2024-05-26 13:58:28.808652 ai_alchemy-0.1.4/ai_alchemy/server.py
+-rw-r--r--   0        0        0      575 2024-05-26 15:10:52.622641 ai_alchemy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 ai_alchemy-0.1.4/setup.py
+-rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 ai_alchemy-0.1.4/PKG-INFO
```

### Comparing `ai_alchemy-0.1.3/README.md` & `ai_alchemy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ai_alchemy-0.1.3/ai_alchemy/core/ai.py` & `ai_alchemy-0.1.4/ai_alchemy/core/ai.py`

 * *Files identical despite different names*

### Comparing `ai_alchemy-0.1.3/ai_alchemy/core/cast.py` & `ai_alchemy-0.1.4/ai_alchemy/core/cast.py`

 * *Files identical despite different names*

### Comparing `ai_alchemy-0.1.3/pyproject.toml` & `ai_alchemy-0.1.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-alchemy"
-version = "0.1.3"
+version = "0.1.4"
 description = "Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic."
 authors = ["Josh Mogil"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

### Comparing `ai_alchemy-0.1.3/setup.py` & `ai_alchemy-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['openai>=1.30.1,<2.0.0',
  'pandas>=2.2.2,<3.0.0',
  'pydantic>=2.7.1,<3.0.0',
  'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'ai-alchemy',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic.',
     'long_description': '# AI Alchemy\n\nAI Alchemy is a Python library that provides a convenient way to interact with AI models, such as OpenAI\'s GPT-3.5 Turbo, and perform transformations on data.\n\n## Getting Started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nYou need to have Python installed on your machine. You can download Python [here](https://www.python.org/downloads/).\n\n### Installation\n\nYou can install AI Alchemy via pip:\n\n```bash\npip install ai_alchemy\n```\n\n### Usage\nHere\'s a basic example of how to use AI Alchemy:\n\n```python\n# Import necessary libraries\nimport os\nimport ai_alchemy\nfrom ai_alchemy.ai import OpenAIWrapper\nfrom pydantic import BaseModel\n\n# Instantiate a wrapper for an AI model\nopenai = OpenAIWrapper(api_key=os.environ["OPENAI_API_KEY"], model="gpt-3.5-turbo")\n\n# Define a Pydantic model\nclass User(BaseModel):\n    name: str\n    age: int\n\n# Input data\ndata = "John Smith is 25 years old, five foot ten inches tall, and weighs 150 pounds."\n\n# Use AI Alchemy to transform the data into a Pydantic model\nmodel = ai_alchemy.cast.str_to_pydantic_model(data, openai, User)\n\n# Now `model` is a `User` instance with `name` and `age` populated from `data`\n```',
     'author': 'Josh Mogil',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ai_alchemy-0.1.3/PKG-INFO` & `ai_alchemy-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-alchemy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic.
 Author: Josh Mogil
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=1.30.1,<2.0.0)
```

