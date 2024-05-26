# Comparing `tmp/byzerllm-0.1.90.tar.gz` & `tmp/byzerllm-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byzerllm-0.1.90.tar", last modified: Fri May 24 09:09:44 2024, max compression
+gzip compressed data, was "byzerllm-0.1.91.tar", last modified: Sun May 26 09:56:07 2024, max compression
```

## Comparing `byzerllm-0.1.90.tar` & `byzerllm-0.1.91.tar`

### file list

```diff
@@ -1,583 +1,583 @@
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.897934 byzerllm-0.1.90/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11558 2024-03-31 13:19:57.000000 byzerllm-0.1.90/LICENSE
--rw-r--r--   0 allwefantasy   (501) staff       (20)    83884 2024-05-24 09:09:44.897461 byzerllm-0.1.90/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)    83553 2024-05-14 06:52:28.000000 byzerllm-0.1.90/README.md
--rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2024-05-24 09:09:44.898015 byzerllm-0.1.90/setup.cfg
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1377 2024-04-23 10:08:12.000000 byzerllm-0.1.90/setup.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.404599 byzerllm-0.1.90/src/
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.443620 byzerllm-0.1.90/src/byzerllm/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16451 2024-05-24 08:57:11.000000 byzerllm-0.1.90/src/byzerllm/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.446900 byzerllm-0.1.90/src/byzerllm/alpha_moss/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29048 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/alpha_moss/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.451832 byzerllm-0.1.90/src/byzerllm/apps/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      466 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.456814 byzerllm-0.1.90/src/byzerllm/apps/agent/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5003 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2629 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28758 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/conversable_agent.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.469657 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6643 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/assistant_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3586 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/byzer_engine_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1725 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/common_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10177 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/data_analysis.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19116 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/data_analysis_pipeline_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4293 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/llama_index_retrieval_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5254 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/load_data_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2877 2023-12-19 05:48:54.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/output_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1598 2023-12-19 05:48:54.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/planner.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7840 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/preview_file_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8416 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/python_codesandbox_agent.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.473783 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      284 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3578 2024-01-19 04:16:39.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/condition.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2860 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/context.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3850 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/rhetorical.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2864 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/time.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7281 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/retrieval_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6494 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/rhetorical_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11826 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/simple_retrieval_client.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    14880 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/spark_sql_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4980 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/sql_reviewer_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4190 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/subquestion_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6760 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/visualization_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10100 2023-12-19 05:48:54.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/groupchat.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1071 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/registry.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.475814 byzerllm-0.1.90/src/byzerllm/apps/agent/store/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      439 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/store/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1307 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/store/memory_store.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1016 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/store/stores.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5584 2023-12-19 05:48:54.000000 byzerllm-0.1.90/src/byzerllm/apps/agent/user_proxy_agent.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3942 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/builder.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.476336 byzerllm-0.1.90/src/byzerllm/apps/byzer_sql/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6184 2024-05-14 06:51:51.000000 byzerllm-0.1.90/src/byzerllm/apps/byzer_sql/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.478990 byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-05-10 08:09:49.000000 byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8507 2024-05-10 09:06:58.000000 byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/command.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5747 2024-05-11 01:14:09.000000 byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/env.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3350 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/client.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.485509 byzerllm-0.1.90/src/byzerllm/apps/llama_index/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1506 2024-04-16 10:36:39.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4081 2024-05-14 09:17:42.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1218 2024-04-16 10:34:46.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_docstore.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1467 2024-04-22 02:58:54.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_embedding.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1199 2024-04-24 04:47:48.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_index_store.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4237 2024-04-24 05:29:47.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_kvstore.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6734 2024-04-25 06:57:07.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_vectordb.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2693 2024-05-01 12:00:48.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/collection_manager.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    14057 2024-04-24 05:31:49.000000 byzerllm-0.1.90/src/byzerllm/apps/llama_index/simple_retrieval.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6276 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/qa.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4934 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/qa_strategy.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1687 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/apps/vector_db.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.487823 byzerllm-0.1.90/src/byzerllm/auto/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20799 2024-05-06 06:30:19.000000 byzerllm-0.1.90/src/byzerllm/auto/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7577 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/auto/backend_ds.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10678 2024-04-26 07:58:28.000000 byzerllm-0.1.90/src/byzerllm/auto/backend_llama_cpp.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.488961 byzerllm-0.1.90/src/byzerllm/baichuan/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4370 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/baichuan/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.492664 byzerllm-0.1.90/src/byzerllm/bark/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4243 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/api.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.407679 byzerllm-0.1.90/src/byzerllm/bark/assets/
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.666622 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16794 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/announcer.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20316 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31724 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    59348 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25116 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33860 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    38124 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    15516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    13436 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18980 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25436 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24420 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34820 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30604 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29324 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    51084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    44044 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    43564 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    53908 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31244 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23036 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26820 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28684 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33004 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    46604 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    45268 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    52684 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    41268 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29964 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    44148 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24796 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    37964 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22716 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    50548 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29540 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29004 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21916 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    39780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    43084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42284 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42548 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    45324 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    37380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32420 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    58492 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    49004 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34444 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30284 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    58652 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1943 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/readme.md
--rw-r--r--   0 allwefantasy   (501) staff       (20)    57852 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    51668 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29164 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    45748 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42924 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    38500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21276 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    35724 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.794759 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    39620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23196 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    40100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28524 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    51084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26236 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34980 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25540 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22716 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25116 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26236 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25700 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25436 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    45804 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25700 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    52204 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    50764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    49908 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    45108 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    55932 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32524 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    43244 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25860 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29804 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    51404 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    39404 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33804 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    40788 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30444 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29644 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    43724 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    42708 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    37644 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24420 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31244 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26716 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    40788 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31140 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26556 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26340 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19196 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    39564 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23140 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23196 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27884 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31140 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23676 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    41428 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    38180 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    38820 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30980 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    27724 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34500 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    36844 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26980 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30764 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28100 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28524 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    39780 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    39884 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19940 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28204 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    44628 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    26020 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    39084 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    34660 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22076 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28684 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33164 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    17220 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25276 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28204 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20636 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19836 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    29964 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    17436 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16900 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21060 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19300 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16156 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3759 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/bark_voice.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    33373 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/generation.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     9139 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/model.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5955 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bark/model_fine.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.795727 byzerllm-0.1.90/src/byzerllm/bge/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1022 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/bge/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.796179 byzerllm-0.1.90/src/byzerllm/bge_rerank/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      929 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/bge_rerank/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5748 2024-05-11 00:58:40.000000 byzerllm-0.1.90/src/byzerllm/byzerllm_command.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.797088 byzerllm-0.1.90/src/byzerllm/chatglm2/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2439 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/chatglm2/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.799317 byzerllm-0.1.90/src/byzerllm/chatglm6b/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/arguments.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/finetune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/trainer_seq2seq.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.800872 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3000 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/finetune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1404 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/infer.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.803253 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      277 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16907 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/common.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7620 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/config.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6263 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/other.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11082 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7984 2024-05-11 00:58:29.000000 byzerllm-0.1.90/src/byzerllm/command_args.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.806188 byzerllm-0.1.90/src/byzerllm/dolly/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/consts.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1112 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/dolly_inference.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10065 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/generate.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    12156 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/dolly/trainer.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.806769 byzerllm-0.1.90/src/byzerllm/falcon/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4414 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/falcon/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2362 2024-05-11 00:55:17.000000 byzerllm-0.1.90/src/byzerllm/lang.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.807395 byzerllm-0.1.90/src/byzerllm/llama/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6504 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/llama/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.807944 byzerllm-0.1.90/src/byzerllm/llama2/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6675 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/llama2/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2010 2024-04-01 10:03:54.000000 byzerllm-0.1.90/src/byzerllm/log.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.808623 byzerllm-0.1.90/src/byzerllm/m3e/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      189 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/m3e/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.810358 byzerllm-0.1.90/src/byzerllm/moss/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    12657 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/finetune_moss.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.814472 byzerllm-0.1.90/src/byzerllm/moss/models/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5097 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/configuration_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6735 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/custom_autotune.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31351 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/modeling_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    18866 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/quantization.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    15952 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/models/tokenization_moss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16919 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/moss/moss_inference.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.815208 byzerllm-0.1.90/src/byzerllm/processor/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      577 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/processor/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.815923 byzerllm-0.1.90/src/byzerllm/qwen/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6510 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/qwen/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.816540 byzerllm-0.1.90/src/byzerllm/qwen_vl_chat/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3792 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/qwen_vl_chat/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.817203 byzerllm-0.1.90/src/byzerllm/records/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6824 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/records/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.817953 byzerllm-0.1.90/src/byzerllm/saas/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/saas/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.818205 byzerllm-0.1.90/src/byzerllm/saas/aws_bedrock/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11871 2024-05-11 12:03:07.000000 byzerllm-0.1.90/src/byzerllm/saas/aws_bedrock/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.818872 byzerllm-0.1.90/src/byzerllm/saas/azure/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     9857 2024-05-11 11:58:25.000000 byzerllm-0.1.90/src/byzerllm/saas/azure/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.819524 byzerllm-0.1.90/src/byzerllm/saas/azure_openai/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3454 2024-05-11 11:57:58.000000 byzerllm-0.1.90/src/byzerllm/saas/azure_openai/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.820142 byzerllm-0.1.90/src/byzerllm/saas/baichuan/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5331 2024-05-11 11:56:58.000000 byzerllm-0.1.90/src/byzerllm/saas/baichuan/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.820759 byzerllm-0.1.90/src/byzerllm/saas/chatglm/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2306 2023-12-26 06:22:53.000000 byzerllm-0.1.90/src/byzerllm/saas/chatglm/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.821783 byzerllm-0.1.90/src/byzerllm/saas/claude/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5753 2024-05-11 11:54:49.000000 byzerllm-0.1.90/src/byzerllm/saas/claude/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.822338 byzerllm-0.1.90/src/byzerllm/saas/gemini/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4517 2024-05-11 11:54:20.000000 byzerllm-0.1.90/src/byzerllm/saas/gemini/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.823106 byzerllm-0.1.90/src/byzerllm/saas/minimax/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    11064 2024-05-11 11:53:21.000000 byzerllm-0.1.90/src/byzerllm/saas/minimax/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.823726 byzerllm-0.1.90/src/byzerllm/saas/official_openai/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    16675 2024-05-17 14:21:16.000000 byzerllm-0.1.90/src/byzerllm/saas/official_openai/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.824923 byzerllm-0.1.90/src/byzerllm/saas/openai/
--rw-r--r--   0 allwefantasy   (501) staff       (20)       83 2024-04-14 14:38:04.000000 byzerllm-0.1.90/src/byzerllm/saas/openai/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.825684 byzerllm-0.1.90/src/byzerllm/saas/qianfan/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6147 2024-05-11 11:49:15.000000 byzerllm-0.1.90/src/byzerllm/saas/qianfan/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.826623 byzerllm-0.1.90/src/byzerllm/saas/qianwen/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6830 2024-05-11 11:42:52.000000 byzerllm-0.1.90/src/byzerllm/saas/qianwen/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.827518 byzerllm-0.1.90/src/byzerllm/saas/qianwen_vl/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7083 2024-05-17 14:16:35.000000 byzerllm-0.1.90/src/byzerllm/saas/qianwen_vl/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.828585 byzerllm-0.1.90/src/byzerllm/saas/sparkdesk/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6707 2024-05-11 11:47:59.000000 byzerllm-0.1.90/src/byzerllm/saas/sparkdesk/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.829234 byzerllm-0.1.90/src/byzerllm/saas/volcengine/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     9214 2024-05-11 11:50:42.000000 byzerllm-0.1.90/src/byzerllm/saas/volcengine/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.829910 byzerllm-0.1.90/src/byzerllm/saas/zhipu/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5039 2024-05-11 11:51:47.000000 byzerllm-0.1.90/src/byzerllm/saas/zhipu/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.834705 byzerllm-0.1.90/src/byzerllm/stable_diffusion/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6453 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.835785 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.836529 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.837393 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/pipelines/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/pipelines/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4720 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.839186 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1701 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1006 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/generation.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.840197 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/models/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/models/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1260 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/models/diffusion.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      173 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/plugin.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1136 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/config.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.841966 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3127 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/embeddings.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.843665 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3567 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8214 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.846622 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    31226 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10680 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.848580 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8276 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5247 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3104 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/utils.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      673 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/images.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.849264 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.849848 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/diffusers/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/diffusers/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1246 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      434 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/logger.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4681 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/model.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      540 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/shared.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      928 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/stable_diffusion/utils.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.850504 byzerllm-0.1.90/src/byzerllm/starcode/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1882 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/starcode/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2422 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/store.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.859448 byzerllm-0.1.90/src/byzerllm/utils/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    25659 2024-04-26 09:09:23.000000 byzerllm-0.1.90/src/byzerllm/utils/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.865830 byzerllm-0.1.90/src/byzerllm/utils/client/
--rw-r--r--   0 allwefantasy   (501) staff       (20)      884 2024-04-18 06:47:05.000000 byzerllm-0.1.90/src/byzerllm/utils/client/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    65237 2024-05-24 08:19:48.000000 byzerllm-0.1.90/src/byzerllm/utils/client/byzerllm_client.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    19055 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/utils/client/code_utils.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.866783 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.872020 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8922 2024-04-18 09:44:41.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/api_server.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    14198 2024-04-01 10:03:54.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/protocol.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6707 2024-04-23 09:24:35.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serve.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8887 2024-04-26 08:07:36.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serving_chat.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     7581 2024-04-26 08:08:28.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serving_completion.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5854 2024-04-23 05:50:42.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serving_engine.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8573 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/tool.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5777 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/utils/client/img_utils.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10008 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/utils/client/math_utils.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4275 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/utils/client/message_utils.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1017 2024-01-18 03:33:00.000000 byzerllm-0.1.90/src/byzerllm/utils/client/parallel_utils.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    12377 2024-04-26 01:43:44.000000 byzerllm-0.1.90/src/byzerllm/utils/client/types.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.872773 byzerllm-0.1.90/src/byzerllm/utils/config/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1059 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/config/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2194 2024-05-10 09:22:55.000000 byzerllm-0.1.90/src/byzerllm/utils/connect_ray.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4042 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/emb.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.875888 byzerllm-0.1.90/src/byzerllm/utils/fulltune/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2637 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.877784 byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2929 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    30037 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    12755 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/deepspeed_trainner.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     4826 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/launch.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.880158 byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    28458 2023-12-23 13:24:00.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2406 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6924 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/fulltune/trainner.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    14303 2024-04-08 04:52:43.000000 byzerllm-0.1.90/src/byzerllm/utils/json_repaire.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5187 2024-05-11 00:40:06.000000 byzerllm-0.1.90/src/byzerllm/utils/langutil.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.881024 byzerllm-0.1.90/src/byzerllm/utils/metrics/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1216 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/metrics/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)      367 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/object_store_ref_util.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2346 2023-12-26 06:22:53.000000 byzerllm-0.1.90/src/byzerllm/utils/openai_utils.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1446 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/ray_utils.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.883202 byzerllm-0.1.90/src/byzerllm/utils/retrieval/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    13613 2024-04-16 13:20:54.000000 byzerllm-0.1.90/src/byzerllm/utils/retrieval/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     6019 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/utils/retrieval/rest.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1970 2023-12-12 03:30:31.000000 byzerllm-0.1.90/src/byzerllm/utils/retrieval/udf.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.888327 byzerllm-0.1.90/src/byzerllm/utils/sft/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10331 2023-12-23 13:24:00.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1203 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/argument.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/collator.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3248 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/dataset.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1614 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/loss.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2295 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/merge_lora.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2611 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/model.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     8381 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/qlora.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3395 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/sft/trainer.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1288 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/utils/testing.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)    10903 2024-05-11 01:56:39.000000 byzerllm-0.1.90/src/byzerllm/utils/text_generator.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1633 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/utils/tokenizer.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5394 2024-04-27 05:50:08.000000 byzerllm-0.1.90/src/byzerllm/utils/types.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)       23 2024-05-24 08:58:48.000000 byzerllm-0.1.90/src/byzerllm/version.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.888794 byzerllm-0.1.90/src/byzerllm/visualglm/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2462 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/visualglm/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.889617 byzerllm-0.1.90/src/byzerllm/whisper/
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/whisper/__init__.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1254 2023-10-10 02:45:08.000000 byzerllm-0.1.90/src/byzerllm/whisper/whisper_inference.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.890269 byzerllm-0.1.90/src/byzerllm/zephyr/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     5628 2024-03-31 13:19:57.000000 byzerllm-0.1.90/src/byzerllm/zephyr/__init__.py
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.896762 byzerllm-0.1.90/src/byzerllm.egg-info/
--rw-r--r--   0 allwefantasy   (501) staff       (20)    83884 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/PKG-INFO
--rw-r--r--   0 allwefantasy   (501) staff       (20)    23396 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/SOURCES.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/dependency_links.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)       60 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/entry_points.txt
--rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2024-05-24 09:09:44.000000 byzerllm-0.1.90/src/byzerllm.egg-info/top_level.txt
-drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-24 09:09:44.896155 byzerllm-0.1.90/tests/
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1603 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_data_analysis.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3235 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_deepseek_code.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1248 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_deploy.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     2041 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_emb_rerank.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1187 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_model_meta.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1413 2024-04-15 08:05:56.000000 byzerllm-0.1.90/tests/test_prompt.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     3522 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_template.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_transformers_deploy.py
--rw-r--r--   0 allwefantasy   (501) staff       (20)     1664 2024-04-18 05:04:09.000000 byzerllm-0.1.90/tests/test_yi.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.027313 byzerllm-0.1.91/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11558 2024-03-31 13:19:57.000000 byzerllm-0.1.91/LICENSE
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    83884 2024-05-26 09:56:07.026716 byzerllm-0.1.91/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    83553 2024-05-14 06:52:28.000000 byzerllm-0.1.91/README.md
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       38 2024-05-26 09:56:07.027406 byzerllm-0.1.91/setup.cfg
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1377 2024-04-23 10:08:12.000000 byzerllm-0.1.91/setup.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.556516 byzerllm-0.1.91/src/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.577206 byzerllm-0.1.91/src/byzerllm/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16655 2024-05-26 09:54:42.000000 byzerllm-0.1.91/src/byzerllm/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.579504 byzerllm-0.1.91/src/byzerllm/alpha_moss/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29048 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/alpha_moss/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.582315 byzerllm-0.1.91/src/byzerllm/apps/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      466 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/apps/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.586212 byzerllm-0.1.91/src/byzerllm/apps/agent/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5003 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2629 2023-12-12 03:30:31.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28758 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/conversable_agent.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.596289 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-12-12 03:30:31.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6643 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/assistant_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3586 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/byzer_engine_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1725 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/common_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10177 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/data_analysis.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19116 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/data_analysis_pipeline_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4293 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/llama_index_retrieval_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5254 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/load_data_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2877 2023-12-19 05:48:54.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/output_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1598 2023-12-19 05:48:54.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/planner.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7840 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/preview_file_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8416 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/python_codesandbox_agent.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.599745 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      284 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3578 2024-01-19 04:16:39.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/condition.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2860 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/context.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3850 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/rhetorical.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2864 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/time.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7281 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/retrieval_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6494 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/rhetorical_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11826 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/simple_retrieval_client.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    14880 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/spark_sql_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4980 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/sql_reviewer_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4190 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/subquestion_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6760 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/visualization_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10100 2023-12-19 05:48:54.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/groupchat.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1071 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/registry.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.601301 byzerllm-0.1.91/src/byzerllm/apps/agent/store/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      439 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/store/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1307 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/store/memory_store.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1016 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/store/stores.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5584 2023-12-19 05:48:54.000000 byzerllm-0.1.91/src/byzerllm/apps/agent/user_proxy_agent.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3942 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/apps/builder.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.601709 byzerllm-0.1.91/src/byzerllm/apps/byzer_sql/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6184 2024-05-14 06:51:51.000000 byzerllm-0.1.91/src/byzerllm/apps/byzer_sql/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.603324 byzerllm-0.1.91/src/byzerllm/apps/byzer_storage/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-05-10 08:09:49.000000 byzerllm-0.1.91/src/byzerllm/apps/byzer_storage/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8507 2024-05-10 09:06:58.000000 byzerllm-0.1.91/src/byzerllm/apps/byzer_storage/command.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5747 2024-05-11 01:14:09.000000 byzerllm-0.1.91/src/byzerllm/apps/byzer_storage/env.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3350 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/apps/client.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.609392 byzerllm-0.1.91/src/byzerllm/apps/llama_index/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1506 2024-04-16 10:36:39.000000 byzerllm-0.1.91/src/byzerllm/apps/llama_index/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4081 2024-05-14 09:17:42.000000 byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1218 2024-04-16 10:34:46.000000 byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_docstore.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1467 2024-04-22 02:58:54.000000 byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_embedding.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1199 2024-04-24 04:47:48.000000 byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_index_store.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4237 2024-04-24 05:29:47.000000 byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_kvstore.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6734 2024-04-25 06:57:07.000000 byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_vectordb.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2693 2024-05-01 12:00:48.000000 byzerllm-0.1.91/src/byzerllm/apps/llama_index/collection_manager.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    14057 2024-04-24 05:31:49.000000 byzerllm-0.1.91/src/byzerllm/apps/llama_index/simple_retrieval.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6276 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/apps/qa.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4934 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/apps/qa_strategy.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1687 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/apps/vector_db.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.611552 byzerllm-0.1.91/src/byzerllm/auto/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20799 2024-05-06 06:30:19.000000 byzerllm-0.1.91/src/byzerllm/auto/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7577 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/auto/backend_ds.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10678 2024-04-26 07:58:28.000000 byzerllm-0.1.91/src/byzerllm/auto/backend_llama_cpp.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.612297 byzerllm-0.1.91/src/byzerllm/baichuan/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4370 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/baichuan/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.616450 byzerllm-0.1.91/src/byzerllm/bark/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4243 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/api.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.559276 byzerllm-0.1.91/src/byzerllm/bark/assets/
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.743215 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16794 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/announcer.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29060 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20316 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31724 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    59348 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25116 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33860 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38124 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21220 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    15516 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    13436 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35084 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18980 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25436 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27620 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24420 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34820 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18660 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22660 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30604 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29324 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51084 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31460 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    44044 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43564 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    53908 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33060 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31244 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32580 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23036 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26820 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28684 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33004 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30020 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30180 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    46604 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45268 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    52684 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22396 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42764 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34180 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    41268 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29964 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35940 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25220 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    44148 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24796 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    37964 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22716 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24580 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    50548 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29540 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31940 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29004 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30500 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22180 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21916 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39780 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26500 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43084 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42284 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42548 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45324 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    37380 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33380 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    36364 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32420 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    58492 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35300 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    49004 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34444 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34020 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30284 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    58652 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1943 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/readme.md
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    57852 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24260 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51668 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29164 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27940 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45748 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25380 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42924 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38500 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26020 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24156 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20100 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16100 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29220 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21596 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21276 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    35724 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.868295 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39620 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27460 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24740 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31300 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30660 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31300 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23196 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    40100 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28524 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51084 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28100 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25220 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26236 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34980 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23780 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24740 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25540 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22716 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23300 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30180 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22020 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25116 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26236 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23780 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23356 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25700 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22020 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25436 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19940 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45804 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25700 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    52204 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    50764 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    49908 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    45108 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    55932 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32524 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43244 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32100 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32580 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25860 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27780 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29804 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25380 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    51404 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29380 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39404 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28740 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33804 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    40788 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30764 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28740 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30444 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29644 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    43724 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    42708 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    37644 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24420 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31244 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24100 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26716 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    40788 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25060 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20260 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31140 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26556 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26340 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19196 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39564 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23140 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23196 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27884 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31140 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23676 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24900 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34660 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28580 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    41428 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30764 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38180 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    38820 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29060 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30980 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    27724 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34500 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    36844 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26980 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26396 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28260 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30764 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28100 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28524 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39780 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39884 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    56628 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29220 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19940 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28204 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    44628 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20476 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    26020 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    39084 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    34660 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22076 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24476 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    24956 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28684 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33164 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    17220 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25276 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20260 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28204 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20636 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19836 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21060 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31300 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    29964 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    17436 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16900 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21060 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19300 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16156 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19620 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21380 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19460 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    32740 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19676 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    54548 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23516 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    22556 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    20580 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18396 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3759 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/bark_voice.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    33373 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/generation.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     9139 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/model.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5955 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bark/model_fine.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.868764 byzerllm-0.1.91/src/byzerllm/bge/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1022 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/bge/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.869644 byzerllm-0.1.91/src/byzerllm/bge_rerank/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      929 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/bge_rerank/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5748 2024-05-11 00:58:40.000000 byzerllm-0.1.91/src/byzerllm/byzerllm_command.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.870137 byzerllm-0.1.91/src/byzerllm/chatglm2/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2439 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/chatglm2/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.936747 byzerllm-0.1.91/src/byzerllm/chatglm6b/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8182 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/arguments.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    21286 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/finetune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11575 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/trainer_seq2seq.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.938593 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3000 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/finetune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1404 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/infer.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.942408 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      277 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16907 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/common.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7620 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/config.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6263 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/other.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11082 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7984 2024-05-11 00:58:29.000000 byzerllm-0.1.91/src/byzerllm/command_args.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.945913 byzerllm-0.1.91/src/byzerllm/dolly/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/dolly/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/dolly/consts.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1112 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/dolly/dolly_inference.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10065 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/dolly/generate.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12156 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/dolly/trainer.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.946577 byzerllm-0.1.91/src/byzerllm/falcon/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4414 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/falcon/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2362 2024-05-11 00:55:17.000000 byzerllm-0.1.91/src/byzerllm/lang.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.947279 byzerllm-0.1.91/src/byzerllm/llama/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6504 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/llama/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.948054 byzerllm-0.1.91/src/byzerllm/llama2/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6675 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/llama2/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2010 2024-04-01 10:03:54.000000 byzerllm-0.1.91/src/byzerllm/log.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.948705 byzerllm-0.1.91/src/byzerllm/m3e/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      189 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/m3e/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.950530 byzerllm-0.1.91/src/byzerllm/moss/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/moss/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12657 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/moss/finetune_moss.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.955099 byzerllm-0.1.91/src/byzerllm/moss/models/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/moss/models/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5097 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/moss/models/configuration_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6735 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/moss/models/custom_autotune.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31351 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/moss/models/modeling_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    18866 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/moss/models/quantization.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    15952 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/moss/models/tokenization_moss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16919 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/moss/moss_inference.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.955844 byzerllm-0.1.91/src/byzerllm/processor/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      577 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/processor/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.956519 byzerllm-0.1.91/src/byzerllm/qwen/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6510 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/qwen/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.957174 byzerllm-0.1.91/src/byzerllm/qwen_vl_chat/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3792 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/qwen_vl_chat/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.957770 byzerllm-0.1.91/src/byzerllm/records/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6824 2023-12-12 03:30:31.000000 byzerllm-0.1.91/src/byzerllm/records/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.958426 byzerllm-0.1.91/src/byzerllm/saas/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/saas/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.958672 byzerllm-0.1.91/src/byzerllm/saas/aws_bedrock/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11871 2024-05-11 12:03:07.000000 byzerllm-0.1.91/src/byzerllm/saas/aws_bedrock/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.959359 byzerllm-0.1.91/src/byzerllm/saas/azure/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     9857 2024-05-11 11:58:25.000000 byzerllm-0.1.91/src/byzerllm/saas/azure/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.960068 byzerllm-0.1.91/src/byzerllm/saas/azure_openai/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3454 2024-05-11 11:57:58.000000 byzerllm-0.1.91/src/byzerllm/saas/azure_openai/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.960722 byzerllm-0.1.91/src/byzerllm/saas/baichuan/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5331 2024-05-11 11:56:58.000000 byzerllm-0.1.91/src/byzerllm/saas/baichuan/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.961465 byzerllm-0.1.91/src/byzerllm/saas/chatglm/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2306 2023-12-26 06:22:53.000000 byzerllm-0.1.91/src/byzerllm/saas/chatglm/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.962131 byzerllm-0.1.91/src/byzerllm/saas/claude/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5753 2024-05-11 11:54:49.000000 byzerllm-0.1.91/src/byzerllm/saas/claude/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.962753 byzerllm-0.1.91/src/byzerllm/saas/gemini/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4517 2024-05-11 11:54:20.000000 byzerllm-0.1.91/src/byzerllm/saas/gemini/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.963333 byzerllm-0.1.91/src/byzerllm/saas/minimax/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    11064 2024-05-11 11:53:21.000000 byzerllm-0.1.91/src/byzerllm/saas/minimax/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.964142 byzerllm-0.1.91/src/byzerllm/saas/official_openai/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    16675 2024-05-17 14:21:16.000000 byzerllm-0.1.91/src/byzerllm/saas/official_openai/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.965384 byzerllm-0.1.91/src/byzerllm/saas/openai/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       83 2024-04-14 14:38:04.000000 byzerllm-0.1.91/src/byzerllm/saas/openai/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.966020 byzerllm-0.1.91/src/byzerllm/saas/qianfan/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6147 2024-05-11 11:49:15.000000 byzerllm-0.1.91/src/byzerllm/saas/qianfan/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.966634 byzerllm-0.1.91/src/byzerllm/saas/qianwen/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6830 2024-05-11 11:42:52.000000 byzerllm-0.1.91/src/byzerllm/saas/qianwen/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.967289 byzerllm-0.1.91/src/byzerllm/saas/qianwen_vl/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7083 2024-05-17 14:16:35.000000 byzerllm-0.1.91/src/byzerllm/saas/qianwen_vl/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.967910 byzerllm-0.1.91/src/byzerllm/saas/sparkdesk/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6707 2024-05-11 11:47:59.000000 byzerllm-0.1.91/src/byzerllm/saas/sparkdesk/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.968737 byzerllm-0.1.91/src/byzerllm/saas/volcengine/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     9214 2024-05-11 11:50:42.000000 byzerllm-0.1.91/src/byzerllm/saas/volcengine/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.969369 byzerllm-0.1.91/src/byzerllm/saas/zhipu/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5039 2024-05-11 11:51:47.000000 byzerllm-0.1.91/src/byzerllm/saas/zhipu/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.973840 byzerllm-0.1.91/src/byzerllm/stable_diffusion/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6453 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.974750 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.975326 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/diffusion/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/diffusion/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.975835 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/diffusion/pipelines/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/diffusion/pipelines/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4720 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.977148 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/events/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1701 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/events/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1006 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/events/generation.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.977928 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/models/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/models/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1260 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/models/diffusion.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      173 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/plugin.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1136 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/config.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.979647 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3127 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/embeddings.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.981008 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/networks/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3567 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8214 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.982729 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/piplines/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/piplines/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    31226 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10680 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.984242 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/upscalers/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/upscalers/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8276 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5247 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3104 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      673 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/images.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.984864 byzerllm-0.1.91/src/byzerllm/stable_diffusion/lib/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/lib/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.985680 byzerllm-0.1.91/src/byzerllm/stable_diffusion/lib/diffusers/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/lib/diffusers/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1246 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      434 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/logger.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4681 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/model.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      540 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/shared.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      928 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/stable_diffusion/utils.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.986265 byzerllm-0.1.91/src/byzerllm/starcode/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1882 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/starcode/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2422 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/store.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.993133 byzerllm-0.1.91/src/byzerllm/utils/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    25659 2024-04-26 09:09:23.000000 byzerllm-0.1.91/src/byzerllm/utils/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.997792 byzerllm-0.1.91/src/byzerllm/utils/client/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      884 2024-04-18 06:47:05.000000 byzerllm-0.1.91/src/byzerllm/utils/client/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    65237 2024-05-24 08:19:48.000000 byzerllm-0.1.91/src/byzerllm/utils/client/byzerllm_client.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    19055 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/utils/client/code_utils.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:06.998092 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.002357 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8922 2024-04-18 09:44:41.000000 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/api_server.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    14198 2024-04-01 10:03:54.000000 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/protocol.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6707 2024-04-23 09:24:35.000000 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/serve.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8887 2024-04-26 08:07:36.000000 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/serving_chat.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     7581 2024-04-26 08:08:28.000000 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/serving_completion.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5854 2024-04-23 05:50:42.000000 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/serving_engine.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8573 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/tool.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5777 2023-12-12 03:30:31.000000 byzerllm-0.1.91/src/byzerllm/utils/client/img_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10008 2023-12-12 03:30:31.000000 byzerllm-0.1.91/src/byzerllm/utils/client/math_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4275 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/utils/client/message_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1017 2024-01-18 03:33:00.000000 byzerllm-0.1.91/src/byzerllm/utils/client/parallel_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12377 2024-04-26 01:43:44.000000 byzerllm-0.1.91/src/byzerllm/utils/client/types.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.002923 byzerllm-0.1.91/src/byzerllm/utils/config/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1059 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/config/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2194 2024-05-10 09:22:55.000000 byzerllm-0.1.91/src/byzerllm/utils/connect_ray.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4042 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/emb.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.005271 byzerllm-0.1.91/src/byzerllm/utils/fulltune/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2637 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/fulltune/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.006967 byzerllm-0.1.91/src/byzerllm/utils/fulltune/base_model/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/fulltune/base_model/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2929 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    30037 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    12755 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/fulltune/deepspeed_trainner.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     4826 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/fulltune/launch.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.009083 byzerllm-0.1.91/src/byzerllm/utils/fulltune/pretrain/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    28458 2023-12-23 13:24:00.000000 byzerllm-0.1.91/src/byzerllm/utils/fulltune/pretrain/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2406 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6924 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/fulltune/trainner.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    14303 2024-04-08 04:52:43.000000 byzerllm-0.1.91/src/byzerllm/utils/json_repaire.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5187 2024-05-11 00:40:06.000000 byzerllm-0.1.91/src/byzerllm/utils/langutil.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.009844 byzerllm-0.1.91/src/byzerllm/utils/metrics/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1216 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/metrics/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)      367 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/object_store_ref_util.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2346 2023-12-26 06:22:53.000000 byzerllm-0.1.91/src/byzerllm/utils/openai_utils.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1446 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/utils/ray_utils.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.011918 byzerllm-0.1.91/src/byzerllm/utils/retrieval/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    13613 2024-04-16 13:20:54.000000 byzerllm-0.1.91/src/byzerllm/utils/retrieval/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     6019 2023-12-12 03:30:31.000000 byzerllm-0.1.91/src/byzerllm/utils/retrieval/rest.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1970 2023-12-12 03:30:31.000000 byzerllm-0.1.91/src/byzerllm/utils/retrieval/udf.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.017537 byzerllm-0.1.91/src/byzerllm/utils/sft/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10331 2023-12-23 13:24:00.000000 byzerllm-0.1.91/src/byzerllm/utils/sft/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1203 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/sft/argument.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2029 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/sft/collator.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3248 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/sft/dataset.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1614 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/sft/loss.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2295 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/sft/merge_lora.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2611 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/sft/model.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     8381 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/sft/qlora.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3395 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/sft/trainer.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1288 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/utils/testing.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    10903 2024-05-11 01:56:39.000000 byzerllm-0.1.91/src/byzerllm/utils/text_generator.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1633 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/utils/tokenizer.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5394 2024-04-27 05:50:08.000000 byzerllm-0.1.91/src/byzerllm/utils/types.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       23 2024-05-26 09:55:02.000000 byzerllm-0.1.91/src/byzerllm/version.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.018116 byzerllm-0.1.91/src/byzerllm/visualglm/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2462 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/visualglm/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.018895 byzerllm-0.1.91/src/byzerllm/whisper/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/whisper/__init__.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1254 2023-10-10 02:45:08.000000 byzerllm-0.1.91/src/byzerllm/whisper/whisper_inference.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.019844 byzerllm-0.1.91/src/byzerllm/zephyr/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     5628 2024-03-31 13:19:57.000000 byzerllm-0.1.91/src/byzerllm/zephyr/__init__.py
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.025808 byzerllm-0.1.91/src/byzerllm.egg-info/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    83884 2024-05-26 09:56:06.000000 byzerllm-0.1.91/src/byzerllm.egg-info/PKG-INFO
+-rw-r--r--   0 allwefantasy   (501) staff       (20)    23396 2024-05-26 09:56:06.000000 byzerllm-0.1.91/src/byzerllm.egg-info/SOURCES.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        1 2024-05-26 09:56:06.000000 byzerllm-0.1.91/src/byzerllm.egg-info/dependency_links.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)       60 2024-05-26 09:56:06.000000 byzerllm-0.1.91/src/byzerllm.egg-info/entry_points.txt
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        9 2024-05-26 09:56:06.000000 byzerllm-0.1.91/src/byzerllm.egg-info/top_level.txt
+drwxr-xr-x   0 allwefantasy   (501) staff       (20)        0 2024-05-26 09:56:07.025032 byzerllm-0.1.91/tests/
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1603 2024-04-18 05:04:09.000000 byzerllm-0.1.91/tests/test_data_analysis.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3235 2024-04-18 05:04:09.000000 byzerllm-0.1.91/tests/test_deepseek_code.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1248 2024-04-18 05:04:09.000000 byzerllm-0.1.91/tests/test_deploy.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     2041 2024-04-18 05:04:09.000000 byzerllm-0.1.91/tests/test_emb_rerank.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1187 2024-04-18 05:04:09.000000 byzerllm-0.1.91/tests/test_model_meta.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1413 2024-04-15 08:05:56.000000 byzerllm-0.1.91/tests/test_prompt.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     3522 2024-04-18 05:04:09.000000 byzerllm-0.1.91/tests/test_template.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)        0 2024-04-18 05:04:09.000000 byzerllm-0.1.91/tests/test_transformers_deploy.py
+-rw-r--r--   0 allwefantasy   (501) staff       (20)     1664 2024-04-18 05:04:09.000000 byzerllm-0.1.91/tests/test_yi.py
```

### Comparing `byzerllm-0.1.90/LICENSE` & `byzerllm-0.1.91/LICENSE`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/PKG-INFO` & `byzerllm-0.1.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byzerllm
-Version: 0.1.90
+Version: 0.1.91
 Summary: ByzerLLM: Byzer LLM
 Author: allwefantasy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: byzerllm Version: 0.1.90 Summary: ByzerLLM: Byzer
+Metadata-Version: 2.1 Name: byzerllm Version: 0.1.91 Summary: ByzerLLM: Byzer
 LLM Author: allwefantasy Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
 text/markdown License-File: LICENSE
                                   [Byzer-LLM]
     ******** EEaassyy,, ffaasstt,, aanndd cchheeaapp pprreettrraaiinn,,ffiinneettuunnee,, sseerrvviinngg ffoorr eevveerryyoonnee ********
                              | _EE_nn_gg_ll_ii_ss_hh | _?ä_?¸_?­_?æ_?_? |
```

