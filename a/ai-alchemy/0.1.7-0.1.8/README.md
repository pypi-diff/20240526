# Comparing `tmp/ai_alchemy-0.1.7.tar.gz` & `tmp/ai_alchemy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_alchemy-0.1.7.tar", max compression
+gzip compressed data, was "ai_alchemy-0.1.8.tar", max compression
```

## Comparing `ai_alchemy-0.1.7.tar` & `ai_alchemy-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,8 @@
--rw-r--r--   0        0        0     1265 2024-05-26 14:16:20.744590 ai_alchemy-0.1.7/README.md
--rw-r--r--   0        0        0       45 2024-05-26 15:24:57.954957 ai_alchemy-0.1.7/ai_alchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 18:09:08.354325 ai_alchemy-0.1.7/ai_alchemy/core/__init__.py
--rw-r--r--   0        0        0     1138 2024-05-26 15:26:02.491543 ai_alchemy-0.1.7/ai_alchemy/core/_ai.py
--rw-r--r--   0        0        0       53 2024-05-26 15:26:45.203930 ai_alchemy-0.1.7/ai_alchemy/core/ai.py
--rw-r--r--   0        0        0     3907 2024-05-26 15:19:51.920310 ai_alchemy-0.1.7/ai_alchemy/core/cast.py
--rw-r--r--   0        0        0        0 2024-05-26 13:58:28.808652 ai_alchemy-0.1.7/ai_alchemy/server.py
--rw-r--r--   0        0        0      575 2024-05-26 15:27:03.828100 ai_alchemy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 ai_alchemy-0.1.7/setup.py
--rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 ai_alchemy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1265 2024-05-26 14:16:20.744590 ai_alchemy-0.1.8/README.md
+-rw-r--r--   0        0        0       45 2024-05-26 15:24:57.954957 ai_alchemy-0.1.8/ai_alchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 18:09:08.354325 ai_alchemy-0.1.8/ai_alchemy/core/__init__.py
+-rw-r--r--   0        0        0     1154 2024-05-26 15:37:11.833967 ai_alchemy-0.1.8/ai_alchemy/core/ai.py
+-rw-r--r--   0        0        0     3905 2024-05-26 15:38:51.615577 ai_alchemy-0.1.8/ai_alchemy/core/cast.py
+-rw-r--r--   0        0        0      575 2024-05-26 15:41:34.882044 ai_alchemy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 ai_alchemy-0.1.8/setup.py
+-rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 ai_alchemy-0.1.8/PKG-INFO
```

### Comparing `ai_alchemy-0.1.7/README.md` & `ai_alchemy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ai_alchemy-0.1.7/ai_alchemy/core/_ai.py` & `ai_alchemy-0.1.8/ai_alchemy/core/ai.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from abc import ABC, abstractmethod
+from abc import ABC 
+from abc import abstractmethod
 from openai import OpenAI
 from typing import Generator
 
 class AiWrapper(ABC):
     
     @abstractmethod
     def call(self, input: str, **kwargs) -> Generator[str, None, None]:
```

### Comparing `ai_alchemy-0.1.7/ai_alchemy/core/cast.py` & `ai_alchemy-0.1.8/ai_alchemy/core/cast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Type, Any
 from pandas import DataFrame
 from pydantic import BaseModel
-
 from ai_alchemy.core.ai import AiWrapper
 
-
 def dict_to_pydantic_model(input: dict, ai: AiWrapper, output: BaseModel):
     base_prompt = [
         "Given the following Pydantic schema and input dictionary, your task is to transform the dictionary into a JSON object. The JSON object should match the Pydantic schema exactly, and should not include the schema itself.",
         "Pydantic schema:",
         f"{output.model_json_schema()}",
         "Input dictionary:",
         f"{input}",
```

### Comparing `ai_alchemy-0.1.7/pyproject.toml` & `ai_alchemy-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-alchemy"
-version = "0.1.7"
+version = "0.1.8"
 description = "Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic."
 authors = ["Josh Mogil"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

### Comparing `ai_alchemy-0.1.7/setup.py` & `ai_alchemy-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['openai>=1.30.1,<2.0.0',
  'pandas>=2.2.2,<3.0.0',
  'pydantic>=2.7.1,<3.0.0',
  'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'ai-alchemy',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic.',
     'long_description': '# AI Alchemy\n\nAI Alchemy is a Python library that provides a convenient way to interact with AI models, such as OpenAI\'s GPT-3.5 Turbo, and perform transformations on data.\n\n## Getting Started\n\nThese instructions will get you a copy of the project up and running on your local machine for development and testing purposes.\n\n### Prerequisites\n\nYou need to have Python installed on your machine. You can download Python [here](https://www.python.org/downloads/).\n\n### Installation\n\nYou can install AI Alchemy via pip:\n\n```bash\npip install ai_alchemy\n```\n\n### Usage\nHere\'s a basic example of how to use AI Alchemy:\n\n```python\n# Import necessary libraries\nimport os\nimport ai_alchemy\nfrom ai_alchemy.ai import OpenAIWrapper\nfrom pydantic import BaseModel\n\n# Instantiate a wrapper for an AI model\nopenai = OpenAIWrapper(api_key=os.environ["OPENAI_API_KEY"], model="gpt-3.5-turbo")\n\n# Define a Pydantic model\nclass User(BaseModel):\n    name: str\n    age: int\n\n# Input data\ndata = "John Smith is 25 years old, five foot ten inches tall, and weighs 150 pounds."\n\n# Use AI Alchemy to transform the data into a Pydantic model\nmodel = ai_alchemy.cast.str_to_pydantic_model(data, openai, User)\n\n# Now `model` is a `User` instance with `name` and `age` populated from `data`\n```',
     'author': 'Josh Mogil',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ai_alchemy-0.1.7/PKG-INFO` & `ai_alchemy-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-alchemy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic.
 Author: Josh Mogil
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=1.30.1,<2.0.0)
```

