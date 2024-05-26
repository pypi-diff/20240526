# Comparing `tmp/eras-0.4.4.tar.gz` & `tmp/eras-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.4.4.tar", last modified: Sun May 26 03:42:23 2024, max compression
+gzip compressed data, was "eras-0.4.5.tar", last modified: Sun May 26 03:46:36 2024, max compression
```

## Comparing `eras-0.4.4.tar` & `eras-0.4.5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.620652 eras-0.4.4/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.4/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.4/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 03:42:23.620216 eras-0.4.4/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.4/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.589841 eras-0.4.4/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.4/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.592140 eras-0.4.4/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.4/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.4/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.4/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.593575 eras-0.4.4/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.4/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.596521 eras-0.4.4/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.4/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.4/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.4/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.4/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.4/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.4/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.4/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.4/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.597464 eras-0.4.4/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.4/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.598694 eras-0.4.4/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.4/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.4/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.4/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.4/eras/config/config.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.599395 eras-0.4.4/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.4/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.600187 eras-0.4.4/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.4/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.601228 eras-0.4.4/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.4/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.603018 eras-0.4.4/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.4/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.4/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.4/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.4/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.4/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.4/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.605146 eras-0.4.4/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.4/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.609429 eras-0.4.4/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.4/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.4/eras/models/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.4/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.4/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.4/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.4/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.4/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.4/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.4/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.4/eras/models/constants.py
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.4/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.4/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.4/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.4/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.4/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.4/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.611600 eras-0.4.4/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.4/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.614412 eras-0.4.4/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.4/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.4/eras/services/__pycache__/user_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7597 2024-05-26 03:41:31.000000 eras-0.4.4/eras/services/__pycache__/user_config_service.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.616264 eras-0.4.4/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.4/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.618352 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.4/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.4/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.4/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.4/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.4/eras/services/user_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)    10414 2024-05-26 03:41:58.000000 eras-0.4.4/eras/services/user_config_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.618951 eras-0.4.4/eras/utils/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.4/eras/utils/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.619592 eras-0.4.4/eras/utils/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.4/eras/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.4/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.4/eras/utils/env_vars_and_profile_files.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.591364 eras-0.4.4/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       86 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 03:42:23.620755 eras-0.4.4/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1066 2024-05-26 03:42:14.000000 eras-0.4.4/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.655073 eras-0.4.5/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.5/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.5/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     4904 2024-05-26 03:46:36.654518 eras-0.4.5/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.5/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.623187 eras-0.4.5/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.5/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.626584 eras-0.4.5/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.5/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.5/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.5/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.628878 eras-0.4.5/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.5/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.631694 eras-0.4.5/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.5/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.5/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.5/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.5/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.5/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.5/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.5/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.5/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.5/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.5/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.5/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.5/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.5/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.632261 eras-0.4.5/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.5/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.633554 eras-0.4.5/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.5/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.5/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.5/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.5/eras/config/config.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.634262 eras-0.4.5/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.5/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.635305 eras-0.4.5/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.5/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.636757 eras-0.4.5/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.5/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.639034 eras-0.4.5/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.5/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.5/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.5/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.5/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.5/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.5/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.5/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.5/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.641916 eras-0.4.5/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.5/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.645757 eras-0.4.5/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.5/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.5/eras/models/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.5/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.5/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.5/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.5/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.5/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.5/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.5/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.5/eras/models/constants.py
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.5/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.5/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.5/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.5/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.5/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.5/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.647103 eras-0.4.5/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.5/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.649213 eras-0.4.5/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.5/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.5/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.5/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.5/eras/services/__pycache__/user_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7795 2024-05-26 03:46:21.000000 eras-0.4.5/eras/services/__pycache__/user_config_service.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.650674 eras-0.4.5/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.5/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.652447 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.5/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.5/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.5/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.5/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.5/eras/services/user_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)    10761 2024-05-26 03:46:18.000000 eras-0.4.5/eras/services/user_config_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.653134 eras-0.4.5/eras/utils/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.5/eras/utils/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.653854 eras-0.4.5/eras/utils/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.5/eras/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.5/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.5/eras/utils/env_vars_and_profile_files.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:46:36.625510 eras-0.4.5/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     4904 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)      102 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 03:46:36.000000 eras-0.4.5/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 03:46:36.655175 eras-0.4.5/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1093 2024-05-26 03:46:30.000000 eras-0.4.5/setup.py
```

### Comparing `eras-0.4.4/PKG-INFO` & `eras-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.4
+Version: 0.4.5
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: InquirerPy==0.3.4
+Requires-Dist: colorama==0.4.6
 
 # ERAS
 Easily Runnable AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
 Eras works on Windows, Mac, and Linux!
