# Comparing `tmp/eras-0.3.6.tar.gz` & `tmp/eras-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.3.6.tar", last modified: Fri May 24 03:18:53 2024, max compression
+gzip compressed data, was "eras-0.3.7.tar", last modified: Sat May 25 23:48:11 2024, max compression
```

## Comparing `eras-0.3.6.tar` & `eras-0.3.7.tar`

### file list

```diff
@@ -1,100 +1,108 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.550129 eras-0.3.6/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.3.6/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.3.6/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)     2866 2024-05-24 03:18:53.549481 eras-0.3.6/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     2243 2024-05-24 03:18:21.000000 eras-0.3.6/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.519797 eras-0.3.6/eras/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.3.6/eras/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.521767 eras-0.3.6/eras/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.3.6/eras/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.3.6/eras/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1367 2024-05-23 02:54:10.000000 eras-0.3.6/eras/__pycache__/main.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.523485 eras-0.3.6/eras/agents/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.3.6/eras/agents/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.526262 eras-0.3.6/eras/agents/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.6/eras/agents/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.3.6/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.3.6/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.3.6/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.3.6/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2628 2024-05-23 03:13:09.000000 eras-0.3.6/eras/agents/__pycache__/simple_llm.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.3.6/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.3.6/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.3.6/eras/agents/llama_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.3.6/eras/agents/llama_terminal_command_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.3.6/eras/agents/llm_functions_agent.py
--rw-r--r--   0 jason      (501) staff       (20)     1798 2024-05-23 03:13:06.000000 eras-0.3.6/eras/agents/simple_llm.py
--rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.3.6/eras/agents/terminal_llama_agent.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.527323 eras-0.3.6/eras/config/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.3.6/eras/config/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.528604 eras-0.3.6/eras/config/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.6/eras/config/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1864 2024-05-23 03:06:20.000000 eras-0.3.6/eras/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.3.6/eras/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     6625 2024-05-23 02:41:23.000000 eras-0.3.6/eras/config/__pycache__/post_install.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1531 2024-05-24 03:12:51.000000 eras-0.3.6/eras/config/config.py
--rw-r--r--   0 jason      (501) staff       (20)     4360 2024-05-24 03:12:51.000000 eras-0.3.6/eras/config/post_install.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.529132 eras-0.3.6/eras/decorators/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.3.6/eras/decorators/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.529862 eras-0.3.6/eras/decorators/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.3.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.3.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.3.6/eras/decorators/chatgpt_tool_data.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.531316 eras-0.3.6/eras/factories/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.3.6/eras/factories/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.534135 eras-0.3.6/eras/factories/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.3.6/eras/factories/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.3.6/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.3.6/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.3.6/eras/factories/__pycache__/message_factory.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.3.6/eras/factories/__pycache__/message_factory.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.3.6/eras/factories/function_details_factory.py
--rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.3.6/eras/factories/message_factory.py
--rw-r--r--   0 jason      (501) staff       (20)      735 2024-05-23 02:52:24.000000 eras-0.3.6/eras/main.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.536907 eras-0.3.6/eras/models/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.3.6/eras/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.540712 eras-0.3.6/eras/models/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.6/eras/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.3.6/eras/models/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.3.6/eras/models/__pycache__/conversation.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.3.6/eras/models/__pycache__/function_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.3.6/eras/models/__pycache__/function_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.3.6/eras/models/__pycache__/message.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.3.6/eras/models/__pycache__/message.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.3.6/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.3.6/eras/models/conversation.py
--rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.3.6/eras/models/function_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.3.6/eras/models/message.py
--rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.3.6/eras/models/simple_stream_inference_callable.py
--rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.3.6/eras/models/transaction.py
--rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.3.6/eras/run.ipynb
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.542157 eras-0.3.6/eras/services/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.3.6/eras/services/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.544027 eras-0.3.6/eras/services/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.3.6/eras/services/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.3.6/eras/services/__pycache__/shell_command_service.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.3.6/eras/services/__pycache__/shell_command_service.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     3776 2024-05-23 03:17:34.000000 eras-0.3.6/eras/services/__pycache__/user_command_service.cpython-311.pyc
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.545480 eras-0.3.6/eras/services/llm_callable_functions/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.3.6/eras/services/llm_callable_functions/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.548652 eras-0.3.6/eras/services/llm_callable_functions/__pycache__/
--rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.3.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.3.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.3.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.3.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.3.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
--rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.3.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
--rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.3.6/eras/services/llm_callable_functions/callable_function_service_base.py
--rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.3.6/eras/services/llm_callable_functions/terminal_command.py
--rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.3.6/eras/services/llm_callable_functions/user_details.py
--rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.3.6/eras/services/shell_command_service.py
--rw-r--r--   0 jason      (501) staff       (20)     1846 2024-05-23 03:16:10.000000 eras-0.3.6/eras/services/user_command_service.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-24 03:18:53.521109 eras-0.3.6/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)     2866 2024-05-24 03:18:53.000000 eras-0.3.6/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     3632 2024-05-24 03:18:53.000000 eras-0.3.6/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-24 03:18:53.000000 eras-0.3.6/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-24 03:18:53.000000 eras-0.3.6/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       68 2024-05-24 03:18:53.000000 eras-0.3.6/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-24 03:18:53.000000 eras-0.3.6/eras.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-24 03:18:53.550272 eras-0.3.6/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     2549 2024-05-24 03:18:47.000000 eras-0.3.6/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.197041 eras-0.3.7/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.3.7/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)      104 2024-05-19 21:51:44.000000 eras-0.3.7/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)     2899 2024-05-25 23:48:11.196303 eras-0.3.7/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     2243 2024-05-24 03:18:21.000000 eras-0.3.7/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.162389 eras-0.3.7/eras/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 19:56:59.000000 eras-0.3.7/eras/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.165152 eras-0.3.7/eras/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      157 2024-05-23 02:41:00.000000 eras-0.3.7/eras/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-05-19 20:28:39.000000 eras-0.3.7/eras/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1501 2024-05-25 15:40:54.000000 eras-0.3.7/eras/__pycache__/main.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.167791 eras-0.3.7/eras/agents/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:47.000000 eras-0.3.7/eras/agents/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.171074 eras-0.3.7/eras/agents/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.7/eras/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7294 2024-05-19 00:22:09.000000 eras-0.3.7/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     7470 2024-05-19 01:33:26.000000 eras-0.3.7/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4851 2024-05-18 23:32:12.000000 eras-0.3.7/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3157 2024-05-12 03:03:23.000000 eras-0.3.7/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2636 2024-05-25 23:41:32.000000 eras-0.3.7/eras/agents/__pycache__/simple_llm.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3858 2024-05-23 03:06:20.000000 eras-0.3.7/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4934 2024-05-19 20:28:39.000000 eras-0.3.7/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)    17170 2024-05-19 01:34:25.000000 eras-0.3.7/eras/agents/llama_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     9360 2024-05-19 01:35:28.000000 eras-0.3.7/eras/agents/llama_terminal_command_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     6378 2024-05-19 23:25:46.000000 eras-0.3.7/eras/agents/llm_functions_agent.py
+-rw-r--r--   0 jason      (501) staff       (20)     1822 2024-05-25 23:41:09.000000 eras-0.3.7/eras/agents/simple_llm.py
+-rw-r--r--   0 jason      (501) staff       (20)     4784 2024-05-23 03:02:01.000000 eras-0.3.7/eras/agents/terminal_llama_agent.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.172000 eras-0.3.7/eras/config/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:43.000000 eras-0.3.7/eras/config/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.173051 eras-0.3.7/eras/config/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.7/eras/config/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2958 2024-05-25 23:29:53.000000 eras-0.3.7/eras/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1017 2024-05-19 20:28:39.000000 eras-0.3.7/eras/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1768 2024-05-25 23:29:50.000000 eras-0.3.7/eras/config/config.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.173784 eras-0.3.7/eras/decorators/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:37.000000 eras-0.3.7/eras/decorators/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.174809 eras-0.3.7/eras/decorators/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      532 2024-05-18 23:32:12.000000 eras-0.3.7/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      445 2024-05-12 00:49:22.000000 eras-0.3.7/eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1278 2024-01-29 15:43:14.000000 eras-0.3.7/eras/decorators/chatgpt_tool_data.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.176111 eras-0.3.7/eras/factories/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:17.000000 eras-0.3.7/eras/factories/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.178471 eras-0.3.7/eras/factories/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      167 2024-05-19 20:56:32.000000 eras-0.3.7/eras/factories/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2282 2024-05-19 01:02:12.000000 eras-0.3.7/eras/factories/__pycache__/function_details_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1459 2024-05-19 18:18:30.000000 eras-0.3.7/eras/factories/__pycache__/function_details_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3160 2024-05-23 02:41:23.000000 eras-0.3.7/eras/factories/__pycache__/message_factory.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2075 2024-05-19 18:18:30.000000 eras-0.3.7/eras/factories/__pycache__/message_factory.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2056 2024-05-19 21:15:29.000000 eras-0.3.7/eras/factories/function_details_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)     2702 2024-05-19 23:27:04.000000 eras-0.3.7/eras/factories/message_factory.py
+-rw-r--r--   0 jason      (501) staff       (20)      846 2024-05-25 15:14:49.000000 eras-0.3.7/eras/main.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.181725 eras-0.3.7/eras/models/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:07.000000 eras-0.3.7/eras/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.185309 eras-0.3.7/eras/models/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      164 2024-05-19 20:56:32.000000 eras-0.3.7/eras/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      431 2024-05-25 22:59:33.000000 eras-0.3.7/eras/models/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4361 2024-05-23 02:41:23.000000 eras-0.3.7/eras/models/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2979 2024-05-19 18:18:30.000000 eras-0.3.7/eras/models/__pycache__/conversation.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1458 2024-05-23 02:41:23.000000 eras-0.3.7/eras/models/__pycache__/function_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1044 2024-05-12 00:49:22.000000 eras-0.3.7/eras/models/__pycache__/function_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1503 2024-05-18 23:32:12.000000 eras-0.3.7/eras/models/__pycache__/message.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1078 2024-05-12 00:49:22.000000 eras-0.3.7/eras/models/__pycache__/message.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      460 2024-05-23 03:06:20.000000 eras-0.3.7/eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-25 22:58:32.000000 eras-0.3.7/eras/models/constants.py
+-rw-r--r--   0 jason      (501) staff       (20)     2535 2024-05-19 21:14:20.000000 eras-0.3.7/eras/models/conversation.py
+-rw-r--r--   0 jason      (501) staff       (20)      732 2024-05-19 21:15:38.000000 eras-0.3.7/eras/models/function_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1498 2024-01-29 15:43:14.000000 eras-0.3.7/eras/models/message.py
+-rw-r--r--   0 jason      (501) staff       (20)      394 2024-05-23 02:58:36.000000 eras-0.3.7/eras/models/simple_stream_inference_callable.py
+-rw-r--r--   0 jason      (501) staff       (20)      590 2024-01-29 15:43:14.000000 eras-0.3.7/eras/models/transaction.py
+-rw-r--r--   0 jason      (501) staff       (20)     6850 2024-05-19 02:17:49.000000 eras-0.3.7/eras/run.ipynb
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.186902 eras-0.3.7/eras/services/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:02.000000 eras-0.3.7/eras/services/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.188751 eras-0.3.7/eras/services/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      166 2024-05-19 20:56:32.000000 eras-0.3.7/eras/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2573 2024-05-23 02:54:10.000000 eras-0.3.7/eras/services/__pycache__/shell_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1771 2024-05-19 20:28:39.000000 eras-0.3.7/eras/services/__pycache__/shell_command_service.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4550 2024-05-25 23:05:46.000000 eras-0.3.7/eras/services/__pycache__/user_command_service.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     3927 2024-05-25 23:35:32.000000 eras-0.3.7/eras/services/__pycache__/user_config_service.cpython-311.pyc
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.190351 eras-0.3.7/eras/services/llm_callable_functions/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-19 20:55:10.000000 eras-0.3.7/eras/services/llm_callable_functions/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.193476 eras-0.3.7/eras/services/llm_callable_functions/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)     2365 2024-05-18 23:32:12.000000 eras-0.3.7/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1625 2024-05-12 00:49:22.000000 eras-0.3.7/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1826 2024-05-19 01:04:12.000000 eras-0.3.7/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1315 2024-05-19 18:18:30.000000 eras-0.3.7/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2363 2024-05-18 23:32:12.000000 eras-0.3.7/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     1695 2024-05-12 00:49:22.000000 eras-0.3.7/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     2415 2024-01-29 15:43:14.000000 eras-0.3.7/eras/services/llm_callable_functions/callable_function_service_base.py
+-rw-r--r--   0 jason      (501) staff       (20)     1188 2024-05-19 21:15:55.000000 eras-0.3.7/eras/services/llm_callable_functions/terminal_command.py
+-rw-r--r--   0 jason      (501) staff       (20)     1848 2024-05-19 21:16:00.000000 eras-0.3.7/eras/services/llm_callable_functions/user_details.py
+-rw-r--r--   0 jason      (501) staff       (20)     1689 2024-05-23 02:53:26.000000 eras-0.3.7/eras/services/shell_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     2189 2024-05-25 23:04:34.000000 eras-0.3.7/eras/services/user_command_service.py
+-rw-r--r--   0 jason      (501) staff       (20)     2885 2024-05-25 23:34:52.000000 eras-0.3.7/eras/services/user_config_service.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.194630 eras-0.3.7/eras/utils/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-05-25 14:20:53.000000 eras-0.3.7/eras/utils/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.195566 eras-0.3.7/eras/utils/__pycache__/
+-rw-r--r--   0 jason      (501) staff       (20)      163 2024-05-25 15:40:55.000000 eras-0.3.7/eras/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     6476 2024-05-25 23:19:24.000000 eras-0.3.7/eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
+-rw-r--r--   0 jason      (501) staff       (20)     4198 2024-05-25 23:17:27.000000 eras-0.3.7/eras/utils/env_vars_and_profile_files.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-25 23:48:11.164162 eras-0.3.7/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)     2899 2024-05-25 23:48:11.000000 eras-0.3.7/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     3903 2024-05-25 23:48:11.000000 eras-0.3.7/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-25 23:48:11.000000 eras-0.3.7/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       40 2024-05-25 23:48:11.000000 eras-0.3.7/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       86 2024-05-25 23:48:11.000000 eras-0.3.7/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        5 2024-05-25 23:48:11.000000 eras-0.3.7/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-25 23:48:11.197196 eras-0.3.7/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1066 2024-05-25 23:47:42.000000 eras-0.3.7/setup.py
```

### Comparing `eras-0.3.6/PKG-INFO` & `eras-0.3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.3.6
+Version: 0.3.7
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
+Requires-Dist: InquirerPy==0.3.4
 
 # ERAS
 Easily Runnable AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
 Works on Windows, Mac, and Linux!
