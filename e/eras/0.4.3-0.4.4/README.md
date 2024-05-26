# Comparing `tmp/eras-0.4.3.tar.gz` & `tmp/eras-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.4.3.tar", last modified: Sun May 26 03:35:08 2024, max compression
+gzip compressed data, was "eras-0.4.4.tar", last modified: Sun May 26 03:42:23 2024, max compression
```

## Comparing `eras-0.4.3.tar` & `eras-0.4.4.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.752804 eras-0.4.3/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.3/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.3/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 03:35:08.752285 eras-0.4.3/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.3/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.720673 eras-0.4.3/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.3/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.723967 eras-0.4.3/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.3/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.3/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.3/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.726215 eras-0.4.3/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.3/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.729352 eras-0.4.3/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.3/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.3/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.3/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.3/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.3/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.3/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.3/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.3/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.3/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.3/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.3/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.3/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.3/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.729909 eras-0.4.3/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.3/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.731112 eras-0.4.3/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.3/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.3/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.3/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.3/eras/config/config.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.731830 eras-0.4.3/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.3/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.732623 eras-0.4.3/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.3/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.733697 eras-0.4.3/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.3/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.735485 eras-0.4.3/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.3/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.3/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.3/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.3/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.3/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.3/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.3/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.3/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.738327 eras-0.4.3/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.3/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.742588 eras-0.4.3/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.3/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.3/eras/models/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.3/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.3/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.3/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.3/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.3/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.3/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.3/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.3/eras/models/constants.py
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.3/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.3/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.3/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.3/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.3/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.3/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.743859 eras-0.4.3/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.3/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.745222 eras-0.4.3/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.3/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.3/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.3/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.3/eras/services/__pycache__/user_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7514 2024-05-26 03:32:31.000000 eras-0.4.3/eras/services/__pycache__/user_config_service.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.747018 eras-0.4.3/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.3/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.749529 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.3/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.3/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.3/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.3/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.3/eras/services/user_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)    10421 2024-05-26 03:32:28.000000 eras-0.4.3/eras/services/user_config_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.750735 eras-0.4.3/eras/utils/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.3/eras/utils/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.751543 eras-0.4.3/eras/utils/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.3/eras/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.3/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.3/eras/utils/env_vars_and_profile_files.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:35:08.723039 eras-0.4.3/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       86 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 03:35:08.000000 eras-0.4.3/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 03:35:08.752913 eras-0.4.3/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1066 2024-05-26 03:35:03.000000 eras-0.4.3/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.620652 eras-0.4.4/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.4/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.4/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 03:42:23.620216 eras-0.4.4/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.4/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.589841 eras-0.4.4/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.4/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.592140 eras-0.4.4/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.4/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.4/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.4/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.593575 eras-0.4.4/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.4/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.596521 eras-0.4.4/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.4/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.4/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.4/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.4/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.4/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.4/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.4/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.4/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.597464 eras-0.4.4/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.4/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.598694 eras-0.4.4/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.4/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.4/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.4/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.4/eras/config/config.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.599395 eras-0.4.4/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.4/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.600187 eras-0.4.4/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.4/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.601228 eras-0.4.4/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.4/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.603018 eras-0.4.4/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.4/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.4/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.4/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.4/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.4/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.4/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.605146 eras-0.4.4/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.4/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.609429 eras-0.4.4/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.4/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.4/eras/models/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.4/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.4/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.4/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.4/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.4/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.4/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.4/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.4/eras/models/constants.py
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.4/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.4/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.4/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.4/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.4/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.4/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.611600 eras-0.4.4/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.4/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.614412 eras-0.4.4/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.4/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4058 2024-05-26 03:24:57.000000 eras-0.4.4/eras/services/__pycache__/user_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7597 2024-05-26 03:41:31.000000 eras-0.4.4/eras/services/__pycache__/user_config_service.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.616264 eras-0.4.4/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.4/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.618352 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.4/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.4/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.4/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.4/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     1805 2024-05-26 03:24:52.000000 eras-0.4.4/eras/services/user_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)    10414 2024-05-26 03:41:58.000000 eras-0.4.4/eras/services/user_config_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.618951 eras-0.4.4/eras/utils/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.4/eras/utils/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.619592 eras-0.4.4/eras/utils/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.4/eras/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.4/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.4/eras/utils/env_vars_and_profile_files.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 03:42:23.591364 eras-0.4.4/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       86 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 03:42:23.000000 eras-0.4.4/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 03:42:23.620755 eras-0.4.4/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1066 2024-05-26 03:42:14.000000 eras-0.4.4/setup.py
```

### Comparing `eras-0.4.3/PKG-INFO` & `eras-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.3
+Version: 0.4.4
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.4.3/README.md` & `eras-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/__pycache__/main.cpython-311.pyc` & `eras-0.4.4/eras/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.4.4/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.4.4/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.4.4/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.4.4/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.4.4/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.4.4/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.4.4/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/llama_functions_agent.py` & `eras-0.4.4/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.4.4/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/llm_functions_agent.py` & `eras-0.4.4/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/simple_llm.py` & `eras-0.4.4/eras/agents/simple_llm.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/agents/terminal_llama_agent.py` & `eras-0.4.4/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.4.4/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.4.4/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/config/config.py` & `eras-0.4.4/eras/config/config.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.4.4/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/decorators/chatgpt_tool_data.py` & `eras-0.4.4/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.4.4/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.4.4/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.4.4/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.4.4/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/factories/function_details_factory.py` & `eras-0.4.4/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/factories/message_factory.py` & `eras-0.4.4/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/main.py` & `eras-0.4.4/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.4.4/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.4.4/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.4.4/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.4.4/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.4.4/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.4.4/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/conversation.py` & `eras-0.4.4/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/function_details.py` & `eras-0.4.4/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/message.py` & `eras-0.4.4/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/models/transaction.py` & `eras-0.4.4/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/run.ipynb` & `eras-0.4.4/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.4.4/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.4.4/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.4.4/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/__pycache__/user_config_service.cpython-311.pyc` & `eras-0.4.4/eras/services/__pycache__/user_config_service.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0x4cad5266 (Sun May 26 03:32:28 2024 UTC)
-files sz: 10421
+moddate:  0x68af5266 (Sun May 26 03:41:28 2024 UTC)
+files sz: 11092
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c045a04640064036c055a05640064046c066d075a076d085a086d095a
       096d0a5a0a0100640064056c0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f01