```

### Comparing `eras-0.4.4/README.md` & `eras-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/__pycache__/main.cpython-311.pyc` & `eras-0.4.5/eras/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.4.5/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.4.5/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.4.5/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.4.5/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.4.5/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.4.5/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.4.5/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/llama_functions_agent.py` & `eras-0.4.5/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.4.5/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/llm_functions_agent.py` & `eras-0.4.5/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/simple_llm.py` & `eras-0.4.5/eras/agents/simple_llm.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/agents/terminal_llama_agent.py` & `eras-0.4.5/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.4.5/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.4.5/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/config/config.py` & `eras-0.4.5/eras/config/config.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.4.5/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/decorators/chatgpt_tool_data.py` & `eras-0.4.5/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.4.5/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.4.5/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.4.5/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.4.5/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/factories/function_details_factory.py` & `eras-0.4.5/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/factories/message_factory.py` & `eras-0.4.5/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/main.py` & `eras-0.4.5/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.4.5/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.4.5/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.4.5/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.4.5/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.4.5/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.4.5/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/conversation.py` & `eras-0.4.5/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/function_details.py` & `eras-0.4.5/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/message.py` & `eras-0.4.5/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/models/transaction.py` & `eras-0.4.5/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/run.ipynb` & `eras-0.4.5/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.4.5/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.4.5/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.4.5/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/__pycache__/user_config_service.cpython-311.pyc` & `eras-0.4.5/eras/services/__pycache__/user_config_service.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,22 @@
 magic:    0xa70d0d0a
-moddate:  0x68af5266 (Sun May 26 03:41:28 2024 UTC)
-files sz: 11092
+moddate:  0x8ab05266 (Sun May 26 03:46:18 2024 UTC)
+files sz: 10761
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c045a04640064036c055a05640064046c066d075a076d085a086d095a
       096d0a5a0a0100640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f01
-      00640064066c106d115a110100640064036c125a12640064036c135a1302
-      004700640784006408a6020000ab0200000000000000005a1464035300
+      00640064066c106d115a110100640064036c125a12640064036c135a1364
+      0064076c146d155a156d165a166d175a17010002004700640884006409a6
+      020000ab0200000000000000005a1864035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('prompt',))
                  6 IMPORT_NAME              0 (InquirerPy)
                  8 IMPORT_FROM              1 (prompt)
                 10 STORE_NAME               1 (prompt)
@@ -77,32 +78,44 @@
                108 STORE_NAME              18 (textwrap)
    
      9         110 LOAD_CONST               0 (0)
                112 LOAD_CONST               3 (None)
                114 IMPORT_NAME             19 (platform)
                116 STORE_NAME              19 (platform)
    