```

### Comparing `eras-0.3.6/README.md` & `eras-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/__pycache__/main.cpython-311.pyc` & `eras-0.3.7/eras/__pycache__/main.cpython-311.pyc`

 * *Files 27% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x68af4e66 (Thu May 23 02:52:24 2024 UTC)
-files sz: 735
+moddate:  0x69005266 (Sat May 25 15:14:49 2024 UTC)
+files sz: 846
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -46,132 +46,139 @@
                 60 LOAD_CONST               3 (('UserCommandService',))
                 62 IMPORT_NAME              5 (eras.services.user_command_service)
                 64 IMPORT_FROM              6 (UserCommandService)
                 66 STORE_NAME               6 (UserCommandService)
                 68 POP_TOP
    
      8          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               4 (('ensure',))
-                74 IMPORT_NAME              7 (eras.config.post_install)
-                76 IMPORT_FROM              8 (ensure)
-                78 STORE_NAME               8 (ensure)
+                72 LOAD_CONST               4 (('UserConfigService',))
+                74 IMPORT_NAME              7 (eras.services.user_config_service)
+                76 IMPORT_FROM              8 (UserConfigService)
+                78 STORE_NAME               8 (UserConfigService)
                 80 POP_TOP
    
-    10          82 LOAD_CONST               5 (<code object main, file "/Users/jason/Documents/dev/eras/eras/main.py", line 10>)
+    11          82 LOAD_CONST               5 (<code object main, file "/Users/jason/Documents/dev/eras/eras/main.py", line 11>)
                 84 MAKE_FUNCTION            0
                 86 STORE_NAME               9 (main)
    
-    21          88 LOAD_NAME               10 (__name__)
+    24          88 LOAD_NAME               10 (__name__)
                 90 LOAD_CONST               6 ('__main__')
                 92 COMPARE_OP               2 (==)
                 98 POP_JUMP_FORWARD_IF_FALSE    12 (to 124)
    
-    22         100 PUSH_NULL
+    25         100 PUSH_NULL
                102 LOAD_NAME                9 (main)
                104 PRECALL                  0
                108 CALL                     0
                118 POP_TOP
                120 LOAD_CONST               1 (None)
                122 RETURN_VALUE
    
-    21     >>  124 LOAD_CONST               1 (None)
+    24     >>  124 LOAD_CONST               1 (None)
                126 RETURN_VALUE
    consts
       0
       None
       ('load_dotenv',)
       ('UserCommandService',)
-      ('ensure',)
+      ('UserConfigService',)
       code
          argcount  : 0
-         nlocals   : 4
+         nlocals   : 5
          stacksize : 5
          flags     : 3
          code
-            0x9700740100000000000000000000a6000000ab00000000000000000001
-            007403000000000000000000006a0200000000000000006401ac02a60100
-            00ab0100000000000000007d007c00a00300000000000000000000000000
-            00000000000000640364046405ac06a6030000ab03000000000000000001
-            007c00a0040000000000000000000000000000000000000000a6000000ab
-            0000000000000000007d016407a005000000000000000000000000000000
-            00000000007c016a060000000000000000a6010000ab0100000000000000
-            007d02740f00000000000000000000a6000000ab0000000000000000007d
-            037c03a00800000000000000000000000000000000000000007c02a60100
-            00ab010000000000000000010064005300
-          10           0 RESUME                   0
+            0x9700740100000000000000000000a6000000ab0000000000000000007d
+            007c00a0010000000000000000000000000000000000000000a6000000ab
+            00000000000000000001007405000000000000000000006a030000000000
+            0000006401ac02a6010000ab0100000000000000007d017c01a004000000
+            0000000000000000000000000000000000640364046405ac06a6030000ab
+            03000000000000000001007c01a005000000000000000000000000000000
+            0000000000a6000000ab0000000000000000007d026407a0060000000000
+            0000000000000000000000000000007c026a070000000000000000a60100
+            00ab0100000000000000007d03741100000000000000000000a6000000ab
+            0000000000000000007d047c04a009000000000000000000000000000000
+            00000000007c03a6010000ab010000000000000000010064005300
+          11           0 RESUME                   0
          
-          12           2 LOAD_GLOBAL              1 (NULL + ensure)
+          13           2 LOAD_GLOBAL              1 (NULL + UserConfigService)
                       14 PRECALL                  0
                       18 CALL                     0
-                      28 POP_TOP
+                      28 STORE_FAST               0 (user_config_service)
          
-          13          30 LOAD_GLOBAL              3 (NULL + argparse)
-                      42 LOAD_ATTR                2 (ArgumentParser)
-                      52 LOAD_CONST               1 ('AI Natural Language Interface for running shell commands')
-                      54 KW_NAMES                 2
-                      56 PRECALL                  1
-                      60 CALL                     1
-                      70 STORE_FAST               0 (parser)
-         
-          14          72 LOAD_FAST                0 (parser)
-                      74 LOAD_METHOD              3 (add_argument)
-                      96 LOAD_CONST               3 ('question')
-                      98 LOAD_CONST               4 ('+')
-                     100 LOAD_CONST               5 ('question or instruction to turn into a shell command')
-                     102 KW_NAMES                 6
-                     104 PRECALL                  3
-                     108 CALL                     3
-                     118 POP_TOP
-         
-          15         120 LOAD_FAST                0 (parser)
-                     122 LOAD_METHOD              4 (parse_args)
-                     144 PRECALL                  0
-                     148 CALL                     0
-                     158 STORE_FAST               1 (args)
-         
-          16         160 LOAD_CONST               7 (' ')
-                     162 LOAD_METHOD              5 (join)
-                     184 LOAD_FAST                1 (args)
-                     186 LOAD_ATTR                6 (question)
-                     196 PRECALL                  1
-                     200 CALL                     1
-                     210 STORE_FAST               2 (user_input)
-         
-          17         212 LOAD_GLOBAL             15 (NULL + UserCommandService)
-                     224 PRECALL                  0
-                     228 CALL                     0
-                     238 STORE_FAST               3 (user_command_service)
-         
-          18         240 LOAD_FAST                3 (user_command_service)
-                     242 LOAD_METHOD              8 (handle_request)
-                     264 LOAD_FAST                2 (user_input)
-                     266 PRECALL                  1
-                     270 CALL                     1
-                     280 POP_TOP
-                     282 LOAD_CONST               0 (None)
-                     284 RETURN_VALUE
+          14          30 LOAD_FAST                0 (user_config_service)
+                      32 LOAD_METHOD              1 (ensure_needed_configs_are_set)
+                      54 PRECALL                  0
+                      58 CALL                     0
+                      68 POP_TOP
+         
+          16          70 LOAD_GLOBAL              5 (NULL + argparse)
+                      82 LOAD_ATTR                3 (ArgumentParser)
+                      92 LOAD_CONST               1 ('AI Natural Language Interface for running shell commands')
+                      94 KW_NAMES                 2
+                      96 PRECALL                  1
+                     100 CALL                     1
+                     110 STORE_FAST               1 (parser)
+         
+          17         112 LOAD_FAST                1 (parser)
+                     114 LOAD_METHOD              4 (add_argument)
+                     136 LOAD_CONST               3 ('question')
+                     138 LOAD_CONST               4 ('+')
+                     140 LOAD_CONST               5 ('question or instruction to turn into a shell command')
+                     142 KW_NAMES                 6
+                     144 PRECALL                  3
+                     148 CALL                     3
+                     158 POP_TOP
+         
+          18         160 LOAD_FAST                1 (parser)
+                     162 LOAD_METHOD              5 (parse_args)
+                     184 PRECALL                  0
+                     188 CALL                     0
+                     198 STORE_FAST               2 (args)
+         
+          19         200 LOAD_CONST               7 (' ')
+                     202 LOAD_METHOD              6 (join)
+                     224 LOAD_FAST                2 (args)
+                     226 LOAD_ATTR                7 (question)
+                     236 PRECALL                  1
+                     240 CALL                     1
+                     250 STORE_FAST               3 (user_input)
+         
+          20         252 LOAD_GLOBAL             17 (NULL + UserCommandService)
+                     264 PRECALL                  0
+                     268 CALL                     0
+                     278 STORE_FAST               4 (user_command_service)
+         
+          21         280 LOAD_FAST                4 (user_command_service)
+                     282 LOAD_METHOD              9 (handle_request)
+                     304 LOAD_FAST                3 (user_input)
+                     306 PRECALL                  1
+                     310 CALL                     1
+                     320 POP_TOP
+                     322 LOAD_CONST               0 (None)
+                     324 RETURN_VALUE
          consts
             None
             'AI Natural Language Interface for running shell commands'
             ('description',)
             'question'
             '+'
             'question or instruction to turn into a shell command'
             ('nargs', 'help')
             ' '
-         names      ('ensure', 'argparse', 'ArgumentParser', 'add_argument', 'parse_args', 'join', 'question', 'UserCommandService', 'handle_request')
-         varnames   ('parser', 'args', 'user_input', 'user_command_service')
+         names      ('UserConfigService', 'ensure_needed_configs_are_set', 'argparse', 'ArgumentParser', 'add_argument', 'parse_args', 'join', 'question', 'UserCommandService', 'handle_request')
+         varnames   ('user_config_service', 'parser', 'args', 'user_input', 'user_command_service')
          freevars   ()
          cellvars   ()
          filename   '/Users/jason/Documents/dev/eras/eras/main.py'
          name       'main'
-         firstlineno 10
-         lnotab 0x02021c012a013001280134011c01
+         firstlineno 11
+         lnotab 0x02021c0128022a013001280134011c01
       '__main__'
-   names      ('argparse', 'sys', 'os', 'dotenv', 'load_dotenv', 'eras.services.user_command_service', 'UserCommandService', 'eras.config.post_install', 'ensure', 'main', '__name__')
+   names      ('argparse', 'sys', 'os', 'dotenv', 'load_dotenv', 'eras.services.user_command_service', 'UserCommandService', 'eras.services.user_config_service', 'UserConfigService', 'main', '__name__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jason/Documents/dev/eras/eras/main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010801080108010c0114020c010c02060b0c0118ff
+   lnotab 0x00ff02010801080108010c0114020c010c03060d0c0118ff
```