-      00640064066c106d115a110100640064036c125a12020047006407840064
-      08a6020000ab0200000000000000005a1364035300
+      00640064066c106d115a110100640064036c125a12640064036c135a1302
+      004700640784006408a6020000ab0200000000000000005a1464035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('prompt',))
                  6 IMPORT_NAME              0 (InquirerPy)
                  8 IMPORT_FROM              1 (prompt)
                 10 STORE_NAME               1 (prompt)
@@ -72,24 +72,29 @@
                100 POP_TOP
    
      8         102 LOAD_CONST               0 (0)
                104 LOAD_CONST               3 (None)
                106 IMPORT_NAME             18 (textwrap)
                108 STORE_NAME              18 (textwrap)
    
-    10         110 PUSH_NULL
-               112 LOAD_BUILD_CLASS
-               114 LOAD_CONST               7 (<code object UserConfigService, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 10>)
-               116 MAKE_FUNCTION            0
-               118 LOAD_CONST               8 ('UserConfigService')
-               120 PRECALL                  2
-               124 CALL                     2
-               134 STORE_NAME              19 (UserConfigService)
-               136 LOAD_CONST               3 (None)
-               138 RETURN_VALUE
+     9         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               3 (None)
+               114 IMPORT_NAME             19 (platform)
+               116 STORE_NAME              19 (platform)
+   
+    11         118 PUSH_NULL
+               120 LOAD_BUILD_CLASS
+               122 LOAD_CONST               7 (<code object UserConfigService, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 11>)
+               124 MAKE_FUNCTION            0
+               126 LOAD_CONST               8 ('UserConfigService')
+               128 PRECALL                  2
+               132 CALL                     2
+               142 STORE_NAME              20 (UserConfigService)
+               144 LOAD_CONST               3 (None)
+               146 RETURN_VALUE
    consts
       0
       ('prompt',)
       ('Choice',)
       None
       ('env_var_exists', 'reload_profile', 'get_profile_file', 'set_env_var')
       ('ERAS_OPENAI_KEY_ENV_VAR_NAME', 'ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME', 'ERAS_MODEL_ENV_VAR_NAME', 'ERAS_BASE_URL_ENV_VAR_NAME')
@@ -98,38 +103,38 @@
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640184005a036408640384015a04640484005a
             05640584005a06640684005a0764075300
-          10           0 RESUME                   0
+          11           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('UserConfigService')
                        8 STORE_NAME               2 (__qualname__)
          