-    11         118 PUSH_NULL
-               120 LOAD_BUILD_CLASS
-               122 LOAD_CONST               7 (<code object UserConfigService, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 11>)
-               124 MAKE_FUNCTION            0
-               126 LOAD_CONST               8 ('UserConfigService')
-               128 PRECALL                  2
-               132 CALL                     2
-               142 STORE_NAME              20 (UserConfigService)
-               144 LOAD_CONST               3 (None)
-               146 RETURN_VALUE
+    10         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               7 (('init', 'Fore', 'Style'))
+               122 IMPORT_NAME             20 (colorama)
+               124 IMPORT_FROM             21 (init)
+               126 STORE_NAME              21 (init)
+               128 IMPORT_FROM             22 (Fore)
+               130 STORE_NAME              22 (Fore)
+               132 IMPORT_FROM             23 (Style)
+               134 STORE_NAME              23 (Style)
+               136 POP_TOP
+   
+    11         138 PUSH_NULL
+               140 LOAD_BUILD_CLASS
+               142 LOAD_CONST               8 (<code object UserConfigService, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 11>)
+               144 MAKE_FUNCTION            0
+               146 LOAD_CONST               9 ('UserConfigService')
+               148 PRECALL                  2
+               152 CALL                     2
+               162 STORE_NAME              24 (UserConfigService)
+               164 LOAD_CONST               3 (None)
+               166 RETURN_VALUE
    consts
       0
       ('prompt',)
       ('Choice',)
       None
       ('env_var_exists', 'reload_profile', 'get_profile_file', 'set_env_var')
       ('ERAS_OPENAI_KEY_ENV_VAR_NAME', 'ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME', 'ERAS_MODEL_ENV_VAR_NAME', 'ERAS_BASE_URL_ENV_VAR_NAME')
       ('config',)
+      ('init', 'Fore', 'Style')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640184005a036408640384015a04640484005a
@@ -547,173 +560,172 @@
                lnotab 0x02013001040124022a011e011e011e011e011e011e01
             code
                argcount  : 1
                nlocals   : 10
                stacksize : 8
                flags     : 3
                code
-                  0x870a97007400000000000000000000006a01000000000000000064016b
-                  0300000000720767006402a2017d0164037d026e0667006402a2017d0164
-                  037d0267006404a2017d03640584007c034400a6000000ab000000000000
-                  0000007d04740500000000000000000000640684007c044400a6000000ab
-                  000000000000000000a6010000ab0100000000000000008a0a880a660164
-                  0784087c044400a6000000ab0000000000000000007d0564087d06740700
-                  000000000000000000890aa6010000ab01000000000000000044005d5e7d
-                  077409000000000000000000007c05a6010000ab01000000000000000044
-                  005d475c0200007d087d097c067c017c08740b000000000000000000007c
-                  01a6010000ab0100000000000000007a060000190000000000000000007c
-                  097c07190000000000000000007a0000007c027a0000007a0d00007d067c
-                  08740b000000000000000000007c05a6010000ab01000000000000000064
-                  097a0a00006b000000000072057c06640a7a0d00007d068c487c06640b7a
-                  0d00007d068c5f740d000000000000000000007c06a6010000ab01000000
-                  0000000000010064005300
+                  0x870a97007400000000000000000000006a010000000000000000740000
+                  0000000000000000006a0200000000000000007400000000000000000000
+                  006a0300000000000000007400000000000000000000006a040000000000
+                  0000007400000000000000000000006a05000000000000000067057d0174
+                  0c000000000000000000006a0700000000000000007d0267006401a2017d
+                  03640284007c034400a6000000ab0000000000000000007d047411000000
+                  00000000000000640384007c044400a6000000ab000000000000000000a6
+                  010000ab0100000000000000008a0a880a6601640484087c044400a60000
+                  00ab0000000000000000007d0564057d0674130000000000000000000089
+                  0aa6010000ab01000000000000000044005d5e7d07741500000000000000
+                  0000007c05a6010000ab01000000000000000044005d475c0200007d087d
+                  097c067c017c087417000000000000000000007c01a6010000ab01000000
+                  00000000007a060000190000000000000000007c097c0719000000000000
+                  0000007a0000007c027a0000007a0d00007d067c08741700000000000000
+                  0000007c05a6010000ab01000000000000000064067a0a00006b00000000
+                  0072057c0664077a0d00007d068c487c0664087a0d00007d068c5f741900
+                  0000000000000000007c06a6010000ab0100000000000000000100640053
+                  00
                              0 MAKE_CELL               10 (max_lines)
                
                 74           2 RESUME                   0
                
