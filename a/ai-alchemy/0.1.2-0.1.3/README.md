# Comparing `tmp/ai_alchemy-0.1.2.tar.gz` & `tmp/ai_alchemy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_alchemy-0.1.2.tar", max compression
+gzip compressed data, was "ai_alchemy-0.1.3.tar", max compression
```

## Comparing `ai_alchemy-0.1.2.tar` & `ai_alchemy-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0        0 2024-05-11 15:33:37.265411 ai_alchemy-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-11 15:33:37.265411 ai_alchemy-0.1.2/ai_alchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 18:09:08.354325 ai_alchemy-0.1.2/ai_alchemy/core/__init__.py
--rw-r--r--   0        0        0     1122 2024-05-26 13:58:19.892493 ai_alchemy-0.1.2/ai_alchemy/core/ai.py
--rw-r--r--   0        0        0     3908 2024-05-26 13:57:31.843641 ai_alchemy-0.1.2/ai_alchemy/core/cast.py
--rw-r--r--   0        0        0        0 2024-05-26 13:58:28.808652 ai_alchemy-0.1.2/ai_alchemy/server.py
--rw-r--r--   0        0        0      575 2024-05-26 14:06:06.779655 ai_alchemy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 ai_alchemy-0.1.2/setup.py
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 ai_alchemy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1265 2024-05-26 14:16:20.744590 ai_alchemy-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 15:33:37.265411 ai_alchemy-0.1.3/ai_alchemy/__init__.py
+-rw-r--r--   0        0        0       85 2024-05-26 15:05:18.718403 ai_alchemy-0.1.3/ai_alchemy/ai.py
+-rw-r--r--   0        0        0      178 2024-05-26 15:04:12.359955 ai_alchemy-0.1.3/ai_alchemy/cast.py
+-rw-r--r--   0        0        0        0 2024-05-18 18:09:08.354325 ai_alchemy-0.1.3/ai_alchemy/core/__init__.py
+-rw-r--r--   0        0        0     1134 2024-05-26 14:08:36.369856 ai_alchemy-0.1.3/ai_alchemy/core/ai.py
+-rw-r--r--   0        0        0     3908 2024-05-26 13:57:31.843641 ai_alchemy-0.1.3/ai_alchemy/core/cast.py
+-rw-r--r--   0        0        0        0 2024-05-26 13:58:28.808652 ai_alchemy-0.1.3/ai_alchemy/server.py
+-rw-r--r--   0        0        0      575 2024-05-26 15:06:23.185741 ai_alchemy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 ai_alchemy-0.1.3/setup.py
+-rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 ai_alchemy-0.1.3/PKG-INFO
```

### Comparing `ai_alchemy-0.1.2/ai_alchemy/core/ai.py` & `ai_alchemy-0.1.3/ai_alchemy/core/ai.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 
 class OpenAIWrapper(AiWrapper):
     # overriding abstract method
     def __init__(self, api_key: str) -> None:
         self.api_key = api_key
         self.client = OpenAI()
         self.client.api_key = api_key
+        self.model = "gpt-3.5-turbo"
 
-    def call(self, input:str, model: str = "gpt-3.5-turbo") -> Generator[str, None, None]: # type: ignore
+    def call(self, input:str) -> Generator[str, None, None]: # type: ignore
         client = OpenAI()
         client.api_key = self.api_key
         stream = client.chat.completions.create(
-            model=model,
+            model=self.model,
             messages=[{"role": "user", "content": input}],
             stream=True,
         )
         for chunk in stream:
             if chunk.choices[0].delta.content is not None:
                 yield chunk.choices[0].delta.content
```

### Comparing `ai_alchemy-0.1.2/ai_alchemy/core/cast.py` & `ai_alchemy-0.1.3/ai_alchemy/core/cast.py`

 * *Files identical despite different names*

### Comparing `ai_alchemy-0.1.2/pyproject.toml` & `ai_alchemy-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-alchemy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic."
 authors = ["Josh Mogil"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