### Comparing `byzerllm-0.1.90/README.md` & `byzerllm-0.1.91/README.md`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/setup.py` & `byzerllm-0.1.91/setup.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/__init__.py` & `byzerllm-0.1.91/src/byzerllm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,30 +317,36 @@
 
         is_lambda = inspect.isfunction(llm) and llm.__name__ == '<lambda>'
         if is_lambda:      
             return_origin_response = True if self.response_markers else False
             v = llm(self.instance).prompt(render=render,check_result=check_result,
                                           options=self._options,
                                           return_origin_response=return_origin_response)(func)(**input_dict)
+            if not return_origin_response:
+                return v
             return self._multi_turn_wrapper(llm(self.instance),v,signature)    
 
             
         if isinstance(llm,ByzerLLM):
             return_origin_response = True if self.response_markers else False
             v = llm.prompt(render=render,check_result=check_result,options=self._options,
                            return_origin_response=return_origin_response)(func)(**input_dict)
+            if not return_origin_response:
+                return v
             return self._multi_turn_wrapper(llm,v,signature)
         
         if isinstance(llm,str):
             _llm = ByzerLLM()
             _llm.setup_default_model_name(llm)
             _llm.setup_template(llm,"auto")  
             return_origin_response = True if self.response_markers else False       
             v = _llm.prompt(render=render,check_result=check_result,options=self._options,
-                            return_origin_response=return_origin_response)(func)(**input_dict)  
+                            return_origin_response=return_origin_response)(func)(**input_dict) 
+            if not return_origin_response:
+                return v 
             return self._multi_turn_wrapper(llm,v,signature)
                 
         else:
             raise ValueError("llm should be a lambda function or ByzerLLM instance or a string of model name")  
     
 
 class _DescriptorPrompt:
```

### Comparing `byzerllm-0.1.90/src/byzerllm/alpha_moss/__init__.py` & `byzerllm-0.1.91/src/byzerllm/alpha_moss/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/__init__.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/conversable_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/conversable_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/assistant_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/assistant_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/byzer_engine_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/byzer_engine_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/common_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/common_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/data_analysis.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/data_analysis.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/data_analysis_pipeline_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/data_analysis_pipeline_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/llama_index_retrieval_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/llama_index_retrieval_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/load_data_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/load_data_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/output_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/output_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/planner.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/planner.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/preview_file_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/preview_file_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/python_codesandbox_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/python_codesandbox_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/condition.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/condition.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/context.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/context.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/rhetorical.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/rhetorical.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/query_rewrite/time.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/query_rewrite/time.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/retrieval_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/retrieval_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/rhetorical_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/rhetorical_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/simple_retrieval_client.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/simple_retrieval_client.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/spark_sql_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/spark_sql_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/sql_reviewer_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/sql_reviewer_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/subquestion_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/subquestion_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/extensions/visualization_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/extensions/visualization_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/groupchat.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/groupchat.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/registry.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/registry.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/store/memory_store.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/store/memory_store.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/store/stores.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/store/stores.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/agent/user_proxy_agent.py` & `byzerllm-0.1.91/src/byzerllm/apps/agent/user_proxy_agent.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/builder.py` & `byzerllm-0.1.91/src/byzerllm/apps/builder.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/byzer_sql/__init__.py` & `byzerllm-0.1.91/src/byzerllm/apps/byzer_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/command.py` & `byzerllm-0.1.91/src/byzerllm/apps/byzer_storage/command.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/byzer_storage/env.py` & `byzerllm-0.1.91/src/byzerllm/apps/byzer_storage/env.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/client.py` & `byzerllm-0.1.91/src/byzerllm/apps/client.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/llama_index/__init__.py` & `byzerllm-0.1.91/src/byzerllm/apps/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai.py` & `byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_docstore.py` & `byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_docstore.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_embedding.py` & `byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_embedding.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_index_store.py` & `byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_index_store.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_kvstore.py` & `byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_kvstore.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/llama_index/byzerai_vectordb.py` & `byzerllm-0.1.91/src/byzerllm/apps/llama_index/byzerai_vectordb.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/llama_index/collection_manager.py` & `byzerllm-0.1.91/src/byzerllm/apps/llama_index/collection_manager.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/llama_index/simple_retrieval.py` & `byzerllm-0.1.91/src/byzerllm/apps/llama_index/simple_retrieval.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/qa.py` & `byzerllm-0.1.91/src/byzerllm/apps/qa.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/qa_strategy.py` & `byzerllm-0.1.91/src/byzerllm/apps/qa_strategy.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/apps/vector_db.py` & `byzerllm-0.1.91/src/byzerllm/apps/vector_db.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/auto/__init__.py` & `byzerllm-0.1.91/src/byzerllm/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/auto/backend_ds.py` & `byzerllm-0.1.91/src/byzerllm/auto/backend_ds.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/auto/backend_llama_cpp.py` & `byzerllm-0.1.91/src/byzerllm/auto/backend_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/baichuan/__init__.py` & `byzerllm-0.1.91/src/byzerllm/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/api.py` & `byzerllm-0.1.91/src/byzerllm/bark/api.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/announcer.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/announcer.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/de_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/de_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/en_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/en_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/es_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/es_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/it_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/it_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/readme.md` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/readme.md`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz` & `byzerllm-0.1.91/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/bark_voice.py` & `byzerllm-0.1.91/src/byzerllm/bark/bark_voice.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/generation.py` & `byzerllm-0.1.91/src/byzerllm/bark/generation.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/model.py` & `byzerllm-0.1.91/src/byzerllm/bark/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bark/model_fine.py` & `byzerllm-0.1.91/src/byzerllm/bark/model_fine.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bge/__init__.py` & `byzerllm-0.1.91/src/byzerllm/bge/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/bge_rerank/__init__.py` & `byzerllm-0.1.91/src/byzerllm/bge_rerank/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/byzerllm_command.py` & `byzerllm-0.1.91/src/byzerllm/byzerllm_command.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm2/__init__.py` & `byzerllm-0.1.91/src/byzerllm/chatglm2/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm6b/arguments.py` & `byzerllm-0.1.91/src/byzerllm/chatglm6b/arguments.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm6b/finetune.py` & `byzerllm-0.1.91/src/byzerllm/chatglm6b/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm6b/trainer_seq2seq.py` & `byzerllm-0.1.91/src/byzerllm/chatglm6b/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/finetune.py` & `byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/infer.py` & `byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/infer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/common.py` & `byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/common.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/config.py` & `byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/config.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/other.py` & `byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/other.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py` & `byzerllm-0.1.91/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/command_args.py` & `byzerllm-0.1.91/src/byzerllm/command_args.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/dolly/consts.py` & `byzerllm-0.1.91/src/byzerllm/dolly/consts.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/dolly/dolly_inference.py` & `byzerllm-0.1.91/src/byzerllm/dolly/dolly_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/dolly/generate.py` & `byzerllm-0.1.91/src/byzerllm/dolly/generate.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/dolly/trainer.py` & `byzerllm-0.1.91/src/byzerllm/dolly/trainer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/falcon/__init__.py` & `byzerllm-0.1.91/src/byzerllm/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/lang.py` & `byzerllm-0.1.91/src/byzerllm/lang.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/llama/__init__.py` & `byzerllm-0.1.91/src/byzerllm/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/llama2/__init__.py` & `byzerllm-0.1.91/src/byzerllm/llama2/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/log.py` & `byzerllm-0.1.91/src/byzerllm/log.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/moss/finetune_moss.py` & `byzerllm-0.1.91/src/byzerllm/moss/finetune_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/moss/models/configuration_moss.py` & `byzerllm-0.1.91/src/byzerllm/moss/models/configuration_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/moss/models/custom_autotune.py` & `byzerllm-0.1.91/src/byzerllm/moss/models/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/moss/models/modeling_moss.py` & `byzerllm-0.1.91/src/byzerllm/moss/models/modeling_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/moss/models/quantization.py` & `byzerllm-0.1.91/src/byzerllm/moss/models/quantization.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/moss/models/tokenization_moss.py` & `byzerllm-0.1.91/src/byzerllm/moss/models/tokenization_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/moss/moss_inference.py` & `byzerllm-0.1.91/src/byzerllm/moss/moss_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/processor/__init__.py` & `byzerllm-0.1.91/src/byzerllm/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/qwen/__init__.py` & `byzerllm-0.1.91/src/byzerllm/qwen/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/qwen_vl_chat/__init__.py` & `byzerllm-0.1.91/src/byzerllm/qwen_vl_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/records/__init__.py` & `byzerllm-0.1.91/src/byzerllm/records/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/aws_bedrock/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/aws_bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/azure/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/azure_openai/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/azure_openai/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/baichuan/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/chatglm/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/claude/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/claude/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/gemini/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/minimax/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/minimax/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/official_openai/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/official_openai/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/qianfan/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/qianfan/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/qianwen/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/qianwen/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/qianwen_vl/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/qianwen_vl/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/sparkdesk/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/sparkdesk/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/volcengine/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/volcengine/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/saas/zhipu/__init__.py` & `byzerllm-0.1.91/src/byzerllm/saas/zhipu/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/__init__.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/__init__.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/events/generation.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/events/generation.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/api/models/diffusion.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/api/models/diffusion.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/config.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/embeddings.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/embeddings.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/diffusion/utils.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/images.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/images.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/model.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/shared.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/shared.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/stable_diffusion/utils.py` & `byzerllm-0.1.91/src/byzerllm/stable_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/starcode/__init__.py` & `byzerllm-0.1.91/src/byzerllm/starcode/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/store.py` & `byzerllm-0.1.91/src/byzerllm/store.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/__init__.py` & `byzerllm-0.1.91/src/byzerllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/__init__.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/byzerllm_client.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/byzerllm_client.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/code_utils.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/code_utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/api_server.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/api_server.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/protocol.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/protocol.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serve.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/serve.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serving_chat.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/serving_chat.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serving_completion.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/serving_completion.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/serving_engine.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/serving_engine.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/entrypoints/openai/tool.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/entrypoints/openai/tool.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/img_utils.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/img_utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/math_utils.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/math_utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/message_utils.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/message_utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/parallel_utils.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/client/types.py` & `byzerllm-0.1.91/src/byzerllm/utils/client/types.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/config/__init__.py` & `byzerllm-0.1.91/src/byzerllm/utils/config/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/connect_ray.py` & `byzerllm-0.1.91/src/byzerllm/utils/connect_ray.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/emb.py` & `byzerllm-0.1.91/src/byzerllm/utils/emb.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/fulltune/__init__.py` & `byzerllm-0.1.91/src/byzerllm/utils/fulltune/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py` & `byzerllm-0.1.91/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py` & `byzerllm-0.1.91/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/fulltune/deepspeed_trainner.py` & `byzerllm-0.1.91/src/byzerllm/utils/fulltune/deepspeed_trainner.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/fulltune/launch.py` & `byzerllm-0.1.91/src/byzerllm/utils/fulltune/launch.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/__init__.py` & `byzerllm-0.1.91/src/byzerllm/utils/fulltune/pretrain/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py` & `byzerllm-0.1.91/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/fulltune/trainner.py` & `byzerllm-0.1.91/src/byzerllm/utils/fulltune/trainner.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/json_repaire.py` & `byzerllm-0.1.91/src/byzerllm/utils/json_repaire.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/langutil.py` & `byzerllm-0.1.91/src/byzerllm/utils/langutil.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/metrics/__init__.py` & `byzerllm-0.1.91/src/byzerllm/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/openai_utils.py` & `byzerllm-0.1.91/src/byzerllm/utils/openai_utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/ray_utils.py` & `byzerllm-0.1.91/src/byzerllm/utils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/retrieval/__init__.py` & `byzerllm-0.1.91/src/byzerllm/utils/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/retrieval/rest.py` & `byzerllm-0.1.91/src/byzerllm/utils/retrieval/rest.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/retrieval/udf.py` & `byzerllm-0.1.91/src/byzerllm/utils/retrieval/udf.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/sft/__init__.py` & `byzerllm-0.1.91/src/byzerllm/utils/sft/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/sft/argument.py` & `byzerllm-0.1.91/src/byzerllm/utils/sft/argument.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/sft/collator.py` & `byzerllm-0.1.91/src/byzerllm/utils/sft/collator.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/sft/dataset.py` & `byzerllm-0.1.91/src/byzerllm/utils/sft/dataset.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/sft/loss.py` & `byzerllm-0.1.91/src/byzerllm/utils/sft/loss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/sft/merge_lora.py` & `byzerllm-0.1.91/src/byzerllm/utils/sft/merge_lora.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/sft/model.py` & `byzerllm-0.1.91/src/byzerllm/utils/sft/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/sft/qlora.py` & `byzerllm-0.1.91/src/byzerllm/utils/sft/qlora.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/sft/trainer.py` & `byzerllm-0.1.91/src/byzerllm/utils/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/testing.py` & `byzerllm-0.1.91/src/byzerllm/utils/testing.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/text_generator.py` & `byzerllm-0.1.91/src/byzerllm/utils/text_generator.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/tokenizer.py` & `byzerllm-0.1.91/src/byzerllm/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/utils/types.py` & `byzerllm-0.1.91/src/byzerllm/utils/types.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/visualglm/__init__.py` & `byzerllm-0.1.91/src/byzerllm/visualglm/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/whisper/whisper_inference.py` & `byzerllm-0.1.91/src/byzerllm/whisper/whisper_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm/zephyr/__init__.py` & `byzerllm-0.1.91/src/byzerllm/zephyr/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/src/byzerllm.egg-info/PKG-INFO` & `byzerllm-0.1.91/src/byzerllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byzerllm
-Version: 0.1.90
+Version: 0.1.91
 Summary: ByzerLLM: Byzer LLM
 Author: allwefantasy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: byzerllm Version: 0.1.90 Summary: ByzerLLM: Byzer