-                77           4 LOAD_GLOBAL              0 (os)
-                            16 LOAD_ATTR                1 (name)
-                            26 LOAD_CONST               1 ('nt')
-                            28 COMPARE_OP               3 (!=)
-                            34 POP_JUMP_FORWARD_IF_FALSE     7 (to 50)
-               
-                78          36 BUILD_LIST               0
-                            38 LOAD_CONST               2 (('\x1b[94m', '\x1b[96m', '\x1b[91m', '\x1b[93m', '\x1b[95m'))
-                            40 LIST_EXTEND              1
-                            42 STORE_FAST               1 (colors)
-               
-                85          44 LOAD_CONST               3 ('\x1b[0m')
-                            46 STORE_FAST               2 (RESET)
-                            48 JUMP_FORWARD             6 (to 62)
-               
-                94     >>   50 BUILD_LIST               0
-                            52 LOAD_CONST               2 (('\x1b[94m', '\x1b[96m', '\x1b[91m', '\x1b[93m', '\x1b[95m'))
-                            54 LIST_EXTEND              1
-                            56 STORE_FAST               1 (colors)
-               
-               101          58 LOAD_CONST               3 ('\x1b[0m')
-                            60 STORE_FAST               2 (RESET)
-               
-               103     >>   62 BUILD_LIST               0
-                            64 LOAD_CONST               4 (('\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\:\\~\\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\ \\/__/  \n    \\:\\__\\    \n     \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/_|::\\/:/  /\n    |:|::/  / \n    |:|\\/__/  \n    |:|  |    \n    \\|__|     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/__\\:\\/:/  /\n      \\::/  / \n      /:/  /  \n     /:/  /   \n    \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\ \\  \\  \n  _\\:\\~\\ \\  \\ \n /\\ \\:\\ \\ \\__\\\n \\:\\ \\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\/:/  /  \n    \\::/  /   \n    \\/__/    \n            '))
-                            66 LIST_EXTEND              1
-                            68 STORE_FAST               3 (text_blocks)
-               
-               159          70 LOAD_CONST               5 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 159>)
-                            72 MAKE_FUNCTION            0
-                            74 LOAD_FAST                3 (text_blocks)
-                            76 GET_ITER
-                            78 PRECALL                  0
-                            82 CALL                     0
-                            92 STORE_FAST               4 (lines)
-               
-               160          94 LOAD_GLOBAL              5 (NULL + max)
-                           106 LOAD_CONST               6 (<code object <genexpr>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 160>)
-                           108 MAKE_FUNCTION            0
-                           110 LOAD_FAST                4 (lines)
-                           112 GET_ITER
-                           114 PRECALL                  0
-                           118 CALL                     0
-                           128 PRECALL                  1
-                           132 CALL                     1
-                           142 STORE_DEREF             10 (max_lines)
-               
-               161         144 LOAD_CLOSURE            10 (max_lines)
-                           146 BUILD_TUPLE              1
-                           148 LOAD_CONST               7 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 161>)
-                           150 MAKE_FUNCTION            8 (closure)
-                           152 LOAD_FAST                4 (lines)
-                           154 GET_ITER
-                           156 PRECALL                  0
-                           160 CALL                     0
-                           170 STORE_FAST               5 (padded_blocks)
-               
-               163         172 LOAD_CONST               8 ('')
-                           174 STORE_FAST               6 (colored_output)
-               
-               165         176 LOAD_GLOBAL              7 (NULL + range)
-                           188 LOAD_DEREF              10 (max_lines)
-                           190 PRECALL                  1
-                           194 CALL                     1
-                           204 GET_ITER
-                       >>  206 FOR_ITER                94 (to 396)
-                           208 STORE_FAST               7 (i)
-               
-               166         210 LOAD_GLOBAL              9 (NULL + enumerate)
-                           222 LOAD_FAST                5 (padded_blocks)
-                           224 PRECALL                  1
-                           228 CALL                     1
-                           238 GET_ITER
-                       >>  240 FOR_ITER                71 (to 384)
-                           242 UNPACK_SEQUENCE          2
-                           246 STORE_FAST               8 (j)
-                           248 STORE_FAST               9 (block)
-               
-               167         250 LOAD_FAST                6 (colored_output)
-                           252 LOAD_FAST                1 (colors)
-                           254 LOAD_FAST                8 (j)
-                           256 LOAD_GLOBAL             11 (NULL + len)
-                           268 LOAD_FAST                1 (colors)
+                86           4 LOAD_GLOBAL              0 (Fore)
+                            16 LOAD_ATTR                1 (LIGHTCYAN_EX)
+               
+                87          26 LOAD_GLOBAL              0 (Fore)
+                            38 LOAD_ATTR                2 (LIGHTBLUE_EX)
+               
+                88          48 LOAD_GLOBAL              0 (Fore)
+                            60 LOAD_ATTR                3 (LIGHTRED_EX)
+               
+                89          70 LOAD_GLOBAL              0 (Fore)
+                            82 LOAD_ATTR                4 (LIGHTYELLOW_EX)
+               
+                90          92 LOAD_GLOBAL              0 (Fore)
+                           104 LOAD_ATTR                5 (LIGHTMAGENTA_EX)
+               
+                85         114 BUILD_LIST               5
+                           116 STORE_FAST               1 (colors)
+               
+                92         118 LOAD_GLOBAL             12 (Style)
+                           130 LOAD_ATTR                7 (RESET_ALL)
+                           140 STORE_FAST               2 (RESET)
+               
+                94         142 BUILD_LIST               0
+                           144 LOAD_CONST               1 (('\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\:\\~\\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\ \\/__/  \n    \\:\\__\\    \n     \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/_|::\\/:/  /\n    |:|::/  / \n    |:|\\/__/  \n    |:|  |    \n    \\|__|     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/__\\:\\/:/  /\n      \\::/  / \n      /:/  /  \n     /:/  /   \n    \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\ \\  \\  \n  _\\:\\~\\ \\  \\ \n /\\ \\:\\ \\ \\__\\\n \\:\\ \\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\/:/  /  \n    \\::/  /   \n    \\/__/    \n            '))
+                           146 LIST_EXTEND              1
+                           148 STORE_FAST               3 (text_blocks)
+               
+               150         150 LOAD_CONST               2 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 150>)
+                           152 MAKE_FUNCTION            0
+                           154 LOAD_FAST                3 (text_blocks)
+                           156 GET_ITER
+                           158 PRECALL                  0
+                           162 CALL                     0
+                           172 STORE_FAST               4 (lines)
+               
+               151         174 LOAD_GLOBAL             17 (NULL + max)
+                           186 LOAD_CONST               3 (<code object <genexpr>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 151>)
+                           188 MAKE_FUNCTION            0
+                           190 LOAD_FAST                4 (lines)
+                           192 GET_ITER
+                           194 PRECALL                  0
+                           198 CALL                     0
+                           208 PRECALL                  1
+                           212 CALL                     1
+                           222 STORE_DEREF             10 (max_lines)
+               
+               152         224 LOAD_CLOSURE            10 (max_lines)
+                           226 BUILD_TUPLE              1
+                           228 LOAD_CONST               4 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 152>)
+                           230 MAKE_FUNCTION            8 (closure)
+                           232 LOAD_FAST                4 (lines)
+                           234 GET_ITER
+                           236 PRECALL                  0
+                           240 CALL                     0
+                           250 STORE_FAST               5 (padded_blocks)
+               
+               154         252 LOAD_CONST               5 ('')
+                           254 STORE_FAST               6 (colored_output)
+               
+               156         256 LOAD_GLOBAL             19 (NULL + range)
+                           268 LOAD_DEREF              10 (max_lines)
                            270 PRECALL                  1
                            274 CALL                     1