### Comparing `eras-0.3.6/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc` & `eras-0.3.7/eras/agents/__pycache__/llama_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc` & `eras-0.3.7/eras/agents/__pycache__/llama_terminal_command_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc` & `eras-0.3.7/eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc` & `eras-0.3.7/eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/agents/__pycache__/simple_llm.cpython-311.pyc` & `eras-0.3.7/eras/agents/__pycache__/simple_llm.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x42b44e66 (Thu May 23 03:13:06 2024 UTC)
-files sz: 1798
+moddate:  0x15775266 (Sat May 25 23:41:09 2024 UTC)
+files sz: 1822
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -137,23 +137,23 @@
                   0164049c0267026406ac07a6030000ab0300000000000000007d057c0544
                   005d267d067c066a0700000000000000006408190000000000000000006a
                   0800000000000000006a0900000000000000007d077c07810b02007c027c
                   07a6010000ab01000000000000000001008c2702007c03a6000000ab0000
                   00000000000000010064005300
                 13           0 RESUME                   0
                
-                16           2 LOAD_CONST               1 ('\n        You are friendly AI assistant that runs in a terminal.  Format all responses you provide for the terminal for the operating system ')
+                16           2 LOAD_CONST               1 ('\n        You are friendly AI assistant that runs in a terminal for the operating system ')
                
                 17           4 LOAD_GLOBAL              1 (NULL + config)
                             16 LOAD_ATTR                1 (get_user_operating_system)
                             26 PRECALL                  0
                             30 CALL                     0
                
                 16          40 FORMAT_VALUE             0