+Metadata-Version: 2.1 Name: byzerllm Version: 0.1.91 Summary: ByzerLLM: Byzer
 LLM Author: allwefantasy Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
 text/markdown License-File: LICENSE
                                   [Byzer-LLM]
     ******** EEaassyy,, ffaasstt,, aanndd cchheeaapp pprreettrraaiinn,,ffiinneettuunnee,, sseerrvviinngg ffoorr eevveerryyoonnee ********
                              | _EE_nn_gg_ll_ii_ss_hh | _?ä_?¸_?­_?æ_?_? |
```

### Comparing `byzerllm-0.1.90/src/byzerllm.egg-info/SOURCES.txt` & `byzerllm-0.1.91/src/byzerllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/tests/test_data_analysis.py` & `byzerllm-0.1.91/tests/test_data_analysis.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/tests/test_deepseek_code.py` & `byzerllm-0.1.91/tests/test_deepseek_code.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/tests/test_deploy.py` & `byzerllm-0.1.91/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/tests/test_emb_rerank.py` & `byzerllm-0.1.91/tests/test_emb_rerank.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/tests/test_model_meta.py` & `byzerllm-0.1.91/tests/test_model_meta.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/tests/test_prompt.py` & `byzerllm-0.1.91/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/tests/test_template.py` & `byzerllm-0.1.91/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.90/tests/test_yi.py` & `byzerllm-0.1.91/tests/test_yi.py`

 * *Files identical despite different names*