-                           284 BINARY_OP                6 (%)
-                           288 BINARY_SUBSCR
-                           298 LOAD_FAST                9 (block)
-                           300 LOAD_FAST                7 (i)
-                           302 BINARY_SUBSCR
-                           312 BINARY_OP                0 (+)
-                           316 LOAD_FAST                2 (RESET)
-                           318 BINARY_OP                0 (+)
-                           322 BINARY_OP               13 (+=)
-                           326 STORE_FAST               6 (colored_output)
-               
-               168         328 LOAD_FAST                8 (j)
-                           330 LOAD_GLOBAL             11 (NULL + len)
-                           342 LOAD_FAST                5 (padded_blocks)
-                           344 PRECALL                  1
-                           348 CALL                     1
-                           358 LOAD_CONST               9 (1)
-                           360 BINARY_OP               10 (-)
-                           364 COMPARE_OP               0 (<)
-                           370 POP_JUMP_FORWARD_IF_FALSE     5 (to 382)
-               
-               169         372 LOAD_FAST                6 (colored_output)
-                           374 LOAD_CONST              10 (' ')
-                           376 BINARY_OP               13 (+=)
-                           380 STORE_FAST               6 (colored_output)
-                       >>  382 JUMP_BACKWARD           72 (to 240)
-               
-               170     >>  384 LOAD_FAST                6 (colored_output)
-                           386 LOAD_CONST              11 ('\n')
-                           388 BINARY_OP               13 (+=)
-                           392 STORE_FAST               6 (colored_output)
-                           394 JUMP_BACKWARD           95 (to 206)
-               
-               172     >>  396 LOAD_GLOBAL             13 (NULL + print)
-                           408 LOAD_FAST                6 (colored_output)
-                           410 PRECALL                  1
-                           414 CALL                     1
-                           424 POP_TOP
-                           426 LOAD_CONST               0 (None)
-                           428 RETURN_VALUE
+                           284 GET_ITER
+                       >>  286 FOR_ITER                94 (to 476)
+                           288 STORE_FAST               7 (i)
+               
+               157         290 LOAD_GLOBAL             21 (NULL + enumerate)
+                           302 LOAD_FAST                5 (padded_blocks)
+                           304 PRECALL                  1
+                           308 CALL                     1
+                           318 GET_ITER
+                       >>  320 FOR_ITER                71 (to 464)
+                           322 UNPACK_SEQUENCE          2
+                           326 STORE_FAST               8 (j)
+                           328 STORE_FAST               9 (block)
+               
+               158         330 LOAD_FAST                6 (colored_output)
+                           332 LOAD_FAST                1 (colors)
+                           334 LOAD_FAST                8 (j)
+                           336 LOAD_GLOBAL             23 (NULL + len)
+                           348 LOAD_FAST                1 (colors)
+                           350 PRECALL                  1
+                           354 CALL                     1
+                           364 BINARY_OP                6 (%)
+                           368 BINARY_SUBSCR
+                           378 LOAD_FAST                9 (block)
+                           380 LOAD_FAST                7 (i)
+                           382 BINARY_SUBSCR
+                           392 BINARY_OP                0 (+)
+                           396 LOAD_FAST                2 (RESET)
+                           398 BINARY_OP                0 (+)
+                           402 BINARY_OP               13 (+=)
+                           406 STORE_FAST               6 (colored_output)
+               
+               159         408 LOAD_FAST                8 (j)
+                           410 LOAD_GLOBAL             23 (NULL + len)
+                           422 LOAD_FAST                5 (padded_blocks)
+                           424 PRECALL                  1
+                           428 CALL                     1
+                           438 LOAD_CONST               6 (1)
+                           440 BINARY_OP               10 (-)
+                           444 COMPARE_OP               0 (<)
+                           450 POP_JUMP_FORWARD_IF_FALSE     5 (to 462)
+               
+               160         452 LOAD_FAST                6 (colored_output)
+                           454 LOAD_CONST               7 (' ')
+                           456 BINARY_OP               13 (+=)
+                           460 STORE_FAST               6 (colored_output)
+                       >>  462 JUMP_BACKWARD           72 (to 320)
+               
+               161     >>  464 LOAD_FAST                6 (colored_output)
+                           466 LOAD_CONST               8 ('\n')
+                           468 BINARY_OP               13 (+=)
+                           472 STORE_FAST               6 (colored_output)
+                           474 JUMP_BACKWARD           95 (to 286)
+               
+               163     >>  476 LOAD_GLOBAL             25 (NULL + print)
+                           488 LOAD_FAST                6 (colored_output)
+                           490 PRECALL                  1
+                           494 CALL                     1
+                           504 POP_TOP
+                           506 LOAD_CONST               0 (None)
+                           508 RETURN_VALUE
                consts
                   None