-          14          10 LOAD_CONST               1 (<code object ensure_needed_configs_are_set, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 14>)
+          15          10 LOAD_CONST               1 (<code object ensure_needed_configs_are_set, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 15>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (ensure_needed_configs_are_set)
          
-          20          16 LOAD_CONST               8 ((True,))
-                      18 LOAD_CONST               3 (<code object prompt_for_all_configs, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 20>)
+          21          16 LOAD_CONST               8 ((True,))
+                      18 LOAD_CONST               3 (<code object prompt_for_all_configs, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 21>)
                       20 MAKE_FUNCTION            1 (defaults)
                       22 STORE_NAME               4 (prompt_for_all_configs)
          
-          51          24 LOAD_CONST               4 (<code object reload_prof, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 51>)
+          52          24 LOAD_CONST               4 (<code object reload_prof, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 52>)
                       26 MAKE_FUNCTION            0
                       28 STORE_NAME               5 (reload_prof)
          
-          59          30 LOAD_CONST               5 (<code object show_commands, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 59>)
+          60          30 LOAD_CONST               5 (<code object show_commands, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 60>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               6 (show_commands)
          
-          73          36 LOAD_CONST               6 (<code object print_eras_logo, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 73>)
+          74          36 LOAD_CONST               6 (<code object print_eras_logo, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 74>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               7 (print_eras_logo)
                       42 LOAD_CONST               7 (None)
                       44 RETURN_VALUE
          consts
             'UserConfigService'
             code
@@ -140,59 +145,59 @@
                code
                   0x9700740100000000000000000000740200000000000000000000a60100
                   00ab01000000000000000073417c00a00200000000000000000000000000
                   000000000000006401ac02a6010000ab0100000000000000000100740700
                   0000000000000000007402000000000000000000006403a6020000ab0200
                   0000000000000001007c00a0040000000000000000000000000000000000
                   000000a6000000ab00000000000000000001006400530064005300
-                14           0 RESUME                   0
+                15           0 RESUME                   0
                
-                15           2 LOAD_GLOBAL              1 (NULL + env_var_exists)
+                16           2 LOAD_GLOBAL              1 (NULL + env_var_exists)
                             14 LOAD_GLOBAL              2 (ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 POP_JUMP_FORWARD_IF_TRUE    65 (to 172)
                
-                16          42 LOAD_FAST                0 (self)
+                17          42 LOAD_FAST                0 (self)
                             44 LOAD_METHOD              2 (prompt_for_all_configs)
                             66 LOAD_CONST               1 (False)
                             68 KW_NAMES                 2
                             70 PRECALL                  1
                             74 CALL                     1
                             84 POP_TOP
                
-                17          86 LOAD_GLOBAL              7 (NULL + set_env_var)
+                18          86 LOAD_GLOBAL              7 (NULL + set_env_var)
                             98 LOAD_GLOBAL              2 (ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME)
                            110 LOAD_CONST               3 ('true')
                            112 PRECALL                  2
                            116 CALL                     2
                            126 POP_TOP
                
-                18         128 LOAD_FAST                0 (self)
+                19         128 LOAD_FAST                0 (self)
                            130 LOAD_METHOD              4 (reload_prof)
                            152 PRECALL                  0
                            156 CALL                     0
                            166 POP_TOP
                            168 LOAD_CONST               0 (None)
                            170 RETURN_VALUE
                
-                15     >>  172 LOAD_CONST               0 (None)
+                16     >>  172 LOAD_CONST               0 (None)
                            174 RETURN_VALUE
                consts
                   None
                   False
                   ('should_reload_profile',)
                   'true'
                names      ('env_var_exists', 'ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME', 'prompt_for_all_configs', 'set_env_var', 'reload_prof')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                name       'ensure_needed_configs_are_set'
-               firstlineno 14
+               firstlineno 15
                lnotab 0x020128012c012a012cfd
             True
             code
                argcount  : 2
                nlocals   : 13
                stacksize : 5
                flags     : 3
@@ -215,154 +220,154 @@
                   007d0c740f000000000000000000007410000000000000000000007c0ca6
                   020000ab0200000000000000000100740f00000000000000000000741200
                   0000000000000000007c0ba6020000ab0200000000000000000100740f00
                   0000000000000000007414000000000000000000007c0aa6020000ab0200
                   0000000000000001007c0172167c00a00b00000000000000000000000000
                   00000000000000a6000000ab000000000000000000010064005300640053
                   00
-                20           0 RESUME                   0
+                21           0 RESUME                   0
                
-                21           2 LOAD_FAST                0 (self)
+                22           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (print_eras_logo)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                
-                22          42 LOAD_FAST                0 (self)
+                23          42 LOAD_FAST                0 (self)
                             44 LOAD_METHOD              1 (show_commands)
                             66 PRECALL                  0
                             70 CALL                     0
                             80 POP_TOP
                
-                23          82 LOAD_GLOBAL              5 (NULL + config)
+                24          82 LOAD_GLOBAL              5 (NULL + config)
                             94 LOAD_ATTR                3 (get_eras_open_ai_key)
                            104 PRECALL                  0
                            108 CALL                     0
                            118 POP_JUMP_FORWARD_IF_NONE    19 (to 158)
                            120 LOAD_GLOBAL              5 (NULL + config)
                            132 LOAD_ATTR                3 (get_eras_open_ai_key)
                            142 PRECALL                  0
                            146 CALL                     0
                            156 JUMP_FORWARD             1 (to 160)
                        >>  158 LOAD_CONST               1 ('')
                        >>  160 STORE_FAST               2 (openai_key_value)
                
-                24         162 LOAD_GLOBAL              5 (NULL + config)
+                25         162 LOAD_GLOBAL              5 (NULL + config)
                            174 LOAD_ATTR                4 (get_model_name)
                            184 PRECALL                  0
                            188 CALL                     0
                            198 POP_JUMP_FORWARD_IF_NONE    19 (to 238)
                            200 LOAD_GLOBAL              5 (NULL + config)
                            212 LOAD_ATTR                4 (get_model_name)
                            222 PRECALL                  0
                            226 CALL                     0
                            236 JUMP_FORWARD             1 (to 240)
                        >>  238 LOAD_CONST               1 ('')
                        >>  240 STORE_FAST               3 (model_name_value)
                
-                25         242 LOAD_GLOBAL              5 (NULL + config)
+                26         242 LOAD_GLOBAL              5 (NULL + config)
                            254 LOAD_ATTR                5 (get_eras_base_url)
                            264 PRECALL                  0
                            268 CALL                     0
                            278 POP_JUMP_FORWARD_IF_NONE    19 (to 318)
                            280 LOAD_GLOBAL              5 (NULL + config)
                            292 LOAD_ATTR                5 (get_eras_base_url)
                            302 PRECALL                  0
                            306 CALL                     0
                            316 JUMP_FORWARD             1 (to 320)
                        >>  318 LOAD_CONST               1 ('')
                        >>  320 STORE_FAST               4 (base_url_value)
                
-                28         322 LOAD_CONST               2 ('input')
+                29         322 LOAD_CONST               2 ('input')
                            324 LOAD_CONST               3 ('OpenAI key (or local llama key). Cannot be blank! :')
                            326 LOAD_CONST               4 ('openai_key_value')
                            328 LOAD_FAST                2 (openai_key_value)
                            330 LOAD_CONST               5 (('type', 'message', 'name', 'default'))
                            332 BUILD_CONST_KEY_MAP      4
                            334 STORE_FAST               5 (openai_key_question)
                
-                29         336 LOAD_CONST               2 ('input')
+                30         336 LOAD_CONST               2 ('input')
                            338 LOAD_CONST               6 ('Enter which model to use. e.g. Llama-3 or https://platform.openai.com/docs/models/gpt-4o :')
                            340 LOAD_CONST               7 ('model_name_value')
                            342 LOAD_FAST                3 (model_name_value)
                            344 LOAD_CONST               5 (('type', 'message', 'name', 'default'))
                            346 BUILD_CONST_KEY_MAP      4
                            348 STORE_FAST               6 (model_name_question)
                
-                30         350 LOAD_CONST               2 ('input')
+                31         350 LOAD_CONST               2 ('input')
                            352 LOAD_CONST               8 ('(Optional) Enter alternative base url (defaults to openai). (llama.cpp is http://127.0.0.1:8080) :  ')
                            354 LOAD_CONST               9 ('base_url_value')
                            356 LOAD_FAST                4 (base_url_value)
                            358 LOAD_CONST               5 (('type', 'message', 'name', 'default'))
                            360 BUILD_CONST_KEY_MAP      4
                            362 STORE_FAST               7 (base_url_question)
                
-                33         364 LOAD_FAST                5 (openai_key_question)
+                34         364 LOAD_FAST                5 (openai_key_question)
                
-                34         366 LOAD_FAST                6 (model_name_question)
+                35         366 LOAD_FAST                6 (model_name_question)
                
-                35         368 LOAD_FAST                7 (base_url_question)
+                36         368 LOAD_FAST                7 (base_url_question)
                
-                32         370 BUILD_LIST               3
+                33         370 BUILD_LIST               3
                            372 STORE_FAST               8 (questions)
                
-                38         374 LOAD_GLOBAL             13 (NULL + prompt)
+                39         374 LOAD_GLOBAL             13 (NULL + prompt)
                            386 LOAD_FAST                8 (questions)
                            388 PRECALL                  1
                            392 CALL                     1
                            402 STORE_FAST               9 (result)
                
-                39         404 LOAD_FAST                9 (result)
+                40         404 LOAD_FAST                9 (result)
                            406 LOAD_CONST               9 ('base_url_value')
                            408 BINARY_SUBSCR
                            418 STORE_FAST              10 (new_base_url_value)
                
-                40         420 LOAD_FAST                9 (result)
+                41         420 LOAD_FAST                9 (result)
                            422 LOAD_CONST               7 ('model_name_value')
                            424 BINARY_SUBSCR
                            434 STORE_FAST              11 (new_model_name_value)
                
-                41         436 LOAD_FAST                9 (result)
+                42         436 LOAD_FAST                9 (result)
                            438 LOAD_CONST               4 ('openai_key_value')
                            440 BINARY_SUBSCR
                            450 STORE_FAST              12 (new_openai_key_value)
                
-                43         452 LOAD_GLOBAL             15 (NULL + set_env_var)
+                44         452 LOAD_GLOBAL             15 (NULL + set_env_var)
                            464 LOAD_GLOBAL             16 (ERAS_OPENAI_KEY_ENV_VAR_NAME)
                            476 LOAD_FAST               12 (new_openai_key_value)
                            478 PRECALL                  2
                            482 CALL                     2
                            492 POP_TOP
                
-                44         494 LOAD_GLOBAL             15 (NULL + set_env_var)
+                45         494 LOAD_GLOBAL             15 (NULL + set_env_var)
                            506 LOAD_GLOBAL             18 (ERAS_MODEL_ENV_VAR_NAME)
                            518 LOAD_FAST               11 (new_model_name_value)
                            520 PRECALL                  2
                            524 CALL                     2
                            534 POP_TOP
                
-                45         536 LOAD_GLOBAL             15 (NULL + set_env_var)
+                46         536 LOAD_GLOBAL             15 (NULL + set_env_var)
                            548 LOAD_GLOBAL             20 (ERAS_BASE_URL_ENV_VAR_NAME)
                            560 LOAD_FAST               10 (new_base_url_value)
                            562 PRECALL                  2
                            566 CALL                     2
                            576 POP_TOP
                
-                48         578 LOAD_FAST                1 (should_reload_profile)
+                49         578 LOAD_FAST                1 (should_reload_profile)
                            580 POP_JUMP_FORWARD_IF_FALSE    22 (to 626)
                
-                49         582 LOAD_FAST                0 (self)
+                50         582 LOAD_FAST                0 (self)
                            584 LOAD_METHOD             11 (reload_prof)
                            606 PRECALL                  0
                            610 CALL                     0
                            620 POP_TOP
                            622 LOAD_CONST               0 (None)
                            624 RETURN_VALUE
                
-                48     >>  626 LOAD_CONST               0 (None)
+                49     >>  626 LOAD_CONST               0 (None)
                            628 RETURN_VALUE
                consts
                   None
                   ''
                   'input'
                   'OpenAI key (or local llama key). Cannot be blank! :'
                   'openai_key_value'
@@ -373,48 +378,48 @@
                   'base_url_value'
                names      ('print_eras_logo', 'show_commands', 'config', 'get_eras_open_ai_key', 'get_model_name', 'get_eras_base_url', 'prompt', 'set_env_var', 'ERAS_OPENAI_KEY_ENV_VAR_NAME', 'ERAS_MODEL_ENV_VAR_NAME', 'ERAS_BASE_URL_ENV_VAR_NAME', 'reload_prof')
                varnames   ('self', 'should_reload_profile', 'openai_key_value', 'model_name_value', 'base_url_value', 'openai_key_question', 'model_name_question', 'base_url_question', 'questions', 'result', 'new_base_url_value', 'new_model_name_value', 'new_openai_key_value')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                name       'prompt_for_all_configs'
-               firstlineno 20
+               firstlineno 21
                lnotab
                   0x0201280128015001500150030e010e010e030201020102fd04061e0110
                   01100110022a012a012a0304012cff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007400000000000000000000006a01000000000000000064016b0300
                   000000721d740500000000000000000000740700000000000000000000a6
                   000000ab000000000000000000a6010000ab010000000000000000010064
                   0353007409000000000000000000006402a6010000ab0100000000000000
                   00010064035300
-                51           0 RESUME                   0
+                52           0 RESUME                   0
                
-                53           2 LOAD_GLOBAL              0 (os)
+                54           2 LOAD_GLOBAL              0 (os)
                             14 LOAD_ATTR                1 (name)
                             24 LOAD_CONST               1 ('nt')
                             26 COMPARE_OP               3 (!=)
                             32 POP_JUMP_FORWARD_IF_FALSE    29 (to 92)
                
-                55          34 LOAD_GLOBAL              5 (NULL + reload_profile)
+                56          34 LOAD_GLOBAL              5 (NULL + reload_profile)
                             46 LOAD_GLOBAL              7 (NULL + get_profile_file)
                             58 PRECALL                  0
                             62 CALL                     0
                             72 PRECALL                  1
                             76 CALL                     1
                             86 POP_TOP
                             88 LOAD_CONST               3 (None)
                             90 RETURN_VALUE
                
-                57     >>   92 LOAD_GLOBAL              9 (NULL + print)
+                58     >>   92 LOAD_GLOBAL              9 (NULL + print)
                            104 LOAD_CONST               2 ('======= PLEASE CLOSE THIS TERMINAL WINDOW AND OPEN A NEW ONE =========')
                            106 PRECALL                  1
                            110 CALL                     1
                            120 POP_TOP
                            122 LOAD_CONST               3 (None)
                            124 RETURN_VALUE
                consts
@@ -424,15 +429,15 @@
                   None
                names      ('os', 'name', 'reload_profile', 'get_profile_file', 'print')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                name       'reload_prof'
-               firstlineno 51
+               firstlineno 52
                lnotab 0x020220023a02
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
@@ -444,81 +449,81 @@
                   00ab01000000000000000001007409000000000000000000006404a60100
                   00ab01000000000000000001007409000000000000000000006405a60100
                   00ab01000000000000000001007409000000000000000000006406a60100
                   00ab01000000000000000001007409000000000000000000006407a60100
                   00ab01000000000000000001007409000000000000000000006403a60100
                   00ab010000000000000000010074090000000000000000000064027c017a
                   050000a6010000ab010000000000000000010064005300
-                59           0 RESUME                   0
+                60           0 RESUME                   0
                
-                60           2 LOAD_GLOBAL              1 (NULL + os)
+                61           2 LOAD_GLOBAL              1 (NULL + os)
                             14 LOAD_ATTR                1 (get_terminal_size)
                             24 PRECALL                  0
                             28 CALL                     0
                             38 LOAD_ATTR                2 (columns)
                             48 STORE_FAST               1 (terminal_width)
                
-                61          50 LOAD_CONST               1 ('====== Commands ')
+                62          50 LOAD_CONST               1 ('====== Commands ')
                             52 STORE_FAST               2 (command_text_start)
                
-                62          54 LOAD_FAST                1 (terminal_width)
+                63          54 LOAD_FAST                1 (terminal_width)
                             56 LOAD_GLOBAL              7 (NULL + len)
                             68 LOAD_FAST                2 (command_text_start)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 BINARY_OP               10 (-)
                             88 STORE_FAST               3 (num_equals)
                
-                64          90 LOAD_GLOBAL              9 (NULL + print)
+                65          90 LOAD_GLOBAL              9 (NULL + print)
                            102 LOAD_FAST                2 (command_text_start)
                            104 LOAD_CONST               2 ('=')
                            106 LOAD_FAST                3 (num_equals)
                            108 BINARY_OP                5 (*)
                            112 BINARY_OP                0 (+)
                            116 PRECALL                  1
                            120 CALL                     1
                            130 POP_TOP
                
-                65         132 LOAD_GLOBAL              9 (NULL + print)
+                66         132 LOAD_GLOBAL              9 (NULL + print)
                            144 LOAD_CONST               3 ('')
                            146 PRECALL                  1
                            150 CALL                     1
                            160 POP_TOP
                
-                66         162 LOAD_GLOBAL              9 (NULL + print)
+                67         162 LOAD_GLOBAL              9 (NULL + print)
                            174 LOAD_CONST               4 ('{defualt usage} - Natural Languge Interface for running commands. e.g. eras how do I list all files in a directory -> %ls')
                            176 PRECALL                  1
                            180 CALL                     1
                            190 POP_TOP
                
-                67         192 LOAD_GLOBAL              9 (NULL + print)
+                68         192 LOAD_GLOBAL              9 (NULL + print)
                            204 LOAD_CONST               5 ('/help - get info about commands')
                            206 PRECALL                  1
                            210 CALL                     1
                            220 POP_TOP
                
-                68         222 LOAD_GLOBAL              9 (NULL + print)
+                69         222 LOAD_GLOBAL              9 (NULL + print)
                            234 LOAD_CONST               6 ('/chat - ask the LLM a question about anything. e.g. /chat tell me about quantum physics')
                            236 PRECALL                  1
                            240 CALL                     1
                            250 POP_TOP
                
-                69         252 LOAD_GLOBAL              9 (NULL + print)
+                70         252 LOAD_GLOBAL              9 (NULL + print)
                            264 LOAD_CONST               7 ('/conf - configure eras. urls, keys, etc')
                            266 PRECALL                  1
                            270 CALL                     1
                            280 POP_TOP
                
-                70         282 LOAD_GLOBAL              9 (NULL + print)
+                71         282 LOAD_GLOBAL              9 (NULL + print)
                            294 LOAD_CONST               3 ('')
                            296 PRECALL                  1
                            300 CALL                     1
                            310 POP_TOP
                
-                71         312 LOAD_GLOBAL              9 (NULL + print)
+                72         312 LOAD_GLOBAL              9 (NULL + print)
                            324 LOAD_CONST               2 ('=')
                            326 LOAD_FAST                1 (terminal_width)
                            328 BINARY_OP                5 (*)
                            332 PRECALL                  1
                            336 CALL                     1
                            346 POP_TOP
                            348 LOAD_CONST               0 (None)
@@ -534,163 +539,181 @@
                   '/conf - configure eras. urls, keys, etc'
                names      ('os', 'get_terminal_size', 'columns', 'len', 'print')
                varnames   ('self', 'terminal_width', 'command_text_start', 'num_equals')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                name       'show_commands'
-               firstlineno 59
+               firstlineno 60
                lnotab 0x02013001040124022a011e011e011e011e011e011e01
             code
                argcount  : 1
                nlocals   : 10
                stacksize : 8
                flags     : 3
                code
-                  0x870a970067006401a2017d0164027d0267006403a2017d03640484007c
-                  034400a6000000ab0000000000000000007d047401000000000000000000
-                  00640584007c044400a6000000ab000000000000000000a6010000ab0100
-                  000000000000008a0a880a6601640684087c044400a6000000ab00000000
-                  00000000007d0564077d06740300000000000000000000890aa6010000ab
-                  01000000000000000044005d5e7d077405000000000000000000007c05a6
-                  010000ab01000000000000000044005d475c0200007d087d097c067c017c
-                  087407000000000000000000007c01a6010000ab0100000000000000007a
-                  060000190000000000000000007c097c07190000000000000000007a0000
-                  007c027a0000007a0d00007d067c087407000000000000000000007c05a6
-                  010000ab01000000000000000064087a0a00006b000000000072057c0664
-                  097a0d00007d068c487c06640a7a0d00007d068c5f740900000000000000
-                  0000007c06a6010000ab010000000000000000010064005300
+                  0x870a97007400000000000000000000006a01000000000000000064016b
+                  0300000000720767006402a2017d0164037d026e0667006402a2017d0164
+                  037d0267006404a2017d03640584007c034400a6000000ab000000000000
+                  0000007d04740500000000000000000000640684007c044400a6000000ab
+                  000000000000000000a6010000ab0100000000000000008a0a880a660164
+                  0784087c044400a6000000ab0000000000000000007d0564087d06740700
+                  000000000000000000890aa6010000ab01000000000000000044005d5e7d
+                  077409000000000000000000007c05a6010000ab01000000000000000044
+                  005d475c0200007d087d097c067c017c08740b000000000000000000007c
+                  01a6010000ab0100000000000000007a060000190000000000000000007c
+                  097c07190000000000000000007a0000007c027a0000007a0d00007d067c
+                  08740b000000000000000000007c05a6010000ab01000000000000000064
+                  097a0a00006b000000000072057c06640a7a0d00007d068c487c06640b7a
+                  0d00007d068c5f740d000000000000000000007c06a6010000ab01000000
+                  0000000000010064005300
                              0 MAKE_CELL               10 (max_lines)
                
-                73           2 RESUME                   0
+                74           2 RESUME                   0
+               
+                77           4 LOAD_GLOBAL              0 (os)
+                            16 LOAD_ATTR                1 (name)
+                            26 LOAD_CONST               1 ('nt')
+                            28 COMPARE_OP               3 (!=)
+                            34 POP_JUMP_FORWARD_IF_FALSE     7 (to 50)
+               
+                78          36 BUILD_LIST               0
+                            38 LOAD_CONST               2 (('\x1b[94m', '\x1b[96m', '\x1b[91m', '\x1b[93m', '\x1b[95m'))
+                            40 LIST_EXTEND              1
+                            42 STORE_FAST               1 (colors)
+               
+                85          44 LOAD_CONST               3 ('\x1b[0m')
+                            46 STORE_FAST               2 (RESET)
+                            48 JUMP_FORWARD             6 (to 62)
+               
+                94     >>   50 BUILD_LIST               0
+                            52 LOAD_CONST               2 (('\x1b[94m', '\x1b[96m', '\x1b[91m', '\x1b[93m', '\x1b[95m'))
+                            54 LIST_EXTEND              1
+                            56 STORE_FAST               1 (colors)
+               
+               101          58 LOAD_CONST               3 ('\x1b[0m')
+                            60 STORE_FAST               2 (RESET)
+               
+               103     >>   62 BUILD_LIST               0
+                            64 LOAD_CONST               4 (('\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\:\\~\\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\ \\/__/  \n    \\:\\__\\    \n     \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/_|::\\/:/  /\n    |:|::/  / \n    |:|\\/__/  \n    |:|  |    \n    \\|__|     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/__\\:\\/:/  /\n      \\::/  / \n      /:/  /  \n     /:/  /   \n    \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\ \\  \\  \n  _\\:\\~\\ \\  \\ \n /\\ \\:\\ \\ \\__\\\n \\:\\ \\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\/:/  /  \n    \\::/  /   \n    \\/__/    \n            '))
+                            66 LIST_EXTEND              1
+                            68 STORE_FAST               3 (text_blocks)
+               
+               159          70 LOAD_CONST               5 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 159>)
+                            72 MAKE_FUNCTION            0
+                            74 LOAD_FAST                3 (text_blocks)
+                            76 GET_ITER
+                            78 PRECALL                  0
+                            82 CALL                     0
+                            92 STORE_FAST               4 (lines)
+               
+               160          94 LOAD_GLOBAL              5 (NULL + max)
+                           106 LOAD_CONST               6 (<code object <genexpr>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 160>)
+                           108 MAKE_FUNCTION            0
+                           110 LOAD_FAST                4 (lines)
+                           112 GET_ITER
+                           114 PRECALL                  0
+                           118 CALL                     0
+                           128 PRECALL                  1
+                           132 CALL                     1
+                           142 STORE_DEREF             10 (max_lines)
+               
+               161         144 LOAD_CLOSURE            10 (max_lines)
+                           146 BUILD_TUPLE              1
+                           148 LOAD_CONST               7 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 161>)
+                           150 MAKE_FUNCTION            8 (closure)
+                           152 LOAD_FAST                4 (lines)
+                           154 GET_ITER
+                           156 PRECALL                  0
+                           160 CALL                     0
+                           170 STORE_FAST               5 (padded_blocks)
+               
+               163         172 LOAD_CONST               8 ('')
+                           174 STORE_FAST               6 (colored_output)
+               
+               165         176 LOAD_GLOBAL              7 (NULL + range)
+                           188 LOAD_DEREF              10 (max_lines)
+                           190 PRECALL                  1
+                           194 CALL                     1
+                           204 GET_ITER
+                       >>  206 FOR_ITER                94 (to 396)
+                           208 STORE_FAST               7 (i)
                
-                75           4 BUILD_LIST               0
-                             6 LOAD_CONST               1 (('\x1b[38;2;230;57;70m', '\x1b[38;2;33;158;188m', '\x1b[38;138;201;38;71m', '\x1b[38;2;255;183;3m'))
-                             8 LIST_EXTEND              1
-                            10 STORE_FAST               1 (colors)
-               
-                81          12 LOAD_CONST               2 ('\x1b[0m')
-                            14 STORE_FAST               2 (RESET)
-               
-                83          16 BUILD_LIST               0
-                            18 LOAD_CONST               3 (('\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\:\\~\\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\ \\/__/  \n    \\:\\__\\    \n     \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/_|::\\/:/  /\n    |:|::/  / \n    |:|\\/__/  \n    |:|  |    \n    \\|__|     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/__\\:\\/:/  /\n      \\::/  / \n      /:/  /  \n     /:/  /   \n    \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\ \\  \\  \n  _\\:\\~\\ \\  \\ \n /\\ \\:\\ \\ \\__\\\n \\:\\ \\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\/:/  /  \n    \\::/  /   \n    \\/__/    \n            '))
-                            20 LIST_EXTEND              1
-                            22 STORE_FAST               3 (text_blocks)
-               
-               139          24 LOAD_CONST               4 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 139>)
-                            26 MAKE_FUNCTION            0
-                            28 LOAD_FAST                3 (text_blocks)
-                            30 GET_ITER
-                            32 PRECALL                  0
-                            36 CALL                     0
-                            46 STORE_FAST               4 (lines)
-               
-               140          48 LOAD_GLOBAL              1 (NULL + max)
-                            60 LOAD_CONST               5 (<code object <genexpr>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 140>)
-                            62 MAKE_FUNCTION            0
-                            64 LOAD_FAST                4 (lines)
-                            66 GET_ITER
-                            68 PRECALL                  0
-                            72 CALL                     0
-                            82 PRECALL                  1
-                            86 CALL                     1
-                            96 STORE_DEREF             10 (max_lines)
-               
-               141          98 LOAD_CLOSURE            10 (max_lines)
-                           100 BUILD_TUPLE              1
-                           102 LOAD_CONST               6 (<code object <listcomp>, file "/Users/jason/Documents/dev/eras/eras/services/user_config_service.py", line 141>)
-                           104 MAKE_FUNCTION            8 (closure)
-                           106 LOAD_FAST                4 (lines)
-                           108 GET_ITER
-                           110 PRECALL                  0
-                           114 CALL                     0
-                           124 STORE_FAST               5 (padded_blocks)
-               
-               143         126 LOAD_CONST               7 ('')
-                           128 STORE_FAST               6 (colored_output)
-               
-               145         130 LOAD_GLOBAL              3 (NULL + range)
-                           142 LOAD_DEREF              10 (max_lines)
-                           144 PRECALL                  1
-                           148 CALL                     1
-                           158 GET_ITER
-                       >>  160 FOR_ITER                94 (to 350)
-                           162 STORE_FAST               7 (i)
-               
-               146         164 LOAD_GLOBAL              5 (NULL + enumerate)
-                           176 LOAD_FAST                5 (padded_blocks)
-                           178 PRECALL                  1
-                           182 CALL                     1
-                           192 GET_ITER
-                       >>  194 FOR_ITER                71 (to 338)
-                           196 UNPACK_SEQUENCE          2
-                           200 STORE_FAST               8 (j)
-                           202 STORE_FAST               9 (block)
-               
-               147         204 LOAD_FAST                6 (colored_output)
-                           206 LOAD_FAST                1 (colors)
-                           208 LOAD_FAST                8 (j)
-                           210 LOAD_GLOBAL              7 (NULL + len)
-                           222 LOAD_FAST                1 (colors)
+               166         210 LOAD_GLOBAL              9 (NULL + enumerate)
+                           222 LOAD_FAST                5 (padded_blocks)
                            224 PRECALL                  1
                            228 CALL                     1
-                           238 BINARY_OP                6 (%)
-                           242 BINARY_SUBSCR
-                           252 LOAD_FAST                9 (block)
-                           254 LOAD_FAST                7 (i)
-                           256 BINARY_SUBSCR
-                           266 BINARY_OP                0 (+)
-                           270 LOAD_FAST                2 (RESET)
-                           272 BINARY_OP                0 (+)
-                           276 BINARY_OP               13 (+=)
-                           280 STORE_FAST               6 (colored_output)
-               
-               148         282 LOAD_FAST                8 (j)
-                           284 LOAD_GLOBAL              7 (NULL + len)
-                           296 LOAD_FAST                5 (padded_blocks)
-                           298 PRECALL                  1
-                           302 CALL                     1
-                           312 LOAD_CONST               8 (1)
-                           314 BINARY_OP               10 (-)
-                           318 COMPARE_OP               0 (<)
-                           324 POP_JUMP_FORWARD_IF_FALSE     5 (to 336)
-               
-               149         326 LOAD_FAST                6 (colored_output)
-                           328 LOAD_CONST               9 (' ')
-                           330 BINARY_OP               13 (+=)
-                           334 STORE_FAST               6 (colored_output)
-                       >>  336 JUMP_BACKWARD           72 (to 194)
-               
-               150     >>  338 LOAD_FAST                6 (colored_output)
-                           340 LOAD_CONST              10 ('\n')
-                           342 BINARY_OP               13 (+=)
-                           346 STORE_FAST               6 (colored_output)
-                           348 JUMP_BACKWARD           95 (to 160)
-               
-               152     >>  350 LOAD_GLOBAL              9 (NULL + print)
-                           362 LOAD_FAST                6 (colored_output)
-                           364 PRECALL                  1
-                           368 CALL                     1
-                           378 POP_TOP
-                           380 LOAD_CONST               0 (None)
-                           382 RETURN_VALUE
+                           238 GET_ITER
+                       >>  240 FOR_ITER                71 (to 384)
+                           242 UNPACK_SEQUENCE          2
+                           246 STORE_FAST               8 (j)
+                           248 STORE_FAST               9 (block)
+               
+               167         250 LOAD_FAST                6 (colored_output)
+                           252 LOAD_FAST                1 (colors)
+                           254 LOAD_FAST                8 (j)
+                           256 LOAD_GLOBAL             11 (NULL + len)
+                           268 LOAD_FAST                1 (colors)
+                           270 PRECALL                  1
+                           274 CALL                     1
+                           284 BINARY_OP                6 (%)
+                           288 BINARY_SUBSCR
+                           298 LOAD_FAST                9 (block)
+                           300 LOAD_FAST                7 (i)
+                           302 BINARY_SUBSCR
+                           312 BINARY_OP                0 (+)
+                           316 LOAD_FAST                2 (RESET)
+                           318 BINARY_OP                0 (+)
+                           322 BINARY_OP               13 (+=)
+                           326 STORE_FAST               6 (colored_output)
+               
+               168         328 LOAD_FAST                8 (j)
+                           330 LOAD_GLOBAL             11 (NULL + len)
+                           342 LOAD_FAST                5 (padded_blocks)
+                           344 PRECALL                  1
+                           348 CALL                     1
+                           358 LOAD_CONST               9 (1)
+                           360 BINARY_OP               10 (-)
+                           364 COMPARE_OP               0 (<)
+                           370 POP_JUMP_FORWARD_IF_FALSE     5 (to 382)
+               
+               169         372 LOAD_FAST                6 (colored_output)
+                           374 LOAD_CONST              10 (' ')
+                           376 BINARY_OP               13 (+=)
+                           380 STORE_FAST               6 (colored_output)
+                       >>  382 JUMP_BACKWARD           72 (to 240)
+               
+               170     >>  384 LOAD_FAST                6 (colored_output)
+                           386 LOAD_CONST              11 ('\n')
+                           388 BINARY_OP               13 (+=)
+                           392 STORE_FAST               6 (colored_output)
+                           394 JUMP_BACKWARD           95 (to 206)
+               
+               172     >>  396 LOAD_GLOBAL             13 (NULL + print)
+                           408 LOAD_FAST                6 (colored_output)
+                           410 PRECALL                  1
+                           414 CALL                     1
+                           424 POP_TOP
+                           426 LOAD_CONST               0 (None)
+                           428 RETURN_VALUE
                consts
                   None
-                  ('\x1b[38;2;230;57;70m', '\x1b[38;2;33;158;188m', '\x1b[38;138;201;38;71m', '\x1b[38;2;255;183;3m')
+                  'nt'
+                  ('\x1b[94m', '\x1b[96m', '\x1b[91m', '\x1b[93m', '\x1b[95m')
                   '\x1b[0m'
                   ('\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\:\\~\\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\ \\/__/  \n    \\:\\__\\    \n     \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/_|::\\/:/  /\n    |:|::/  / \n    |:|\\/__/  \n    |:|  |    \n    \\|__|     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\:\\  \\  \n  /::\\~\\:\\  \\ \n /:/\\:\\ \\:\\__\\\n \\/__\\:\\/:/  /\n      \\::/  / \n      /:/  /  \n     /:/  /   \n    \\/__/     \n            ', '\n      ___     \n     /\\  \\    \n    /::\\  \\   \n   /:/\\ \\  \\  \n  _\\:\\~\\ \\  \\ \n /\\ \\:\\ \\ \\__\\\n \\:\\ \\:\\ \\/__/\n  \\:\\ \\:\\__\\  \n   \\:\\/:/  /  \n    \\::/  /   \n    \\/__/    \n            ')
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d177d017c01a000000000000000000000000000000000
                         00000000006400a6010000ab01000000000000000091028c185300
-                     139           0 RESUME                   0
+                     159           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                23 (to 54)
                                    8 STORE_FAST               1 (block)
                                   10 LOAD_FAST                1 (block)
                                   12 LOAD_METHOD              0 (split)
                                   34 LOAD_CONST               0 ('\n')
@@ -703,25 +726,25 @@
                         '\n'
                      names      ('split',)
                      varnames   ('.0', 'block')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                      name       '<listcomp>'
-                     firstlineno 139
+                     firstlineno 159
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 51
                      code
                         0x4b00010097007c005d137d017401000000000000000000007c01a60100
                         00ab0100000000000000005600970101008c1464005300
-                     140           0 RETURN_GENERATOR
+                     160           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                19 (to 48)
                                   10 STORE_FAST               1 (block)
                                   12 LOAD_GLOBAL              1 (NULL + len)
                                   24 LOAD_FAST                1 (block)
@@ -737,28 +760,28 @@
                         None
                      names      ('len',)
                      varnames   ('.0', 'block')
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                      name       '<genexpr>'
-                     firstlineno 140
+                     firstlineno 160
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
                      
-                     141           2 RESUME                   0
+                     161           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                27 (to 64)
                                   10 STORE_FAST               1 (block)
                                   12 LOAD_FAST                1 (block)
                                   14 LOAD_CONST               0 ('')
                                   16 BUILD_LIST               1
@@ -777,40 +800,42 @@
                         ''
                      names      ('len',)
                      varnames   ('.0', 'block')
                      freevars   ('max_lines',)
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                      name       '<listcomp>'
-                     firstlineno 141
+                     firstlineno 161
                      lnotab 0x
                   ''
                   1
                   ' '
                   '\n'
-               names      ('max', 'range', 'enumerate', 'len', 'print')
+               names      ('os', 'name', 'max', 'range', 'enumerate', 'len', 'print')
                varnames   ('self', 'colors', 'RESET', 'text_blocks', 'lines', 'padded_blocks', 'colored_output', 'i', 'j', 'block')
                freevars   ()
                cellvars   ('max_lines',)
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
                name       'print_eras_logo'
-               firstlineno 73
-               lnotab 0x0402080604020838180132011c020402220128014e012c010c010c02
+               firstlineno 74
+               lnotab
+                  0x0403200108070609080704020838180132011c020402220128014e012c
+                  010c010c02
             None
             (True,)
          names      ('__name__', '__module__', '__qualname__', 'ensure_needed_configs_are_set', 'prompt_for_all_configs', 'reload_prof', 'show_commands', 'print_eras_logo')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
          name       'UserConfigService'
-         firstlineno 10
+         firstlineno 11
          lnotab 0x0a040606081f0608060e
       'UserConfigService'
-   names      ('InquirerPy', 'prompt', 'InquirerPy.base.control', 'Choice', 'os', 'sys', 'eras.utils.env_vars_and_profile_files', 'env_var_exists', 'reload_profile', 'get_profile_file', 'set_env_var', 'eras.models.constants', 'ERAS_OPENAI_KEY_ENV_VAR_NAME', 'ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME', 'ERAS_MODEL_ENV_VAR_NAME', 'ERAS_BASE_URL_ENV_VAR_NAME', 'eras.config.config', 'config', 'textwrap', 'UserConfigService')
+   names      ('InquirerPy', 'prompt', 'InquirerPy.base.control', 'Choice', 'os', 'sys', 'eras.utils.env_vars_and_profile_files', 'env_var_exists', 'reload_profile', 'get_profile_file', 'set_env_var', 'eras.models.constants', 'ERAS_OPENAI_KEY_ENV_VAR_NAME', 'ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME', 'ERAS_MODEL_ENV_VAR_NAME', 'ERAS_BASE_URL_ENV_VAR_NAME', 'eras.config.config', 'config', 'textwrap', 'platform', 'UserConfigService')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jason/Documents/dev/eras/eras/services/user_config_service.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0108010801180118010c010802
+   lnotab 0x00ff02010c010c0108010801180118010c0108010802
```

### Comparing `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.4.4/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.4.4/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.4.4/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/llm_callable_functions/user_details.py` & `eras-0.4.4/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/shell_command_service.py` & `eras-0.4.4/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/user_command_service.py` & `eras-0.4.4/eras/services/user_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/services/user_config_service.py` & `eras-0.4.4/eras/services/user_config_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from InquirerPy.base.control import Choice
 import os
 import sys
 from eras.utils.env_vars_and_profile_files import env_var_exists, reload_profile, get_profile_file, set_env_var
 from eras.models.constants import ERAS_OPENAI_KEY_ENV_VAR_NAME, ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME, ERAS_MODEL_ENV_VAR_NAME, ERAS_BASE_URL_ENV_VAR_NAME
 from eras.config.config import config
 import textwrap
+import platform
 
 class UserConfigService:
     # def __init__(self):
     #     print('init')
 
     def ensure_needed_configs_are_set(self):
         if not env_var_exists(ERAS_HAS_RUN_INITIAL_CONFIG_VAR_NAME):
@@ -68,19 +69,21 @@
         print("/chat - ask the LLM a question about anything. e.g. /chat tell me about quantum physics")
         print("/conf - configure eras. urls, keys, etc")
         print("")
         print("=" * terminal_width)
 
     def print_eras_logo(self):
         # Define ANSI escape codes for 256-color mode with given RGB colors
+
         colors = [
-            "\033[38;2;230;57;70m",  # RGB (142, 202, 230)
-            "\033[38;2;33;158;188m",  # RGB (33, 158, 188)
-            "\033[38;138;201;38;71m",  # white
-            "\033[38;2;255;183;3m",  # RGB (255, 183, 3)
+            "\033[94m",  # Bright blue
+            "\033[96m",  # Bright cyan
+            "\033[91m",  # Bright red
+            "\033[93m",  # Bright yellow
+            "\033[95m"  # Bright magenta
         ]
         RESET = "\033[0m"
 
         text_blocks = [
             r"""
       ___     
      /\  \
```

### Comparing `eras-0.4.3/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc` & `eras-0.4.4/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras/utils/env_vars_and_profile_files.py` & `eras-0.4.4/eras/utils/env_vars_and_profile_files.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/eras.egg-info/PKG-INFO` & `eras-0.4.4/eras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.3
+Version: 0.4.4
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.4.3/eras.egg-info/SOURCES.txt` & `eras-0.4.4/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.4.3/setup.py` & `eras-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eras',
-    version='0.4.3',
+    version='0.4.4',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