-                            42 LOAD_CONST               2 ('.\n        Your responses are streamed to the terminal via python print statements.\n        ')
+                            42 LOAD_CONST               2 ('.  \n        All responses you provide will be shown in a terminal.  You are an expert in ensuring your response text is plain text, and does not use markdown.\n        ')
                             44 BUILD_STRING             3
                             46 STORE_FAST               4 (system_message)
                
                 20          48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                2 (client)
                             60 LOAD_ATTR                3 (chat)
                             70 LOAD_ATTR                4 (completions)
@@ -212,16 +212,16 @@
                            262 PRECALL                  0
                            266 CALL                     0
                            276 POP_TOP
                            278 LOAD_CONST               0 (None)
                            280 RETURN_VALUE
                consts
                   None
-                  '\n        You are friendly AI assistant that runs in a terminal.  Format all responses you provide for the terminal for the operating system '
-                  '.\n        Your responses are streamed to the terminal via python print statements.\n        '
+                  '\n        You are friendly AI assistant that runs in a terminal for the operating system '
+                  '.  \n        All responses you provide will be shown in a terminal.  You are an expert in ensuring your response text is plain text, and does not use markdown.\n        '
                   'system'
                   ('role', 'content')
                   'user'
                   True
                   ('model', 'messages', 'stream')
                   0
                names      ('config', 'get_user_operating_system', 'client', 'chat', 'completions', 'create', 'get_model_name', 'choices', 'delta', 'content')