-                  'nt'
-                  ('\x1b[94m', '\x1b[96m', '\x1b[91m', '\x1b[93m', '\x1b[95m')
-                  '\x1b[0m'
                   ('\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\:\\~\\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\ \\/__/  \n    \\:\\__\\    \n     \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/_|::\\/:/  /\n    |:|::/  / \n    |:|\\/__/  \n    |:|  |    \n    \\|__|     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/__\\:\\/:/  /\n      \\::/  / \n      /:/  /  \n     /:/  /   \n    \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\ \\  \\  \n  _\\:\\~\\ \\  \\ \n /\\ \\:\\ \\ \\__\\\n \\:\\ \\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\/:/  /  \n    \\::/  /   \n    \\/__/    \n            ')
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d177d017c01a000000000000000000000000000000000
                         00000000006400a6010000ab01000000000000000091028c185300
-                     159           0 RESUME                   0
+                     150           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                23 (to 54)
                                    8 STORE_FAST               1 (block)
                                   10 LOAD_FAST                1 (block)
                                   12 LOAD_METHOD              0 (split)
                                   34 LOAD_CONST               0 ('\n')
@@ -726,25 +738,25 @@
                         '\n'
                      names      ('split',)
                      varnames   ('.0', 'block')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                      name       '<listcomp>'
