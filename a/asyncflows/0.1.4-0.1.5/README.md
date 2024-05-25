# Comparing `tmp/asyncflows-0.1.4.tar.gz` & `tmp/asyncflows-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncflows-0.1.4.tar", max compression
+gzip compressed data, was "asyncflows-0.1.5.tar", max compression
```

## Comparing `asyncflows-0.1.4.tar` & `asyncflows-0.1.5.tar`

### file list

```diff
@@ -1,97 +1,99 @@
--rw-r--r--   0        0        0     4019 2024-05-22 14:49:22.081858 asyncflows-0.1.4/LICENSE
--rw-r--r--   0        0        0    32784 2024-05-22 21:59:56.341625 asyncflows-0.1.4/README.md
--rw-r--r--   0        0        0      215 2024-05-22 14:47:42.260962 asyncflows-0.1.4/asyncflows/__init__.py
--rw-r--r--   0        0        0      721 2024-05-22 14:46:03.753765 asyncflows-0.1.4/asyncflows/actions/__init__.py
--rw-r--r--   0        0        0     6399 2024-05-22 14:47:42.261515 asyncflows-0.1.4/asyncflows/actions/base.py
--rw-r--r--   0        0        0     1867 2024-05-22 14:48:15.151039 asyncflows-0.1.4/asyncflows/actions/execute_db_statement.py
--rw-r--r--   0        0        0     1385 2024-05-22 14:49:22.057325 asyncflows-0.1.4/asyncflows/actions/extract_list.py
--rw-r--r--   0        0        0     1982 2024-05-22 18:55:04.922974 asyncflows-0.1.4/asyncflows/actions/extract_pdf_text.py
--rw-r--r--   0        0        0     1428 2024-05-22 14:47:42.368774 asyncflows-0.1.4/asyncflows/actions/extract_xml_tag.py
--rw-r--r--   0        0        0     1168 2024-05-22 14:48:15.151258 asyncflows-0.1.4/asyncflows/actions/get_db_schema.py
--rw-r--r--   0        0        0      582 2024-05-22 14:47:42.261922 asyncflows-0.1.4/asyncflows/actions/get_url.py
--rw-r--r--   0        0        0      860 2024-05-22 14:47:42.317491 asyncflows-0.1.4/asyncflows/actions/ocr.py
--rw-r--r--   0        0        0    13123 2024-05-22 21:28:30.269737 asyncflows-0.1.4/asyncflows/actions/prompt.py
--rw-r--r--   0        0        0     1297 2024-05-22 14:47:42.262400 asyncflows-0.1.4/asyncflows/actions/score.py
--rw-r--r--   0        0        0     4309 2024-05-22 18:55:04.923294 asyncflows-0.1.4/asyncflows/actions/transformer.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755456 asyncflows-0.1.4/asyncflows/actions/utils/__init__.py
--rw-r--r--   0        0        0     5351 2024-05-22 21:28:30.270167 asyncflows-0.1.4/asyncflows/actions/utils/prompt_context.py
--rw-r--r--   0        0        0     3678 2024-05-22 14:49:22.043426 asyncflows-0.1.4/asyncflows/asyncflows.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755962 asyncflows-0.1.4/asyncflows/examples/__init__.py
--rw-r--r--   0        0        0   287615 2024-05-22 18:55:04.925115 asyncflows-0.1.4/asyncflows/examples/books/Alice's Adventures in Wonderland, by Lewis Carroll.pdf
--rw-r--r--   0        0        0     1533 2024-05-22 18:55:04.925408 asyncflows-0.1.4/asyncflows/examples/chatbot.py
--rw-r--r--   0        0        0     3146 2024-05-22 21:52:45.305210 asyncflows-0.1.4/asyncflows/examples/chatbot.yaml
--rw-r--r--   0        0        0      716 2024-05-22 14:47:42.404980 asyncflows-0.1.4/asyncflows/examples/debono.py
--rw-r--r--   0        0        0     3411 2024-05-22 21:52:45.351058 asyncflows-0.1.4/asyncflows/examples/debono.yaml
--rw-r--r--   0        0        0      699 2024-05-22 14:47:42.405239 asyncflows-0.1.4/asyncflows/examples/get_page_title.py
--rw-r--r--   0        0        0      486 2024-05-22 21:52:45.283127 asyncflows-0.1.4/asyncflows/examples/get_page_title.yaml
--rw-r--r--   0        0        0   294692 2024-05-22 14:49:22.077191 asyncflows-0.1.4/asyncflows/examples/hello_world.ipynb
--rw-r--r--   0        0        0      651 2024-05-22 14:47:42.405500 asyncflows-0.1.4/asyncflows/examples/hello_world.py
--rw-r--r--   0        0        0      323 2024-05-22 21:52:45.315267 asyncflows-0.1.4/asyncflows/examples/hello_world.yaml
--rw-r--r--   0        0        0     1309 2024-05-22 18:55:04.927602 asyncflows-0.1.4/asyncflows/examples/rag.py
--rw-r--r--   0        0        0     1133 2024-05-22 21:52:45.345900 asyncflows-0.1.4/asyncflows/examples/rag.yaml
--rw-r--r--   0        0        0      280 2024-05-22 14:46:03.758066 asyncflows-0.1.4/asyncflows/examples/recipes/caprese.md
--rw-r--r--   0        0        0      380 2024-05-22 14:46:03.758468 asyncflows-0.1.4/asyncflows/examples/recipes/chana_masala.md
--rw-r--r--   0        0        0      329 2024-05-22 14:46:03.758593 asyncflows-0.1.4/asyncflows/examples/recipes/coconut_soup.md
--rw-r--r--   0        0        0      413 2024-05-22 14:46:03.758715 asyncflows-0.1.4/asyncflows/examples/recipes/gazpacho.md
--rw-r--r--   0        0        0      326 2024-05-22 14:46:03.758850 asyncflows-0.1.4/asyncflows/examples/recipes/guacamole.md
--rw-r--r--   0        0        0      375 2024-05-22 14:46:03.758989 asyncflows-0.1.4/asyncflows/examples/recipes/hummus.md
--rw-r--r--   0        0        0      326 2024-05-22 14:46:03.759115 asyncflows-0.1.4/asyncflows/examples/recipes/miso_soup.md
--rw-r--r--   0        0        0      331 2024-05-22 14:46:03.759255 asyncflows-0.1.4/asyncflows/examples/recipes/omelette.md
--rw-r--r--   0        0        0      327 2024-05-22 14:46:03.759525 asyncflows-0.1.4/asyncflows/examples/recipes/stir_fry.md
--rw-r--r--   0        0        0      321 2024-05-22 14:46:03.759651 asyncflows-0.1.4/asyncflows/examples/recipes/yogurt_parfait.md
--rw-r--r--   0        0        0     1105 2024-05-22 14:47:42.413403 asyncflows-0.1.4/asyncflows/examples/sql_rag.py
--rw-r--r--   0        0        0     1604 2024-05-22 21:52:45.343017 asyncflows-0.1.4/asyncflows/examples/sql_rag.yaml
--rw-r--r--   0        0        0     1198 2024-05-22 21:28:30.271238 asyncflows-0.1.4/asyncflows/examples/text_style_transfer.py
--rw-r--r--   0        0        0      571 2024-05-22 21:52:45.319275 asyncflows-0.1.4/asyncflows/examples/text_style_transfer.yaml
--rw-r--r--   0        0        0     1890 2024-05-22 14:46:03.761643 asyncflows-0.1.4/asyncflows/log_config.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.761683 asyncflows-0.1.4/asyncflows/models/__init__.py
--rw-r--r--   0        0        0      204 2024-05-22 14:46:03.761990 asyncflows-0.1.4/asyncflows/models/blob.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.762029 asyncflows-0.1.4/asyncflows/models/config/__init__.py
--rw-r--r--   0        0        0     3639 2024-05-22 14:49:41.998538 asyncflows-0.1.4/asyncflows/models/config/action.py
--rw-r--r--   0        0        0     2681 2024-05-22 14:46:03.762355 asyncflows-0.1.4/asyncflows/models/config/common.py
--rw-r--r--   0        0        0     1115 2024-05-22 14:49:41.998821 asyncflows-0.1.4/asyncflows/models/config/flow.py
--rw-r--r--   0        0        0     2422 2024-05-22 21:28:30.271703 asyncflows-0.1.4/asyncflows/models/config/model.py
--rw-r--r--   0        0        0     5075 2024-05-22 14:49:41.999198 asyncflows-0.1.4/asyncflows/models/config/transform.py
--rw-r--r--   0        0        0     5022 2024-05-22 14:49:22.058252 asyncflows-0.1.4/asyncflows/models/config/value_declarations.py
--rw-r--r--   0        0        0     3303 2024-05-22 14:49:22.058580 asyncflows-0.1.4/asyncflows/models/file.py
--rw-r--r--   0        0        0      700 2024-05-22 14:47:42.230677 asyncflows-0.1.4/asyncflows/models/primitives.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.763641 asyncflows-0.1.4/asyncflows/repos/__init__.py
--rw-r--r--   0        0        0    20233 2024-05-22 14:46:03.764021 asyncflows-0.1.4/asyncflows/repos/blob_repo.py
--rw-r--r--   0        0        0     4421 2024-05-22 14:46:03.764605 asyncflows-0.1.4/asyncflows/repos/cache_repo.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764679 asyncflows-0.1.4/asyncflows/scripts/__init__.py
--rw-r--r--   0        0        0     4943 2024-05-22 14:49:41.999576 asyncflows-0.1.4/asyncflows/scripts/generate_config_schema.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764985 asyncflows-0.1.4/asyncflows/services/__init__.py
--rw-r--r--   0        0        0    38289 2024-05-22 14:49:22.059469 asyncflows-0.1.4/asyncflows/services/action_service.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765630 asyncflows-0.1.4/asyncflows/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765743 asyncflows-0.1.4/asyncflows/tests/action_tests/__init__.py
--rw-r--r--   0        0        0      724 2024-05-22 14:48:15.166644 asyncflows-0.1.4/asyncflows/tests/action_tests/test_execute_db_statement.py
--rw-r--r--   0        0        0     1260 2024-05-22 14:47:42.369030 asyncflows-0.1.4/asyncflows/tests/action_tests/test_extract_xml_tag.py
--rw-r--r--   0        0        0      683 2024-05-22 14:48:15.166773 asyncflows-0.1.4/asyncflows/tests/action_tests/test_get_db_schema.py
--rw-r--r--   0        0        0     7949 2024-05-22 21:28:30.271910 asyncflows-0.1.4/asyncflows/tests/action_tests/test_prompt.py
--rw-r--r--   0        0        0     1902 2024-05-22 14:46:03.766510 asyncflows-0.1.4/asyncflows/tests/action_tests/test_transformers.py
--rw-r--r--   0        0        0    11472 2024-05-22 18:55:04.928549 asyncflows-0.1.4/asyncflows/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.766988 asyncflows-0.1.4/asyncflows/tests/repos/__init__.py
--rw-r--r--   0        0        0     8319 2024-05-22 14:46:03.767510 asyncflows-0.1.4/asyncflows/tests/repos/test_blob_repo.py
--rw-r--r--   0        0        0     6567 2024-05-22 14:46:03.767743 asyncflows-0.1.4/asyncflows/tests/repos/test_cache_repo.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.767812 asyncflows-0.1.4/asyncflows/tests/resources/__init__.py
--rw-r--r--   0        0        0     5737 2024-05-22 14:47:42.263059 asyncflows-0.1.4/asyncflows/tests/resources/actions.py
--rw-r--r--   0        0        0     4075 2024-05-22 14:47:42.287921 asyncflows-0.1.4/asyncflows/tests/resources/testing_actions.yaml
--rw-r--r--   0        0        0    26138 2024-05-22 14:47:42.323379 asyncflows-0.1.4/asyncflows/tests/test_action_service.py
--rw-r--r--   0        0        0     6172 2024-05-22 14:47:42.263271 asyncflows-0.1.4/asyncflows/tests/test_async_utils.py
--rw-r--r--   0        0        0    11747 2024-05-22 18:55:04.928969 asyncflows-0.1.4/asyncflows/tests/test_config.py
--rw-r--r--   0        0        0     2053 2024-05-22 14:48:15.167483 asyncflows-0.1.4/asyncflows/tests/test_run_examples.py
--rw-r--r--   0        0        0        0 2024-05-22 14:46:03.769749 asyncflows-0.1.4/asyncflows/utils/__init__.py
--rw-r--r--   0        0        0     9747 2024-05-22 14:49:22.060097 asyncflows-0.1.4/asyncflows/utils/async_utils.py
--rw-r--r--   0        0        0      676 2024-05-22 14:46:03.770301 asyncflows-0.1.4/asyncflows/utils/cache_utils.py
--rw-r--r--   0        0        0     8592 2024-05-22 18:55:04.929288 asyncflows-0.1.4/asyncflows/utils/config_utils.py
--rw-r--r--   0        0        0      725 2024-05-22 14:47:42.393837 asyncflows-0.1.4/asyncflows/utils/db_utils.py
--rw-r--r--   0        0        0     1320 2024-05-22 14:46:03.771069 asyncflows-0.1.4/asyncflows/utils/jinja_utils.py
--rw-r--r--   0        0        0     1482 2024-05-22 14:46:03.771192 asyncflows-0.1.4/asyncflows/utils/redis_utils.py
--rw-r--r--   0        0        0     2686 2024-05-22 14:46:03.771325 asyncflows-0.1.4/asyncflows/utils/request_utils.py
--rw-r--r--   0        0        0      382 2024-05-22 14:46:03.771449 asyncflows-0.1.4/asyncflows/utils/secret_utils.py
--rw-r--r--   0        0        0      479 2024-05-22 14:46:03.771565 asyncflows-0.1.4/asyncflows/utils/sentinel_utils.py
--rw-r--r--   0        0        0      451 2024-05-22 14:46:03.771681 asyncflows-0.1.4/asyncflows/utils/singleton_utils.py
--rw-r--r--   0        0        0     3333 2024-05-22 14:47:42.303806 asyncflows-0.1.4/asyncflows/utils/transformers_utils.py
--rw-r--r--   0        0        0     2507 2024-05-22 14:46:03.772050 asyncflows-0.1.4/asyncflows/utils/type_utils.py
--rw-r--r--   0        0        0     2547 2024-05-22 22:08:06.376173 asyncflows-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    34895 1970-01-01 00:00:00.000000 asyncflows-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4019 2024-05-22 14:49:22.081858 asyncflows-0.1.5/LICENSE
+-rw-r--r--   0        0        0    32806 2024-05-25 22:56:21.937598 asyncflows-0.1.5/README.md
+-rw-r--r--   0        0        0      215 2024-05-22 14:47:42.260962 asyncflows-0.1.5/asyncflows/__init__.py
+-rw-r--r--   0        0        0      721 2024-05-22 14:46:03.753765 asyncflows-0.1.5/asyncflows/actions/__init__.py
+-rw-r--r--   0        0        0     6399 2024-05-22 14:47:42.261515 asyncflows-0.1.5/asyncflows/actions/base.py
+-rw-r--r--   0        0        0     2143 2024-05-25 22:56:21.938190 asyncflows-0.1.5/asyncflows/actions/execute_db_statement.py
+-rw-r--r--   0        0        0     1385 2024-05-22 14:49:22.057325 asyncflows-0.1.5/asyncflows/actions/extract_list.py
+-rw-r--r--   0        0        0     1982 2024-05-22 18:55:04.922974 asyncflows-0.1.5/asyncflows/actions/extract_pdf_text.py
+-rw-r--r--   0        0        0     1428 2024-05-22 14:47:42.368774 asyncflows-0.1.5/asyncflows/actions/extract_xml_tag.py
+-rw-r--r--   0        0        0     1267 2024-05-25 22:56:21.943880 asyncflows-0.1.5/asyncflows/actions/get_db_schema.py
+-rw-r--r--   0        0        0      582 2024-05-22 14:47:42.261922 asyncflows-0.1.5/asyncflows/actions/get_url.py
+-rw-r--r--   0        0        0      860 2024-05-22 14:47:42.317491 asyncflows-0.1.5/asyncflows/actions/ocr.py
+-rw-r--r--   0        0        0    16519 2024-05-25 22:46:36.212088 asyncflows-0.1.5/asyncflows/actions/prompt.py
+-rw-r--r--   0        0        0     1297 2024-05-22 14:47:42.262400 asyncflows-0.1.5/asyncflows/actions/score.py
+-rw-r--r--   0        0        0     4309 2024-05-22 18:55:04.923294 asyncflows-0.1.5/asyncflows/actions/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755456 asyncflows-0.1.5/asyncflows/actions/utils/__init__.py
+-rw-r--r--   0        0        0     5351 2024-05-22 21:28:30.270167 asyncflows-0.1.5/asyncflows/actions/utils/prompt_context.py
+-rw-r--r--   0        0        0     4447 2024-05-25 20:36:32.571393 asyncflows-0.1.5/asyncflows/asyncflows.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755962 asyncflows-0.1.5/asyncflows/examples/__init__.py
+-rw-r--r--   0        0        0   287615 2024-05-22 18:55:04.925115 asyncflows-0.1.5/asyncflows/examples/books/Alice's Adventures in Wonderland, by Lewis Carroll.pdf
+-rw-r--r--   0        0        0     1533 2024-05-22 18:55:04.925408 asyncflows-0.1.5/asyncflows/examples/chatbot.py
+-rw-r--r--   0        0        0     3150 2024-05-25 22:40:56.343582 asyncflows-0.1.5/asyncflows/examples/chatbot.yaml
+-rw-r--r--   0        0        0      716 2024-05-22 14:47:42.404980 asyncflows-0.1.5/asyncflows/examples/debono.py
+-rw-r--r--   0        0        0     3415 2024-05-25 22:40:56.344104 asyncflows-0.1.5/asyncflows/examples/debono.yaml
+-rw-r--r--   0        0        0      699 2024-05-22 14:47:42.405239 asyncflows-0.1.5/asyncflows/examples/get_page_title.py
+-rw-r--r--   0        0        0      490 2024-05-25 22:40:56.344484 asyncflows-0.1.5/asyncflows/examples/get_page_title.yaml
+-rw-r--r--   0        0        0   294692 2024-05-25 22:40:56.345676 asyncflows-0.1.5/asyncflows/examples/hello_world.ipynb
+-rw-r--r--   0        0        0      651 2024-05-25 20:56:51.983126 asyncflows-0.1.5/asyncflows/examples/hello_world.py
+-rw-r--r--   0        0        0      327 2024-05-25 22:40:56.346635 asyncflows-0.1.5/asyncflows/examples/hello_world.yaml
+-rw-r--r--   0        0        0     1309 2024-05-25 22:40:56.347377 asyncflows-0.1.5/asyncflows/examples/rag.py
+-rw-r--r--   0        0        0     1137 2024-05-25 22:40:56.347667 asyncflows-0.1.5/asyncflows/examples/rag.yaml
+-rw-r--r--   0        0        0      280 2024-05-22 14:46:03.758066 asyncflows-0.1.5/asyncflows/examples/recipes/caprese.md
+-rw-r--r--   0        0        0      380 2024-05-22 14:46:03.758468 asyncflows-0.1.5/asyncflows/examples/recipes/chana_masala.md
+-rw-r--r--   0        0        0      329 2024-05-22 14:46:03.758593 asyncflows-0.1.5/asyncflows/examples/recipes/coconut_soup.md
+-rw-r--r--   0        0        0      413 2024-05-22 14:46:03.758715 asyncflows-0.1.5/asyncflows/examples/recipes/gazpacho.md
+-rw-r--r--   0        0        0      326 2024-05-22 14:46:03.758850 asyncflows-0.1.5/asyncflows/examples/recipes/guacamole.md
+-rw-r--r--   0        0        0      375 2024-05-22 14:46:03.758989 asyncflows-0.1.5/asyncflows/examples/recipes/hummus.md
+-rw-r--r--   0        0        0      326 2024-05-22 14:46:03.759115 asyncflows-0.1.5/asyncflows/examples/recipes/miso_soup.md
+-rw-r--r--   0        0        0      331 2024-05-22 14:46:03.759255 asyncflows-0.1.5/asyncflows/examples/recipes/omelette.md
+-rw-r--r--   0        0        0      327 2024-05-22 14:46:03.759525 asyncflows-0.1.5/asyncflows/examples/recipes/stir_fry.md
+-rw-r--r--   0        0        0      321 2024-05-22 14:46:03.759651 asyncflows-0.1.5/asyncflows/examples/recipes/yogurt_parfait.md
+-rw-r--r--   0        0        0     1105 2024-05-22 14:47:42.413403 asyncflows-0.1.5/asyncflows/examples/sql_rag.py
+-rw-r--r--   0        0        0     1606 2024-05-25 22:56:21.938495 asyncflows-0.1.5/asyncflows/examples/sql_rag.yaml
+-rw-r--r--   0        0        0     1198 2024-05-22 21:28:30.271238 asyncflows-0.1.5/asyncflows/examples/text_style_transfer.py
+-rw-r--r--   0        0        0      575 2024-05-25 22:40:56.348440 asyncflows-0.1.5/asyncflows/examples/text_style_transfer.yaml
+-rw-r--r--   0        0        0     1890 2024-05-22 14:46:03.761643 asyncflows-0.1.5/asyncflows/log_config.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.761683 asyncflows-0.1.5/asyncflows/models/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-22 14:46:03.761990 asyncflows-0.1.5/asyncflows/models/blob.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.762029 asyncflows-0.1.5/asyncflows/models/config/__init__.py
+-rw-r--r--   0        0        0     3960 2024-05-25 20:36:32.571870 asyncflows-0.1.5/asyncflows/models/config/action.py
+-rw-r--r--   0        0        0     2681 2024-05-22 14:46:03.762355 asyncflows-0.1.5/asyncflows/models/config/common.py
+-rw-r--r--   0        0        0     2208 2024-05-25 20:36:32.572264 asyncflows-0.1.5/asyncflows/models/config/flow.py
+-rw-r--r--   0        0        0     2491 2024-05-25 20:36:32.572548 asyncflows-0.1.5/asyncflows/models/config/model.py
+-rw-r--r--   0        0        0     5075 2024-05-22 14:49:41.999198 asyncflows-0.1.5/asyncflows/models/config/transform.py
+-rw-r--r--   0        0        0     5022 2024-05-22 14:49:22.058252 asyncflows-0.1.5/asyncflows/models/config/value_declarations.py
+-rw-r--r--   0        0        0     3303 2024-05-22 14:49:22.058580 asyncflows-0.1.5/asyncflows/models/file.py
+-rw-r--r--   0        0        0      700 2024-05-22 14:47:42.230677 asyncflows-0.1.5/asyncflows/models/primitives.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.763641 asyncflows-0.1.5/asyncflows/repos/__init__.py
+-rw-r--r--   0        0        0    20233 2024-05-22 14:46:03.764021 asyncflows-0.1.5/asyncflows/repos/blob_repo.py
+-rw-r--r--   0        0        0     4421 2024-05-22 14:46:03.764605 asyncflows-0.1.5/asyncflows/repos/cache_repo.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764679 asyncflows-0.1.5/asyncflows/scripts/__init__.py
+-rw-r--r--   0        0        0     4975 2024-05-23 10:43:58.865278 asyncflows-0.1.5/asyncflows/scripts/generate_config_schema.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764985 asyncflows-0.1.5/asyncflows/services/__init__.py
+-rw-r--r--   0        0        0    38941 2024-05-25 22:46:36.212742 asyncflows-0.1.5/asyncflows/services/action_service.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765630 asyncflows-0.1.5/asyncflows/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765743 asyncflows-0.1.5/asyncflows/tests/action_tests/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-25 22:56:21.938792 asyncflows-0.1.5/asyncflows/tests/action_tests/test_execute_db_statement.py
+-rw-r--r--   0        0        0     1260 2024-05-22 14:47:42.369030 asyncflows-0.1.5/asyncflows/tests/action_tests/test_extract_xml_tag.py
+-rw-r--r--   0        0        0      683 2024-05-22 14:48:15.166773 asyncflows-0.1.5/asyncflows/tests/action_tests/test_get_db_schema.py
+-rw-r--r--   0        0        0     7985 2024-05-25 22:40:56.350212 asyncflows-0.1.5/asyncflows/tests/action_tests/test_prompt.py
+-rw-r--r--   0        0        0     1902 2024-05-22 14:46:03.766510 asyncflows-0.1.5/asyncflows/tests/action_tests/test_transformers.py
+-rw-r--r--   0        0        0    11472 2024-05-25 22:40:56.350881 asyncflows-0.1.5/asyncflows/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.766988 asyncflows-0.1.5/asyncflows/tests/repos/__init__.py
+-rw-r--r--   0        0        0     8319 2024-05-22 14:46:03.767510 asyncflows-0.1.5/asyncflows/tests/repos/test_blob_repo.py
+-rw-r--r--   0        0        0     6567 2024-05-22 14:46:03.767743 asyncflows-0.1.5/asyncflows/tests/repos/test_cache_repo.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.767812 asyncflows-0.1.5/asyncflows/tests/resources/__init__.py
+-rw-r--r--   0        0        0     5737 2024-05-22 14:47:42.263059 asyncflows-0.1.5/asyncflows/tests/resources/actions.py
+-rw-r--r--   0        0        0      263 2024-05-25 22:40:56.351632 asyncflows-0.1.5/asyncflows/tests/resources/default_model_var.yaml
+-rw-r--r--   0        0        0     4079 2024-05-23 10:43:58.791187 asyncflows-0.1.5/asyncflows/tests/resources/testing_actions.yaml
+-rw-r--r--   0        0        0    26138 2024-05-25 22:32:38.860953 asyncflows-0.1.5/asyncflows/tests/test_action_service.py
+-rw-r--r--   0        0        0     6172 2024-05-25 22:40:56.352181 asyncflows-0.1.5/asyncflows/tests/test_async_utils.py
+-rw-r--r--   0        0        0     1069 2024-05-25 22:40:56.352473 asyncflows-0.1.5/asyncflows/tests/test_asyncflows_interface.py
+-rw-r--r--   0        0        0    11747 2024-05-22 18:55:04.928969 asyncflows-0.1.5/asyncflows/tests/test_config.py
+-rw-r--r--   0        0        0     2053 2024-05-22 14:48:15.167483 asyncflows-0.1.5/asyncflows/tests/test_run_examples.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.769749 asyncflows-0.1.5/asyncflows/utils/__init__.py
+-rw-r--r--   0        0        0     9877 2024-05-25 22:46:36.213306 asyncflows-0.1.5/asyncflows/utils/async_utils.py
+-rw-r--r--   0        0        0      676 2024-05-22 14:46:03.770301 asyncflows-0.1.5/asyncflows/utils/cache_utils.py
+-rw-r--r--   0        0        0     8602 2024-05-25 20:36:32.574834 asyncflows-0.1.5/asyncflows/utils/config_utils.py
+-rw-r--r--   0        0        0      725 2024-05-22 14:47:42.393837 asyncflows-0.1.5/asyncflows/utils/db_utils.py
+-rw-r--r--   0        0        0     1320 2024-05-22 14:46:03.771069 asyncflows-0.1.5/asyncflows/utils/jinja_utils.py
+-rw-r--r--   0        0        0     1482 2024-05-22 14:46:03.771192 asyncflows-0.1.5/asyncflows/utils/redis_utils.py
+-rw-r--r--   0        0        0     2686 2024-05-22 14:46:03.771325 asyncflows-0.1.5/asyncflows/utils/request_utils.py
+-rw-r--r--   0        0        0      382 2024-05-22 14:46:03.771449 asyncflows-0.1.5/asyncflows/utils/secret_utils.py
+-rw-r--r--   0        0        0      479 2024-05-22 14:46:03.771565 asyncflows-0.1.5/asyncflows/utils/sentinel_utils.py
+-rw-r--r--   0        0        0      451 2024-05-22 14:46:03.771681 asyncflows-0.1.5/asyncflows/utils/singleton_utils.py
+-rw-r--r--   0        0        0     3333 2024-05-22 14:47:42.303806 asyncflows-0.1.5/asyncflows/utils/transformers_utils.py
+-rw-r--r--   0        0        0     2507 2024-05-22 14:46:03.772050 asyncflows-0.1.5/asyncflows/utils/type_utils.py
+-rw-r--r--   0        0        0     2547 2024-05-25 22:56:21.947894 asyncflows-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    34917 1970-01-01 00:00:00.000000 asyncflows-0.1.5/PKG-INFO
```

### Comparing `asyncflows-0.1.4/LICENSE` & `asyncflows-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/README.md` & `asyncflows-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <div align="center">
 <h1>♾️ asyncflows 🌊</h1>
 
 [![Discord](https://img.shields.io/badge/discord-7289da)](https://discord.gg/AGZ6GrcJCh)
-[![Try in Colab](https://img.shields.io/badge/colab-red)](https://colab.research.google.com/github/asynchronous-flows/asyncflows/blob/main/examples/hello_world.ipynb)
+[![Try in Colab](https://img.shields.io/badge/colab-red)](https://colab.research.google.com/github/asynchronous-flows/asyncflows/blob/main/asyncflows/examples/hello_world.ipynb)
 
 Config-Driven Asynchronous AI Pipelines  
 Built with asyncio, pydantic, YAML, jinja  
 </div>
 
 
 **Table of Contents**
@@ -74,15 +74,15 @@
 
 ```bash
 python -m asyncflows.examples.hello_world
 ```
 
 Or:
 
-[![Try in Colab](https://img.shields.io/badge/Run_it_in_Google_Colab-red)](https://colab.research.google.com/github/asynchronous-flows/asyncflows/blob/main/examples/hello_world.ipynb)
+[![Try in Colab](https://img.shields.io/badge/Run_it_in_Google_Colab-red)](https://colab.research.google.com/github/asynchronous-flows/asyncflows/blob/main/asyncflows/examples/hello_world.ipynb)
 
 # Installation
 
 ## With pip
 
 Get started with:
 
@@ -667,15 +667,15 @@
     action: prompt
     prompt:
       - heading: SQL statement
         link: extract_sql_statement.result
       - text: |
           Here is the result of executing the SQL statement:
           ```
-          {{ exec.result }}
+          {{ exec.text }}
           ```
           Can you answer the user query based on this result?
       - heading: User query
         var: query
 
 default_output: answer_user_query.result
 ```
@@ -1000,15 +1000,15 @@
 ## Writing Flows with Autocomplete
 
 For an easier time writing flows, use YAML Language Server in your editor with our JsonSchema.
 
 Put the following at the top of your YAML flow config file:
 
 ```yaml
-# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/action_schema.json
+# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/asyncflows_schema.json
 ```
 
 The JsonSchema will only catch some errors, 
 stay tuned for a domain-specific language server that will provide more advanced features.
 
 ## Setting up Ollama for Local Inference
 
@@ -1081,15 +1081,15 @@
 ANTHROPIC_API_KEY=... python -m asyncflows.examples.hello_world
 ```
 
 </details>
 
 ## Prompting in-depth
 
-The `prompt` action constructs a prommpt from a list of text and variables, and sends it to the LLM.
+The `prompt` action constructs a prompt from a list of text and variables, and sends it to the LLM.
 
 The simplest prompt contains a single string:
 
 ```yaml
 my_prompt:
   action: prompt
   prompt: 
@@ -1115,31 +1115,31 @@
     - text: "What's your name?"
 my_prompt:
   action: prompt
   prompt: 
     - text: "Can you say hello to {{ name_prompt.result }}?"
 ```
 
-Often-times, the prompt is more complex, and includes multiple strings and variables in a multi-line string:
+Often-times, the prompt is more complex, and includes multiple variables in a multi-line string.
+
+The following two prompts are **equivalent**, but the second one uses syntactic sugar for referring to the `sample_text` variable:
 
 ```yaml
 my_prompt:
   action: prompt
   prompt: 
     - text: |
         A writing sample:
         ```
         {{ sample_text }}
         ```
 
         Write a story about {{ subject }} in the style of the sample.
 ```
 
-The following prompt is **equivalent** to the prompt above, but using syntactic sugar for referring to the `sample_text` variable:
-
 ```yaml
 my_prompt:
   action: prompt
   prompt: 
     - heading: A writing sample
       var: sample_text
     - text: Write a story about {{ subject }} in the style of the sample.
@@ -1172,15 +1172,15 @@
   prompt: 
     - heading: writing sample
       var: sample_text
     - text: |
         Write a story about {{ subject }} in the style of the sample, placing it between <story> and </story> tags.
 ```
 
-From this prompt, extract the story with the `extract_xml_tag` action:
+From this prompt's response, extract the story with the `extract_xml_tag` action:
 
 ```yaml
 extract_story:
   action: extract_xml_tag
   tag: story
   text:
     link: my_prompt.result
```

### Comparing `asyncflows-0.1.4/asyncflows/actions/__init__.py` & `asyncflows-0.1.5/asyncflows/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/actions/base.py` & `asyncflows-0.1.5/asyncflows/actions/base.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/actions/execute_db_statement.py` & `asyncflows-0.1.5/asyncflows/actions/execute_db_statement.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Any
+
+
 from asyncflows.actions.base import Action, BaseModel, Field
 from asyncflows.utils.db_utils import get_async_db_url
 
 
 class Inputs(BaseModel):
     database_url: str = Field(description="Database URL (asynchronous)")
     statement: str = Field(description="SQL statement to execute")
@@ -13,15 +16,17 @@
     max_rows: int = Field(
         default=5,
         description="Maximum number of rows to return",
     )
 
 
 class Outputs(BaseModel):
-    result: str = Field(description="Result of the SQL statement")
+    text: str = Field(description="Result of the SQL statement")
+    data: list[list[Any]]
+    headers: list[str]
 
 
 class ExecuteDBStatement(Action[Inputs, Outputs]):
     name = "execute_db_statement"
 
     async def run(self, inputs: Inputs) -> Outputs:
         from sqlalchemy import text
@@ -51,8 +56,16 @@
             result = await conn.execute(statement)
             rows = result.fetchall()[: inputs.max_rows]
             column_names = list(result.keys())
 
         df = pd.DataFrame(rows, columns=Index(column_names))
         result_str = df.to_string(index=False, justify="left")
 
-        return Outputs(result=result_str)
+        headers = list(df.columns)
+        data = df.values.tolist()
+        data = [[str(cell) for cell in row] for row in data]
+
+        return Outputs(
+            text=result_str,
+            data=data,
+            headers=headers,
+        )
```

### Comparing `asyncflows-0.1.4/asyncflows/actions/extract_list.py` & `asyncflows-0.1.5/asyncflows/actions/extract_list.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/actions/extract_pdf_text.py` & `asyncflows-0.1.5/asyncflows/actions/extract_pdf_text.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/actions/extract_xml_tag.py` & `asyncflows-0.1.5/asyncflows/actions/extract_xml_tag.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/actions/get_db_schema.py` & `asyncflows-0.1.5/asyncflows/actions/get_db_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,10 +29,13 @@
 
         create_statements = []
 
         for table_name in metadata.tables:
             table = metadata.tables[table_name]
             create_statements.append(str(CreateTable(table).compile(engine)))
 
+        if not create_statements:
+            self.log.warning("No tables found in the database")
+
         schema_text = "\n".join(create_statements)
 
         return Outputs(schema_text=schema_text)
```

### Comparing `asyncflows-0.1.4/asyncflows/actions/get_url.py` & `asyncflows-0.1.5/asyncflows/actions/get_url.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/actions/ocr.py` & `asyncflows-0.1.5/asyncflows/actions/ocr.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/actions/prompt.py` & `asyncflows-0.1.5/asyncflows/actions/prompt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import os
 import tempfile
 import base64
 from typing import Optional, AsyncIterator
 
 import aiohttp
@@ -252,23 +253,115 @@
             if model_config.temperature is not None
             else NOT_GIVEN,
             top_p=model_config.top_p if model_config.top_p is not None else NOT_GIVEN,
         ) as stream:
             async for completion in stream.text_stream:
                 yield completion
 
+    @tenacity.retry(
+        wait=tenacity.wait_exponential(multiplier=1, max=10),
+        stop=tenacity.stop_after_attempt(5),
+        retry=tenacity.retry_if_exception_type(aiohttp.ClientError),
+    )
+    async def _invoke_ollama(
+        self,
+        messages: list[dict[str, str]],
+        model_config: ModelConfig,
+    ):
+        api_base = (
+            model_config.api_base
+            or get_secret("OLLAMA_API_BASE")
+            or "http://localhost:11434"
+        )
+
+        api_url = os.path.join(
+            api_base,
+            "api",
+            "chat",
+        )
+
+        model_name = model_config.model.removeprefix("ollama/")
+
+        headers = {}
+        if model_config.auth_token is not None:
+            headers["Authorization"] = f"Bearer {model_config.auth_token}"
+
+        options = {}
+
+        if model_config.temperature is not None:
+            options["temperature"] = model_config.temperature
+        if model_config.max_output_tokens is not None:
+            options["num_predict"] = model_config.max_output_tokens
+
+        # TODO support the other optional parameters
+        # if model_config.top_p is not None:
+        #     options["top_p"] = model_config.top_p
+        # if model_config.frequency_penalty is not None:
+        #     options["frequency_penalty"] = model_config.frequency_penalty
+
+        data = {
+            "model": model_name,
+            "messages": messages,
+            "stream": True,
+            "options": options,
+        }
+
+        def process_completion(completion):
+            if not completion:
+                return None
+            try:
+                data = json.loads(completion)
+            except json.JSONDecodeError:
+                return None
+            if (
+                not isinstance(data, dict)
+                or "message" not in data
+                or not isinstance(data["message"], dict)
+                or "content" not in data["message"]
+            ):
+                return None
+            delta = data["message"]["content"]
+            if delta:
+                return delta
+
+        async with aiohttp.ClientSession() as session:
+            async with session.post(
+                api_url,
+                json=data,
+                headers=headers,
+            ) as response:
+                response.raise_for_status()
+
+                # can't use `response.json` cus of unexpected mimetype: application/x-ndjson
+                buffer = ""
+                async for completion in response.content.iter_any():
+                    buffer += completion.decode()
+                    while "\n" in buffer:
+                        json_, buffer = buffer.split("\n", 1)
+                        completion = process_completion(json_)
+                        if completion is not None:
+                            yield completion
+                if buffer:
+                    completion = process_completion(buffer)
+                    if completion is not None:
+                        yield completion
+
     async def _invoke_litellm(
         self,
         messages: list[dict[str, str]],
         model_config: ModelConfig,
     ):
         openai_api_key = get_secret("OPENAI_API_KEY")
         if openai_api_key is None and "gpt" in model_config.model:
             self.log.warning("OpenAI API key not set")
 
+        headers = {}
+        if model_config.auth_token is not None:
+            headers["Authorization"] = f"Bearer {model_config.auth_token}"
+
         client = None
         try:
             if "gpt" in model_config.model:
                 from openai import AsyncOpenAI
 
                 client = AsyncOpenAI(api_key=openai_api_key)
 
@@ -281,14 +374,15 @@
                     model=model_config.model,
                     temperature=model_config.temperature,
                     max_tokens=model_config.max_output_tokens,
                     top_p=model_config.top_p,
                     frequency_penalty=model_config.frequency_penalty,
                     presence_penalty=model_config.presence_penalty,
                     base_url=model_config.api_base,
+                    extra_headers=headers,
                     # **model_config.model_dump(),
                 ):
                     delta = completion.choices[0].delta.content  # type: ignore
                     if delta is None:
                         break
                     yield delta
         finally:
@@ -301,14 +395,19 @@
         model_config: ModelConfig,
     ) -> AsyncIterator[str]:
         if "claude" in model_config.model:
             iterator = self._invoke_anthropic(
                 messages=messages,
                 model_config=model_config,
             )
+        elif model_config.model.startswith("ollama/"):
+            iterator = self._invoke_ollama(
+                messages=messages,
+                model_config=model_config,
+            )
         else:
             iterator = self._invoke_litellm(
                 messages=messages,
                 model_config=model_config,
             )
 
         timer = Timer()
```

### Comparing `asyncflows-0.1.4/asyncflows/actions/score.py` & `asyncflows-0.1.5/asyncflows/actions/score.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/actions/transformer.py` & `asyncflows-0.1.5/asyncflows/actions/transformer.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/actions/utils/prompt_context.py` & `asyncflows-0.1.5/asyncflows/actions/utils/prompt_context.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/asyncflows.py` & `asyncflows-0.1.5/asyncflows/asyncflows.py`

 * *Files 12% similar despite different names*

```diff
@@ -113,7 +113,31 @@
             variables=self.variables,
         )
         context = {
             executable_id: outputs,
         }
 
         return await declaration.render(context)
+
+    async def stream(self, target_output: None | str = None):
+        if target_output is None:
+            target_output = self.action_config.default_output
+
+        declaration = VarDeclaration(
+            var=target_output,
+        )
+
+        dependencies = declaration.get_dependencies()
+        if len(dependencies) != 1:
+            raise NotImplementedError("Only one dependency is supported for now")
+        executable_id = list(dependencies)[0]
+
+        async for outputs in self.action_service.stream_executable(
+            self.log,
+            executable_id=executable_id,
+            variables=self.variables,
+        ):
+            context = {
+                executable_id: outputs,
+            }
+
+            yield await declaration.render(context)
```

### Comparing `asyncflows-0.1.4/asyncflows/examples/books/Alice's Adventures in Wonderland, by Lewis Carroll.pdf` & `asyncflows-0.1.5/asyncflows/examples/books/Alice's Adventures in Wonderland, by Lewis Carroll.pdf`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/examples/chatbot.py` & `asyncflows-0.1.5/asyncflows/examples/chatbot.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/examples/chatbot.yaml` & `asyncflows-0.1.5/asyncflows/examples/chatbot.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/action_schema.json
+# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/asyncflows_schema.json
 
 default_model:
   model: ollama/llama3
 flow:
   # Iterate over the PDF filepaths
   extract_pdf_texts:
     for: filepath
```

### Comparing `asyncflows-0.1.4/asyncflows/examples/debono.py` & `asyncflows-0.1.5/asyncflows/examples/debono.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/examples/debono.yaml` & `asyncflows-0.1.5/asyncflows/examples/debono.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/action_schema.json
+# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/asyncflows_schema.json
 
 default_model:
   model: ollama/llama3
   temperature: 1
   max_output_tokens: 2000
 # De Bono's Six Thinking Hats is a powerful technique for creative problem-solving and decision-making.
 flow:
```

### Comparing `asyncflows-0.1.4/asyncflows/examples/get_page_title.py` & `asyncflows-0.1.5/asyncflows/examples/get_page_title.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/examples/hello_world.ipynb` & `asyncflows-0.1.5/asyncflows/examples/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/examples/hello_world.py` & `asyncflows-0.1.5/asyncflows/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/examples/rag.py` & `asyncflows-0.1.5/asyncflows/examples/rag.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/examples/rag.yaml` & `asyncflows-0.1.5/asyncflows/examples/rag.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/action_schema.json
+# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/asyncflows_schema.json
 
 default_model:
   model: ollama/llama3
   temperature: 1
   max_output_tokens: 2000
 flow:
   # `retrieve` performs a vector search, fast for large datasets
```

### Comparing `asyncflows-0.1.4/asyncflows/examples/sql_rag.py` & `asyncflows-0.1.5/asyncflows/examples/sql_rag.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/examples/sql_rag.yaml` & `asyncflows-0.1.5/asyncflows/examples/sql_rag.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/action_schema.json
+# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/asyncflows_schema.json
 
 default_model:
   model: ollama/llama3
   temperature: 1
   max_output_tokens: 2000
 flow:
 
@@ -45,14 +45,14 @@
     action: prompt
     prompt:
       - heading: SQL statement
         link: extract_sql_statement.result
       - text: |
           Here is the result of executing the SQL statement:
           ```
-          {{ exec.result }}
+          {{ exec.text }}
           ```
           Can you answer the user query based on this result?
       - var: query
         heading: User query
 
 default_output: answer_user_query.result
```

### Comparing `asyncflows-0.1.4/asyncflows/examples/text_style_transfer.py` & `asyncflows-0.1.5/asyncflows/examples/text_style_transfer.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/examples/text_style_transfer.yaml` & `asyncflows-0.1.5/asyncflows/examples/text_style_transfer.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/action_schema.json
+# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/asyncflows_schema.json
 
 default_model:
   model: ollama/llama3
 
 flow:
   text_style_transfer:
     action: prompt
```

### Comparing `asyncflows-0.1.4/asyncflows/log_config.py` & `asyncflows-0.1.5/asyncflows/log_config.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/models/config/action.py` & `asyncflows-0.1.5/asyncflows/models/config/action.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,35 +33,40 @@
     )
 
 
 def build_hinted_value_declaration(
     vars_: HintType | None = None,
     links: HintType | None = None,
     strict: bool = False,
+    excluded_declaration_types: None | list[type[ValueDeclaration]] = None,
 ):
+    if excluded_declaration_types is None:
+        excluded_declaration_types = []
+
     union_elements = []
 
     if vars_:
         union_elements.append(
             VarDeclaration.from_vars(vars_, strict),
         )
-    if not vars_ or not strict:
+    if not vars_ or not strict and VarDeclaration not in excluded_declaration_types:
         union_elements.append(VarDeclaration)
 
     if links:
         union_elements.append(
             LinkDeclaration.from_vars(links, strict),
         )
-    if not links or not strict:
+    if not links or not strict and LinkDeclaration not in excluded_declaration_types:
         union_elements.append(LinkDeclaration)
 
     other_elements = [
         element
         for element in typing.get_args(ValueDeclaration)
         if element not in (VarDeclaration, LinkDeclaration)
+        and element not in excluded_declaration_types
     ]
     union_elements.extend(other_elements)
 
     return Union[tuple(union_elements)]  # type: ignore
 
 
 def build_actions(
```

### Comparing `asyncflows-0.1.4/asyncflows/models/config/common.py` & `asyncflows-0.1.5/asyncflows/models/config/common.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/models/config/flow.py` & `asyncflows-0.1.5/asyncflows/models/config/flow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from typing import Union
 
+import pydantic
 from pydantic import Field
 
 from asyncflows.models.config.action import (
     ActionInvocationUnion,
     TestingActionInvocationUnion,
 )
 from asyncflows.models.config.common import StrictModel
 from asyncflows.models.config.model import ModelConfig
 from asyncflows.models.config.value_declarations import ValueDeclaration
 from asyncflows.models.primitives import ContextVarName, ContextVarPath, ExecutableId
+from asyncflows.models.config.action import build_hinted_value_declaration
+from asyncflows.models.config.value_declarations import (
+    LinkDeclaration,
+    LambdaDeclaration,
+)
+from asyncflows.utils.config_utils import templatify_model
 
 
 class Loop(StrictModel):
     for_: ContextVarName = Field(
         ...,
         alias="for",
     )
@@ -24,16 +31,47 @@
     flow: "FlowConfig"
 
 
 class TestLoop(Loop):
     flow: "TestFlowConfig"
 
 
+def build_model_config(
+    strict: bool = False,
+):
+    # Dynamically build the model config like ActionModel, with the ValueDeclarations
+
+    HintedValueDeclaration = build_hinted_value_declaration(
+        strict=strict, excluded_declaration_types=[LinkDeclaration, LambdaDeclaration]
+    )
+
+    fields = templatify_model(
+        ModelConfig,
+        vars_=None,
+        links=None,
+        add_union=HintedValueDeclaration,  # type: ignore
+        strict=strict,
+    )
+
+    return pydantic.create_model(
+        "ModelConfigDeclaration",
+        __base__=ModelConfig,
+        __module__=__name__,
+        # model_config=ConfigDict(
+        #     arbitrary_types_allowed=True,
+        # ),
+        **fields,  # pyright: ignore[reportGeneralTypeIssues]
+    )
+
+
+ModelConfigDeclaration = build_model_config()
+
+
 class ActionConfig(StrictModel):
-    default_model: ModelConfig
+    default_model: ModelConfigDeclaration  # type: ignore
     action_timeout: float = 360
     flow: "FlowConfig"
     default_output: ContextVarPath
 
 
 class TestActionConfig(ActionConfig):
     flow: "TestFlowConfig"
```

### Comparing `asyncflows-0.1.4/asyncflows/models/config/model.py` & `asyncflows-0.1.5/asyncflows/models/config/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,37 +54,39 @@
         ],
         Doc("Anthropic model; requires `ANTHROPIC_API_KEY` environment variable"),
     ]
     | str
 )
 
 
+BiEncoderModelType = Literal[
+    "sentence-transformers/all-mpnet-base-v2",
+    "BAAI/bge-small-en-v1.5",
+]
+CrossEncoderModelType = Literal[
+    "cross-encoder/ms-marco-TinyBERT-L-2-v2",
+    "BAAI/bge-reranker-base",
+]
+
+
 class ModelConfig(StrictModel):
     max_output_tokens: int = 2000
     max_prompt_tokens: int = 8000
     temperature: float | None = None
     top_p: float | None = None
     frequency_penalty: float | None = None
     presence_penalty: float | None = None
-    model: ModelType = "gpt-3.5-turbo-1106"
+    model: ModelType = "ollama/llama3"
     api_base: Optional[str] = None
+    auth_token: Optional[str] = None
 
 
 class OptionalModelConfig(ModelConfig):
     max_output_tokens: Optional[int] = None
     max_prompt_tokens: Optional[int] = None
     temperature: Optional[float] = None
     top_p: Optional[float] = None
     frequency_penalty: Optional[float] = None
     presence_penalty: Optional[float] = None
     model: Optional[ModelType] = None
     api_base: Optional[str] = None
-
-
-BiEncoderModelType = Literal[
-    "sentence-transformers/all-mpnet-base-v2",
-    "BAAI/bge-small-en-v1.5",
-]
-CrossEncoderModelType = Literal[
-    "cross-encoder/ms-marco-TinyBERT-L-2-v2",
-    "BAAI/bge-reranker-base",
-]
+    auth_token: Optional[str] = None
```

### Comparing `asyncflows-0.1.4/asyncflows/models/config/transform.py` & `asyncflows-0.1.5/asyncflows/models/config/transform.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/models/config/value_declarations.py` & `asyncflows-0.1.5/asyncflows/models/config/value_declarations.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/models/file.py` & `asyncflows-0.1.5/asyncflows/models/file.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/models/primitives.py` & `asyncflows-0.1.5/asyncflows/models/primitives.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/repos/blob_repo.py` & `asyncflows-0.1.5/asyncflows/repos/blob_repo.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/repos/cache_repo.py` & `asyncflows-0.1.5/asyncflows/repos/cache_repo.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/scripts/generate_config_schema.py` & `asyncflows-0.1.5/asyncflows/scripts/generate_config_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         flow: HintedFlowConfig  # type: ignore
 
     # HintedLoop.model_rebuild()  # TODO is this necessary?
 
     return HintedActionConfig
 
 
-def _build_action_schema(
+def _build_asyncflows_schema(
     action_names: list[str],
     config_class: type[ActionConfig],
     strict: bool,
     config_filename: str | None = None,
 ):
     HintedActionConfig = build_hinted_flow_model(
         action_names=action_names,
@@ -133,22 +133,22 @@
         config_filename=config_filename,
         strict=strict,
     )
     workflow_schema = HintedActionConfig.model_json_schema()
     return workflow_schema
 
 
-def _build_and_save_action_schema(
+def _build_and_save_asyncflows_schema(
     action_names: list[str],
     config_class: type[ActionConfig],
     output_file: str,
     strict: bool,
     config_filename: str | None = None,
 ):
-    workflow_schema = _build_action_schema(
+    workflow_schema = _build_asyncflows_schema(
         action_names=action_names,
         config_class=config_class,
         strict=strict,
         config_filename=config_filename,
     )
     with open(os.path.join("schemas", output_file), "w") as f:
         json.dump(workflow_schema, f, indent=2)
@@ -161,30 +161,30 @@
         default="",
         help="Path to flow for populating link fields with",
     )
 
     args = parser.parse_args()
 
     if args.flow:
-        schema = _build_action_schema(
+        schema = _build_asyncflows_schema(
             action_names=_action_names,
             config_class=ActionConfig,
             config_filename=args.flow,
             strict=True,
         )
         # straight to stdout we go
         print(json.dumps(schema, indent=2))
     else:
         # build default action and test action schemas
-        _build_and_save_action_schema(
+        _build_and_save_asyncflows_schema(
             action_names=_action_names,
             config_class=ActionConfig,
-            output_file="action_schema.json",
+            output_file="asyncflows_schema.json",
             strict=False,
         )
 
-        _build_and_save_action_schema(
+        _build_and_save_asyncflows_schema(
             action_names=_testing_action_names,
             config_class=TestActionConfig,
-            output_file="testing_action_schema.json",
+            output_file="testing_asyncflows_schema.json",
             strict=False,
         )
```

### Comparing `asyncflows-0.1.4/asyncflows/services/action_service.py` & `asyncflows-0.1.5/asyncflows/services/action_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     BlobRepoInputs,
     DefaultModelInputs,
     RedisUrlInputs,
 )
 from asyncflows.models.blob import Blob
 from asyncflows.models.config.action import ActionInvocation
 from asyncflows.models.config.flow import ActionConfig, Loop, FlowConfig
+from asyncflows.models.config.model import ModelConfig
 from asyncflows.models.config.transform import TransformsInto
 from asyncflows.models.config.value_declarations import (
     TextDeclaration,
     ValueDeclaration,
 )
 from asyncflows.models.primitives import ExecutableName, ExecutableId, TaskId
 
@@ -102,22 +103,30 @@
 
     async def _run_action(
         self,
         log: structlog.stdlib.BoundLogger,
         action_id: ExecutableId,
         inputs: Inputs | None,
         flow: FlowConfig,
+        variables: dict[str, Any],
     ) -> AsyncIterator[Outputs | None]:
         # Prepare inputs
         if isinstance(inputs, RedisUrlInputs):
             inputs._redis_url = get_redis_url()
         if isinstance(inputs, BlobRepoInputs):
             inputs._blob_repo = self.blob_repo
         if isinstance(inputs, DefaultModelInputs):
-            inputs._default_model = self.config.default_model
+            # default_model is a special case,
+            # allows ValueDeclaration union except for links and lambdas
+            model_config_dict = await self._collect_inputs_from_context(
+                log,
+                self.config.default_model,
+                variables,
+            )
+            inputs._default_model = ModelConfig.model_validate(model_config_dict)
 
         # Get the action instance
         action = self._get_action_instance(log, action_id, flow=flow)
         if not isinstance(inputs, action._get_inputs_type()):
             raise ValueError(
                 f"Inputs type mismatch: {type(inputs)} != {action._get_inputs_type()}"
             )
@@ -349,18 +358,19 @@
                 log,
                 input_spec=input_spec,
                 context=variables,
             )
             try:
                 yield inputs_type.model_validate(rendered)
             except Exception as e:
+                tb = traceback.format_exception(type(e), e, e.__traceback__)
                 log.exception(
                     "Invalid inputs",
-                    exc_info=True,
                     inputs_dict=rendered,
+                    traceback="".join(tb),
                 )
                 sentry_sdk.capture_exception(e)
             return
 
         async for dependency_outputs in self.stream_dependencies(
             log,
             dependencies,
@@ -378,18 +388,19 @@
                 log,
                 input_spec=input_spec,
                 context=context,
             )
             try:
                 yield inputs_type.model_validate(inputs_dict)
             except Exception as e:
+                tb = traceback.format_exception(type(e), e, e.__traceback__)
                 log.exception(
                     "Invalid inputs",
-                    exc_info=True,
                     inputs_dict=inputs_dict,
+                    traceback="".join(tb),
                 )
                 sentry_sdk.capture_exception(e)
 
     async def stream_executable_tasks(
         self,
         log: structlog.stdlib.BoundLogger,
         dependencies: set[tuple[ExecutableId, bool]] | set[ExecutableId],
@@ -670,14 +681,15 @@
 
             # TODO rework this to handle partial outputs, not just full output objects
             async for outputs in self._run_action(
                 log=log,
                 action_id=action_id,
                 inputs=inputs,
                 flow=flow,
+                variables=variables,
             ):
                 # TODO are there any race conditions here, between result caching and in-progress action awaiting?
                 #  also consider paradigm of multiple workers, indexing tasks in a database and pulling from cache instead
 
                 # Send result to queue
                 # log.debug("Broadcasting outputs")
                 self._broadcast_outputs(log, task_id, outputs)
@@ -691,14 +703,15 @@
             log.info("Running action with final invocation flag")
             inputs._finished = True
             async for outputs in self._run_action(
                 log=log,
                 action_id=task_id,
                 inputs=inputs,
                 flow=flow,
+                variables=variables,
             ):
                 self._broadcast_outputs(log, task_id, outputs)
 
         # Cache result
         # TODO should we cache intermediate results too, or only on the final set of inputs/outputs?
         # TODO we shouldn't cache if all we did was pull from cache
         if (
```

### Comparing `asyncflows-0.1.4/asyncflows/tests/action_tests/test_extract_xml_tag.py` & `asyncflows-0.1.5/asyncflows/tests/action_tests/test_extract_xml_tag.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/action_tests/test_get_db_schema.py` & `asyncflows-0.1.5/asyncflows/tests/action_tests/test_get_db_schema.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/action_tests/test_prompt.py` & `asyncflows-0.1.5/asyncflows/tests/action_tests/test_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,17 @@
     inputs = Inputs(
         prompt=[
             TextElement(
                 text="This is the prompt.",
             )
         ],
     )
-    inputs._default_model = ModelConfig()
+    inputs._default_model = ModelConfig(
+        model="gpt-3.5-turbo",
+    )
     async for outputs in action.run(inputs):
         result = outputs.result
         assert expected_response.startswith(result)
 
     assert result == expected_response
```

### Comparing `asyncflows-0.1.4/asyncflows/tests/action_tests/test_transformers.py` & `asyncflows-0.1.5/asyncflows/tests/action_tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/conftest.py` & `asyncflows-0.1.5/asyncflows/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/repos/test_blob_repo.py` & `asyncflows-0.1.5/asyncflows/tests/repos/test_blob_repo.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/repos/test_cache_repo.py` & `asyncflows-0.1.5/asyncflows/tests/repos/test_cache_repo.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/resources/actions.py` & `asyncflows-0.1.5/asyncflows/tests/resources/actions.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/resources/testing_actions.yaml` & `asyncflows-0.1.5/asyncflows/tests/resources/testing_actions.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# yaml-language-server: $schema=../../../../schemas/testing_action_schema.json
+# yaml-language-server: $schema=../../../../schemas/testing_asyncflows_schema.json
 
 default_model:
   model: gpt-3.5-turbo-1106
 action_timeout: 5
 flow:
   first_sum:
     action: test_add
```

### Comparing `asyncflows-0.1.4/asyncflows/tests/test_action_service.py` & `asyncflows-0.1.5/asyncflows/tests/test_action_service.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/test_async_utils.py` & `asyncflows-0.1.5/asyncflows/tests/test_async_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/test_config.py` & `asyncflows-0.1.5/asyncflows/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/tests/test_run_examples.py` & `asyncflows-0.1.5/asyncflows/tests/test_run_examples.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/utils/async_utils.py` & `asyncflows-0.1.5/asyncflows/utils/async_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,15 @@
     log: structlog.stdlib.BoundLogger,
     f: Awaitable[T],
     timer: Timer,
     timeout: int = 180,
 ) -> T:
     coro_wrapper = f.__await__()
     arg = None
+    exc = None
     fut = None
     first_run = True
 
     while True:
         try:
             if first_run:
                 first_run = False
@@ -199,19 +200,23 @@
                         # exc_info=e,
                     )
                     # fut.set_exception(e)
                 except Exception as e:
                     log.warning(
                         "Subcoroutine raised exception",
                         arg=arg,
-                        exc_info=e,
+                        # exc_info=e,
                     )
-                    coro_wrapper.throw(e)
+                    exc = e
             timer.start()
-            fut = coro_wrapper.send(arg)
+            if exc is not None:
+                fut = coro_wrapper.throw(exc)
+                exc = None
+            else:
+                fut = coro_wrapper.send(arg)
         except StopIteration as e:
             return e.value
         finally:
             timer.end()
             arg = None
```

### Comparing `asyncflows-0.1.4/asyncflows/utils/cache_utils.py` & `asyncflows-0.1.5/asyncflows/utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/utils/config_utils.py` & `asyncflows-0.1.5/asyncflows/utils/config_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             type_ = Union[type_, None]
 
         # Annotate optional fields with a default of None
         kwargs = {}
         if not field_.is_required() or (
             add_union is not None and isinstance(None, add_union)
         ):
-            kwargs["default"] = None
+            kwargs["default"] = field_.default
         if field_.alias is not None:
             kwargs["alias"] = field_.alias
         # else:
         #     default = ...
         if not kwargs:
             template_field = ...
         else:
```

### Comparing `asyncflows-0.1.4/asyncflows/utils/db_utils.py` & `asyncflows-0.1.5/asyncflows/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/utils/jinja_utils.py` & `asyncflows-0.1.5/asyncflows/utils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/utils/redis_utils.py` & `asyncflows-0.1.5/asyncflows/utils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/utils/request_utils.py` & `asyncflows-0.1.5/asyncflows/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/utils/transformers_utils.py` & `asyncflows-0.1.5/asyncflows/utils/transformers_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/asyncflows/utils/type_utils.py` & `asyncflows-0.1.5/asyncflows/utils/type_utils.py`

 * *Files identical despite different names*

### Comparing `asyncflows-0.1.4/pyproject.toml` & `asyncflows-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncflows"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Rafael Irgolic <hello@irgolic.com>"]
 readme = "README.md"
 license = "BSL-1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
```

### Comparing `asyncflows-0.1.4/PKG-INFO` & `asyncflows-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncflows
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: BSL-1.1
 Author: Rafael Irgolic
 Author-email: hello@irgolic.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -48,15 +48,15 @@
 Requires-Dist: types-aioboto3[s3] (>=12.2.0,<13.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 <h1>♾️ asyncflows 🌊</h1>
 
 [![Discord](https://img.shields.io/badge/discord-7289da)](https://discord.gg/AGZ6GrcJCh)
-[![Try in Colab](https://img.shields.io/badge/colab-red)](https://colab.research.google.com/github/asynchronous-flows/asyncflows/blob/main/examples/hello_world.ipynb)
+[![Try in Colab](https://img.shields.io/badge/colab-red)](https://colab.research.google.com/github/asynchronous-flows/asyncflows/blob/main/asyncflows/examples/hello_world.ipynb)
 
 Config-Driven Asynchronous AI Pipelines  
 Built with asyncio, pydantic, YAML, jinja  
 </div>
 
 
 **Table of Contents**
@@ -124,15 +124,15 @@
 
 ```bash
 python -m asyncflows.examples.hello_world
 ```
 
 Or:
 
-[![Try in Colab](https://img.shields.io/badge/Run_it_in_Google_Colab-red)](https://colab.research.google.com/github/asynchronous-flows/asyncflows/blob/main/examples/hello_world.ipynb)
+[![Try in Colab](https://img.shields.io/badge/Run_it_in_Google_Colab-red)](https://colab.research.google.com/github/asynchronous-flows/asyncflows/blob/main/asyncflows/examples/hello_world.ipynb)
 
 # Installation
 
 ## With pip
 
 Get started with:
 
@@ -717,15 +717,15 @@
     action: prompt
     prompt:
       - heading: SQL statement
         link: extract_sql_statement.result
       - text: |
           Here is the result of executing the SQL statement:
           ```
-          {{ exec.result }}
+          {{ exec.text }}
           ```
           Can you answer the user query based on this result?
       - heading: User query
         var: query
 
 default_output: answer_user_query.result
 ```
@@ -1050,15 +1050,15 @@
 ## Writing Flows with Autocomplete
 
 For an easier time writing flows, use YAML Language Server in your editor with our JsonSchema.
 
 Put the following at the top of your YAML flow config file:
 
 ```yaml
-# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/action_schema.json
+# yaml-language-server: $schema=https://raw.githubusercontent.com/asynchronous-flows/asyncflows/main/schemas/asyncflows_schema.json
 ```
 
 The JsonSchema will only catch some errors, 
 stay tuned for a domain-specific language server that will provide more advanced features.
 
 ## Setting up Ollama for Local Inference
 
@@ -1131,15 +1131,15 @@
 ANTHROPIC_API_KEY=... python -m asyncflows.examples.hello_world
 ```
 
 </details>
 
 ## Prompting in-depth
 
-The `prompt` action constructs a prommpt from a list of text and variables, and sends it to the LLM.
+The `prompt` action constructs a prompt from a list of text and variables, and sends it to the LLM.
 
 The simplest prompt contains a single string:
 
 ```yaml
 my_prompt:
   action: prompt
   prompt: 
@@ -1165,31 +1165,31 @@
     - text: "What's your name?"
 my_prompt:
   action: prompt
   prompt: 
     - text: "Can you say hello to {{ name_prompt.result }}?"
 ```
 
-Often-times, the prompt is more complex, and includes multiple strings and variables in a multi-line string:
+Often-times, the prompt is more complex, and includes multiple variables in a multi-line string.
+
+The following two prompts are **equivalent**, but the second one uses syntactic sugar for referring to the `sample_text` variable:
 
 ```yaml
 my_prompt:
   action: prompt
   prompt: 
     - text: |
         A writing sample:
         ```
         {{ sample_text }}
         ```
 
         Write a story about {{ subject }} in the style of the sample.
 ```
 
-The following prompt is **equivalent** to the prompt above, but using syntactic sugar for referring to the `sample_text` variable:
-
 ```yaml
 my_prompt:
   action: prompt
   prompt: 
     - heading: A writing sample
       var: sample_text
     - text: Write a story about {{ subject }} in the style of the sample.
@@ -1222,15 +1222,15 @@
   prompt: 
     - heading: writing sample
       var: sample_text
     - text: |
         Write a story about {{ subject }} in the style of the sample, placing it between <story> and </story> tags.
 ```
 
-From this prompt, extract the story with the `extract_xml_tag` action:
+From this prompt's response, extract the story with the `extract_xml_tag` action:
 
 ```yaml
 extract_story:
   action: extract_xml_tag
   tag: story
   text:
     link: my_prompt.result
```

