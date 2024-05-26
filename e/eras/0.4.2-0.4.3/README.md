# Comparing `tmp/eras-0.4.2.tar.gz` & `tmp/eras-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.4.2.tar", last modified: Sun May 26 00:20:29 2024, max compression
+gzip compressed data, was "eras-0.4.3.tar", last modified: Sun May 26 03:35:08 2024, max compression
```

## Comparing `eras-0.4.2.tar` & `eras-0.4.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.882862 eras-0.4.2/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.2/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.2/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 00:20:29.882037 eras-0.4.2/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.2/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.853708 eras-0.4.2/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.2/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.855881 eras-0.4.2/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.2/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.2/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.2/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.857537 eras-0.4.2/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.2/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.860650 eras-0.4.2/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.2/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.2/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.2/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.2/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.2/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.2/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.2/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.2/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.2/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.2/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.2/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.2/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.2/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.861406 eras-0.4.2/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.2/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.862658 eras-0.4.2/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.2/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.2/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.2/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.2/eras/config/config.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.863318 eras-0.4.2/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.2/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.864057 eras-0.4.2/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.2/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.2/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.2/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.865026 eras-0.4.2/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.2/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.866687 eras-0.4.2/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.2/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.2/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.2/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.2/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.2/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.2/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.2/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.2/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.869090 eras-0.4.2/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.2/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.872859 eras-0.4.2/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.2/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.2/eras/models/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.2/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.2/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.2/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.2/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.2/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.2/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.2/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.2/eras/models/constants.py
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.2/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.2/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.2/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.2/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.2/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.2/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.874523 eras-0.4.2/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.2/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.876384 eras-0.4.2/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.2/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.2/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.2/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4550 2024-05-25 23:05:46.000000 eras-0.4.2/eras/services/__pycache__/user_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3927 2024-05-25 23:35:32.000000 eras-0.4.2/eras/services/__pycache__/user_config_service.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.877821 eras-0.4.2/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.2/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.879770 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.2/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.2/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.2/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.2/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     2189 2024-05-25 23:04:34.000000 eras-0.4.2/eras/services/user_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     2885 2024-05-25 23:34:52.000000 eras-0.4.2/eras/services/user_config_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.880444 eras-0.4.2/eras/utils/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.2/eras/utils/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.881221 eras-0.4.2/eras/utils/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.2/eras/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.2/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.2/eras/utils/env_vars_and_profile_files.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.855104 eras-0.4.2/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       86 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 00:20:29.883041 eras-0.4.2/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1066 2024-05-26 00:20:04.000000 eras-0.4.2/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.752804 eras-0.4.3/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.3/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.3/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 03:35:08.752285 eras-0.4.3/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.3/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.720673 eras-0.4.3/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.3/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.723967 eras-0.4.3/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.3/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.3/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.3/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.726215 eras-0.4.3/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.3/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.729352 eras-0.4.3/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.3/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.3/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.3/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.3/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.3/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.3/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.3/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.3/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.3/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.3/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.3/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.3/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.3/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.729909 eras-0.4.3/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.3/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.731112 eras-0.4.3/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.3/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.3/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.3/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.3/eras/config/config.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.731830 eras-0.4.3/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.3/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.732623 eras-0.4.3/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.3/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.733697 eras-0.4.3/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.3/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.735485 eras-0.4.3/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.3/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.3/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.3/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.3/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.3/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.3/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.3/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.3/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.738327 eras-0.4.3/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.3/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.742588 eras-0.4.3/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.3/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.3/eras/models/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.3/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.3/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.3/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.3/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.3/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.3/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.3/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.3/eras/models/constants.py
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.3/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.3/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.3/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.3/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.3/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.3/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.743859 eras-0.4.3/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.3/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.745222 eras-0.4.3/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.3/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.3/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.3/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.3/eras/services/__pycache__/user_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7514 2024-05-26 03:32:31.000000 eras-0.4.3/eras/services/__pycache__/user_config_service.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.747018 eras-0.4.3/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.3/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.749529 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.3/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.3/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.3/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.3/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.3/eras/services/user_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)    10421 2024-05-26 03:32:28.000000 eras-0.4.3/eras/services/user_config_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.750735 eras-0.4.3/eras/utils/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.3/eras/utils/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.751543 eras-0.4.3/eras/utils/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.3/eras/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.3/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.3/eras/utils/env_vars_and_profile_files.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.723039 eras-0.4.3/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       86 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 03:35:08.752913 eras-0.4.3/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1066 2024-05-26 03:35:03.000000 eras-0.4.3/setup.py
```

### Comparing `eras-0.4.2/PKG-INFO` & `eras-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.2
+Version: 0.4.3
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.4.2/README.md` & `eras-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/__pycache__/main.cpython-311.pyc` & `eras-0.4.3/eras/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.4.3/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.4.3/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.4.3/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.4.3/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.4.3/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.4.3/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.4.3/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/llama_functions_agent.py` & `eras-0.4.3/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.4.3/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/llm_functions_agent.py` & `eras-0.4.3/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/simple_llm.py` & `eras-0.4.3/eras/agents/simple_llm.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/agents/terminal_llama_agent.py` & `eras-0.4.3/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.4.3/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.4.3/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/config/config.py` & `eras-0.4.3/eras/config/config.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.4.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/decorators/chatgpt_tool_data.py` & `eras-0.4.3/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.4.3/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.4.3/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.4.3/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.4.3/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/factories/function_details_factory.py` & `eras-0.4.3/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/factories/message_factory.py` & `eras-0.4.3/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/main.py` & `eras-0.4.3/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.4.3/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.4.3/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.4.3/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.4.3/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.4.3/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.4.3/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/conversation.py` & `eras-0.4.3/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/function_details.py` & `eras-0.4.3/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/message.py` & `eras-0.4.3/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/models/transaction.py` & `eras-0.4.3/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/run.ipynb` & `eras-0.4.3/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.4.3/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.4.3/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.4.3/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x826e5266 (Sat May 25 23:04:34 2024 UTC)
-files sz: 2189
+moddate:  0x84ab5266 (Sun May 26 03:24:52 2024 UTC)
+files sz: 1805
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -98,23 +98,23 @@
                       24 MAKE_FUNCTION            4 (annotations)
                       26 STORE_NAME               5 (handle_request)
          
           32          28 LOAD_CONST               4 (<code object handle_help_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 32>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (handle_help_request)
          
-          40          34 LOAD_CONST               5 (<code object handle_chat_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 40>)
+          36          34 LOAD_CONST               5 (<code object handle_chat_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 36>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               7 (handle_chat_request)
          
-          53          40 LOAD_CONST               6 (<code object handle_shell_nli_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 53>)
+          49          40 LOAD_CONST               6 (<code object handle_shell_nli_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 49>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               8 (handle_shell_nli_request)
          
-          56          46 LOAD_CONST               7 (<code object handle_config_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 56>)
+          52          46 LOAD_CONST               7 (<code object handle_config_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 52>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               9 (handle_config_request)
                       52 LOAD_CONST               8 (None)
                       54 RETURN_VALUE
          consts
             'UserCommandService'
             code
@@ -275,121 +275,90 @@
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_request'
                firstlineno 22
                lnotab 0x02012a012e012a012e012a012e02
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 3
+               stacksize : 2
                flags     : 3
                code
-                  0x97007401000000000000000000006401a6010000ab0100000000000000
-                  0001007401000000000000000000006402a6010000ab0100000000000000
-                  0001007401000000000000000000006403a6010000ab0100000000000000
-                  0001007401000000000000000000006404a6010000ab0100000000000000
-                  0001007401000000000000000000006405a6010000ab0100000000000000
-                  0001007401000000000000000000006406a6010000ab0100000000000000
-                  00010064005300
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  00000000000000a6000000ab00000000000000000001007c006a00000000
+                  0000000000a0020000000000000000000000000000000000000000a60000
+                  00ab000000000000000000010064005300
                 32           0 RESUME                   0
                
-                33           2 LOAD_GLOBAL              1 (NULL + print)
-                            14 LOAD_CONST               1 ('Welcome to ERAS - Easily Runnable AI Shell')
-                            16 PRECALL                  1
-                            20 CALL                     1
-                            30 POP_TOP
-               
-                34          32 LOAD_GLOBAL              1 (NULL + print)
-                            44 LOAD_CONST               2 ('Commands: ==============================================')
-                            46 PRECALL                  1
-                            50 CALL                     1
-                            60 POP_TOP
-               
-                35          62 LOAD_GLOBAL              1 (NULL + print)
-                            74 LOAD_CONST               3 ('{defualt usage} - Natural Languge Interface for running commands. e.g. eras how do I list all files in a directory -> %ls')
-                            76 PRECALL                  1
-                            80 CALL                     1
-                            90 POP_TOP
-               
-                36          92 LOAD_GLOBAL              1 (NULL + print)
-                           104 LOAD_CONST               4 ('/help - get info about commands')
-                           106 PRECALL                  1
-                           110 CALL                     1
-                           120 POP_TOP
-               
-                37         122 LOAD_GLOBAL              1 (NULL + print)
-                           134 LOAD_CONST               5 ('/chat - ask the LLM a question about anything. e.g. /chat tell me about quantum physics')
-                           136 PRECALL                  1
-                           140 CALL                     1
-                           150 POP_TOP
-               
-                38         152 LOAD_GLOBAL              1 (NULL + print)
-                           164 LOAD_CONST               6 ('/conf - configure eras. urls, keys, etc')
-                           166 PRECALL                  1
-                           170 CALL                     1
-                           180 POP_TOP
-                           182 LOAD_CONST               0 (None)
-                           184 RETURN_VALUE
+                33           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (user_config_service)
+                            14 LOAD_METHOD              1 (print_eras_logo)
+                            36 PRECALL                  0
+                            40 CALL                     0
+                            50 POP_TOP
+               
+                34          52 LOAD_FAST                0 (self)
+                            54 LOAD_ATTR                0 (user_config_service)
+                            64 LOAD_METHOD              2 (show_commands)
+                            86 PRECALL                  0
+                            90 CALL                     0
+                           100 POP_TOP
+                           102 LOAD_CONST               0 (None)
+                           104 RETURN_VALUE
                consts
                   None
-                  'Welcome to ERAS - Easily Runnable AI Shell'
-                  'Commands: =============================================='
-                  '{defualt usage} - Natural Languge Interface for running commands. e.g. eras how do I list all files in a directory -> %ls'
-                  '/help - get info about commands'
-                  '/chat - ask the LLM a question about anything. e.g. /chat tell me about quantum physics'
-                  '/conf - configure eras. urls, keys, etc'
-               names      ('print',)
+               names      ('user_config_service', 'print_eras_logo', 'show_commands')
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_help_request'
                firstlineno 32
-               lnotab 0x02011e011e011e011e011e01
+               lnotab 0x02013201
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a01000000000000000064017c01a6
                   020000ab0200000000000000007d027c0272157c02a00200000000000000
                   000000000000000000000000006402a6010000ab0100000000000000006e
                   0164007d03640384007d04640484007d057c006a030000000000000000a0
                   0400000000000000000000000000000000000000007c037c047c05a60300
                   00ab030000000000000000010064005300
-                40           0 RESUME                   0
+                36           0 RESUME                   0
                
-                41           2 LOAD_GLOBAL              1 (NULL + re)
+                37           2 LOAD_GLOBAL              1 (NULL + re)
                             14 LOAD_ATTR                1 (match)
                             24 LOAD_CONST               1 ('^/chat\\s+(.*)')
                             26 LOAD_FAST                1 (user_input)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 STORE_FAST               2 (match)
                
-                42          44 LOAD_FAST                2 (match)
+                38          44 LOAD_FAST                2 (match)
                             46 POP_JUMP_FORWARD_IF_FALSE    21 (to 90)
                             48 LOAD_FAST                2 (match)
                             50 LOAD_METHOD              2 (group)
                             72 LOAD_CONST               2 (1)
                             74 PRECALL                  1
                             78 CALL                     1
                             88 JUMP_FORWARD             1 (to 92)
                        >>   90 LOAD_CONST               0 (None)
                        >>   92 STORE_FAST               3 (prompt)
                
-                44          94 LOAD_CONST               3 (<code object handle_text_received, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 44>)
+                40          94 LOAD_CONST               3 (<code object handle_text_received, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 40>)
                             96 MAKE_FUNCTION            0
                             98 STORE_FAST               4 (handle_text_received)
                
-                47         100 LOAD_CONST               4 (<code object handle_response_complete, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 47>)
+                43         100 LOAD_CONST               4 (<code object handle_response_complete, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 43>)
                            102 MAKE_FUNCTION            0
                            104 STORE_FAST               5 (handle_response_complete)
                
-                50         106 LOAD_FAST                0 (self)
+                46         106 LOAD_FAST                0 (self)
                            108 LOAD_ATTR                3 (simple_llm)
                            118 LOAD_METHOD              4 (stream_inference)
                            140 LOAD_FAST                3 (prompt)
                            142 LOAD_FAST                4 (handle_text_received)
                            144 LOAD_FAST                5 (handle_response_complete)
                            146 PRECALL                  3
                            150 CALL                     3
@@ -404,17 +373,17 @@
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 4
                      flags     : 19
                      code
                         0x97007401000000000000000000007c006401ac02a6020000ab02000000
                         0000000000010064005300
-                      44           0 RESUME                   0
+                      40           0 RESUME                   0
                      
-                      45           2 LOAD_GLOBAL              1 (NULL + print)
+                      41           2 LOAD_GLOBAL              1 (NULL + print)
                                   14 LOAD_FAST                0 (text)
                                   16 LOAD_CONST               1 ('')
                                   18 KW_NAMES                 2
                                   20 PRECALL                  2
                                   24 CALL                     2
                                   34 POP_TOP
                                   36 LOAD_CONST               0 (None)
@@ -425,61 +394,61 @@
                         ('end',)
                      names      ('print',)
                      varnames   ('text',)
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                      name       'handle_text_received'
-                     firstlineno 44
+                     firstlineno 40
                      lnotab 0x0201
                   code
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 2
                      flags     : 19
                      code
                         0x9700740100000000000000000000a6000000ab00000000000000000001
                         0064005300
-                      47           0 RESUME                   0
+                      43           0 RESUME                   0
                      
-                      48           2 LOAD_GLOBAL              1 (NULL + print)
+                      44           2 LOAD_GLOBAL              1 (NULL + print)
                                   14 PRECALL                  0
                                   18 CALL                     0
                                   28 POP_TOP
                                   30 LOAD_CONST               0 (None)
                                   32 RETURN_VALUE
                      consts
                         None
                      names      ('print',)
                      varnames   ()
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                      name       'handle_response_complete'
-                     firstlineno 47
+                     firstlineno 43
                      lnotab 0x0201
                names      ('re', 'match', 'group', 'simple_llm', 'stream_inference')
                varnames   ('self', 'user_input', 'match', 'prompt', 'handle_text_received', 'handle_response_complete')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_chat_request'
-               firstlineno 40
+               firstlineno 36
                lnotab 0x02012a01320206030603
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab010000000000000000010064005300
-                53           0 RESUME                   0
+                49           0 RESUME                   0
                
-                54           2 LOAD_FAST                0 (self)
+                50           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (shell_command_service)
                             14 LOAD_METHOD              1 (handle_prompt)
                             36 LOAD_FAST                1 (user_input)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
@@ -488,27 +457,27 @@
                   None
                names      ('shell_command_service', 'handle_prompt')
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_shell_nli_request'
-               firstlineno 53
+               firstlineno 49
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab000000000000000000010064005300
-                56           0 RESUME                   0
+                52           0 RESUME                   0
                
-                57           2 LOAD_FAST                0 (self)
+                53           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user_config_service)
                             14 LOAD_METHOD              1 (prompt_for_all_configs)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 POP_TOP
                             52 LOAD_CONST               0 (None)
                             54 RETURN_VALUE
@@ -516,25 +485,25 @@
                   None
                names      ('user_config_service', 'prompt_for_all_configs')
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_config_request'
-               firstlineno 56
+               firstlineno 52
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'str', 'handle_request', 'handle_help_request', 'handle_chat_request', 'handle_shell_nli_request', 'handle_config_request')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
          name       'UserCommandService'
          firstlineno 12
-         lnotab 0x0a0106090c0a0608060d0603
+         lnotab 0x0a0106090c0a0604060d0603
       'UserCommandService'
    names      ('re', 'eras.agents.simple_llm', 'SimpleLLM', 'eras.config.config', 'config', 'eras.services.shell_command_service', 'ShellCommandService', 'openai', 'eras.services.user_config_service', 'UserConfigService', 'httpx', 'UserCommandService')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
    name       '<module>'
```

### Comparing `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.4.3/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.4.3/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/llm_callable_functions/user_details.py` & `eras-0.4.3/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/shell_command_service.py` & `eras-0.4.3/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/services/user_command_service.py` & `eras-0.4.3/eras/services/user_command_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,20 +26,16 @@
             self.handle_chat_request(user_input)
         elif user_input.startswith("/config"):
             self.handle_config_request(user_input)
         else:
             self.handle_shell_nli_request(user_input)
 
     def handle_help_request(self, user_input):
-        print("Welcome to ERAS - Easily Runnable AI Shell")
-        print("Commands: ==============================================")
-        print("{defualt usage} - Natural Languge Interface for running commands. e.g. eras how do I list all files in a directory -> %ls")
-        print("/help - get info about commands")
-        print("/chat - ask the LLM a question about anything. e.g. /chat tell me about quantum physics")
-        print("/conf - configure eras. urls, keys, etc")
+        self.user_config_service.print_eras_logo()
+        self.user_config_service.show_commands()
 
     def handle_chat_request(self, user_input):
         match = re.match(r'^/chat\s+(.*)', user_input)
         prompt = match.group(1) if match else None
 
         def handle_text_received(text):
             print(text, end="")
```

### Comparing `eras-0.4.2/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc` & `eras-0.4.3/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras/utils/env_vars_and_profile_files.py` & `eras-0.4.3/eras/utils/env_vars_and_profile_files.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/eras.egg-info/PKG-INFO` & `eras-0.4.3/eras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.2
+Version: 0.4.3
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.4.2/eras.egg-info/SOURCES.txt` & `eras-0.4.3/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.4.2/setup.py` & `eras-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eras',
-    version='0.4.2',
+    version='0.4.3',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