-                     firstlineno 159
+                     firstlineno 150
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d137d017401000000000000000000007c01a60100
                         00ab0100000000000000005600970101008c1464005300
-                     160           0 RETURN_GENERATOR
+                     151           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                19 (to 48)
                                   10 STORE_FAST               1 (block)
                                   12 LOAD_GLOBAL              1 (NULL + len)
                                   24 LOAD_FAST                1 (block)
@@ -760,28 +772,28 @@
                         None
                      names      ('len',)
                      varnames   ('.0', 'block')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                      name       '<genexpr>'
-                     firstlineno 160
+                     firstlineno 151
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 8
                      flags     : 19
                      code
                         0x9501970067007c005d1b7d017c01640067018902740100000000000000
                         0000007c01a6010000ab0100000000000000007a0a00007a0500007a0000
                         0091028c1c5300
                                    0 COPY_FREE_VARS           1
                      
-                     161           2 RESUME                   0
+                     152           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                27 (to 64)
                                   10 STORE_FAST               1 (block)
                                   12 LOAD_FAST                1 (block)
                                   14 LOAD_CONST               0 ('')
                                   16 BUILD_LIST               1
@@ -800,42 +812,42 @@
                         ''
                      names      ('len',)
                      varnames   ('.0', 'block')
                      freevars   ('max_lines',)
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                      name       '<listcomp>'
-                     firstlineno 161
+                     firstlineno 152
                      lnotab 0x
                   ''
                   1
                   ' '
                   '\n'
-               names      ('os', 'name', 'max', 'range', 'enumerate', 'len', 'print')
+               names      ('Fore', 'LIGHTCYAN_EX', 'LIGHTBLUE_EX', 'LIGHTRED_EX', 'LIGHTYELLOW_EX', 'LIGHTMAGENTA_EX', 'Style', 'RESET_ALL', 'max', 'range', 'enumerate', 'len', 'print')
                varnames   ('self', 'colors', 'RESET', 'text_blocks', 'lines', 'padded_blocks', 'colored_output', 'i', 'j', 'block')
                freevars   ()
                cellvars   ('max_lines',)
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                name       'print_eras_logo'
                firstlineno 74
                lnotab
-                  0x0403200108070609080704020838180132011c020402220128014e012c
-                  010c010c02
+                  0x040c160116011601160116fb040718020838180132011c020402220128
+                  014e012c010c010c02
             None
             (True,)
          names      ('__name__', '__module__', '__qualname__', 'ensure_needed_configs_are_set', 'prompt_for_all_configs', 'reload_prof', 'show_commands', 'print_eras_logo')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
          name       'UserConfigService'
          firstlineno 11
          lnotab 0x0a040606081f0608060e
       'UserConfigService'
