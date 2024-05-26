# Comparing `tmp/ai_alchemy-0.1.1.tar.gz` & `tmp/ai_alchemy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_alchemy-0.1.1.tar", max compression
+gzip compressed data, was "ai_alchemy-0.1.2.tar", max compression
```

## Comparing `ai_alchemy-0.1.1.tar` & `ai_alchemy-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-11 15:33:37.265411 ai_alchemy-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-11 15:33:37.265411 ai_alchemy-0.1.1/ai_alchemy/__init__.py
--rw-r--r--   0        0        0     1788 2024-05-11 19:44:02.911338 ai_alchemy-0.1.1/ai_alchemy/cast.py
--rw-r--r--   0        0        0        0 2024-05-11 18:18:45.413312 ai_alchemy-0.1.1/ai_alchemy/core/llm_wrapper.py
--rw-r--r--   0        0        0      840 2024-05-11 15:43:31.482338 ai_alchemy-0.1.1/ai_alchemy/server.py
--rw-r--r--   0        0        0      406 2024-05-11 18:24:18.795510 ai_alchemy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 ai_alchemy-0.1.1/setup.py
--rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 ai_alchemy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-11 15:33:37.265411 ai_alchemy-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 15:33:37.265411 ai_alchemy-0.1.2/ai_alchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 18:09:08.354325 ai_alchemy-0.1.2/ai_alchemy/core/__init__.py
+-rw-r--r--   0        0        0     1122 2024-05-26 13:58:19.892493 ai_alchemy-0.1.2/ai_alchemy/core/ai.py
+-rw-r--r--   0        0        0     3908 2024-05-26 13:57:31.843641 ai_alchemy-0.1.2/ai_alchemy/core/cast.py
+-rw-r--r--   0        0        0        0 2024-05-26 13:58:28.808652 ai_alchemy-0.1.2/ai_alchemy/server.py
+-rw-r--r--   0        0        0      575 2024-05-26 14:06:06.779655 ai_alchemy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      820 1970-01-01 00:00:00.000000 ai_alchemy-0.1.2/setup.py
+-rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 ai_alchemy-0.1.2/PKG-INFO
```

### Comparing `ai_alchemy-0.1.1/setup.py` & `ai_alchemy-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 packages = \
 ['ai_alchemy', 'ai_alchemy.core']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pandas>=2.2.2,<3.0.0', 'pydantic>=2.7.1,<3.0.0', 'requests>=2.31.0,<3.0.0']
+['openai>=1.30.1,<2.0.0',
+ 'pandas>=2.2.2,<3.0.0',
+ 'pydantic>=2.7.1,<3.0.0',
+ 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'ai-alchemy',
-    'version': '0.1.1',
-    'description': '',
+    'version': '0.1.2',
+    'description': 'Lightweight package for arbitrary data transformation and validation using AI models and first class python libraries like Pandas and Pydantic.',
     'long_description': '',
-    'author': 'Your Name',
-    'author_email': 'you@example.com',
+    'author': 'Josh Mogil',
+    'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
```