```

### Comparing `eras-0.3.6/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc` & `eras-0.3.7/eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc` & `eras-0.3.7/eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/agents/llama_functions_agent.py` & `eras-0.3.7/eras/agents/llama_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/agents/llama_terminal_command_functions_agent.py` & `eras-0.3.7/eras/agents/llama_terminal_command_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/agents/llm_functions_agent.py` & `eras-0.3.7/eras/agents/llm_functions_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/agents/simple_llm.py` & `eras-0.3.7/eras/agents/simple_llm.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
         self.client = openai_client
 
     def stream_inference(self, prompt: str, handle_on_text_received: LLMTextReceivedCallable,
                          handle_response_complete: LLMResponseCompletedCallable) -> None:
         # start_time_seconds = time.time()
         system_message = f"""
-        You are friendly AI assistant that runs in a terminal.  Format all responses you provide for the terminal for the operating system {config.get_user_operating_system()}.
-        Your responses are streamed to the terminal via python print statements.
+        You are friendly AI assistant that runs in a terminal for the operating system {config.get_user_operating_system()}.  
+        All responses you provide will be shown in a terminal.  You are an expert in ensuring your response text is plain text, and does not use markdown.
         """
         completion = self.client.chat.completions.create(
             model=config.get_model_name(),
             messages=[
                 {"role": "system", "content": system_message},
                 {"role": "user", "content": prompt}
             ],
```

### Comparing `eras-0.3.6/eras/agents/terminal_llama_agent.py` & `eras-0.3.7/eras/agents/terminal_llama_agent.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/config/__pycache__/config.cpython-39.pyc` & `eras-0.3.7/eras/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/config/config.py` & `eras-0.3.7/eras/config/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
 import platform
+from eras.models.constants import OPENAI_MODEL_DEFAULT, ERAS_MODEL_ENV_VAR_NAME, ERAS_OPENAI_KEY_ENV_VAR_NAME, ERAS_BASE_URL_ENV_VAR_NAME
 
 class Config:
     _instance = None
 
     def __new__(cls):
         if cls._instance is None:
             cls._instance = super(Config, cls).__new__(cls)
         return cls._instance
 
-    def get_open_ai_key(self):
-        return os.getenv('OPEN_AI_KEY')
-
     def get_eras_open_ai_key(self):
-        return os.getenv('ERAS_OPENAI_KEY')
+        return os.getenv(ERAS_OPENAI_KEY_ENV_VAR_NAME)
 
     def get_eras_base_url(self):
-        return os.getenv('ERAS_BASE_URL')
+        base_url = os.getenv(ERAS_BASE_URL_ENV_VAR_NAME)
+        if base_url == "":
+            return None
+        return os.getenv(ERAS_BASE_URL_ENV_VAR_NAME)
 
     def get_model_name(self):
-        return "gpt-3.5-turbo"
+        return os.getenv(ERAS_MODEL_ENV_VAR_NAME, OPENAI_MODEL_DEFAULT)
 
     def get_user_operating_system(self):
         # return "System: Mac , macOS: Monterey, osVersion: 12.4"
         os_name = platform.system()
         os_version = platform.version()
         os_release = platform.release()
```

### Comparing `eras-0.3.6/eras/config/post_install.py` & `eras-0.3.7/eras/utils/env_vars_and_profile_files.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,75 @@
 import os
 import sys
 import subprocess
-
-def alias_exists(alias_name):
-    home = os.path.expanduser("~")
-    shell_config_files = [".bashrc", ".zshrc", ".bash_profile"]
-
-    for config_file in shell_config_files:
-        config_path = os.path.join(home, config_file)
-        if os.path.exists(config_path):
-            with open(config_path, "r") as file:
-                if alias_name in file.read():
-                    return True
-    return False
+import re
 
 def env_var_exists(var_name):
     if os.name == 'nt':  # Windows
         return os.getenv(var_name) is not None
     else:  # Unix-based systems
         home = os.path.expanduser("~")
         shell_config_files = [".bashrc", ".zshrc", ".bash_profile"]
 
         for config_file in shell_config_files:
             config_path = os.path.join(home, config_file)
             if os.path.exists(config_path):
                 with open(config_path, "r") as file:
+                    # print(file.read())
+                    # print(f'{var_name} is in file? : {var_name in file.read()}')
                     if var_name in file.read():
+                        # print(file.read())
+                        # print(f'{var_name} is in {file.read()} {config_path}')
                         return True
         return False
 
-# def refresh_windows_environment_variables():
-#     # Refresh user environment variables
-#     user_vars = os.popen('powershell -Command "[System.Environment]::GetEnvironmentVariables(\'User\')"').read()
-#     for line in user_vars.splitlines():
-#         if '=' in line:
-#             key, value = line.split('=', 1)
-#             os.environ[key.strip()] = value.strip()
-#
-#     # Refresh system environment variables
-#     system_vars = os.popen('powershell -Command "[System.Environment]::GetEnvironmentVariables(\'Machine\')"').read()
-#     for line in system_vars.splitlines():
-#         if '=' in line:
-#             key, value = line.split('=', 1)
-#             os.environ[key.strip()] = value.strip()
+def set_env_var(env_var_name, value):
+    env_var_command = f"{env_var_name}={value}"
+    print(f"setting env var: {env_var_command}")
+    os.environ[env_var_name] = value
+    set_env_var_to_shell(env_var_command)
 
-def add_env_var_to_shell(env_var_command):
+def set_env_var_to_shell(env_var_command):
     if os.name == 'nt':  # Windows
         print('setting windows shell env var')
         var_name, var_value = env_var_command.split('=', 1)
         os.system(f'setx {var_name} {var_value}')
-        # Set the environment variable persistently using setx
-        # subprocess.run(['setx', var_name, var_value], check=True)
 
     else:  # Unix-based systems
         home = os.path.expanduser("~")
         shell_config_files = [".bashrc", ".zshrc", ".bash_profile"]
+        var_name, var_value = env_var_command.split('=', 1)
+        export_command = f"export {env_var_command}"
 
         for config_file in shell_config_files:
             config_path = os.path.join(home, config_file)
             if os.path.exists(config_path):
-                with open(config_path, "a") as file:
-                    file.write(f"\nexport {env_var_command}\n")
+                with open(config_path, "r") as file:
+                    lines = file.readlines()
+
+                with open(config_path, "w") as file:
+                    var_found = False
+                    for line in lines:
+                        if re.match(f"^export {var_name}=", line):
+                            file.write(f"{export_command}\n")
+                            var_found = True
+                        else:
+                            file.write(line)
+                    if not var_found:
+                        file.write(f"\n{export_command}\n")
 
 def ensure():
     if not env_var_exists("ERAS_OPENAI_KEY"):
         openai_key = input("Please enter your OpenAI API key (ERAS_OPENAI_KEY): ").strip()
         if not openai_key:
             print("Error: OpenAI API key cannot be empty.")
             sys.exit(1)
         env_var_command = f"ERAS_OPENAI_KEY={openai_key}"
         os.environ['ERAS_OPENAI_KEY'] = openai_key
-        add_env_var_to_shell(env_var_command)
+        set_env_var_to_shell(env_var_command)
         print("Environment variable 'ERAS_OPENAI_KEY' added to environment.")
 
         if os.name != 'nt':  # Unix-based systems
             reload_profile(get_profile_file())
         else:
             print('======= PLEASE CLOSE THIS TERMINAL WINDOW AND OPEN A NEW ONE =========')
 
@@ -88,23 +83,23 @@
         elif 'bash' in shell:
             bash_profile = os.path.expanduser('~/.bash_profile')
             if os.path.exists(bash_profile):
                 return bash_profile
             else:
                 return os.path.expanduser('~/.bashrc')
         else:
-            raise ValueError("Unsupported shell type")
+            print("Unsupported shell type.  Close this terminal windows and open a new one.")
 
 def reload_profile(profile_file):
     if os.name != 'nt':  # Unix-based systems
         shell = os.environ.get('SHELL', '')
         if 'zsh' in shell:
-            subprocess.run(['zsh', '-c', f'source {profile_file}'], check=True)
+            os.execvp('zsh', ['zsh', '-c', f'source {profile_file} && exec zsh'])
         elif 'bash' in shell:
-            subprocess.run(['bash', '-c', f'source {profile_file}'], check=True)
+            os.execvp('bash', ['bash', '-c', f'source {profile_file} && exec bash'])
         else:
             print(f"Please manually source your profile file: {profile_file}")
     else:
         print("Please restart your Command Prompt or PowerShell session to apply the changes.")
 
 if __name__ == "__main__":
     ensure()
```

### Comparing `eras-0.3.6/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc` & `eras-0.3.7/eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/decorators/chatgpt_tool_data.py` & `eras-0.3.7/eras/decorators/chatgpt_tool_data.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/factories/__pycache__/function_details_factory.cpython-311.pyc` & `eras-0.3.7/eras/factories/__pycache__/function_details_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/factories/__pycache__/function_details_factory.cpython-39.pyc` & `eras-0.3.7/eras/factories/__pycache__/function_details_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/factories/__pycache__/message_factory.cpython-311.pyc` & `eras-0.3.7/eras/factories/__pycache__/message_factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/factories/__pycache__/message_factory.cpython-39.pyc` & `eras-0.3.7/eras/factories/__pycache__/message_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/factories/function_details_factory.py` & `eras-0.3.7/eras/factories/function_details_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/factories/message_factory.py` & `eras-0.3.7/eras/factories/message_factory.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/__pycache__/conversation.cpython-311.pyc` & `eras-0.3.7/eras/models/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/__pycache__/conversation.cpython-39.pyc` & `eras-0.3.7/eras/models/__pycache__/conversation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/__pycache__/function_details.cpython-311.pyc` & `eras-0.3.7/eras/models/__pycache__/function_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/__pycache__/function_details.cpython-39.pyc` & `eras-0.3.7/eras/models/__pycache__/function_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/__pycache__/message.cpython-311.pyc` & `eras-0.3.7/eras/models/__pycache__/message.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/__pycache__/message.cpython-39.pyc` & `eras-0.3.7/eras/models/__pycache__/message.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/conversation.py` & `eras-0.3.7/eras/models/conversation.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/function_details.py` & `eras-0.3.7/eras/models/function_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/message.py` & `eras-0.3.7/eras/models/message.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/models/transaction.py` & `eras-0.3.7/eras/models/transaction.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/run.ipynb` & `eras-0.3.7/eras/run.ipynb`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/__pycache__/shell_command_service.cpython-311.pyc` & `eras-0.3.7/eras/services/__pycache__/shell_command_service.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/__pycache__/shell_command_service.cpython-39.pyc` & `eras-0.3.7/eras/services/__pycache__/shell_command_service.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/__pycache__/user_command_service.cpython-311.pyc` & `eras-0.3.7/eras/services/__pycache__/user_command_service.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0xfab44e66 (Thu May 23 03:16:10 2024 UTC)
-files sz: 1846
+moddate:  0x826e5266 (Sat May 25 23:04:34 2024 UTC)
+files sz: 2189
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
-      045a040100640064046c056d065a060100640064016c075a070200470064
-      0584006406a6020000ab0200000000000000005a0864015300
+      045a040100640064046c056d065a060100640064016c075a07640064056c
+      086d095a090100640064016c0a5a0a02004700640684006407a6020000ab
+      0200000000000000005a0b64015300
      0           0 RESUME                   0
    
      2           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
    
@@ -39,298 +40,356 @@
                 44 POP_TOP
    
      7          46 LOAD_CONST               0 (0)
                 48 LOAD_CONST               1 (None)
                 50 IMPORT_NAME              7 (openai)
                 52 STORE_NAME               7 (openai)
    
-     9          54 PUSH_NULL
-                56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               5 (<code object UserCommandService, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 9>)
-                60 MAKE_FUNCTION            0
-                62 LOAD_CONST               6 ('UserCommandService')
-                64 PRECALL                  2
-                68 CALL                     2
-                78 STORE_NAME               8 (UserCommandService)
-                80 LOAD_CONST               1 (None)
-                82 RETURN_VALUE
+     9          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               5 (('UserConfigService',))
+                58 IMPORT_NAME              8 (eras.services.user_config_service)
+                60 IMPORT_FROM              9 (UserConfigService)
+                62 STORE_NAME               9 (UserConfigService)
+                64 POP_TOP
+   
+    10          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               1 (None)
+                70 IMPORT_NAME             10 (httpx)
+                72 STORE_NAME              10 (httpx)
+   
+    12          74 PUSH_NULL
+                76 LOAD_BUILD_CLASS
+                78 LOAD_CONST               6 (<code object UserCommandService, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 12>)
+                80 MAKE_FUNCTION            0
+                82 LOAD_CONST               7 ('UserCommandService')
+                84 PRECALL                  2
+                88 CALL                     2
+                98 STORE_NAME              11 (UserCommandService)
+               100 LOAD_CONST               1 (None)
+               102 RETURN_VALUE
    consts
       0
       None
       ('SimpleLLM',)
       ('config',)
       ('ShellCommandService',)
+      ('UserConfigService',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640265046602640384045a0564
-            0484005a06640584005a07640684005a0864075300
-           9           0 RESUME                   0
+            0484005a06640584005a07640684005a08640784005a0964085300
+          12           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('UserCommandService')
                        8 STORE_NAME               2 (__qualname__)
          
-          10          10 LOAD_CONST               1 (<code object __init__, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 10>)
+          13          10 LOAD_CONST               1 (<code object __init__, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 13>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          21          16 LOAD_CONST               2 ('user_input')
+          22          16 LOAD_CONST               2 ('user_input')
                       18 LOAD_NAME                4 (str)
                       20 BUILD_TUPLE              2
-                      22 LOAD_CONST               3 (<code object handle_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 21>)
+                      22 LOAD_CONST               3 (<code object handle_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 22>)
                       24 MAKE_FUNCTION            4 (annotations)
                       26 STORE_NAME               5 (handle_request)
          
-          29          28 LOAD_CONST               4 (<code object handle_help_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 29>)
+          32          28 LOAD_CONST               4 (<code object handle_help_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 32>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (handle_help_request)
          
-          38          34 LOAD_CONST               5 (<code object handle_chat_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 38>)
+          40          34 LOAD_CONST               5 (<code object handle_chat_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 40>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               7 (handle_chat_request)
          
-          51          40 LOAD_CONST               6 (<code object handle_shell_nli_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 51>)
+          53          40 LOAD_CONST               6 (<code object handle_shell_nli_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 53>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               8 (handle_shell_nli_request)
-                      46 LOAD_CONST               7 (None)
-                      48 RETURN_VALUE
+         
+          56          46 LOAD_CONST               7 (<code object handle_config_request, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 56>)
+                      48 MAKE_FUNCTION            0
+                      50 STORE_NAME               9 (handle_config_request)
+                      52 LOAD_CONST               8 (None)
+                      54 RETURN_VALUE
          consts
             'UserCommandService'
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 4
+               stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000006a030000000000000000a6000000ab0000000000000000
-                  00ac01a6010000ab0100000000000000007c005f04000000000000000074
-                  0b000000000000000000007c006a040000000000000000a6010000ab0100
-                  000000000000007c005f060000000000000000740f000000000000000000
-                  007c006a040000000000000000a6010000ab0100000000000000007c005f
-                  08000000000000000064005300
-                10           0 RESUME                   0
+                  007405000000000000000000006a040000000000000000a6000000ab0000
+                  00000000000000ac01a6020000ab0200000000000000007c005f05000000
+                  0000000000740d000000000000000000007c006a050000000000000000a6
+                  010000ab0100000000000000007c005f0700000000000000007411000000
+                  000000000000007c006a050000000000000000a6010000ab010000000000
+                  0000007c005f090000000000000000741500000000000000000000a60000
+                  00ab0000000000000000007c005f0b000000000000000064005300
+                13           0 RESUME                   0
                
-                11           2 LOAD_GLOBAL              1 (NULL + openai)
+                14           2 LOAD_GLOBAL              1 (NULL + openai)
                             14 LOAD_ATTR                1 (OpenAI)
                
-                13          24 LOAD_GLOBAL              5 (NULL + config)
-                            36 LOAD_ATTR                3 (get_eras_open_ai_key)
+                15          24 LOAD_GLOBAL              5 (NULL + config)
+                            36 LOAD_ATTR                3 (get_eras_base_url)
                             46 PRECALL                  0
                             50 CALL                     0
                
-                11          60 KW_NAMES                 1
-                            62 PRECALL                  1
-                            66 CALL                     1
-                            76 LOAD_FAST                0 (self)
-                            78 STORE_ATTR               4 (openai_client)
-               
-                16          88 LOAD_GLOBAL             11 (NULL + ShellCommandService)
-                           100 LOAD_FAST                0 (self)
-                           102 LOAD_ATTR                4 (openai_client)
-                           112 PRECALL                  1
-                           116 CALL                     1
-                           126 LOAD_FAST                0 (self)
-                           128 STORE_ATTR               6 (shell_command_service)
-               
-                17         138 LOAD_GLOBAL             15 (NULL + SimpleLLM)
-                           150 LOAD_FAST                0 (self)
-                           152 LOAD_ATTR                4 (openai_client)
-                           162 PRECALL                  1
-                           166 CALL                     1
-                           176 LOAD_FAST                0 (self)
-                           178 STORE_ATTR               8 (simple_llm)
-                           188 LOAD_CONST               0 (None)
-                           190 RETURN_VALUE
+                16          60 LOAD_GLOBAL              5 (NULL + config)
+                            72 LOAD_ATTR                4 (get_eras_open_ai_key)
+                            82 PRECALL                  0
+                            86 CALL                     0
+               
+                14          96 KW_NAMES                 1
+                            98 PRECALL                  2
+                           102 CALL                     2
+                           112 LOAD_FAST                0 (self)
+                           114 STORE_ATTR               5 (openai_client)
+               
+                18         124 LOAD_GLOBAL             13 (NULL + ShellCommandService)
+                           136 LOAD_FAST                0 (self)
+                           138 LOAD_ATTR                5 (openai_client)
+                           148 PRECALL                  1
+                           152 CALL                     1
+                           162 LOAD_FAST                0 (self)
+                           164 STORE_ATTR               7 (shell_command_service)
+               
+                19         174 LOAD_GLOBAL             17 (NULL + SimpleLLM)
+                           186 LOAD_FAST                0 (self)
+                           188 LOAD_ATTR                5 (openai_client)
+                           198 PRECALL                  1
+                           202 CALL                     1
+                           212 LOAD_FAST                0 (self)
+                           214 STORE_ATTR               9 (simple_llm)
+               
+                20         224 LOAD_GLOBAL             21 (NULL + UserConfigService)
+                           236 PRECALL                  0
+                           240 CALL                     0
+                           250 LOAD_FAST                0 (self)
+                           252 STORE_ATTR              11 (user_config_service)
+                           262 LOAD_CONST               0 (None)
+                           264 RETURN_VALUE
                consts
                   None
-                  ('api_key',)
-               names      ('openai', 'OpenAI', 'config', 'get_eras_open_ai_key', 'openai_client', 'ShellCommandService', 'shell_command_service', 'SimpleLLM', 'simple_llm')
+                  ('base_url', 'api_key')
+               names      ('openai', 'OpenAI', 'config', 'get_eras_base_url', 'get_eras_open_ai_key', 'openai_client', 'ShellCommandService', 'shell_command_service', 'SimpleLLM', 'simple_llm', 'UserConfigService', 'user_config_service')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       '__init__'
-               firstlineno 10
-               lnotab 0x0201160224fe1c053201
+               firstlineno 13
+               lnotab 0x02011601240124fe1c0432013201
             'user_input'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c01a00000000000000000000000000000000000000000006401a6
                   010000ab01000000000000000072177c00a0010000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000000100640053
                   007c01a00000000000000000000000000000000000000000006402a60100
                   00ab01000000000000000072177c00a00200000000000000000000000000
                   000000000000007c01a6010000ab0100000000000000000100640053007c
-                  00a00300000000000000000000000000000000000000007c01a6010000ab
-                  010000000000000000010064005300
-                21           0 RESUME                   0
+                  01a00000000000000000000000000000000000000000006403a6010000ab
+                  01000000000000000072177c00a003000000000000000000000000000000
+                  00000000007c01a6010000ab0100000000000000000100640053007c00a0
+                  0400000000000000000000000000000000000000007c01a6010000ab0100
+                  00000000000000010064005300
+                22           0 RESUME                   0
                
-                22           2 LOAD_FAST                1 (user_input)
+                23           2 LOAD_FAST                1 (user_input)
                              4 LOAD_METHOD              0 (startswith)
                             26 LOAD_CONST               1 ('/help')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    23 (to 90)
                
-                23          44 LOAD_FAST                0 (self)
+                24          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (handle_help_request)
                             68 LOAD_FAST                1 (user_input)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 POP_TOP
                             86 LOAD_CONST               0 (None)
                             88 RETURN_VALUE
                
-                24     >>   90 LOAD_FAST                1 (user_input)
+                25     >>   90 LOAD_FAST                1 (user_input)
                             92 LOAD_METHOD              0 (startswith)
                            114 LOAD_CONST               2 ('/chat')
                            116 PRECALL                  1
                            120 CALL                     1
                            130 POP_JUMP_FORWARD_IF_FALSE    23 (to 178)
                
-                25         132 LOAD_FAST                0 (self)
+                26         132 LOAD_FAST                0 (self)
                            134 LOAD_METHOD              2 (handle_chat_request)
                            156 LOAD_FAST                1 (user_input)
                            158 PRECALL                  1
                            162 CALL                     1
                            172 POP_TOP
                            174 LOAD_CONST               0 (None)
                            176 RETURN_VALUE
                
-                27     >>  178 LOAD_FAST                0 (self)
-                           180 LOAD_METHOD              3 (handle_shell_nli_request)
-                           202 LOAD_FAST                1 (user_input)
+                27     >>  178 LOAD_FAST                1 (user_input)
+                           180 LOAD_METHOD              0 (startswith)
+                           202 LOAD_CONST               3 ('/config')
                            204 PRECALL                  1
                            208 CALL                     1
-                           218 POP_TOP
-                           220 LOAD_CONST               0 (None)
-                           222 RETURN_VALUE
+                           218 POP_JUMP_FORWARD_IF_FALSE    23 (to 266)
+               
+                28         220 LOAD_FAST                0 (self)
+                           222 LOAD_METHOD              3 (handle_config_request)
+                           244 LOAD_FAST                1 (user_input)
+                           246 PRECALL                  1
+                           250 CALL                     1
+                           260 POP_TOP
+                           262 LOAD_CONST               0 (None)
+                           264 RETURN_VALUE
+               
+                30     >>  266 LOAD_FAST                0 (self)
+                           268 LOAD_METHOD              4 (handle_shell_nli_request)
+                           290 LOAD_FAST                1 (user_input)
+                           292 PRECALL                  1
+                           296 CALL                     1
+                           306 POP_TOP
+                           308 LOAD_CONST               0 (None)
+                           310 RETURN_VALUE
                consts
                   None
                   '/help'
                   '/chat'
-               names      ('startswith', 'handle_help_request', 'handle_chat_request', 'handle_shell_nli_request')
+                  '/config'
+               names      ('startswith', 'handle_help_request', 'handle_chat_request', 'handle_config_request', 'handle_shell_nli_request')
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_request'
-               firstlineno 21
-               lnotab 0x02012a012e012a012e02
+               firstlineno 22
+               lnotab 0x02012a012e012a012e012a012e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000006401a6010000ab0100000000000000
                   0001007401000000000000000000006402a6010000ab0100000000000000
                   0001007401000000000000000000006403a6010000ab0100000000000000
                   0001007401000000000000000000006404a6010000ab0100000000000000
                   0001007401000000000000000000006405a6010000ab0100000000000000
+                  0001007401000000000000000000006406a6010000ab0100000000000000
                   00010064005300
-                29           0 RESUME                   0
+                32           0 RESUME                   0
                
-                30           2 LOAD_GLOBAL              1 (NULL + print)
+                33           2 LOAD_GLOBAL              1 (NULL + print)
                             14 LOAD_CONST               1 ('Welcome to ERAS - Easily Runnable AI Shell')
                             16 PRECALL                  1
                             20 CALL                     1
                             30 POP_TOP
                
-                31          32 LOAD_GLOBAL              1 (NULL + print)
+                34          32 LOAD_GLOBAL              1 (NULL + print)
                             44 LOAD_CONST               2 ('Commands: ==============================================')
                             46 PRECALL                  1
                             50 CALL                     1
                             60 POP_TOP
                
-                32          62 LOAD_GLOBAL              1 (NULL + print)
+                35          62 LOAD_GLOBAL              1 (NULL + print)
                             74 LOAD_CONST               3 ('{defualt usage} - Natural Languge Interface for running commands. e.g. eras how do I list all files in a directory -> %ls')
                             76 PRECALL                  1
                             80 CALL                     1
                             90 POP_TOP
                
-                33          92 LOAD_GLOBAL              1 (NULL + print)
+                36          92 LOAD_GLOBAL              1 (NULL + print)
                            104 LOAD_CONST               4 ('/help - get info about commands')
                            106 PRECALL                  1
                            110 CALL                     1
                            120 POP_TOP
                
-                34         122 LOAD_GLOBAL              1 (NULL + print)
+                37         122 LOAD_GLOBAL              1 (NULL + print)
                            134 LOAD_CONST               5 ('/chat - ask the LLM a question about anything. e.g. /chat tell me about quantum physics')
                            136 PRECALL                  1
                            140 CALL                     1
                            150 POP_TOP
-                           152 LOAD_CONST               0 (None)
-                           154 RETURN_VALUE
+               
+                38         152 LOAD_GLOBAL              1 (NULL + print)
+                           164 LOAD_CONST               6 ('/conf - configure eras. urls, keys, etc')
+                           166 PRECALL                  1
+                           170 CALL                     1
+                           180 POP_TOP
+                           182 LOAD_CONST               0 (None)
+                           184 RETURN_VALUE
                consts
                   None
                   'Welcome to ERAS - Easily Runnable AI Shell'
                   'Commands: =============================================='
                   '{defualt usage} - Natural Languge Interface for running commands. e.g. eras how do I list all files in a directory -> %ls'
                   '/help - get info about commands'
                   '/chat - ask the LLM a question about anything. e.g. /chat tell me about quantum physics'
+                  '/conf - configure eras. urls, keys, etc'
                names      ('print',)
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_help_request'
-               firstlineno 29
-               lnotab 0x02011e011e011e011e01
+               firstlineno 32
+               lnotab 0x02011e011e011e011e011e01
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
-                38           0 RESUME                   0
+                40           0 RESUME                   0
                
-                39           2 LOAD_GLOBAL              1 (NULL + re)
+                41           2 LOAD_GLOBAL              1 (NULL + re)
                             14 LOAD_ATTR                1 (match)
                             24 LOAD_CONST               1 ('^/chat\\s+(.*)')
                             26 LOAD_FAST                1 (user_input)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 STORE_FAST               2 (match)
                
-                40          44 LOAD_FAST                2 (match)
+                42          44 LOAD_FAST                2 (match)
                             46 POP_JUMP_FORWARD_IF_FALSE    21 (to 90)
                             48 LOAD_FAST                2 (match)
                             50 LOAD_METHOD              2 (group)
                             72 LOAD_CONST               2 (1)
                             74 PRECALL                  1
                             78 CALL                     1
                             88 JUMP_FORWARD             1 (to 92)
                        >>   90 LOAD_CONST               0 (None)
                        >>   92 STORE_FAST               3 (prompt)
                
-                42          94 LOAD_CONST               3 (<code object handle_text_received, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 42>)
+                44          94 LOAD_CONST               3 (<code object handle_text_received, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 44>)
                             96 MAKE_FUNCTION            0
                             98 STORE_FAST               4 (handle_text_received)
                
-                45         100 LOAD_CONST               4 (<code object handle_response_complete, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 45>)
+                47         100 LOAD_CONST               4 (<code object handle_response_complete, file "/Users/jason/Documents/dev/eras/eras/services/user_command_service.py", line 47>)
                            102 MAKE_FUNCTION            0
                            104 STORE_FAST               5 (handle_response_complete)
                
-                48         106 LOAD_FAST                0 (self)
+                50         106 LOAD_FAST                0 (self)
                            108 LOAD_ATTR                3 (simple_llm)
                            118 LOAD_METHOD              4 (stream_inference)
                            140 LOAD_FAST                3 (prompt)
                            142 LOAD_FAST                4 (handle_text_received)
                            144 LOAD_FAST                5 (handle_response_complete)
                            146 PRECALL                  3
                            150 CALL                     3
@@ -345,17 +404,17 @@
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 4
                      flags     : 19
                      code
                         0x97007401000000000000000000007c006401ac02a6020000ab02000000
                         0000000000010064005300
-                      42           0 RESUME                   0
+                      44           0 RESUME                   0
                      
-                      43           2 LOAD_GLOBAL              1 (NULL + print)
+                      45           2 LOAD_GLOBAL              1 (NULL + print)
                                   14 LOAD_FAST                0 (text)
                                   16 LOAD_CONST               1 ('')
                                   18 KW_NAMES                 2
                                   20 PRECALL                  2
                                   24 CALL                     2
                                   34 POP_TOP
                                   36 LOAD_CONST               0 (None)
@@ -366,61 +425,61 @@
                         ('end',)
                      names      ('print',)
                      varnames   ('text',)
                      freevars   ()
                      cellvars   ()
                      filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                      name       'handle_text_received'
-                     firstlineno 42
+                     firstlineno 44
                      lnotab 0x0201
                   code
                      argcount  : 0
                      nlocals   : 0
                      stacksize : 2
                      flags     : 19
                      code
                         0x9700740100000000000000000000a6000000ab00000000000000000001
                         0064005300
-                      45           0 RESUME                   0
+                      47           0 RESUME                   0
                      
-                      46           2 LOAD_GLOBAL              1 (NULL + print)
+                      48           2 LOAD_GLOBAL              1 (NULL + print)
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
-                     firstlineno 45
+                     firstlineno 47
                      lnotab 0x0201
                names      ('re', 'match', 'group', 'simple_llm', 'stream_inference')
                varnames   ('self', 'user_input', 'match', 'prompt', 'handle_text_received', 'handle_response_complete')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_chat_request'
-               firstlineno 38
+               firstlineno 40
                lnotab 0x02012a01320206030603
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c01a6010000ab010000000000000000010064005300
-                51           0 RESUME                   0
+                53           0 RESUME                   0
                
-                52           2 LOAD_FAST                0 (self)
+                54           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (shell_command_service)
                             14 LOAD_METHOD              1 (handle_prompt)
                             36 LOAD_FAST                1 (user_input)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
@@ -429,27 +488,55 @@
                   None
                names      ('shell_command_service', 'handle_prompt')
                varnames   ('self', 'user_input')
                freevars   ()
                cellvars   ()
                filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
                name       'handle_shell_nli_request'
-               firstlineno 51
+               firstlineno 53
+               lnotab 0x0201
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 2
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  00000000000000a6000000ab000000000000000000010064005300
+                56           0 RESUME                   0
+               
+                57           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (user_config_service)
+                            14 LOAD_METHOD              1 (prompt_for_all_configs)
+                            36 PRECALL                  0
+                            40 CALL                     0
+                            50 POP_TOP
+                            52 LOAD_CONST               0 (None)
+                            54 RETURN_VALUE
+               consts
+                  None
+               names      ('user_config_service', 'prompt_for_all_configs')
+               varnames   ('self', 'user_input')
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
+               name       'handle_config_request'
+               firstlineno 56
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'str', 'handle_request', 'handle_help_request', 'handle_chat_request', 'handle_shell_nli_request')
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'str', 'handle_request', 'handle_help_request', 'handle_chat_request', 'handle_shell_nli_request', 'handle_config_request')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
          name       'UserCommandService'
-         firstlineno 9
-         lnotab 0x0a01060b0c080609060d
+         firstlineno 12
+         lnotab 0x0a0106090c0a0608060d0603
       'UserCommandService'
-   names      ('re', 'eras.agents.simple_llm', 'SimpleLLM', 'eras.config.config', 'config', 'eras.services.shell_command_service', 'ShellCommandService', 'openai', 'UserCommandService')
+   names      ('re', 'eras.agents.simple_llm', 'SimpleLLM', 'eras.config.config', 'config', 'eras.services.shell_command_service', 'ShellCommandService', 'openai', 'eras.services.user_config_service', 'UserConfigService', 'httpx', 'UserCommandService')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/jason/Documents/dev/eras/eras/services/user_command_service.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020208020c010c010c010802
+   lnotab 0x00ff020208020c010c010c0108020c010802
```

### Comparing `eras-0.3.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc` & `eras-0.3.7/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc` & `eras-0.3.7/eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc` & `eras-0.3.7/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc` & `eras-0.3.7/eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc` & `eras-0.3.7/eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc` & `eras-0.3.7/eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/llm_callable_functions/callable_function_service_base.py` & `eras-0.3.7/eras/services/llm_callable_functions/callable_function_service_base.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/llm_callable_functions/terminal_command.py` & `eras-0.3.7/eras/services/llm_callable_functions/terminal_command.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/llm_callable_functions/user_details.py` & `eras-0.3.7/eras/services/llm_callable_functions/user_details.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/shell_command_service.py` & `eras-0.3.7/eras/services/shell_command_service.py`

 * *Files identical despite different names*

### Comparing `eras-0.3.6/eras/services/user_command_service.py` & `eras-0.3.7/eras/services/user_command_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 import re
 
 from eras.agents.simple_llm import SimpleLLM
 from eras.config.config import config
 from eras.services.shell_command_service import ShellCommandService
 import openai
 
+from eras.services.user_config_service import UserConfigService
+import httpx
+
 class UserCommandService:
     def __init__(self):
         self.openai_client = openai.OpenAI(
-            # base_url=config.get_eras_base_url(),
+            base_url=config.get_eras_base_url(),
             api_key=config.get_eras_open_ai_key()
-            # api_key=config.get_open_ai_key()
         )
         self.shell_command_service = ShellCommandService(self.openai_client)
         self.simple_llm = SimpleLLM(self.openai_client)
-
-
+        self.user_config_service = UserConfigService()
 
     def handle_request(self, user_input: str):
-        if user_input.startswith("/help" ):
+        if user_input.startswith("/help"):
             self.handle_help_request(user_input)
         elif user_input.startswith("/chat"):
             self.handle_chat_request(user_input)
+        elif user_input.startswith("/config"):
+            self.handle_config_request(user_input)
         else:
             self.handle_shell_nli_request(user_input)
 
     def handle_help_request(self, user_input):
         print("Welcome to ERAS - Easily Runnable AI Shell")
         print("Commands: ==============================================")
         print("{defualt usage} - Natural Languge Interface for running commands. e.g. eras how do I list all files in a directory -> %ls")
         print("/help - get info about commands")
         print("/chat - ask the LLM a question about anything. e.g. /chat tell me about quantum physics")
-
-
+        print("/conf - configure eras. urls, keys, etc")
 
     def handle_chat_request(self, user_input):
         match = re.match(r'^/chat\s+(.*)', user_input)
         prompt = match.group(1) if match else None
 
         def handle_text_received(text):
             print(text, end="")
@@ -46,7 +48,11 @@
             print()
 
         self.simple_llm.stream_inference(prompt, handle_text_received, handle_response_complete)
 
 
     def handle_shell_nli_request(self, user_input):
         self.shell_command_service.handle_prompt(user_input)
+
+    def handle_config_request(self, user_input):
+        self.user_config_service.prompt_for_all_configs()
+
```

### Comparing `eras-0.3.6/eras.egg-info/PKG-INFO` & `eras-0.3.7/eras.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.3.6
+Version: 0.3.7
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: asyncio==3.4.3
+Requires-Dist: InquirerPy==0.3.4
 
 # ERAS
 Easily Runnable AI Shell allows you to run shell commands using natural language.   
 
 No more having to leave the terminal to look up how to run a command!
 
 Works on Windows, Mac, and Linux!
```

### Comparing `eras-0.3.6/eras.egg-info/SOURCES.txt` & `eras-0.3.7/eras.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,55 +26,61 @@
 eras/agents/__pycache__/llm_functions_agent.cpython-311.pyc
 eras/agents/__pycache__/llm_functions_agent.cpython-39.pyc
 eras/agents/__pycache__/simple_llm.cpython-311.pyc
 eras/agents/__pycache__/terminal_llama_agent.cpython-311.pyc
 eras/agents/__pycache__/terminal_llama_agent.cpython-39.pyc
 eras/config/__init__.py
 eras/config/config.py
-eras/config/post_install.py
 eras/config/__pycache__/__init__.cpython-311.pyc
 eras/config/__pycache__/config.cpython-311.pyc
 eras/config/__pycache__/config.cpython-39.pyc
-eras/config/__pycache__/post_install.cpython-311.pyc
 eras/decorators/__init__.py
 eras/decorators/chatgpt_tool_data.py
 eras/decorators/__pycache__/chatgpt_tool_data.cpython-311.pyc
 eras/decorators/__pycache__/chatgpt_tool_data.cpython-39.pyc
 eras/factories/__init__.py
 eras/factories/function_details_factory.py
 eras/factories/message_factory.py
 eras/factories/__pycache__/__init__.cpython-311.pyc
 eras/factories/__pycache__/function_details_factory.cpython-311.pyc
 eras/factories/__pycache__/function_details_factory.cpython-39.pyc
 eras/factories/__pycache__/message_factory.cpython-311.pyc
 eras/factories/__pycache__/message_factory.cpython-39.pyc
 eras/models/__init__.py
+eras/models/constants.py
 eras/models/conversation.py
 eras/models/function_details.py
 eras/models/message.py
 eras/models/simple_stream_inference_callable.py
 eras/models/transaction.py
 eras/models/__pycache__/__init__.cpython-311.pyc
+eras/models/__pycache__/constants.cpython-311.pyc
 eras/models/__pycache__/conversation.cpython-311.pyc
 eras/models/__pycache__/conversation.cpython-39.pyc
 eras/models/__pycache__/function_details.cpython-311.pyc
 eras/models/__pycache__/function_details.cpython-39.pyc
 eras/models/__pycache__/message.cpython-311.pyc
 eras/models/__pycache__/message.cpython-39.pyc
 eras/models/__pycache__/simple_stream_inference_callable.cpython-311.pyc
 eras/services/__init__.py
 eras/services/shell_command_service.py
 eras/services/user_command_service.py
+eras/services/user_config_service.py
 eras/services/__pycache__/__init__.cpython-311.pyc
 eras/services/__pycache__/shell_command_service.cpython-311.pyc
 eras/services/__pycache__/shell_command_service.cpython-39.pyc
 eras/services/__pycache__/user_command_service.cpython-311.pyc
+eras/services/__pycache__/user_config_service.cpython-311.pyc
 eras/services/llm_callable_functions/__init__.py
 eras/services/llm_callable_functions/callable_function_service_base.py
 eras/services/llm_callable_functions/terminal_command.py
 eras/services/llm_callable_functions/user_details.py
 eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-311.pyc
 eras/services/llm_callable_functions/__pycache__/callable_function_service_base.cpython-39.pyc
 eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-311.pyc
 eras/services/llm_callable_functions/__pycache__/terminal_command.cpython-39.pyc
 eras/services/llm_callable_functions/__pycache__/user_details.cpython-311.pyc
-eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+eras/services/llm_callable_functions/__pycache__/user_details.cpython-39.pyc
+eras/utils/__init__.py
+eras/utils/env_vars_and_profile_files.py
+eras/utils/__pycache__/__init__.cpython-311.pyc
+eras/utils/__pycache__/env_vars_and_profile_files.cpython-311.pyc
```

