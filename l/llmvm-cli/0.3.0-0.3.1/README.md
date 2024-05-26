# Comparing `tmp/llmvm_cli-0.3.0.tar.gz` & `tmp/llmvm_cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmvm_cli-0.3.0.tar", max compression
+gzip compressed data, was "llmvm_cli-0.3.1.tar", max compression
```

## Comparing `llmvm_cli-0.3.0.tar` & `llmvm_cli-0.3.1.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0     1495 2024-01-03 07:02:07.545205 llmvm_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0    28302 2024-04-02 06:01:38.458668 llmvm_cli-0.3.0/README.md
--rw-r--r--   0        0        0      106 2024-02-25 23:41:30.071592 llmvm_cli-0.3.0/llmvm/client/__main__.py
--rw-r--r--   0        0        0    65054 2024-02-07 02:24:12.376520 llmvm_cli-0.3.0/llmvm/client/awesome_prompts.csv
--rw-r--r--   0        0        0    76135 2024-04-05 17:39:11.686252 llmvm_cli-0.3.0/llmvm/client/client.py
--rw-r--r--   0        0        0        0 2024-02-07 02:24:12.376988 llmvm_cli-0.3.0/llmvm/common/__init__.py
--rw-r--r--   0        0        0    19995 2024-04-05 04:13:18.903735 llmvm_cli-0.3.0/llmvm/common/anthropic_executor.py
--rw-r--r--   0        0        0     3828 2024-02-07 02:24:12.377381 llmvm_cli-0.3.0/llmvm/common/container.py
--rw-r--r--   0        0        0     7735 2024-04-02 06:01:38.459780 llmvm_cli-0.3.0/llmvm/common/gemini_executor.py
--rw-r--r--   0        0        0    40120 2024-04-05 04:13:18.904346 llmvm_cli-0.3.0/llmvm/common/helpers.py
--rw-r--r--   0        0        0     7472 2024-03-01 18:22:41.276981 llmvm_cli-0.3.0/llmvm/common/logging_helpers.py
--rw-r--r--   0        0        0     7100 2024-04-02 06:01:38.460105 llmvm_cli-0.3.0/llmvm/common/mistral_executor.py
--rw-r--r--   0        0        0     3861 2024-04-05 04:13:18.904513 llmvm_cli-0.3.0/llmvm/common/object_transformers.py
--rw-r--r--   0        0        0    28450 2024-04-05 17:39:11.686652 llmvm_cli-0.3.0/llmvm/common/objects.py
--rw-r--r--   0        0        0    10655 2024-04-05 17:39:11.686930 llmvm_cli-0.3.0/llmvm/common/openai_executor.py
--rw-r--r--   0        0        0     7404 2024-04-05 04:13:18.905099 llmvm_cli-0.3.0/llmvm/common/pdf.py
--rw-r--r--   0        0        0    10711 2024-04-02 06:01:38.460644 llmvm_cli-0.3.0/llmvm/common/perf.py
--rw-r--r--   0        0        0      457 2024-02-07 02:24:12.378504 llmvm_cli-0.3.0/llmvm/common/singleton.py
--rw-r--r--   0        0        0     1608 2024-03-18 05:16:30.191195 llmvm_cli-0.3.0/llmvm/config.yaml
--rw-r--r--   0        0        0    76737 2024-04-02 06:01:38.460972 llmvm_cli-0.3.0/llmvm/model_prices_and_context_window.json
--rw-r--r--   0        0        0        0 2024-02-07 02:24:12.378662 llmvm_cli-0.3.0/llmvm/server/__init__.py
--rw-r--r--   0        0        0      106 2024-02-25 23:41:30.074183 llmvm_cli-0.3.0/llmvm/server/__main__.py
--rw-r--r--   0        0        0     5977 2024-03-01 18:22:41.278186 llmvm_cli-0.3.0/llmvm/server/ast_parser.py
--rw-r--r--   0        0        0    20300 2024-04-02 06:01:38.461151 llmvm_cli-0.3.0/llmvm/server/base_library/browser.py
--rw-r--r--   0        0        0     2255 2024-03-18 05:16:30.191315 llmvm_cli-0.3.0/llmvm/server/base_library/content_downloader.py
--rw-r--r--   0        0        0    13460 2024-04-02 06:01:38.461337 llmvm_cli-0.3.0/llmvm/server/base_library/function_bindable.py
--rw-r--r--   0        0        0    16053 2024-04-02 06:01:38.461512 llmvm_cli-0.3.0/llmvm/server/base_library/searcher.py
--rw-r--r--   0        0        0     5457 2024-03-18 05:16:30.191913 llmvm_cli-0.3.0/llmvm/server/base_library/source.py
--rw-r--r--   0        0        0     6006 2024-04-02 06:01:38.461658 llmvm_cli-0.3.0/llmvm/server/base_library/source_project.py
--rw-r--r--   0        0        0      607 2024-03-18 05:16:30.192200 llmvm_cli-0.3.0/llmvm/server/bcl.py
--rw-r--r--   0        0        0     1731 2024-02-07 02:24:12.379056 llmvm_cli-0.3.0/llmvm/server/persistent_cache.py
--rw-r--r--   0        0        0        0 2024-02-07 02:24:12.379148 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/__init__.py
--rw-r--r--   0        0        0     1148 2024-02-07 02:24:12.379247 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer.prompt
--rw-r--r--   0        0        0     4983 2024-03-18 05:16:30.192346 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_error_correction.prompt
--rw-r--r--   0        0        0     1339 2024-03-18 05:16:30.192471 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_nocontext.prompt
--rw-r--r--   0        0        0      362 2024-03-18 05:16:30.192566 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_primitive.prompt
--rw-r--r--   0        0        0     5532 2024-03-18 05:16:30.192634 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_regen_code_or_rewrite.prompt
--rw-r--r--   0        0        0       84 2024-02-07 02:24:12.379686 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/assistant_result.prompt
--rw-r--r--   0        0        0     2542 2024-04-02 06:01:38.461773 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/browser_execute_plan.prompt
--rw-r--r--   0        0        0     1883 2024-04-02 06:01:38.461872 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/browser_generate_plan.prompt
--rw-r--r--   0        0        0     1463 2024-02-07 02:24:12.384341 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/code_get_source_summary.prompt
--rw-r--r--   0        0        0      380 2024-02-07 02:24:12.384491 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/code_method_definition.prompt
--rw-r--r--   0        0        0      810 2024-02-07 02:24:12.384600 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/coerce.prompt
--rw-r--r--   0        0        0      788 2024-02-07 02:24:12.384694 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/document_chunk.prompt
--rw-r--r--   0        0        0       81 2024-02-07 02:24:12.384782 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/foreach_result.prompt
--rw-r--r--   0        0        0      343 2024-02-07 02:24:12.384857 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/function_call_result.prompt
--rw-r--r--   0        0        0      320 2024-02-07 02:24:12.384939 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/functionmeta_result.prompt
--rw-r--r--   0        0        0      215 2024-02-07 02:24:12.385017 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/list_result.prompt
--rw-r--r--   0        0        0      757 2024-02-07 02:24:12.385103 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_error_correction.prompt
--rw-r--r--   0        0        0     1544 2024-03-18 05:16:30.192749 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_global.prompt
--rw-r--r--   0        0        0      935 2024-02-07 02:24:12.385254 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_list.prompt
--rw-r--r--   0        0        0      784 2024-02-07 02:24:12.385408 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_local.prompt
--rw-r--r--   0        0        0      862 2024-02-07 02:24:12.385520 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_old.prompt
--rw-r--r--   0        0        0      556 2024-03-18 05:16:30.192871 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_call.prompt
--rw-r--r--   0        0        0      167 2024-02-07 02:24:12.385701 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_call_result.prompt
--rw-r--r--   0        0        0      545 2024-02-07 02:24:12.385794 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_loop_bind.prompt
--rw-r--r--   0        0        0      876 2024-02-07 02:24:12.385890 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/map_reduce_map.prompt
--rw-r--r--   0        0        0      783 2024-02-07 02:24:12.387514 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/map_reduce_reduce.prompt
--rw-r--r--   0        0        0      592 2024-02-07 02:24:12.387584 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/pandas_bind.prompt
--rw-r--r--   0        0        0      641 2024-02-07 02:24:12.387647 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/pdf_content.prompt
--rw-r--r--   0        0        0     2639 2024-02-07 02:24:12.387730 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/query_understanding.prompt
--rw-r--r--   0        0        0      762 2024-02-07 02:24:12.387793 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_classifier.prompt
--rw-r--r--   0        0        0      458 2024-02-07 02:24:12.387857 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_expander.prompt
--rw-r--r--   0        0        0     1003 2024-02-07 02:24:12.387923 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_location.prompt
--rw-r--r--   0        0        0      746 2024-02-07 02:24:12.388003 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_ranker.prompt
--rw-r--r--   0        0        0     8200 2024-02-07 02:24:12.388113 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_code_insights.prompt
--rw-r--r--   0        0        0     4940 2024-02-07 02:24:12.388202 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_code_prompt_old.prompt
--rw-r--r--   0        0        0    12639 2024-02-07 02:24:12.388275 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_continuation_execution.prompt
--rw-r--r--   0        0        0     4927 2024-03-18 05:16:30.193009 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_error_correction.prompt
--rw-r--r--   0        0        0    15324 2024-03-18 05:16:30.193153 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_tool_execution.prompt
--rw-r--r--   0        0        0      156 2024-02-07 02:24:12.388557 llmvm_cli-0.3.0/llmvm/server/prompts/starlark/str_result.prompt
--rw-r--r--   0        0        0    23395 2024-03-18 05:16:30.193315 llmvm_cli-0.3.0/llmvm/server/server.py
--rw-r--r--   0        0        0    37254 2024-04-02 06:01:38.462118 llmvm_cli-0.3.0/llmvm/server/starlark_execution_controller.py
--rw-r--r--   0        0        0    40722 2024-04-02 06:01:38.462363 llmvm_cli-0.3.0/llmvm/server/starlark_runtime.py
--rw-r--r--   0        0        0     6327 2024-03-18 05:16:30.194183 llmvm_cli-0.3.0/llmvm/server/tools/edgar.py
--rw-r--r--   0        0        0    13091 2024-04-02 06:01:38.462546 llmvm_cli-0.3.0/llmvm/server/tools/firefox.py
--rw-r--r--   0        0        0        0 2024-02-07 02:24:12.389702 llmvm_cli-0.3.0/llmvm/server/tools/legacy.py
--rw-r--r--   0        0        0     1872 2024-02-07 02:24:12.389891 llmvm_cli-0.3.0/llmvm/server/tools/market.py
--rw-r--r--   0        0        0     4270 2024-02-07 02:24:12.390078 llmvm_cli-0.3.0/llmvm/server/tools/scraper.py
--rw-r--r--   0        0        0     6839 2024-02-25 23:41:30.075967 llmvm_cli-0.3.0/llmvm/server/tools/search.py
--rw-r--r--   0        0        0     8704 2024-02-07 02:24:12.390266 llmvm_cli-0.3.0/llmvm/server/tools/search_hn.py
--rw-r--r--   0        0        0     4603 2024-04-02 06:01:38.462796 llmvm_cli-0.3.0/llmvm/server/tools/webhelpers.py
--rw-r--r--   0        0        0     9391 2024-03-18 05:16:30.194621 llmvm_cli-0.3.0/llmvm/server/vector_search.py
--rw-r--r--   0        0        0     6848 2024-02-25 23:41:30.076167 llmvm_cli-0.3.0/llmvm/server/vector_store.py
--rw-r--r--   0        0        0     1562 2024-04-05 17:39:25.432631 llmvm_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    30688 1970-01-01 00:00:00.000000 llmvm_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1495 2024-05-22 17:01:44.240387 llmvm_cli-0.3.1/LICENSE
+-rw-r--r--   0        0        0    28267 2024-05-26 20:40:23.400924 llmvm_cli-0.3.1/README.md
+-rw-r--r--   0        0        0      106 2024-05-22 17:01:44.273607 llmvm_cli-0.3.1/llmvm/client/__main__.py
+-rw-r--r--   0        0        0    65054 2024-05-22 17:01:44.273764 llmvm_cli-0.3.1/llmvm/client/awesome_prompts.csv
+-rw-r--r--   0        0        0    76121 2024-05-26 20:40:18.511234 llmvm_cli-0.3.1/llmvm/client/client.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:01:44.274037 llmvm_cli-0.3.1/llmvm/common/__init__.py
+-rw-r--r--   0        0        0    20006 2024-05-26 19:55:03.094946 llmvm_cli-0.3.1/llmvm/common/anthropic_executor.py
+-rw-r--r--   0        0        0     3988 2024-05-26 19:54:49.529683 llmvm_cli-0.3.1/llmvm/common/container.py
+-rw-r--r--   0        0        0     7735 2024-05-22 17:01:44.274335 llmvm_cli-0.3.1/llmvm/common/gemini_executor.py
+-rw-r--r--   0        0        0    40120 2024-05-22 17:01:44.274455 llmvm_cli-0.3.1/llmvm/common/helpers.py
+-rw-r--r--   0        0        0     7472 2024-05-22 17:01:44.274577 llmvm_cli-0.3.1/llmvm/common/logging_helpers.py
+-rw-r--r--   0        0        0     7100 2024-05-22 17:01:44.274695 llmvm_cli-0.3.1/llmvm/common/mistral_executor.py
+-rw-r--r--   0        0        0     3861 2024-05-22 17:01:44.274746 llmvm_cli-0.3.1/llmvm/common/object_transformers.py
+-rw-r--r--   0        0        0    28450 2024-05-22 17:01:44.274839 llmvm_cli-0.3.1/llmvm/common/objects.py
+-rw-r--r--   0        0        0    10681 2024-05-26 20:40:11.177546 llmvm_cli-0.3.1/llmvm/common/openai_executor.py
+-rw-r--r--   0        0        0     7404 2024-05-22 17:01:44.275308 llmvm_cli-0.3.1/llmvm/common/pdf.py
+-rw-r--r--   0        0        0    10711 2024-05-22 17:01:44.275592 llmvm_cli-0.3.1/llmvm/common/perf.py
+-rw-r--r--   0        0        0      457 2024-05-22 17:01:44.275640 llmvm_cli-0.3.1/llmvm/common/singleton.py
+-rw-r--r--   0        0        0     1595 2024-05-26 20:40:15.616260 llmvm_cli-0.3.1/llmvm/config.yaml
+-rw-r--r--   0        0        0   127295 2024-05-26 20:37:40.833181 llmvm_cli-0.3.1/llmvm/model_prices_and_context_window.json
+-rw-r--r--   0        0        0        0 2024-05-22 17:01:44.275926 llmvm_cli-0.3.1/llmvm/server/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-22 17:01:44.275978 llmvm_cli-0.3.1/llmvm/server/__main__.py
+-rw-r--r--   0        0        0     5977 2024-05-22 17:01:44.276057 llmvm_cli-0.3.1/llmvm/server/ast_parser.py
+-rw-r--r--   0        0        0    20300 2024-05-22 17:01:44.276177 llmvm_cli-0.3.1/llmvm/server/base_library/browser.py
+-rw-r--r--   0        0        0     2255 2024-05-22 17:01:44.276272 llmvm_cli-0.3.1/llmvm/server/base_library/content_downloader.py
+-rw-r--r--   0        0        0    13460 2024-05-22 17:01:44.276441 llmvm_cli-0.3.1/llmvm/server/base_library/function_bindable.py
+-rw-r--r--   0        0        0    16053 2024-05-22 17:01:44.276573 llmvm_cli-0.3.1/llmvm/server/base_library/searcher.py
+-rw-r--r--   0        0        0     5457 2024-05-22 17:01:44.276679 llmvm_cli-0.3.1/llmvm/server/base_library/source.py
+-rw-r--r--   0        0        0     6006 2024-05-22 17:01:44.276764 llmvm_cli-0.3.1/llmvm/server/base_library/source_project.py
+-rw-r--r--   0        0        0      607 2024-05-22 17:01:44.276821 llmvm_cli-0.3.1/llmvm/server/bcl.py
+-rw-r--r--   0        0        0     1731 2024-05-22 17:01:44.276875 llmvm_cli-0.3.1/llmvm/server/persistent_cache.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:01:44.276962 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-26 20:44:59.445232 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1148 2024-05-22 17:01:44.277037 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/answer.prompt
+-rw-r--r--   0        0        0     4983 2024-05-22 17:01:44.277159 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/answer_error_correction.prompt
+-rw-r--r--   0        0        0     1339 2024-05-22 17:01:44.277221 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/answer_nocontext.prompt
+-rw-r--r--   0        0        0      362 2024-05-22 17:01:44.277287 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/answer_primitive.prompt
+-rw-r--r--   0        0        0     5532 2024-05-22 17:01:44.277369 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/answer_regen_code_or_rewrite.prompt
+-rw-r--r--   0        0        0       84 2024-05-22 17:01:44.277415 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/assistant_result.prompt
+-rw-r--r--   0        0        0     2542 2024-05-22 17:01:44.277474 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/browser_execute_plan.prompt
+-rw-r--r--   0        0        0     1883 2024-05-22 17:01:44.277537 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/browser_generate_plan.prompt
+-rw-r--r--   0        0        0     1463 2024-05-22 17:01:44.277590 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/code_get_source_summary.prompt
+-rw-r--r--   0        0        0      380 2024-05-22 17:01:44.277646 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/code_method_definition.prompt
+-rw-r--r--   0        0        0      810 2024-05-22 17:01:44.277694 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/coerce.prompt
+-rw-r--r--   0        0        0      788 2024-05-22 17:01:44.277768 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/document_chunk.prompt
+-rw-r--r--   0        0        0       81 2024-05-22 17:01:44.277815 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/foreach_result.prompt
+-rw-r--r--   0        0        0      343 2024-05-22 17:01:44.277867 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/function_call_result.prompt
+-rw-r--r--   0        0        0      320 2024-05-22 17:01:44.277923 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/functionmeta_result.prompt
+-rw-r--r--   0        0        0      215 2024-05-22 17:01:44.277983 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/list_result.prompt
+-rw-r--r--   0        0        0      757 2024-05-22 17:01:44.278028 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_error_correction.prompt
+-rw-r--r--   0        0        0     1544 2024-05-22 17:01:44.278096 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_global.prompt
+-rw-r--r--   0        0        0      935 2024-05-22 17:01:44.278160 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_list.prompt
+-rw-r--r--   0        0        0      784 2024-05-22 17:01:44.278233 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_local.prompt
+-rw-r--r--   0        0        0      862 2024-05-22 17:01:44.278292 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_old.prompt
+-rw-r--r--   0        0        0      556 2024-05-22 17:01:44.278348 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_call.prompt
+-rw-r--r--   0        0        0      167 2024-05-22 17:01:44.278406 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_call_result.prompt
+-rw-r--r--   0        0        0      545 2024-05-22 17:01:44.278478 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_loop_bind.prompt
+-rw-r--r--   0        0        0      876 2024-05-22 17:01:44.278529 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/map_reduce_map.prompt
+-rw-r--r--   0        0        0      783 2024-05-22 17:01:44.278576 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/map_reduce_reduce.prompt
+-rw-r--r--   0        0        0      592 2024-05-22 17:01:44.278626 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/pandas_bind.prompt
+-rw-r--r--   0        0        0      641 2024-05-22 17:01:44.278694 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/pdf_content.prompt
+-rw-r--r--   0        0        0     2639 2024-05-22 17:01:44.278751 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/query_understanding.prompt
+-rw-r--r--   0        0        0      762 2024-05-22 17:01:44.278802 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/search_classifier.prompt
+-rw-r--r--   0        0        0      458 2024-05-22 17:01:44.278860 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/search_expander.prompt
+-rw-r--r--   0        0        0     1003 2024-05-22 17:01:44.278931 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/search_location.prompt
+-rw-r--r--   0        0        0      746 2024-05-22 17:01:44.278981 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/search_ranker.prompt
+-rw-r--r--   0        0        0     8200 2024-05-22 17:01:44.279252 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_code_insights.prompt
+-rw-r--r--   0        0        0     4940 2024-05-22 17:01:44.279355 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_code_prompt_old.prompt
+-rw-r--r--   0        0        0    12639 2024-05-22 17:01:44.279496 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_continuation_execution.prompt
+-rw-r--r--   0        0        0     4927 2024-05-22 17:01:44.279573 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_error_correction.prompt
+-rw-r--r--   0        0        0    15324 2024-05-22 17:01:44.279693 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_tool_execution.prompt
+-rw-r--r--   0        0        0      156 2024-05-22 17:01:44.279738 llmvm_cli-0.3.1/llmvm/server/prompts/starlark/str_result.prompt
+-rw-r--r--   0        0        0    23395 2024-05-22 17:01:44.279837 llmvm_cli-0.3.1/llmvm/server/server.py
+-rw-r--r--   0        0        0    37254 2024-05-22 17:01:44.279969 llmvm_cli-0.3.1/llmvm/server/starlark_execution_controller.py
+-rw-r--r--   0        0        0    40722 2024-05-22 17:01:44.280074 llmvm_cli-0.3.1/llmvm/server/starlark_runtime.py
+-rw-r--r--   0        0        0     6327 2024-05-22 17:01:44.280213 llmvm_cli-0.3.1/llmvm/server/tools/edgar.py
+-rw-r--r--   0        0        0    13091 2024-05-22 17:01:44.280337 llmvm_cli-0.3.1/llmvm/server/tools/firefox.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:01:44.280370 llmvm_cli-0.3.1/llmvm/server/tools/legacy.py
+-rw-r--r--   0        0        0     1872 2024-05-22 17:01:44.280426 llmvm_cli-0.3.1/llmvm/server/tools/market.py
+-rw-r--r--   0        0        0     4270 2024-05-22 17:01:44.280514 llmvm_cli-0.3.1/llmvm/server/tools/scraper.py
+-rw-r--r--   0        0        0     6839 2024-05-22 17:01:44.280606 llmvm_cli-0.3.1/llmvm/server/tools/search.py
+-rw-r--r--   0        0        0     8704 2024-05-22 17:01:44.280893 llmvm_cli-0.3.1/llmvm/server/tools/search_hn.py
+-rw-r--r--   0        0        0     4603 2024-05-22 17:01:44.280987 llmvm_cli-0.3.1/llmvm/server/tools/webhelpers.py
+-rw-r--r--   0        0        0     9391 2024-05-22 17:01:44.281269 llmvm_cli-0.3.1/llmvm/server/vector_search.py
+-rw-r--r--   0        0        0     6848 2024-05-22 17:01:44.281365 llmvm_cli-0.3.1/llmvm/server/vector_store.py
+-rw-r--r--   0        0        0     1562 2024-05-26 21:33:22.613460 llmvm_cli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    30653 1970-01-01 00:00:00.000000 llmvm_cli-0.3.1/PKG-INFO
```

### Comparing `llmvm_cli-0.3.0/LICENSE` & `llmvm_cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/README.md` & `llmvm_cli-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # LLMVM
 
 LLMVM is a CLI based productivity tool that uses Large Language Models and local Python tools/helpers to reason about and execute your tasks. A CLI client (client.py) either connects directly to an LLM provider or will connect to a local server (server.py) that coordinates tool execution, [Retrieval Agumented Generation](https://blogs.nvidia.com/blog/what-is-retrieval-augmented-generation/), document search and more.
 
-It supports [Anthropic's](https://www.anthropic.com) Claude 3 (Opus, Sonnet and Haiku) vision models, [OpenAI](https://openai.com/blog/openai-api) GPT 3.5/4/4 Turbo and Vision models from OpenAI. [Gemini](https://deepmind.google/technologies/gemini/) and [Mistral](https://deepmind.google/technologies/gemini/) are currently experimental. It's best used with the [kitty](https://github.com/kovidgoyal/kitty) terminal as LLMVM will screenshot and render images as work on vision based tasks progresses.
+It supports [Anthropic's](https://www.anthropic.com) Claude 3 (Opus, Sonnet and Haiku) vision models, [OpenAI](https://openai.com/blog/openai-api) GPT 3.5/4/4 Turbo/4o models from OpenAI. [Gemini](https://deepmind.google/technologies/gemini/) and [Mistral](https://deepmind.google/technologies/gemini/) are currently experimental. It's best used with the [kitty](https://github.com/kovidgoyal/kitty) terminal as LLMVM will screenshot and render images as work on vision based tasks progresses.
 
 LLMVM's features are best explored through examples. Let's install, then go through some:
 
 ```$ pip install llmvm-cli```
 ```$ playwright install firefox```
 
 ```$ python -m llmvm.server```
@@ -97,15 +97,15 @@
 
 and then:
 
 ```bash
 cat somecode.py | llm -o direct "rewrite this code; make it cleaner and easier to read"
 ```
 
-Image understanding is supported on Anthropic Claude 3 models and OpenAI's GPT 4 turbo vision preview model.
+Image understanding is supported on Anthropic Claude 3 models and OpenAI's GPT 4o vision model.
 
 ```bash
 cat docs/beach.jpg | llm "generate a dalle prompt for the exact inverse of this image"
 ```
 
 ![](docs/2023-11-11-12-59-39.png)
 
@@ -214,15 +214,15 @@
 executor: 'anthropic'  # or 'openai'
 ```
 
 or, you can set environment variables that specify the execution backend and the model you'd like to use:
 
 ```bash
 export LLMVM_EXECUTOR='openai'
-export LLMVM_MODEL='gpt-4-vision-preview'
+export LLMVM_MODEL='gpt-4o'
 python -m llmvm.client "hello, who are you?"
 ```
 
 #### Performance Profiling
 
 * open `~/.config/llmvm/config.yaml` and change profiling to 'true' or 'false'.
```

### Comparing `llmvm_cli-0.3.0/llmvm/client/awesome_prompts.csv` & `llmvm_cli-0.3.1/llmvm/client/awesome_prompts.csv`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/client/client.py` & `llmvm_cli-0.3.1/llmvm/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,15 +613,15 @@
         else:
             raise ValueError(f'Executor {executor} and model {model} are set, but no API key is set.')
     elif Container.get_config_variable('OPENAI_API_KEY'):
         assistant = await execute_llm_call_direct(
             message,
             Container.get_config_variable('OPENAI_API_KEY'),
             'openai',
-            'gpt-4-vision-preview',
+            'gpt-4o',
             context_messages
         )
         return SessionThread(
             id=-1,
             messages=[MessageModel.from_message(message) for message in list(context_messages) + [message, assistant]]
         )
     elif os.environ.get('ANTHROPIC_API_KEY'):
```

### Comparing `llmvm_cli-0.3.0/llmvm/common/anthropic_executor.py` & `llmvm_cli-0.3.1/llmvm/common/anthropic_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
 
         # anthropic disallows empty messages, so we're going to remove any Message that doesn't contain content
         for message in messages:
             if not message['content'] or message['content'] == '' or message['content'] == b'':
                 logging.warning(f"Removing empty message: {message}")
                 messages.remove(message)
 
-        if Container().get_config_variable('ANTHROPIC_COLLAPSE_MESSAGES', default=False):
+        if Container(throw=False).get_config_variable('ANTHROPIC_COLLAPSE_MESSAGES', default=False):
             collapsed_messages = []
             accumulator = ''
             for i in range(len(messages)):
                 if messages[i]['role'] == 'user' and not isinstance(messages[i]['content'], list):
                     accumulator += messages[i]['content'] + '\n\n'
                 elif messages[i]['role'] == 'user' and isinstance(messages[i]['content'], list) and accumulator:
                     collapsed_messages.append({'role': 'user', 'content': accumulator})
```

### Comparing `llmvm_cli-0.3.0/llmvm/common/container.py` & `llmvm_cli-0.3.1/llmvm/common/container.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,22 +11,28 @@
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 class Container(metaclass=Singleton):
-    def __init__(self, config_file: str = os.path.expanduser('~/.config/llmvm/config.yaml')):
+    def __init__(
+            self,
+            config_file: str = os.path.expanduser('~/.config/llmvm/config.yaml'),
+            throw: bool = True
+        ):
         self.config_file = config_file
 
         if os.getenv('LLMVM_CONFIG'):
             self.config_file = cast(str, os.getenv('LLMVM_CONFIG'))
 
-        if not os.path.exists(self.config_file):
+        if not os.path.exists(self.config_file) and throw:
             raise ValueError('configuration_file {} is not found. Put config in ~/.config/llmvm or set LLMVM_CONFIG'.format(config_file))
+        elif not os.path.exists(self.config_file) and not throw:
+            return
 
         with open(self.config_file, 'r') as conf_file:
             self.configuration: Dict = yaml.load(conf_file, Loader=yaml.FullLoader)  # type: ignore
             self.type_instance_cache: Dict[Type, object] = {}
 
     def resolve(self, t: Type, **extra_args):
         args = {}
```

### Comparing `llmvm_cli-0.3.0/llmvm/common/gemini_executor.py` & `llmvm_cli-0.3.1/llmvm/common/gemini_executor.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/common/helpers.py` & `llmvm_cli-0.3.1/llmvm/common/helpers.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/common/logging_helpers.py` & `llmvm_cli-0.3.1/llmvm/common/logging_helpers.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/common/mistral_executor.py` & `llmvm_cli-0.3.1/llmvm/common/mistral_executor.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/common/object_transformers.py` & `llmvm_cli-0.3.1/llmvm/common/object_transformers.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/common/objects.py` & `llmvm_cli-0.3.1/llmvm/common/objects.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/common/openai_executor.py` & `llmvm_cli-0.3.1/llmvm/common/openai_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,15 @@
                 "gpt-3.5-turbo-16k-0613",
                 "gpt-3.5-turbo-0125",
                 "gpt-3.5-turbo-1106",
                 "gpt-3.5-turbo",
                 "gpt-4",
                 "gpt-4-0314",
                 "gpt-4-vision-preview",
+                "gpt-4o",
                 "gpt-4-1106-preview",
                 "gpt-4-32k-0314",
                 "gpt-4-0613",
                 "gpt-4-32k-0613",
             }:
                 tokens_per_message = 3
                 tokens_per_name = 1
```

### Comparing `llmvm_cli-0.3.0/llmvm/common/pdf.py` & `llmvm_cli-0.3.1/llmvm/common/pdf.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/common/perf.py` & `llmvm_cli-0.3.1/llmvm/common/perf.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/config.yaml` & `llmvm_cli-0.3.1/llmvm/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 cache_directory: '~/.local/share/llmvm/cache'
 cdn_directory: '~/.local/share/llmvm/cdn'
 log_directory: '~/.local/share/llmvm/logs'
 vector_store_index_directory: '~/.local/share/llmvm/faiss'
 vector_store_embedding_model: 'all-MiniLM-L6-v2' # 'BAAI/bge-base-en'
 vector_store_chunk_size: 500
 openai_api_base: 'https://api.openai.com/v1'
-openai_model: 'gpt-4-vision-preview'
-openai_max_tokens: 16384
+openai_model: 'gpt-4o'
+openai_max_tokens: 128000
 anthropic_api_base: 'https://api.anthropic.com'
 anthropic_model: 'claude-3-sonnet-20240229'
 anthropic_max_tokens: 200000
 local_api_base: 'http://localhost:8000/v1'
 local_model: 'llongorca.gguf'
 local_model_max_tokens: 16385
 executor: 'openai'  # openai, anthropic, local
```

### Comparing `llmvm_cli-0.3.0/llmvm/model_prices_and_context_window.json` & `llmvm_cli-0.3.1/llmvm/model_prices_and_context_window.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6550921114337982%*

 * *Differences: {"'ai21.j2-mid-v1'": "{'max_input_tokens': 8191, 'max_output_tokens': 8191}",*

 * * "'ai21.j2-ultra-v1'": "{'max_input_tokens': 8191, 'max_output_tokens': 8191}",*

 * * "'amazon.titan-embed-text-v1'": "{'max_input_tokens': 8192}",*

 * * "'amazon.titan-embed-text-v2:0'": "OrderedDict([('max_tokens', 8192), ('max_input_tokens', 8192), "*

 * *                                   "('output_vector_size', 1024), ('input_cost_per_token', 2e-07), "*

 * *                                   "('output_cost_per_token', 0.0), ('litellm_provider',  […]*

```diff
@@ -44,298 +44,429 @@
         "max_tokens": 77,
         "mode": "image_generation",
         "output_cost_per_image": 0.036
     },
     "ai21.j2-mid-v1": {
         "input_cost_per_token": 1.25e-05,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 8191,
+        "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 1.25e-05
     },
     "ai21.j2-ultra-v1": {
         "input_cost_per_token": 1.88e-05,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 8191,
+        "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 1.88e-05
     },
     "amazon.titan-embed-text-v1": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 8192,
         "max_tokens": 8192,
         "mode": "embedding",
         "output_cost_per_token": 0.0,
         "output_vector_size": 1536
     },
+    "amazon.titan-embed-text-v2:0": {
+        "input_cost_per_token": 2e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0,
+        "output_vector_size": 1024
+    },
     "amazon.titan-text-express-v1": {
         "input_cost_per_token": 1.3e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 42000,
+        "max_output_tokens": 8000,
         "max_tokens": 8000,
         "mode": "chat",
         "output_cost_per_token": 1.7e-06
     },
     "amazon.titan-text-lite-v1": {
         "input_cost_per_token": 3e-07,
         "litellm_provider": "bedrock",
-        "max_tokens": 8000,
+        "max_input_tokens": 42000,
+        "max_output_tokens": 4000,
+        "max_tokens": 4000,
         "mode": "chat",
         "output_cost_per_token": 4e-07
     },
     "anthropic.claude-3-haiku-20240307-v1:0": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 200000,
         "max_output_tokens": 4096,
-        "max_tokens": 200000,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.25e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "anthropic.claude-3-opus-20240229-v1:0": {
+        "input_cost_per_token": 1.5e-05,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-06
+        "output_cost_per_token": 7.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "anthropic.claude-3-sonnet-20240229-v1:0": {
         "input_cost_per_token": 3e-06,
         "litellm_provider": "bedrock",
         "max_input_tokens": 200000,
         "max_output_tokens": 4096,
-        "max_tokens": 200000,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.5e-05
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "anthropic.claude-instant-v1": {
         "input_cost_per_token": 1.63e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 5.51e-06
     },
     "anthropic.claude-v1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "anthropic.claude-v2": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "anthropic.claude-v2:1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 200000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "anyscale/HuggingFaceH4/zephyr-7b-beta": {
         "input_cost_per_token": 1.5e-07,
         "litellm_provider": "anyscale",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 16384,
         "max_tokens": 16384,
         "mode": "chat",
         "output_cost_per_token": 1.5e-07
     },
-    "anyscale/Mixtral-8x7B-Instruct-v0.1": {
-        "input_cost_per_token": 1.5e-07,
+    "anyscale/codellama/CodeLlama-34b-Instruct-hf": {
+        "input_cost_per_token": 1e-06,
         "litellm_provider": "anyscale",
-        "max_tokens": 16384,
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.5e-07,
-        "supports_function_calling": true
+        "output_cost_per_token": 1e-06
     },
-    "anyscale/codellama/CodeLlama-34b-Instruct-hf": {
+    "anyscale/codellama/CodeLlama-70b-Instruct-hf": {
         "input_cost_per_token": 1e-06,
         "litellm_provider": "anyscale",
-        "max_tokens": 16384,
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1e-06
+        "output_cost_per_token": 1e-06,
+        "source": "https://docs.anyscale.com/preview/endpoints/text-generation/supported-models/codellama-CodeLlama-70b-Instruct-hf"
+    },
+    "anyscale/google/gemma-7b-it": {
+        "input_cost_per_token": 1.5e-07,
+        "litellm_provider": "anyscale",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-07,
+        "source": "https://docs.anyscale.com/preview/endpoints/text-generation/supported-models/google-gemma-7b-it"
     },
     "anyscale/meta-llama/Llama-2-13b-chat-hf": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "anyscale",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.5e-07
     },
     "anyscale/meta-llama/Llama-2-70b-chat-hf": {
         "input_cost_per_token": 1e-06,
         "litellm_provider": "anyscale",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1e-06
     },
     "anyscale/meta-llama/Llama-2-7b-chat-hf": {
         "input_cost_per_token": 1.5e-07,
         "litellm_provider": "anyscale",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.5e-07
     },
+    "anyscale/meta-llama/Meta-Llama-3-70B-Instruct": {
+        "input_cost_per_token": 1e-06,
+        "litellm_provider": "anyscale",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 1e-06,
+        "source": "https://docs.anyscale.com/preview/endpoints/text-generation/supported-models/meta-llama-Meta-Llama-3-70B-Instruct"
+    },
+    "anyscale/meta-llama/Meta-Llama-3-8B-Instruct": {
+        "input_cost_per_token": 1.5e-07,
+        "litellm_provider": "anyscale",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-07,
+        "source": "https://docs.anyscale.com/preview/endpoints/text-generation/supported-models/meta-llama-Meta-Llama-3-8B-Instruct"
+    },
     "anyscale/mistralai/Mistral-7B-Instruct-v0.1": {
         "input_cost_per_token": 1.5e-07,
         "litellm_provider": "anyscale",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 16384,
+        "max_tokens": 16384,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-07,
+        "source": "https://docs.anyscale.com/preview/endpoints/text-generation/supported-models/mistralai-Mistral-7B-Instruct-v0.1",
+        "supports_function_calling": true
+    },
+    "anyscale/mistralai/Mixtral-8x22B-Instruct-v0.1": {
+        "input_cost_per_token": 9e-07,
+        "litellm_provider": "anyscale",
+        "max_input_tokens": 65536,
+        "max_output_tokens": 65536,
+        "max_tokens": 65536,
+        "mode": "chat",
+        "output_cost_per_token": 9e-07,
+        "source": "https://docs.anyscale.com/preview/endpoints/text-generation/supported-models/mistralai-Mixtral-8x22B-Instruct-v0.1",
+        "supports_function_calling": true
+    },
+    "anyscale/mistralai/Mixtral-8x7B-Instruct-v0.1": {
+        "input_cost_per_token": 1.5e-07,
+        "litellm_provider": "anyscale",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 16384,
         "max_tokens": 16384,
         "mode": "chat",
         "output_cost_per_token": 1.5e-07,
+        "source": "https://docs.anyscale.com/preview/endpoints/text-generation/supported-models/mistralai-Mixtral-8x7B-Instruct-v0.1",
         "supports_function_calling": true
     },
     "azure/ada": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "azure",
+        "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
+    "azure/command-r-plus": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "azure",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true
+    },
     "azure/gpt-3.5-turbo-instruct-0914": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "text-completion-openai",
+        "max_input_tokens": 4097,
         "max_tokens": 4097,
         "mode": "completion",
         "output_cost_per_token": 2e-06
     },
     "azure/gpt-35-turbo": {
-        "input_cost_per_token": 1.5e-06,
+        "input_cost_per_token": 5e-07,
         "litellm_provider": "azure",
         "max_input_tokens": 4097,
         "max_output_tokens": 4096,
-        "max_tokens": 4097,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 2e-06,
+        "output_cost_per_token": 1.5e-06,
         "supports_function_calling": true
     },
     "azure/gpt-35-turbo-0125": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "azure",
         "max_input_tokens": 16384,
         "max_output_tokens": 4096,
-        "max_tokens": 16384,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.5e-06,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
     "azure/gpt-35-turbo-1106": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "azure",
         "max_input_tokens": 16384,
         "max_output_tokens": 4096,
-        "max_tokens": 16384,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2e-06,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
     "azure/gpt-35-turbo-16k": {
         "input_cost_per_token": 3e-06,
         "litellm_provider": "azure",
         "max_input_tokens": 16385,
         "max_output_tokens": 4096,
-        "max_tokens": 16385,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 4e-06
     },
     "azure/gpt-35-turbo-16k-0613": {
         "input_cost_per_token": 3e-06,
         "litellm_provider": "azure",
         "max_input_tokens": 16385,
         "max_output_tokens": 4096,
-        "max_tokens": 16385,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 4e-06,
         "supports_function_calling": true
     },
     "azure/gpt-35-turbo-instruct": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "text-completion-openai",
+        "max_input_tokens": 4097,
         "max_tokens": 4097,
         "mode": "completion",
         "output_cost_per_token": 2e-06
     },
     "azure/gpt-4": {
         "input_cost_per_token": 3e-05,
         "litellm_provider": "azure",
         "max_input_tokens": 8192,
         "max_output_tokens": 4096,
-        "max_tokens": 8192,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-05,
         "supports_function_calling": true
     },
     "azure/gpt-4-0125-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "azure",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 128000,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 3e-05,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
     "azure/gpt-4-0613": {
         "input_cost_per_token": 3e-05,
         "litellm_provider": "azure",
         "max_input_tokens": 8192,
         "max_output_tokens": 4096,
-        "max_tokens": 8192,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-05,
         "supports_function_calling": true
     },
     "azure/gpt-4-1106-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "azure",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 128000,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 3e-05,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
     "azure/gpt-4-32k": {
         "input_cost_per_token": 6e-05,
         "litellm_provider": "azure",
         "max_input_tokens": 32768,
         "max_output_tokens": 4096,
-        "max_tokens": 32768,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.00012
     },
     "azure/gpt-4-32k-0613": {
         "input_cost_per_token": 6e-05,
         "litellm_provider": "azure",
         "max_input_tokens": 32768,
         "max_output_tokens": 4096,
-        "max_tokens": 32768,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.00012
     },
     "azure/gpt-4-turbo": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "azure",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 128000,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 3e-05,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
+    "azure/gpt-4-turbo-2024-04-09": {
+        "input_cost_per_token": 1e-05,
+        "litellm_provider": "azure",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 3e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
     "azure/gpt-4-turbo-vision-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "azure",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 128000,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 3e-05
+        "output_cost_per_token": 3e-05,
+        "supports_vision": true
     },
     "azure/hd/1024-x-1024/dall-e-3": {
         "input_cost_per_pixel": 7.629e-08,
         "litellm_provider": "azure",
         "mode": "image_generation",
         "output_cost_per_token": 0.0
     },
@@ -350,22 +481,24 @@
         "litellm_provider": "azure",
         "mode": "image_generation",
         "output_cost_per_token": 0.0
     },
     "azure/mistral-large-2402": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "azure",
+        "max_input_tokens": 32000,
         "max_tokens": 32000,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05,
         "supports_function_calling": true
     },
     "azure/mistral-large-latest": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "azure",
+        "max_input_tokens": 32000,
         "max_tokens": 32000,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05,
         "supports_function_calling": true
     },
     "azure/standard/1024-x-1024/dall-e-2": {
         "input_cost_per_pixel": 0.0,
@@ -390,28 +523,31 @@
         "litellm_provider": "azure",
         "mode": "image_generation",
         "output_cost_per_token": 0.0
     },
     "azure/text-embedding-3-large": {
         "input_cost_per_token": 1.3e-07,
         "litellm_provider": "azure",
+        "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
     "azure/text-embedding-3-small": {
         "input_cost_per_token": 2e-08,
         "litellm_provider": "azure",
+        "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
     "azure/text-embedding-ada-002": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "azure",
+        "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
     "azure/whisper-1": {
         "input_cost_per_second": 0,
         "litellm_provider": "azure",
@@ -426,945 +562,1442 @@
         "max_tokens": 16384,
         "mode": "completion",
         "output_cost_per_token": 4e-07
     },
     "bedrock/*/1-month-commitment/cohere.command-light-text-v14": {
         "input_cost_per_second": 0.001902,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_second": 0.001902
     },
     "bedrock/*/1-month-commitment/cohere.command-text-v14": {
         "input_cost_per_second": 0.011,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_second": 0.011
     },
     "bedrock/*/6-month-commitment/cohere.command-light-text-v14": {
         "input_cost_per_second": 0.0011416,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_second": 0.0011416
     },
     "bedrock/*/6-month-commitment/cohere.command-text-v14": {
         "input_cost_per_second": 0.0066027,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_second": 0.0066027
     },
     "bedrock/ap-northeast-1/1-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.01475,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.01475
     },
     "bedrock/ap-northeast-1/1-month-commitment/anthropic.claude-v1": {
         "input_cost_per_second": 0.0455,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0455
     },
     "bedrock/ap-northeast-1/1-month-commitment/anthropic.claude-v2": {
         "input_cost_per_second": 0.0455,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0455
     },
     "bedrock/ap-northeast-1/1-month-commitment/anthropic.claude-v2:1": {
         "input_cost_per_second": 0.0455,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0455
     },
     "bedrock/ap-northeast-1/6-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.008194,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.008194
     },
     "bedrock/ap-northeast-1/6-month-commitment/anthropic.claude-v1": {
         "input_cost_per_second": 0.02527,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.02527
     },
     "bedrock/ap-northeast-1/6-month-commitment/anthropic.claude-v2": {
         "input_cost_per_second": 0.02527,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.02527
     },
     "bedrock/ap-northeast-1/6-month-commitment/anthropic.claude-v2:1": {
         "input_cost_per_second": 0.02527,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.02527
     },
     "bedrock/ap-northeast-1/anthropic.claude-instant-v1": {
         "input_cost_per_token": 2.23e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 7.55e-06
     },
     "bedrock/ap-northeast-1/anthropic.claude-v1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "bedrock/ap-northeast-1/anthropic.claude-v2": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "bedrock/ap-northeast-1/anthropic.claude-v2:1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "bedrock/eu-central-1/1-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.01635,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.01635
     },
     "bedrock/eu-central-1/1-month-commitment/anthropic.claude-v1": {
         "input_cost_per_second": 0.0415,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0415
     },
     "bedrock/eu-central-1/1-month-commitment/anthropic.claude-v2": {
         "input_cost_per_second": 0.0415,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0415
     },
     "bedrock/eu-central-1/1-month-commitment/anthropic.claude-v2:1": {
         "input_cost_per_second": 0.0415,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0415
     },
     "bedrock/eu-central-1/6-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.009083,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.009083
     },
     "bedrock/eu-central-1/6-month-commitment/anthropic.claude-v1": {
         "input_cost_per_second": 0.02305,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.02305
     },
     "bedrock/eu-central-1/6-month-commitment/anthropic.claude-v2": {
         "input_cost_per_second": 0.02305,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.02305
     },
     "bedrock/eu-central-1/6-month-commitment/anthropic.claude-v2:1": {
         "input_cost_per_second": 0.02305,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.02305
     },
     "bedrock/eu-central-1/anthropic.claude-instant-v1": {
         "input_cost_per_token": 2.48e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 8.38e-06
     },
     "bedrock/eu-central-1/anthropic.claude-v1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "bedrock/eu-central-1/anthropic.claude-v2": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "bedrock/eu-central-1/anthropic.claude-v2:1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
+    "bedrock/eu-west-3/mistral.mistral-7b-instruct-v0:2": {
+        "input_cost_per_token": 2e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2.6e-07
+    },
+    "bedrock/eu-west-3/mistral.mistral-large-2402-v1:0": {
+        "input_cost_per_token": 1.04e-05,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 3.12e-05
+    },
+    "bedrock/eu-west-3/mistral.mixtral-8x7b-instruct-v0:1": {
+        "input_cost_per_token": 5.9e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 9.1e-07
+    },
     "bedrock/us-east-1/1-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.011,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.011
     },
     "bedrock/us-east-1/1-month-commitment/anthropic.claude-v1": {
         "input_cost_per_second": 0.0175,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0175
     },
     "bedrock/us-east-1/1-month-commitment/anthropic.claude-v2": {
         "input_cost_per_second": 0.0175,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0175
     },
     "bedrock/us-east-1/1-month-commitment/anthropic.claude-v2:1": {
         "input_cost_per_second": 0.0175,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0175
     },
     "bedrock/us-east-1/6-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.00611,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.00611
     },
     "bedrock/us-east-1/6-month-commitment/anthropic.claude-v1": {
         "input_cost_per_second": 0.00972,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.00972
     },
     "bedrock/us-east-1/6-month-commitment/anthropic.claude-v2": {
         "input_cost_per_second": 0.00972,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.00972
     },
     "bedrock/us-east-1/6-month-commitment/anthropic.claude-v2:1": {
         "input_cost_per_second": 0.00972,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.00972
     },
     "bedrock/us-east-1/anthropic.claude-instant-v1": {
         "input_cost_per_token": 8e-07,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-06
     },
     "bedrock/us-east-1/anthropic.claude-v1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "bedrock/us-east-1/anthropic.claude-v2": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "bedrock/us-east-1/anthropic.claude-v2:1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2.4e-05
+    },
+    "bedrock/us-east-1/mistral.mistral-7b-instruct-v0:2": {
+        "input_cost_per_token": 1.5e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2e-07
+    },
+    "bedrock/us-east-1/mistral.mistral-large-2402-v1:0": {
+        "input_cost_per_token": 8e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
+    "bedrock/us-east-1/mistral.mixtral-8x7b-instruct-v0:1": {
+        "input_cost_per_token": 4.5e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 7e-07
+    },
     "bedrock/us-west-2/1-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.011,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.011
     },
     "bedrock/us-west-2/1-month-commitment/anthropic.claude-v1": {
         "input_cost_per_second": 0.0175,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0175
     },
     "bedrock/us-west-2/1-month-commitment/anthropic.claude-v2": {
         "input_cost_per_second": 0.0175,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0175
     },
     "bedrock/us-west-2/1-month-commitment/anthropic.claude-v2:1": {
         "input_cost_per_second": 0.0175,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.0175
     },
     "bedrock/us-west-2/6-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.00611,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.00611
     },
     "bedrock/us-west-2/6-month-commitment/anthropic.claude-v1": {
         "input_cost_per_second": 0.00972,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.00972
     },
     "bedrock/us-west-2/6-month-commitment/anthropic.claude-v2": {
         "input_cost_per_second": 0.00972,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.00972
     },
     "bedrock/us-west-2/6-month-commitment/anthropic.claude-v2:1": {
         "input_cost_per_second": 0.00972,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_second": 0.00972
     },
     "bedrock/us-west-2/anthropic.claude-instant-v1": {
         "input_cost_per_token": 8e-07,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-06
     },
     "bedrock/us-west-2/anthropic.claude-v1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "bedrock/us-west-2/anthropic.claude-v2": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "bedrock/us-west-2/anthropic.claude-v2:1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
-    "bedrock/us-west-2/mistral.mistral-7b-instruct": {
+    "bedrock/us-west-2/mistral.mistral-7b-instruct-v0:2": {
         "input_cost_per_token": 1.5e-07,
         "litellm_provider": "bedrock",
-        "max_tokens": 32000,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2e-07
     },
-    "bedrock/us-west-2/mistral.mixtral-8x7b-instruct": {
+    "bedrock/us-west-2/mistral.mistral-large-2402-v1:0": {
+        "input_cost_per_token": 8e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2.4e-05
+    },
+    "bedrock/us-west-2/mistral.mixtral-8x7b-instruct-v0:1": {
         "input_cost_per_token": 4.5e-07,
         "litellm_provider": "bedrock",
-        "max_tokens": 32000,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 7e-07
     },
     "chat-bison": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-chat-models",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "chat-bison-32k": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-chat-models",
-        "max_tokens": 32000,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "chat-bison@001": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-chat-models",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "chat-bison@002": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-chat-models",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "chatdolphin": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "nlp_cloud",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 16384,
         "max_tokens": 16384,
         "mode": "chat",
         "output_cost_per_token": 5e-07
     },
     "claude-2": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "anthropic",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "claude-2.1": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "anthropic",
+        "max_input_tokens": 200000,
         "max_output_tokens": 8191,
-        "max_tokens": 200000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
     "claude-3-haiku-20240307": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "anthropic",
+        "max_input_tokens": 200000,
         "max_output_tokens": 4096,
-        "max_tokens": 200000,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-06
+        "output_cost_per_token": 1.25e-06,
+        "supports_function_calling": true,
+        "supports_vision": true,
+        "tool_use_system_prompt_tokens": 264
     },
     "claude-3-opus-20240229": {
         "input_cost_per_token": 1.5e-05,
         "litellm_provider": "anthropic",
+        "max_input_tokens": 200000,
         "max_output_tokens": 4096,
-        "max_tokens": 200000,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 7.5e-05
+        "output_cost_per_token": 7.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true,
+        "tool_use_system_prompt_tokens": 395
     },
     "claude-3-sonnet-20240229": {
         "input_cost_per_token": 3e-06,
         "litellm_provider": "anthropic",
+        "max_input_tokens": 200000,
         "max_output_tokens": 4096,
-        "max_tokens": 200000,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.5e-05
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true,
+        "tool_use_system_prompt_tokens": 159
     },
     "claude-instant-1": {
         "input_cost_per_token": 1.63e-06,
         "litellm_provider": "anthropic",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 5.51e-06
     },
     "claude-instant-1.2": {
         "input_cost_per_token": 1.63e-07,
         "litellm_provider": "anthropic",
+        "max_input_tokens": 100000,
         "max_output_tokens": 8191,
-        "max_tokens": 100000,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 5.51e-07
     },
     "cloudflare/@cf/meta/llama-2-7b-chat-fp16": {
         "input_cost_per_token": 1.923e-06,
         "litellm_provider": "cloudflare",
+        "max_input_tokens": 3072,
+        "max_output_tokens": 3072,
         "max_tokens": 3072,
         "mode": "chat",
         "output_cost_per_token": 1.923e-06
     },
     "cloudflare/@cf/meta/llama-2-7b-chat-int8": {
         "input_cost_per_token": 1.923e-06,
         "litellm_provider": "cloudflare",
+        "max_input_tokens": 2048,
+        "max_output_tokens": 2048,
         "max_tokens": 2048,
         "mode": "chat",
         "output_cost_per_token": 1.923e-06
     },
     "cloudflare/@cf/mistral/mistral-7b-instruct-v0.1": {
         "input_cost_per_token": 1.923e-06,
         "litellm_provider": "cloudflare",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 1.923e-06
     },
     "cloudflare/@hf/thebloke/codellama-7b-instruct-awq": {
         "input_cost_per_token": 1.923e-06,
         "litellm_provider": "cloudflare",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.923e-06
     },
     "code-bison": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-code-text-models",
-        "max_tokens": 6144,
+        "max_input_tokens": 6144,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "code-bison@001": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-code-text-models",
-        "max_tokens": 6144,
+        "max_input_tokens": 6144,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "code-gecko": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-code-text-models",
-        "max_tokens": 2048,
+        "max_input_tokens": 2048,
+        "max_output_tokens": 64,
+        "max_tokens": 64,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "code-gecko@001": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-code-text-models",
-        "max_tokens": 2048,
+        "max_input_tokens": 2048,
+        "max_output_tokens": 64,
+        "max_tokens": 64,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "code-gecko@002": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-code-text-models",
-        "max_tokens": 2048,
+        "max_input_tokens": 2048,
+        "max_output_tokens": 64,
+        "max_tokens": 64,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "codechat-bison": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-code-chat-models",
-        "max_tokens": 6144,
+        "max_input_tokens": 6144,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "codechat-bison-32k": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-code-chat-models",
-        "max_tokens": 32000,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "codechat-bison@001": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-code-chat-models",
-        "max_tokens": 6144,
+        "max_input_tokens": 6144,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "cohere.command-light-text-v14": {
         "input_cost_per_token": 3e-07,
         "litellm_provider": "bedrock",
-        "max_tokens": 4000,
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-07
     },
+    "cohere.command-r-plus-v1:0": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05
+    },
+    "cohere.command-r-v1:0": {
+        "input_cost_per_token": 5e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-06
+    },
     "cohere.command-text-v14": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2e-06
     },
     "cohere.embed-english-v3": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 512,
         "max_tokens": 512,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
     "cohere.embed-multilingual-v3": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 512,
         "max_tokens": 512,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
     "command": {
         "input_cost_per_token": 1.5e-05,
         "litellm_provider": "cohere",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 1.5e-05
     },
     "command-light": {
         "input_cost_per_token": 1.5e-05,
         "litellm_provider": "cohere_chat",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.5e-05
     },
     "command-medium-beta": {
         "input_cost_per_token": 1.5e-05,
         "litellm_provider": "cohere",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 1.5e-05
     },
     "command-nightly": {
         "input_cost_per_token": 1.5e-05,
         "litellm_provider": "cohere",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 1.5e-05
     },
     "command-r": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "cohere_chat",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 128000,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.5e-06
+        "output_cost_per_token": 1.5e-06,
+        "supports_function_calling": true
+    },
+    "command-r-plus": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "cohere_chat",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true
     },
     "command-xlarge-beta": {
         "input_cost_per_token": 1.5e-05,
         "litellm_provider": "cohere",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 1.5e-05
     },
+    "databricks/databricks-bge-large-en": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "databricks",
+        "max_input_tokens": 512,
+        "max_tokens": 512,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0,
+        "output_vector_size": 1024,
+        "source": "https://www.databricks.com/product/pricing/foundation-model-serving"
+    },
+    "databricks/databricks-dbrx-instruct": {
+        "input_cost_per_token": 7.5e-07,
+        "litellm_provider": "databricks",
+        "max_input_tokens": 32768,
+        "max_output_tokens": 32768,
+        "max_tokens": 32768,
+        "mode": "chat",
+        "output_cost_per_token": 2.25e-06,
+        "source": "https://www.databricks.com/product/pricing/foundation-model-serving"
+    },
+    "databricks/databricks-llama-2-70b-chat": {
+        "input_cost_per_token": 5e-07,
+        "litellm_provider": "databricks",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-06,
+        "source": "https://www.databricks.com/product/pricing/foundation-model-serving"
+    },
+    "databricks/databricks-meta-llama-3-70b-instruct": {
+        "input_cost_per_token": 1e-06,
+        "litellm_provider": "databricks",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 3e-06,
+        "source": "https://www.databricks.com/product/pricing/foundation-model-serving"
+    },
+    "databricks/databricks-mixtral-8x7b-instruct": {
+        "input_cost_per_token": 5e-07,
+        "litellm_provider": "databricks",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1e-06,
+        "source": "https://www.databricks.com/product/pricing/foundation-model-serving"
+    },
+    "databricks/databricks-mpt-30b-instruct": {
+        "input_cost_per_token": 1e-06,
+        "litellm_provider": "databricks",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 1e-06,
+        "source": "https://www.databricks.com/product/pricing/foundation-model-serving"
+    },
+    "databricks/databricks-mpt-7b-instruct": {
+        "input_cost_per_token": 5e-07,
+        "litellm_provider": "databricks",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07,
+        "source": "https://www.databricks.com/product/pricing/foundation-model-serving"
+    },
     "davinci-002": {
         "input_cost_per_token": 2e-06,
         "litellm_provider": "text-completion-openai",
         "max_input_tokens": 16384,
         "max_output_tokens": 4096,
         "max_tokens": 16384,
         "mode": "completion",
         "output_cost_per_token": 2e-06
     },
     "deepinfra/01-ai/Yi-34B-200K": {
         "input_cost_per_token": 6e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 6e-07
     },
     "deepinfra/01-ai/Yi-34B-Chat": {
         "input_cost_per_token": 6e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-07
     },
     "deepinfra/01-ai/Yi-6B-200K": {
         "input_cost_per_token": 1.3e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 1.3e-07
     },
     "deepinfra/Gryphe/MythoMax-L2-13b": {
         "input_cost_per_token": 2.2e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.2e-07
     },
     "deepinfra/Phind/Phind-CodeLlama-34B-v2": {
         "input_cost_per_token": 6e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-07
     },
     "deepinfra/amazon/MistralLite": {
         "input_cost_per_token": 2e-07,
         "litellm_provider": "deepinfra",
-        "max_tokens": 32768,
+        "max_input_tokens": 32768,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2e-07
     },
     "deepinfra/codellama/CodeLlama-34b-Instruct-hf": {
         "input_cost_per_token": 6e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-07
     },
     "deepinfra/cognitivecomputations/dolphin-2.6-mixtral-8x7b": {
         "input_cost_per_token": 2.7e-07,
         "litellm_provider": "deepinfra",
-        "max_tokens": 32768,
+        "max_input_tokens": 32768,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.7e-07
     },
     "deepinfra/deepinfra/airoboros-70b": {
         "input_cost_per_token": 7e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 9e-07
     },
     "deepinfra/deepinfra/mixtral": {
         "input_cost_per_token": 2.7e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 2.7e-07
     },
     "deepinfra/jondurbin/airoboros-l2-70b-gpt4-1.4.1": {
         "input_cost_per_token": 7e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 9e-07
     },
     "deepinfra/lizpreciatior/lzlv_70b_fp16_hf": {
         "input_cost_per_token": 7e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 9e-07
     },
     "deepinfra/meta-llama/Llama-2-13b-chat-hf": {
         "input_cost_per_token": 2.2e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.2e-07
     },
     "deepinfra/meta-llama/Llama-2-70b-chat-hf": {
         "input_cost_per_token": 7e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 9e-07
     },
     "deepinfra/meta-llama/Llama-2-7b-chat-hf": {
         "input_cost_per_token": 1.3e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.3e-07
     },
     "deepinfra/mistralai/Mistral-7B-Instruct-v0.1": {
         "input_cost_per_token": 1.3e-07,
         "litellm_provider": "deepinfra",
-        "max_tokens": 32768,
+        "max_input_tokens": 32768,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 1.3e-07
     },
     "deepinfra/mistralai/Mixtral-8x7B-Instruct-v0.1": {
         "input_cost_per_token": 2.7e-07,
         "litellm_provider": "deepinfra",
-        "max_tokens": 32768,
+        "max_input_tokens": 32768,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.7e-07
     },
     "deepinfra/openchat/openchat_3.5": {
         "input_cost_per_token": 1.3e-07,
         "litellm_provider": "deepinfra",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.3e-07
     },
+    "deepseek-chat": {
+        "input_cost_per_token": 1.4e-07,
+        "litellm_provider": "deepseek",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.8e-07
+    },
+    "deepseek-coder": {
+        "input_cost_per_token": 1.4e-07,
+        "litellm_provider": "deepseek",
+        "max_input_tokens": 16000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.8e-07
+    },
     "dolphin": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "nlp_cloud",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 16384,
         "max_tokens": 16384,
         "mode": "completion",
         "output_cost_per_token": 5e-07
     },
+    "ft:babbage-002": {
+        "input_cost_per_token": 4e-07,
+        "litellm_provider": "text-completion-openai",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 4096,
+        "max_tokens": 16384,
+        "mode": "completion",
+        "output_cost_per_token": 4e-07
+    },
+    "ft:davinci-002": {
+        "input_cost_per_token": 2e-06,
+        "litellm_provider": "text-completion-openai",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 4096,
+        "max_tokens": 16384,
+        "mode": "completion",
+        "output_cost_per_token": 2e-06
+    },
     "ft:gpt-3.5-turbo": {
         "input_cost_per_token": 3e-06,
         "litellm_provider": "openai",
         "max_input_tokens": 4097,
         "max_output_tokens": 4096,
         "max_tokens": 4097,
         "mode": "chat",
         "output_cost_per_token": 6e-06
     },
     "gemini-1.0-pro": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "vertex_ai-language-models",
+        "max_input_tokens": 32760,
         "max_output_tokens": 8192,
-        "max_tokens": 32760,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true
+    },
+    "gemini-1.0-pro-001": {
+        "input_cost_per_token": 2.5e-07,
+        "litellm_provider": "vertex_ai-language-models",
+        "max_input_tokens": 32760,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true
+    },
+    "gemini-1.0-pro-002": {
+        "input_cost_per_token": 2.5e-07,
+        "litellm_provider": "vertex_ai-language-models",
+        "max_input_tokens": 32760,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 5e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
         "supports_function_calling": true
     },
     "gemini-1.0-pro-vision": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "vertex_ai-vision-models",
         "max_images_per_prompt": 16,
+        "max_input_tokens": 16384,
         "max_output_tokens": 2048,
-        "max_tokens": 16384,
+        "max_tokens": 2048,
         "max_video_length": 2,
         "max_videos_per_prompt": 1,
         "mode": "chat",
-        "output_cost_per_token": 5e-07
+        "output_cost_per_token": 5e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "gemini-1.0-pro-vision-001": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "vertex_ai-vision-models",
         "max_images_per_prompt": 16,
+        "max_input_tokens": 16384,
         "max_output_tokens": 2048,
-        "max_tokens": 16384,
+        "max_tokens": 2048,
         "max_video_length": 2,
         "max_videos_per_prompt": 1,
         "mode": "chat",
-        "output_cost_per_token": 5e-07
+        "output_cost_per_token": 5e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_vision": true
     },
-    "gemini-1.5-pro": {
+    "gemini-1.5-flash-preview-0514": {
         "input_cost_per_token": 0,
         "litellm_provider": "vertex_ai-language-models",
+        "max_audio_length_hours": 8.4,
+        "max_audio_per_prompt": 1,
+        "max_images_per_prompt": 3000,
+        "max_input_tokens": 1000000,
+        "max_output_tokens": 8192,
+        "max_pdf_size_mb": 30,
+        "max_tokens": 8192,
+        "max_video_length": 1,
+        "max_videos_per_prompt": 10,
+        "mode": "chat",
+        "output_cost_per_token": 0,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "gemini-1.5-pro": {
+        "input_cost_per_token": 6.25e-07,
+        "litellm_provider": "vertex_ai-language-models",
         "max_input_tokens": 1000000,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 0
+        "output_cost_per_token": 1.875e-06,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_tool_choice": true
     },
     "gemini-1.5-pro-preview-0215": {
-        "input_cost_per_token": 0,
+        "input_cost_per_token": 6.25e-07,
+        "litellm_provider": "vertex_ai-language-models",
+        "max_input_tokens": 1000000,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 1.875e-06,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_tool_choice": true
+    },
+    "gemini-1.5-pro-preview-0409": {
+        "input_cost_per_token": 6.25e-07,
+        "litellm_provider": "vertex_ai-language-models",
+        "max_input_tokens": 1000000,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 1.875e-06,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_tool_choice": true
+    },
+    "gemini-1.5-pro-preview-0514": {
+        "input_cost_per_token": 6.25e-07,
         "litellm_provider": "vertex_ai-language-models",
         "max_input_tokens": 1000000,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 0
+        "output_cost_per_token": 1.875e-06,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_tool_choice": true
     },
-    "gemini-1.5-pro-vision": {
+    "gemini-experimental": {
         "input_cost_per_token": 0,
-        "litellm_provider": "vertex_ai-vision-models",
-        "max_images_per_prompt": 16,
+        "litellm_provider": "vertex_ai-language-models",
         "max_input_tokens": 1000000,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
-        "max_video_length": 2,
-        "max_videos_per_prompt": 1,
         "mode": "chat",
-        "output_cost_per_token": 0
+        "output_cost_per_token": 0,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": false,
+        "supports_tool_choice": true
     },
     "gemini-pro": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "vertex_ai-language-models",
-        "max_output_tokens": 2048,
-        "max_tokens": 32760,
+        "max_input_tokens": 32760,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 5e-07
+        "output_cost_per_token": 5e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true
     },
     "gemini-pro-vision": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "vertex_ai-vision-models",
+        "max_images_per_prompt": 16,
+        "max_input_tokens": 16384,
         "max_output_tokens": 2048,
-        "max_tokens": 16384,
+        "max_tokens": 2048,
+        "max_video_length": 2,
+        "max_videos_per_prompt": 1,
         "mode": "chat",
-        "output_cost_per_token": 5e-07
+        "output_cost_per_token": 5e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "gemini/gemini-1.5-flash-latest": {
+        "input_cost_per_token": 0,
+        "litellm_provider": "vertex_ai-language-models",
+        "max_audio_length_hours": 8.4,
+        "max_audio_per_prompt": 1,
+        "max_images_per_prompt": 3000,
+        "max_input_tokens": 1000000,
+        "max_output_tokens": 8192,
+        "max_pdf_size_mb": 30,
+        "max_tokens": 8192,
+        "max_video_length": 1,
+        "max_videos_per_prompt": 10,
+        "mode": "chat",
+        "output_cost_per_token": 0,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "gemini/gemini-1.5-pro": {
         "input_cost_per_token": 0,
         "litellm_provider": "gemini",
         "max_input_tokens": 1000000,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 0
+        "output_cost_per_token": 0,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_tool_choice": true,
+        "supports_vision": true
     },
-    "gemini/gemini-1.5-pro-vision": {
+    "gemini/gemini-1.5-pro-latest": {
         "input_cost_per_token": 0,
         "litellm_provider": "gemini",
-        "max_input_tokens": 1000000,
+        "max_input_tokens": 1048576,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 0
+        "output_cost_per_token": 0,
+        "source": "https://ai.google.dev/models/gemini",
+        "supports_function_calling": true,
+        "supports_tool_choice": true,
+        "supports_vision": true
     },
     "gemini/gemini-pro": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "gemini",
-        "max_output_tokens": 2048,
-        "max_tokens": 30720,
+        "max_input_tokens": 32760,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 0.0
+        "output_cost_per_token": 0.0,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true
     },
     "gemini/gemini-pro-vision": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "gemini",
+        "max_input_tokens": 30720,
         "max_output_tokens": 2048,
-        "max_tokens": 30720,
+        "max_tokens": 2048,
         "mode": "chat",
-        "output_cost_per_token": 0.0
+        "output_cost_per_token": 0.0,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "gpt-3.5-turbo": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "openai",
         "max_input_tokens": 16385,
         "max_output_tokens": 4096,
         "max_tokens": 4097,
@@ -1432,152 +2065,233 @@
         "output_cost_per_token": 4e-06
     },
     "gpt-3.5-turbo-instruct": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "text-completion-openai",
         "max_input_tokens": 8192,
         "max_output_tokens": 4096,
-        "max_tokens": 8192,
+        "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 2e-06
     },
     "gpt-3.5-turbo-instruct-0914": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "text-completion-openai",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 4097,
         "max_tokens": 4097,
         "mode": "completion",
         "output_cost_per_token": 2e-06
     },
     "gpt-4": {
         "input_cost_per_token": 3e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 8192,
         "max_output_tokens": 4096,
-        "max_tokens": 8192,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-05,
         "supports_function_calling": true
     },
     "gpt-4-0125-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 128000,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 3e-05,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
     "gpt-4-0314": {
         "input_cost_per_token": 3e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 8192,
         "max_output_tokens": 4096,
-        "max_tokens": 8192,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-05
     },
     "gpt-4-0613": {
         "input_cost_per_token": 3e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 8192,
         "max_output_tokens": 4096,
-        "max_tokens": 8192,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-05,
         "supports_function_calling": true
     },
     "gpt-4-1106-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 128000,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 3e-05,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
     "gpt-4-1106-vision-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 128000,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 3e-05
+        "output_cost_per_token": 3e-05,
+        "supports_vision": true
     },
     "gpt-4-32k": {
         "input_cost_per_token": 6e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 32768,
         "max_output_tokens": 4096,
-        "max_tokens": 32768,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.00012
     },
     "gpt-4-32k-0314": {
         "input_cost_per_token": 6e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 32768,
         "max_output_tokens": 4096,
-        "max_tokens": 32768,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.00012
     },
     "gpt-4-32k-0613": {
         "input_cost_per_token": 6e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 32768,
         "max_output_tokens": 4096,
-        "max_tokens": 32768,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.00012
     },
+    "gpt-4-turbo": {
+        "input_cost_per_token": 1e-05,
+        "litellm_provider": "openai",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 3e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
+    "gpt-4-turbo-2024-04-09": {
+        "input_cost_per_token": 1e-05,
+        "litellm_provider": "openai",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 3e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
     "gpt-4-turbo-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "openai",
-        "max_input_tokens": 8192,
+        "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 8192,
+        "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 3e-05,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
     "gpt-4-vision-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
-        "max_tokens": 128000,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 3e-05,
+        "supports_vision": true
+    },
+    "gpt-4o": {
+        "input_cost_per_token": 5e-06,
+        "litellm_provider": "openai",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 3e-05
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
+    "gpt-4o-2024-05-13": {
+        "input_cost_per_token": 5e-06,
+        "litellm_provider": "openai",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
     },
     "groq/gemma-7b-it": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "groq",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 1e-07
+        "output_cost_per_token": 1e-07,
+        "supports_function_calling": true
     },
     "groq/llama2-70b-4096": {
         "input_cost_per_token": 7e-07,
         "litellm_provider": "groq",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 8e-07
+        "output_cost_per_token": 8e-07,
+        "supports_function_calling": true
+    },
+    "groq/llama3-70b-8192": {
+        "input_cost_per_token": 6.4e-07,
+        "litellm_provider": "groq",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 8e-07,
+        "supports_function_calling": true
+    },
+    "groq/llama3-8b-8192": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "groq",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 1e-07,
+        "supports_function_calling": true
     },
     "groq/mixtral-8x7b-32768": {
         "input_cost_per_token": 2.7e-07,
         "litellm_provider": "groq",
+        "max_input_tokens": 32768,
+        "max_output_tokens": 32768,
         "max_tokens": 32768,
         "mode": "chat",
-        "output_cost_per_token": 2.7e-07
+        "output_cost_per_token": 2.7e-07,
+        "supports_function_calling": true
     },
     "hd/1024-x-1024/dall-e-3": {
         "input_cost_per_pixel": 7.629e-08,
         "litellm_provider": "openai",
         "mode": "image_generation",
         "output_cost_per_pixel": 0.0
     },
@@ -1592,28 +2306,34 @@
         "litellm_provider": "openai",
         "mode": "image_generation",
         "output_cost_per_pixel": 0.0
     },
     "j2-light": {
         "input_cost_per_token": 3e-06,
         "litellm_provider": "ai21",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "completion",
         "output_cost_per_token": 3e-06
     },
     "j2-mid": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "ai21",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "completion",
         "output_cost_per_token": 1e-05
     },
     "j2-ultra": {
         "input_cost_per_token": 1.5e-05,
         "litellm_provider": "ai21",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "completion",
         "output_cost_per_token": 1.5e-05
     },
     "luminous-base": {
         "input_cost_per_token": 3e-05,
         "litellm_provider": "aleph_alpha",
@@ -1669,157 +2389,402 @@
         "max_tokens": 77,
         "mode": "image_generation",
         "output_cost_per_image": 0.072
     },
     "meta.llama2-13b-chat-v1": {
         "input_cost_per_token": 7.5e-07,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1e-06
     },
     "meta.llama2-70b-chat-v1": {
         "input_cost_per_token": 1.95e-06,
         "litellm_provider": "bedrock",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.56e-06
     },
+    "meta.llama3-70b-instruct-v1:0": {
+        "input_cost_per_token": 2.65e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 3.5e-06
+    },
+    "meta.llama3-8b-instruct-v1:0": {
+        "input_cost_per_token": 4e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 6e-07
+    },
     "mistral.mistral-7b-instruct-v0:2": {
         "input_cost_per_token": 1.5e-07,
         "litellm_provider": "bedrock",
-        "max_tokens": 32000,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2e-07
     },
-    "mistral.mixtral-8x7b-instruct": {
+    "mistral.mistral-large-2402-v1:0": {
+        "input_cost_per_token": 8e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2.4e-05
+    },
+    "mistral.mixtral-8x7b-instruct-v0:1": {
         "input_cost_per_token": 4.5e-07,
         "litellm_provider": "bedrock",
-        "max_tokens": 32000,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 7e-07
     },
     "mistral/mistral-embed": {
         "input_cost_per_token": 1.11e-07,
         "litellm_provider": "mistral",
+        "max_input_tokens": 8192,
         "max_tokens": 8192,
         "mode": "embedding"
     },
+    "mistral/mistral-large-2402": {
+        "input_cost_per_token": 8e-06,
+        "litellm_provider": "mistral",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2.4e-05,
+        "supports_function_calling": true
+    },
     "mistral/mistral-large-latest": {
         "input_cost_per_token": 8e-06,
         "litellm_provider": "mistral",
-        "max_tokens": 32000,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05,
         "supports_function_calling": true
     },
     "mistral/mistral-medium": {
-        "input_cost_per_token": 2.73e-06,
+        "input_cost_per_token": 2.7e-06,
         "litellm_provider": "mistral",
-        "max_tokens": 8192,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 8.1e-06
+    },
+    "mistral/mistral-medium-2312": {
+        "input_cost_per_token": 2.7e-06,
+        "litellm_provider": "mistral",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 8.1e-06
+    },
+    "mistral/mistral-medium-latest": {
+        "input_cost_per_token": 2.7e-06,
+        "litellm_provider": "mistral",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
-        "output_cost_per_token": 8.2e-06
+        "output_cost_per_token": 8.1e-06
     },
     "mistral/mistral-small": {
-        "input_cost_per_token": 6.6e-07,
+        "input_cost_per_token": 2e-06,
         "litellm_provider": "mistral",
-        "max_tokens": 8192,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 6e-06,
+        "supports_function_calling": true
+    },
+    "mistral/mistral-small-latest": {
+        "input_cost_per_token": 2e-06,
+        "litellm_provider": "mistral",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
-        "output_cost_per_token": 1.97e-06
+        "output_cost_per_token": 6e-06,
+        "supports_function_calling": true
     },
     "mistral/mistral-tiny": {
         "input_cost_per_token": 1.5e-07,
         "litellm_provider": "mistral",
-        "max_tokens": 8192,
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 4.6e-07
     },
+    "mistral/open-mixtral-8x7b": {
+        "input_cost_per_token": 2e-06,
+        "litellm_provider": "mistral",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 6e-06,
+        "supports_function_calling": true
+    },
     "ollama/codellama": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "ollama",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
     "ollama/llama2": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "ollama",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
     "ollama/llama2-uncensored": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "ollama",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
     "ollama/llama2:13b": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "ollama",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
     "ollama/llama2:70b": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "ollama",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
+    "ollama/llama3": {
+        "input_cost_per_token": 0.0,
+        "litellm_provider": "ollama",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 0.0
+    },
+    "ollama/llama3:70b": {
+        "input_cost_per_token": 0.0,
+        "litellm_provider": "ollama",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 0.0
+    },
     "ollama/mistral": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "ollama",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
+    "ollama/mistral-7B-Instruct-v0.1": {
+        "input_cost_per_token": 0.0,
+        "litellm_provider": "ollama",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 0.0
+    },
+    "ollama/mistral-7B-Instruct-v0.2": {
+        "input_cost_per_token": 0.0,
+        "litellm_provider": "ollama",
+        "max_input_tokens": 32768,
+        "max_output_tokens": 32768,
+        "max_tokens": 32768,
+        "mode": "chat",
+        "output_cost_per_token": 0.0
+    },
+    "ollama/mixtral-8x22B-Instruct-v0.1": {
+        "input_cost_per_token": 0.0,
+        "litellm_provider": "ollama",
+        "max_input_tokens": 65536,
+        "max_output_tokens": 65536,
+        "max_tokens": 65536,
+        "mode": "chat",
+        "output_cost_per_token": 0.0
+    },
+    "ollama/mixtral-8x7B-Instruct-v0.1": {
+        "input_cost_per_token": 0.0,
+        "litellm_provider": "ollama",
+        "max_input_tokens": 32768,
+        "max_output_tokens": 32768,
+        "max_tokens": 32768,
+        "mode": "chat",
+        "output_cost_per_token": 0.0
+    },
     "ollama/orca-mini": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "ollama",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
     "ollama/vicuna": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "ollama",
+        "max_input_tokens": 2048,
+        "max_output_tokens": 2048,
         "max_tokens": 2048,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
     "openrouter/anthropic/claude-2": {
         "input_cost_per_token": 1.102e-05,
         "litellm_provider": "openrouter",
         "max_output_tokens": 8191,
         "max_tokens": 100000,
         "mode": "chat",
         "output_cost_per_token": 3.268e-05
     },
+    "openrouter/anthropic/claude-3-haiku": {
+        "input_cost_per_image": 0.0004,
+        "input_cost_per_token": 2.5e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 200000,
+        "mode": "chat",
+        "output_cost_per_token": 1.25e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "openrouter/anthropic/claude-3-opus": {
+        "input_cost_per_token": 1.5e-05,
+        "litellm_provider": "openrouter",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 7.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true,
+        "tool_use_system_prompt_tokens": 395
+    },
+    "openrouter/anthropic/claude-3-sonnet": {
+        "input_cost_per_image": 0.0048,
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "openrouter",
+        "max_tokens": 200000,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
     "openrouter/anthropic/claude-instant-v1": {
         "input_cost_per_token": 1.63e-06,
         "litellm_provider": "openrouter",
         "max_output_tokens": 8191,
         "max_tokens": 100000,
         "mode": "chat",
         "output_cost_per_token": 5.51e-06
     },
+    "openrouter/cognitivecomputations/dolphin-mixtral-8x7b": {
+        "input_cost_per_token": 5e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 32769,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07
+    },
+    "openrouter/cohere/command-r-plus": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "openrouter",
+        "max_tokens": 128000,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05
+    },
+    "openrouter/databricks/dbrx-instruct": {
+        "input_cost_per_token": 6e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 32768,
+        "mode": "chat",
+        "output_cost_per_token": 6e-07
+    },
+    "openrouter/fireworks/firellava-13b": {
+        "input_cost_per_token": 2e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2e-07
+    },
+    "openrouter/google/gemini-pro-1.5": {
+        "input_cost_per_image": 0.00265,
+        "input_cost_per_token": 2.5e-06,
+        "litellm_provider": "openrouter",
+        "max_input_tokens": 1000000,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 7.5e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "openrouter/google/gemini-pro-vision": {
+        "input_cost_per_image": 0.0025,
+        "input_cost_per_token": 1.25e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 45875,
+        "mode": "chat",
+        "output_cost_per_token": 3.75e-07,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
     "openrouter/google/palm-2-chat-bison": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "openrouter",
-        "max_tokens": 8000,
+        "max_tokens": 25804,
         "mode": "chat",
         "output_cost_per_token": 5e-07
     },
     "openrouter/google/palm-2-codechat-bison": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "openrouter",
-        "max_tokens": 8000,
+        "max_tokens": 20070,
         "mode": "chat",
         "output_cost_per_token": 5e-07
     },
     "openrouter/gryphe/mythomax-l2-13b": {
         "input_cost_per_token": 1.875e-06,
         "litellm_provider": "openrouter",
         "max_tokens": 8192,
@@ -1839,15 +2804,15 @@
         "max_tokens": 8000,
         "mode": "chat",
         "output_cost_per_token": 5.625e-06
     },
     "openrouter/meta-llama/codellama-34b-instruct": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "openrouter",
-        "max_tokens": 8096,
+        "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 5e-07
     },
     "openrouter/meta-llama/llama-2-13b-chat": {
         "input_cost_per_token": 2e-07,
         "litellm_provider": "openrouter",
         "max_tokens": 4096,
@@ -1857,28 +2822,77 @@
     "openrouter/meta-llama/llama-2-70b-chat": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "openrouter",
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.5e-06
     },
+    "openrouter/meta-llama/llama-3-70b-instruct": {
+        "input_cost_per_token": 5.9e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 7.9e-07
+    },
+    "openrouter/meta-llama/llama-3-70b-instruct:nitro": {
+        "input_cost_per_token": 9e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 9e-07
+    },
+    "openrouter/meta-llama/llama-3-8b-instruct:extended": {
+        "input_cost_per_token": 2.25e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 16384,
+        "mode": "chat",
+        "output_cost_per_token": 2.25e-06
+    },
+    "openrouter/meta-llama/llama-3-8b-instruct:free": {
+        "input_cost_per_token": 0.0,
+        "litellm_provider": "openrouter",
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 0.0
+    },
+    "openrouter/microsoft/wizardlm-2-8x22b:nitro": {
+        "input_cost_per_token": 1e-06,
+        "litellm_provider": "openrouter",
+        "max_tokens": 65536,
+        "mode": "chat",
+        "output_cost_per_token": 1e-06
+    },
     "openrouter/mistralai/mistral-7b-instruct": {
         "input_cost_per_token": 1.3e-07,
         "litellm_provider": "openrouter",
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 1.3e-07
     },
     "openrouter/mistralai/mistral-7b-instruct:free": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "openrouter",
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 0.0
     },
+    "openrouter/mistralai/mistral-large": {
+        "input_cost_per_token": 8e-06,
+        "litellm_provider": "openrouter",
+        "max_tokens": 32000,
+        "mode": "chat",
+        "output_cost_per_token": 2.4e-05
+    },
+    "openrouter/mistralai/mixtral-8x22b-instruct": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 65536,
+        "mode": "chat",
+        "output_cost_per_token": 6.5e-07
+    },
     "openrouter/nousresearch/nous-hermes-llama2-13b": {
         "input_cost_per_token": 2e-07,
         "litellm_provider": "openrouter",
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2e-07
     },
@@ -1899,14 +2913,48 @@
     "openrouter/openai/gpt-4": {
         "input_cost_per_token": 3e-05,
         "litellm_provider": "openrouter",
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 6e-05
     },
+    "openrouter/openai/gpt-4-vision-preview": {
+        "input_cost_per_image": 0.01445,
+        "input_cost_per_token": 1e-05,
+        "litellm_provider": "openrouter",
+        "max_tokens": 130000,
+        "mode": "chat",
+        "output_cost_per_token": 3e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "openrouter/openai/gpt-4o": {
+        "input_cost_per_token": 5e-06,
+        "litellm_provider": "openrouter",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
+    "openrouter/openai/gpt-4o-2024-05-13": {
+        "input_cost_per_token": 5e-06,
+        "litellm_provider": "openrouter",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
     "openrouter/pygmalionai/mythalion-13b": {
         "input_cost_per_token": 1.875e-06,
         "litellm_provider": "openrouter",
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.875e-06
     },
@@ -1916,193 +2964,368 @@
         "max_tokens": 6144,
         "mode": "chat",
         "output_cost_per_token": 1.875e-06
     },
     "palm/chat-bison": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "palm",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "palm/chat-bison-001": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "palm",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "palm/text-bison": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "palm",
-        "max_tokens": 8196,
+        "max_input_tokens": 8192,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "palm/text-bison-001": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "palm",
-        "max_tokens": 8196,
+        "max_input_tokens": 8192,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "palm/text-bison-safety-off": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "palm",
-        "max_tokens": 8196,
+        "max_input_tokens": 8192,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "palm/text-bison-safety-recitation-off": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "palm",
-        "max_tokens": 8196,
+        "max_input_tokens": 8192,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "perplexity/codellama-34b-instruct": {
         "input_cost_per_token": 3.5e-07,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 16384,
         "max_tokens": 16384,
         "mode": "chat",
         "output_cost_per_token": 1.4e-06
     },
     "perplexity/codellama-70b-instruct": {
         "input_cost_per_token": 7e-07,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 16384,
         "max_tokens": 16384,
         "mode": "chat",
         "output_cost_per_token": 2.8e-06
     },
     "perplexity/llama-2-70b-chat": {
         "input_cost_per_token": 7e-07,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.8e-06
     },
     "perplexity/mistral-7b-instruct": {
         "input_cost_per_token": 7e-08,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.8e-07
     },
     "perplexity/mixtral-8x7b-instruct": {
         "input_cost_per_token": 7e-08,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.8e-07
     },
     "perplexity/pplx-70b-chat": {
         "input_cost_per_token": 7e-07,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.8e-06
     },
     "perplexity/pplx-70b-online": {
         "input_cost_per_request": 0.005,
         "input_cost_per_token": 0.0,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.8e-06
     },
     "perplexity/pplx-7b-chat": {
         "input_cost_per_token": 7e-08,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 2.8e-07
     },
     "perplexity/pplx-7b-online": {
         "input_cost_per_request": 0.005,
         "input_cost_per_token": 0.0,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.8e-07
     },
     "perplexity/sonar-medium-chat": {
         "input_cost_per_token": 6e-07,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 16384,
         "max_tokens": 16384,
         "mode": "chat",
         "output_cost_per_token": 1.8e-06
     },
     "perplexity/sonar-medium-online": {
         "input_cost_per_request": 0.005,
         "input_cost_per_token": 0,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 12000,
+        "max_output_tokens": 12000,
         "max_tokens": 12000,
         "mode": "chat",
         "output_cost_per_token": 1.8e-06
     },
     "perplexity/sonar-small-chat": {
         "input_cost_per_token": 7e-08,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 16384,
+        "max_output_tokens": 16384,
         "max_tokens": 16384,
         "mode": "chat",
         "output_cost_per_token": 2.8e-07
     },
     "perplexity/sonar-small-online": {
         "input_cost_per_request": 0.005,
         "input_cost_per_token": 0,
         "litellm_provider": "perplexity",
+        "max_input_tokens": 12000,
+        "max_output_tokens": 12000,
         "max_tokens": 12000,
         "mode": "chat",
         "output_cost_per_token": 2.8e-07
     },
     "replicate/llama-2-70b-chat:2c1608e18606fad2812020dc541930f2d0495ce32eee50074220b87300bc16e1": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.0
     },
+    "replicate/meta/llama-2-13b": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07
+    },
+    "replicate/meta/llama-2-13b-chat": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07
+    },
+    "replicate/meta/llama-2-70b": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.75e-06
+    },
+    "replicate/meta/llama-2-70b-chat": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.75e-06
+    },
+    "replicate/meta/llama-2-7b": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/meta/llama-2-7b-chat": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/meta/llama-3-70b": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 2.75e-06
+    },
+    "replicate/meta/llama-3-70b-instruct": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 2.75e-06
+    },
+    "replicate/meta/llama-3-8b": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 8086,
+        "max_output_tokens": 8086,
+        "max_tokens": 8086,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/meta/llama-3-8b-instruct": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 8086,
+        "max_output_tokens": 8086,
+        "max_tokens": 8086,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/mistralai/mistral-7b-instruct-v0.2": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/mistralai/mistral-7b-v0.1": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/mistralai/mixtral-8x7b-instruct-v0.1": {
+        "input_cost_per_token": 3e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1e-06
+    },
     "sagemaker/meta-textgeneration-llama-2-13b": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "sagemaker",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
     "sagemaker/meta-textgeneration-llama-2-13b-f": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "sagemaker",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.0
     },
     "sagemaker/meta-textgeneration-llama-2-70b": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "sagemaker",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
     "sagemaker/meta-textgeneration-llama-2-70b-b-f": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "sagemaker",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.0
     },
     "sagemaker/meta-textgeneration-llama-2-7b": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "sagemaker",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
         "output_cost_per_token": 0.0
     },
     "sagemaker/meta-textgeneration-llama-2-7b-f": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "sagemaker",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.0
     },
     "standard/1024-x-1024/dall-e-3": {
         "input_cost_per_pixel": 3.81469e-08,
         "litellm_provider": "openai",
@@ -2120,53 +3343,77 @@
         "litellm_provider": "openai",
         "mode": "image_generation",
         "output_cost_per_pixel": 0.0
     },
     "text-bison": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-text-models",
-        "max_tokens": 8192,
+        "max_input_tokens": 8192,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "text-bison@001": {
         "input_cost_per_token": 1.25e-07,
         "litellm_provider": "vertex_ai-text-models",
-        "max_tokens": 8192,
+        "max_input_tokens": 8192,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "completion",
-        "output_cost_per_token": 1.25e-07
+        "output_cost_per_token": 1.25e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "text-embedding-3-large": {
         "input_cost_per_token": 1.3e-07,
         "litellm_provider": "openai",
+        "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
-        "output_cost_per_token": 0.0
+        "output_cost_per_token": 0.0,
+        "output_vector_size": 3072
     },
     "text-embedding-3-small": {
         "input_cost_per_token": 2e-08,
         "litellm_provider": "openai",
+        "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
-        "output_cost_per_token": 0.0
+        "output_cost_per_token": 0.0,
+        "output_vector_size": 1536
     },
     "text-embedding-ada-002": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "openai",
+        "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
-        "output_cost_per_token": 0.0
+        "output_cost_per_token": 0.0,
+        "output_vector_size": 1536
     },
     "text-embedding-ada-002-v2": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "openai",
+        "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
+    "text-embedding-preview-0409": {
+        "input_cost_per_token": 6.25e-09,
+        "input_cost_per_token_batch_requests": 5e-09,
+        "litellm_provider": "vertex_ai-embedding-models",
+        "max_input_tokens": 3072,
+        "max_tokens": 3072,
+        "mode": "embedding",
+        "output_cost_per_token": 0,
+        "output_vector_size": 768,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/pricing"
+    },
     "text-moderation-007": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "openai",
         "max_input_tokens": 32768,
         "max_output_tokens": 0,
         "max_tokens": 32768,
         "mode": "moderations",
@@ -2186,72 +3433,93 @@
         "litellm_provider": "openai",
         "max_input_tokens": 32768,
         "max_output_tokens": 0,
         "max_tokens": 32768,
         "mode": "moderations",
         "output_cost_per_token": 0.0
     },
+    "text-multilingual-embedding-preview-0409": {
+        "input_cost_per_token": 6.25e-09,
+        "litellm_provider": "vertex_ai-embedding-models",
+        "max_input_tokens": 3072,
+        "max_tokens": 3072,
+        "mode": "embedding",
+        "output_cost_per_token": 0,
+        "output_vector_size": 768,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
+    },
     "text-unicorn": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "vertex_ai-text-models",
-        "max_tokens": 8192,
+        "max_input_tokens": 8192,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "completion",
-        "output_cost_per_token": 2.8e-05
+        "output_cost_per_token": 2.8e-05,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "text-unicorn@001": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "vertex_ai-text-models",
-        "max_tokens": 8192,
+        "max_input_tokens": 8192,
+        "max_output_tokens": 1024,
+        "max_tokens": 1024,
         "mode": "completion",
-        "output_cost_per_token": 2.8e-05
+        "output_cost_per_token": 2.8e-05,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "textembedding-gecko": {
         "input_cost_per_token": 6.25e-09,
         "litellm_provider": "vertex_ai-embedding-models",
         "max_input_tokens": 3072,
         "max_tokens": 3072,
         "mode": "embedding",
         "output_cost_per_token": 0,
-        "output_vector_size": 768
+        "output_vector_size": 768,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "textembedding-gecko-multilingual": {
         "input_cost_per_token": 6.25e-09,
         "litellm_provider": "vertex_ai-embedding-models",
         "max_input_tokens": 3072,
         "max_tokens": 3072,
         "mode": "embedding",
         "output_cost_per_token": 0,
-        "output_vector_size": 768
+        "output_vector_size": 768,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "textembedding-gecko-multilingual@001": {
         "input_cost_per_token": 6.25e-09,
         "litellm_provider": "vertex_ai-embedding-models",
         "max_input_tokens": 3072,
         "max_tokens": 3072,
         "mode": "embedding",
         "output_cost_per_token": 0,
-        "output_vector_size": 768
+        "output_vector_size": 768,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "textembedding-gecko@001": {
         "input_cost_per_token": 6.25e-09,
         "litellm_provider": "vertex_ai-embedding-models",
         "max_input_tokens": 3072,
         "max_tokens": 3072,
         "mode": "embedding",
         "output_cost_per_token": 0,
-        "output_vector_size": 768
+        "output_vector_size": 768,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "textembedding-gecko@003": {
         "input_cost_per_token": 6.25e-09,
         "litellm_provider": "vertex_ai-embedding-models",
         "max_input_tokens": 3072,
         "max_tokens": 3072,
         "mode": "embedding",
         "output_cost_per_token": 0,
-        "output_vector_size": 768
+        "output_vector_size": 768,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
     },
     "together-ai-20.1b-40b": {
         "input_cost_per_token": 8e-07,
         "litellm_provider": "together_ai",
         "output_cost_per_token": 8e-07
     },
     "together-ai-3.1b-7b": {
@@ -2288,28 +3556,109 @@
         "supports_parallel_function_calling": true
     },
     "together_ai/togethercomputer/CodeLlama-34b-Instruct": {
         "litellm_provider": "together_ai",
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
+    "vertex_ai/claude-3-haiku@20240307": {
+        "input_cost_per_token": 2.5e-07,
+        "litellm_provider": "vertex_ai-anthropic_models",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.25e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "vertex_ai/claude-3-opus@20240229": {
+        "input_cost_per_token": 1.5e-06,
+        "litellm_provider": "vertex_ai-anthropic_models",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 7.5e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "vertex_ai/claude-3-sonnet@20240229": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "vertex_ai-anthropic_models",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "vertex_ai/imagegeneration@006": {
+        "cost_per_image": 0.02,
+        "litellm_provider": "vertex_ai-image-models",
+        "mode": "image_generation",
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/pricing"
+    },
     "voyage/voyage-01": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "voyage",
+        "max_input_tokens": 4096,
         "max_tokens": 4096,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
+    "voyage/voyage-2": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 4000,
+        "max_tokens": 4000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
+    "voyage/voyage-code-2": {
+        "input_cost_per_token": 1.2e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 16000,
+        "max_tokens": 16000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
+    "voyage/voyage-large-2": {
+        "input_cost_per_token": 1.2e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 16000,
+        "max_tokens": 16000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
+    "voyage/voyage-law-2": {
+        "input_cost_per_token": 1.2e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 16000,
+        "max_tokens": 16000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
     "voyage/voyage-lite-01": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "voyage",
+        "max_input_tokens": 4096,
         "max_tokens": 4096,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
+    "voyage/voyage-lite-02-instruct": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 4000,
+        "max_tokens": 4000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
     "whisper-1": {
         "input_cost_per_second": 0,
         "litellm_provider": "openai",
         "mode": "audio_transcription",
         "output_cost_per_second": 0.0001
     }
 }
```

### Comparing `llmvm_cli-0.3.0/llmvm/server/ast_parser.py` & `llmvm_cli-0.3.1/llmvm/server/ast_parser.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/base_library/browser.py` & `llmvm_cli-0.3.1/llmvm/server/base_library/browser.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/base_library/content_downloader.py` & `llmvm_cli-0.3.1/llmvm/server/base_library/content_downloader.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/base_library/function_bindable.py` & `llmvm_cli-0.3.1/llmvm/server/base_library/function_bindable.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/base_library/searcher.py` & `llmvm_cli-0.3.1/llmvm/server/base_library/searcher.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/base_library/source.py` & `llmvm_cli-0.3.1/llmvm/server/base_library/source.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/base_library/source_project.py` & `llmvm_cli-0.3.1/llmvm/server/base_library/source_project.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/bcl.py` & `llmvm_cli-0.3.1/llmvm/server/bcl.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/persistent_cache.py` & `llmvm_cli-0.3.1/llmvm/server/persistent_cache.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/answer.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_error_correction.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/answer_error_correction.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_nocontext.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/answer_nocontext.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/answer_regen_code_or_rewrite.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/answer_regen_code_or_rewrite.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/browser_execute_plan.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/browser_execute_plan.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/browser_generate_plan.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/browser_generate_plan.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/code_get_source_summary.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/code_get_source_summary.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/coerce.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/coerce.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/document_chunk.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/document_chunk.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_error_correction.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_error_correction.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_global.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_global.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_list.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_list.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_local.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_local.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_bind_old.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_bind_old.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_call.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_call.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/llm_loop_bind.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/llm_loop_bind.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/map_reduce_map.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/map_reduce_map.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/map_reduce_reduce.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/map_reduce_reduce.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/pandas_bind.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/pandas_bind.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/pdf_content.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/pdf_content.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/query_understanding.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/query_understanding.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_classifier.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/search_classifier.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_location.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/search_location.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/search_ranker.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/search_ranker.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_code_insights.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_code_insights.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_code_prompt_old.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_code_prompt_old.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_continuation_execution.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_continuation_execution.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_error_correction.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_error_correction.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/prompts/starlark/starlark_tool_execution.prompt` & `llmvm_cli-0.3.1/llmvm/server/prompts/starlark/starlark_tool_execution.prompt`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/server.py` & `llmvm_cli-0.3.1/llmvm/server/server.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/starlark_execution_controller.py` & `llmvm_cli-0.3.1/llmvm/server/starlark_execution_controller.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/starlark_runtime.py` & `llmvm_cli-0.3.1/llmvm/server/starlark_runtime.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/tools/edgar.py` & `llmvm_cli-0.3.1/llmvm/server/tools/edgar.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/tools/firefox.py` & `llmvm_cli-0.3.1/llmvm/server/tools/firefox.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/tools/market.py` & `llmvm_cli-0.3.1/llmvm/server/tools/market.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/tools/scraper.py` & `llmvm_cli-0.3.1/llmvm/server/tools/scraper.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/tools/search.py` & `llmvm_cli-0.3.1/llmvm/server/tools/search.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/tools/search_hn.py` & `llmvm_cli-0.3.1/llmvm/server/tools/search_hn.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/tools/webhelpers.py` & `llmvm_cli-0.3.1/llmvm/server/tools/webhelpers.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/vector_search.py` & `llmvm_cli-0.3.1/llmvm/server/vector_search.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/llmvm/server/vector_store.py` & `llmvm_cli-0.3.1/llmvm/server/vector_store.py`

 * *Files identical despite different names*

### Comparing `llmvm_cli-0.3.0/pyproject.toml` & `llmvm_cli-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llmvm-cli"
-version = "0.3.0"
+version = "0.3.1"
 description = "Command Line LLM with client-side tools support."
 authors = ["9600 devs <contact@9600.dev>"]
 readme = "README.md"
 packages = [ {include = "llmvm"} ]
 include = ["llmvm/client/awesome_prompts.csv", "llmvm/model_prices_and_context_window.json", "llmvm/server/prompts/**/*", "llmvm/config.yaml"]
 homepage = "https://github.com/9600dev/llmvm"
 repository = "https://github.com/9600dev/llmvm"
```

### Comparing `llmvm_cli-0.3.0/PKG-INFO` & `llmvm_cli-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmvm-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: Command Line LLM with client-side tools support.
 Home-page: https://github.com/9600dev/llmvm
 Author: 9600 devs
 Author-email: contact@9600.dev
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -55,15 +55,15 @@
 Project-URL: Repository, https://github.com/9600dev/llmvm
 Description-Content-Type: text/markdown
 
 # LLMVM
 
 LLMVM is a CLI based productivity tool that uses Large Language Models and local Python tools/helpers to reason about and execute your tasks. A CLI client (client.py) either connects directly to an LLM provider or will connect to a local server (server.py) that coordinates tool execution, [Retrieval Agumented Generation](https://blogs.nvidia.com/blog/what-is-retrieval-augmented-generation/), document search and more.
 
-It supports [Anthropic's](https://www.anthropic.com) Claude 3 (Opus, Sonnet and Haiku) vision models, [OpenAI](https://openai.com/blog/openai-api) GPT 3.5/4/4 Turbo and Vision models from OpenAI. [Gemini](https://deepmind.google/technologies/gemini/) and [Mistral](https://deepmind.google/technologies/gemini/) are currently experimental. It's best used with the [kitty](https://github.com/kovidgoyal/kitty) terminal as LLMVM will screenshot and render images as work on vision based tasks progresses.
+It supports [Anthropic's](https://www.anthropic.com) Claude 3 (Opus, Sonnet and Haiku) vision models, [OpenAI](https://openai.com/blog/openai-api) GPT 3.5/4/4 Turbo/4o models from OpenAI. [Gemini](https://deepmind.google/technologies/gemini/) and [Mistral](https://deepmind.google/technologies/gemini/) are currently experimental. It's best used with the [kitty](https://github.com/kovidgoyal/kitty) terminal as LLMVM will screenshot and render images as work on vision based tasks progresses.
 
 LLMVM's features are best explored through examples. Let's install, then go through some:
 
 ```$ pip install llmvm-cli```
 ```$ playwright install firefox```
 
 ```$ python -m llmvm.server```
@@ -154,15 +154,15 @@
 
 and then:
 
 ```bash
 cat somecode.py | llm -o direct "rewrite this code; make it cleaner and easier to read"
 ```
 
-Image understanding is supported on Anthropic Claude 3 models and OpenAI's GPT 4 turbo vision preview model.
+Image understanding is supported on Anthropic Claude 3 models and OpenAI's GPT 4o vision model.
 
 ```bash
 cat docs/beach.jpg | llm "generate a dalle prompt for the exact inverse of this image"
 ```
 
 ![](docs/2023-11-11-12-59-39.png)
 
@@ -271,15 +271,15 @@
 executor: 'anthropic'  # or 'openai'
 ```
 
 or, you can set environment variables that specify the execution backend and the model you'd like to use:
 
 ```bash
 export LLMVM_EXECUTOR='openai'
-export LLMVM_MODEL='gpt-4-vision-preview'
+export LLMVM_MODEL='gpt-4o'
 python -m llmvm.client "hello, who are you?"
 ```
 
 #### Performance Profiling
 
 * open `~/.config/llmvm/config.yaml` and change profiling to 'true' or 'false'.
```