-   names      ('InquirerPy', 'prompt', 'InquirerPy.base.control', 'Choice', 'os', 'sys', 'eras.utils.env_vars_and_profile_files', 'env_var_exists', 'reload_profile', 'get_profile_file', 'set_env_var', 'eras.models.constants', 'ERAS_OPENAI_KEY_ENV_VAR_NAME', 'ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME', 'ERAS_MODEL_ENV_VAR_NAME', 'ERAS_BASE_URL_ENV_VAR_NAME', 'eras.config.config', 'config', 'textwrap', 'platform', 'UserConfigService')
+   names      ('InquirerPy', 'prompt', 'InquirerPy.base.control', 'Choice', 'os', 'sys', 'eras.utils.env_vars_and_profile_files', 'env_var_exists', 'reload_profile', 'get_profile_file', 'set_env_var', 'eras.models.constants', 'ERAS_OPENAI_KEY_ENV_VAR_NAME', 'ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME', 'ERAS_MODEL_ENV_VAR_NAME', 'ERAS_BASE_URL_ENV_VAR_NAME', 'eras.config.config', 'config', 'textwrap', 'platform', 'colorama', 'init', 'Fore', 'Style', 'UserConfigService')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0108010801180118010c0108010802
+   lnotab 0x00ff02010c010c0108010801180118010c01080108011401
```

### Comparing `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.4.5/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.4.5/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.4.5/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/llm_callable_functions/user_details.py` & `eras-0.4.5/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/shell_command_service.py` & `eras-0.4.5/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/user_command_service.py` & `eras-0.4.5/eras/services/user_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/services/user_config_service.py` & `eras-0.4.5/eras/services/user_config_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import sys
 from eras.utils.env_vars_and_profile_files import env_var_exists, reload_profile, get_profile_file, set_env_var
 from eras.models.constants import ERAS_OPENAI_KEY_ENV_VAR_NAME, ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME, ERAS_MODEL_ENV_VAR_NAME, ERAS_BASE_URL_ENV_VAR_NAME
 from eras.config.config import config
 import textwrap
 import platform
-
+from colorama import init, Fore, Style
 class UserConfigService:
     # def __init__(self):
     #     print('init')
 
     def ensure_needed_configs_are_set(self):
         if not env_var_exists(ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME):
             self.prompt_for_all_configs(should_reload_profile=False)
@@ -70,22 +70,30 @@
         print("/conf - configure eras. urls, keys, etc")
         print("")
         print("=" * terminal_width)
 
     def print_eras_logo(self):
         # Define ANSI escape codes for 256-color mode with given RGB colors
 
+        # colors = [
+        #     "\033[94m",  # Bright blue
+        #     "\033[96m",  # Bright cyan
+        #     "\033[91m",  # Bright red
+        #     "\033[93m",  # Bright yellow
+        #     "\033[95m"  # Bright magenta
+        # ]
+        # RESET = "\033[0m"
         colors = [
-            "\033[94m",  # Bright blue
-            "\033[96m",  # Bright cyan
-            "\033[91m",  # Bright red
-            "\033[93m",  # Bright yellow
-            "\033[95m"  # Bright magenta
+            Fore.LIGHTCYAN_EX,  # Light cyan
+            Fore.LIGHTBLUE_EX,  # Light blue
+            Fore.LIGHTRED_EX,  # Light red
+            Fore.LIGHTYELLOW_EX,  # Light yellow
+            Fore.LIGHTMAGENTA_EX  # Light magenta
         ]
-        RESET = "\033[0m"
+        RESET = Style.RESET_ALL
 
         text_blocks = [
             r"""
       ___     
      /\  \    
     /::\  \   
    /:/\:\  \
```

### Comparing `eras-0.4.4/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc` & `eras-0.4.5/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras/utils/env_vars_and_profile_files.py` & `eras-0.4.5/eras/utils/env_vars_and_profile_files.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.4/eras.egg-info/PKG-INFO` & `eras-0.4.5/eras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.4
+Version: 0.4.5
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: InquirerPy==0.3.4
+Requires-Dist: colorama==0.4.6
 
 # ERAS
 Easily Runnable AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
 Eras works on Windows, Mac, and Linux!
```

### Comparing `eras-0.4.4/eras.egg-info/SOURCES.txt` & `eras-0.4.5/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

