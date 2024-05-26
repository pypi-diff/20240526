# Comparing `tmp/llama_cpp_agent-0.2.8.tar.gz` & `tmp/llama_cpp_agent-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_agent-0.2.8.tar", last modified: Mon May 20 21:19:52 2024, max compression
+gzip compressed data, was "llama_cpp_agent-0.2.9.tar", last modified: Mon May 20 22:01:23 2024, max compression
```

## Comparing `llama_cpp_agent-0.2.8.tar` & `llama_cpp_agent-0.2.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.549673 llama_cpp_agent-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-20 21:19:52.549673 llama_cpp_agent-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/ReadMe.md
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:19:52.549673 llama_cpp_agent-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.537673 llama_cpp_agent-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.541673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/event_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/event_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/basic_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/chat_history_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/function_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/function_calling_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51567 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/hermes_2_pro_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/json_schema_generator/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/json_schema_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/json_schema_generator/schema_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21328 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_documentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_documentation/documentation_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_output_settings/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_output_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32298 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_output_settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11425 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/messages_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/mixtral_8x22b_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/prompt_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/llama_cpp_python.py
--rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/llama_cpp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/provider_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/tgi_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/vllm_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.545673 llama_cpp_agent-0.2.8/src/llama_cpp_agent/rag/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/rag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/rag/rag_colbert_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/structured_output_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-20 21:19:48.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:19:52.549673 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 21:19:52.000000 llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.863770 llama_cpp_agent-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-20 22:01:23.863770 llama_cpp_agent-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/ReadMe.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:01:23.863770 llama_cpp_agent-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.851770 llama_cpp_agent-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.855770 llama_cpp_agent-0.2.9/src/llama_cpp_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.855770 llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/event_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/event_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12331 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.859770 llama_cpp_agent-0.2.9/src/llama_cpp_agent/chat_history/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/chat_history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/chat_history/basic_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/chat_history/chat_history_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/chat_history/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/function_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/function_calling_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.859770 llama_cpp_agent-0.2.9/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51567 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13368 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/hermes_2_pro_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.859770 llama_cpp_agent-0.2.9/src/llama_cpp_agent/json_schema_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/json_schema_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11406 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/json_schema_generator/schema_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21611 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.859770 llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_documentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_documentation/documentation_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.859770 llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_output_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_output_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32298 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_output_settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11425 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/messages_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/mixtral_8x22b_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/prompt_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.859770 llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/llama_cpp_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/llama_cpp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/provider_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/tgi_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/vllm_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.859770 llama_cpp_agent-0.2.9/src/llama_cpp_agent/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/rag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/rag/rag_colbert_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/structured_output_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-20 22:01:19.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:01:23.859770 llama_cpp_agent-0.2.9/src/llama_cpp_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-20 22:01:23.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 22:01:23.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:01:23.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 22:01:23.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 22:01:23.000000 llama_cpp_agent-0.2.9/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama_cpp_agent-0.2.8/LICENSE` & `llama_cpp_agent-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/PKG-INFO` & `llama_cpp_agent-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.8
+Version: 0.2.9
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llama_cpp_agent-0.2.8/ReadMe.md` & `llama_cpp_agent-0.2.9/ReadMe.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/pyproject.toml` & `llama_cpp_agent-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [  "setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llama-cpp-agent"
-version = "0.2.8"
+version = "0.2.9"
 description = "A framework for building LLM based AI agents with llama.cpp."
 
 readme = "ReadMe.md"
 dependencies = [
     "llama-cpp-python>=0.2.60",
     "pydantic>=2.5.3",
     "requests>=2.31.0",
```

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/event_memory.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/event_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/event_memory_manager.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/event_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/chain.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/chain.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/basic_chat_history.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/chat_history/basic_chat_history.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/chat_history_base.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/chat_history/chat_history_base.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/chat_history/messages.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/chat_history/messages.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/function_calling.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/function_calling.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/function_calling_agent.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/function_calling_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/hermes_2_pro_agent.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/hermes_2_pro_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/json_schema_generator/schema_generator.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/json_schema_generator/schema_generator.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_agent.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,14 +376,20 @@
             system_prompt: str = None,
             add_message_to_chat_history: bool = True,
             role: Roles = Roles.user,
             prompt_suffix: str = None,
             llm_sampling_settings: LlmSamplingSettings = None,
             structured_output_settings: LlmStructuredOutputSettings = None,
     ):
+        if len(chat_history.get_chat_messages()) == 0:
+            if system_prompt:
+                chat_history.add_message({"role": "system", "content": system_prompt})
+            else:
+                chat_history.add_message({"role": "system", "content": self.system_prompt})
+
         if message is not None and add_message_to_chat_history:
             chat_history.add_message(
                 {
                     "role": role,
                     "content": message,
                 }
             )
```

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_documentation/documentation_generation.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_documentation/documentation_generation.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_output_settings/settings.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_output_settings/settings.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/llm_prompt_template.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/llm_prompt_template.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/messages_formatter.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/messages_formatter.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/mixtral_8x22b_agent.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/mixtral_8x22b_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/output_parser.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/prompt_templates.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/prompts.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/llama_cpp_python.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/llama_cpp_python.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/llama_cpp_server.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/llama_cpp_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/provider_base.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/provider_base.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/tgi_server.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/tgi_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/providers/vllm_server.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/providers/vllm_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/rag/rag_colbert_reranker.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/rag/rag_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/structured_output_agent.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/structured_output_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent/text_utils.py` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent/text_utils.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/PKG-INFO` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.8
+Version: 0.2.9
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `llama_cpp_agent-0.2.8/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama_cpp_agent-0.2.9/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

