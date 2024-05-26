# Comparing `tmp/eras-0.4.1.tar.gz` & `tmp/eras-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.4.1.tar", last modified: Sun May 26 00:16:43 2024, max compression
+gzip compressed data, was "eras-0.4.2.tar", last modified: Sun May 26 00:20:29 2024, max compression
```

## Comparing `eras-0.4.1.tar` & `eras-0.4.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:43.006729 eras-0.4.1/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.1/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.1/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     4669 2024-05-26 00:16:43.006246 eras-0.4.1/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     4013 2024-05-26 00:16:31.000000 eras-0.4.1/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.976363 eras-0.4.1/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.1/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.979708 eras-0.4.1/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.1/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.1/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.1/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.981536 eras-0.4.1/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.1/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.984269 eras-0.4.1/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.1/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.1/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.1/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.1/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.1/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.1/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.1/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.1/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.1/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.1/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.1/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.1/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.1/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.984834 eras-0.4.1/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.1/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.985658 eras-0.4.1/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.1/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.1/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.1/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.1/eras/config/config.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.986202 eras-0.4.1/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.1/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.986982 eras-0.4.1/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.1/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.1/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.1/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.987910 eras-0.4.1/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.1/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.989722 eras-0.4.1/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.1/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.1/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.1/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.1/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.1/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.1/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.1/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.1/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.992100 eras-0.4.1/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.1/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.996687 eras-0.4.1/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.1/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.1/eras/models/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.1/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.1/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.1/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.1/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.1/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.1/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.1/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.1/eras/models/constants.py
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.1/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.1/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.1/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.1/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.1/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.1/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.998859 eras-0.4.1/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.1/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:43.000999 eras-0.4.1/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.1/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.1/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.1/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4550 2024-05-25 23:05:46.000000 eras-0.4.1/eras/services/__pycache__/user_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3927 2024-05-25 23:35:32.000000 eras-0.4.1/eras/services/__pycache__/user_config_service.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:43.002701 eras-0.4.1/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.1/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:43.004681 eras-0.4.1/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.1/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.1/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.1/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.1/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     2189 2024-05-25 23:04:34.000000 eras-0.4.1/eras/services/user_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     2885 2024-05-25 23:34:52.000000 eras-0.4.1/eras/services/user_config_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:43.005116 eras-0.4.1/eras/utils/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.1/eras/utils/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:43.005630 eras-0.4.1/eras/utils/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.1/eras/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.1/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.1/eras/utils/env_vars_and_profile_files.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:16:42.978528 eras-0.4.1/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     4669 2024-05-26 00:16:42.000000 eras-0.4.1/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 00:16:42.000000 eras-0.4.1/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 00:16:42.000000 eras-0.4.1/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 00:16:42.000000 eras-0.4.1/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       86 2024-05-26 00:16:42.000000 eras-0.4.1/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 00:16:42.000000 eras-0.4.1/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 00:16:43.006819 eras-0.4.1/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1066 2024-05-26 00:16:39.000000 eras-0.4.1/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.882862 eras-0.4.2/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.4.2/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.4.2/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 00:20:29.882037 eras-0.4.2/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     4217 2024-05-26 00:19:57.000000 eras-0.4.2/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.853708 eras-0.4.2/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.4.2/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.855881 eras-0.4.2/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.4.2/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.4.2/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.4.2/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.857537 eras-0.4.2/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.4.2/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.860650 eras-0.4.2/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.2/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.4.2/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.4.2/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.4.2/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.4.2/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.4.2/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.4.2/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.4.2/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.4.2/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.4.2/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.4.2/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.4.2/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.4.2/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.861406 eras-0.4.2/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.4.2/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.862658 eras-0.4.2/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.2/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.4.2/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.4.2/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.4.2/eras/config/config.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.863318 eras-0.4.2/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.4.2/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.864057 eras-0.4.2/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.4.2/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.4.2/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.4.2/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.865026 eras-0.4.2/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.4.2/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.866687 eras-0.4.2/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.4.2/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.4.2/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.4.2/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.4.2/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.4.2/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.4.2/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.4.2/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.4.2/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.869090 eras-0.4.2/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.4.2/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.872859 eras-0.4.2/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.4.2/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.4.2/eras/models/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.4.2/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.4.2/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.4.2/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.4.2/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.4.2/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.4.2/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.4.2/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.4.2/eras/models/constants.py
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.4.2/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.4.2/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.4.2/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.4.2/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.4.2/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.4.2/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.874523 eras-0.4.2/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.4.2/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.876384 eras-0.4.2/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.4.2/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.4.2/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.4.2/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4550 2024-05-25 23:05:46.000000 eras-0.4.2/eras/services/__pycache__/user_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3927 2024-05-25 23:35:32.000000 eras-0.4.2/eras/services/__pycache__/user_config_service.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.877821 eras-0.4.2/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.4.2/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.879770 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.4.2/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.4.2/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.4.2/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.4.2/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.4.2/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     2189 2024-05-25 23:04:34.000000 eras-0.4.2/eras/services/user_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     2885 2024-05-25 23:34:52.000000 eras-0.4.2/eras/services/user_config_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.880444 eras-0.4.2/eras/utils/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.4.2/eras/utils/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.881221 eras-0.4.2/eras/utils/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.4.2/eras/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.4.2/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.4.2/eras/utils/env_vars_and_profile_files.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-26 00:20:29.855104 eras-0.4.2/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     4873 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       86 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-26 00:20:29.000000 eras-0.4.2/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-26 00:20:29.883041 eras-0.4.2/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1066 2024-05-26 00:20:04.000000 eras-0.4.2/setup.py
```

### Comparing `eras-0.4.1/PKG-INFO` & `eras-0.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.1
+Version: 0.4.2
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -89,22 +89,27 @@
 % eras /chat "What is the capital of France?"
 % Paris is the capital of France
 ```
 
 ### Config Examples
 On the first run of eras, you will be prompted to enter config values, which are saved as env vars.
 
+To run the config again, you can run `eras /config`
+
 An API key must be provided when using OpenAI or Llama.cpp (can be anything unless you explicitly set one in Llama.cpp)
 
 #### OpenAI
 For OpenAI you must provide:
 - API Key - Grab an OpenAI key from [here](https://platform.openai.com/api-keys)
 - Model name - (defaults to gpt-4) Find any valid one [here](https://platform.openai.com/docs/models)
 
-#### Llama.cpp server
+#### Alternative OpenAI Server (e.g. Llama.cpp server)
+You will be prompted to enter the alternative base url. e.g. `http://127.0.0.1:8080`
+
+## Llama.cpp Setup Instructions
 Find the server setup instructions at: https://github.com/ggerganov/llama.cpp
 
 ##### NVIDIA GPU Instructions
 If you are running a NVIDIA GPU, you will want to build the llama server with CUDA enabled, as outlined [here](https://github.com/ggerganov/llama.cpp?tab=readme-ov-file#cuda)
 
 I followed [these instructions](https://medium.com/@michaelhumor/how-to-build-llama-cpp-on-windows-with-nvidia-gpu-226a28069a76):
```

### Comparing `eras-0.4.1/README.md` & `eras-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,22 +70,27 @@
 % eras /chat "What is the capital of France?"
 % Paris is the capital of France
 ```
 
 ### Config Examples
 On the first run of eras, you will be prompted to enter config values, which are saved as env vars.
 
+To run the config again, you can run `eras /config`
+
 An API key must be provided when using OpenAI or Llama.cpp (can be anything unless you explicitly set one in Llama.cpp)
 
 #### OpenAI
 For OpenAI you must provide:
 - API Key - Grab an OpenAI key from [here](https://platform.openai.com/api-keys)
 - Model name - (defaults to gpt-4) Find any valid one [here](https://platform.openai.com/docs/models)
 
-#### Llama.cpp server
+#### Alternative OpenAI Server (e.g. Llama.cpp server)
+You will be prompted to enter the alternative base url. e.g. `http://127.0.0.1:8080`
+
+## Llama.cpp Setup Instructions
 Find the server setup instructions at: https://github.com/ggerganov/llama.cpp
 
 ##### NVIDIA GPU Instructions
 If you are running a NVIDIA GPU, you will want to build the llama server with CUDA enabled, as outlined [here](https://github.com/ggerganov/llama.cpp?tab=readme-ov-file#cuda)
 
 I followed [these instructions](https://medium.com/@michaelhumor/how-to-build-llama-cpp-on-windows-with-nvidia-gpu-226a28069a76):
```

### Comparing `eras-0.4.1/eras/__pycache__/main.cpython-311.pyc` & `eras-0.4.2/eras/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.4.2/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.4.2/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.4.2/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.4.2/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.4.2/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.4.2/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.4.2/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/llama_functions_agent.py` & `eras-0.4.2/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.4.2/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/llm_functions_agent.py` & `eras-0.4.2/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/simple_llm.py` & `eras-0.4.2/eras/agents/simple_llm.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/agents/terminal_llama_agent.py` & `eras-0.4.2/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/config/__pycache__/config.cpython-311.pyc` & `eras-0.4.2/eras/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.4.2/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/config/config.py` & `eras-0.4.2/eras/config/config.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.4.2/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/decorators/chatgpt_tool_data.py` & `eras-0.4.2/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.4.2/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.4.2/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.4.2/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.4.2/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/factories/function_details_factory.py` & `eras-0.4.2/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/factories/message_factory.py` & `eras-0.4.2/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/main.py` & `eras-0.4.2/eras/main.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.4.2/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.4.2/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.4.2/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.4.2/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.4.2/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.4.2/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/conversation.py` & `eras-0.4.2/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/function_details.py` & `eras-0.4.2/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/message.py` & `eras-0.4.2/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/models/transaction.py` & `eras-0.4.2/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/run.ipynb` & `eras-0.4.2/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.4.2/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.4.2/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.4.2/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/__pycache__/user_config_service.cpython-311.pyc` & `eras-0.4.2/eras/services/__pycache__/user_config_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.4.2/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.4.2/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.4.2/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/llm_callable_functions/user_details.py` & `eras-0.4.2/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/shell_command_service.py` & `eras-0.4.2/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/user_command_service.py` & `eras-0.4.2/eras/services/user_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/services/user_config_service.py` & `eras-0.4.2/eras/services/user_config_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc` & `eras-0.4.2/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras/utils/env_vars_and_profile_files.py` & `eras-0.4.2/eras/utils/env_vars_and_profile_files.py`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/eras.egg-info/PKG-INFO` & `eras-0.4.2/eras.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.4.1
+Version: 0.4.2
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -89,22 +89,27 @@
 % eras /chat "What is the capital of France?"
 % Paris is the capital of France
 ```
 
 ### Config Examples
 On the first run of eras, you will be prompted to enter config values, which are saved as env vars.
 
+To run the config again, you can run `eras /config`
+
 An API key must be provided when using OpenAI or Llama.cpp (can be anything unless you explicitly set one in Llama.cpp)
 
 #### OpenAI
 For OpenAI you must provide:
 - API Key - Grab an OpenAI key from [here](https://platform.openai.com/api-keys)
 - Model name - (defaults to gpt-4) Find any valid one [here](https://platform.openai.com/docs/models)
 
-#### Llama.cpp server
+#### Alternative OpenAI Server (e.g. Llama.cpp server)
+You will be prompted to enter the alternative base url. e.g. `http://127.0.0.1:8080`
+
+## Llama.cpp Setup Instructions
 Find the server setup instructions at: https://github.com/ggerganov/llama.cpp
 
 ##### NVIDIA GPU Instructions
 If you are running a NVIDIA GPU, you will want to build the llama server with CUDA enabled, as outlined [here](https://github.com/ggerganov/llama.cpp?tab=readme-ov-file#cuda)
 
 I followed [these instructions](https://medium.com/@michaelhumor/how-to-build-llama-cpp-on-windows-with-nvidia-gpu-226a28069a76):
```

### Comparing `eras-0.4.1/eras.egg-info/SOURCES.txt` & `eras-0.4.2/eras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eras-0.4.1/setup.py` & `eras-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eras',
-    version='0.4.1',
+    version='0.4.2',
     include_package_data=True,
     packages=find_packages(include=["eras", "eras.*"]),
     package_data={
         '': ['*.txt', '*.rst'],
         'eras': ['*.md'],
     },
     install_requires=[
```

